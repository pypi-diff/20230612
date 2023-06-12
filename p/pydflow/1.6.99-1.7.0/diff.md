# Comparing `tmp/pydflow-1.6.99.tar.gz` & `tmp/pydflow-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydflow-1.6.99.tar", last modified: Tue Mar 28 10:11:02 2023, max compression
+gzip compressed data, was "pydflow-1.7.0.tar", last modified: Mon Jun 12 13:04:19 2023, max compression
```

## Comparing `pydflow-1.6.99.tar` & `pydflow-1.7.0.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.899428 pydflow-1.6.99/
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-03-28 10:10:52.000000 pydflow-1.6.99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36305 2023-03-28 10:11:02.899428 pydflow-1.6.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35995 2023-03-28 10:10:52.000000 pydflow-1.6.99/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 10:11:02.899428 pydflow-1.6.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-28 10:10:52.000000 pydflow-1.6.99/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.891428 pydflow-1.6.99/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.895428 pydflow-1.6.99/src/dflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/argo_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.895428 pydflow-1.6.99/src/dflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/client/v1alpha1_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/client/v1alpha1_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/client/v1alpha1_retry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/client/v1alpha1_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/client/v1alpha1_value_from.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/context_syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    48414 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    21452 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/op_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.895428 pydflow-1.6.99/src/dflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/bohrium.py
--rw-r--r--   0 runner    (1001) docker     (123)    20216 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/lebesgue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/oss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/plugins/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.895428 pydflow-1.6.99/src/dflow/python/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/python/op.py
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/python/opio.py
--rw-r--r--   0 runner    (1001) docker     (123)    29578 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/python/python_op_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/python/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    96089 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/util_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    26096 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42148 2023-03-28 10:10:52.000000 pydflow-1.6.99/src/dflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.895428 pydflow-1.6.99/src/pydflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36305 2023-03-28 10:11:02.000000 pydflow-1.6.99/src/pydflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-28 10:11:02.000000 pydflow-1.6.99/src/pydflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 10:11:02.000000 pydflow-1.6.99/src/pydflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-28 10:11:02.000000 pydflow-1.6.99/src/pydflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-28 10:11:02.000000 pydflow-1.6.99/src/pydflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-28 10:11:02.000000 pydflow-1.6.99/src/pydflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:11:02.899428 pydflow-1.6.99/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_big_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_conditional_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_group_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_makevasp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_recurse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_reuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-28 10:10:52.000000 pydflow-1.6.99/tests/test_subpath_slices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:04:19.555189 pydflow-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-12 13:04:04.000000 pydflow-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 13:04:04.000000 pydflow-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-12 13:04:19.555189 pydflow-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32758 2023-06-12 13:04:04.000000 pydflow-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 13:04:04.000000 pydflow-1.7.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:04:19.555189 pydflow-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-12 13:04:04.000000 pydflow-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:04:19.543189 pydflow-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:04:19.547189 pydflow-1.7.0/src/dflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/argo_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:04:19.547189 pydflow-1.7.0/src/dflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/client/v1alpha1_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/client/v1alpha1_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/client/v1alpha1_retry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/client/v1alpha1_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/client/v1alpha1_value_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/context_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51335 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/op_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:04:19.551189 pydflow-1.7.0/src/dflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/plugins/bohrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/plugins/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23061 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/plugins/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/plugins/launching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/plugins/lebesgue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/plugins/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/plugins/oss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/plugins/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:04:19.551189 pydflow-1.7.0/src/dflow/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/python/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/python/opio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31692 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/python/python_op_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/python/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102205 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/util_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45085 2023-06-12 13:04:04.000000 pydflow-1.7.0/src/dflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:04:19.555189 pydflow-1.7.0/src/pydflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-12 13:04:19.000000 pydflow-1.7.0/src/pydflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-12 13:04:19.000000 pydflow-1.7.0/src/pydflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:04:19.000000 pydflow-1.7.0/src/pydflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 13:04:19.000000 pydflow-1.7.0/src/pydflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-12 13:04:19.000000 pydflow-1.7.0/src/pydflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 13:04:19.000000 pydflow-1.7.0/src/pydflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:04:19.555189 pydflow-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-12 13:04:04.000000 pydflow-1.7.0/tests/test_big_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-12 13:04:04.000000 pydflow-1.7.0/tests/test_conditional_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-12 13:04:04.000000 pydflow-1.7.0/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-12 13:04:04.000000 pydflow-1.7.0/tests/test_group_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-06-12 13:04:04.000000 pydflow-1.7.0/tests/test_makevasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-12 13:04:04.000000 pydflow-1.7.0/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-12 13:04:04.000000 pydflow-1.7.0/tests/test_recurse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-12 13:04:04.000000 pydflow-1.7.0/tests/test_reuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-12 13:04:04.000000 pydflow-1.7.0/tests/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-12 13:04:04.000000 pydflow-1.7.0/tests/test_subpath_slices.py
```

### Comparing `pydflow-1.6.99/LICENSE` & `pydflow-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/PKG-INFO` & `pydflow-1.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,191 +1,96 @@
-Metadata-Version: 2.1
-Name: pydflow
-Version: 1.6.99
-Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
-Author: Xinzijian Liu
-License: LGPLv3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DFLOW
 
 [Dflow](https://deepmodeling.com/dflow/dflow.html) is a Python framework for constructing scientific computing workflows (e.g. concurrent learning workflows) employing [Argo Workflows](https://argoproj.github.io/) as the workflow engine.
 
 For dflow's users (e.g. ML application developers), dflow offers user-friendly functional programming interfaces for building their own workflows. Users need not be concerned with process control, task scheduling, observability and disaster tolerance. Users can track workflow status and handle exceptions by APIs as well as from frontend UI. Thereby users are enabled to concentrate on implementing operations (OPs) and orchestrating workflows.
 
-For dflow's developers, dflow wraps on argo SDK, keeps details of computing and storage resources from users, and provides extension abilities. While argo is a cloud-native workflow engine, dflow uses containers to decouple computing logic and scheduling logic, and uses Kubernetes to make workflows observable, reproducible and robust. Dflow is designed to be based on a distributed, heterogeneous infrastructure. The most common computing resources in scientific computing may be HPC clusters. User can either use executor to manage HPC jobs within dflow ([dflow-extender](https://github.com/dptech-corp/dflow-extender)) or using [DPDispatcher](https://github.com/deepmodeling/dpdispatcher) plugin, or use virtual node technique to uniformly manage HPC resources in the framework of Kubernetes ([wlm-operator](https://github.com/dptech-corp/wlm-operator)).
+For dflow's developers, dflow wraps on argo SDK, keeps details of computing and storage resources from users, and provides extension abilities. While argo is a cloud-native workflow engine, dflow uses containers to decouple computing logic and scheduling logic, and uses Kubernetes to make workflows observable, reproducible and robust. Dflow is designed to be based on a distributed, heterogeneous infrastructure. The most common computing resources in scientific computing may be HPC clusters. User can either use executor to manage HPC jobs using [DPDispatcher](https://github.com/deepmodeling/dpdispatcher) plugin, or use virtual node technique to uniformly manage HPC resources in the framework of Kubernetes ([wlm-operator](https://github.com/dptech-corp/wlm-operator)).
 
-Dflow's OPs can be reused among workflows and shared among users. Dflow provides a cookie cutter recipe [dflow-op-cutter](https://github.com/deepmodeling/dflow-op-cutter) for template a new OP package. Start developing an OP package at once from
+OP template (abbr. OP) in dflow can be reused among workflows and shared among users. Dflow provides a cookie cutter recipe [dflow-op-cutter](https://github.com/deepmodeling/dflow-op-cutter) for template a new OP package. Start developing an OP package at once from
 ```python
 pip install cookiecutter
 cookiecutter https://github.com/deepmodeling/dflow-op-cutter.git
 ```
 
 Dflow provides a debug mode for running workflows bare-metally whose backend is implemented in dflow in pure Python, independent of Argo/Kubernetes. The debug mode uses local environment to execute OPs instead of containers. It implements most APIs of the default mode in order to provide an identical user experience. The debug mode offer convenience for debugging or testing without container. For the clusters having problem deploying docker and Kubernetes and difficult to access from outside, the debug mode may also be used for production, despite less robustness and observability.
 
 <!-- vscode-markdown-toc -->
 * 1. [ Overview](#Overview)
 	* 1.1. [ Architecture](#Architecture)
-	* 1.2. [ Common layer](#Commonlayer)
+	* 1.2. [ Basics](#Basics)
 		* 1.2.1. [ Parameters and artifacts](#Parametersandartifacts)
 		* 1.2.2. [ OP template](#OPtemplate)
 		* 1.2.3. [ Step](#Step)
 		* 1.2.4. [ Workflow](#Workflow)
-	* 1.3. [ Interface layer](#Interfacelayer)
-		* 1.3.1. [ Python OP](#PythonOP)
 * 2. [ Quick Start](#QuickStart)
-	* 2.1. [ Prepare Kubernetes cluster](#PrepareKubernetescluster)
-	* 2.2. [ Setup Argo Workflows](#SetupArgoWorkflows)
-	* 2.3. [ Install dflow](#Installdflow)
-	* 2.4. [ Run an example](#Runanexample)
-* 3. [ User Guide (dflow-doc)](#UserGuide)
-	* 3.1. [ Common layer](#Commonlayer-1)
+	* 2.1. [ Setup Argo Server](#SetupArgoServer)
+	* 2.2. [ Install dflow](#Installdflow)
+	* 2.3. [ Run an example](#Runanexample)
+* 3. [ User Guide](#UserGuide)
+	* 3.1. [ Common layer](#Commonlayer)
 		* 3.1.1. [ Workflow management](#Workflowmanagement)
 		* 3.1.2. [ Upload/download artifact](#Uploaddownloadartifact)
 		* 3.1.3. [ Steps](#Steps)
 		* 3.1.4. [ DAG](#DAG)
-		* 3.1.5. [ Output parameters and artifacts of Steps](#OutputparametersandartifactsofSteps)
-		* 3.1.6. [ Conditional step, parameters and artifacts](#Conditionalstepparametersandartifacts)
-		* 3.1.7. [ Produce parallel steps using loop](#Produceparallelstepsusingloop)
-		* 3.1.8. [ Timeout](#Timeout)
-		* 3.1.9. [ Continue on failed](#Continueonfailed)
-		* 3.1.10. [ Continue on success number/ratio of parallel steps](#Continueonsuccessnumberratioofparallelsteps)
-		* 3.1.11. [ Optional input artifacts](#Optionalinputartifacts)
-		* 3.1.12. [ Default value for output parameters](#Defaultvalueforoutputparameters)
-		* 3.1.13. [ Key of a step](#Keyofastep)
-		* 3.1.14. [ Resubmit a workflow](#Resubmitaworkflow)
-		* 3.1.15. [ Executor](#Executor)
-		* 3.1.16. [ Submit Slurm job via slurm executor](#SubmitSlurmjobviaslurmexecutor)
-		* 3.1.17. [ Submit HPC job via dispatcher plugin](#SubmitHPCjobviadispatcherplugin)
-		* 3.1.18. [ Submit Slurm job via virtual node](#SubmitSlurmjobviavirtualnode)
-		* 3.1.19. [ Use resources in Kubernetes](#UseresourcesinKubernetes)
-		* 3.1.20. [ Important note: variable names](#Importantnotevariablenames)
-        * 3.1.21. [ Debug mode: dflow independent of Kubernetes](#DebugmodeDflowindependentofKubernetes)
-	* 3.2. [ Interface layer](#Interfacelayer-1)
+		* 3.1.5. [ Conditional step, parameters and artifacts](#Conditionalstepparametersandartifacts)
+		* 3.1.6. [ Produce parallel steps using loop](#Produceparallelstepsusingloop)
+		* 3.1.7. [ Timeout](#Timeout)
+		* 3.1.8. [ Continue on failed](#Continueonfailed)
+		* 3.1.9. [ Continue on success number/ratio of parallel steps](#Continueonsuccessnumberratioofparallelsteps)
+		* 3.1.10. [ Optional input artifacts](#Optionalinputartifacts)
+		* 3.1.11. [ Default value for output parameters](#Defaultvalueforoutputparameters)
+		* 3.1.12. [ Key of a step](#Keyofastep)
+		* 3.1.13. [ Resubmit a workflow](#Resubmitaworkflow)
+		* 3.1.14. [ Executor](#Executor)
+		* 3.1.15. [ Submit HPC/Bohrium job via dispatcher plugin](#SubmitHPCBohriumjobviadispatcherplugin)
+		* 3.1.16. [ Submit Slurm job via virtual node](#SubmitSlurmjobviavirtualnode)
+		* 3.1.17. [ Use resources in Kubernetes](#UseresourcesinKubernetes)
+		* 3.1.18. [ Important note: variable names](#Importantnotevariablenames)
+		* 3.1.19. [ Debug mode: dflow independent of Kubernetes](#DebugmodedflowindependentofKubernetes)
+		* 3.1.20. [Artifact storage plugins](#Artifactstorageplugins)
+	* 3.2. [ Interface layer](#Interfacelayer)
 		* 3.2.1. [ Slices](#Slices)
 		* 3.2.2. [ Retry and error handling](#Retryanderrorhandling)
 		* 3.2.3. [ Progress](#Progress)
 		* 3.2.4. [ Upload python packages for development](#Uploadpythonpackagesfordevelopment)
 
 <!-- vscode-markdown-toc-config
 	numbering=true
 	autoSave=true
 	/vscode-markdown-toc-config -->
 <!-- /vscode-markdown-toc -->
 
 ##  1. <a name='Overview'></a> Overview
 ###  1.1. <a name='Architecture'></a> Architecture
-The dflow consists of a **common layer** and an **interface layer**.  Interface layer takes various OP templates from users, usually in the form of python classes, and transforms them into base OP templates that common layer can handle.
+The dflow consists of a **common layer** and an **interface layer**.  Interface layer takes various OP templates from users, usually in the form of python classes or functions, and transforms them into base OP templates that common layer can handle.
 
 <p align="center">
 <img src="./docs/imgs/dflow_architecture.png" alt="dflow_architecture" width="400"/>
 </p>
 <!-- <style>
 img {
   display: block;
   margin-left: auto;
   margin-right: auto;
 }
 </style> -->
 
-###  1.2. <a name='Commonlayer'></a> Common layer
-Common layer is an extension over argo client which provides functionalities such as file processing, computing resources management, workflow submission and management, etc.
+###  1.2. <a name='Basics'></a> Basics
+
 ####  1.2.1. <a name='Parametersandartifacts'></a> Parameters and artifacts
-Parameters and artifacts are data stored by the workflow and passed within the workflow. Parameters are saved as strings which can be displayed in the UI, while artifacts are saved as files.
+Parameters and artifacts are data stored by the workflow and passed within the workflow. Parameters are saved as text which can be displayed in the UI, while artifacts are saved as files. Parameters are passed to an OP with their values, while artifacts are passed as paths.
 
 ####  1.2.2. <a name='OPtemplate'></a> OP template
-OP template (shown as base OP in the figure above) is the fundamental building block of a workflow. It defines an operation to be executed given the input and output. Both the input and output can be parameters and/or artifacts. The most common OP template is the container OP template. Necessary arguments to be defined for the operation are the container image and scripts to be executed. Currently, two types of container OP templates are supported: `ShellOPTemplate`, `PythonScriptOPTemplate`. Shell OP template (`ShellOPTemplate`) defines an operation by a shell script and Python script OP template (`PythonScriptOPTemplate`) defines an operation by a Python script.
-
-To use the `ShellOPTemplate`:
-
-```python
-from dflow import ShellOPTemplate
-
-simple_example_templ = ShellOPTemplate(
-    name="Hello",
-    image="alpine:latest",
-    script="cp /tmp/foo.txt /tmp/bar.txt && echo {{inputs.parameters.msg}} > /tmp/msg.txt",
-)
-```
-The above example defines a `ShellOPTemplate` with `name = "Hello"` and container image `alpine:latest`. The operation is to copy `/tmp/foo.txt` (input artifacts) to `/tmp/bar.txt` (output artifacts) and printout the properties of the parameters with name `msg` (input parameters) and redirect it to `/tmp/msg.txt` (value in the file is the properties of the output parameters). 
-<!-- 
-Parameters and artifacts can be defined as the following:
-- Input/output parameters: a dictionary that maps the parameter name to its properties.
-- Input/output artifacts: a dictionary that maps the artifact name to its properties. -->
-
-To define the parameters and artifacts of this OPTemplate: 
-
-```python
-from dflow import InputParameter, InputArtifact, OutputParameter, OutputArtifact
-
-# define input
-simple_example_templ.inputs.parameters = {"msg": InputParameter()}
-simple_example_templ.inputs.artifacts = {"inp_art": InputArtifact(path="/tmp/foo.txt")}
-# define output
-simple_example_templ.outputs.parameters = {
-    "msg": OutputParameter(value_from_path="/tmp/msg.txt")
-}
-simple_example_templ.outputs.artifacts = {
-    "out_art": OutputArtifact(path="/tmp/bar.txt")
-}
-```
-
-In the above example, there are three things to clarify. 
-1. The value of the input parameter is optional for the OP template, if provided, it will be regarded as the default value which can be overridden at run time. 
-2. For the output parameter, the source where its value comes from should be specified. For the container OP template, the value may come from a certain file generated in the container (`value_from_path`). 
-3. The paths to the input and output artifact in the container are required to be specified.
-
-On the same level, one can also define a `PythonScriptOPTemplate` to achieve the same operation. 
-
-####  1.2.3. <a name='Step'></a> Step
-`Step` is the central block for building a workflow. A `step` is created by instantiating an OP template. When a `step` is initialized, values of all input parameters and sources of all input artifacts declared in the OP template must be specified.
-<!-- `Steps` is a sequential array of concurrent `Step`'s. A simple example goes like `[[s00, s01],  [s10, s11, s12]]`, where inner array represent concurrent tasks while outer array is sequential. (this part can be put in the User Guide-->
-```python
-from dflow import Step
-
-simple_example_step = Step(
-    name="step0",
-    template=simple_example_templ,
-    parameters={"msg": "HelloWorld!"},
-    artifacts={"inp_art": foo},
-)
-``` 
-This step will instantiate the OP template created in [1.2.2](#122-a-nameoptemplatea-op-template). Note that foo is an artifact either uploaded from local or output of another step.
+OP template (abbr. OP) is a fundamental building block of a workflow. It defines a particular operation to be executed given the input and the expected output. Both the input and output can be parameters and/or artifacts. The most common OP template is the container OP template. Two types of container OP templates are supported: `ShellOPTemplate`, `PythonScriptOPTemplate`. `ShellOPTemplate` defines an operation by shell script and a container image where the script runs. `PythonScriptOPTemplate` defines an operation by Python script and a container image.
 
+As a more Python-native category of OP templates, `PythonOPTemplate` defines OPs in the form of Python classes or Python functions (called class OP or function OP correspondingly). As Python is a weak typed
+language, we impose strict type checking to Python OPs to alleviate ambiguity and unexpected behaviors.
 
-####  1.2.4. <a name='Workflow'></a> Workflow
-`Workflow` is the connecting block for building a workflow. A `workflow` is created by adding `step`s together.
-```python
-from dflow import Workflow
-
-wf = Workflow(name="hello-world")
-wf.add(simple_example_step)
-```
-Submit a workflow by
-```python
-wf.submit()
-```
-One can also add a list of `step`s to a workflow to make them run in parallel
-```python
-wf.add([hello2, hello3])
-```
-An example using all the elements discussed in [1.2](#12-a-namecommonlayera-common-layer) is shown here:
-- [ShellOP example](examples/test_steps.py)
-
-###  1.3. <a name='Interfacelayer'></a> Interface layer
-Interface layer handles more Python-native OPs defined in the form of class.
-####  1.3.1. <a name='PythonOP'></a> Python OP
-`PythonOPTemplate` is another kind of OP template. It inherits from `PythonScriptOPTemplate` but allows users to define operation (OP) in the form of a Python class. As Python is a weak typed language, we impose strict type checking to `PythonOP` to alleviate ambiguity and unexpected behaviors.
-
-The structures of the inputs and outputs of a `PythonOP` are defined in the static methods `get_input_sign` and `get_output_sign`. Each of them returns a `OPIOSign` object, which is a dictionary mapping from the name of a parameter/artifact to its sign. 
-<!-- For a parameter, its sign is its variable type, such as `str`, `float`, `list`, or any user-defined Python class. Since argo only accept string as parameter value, dflow encodes all parameters to json (except string type parameters) before passing them to argo, and decodes argo parameters from json (except string type parameters). For an artifact, its sign must be an instance of `Artifact`. `Artifact` receives the type of the path variable as the constructor argument, only `str`, `pathlib.Path`, `typing.Set[str]`, `typing.Set[pathlib.Path]`, `typing.List[str]`, `typing.List[pathlib.Path]` are supported. If a `OP` returns a list of path as an artifact, dflow not only collects files or directories in the returned list of path, and package them in an artifact, but also records their relative path in the artifact. Thus dflow can unpack the artifact to a list of path again before passing to the next `OP`. When no file or directory exists, dflow regards it as `None`. -->
-
-The execution of the `PythonOP` is defined in the `execute` method. The `execute` method receives a `OPIO` object as input and outputs a `OPIO` object. `OPIO` is a dictionary mapping from the name of a parameter/artifact to its value/path. The type of the parameter value or the artifact path should be in accord with that declared in the sign. Type checking is implemented before and after the `execute` method.
+For an class OP, the structures of the inputs and outputs of an OP are declared in the static methods `get_input_sign` and `get_output_sign`. Each of them returns a dictionary mapping from the name of a parameter/artifact to its type. The execution of the OP is defined in the `execute` method. The types of the parameter values passed in and out should be in accord with those declared in the sign. Type checking is implemented before and after the `execute` method. For an input/output artifact, its sign should be like `Artifact(type)` where `type` can be `Path`, `List[Path]`, `Dict[str, Path]` or `dflow.python.NestedDict[Path]`. For input artifact, the `execute` method will receive a path, a list of paths or a dictionary of paths according to its sign . OP developer can directly process the file or directory at the path. For output artifact, the `execute` method should also return a path, a list of paths or a dictionary of paths according to its sign.
 
 ```python
 from dflow.python import OP, OPIO, OPIOSign, Artifact
 from pathlib import Path
 import shutil
 
 
@@ -194,335 +99,380 @@
         pass
 
     @classmethod
     def get_input_sign(cls):
         return OPIOSign(
             {
                 "msg": str,
-                "inp_art": Artifact(Path),
+                "foo": Artifact(Path),
             }
         )
 
     @classmethod
     def get_output_sign(cls):
         return OPIOSign(
             {
                 "msg": str,
-                "out_art": Artifact(Path),
+                "bar": Artifact(Path),
             }
         )
 
     @OP.exec_sign_check
     def execute(
         self,
         op_in: OPIO,
     ) -> OPIO:
-        shutil.copy(op_in["inp_art"], "bar.txt")
+        shutil.copy(op_in["foo"], "bar.txt")
         out_msg = op_in["msg"]
         op_out = OPIO(
             {
                 "msg": out_msg,
-                "out_art": Path("bar.txt"),
+                "bar": Path("bar.txt"),
             }
         )
         return op_out
 ```
-The above example defines an OP `SimpleExample`. The operation is to copy `foo.txt` to `bar.txt` and write the properties of the parameters with name msg to `msg.txt`. 
 
-One may also define OP using decorator `@OP.function` and Python Annotation as:
+The above example defines an OP `SimpleExample`. The operation is to copy the input artifact `foo` to output artifact `bar` and to copy the input parameter `msg` to output parameter `msg`.
+
+For an function OP, the structure of the inputs and outputs are declared in the type annotations more compactly and execution is defined in the function body. Type checking is implemented before and after the function as well. We recommend `python>=3.9` to use this syntax sugar. See more about Python Annotation at [Python official howtos](https://docs.python.org/3/howto/annotations.html).
 
 ```python
 from dflow.python import OP, Artifact
 from pathlib import Path
 import shutil
 
 @OP.function
 def SimpleExample(
 		msg: str,
-		inp_art: Artifact(Path),
-)->{"msg": str, "out_art": Artifact(Path),}:
-    shutil.copy(inp_art, "bar.txt")
+		foo: Artifact(Path),
+) -> {"msg": str, "bar": Artifact(Path)}:
+    shutil.copy(foo, "bar.txt")
     out_msg = msg
-    return {"msg": out_msg, "out_art": Path("bar.txt"),}
+    return {"msg": out_msg, "bar": Path("bar.txt")}
 ```
 
-We recommend `python>=3.9` to use this syntax sugar.
-See more about Python Annotation at [Python official howtos](https://docs.python.org/3/howto/annotations.html).
+To define an OP template from the above class or function, we need to specify the container image and other optional arguments to `PythonOPTemplate`. `pydflow` need not to be installed in this image because local `pydflow` package will be uploaded into the container by default
 
-To use the above class as a PythonOPTemplate, we need to pass the above class to `PythonOPTemplate` and specify the container image. Note that `pydflow` must be installed in this image
 ```python
 from dflow.python import PythonOPTemplate
 
 simple_example_templ = PythonOPTemplate(SimpleExample, image="python:3.8")
 ```
 
-An example using all the elements discussed in [1.3](#12-a-namecommonlayera-common-layer)  is shown here:
-- [PythonOP example](examples/test_python.py)
+An example is here
+- [Python OP example](examples/test_python.py)
 
-##  2. <a name='QuickStart'></a> Quick Start
-###  2.1. <a name='PrepareKubernetescluster'></a> Prepare Kubernetes cluster
-Firstly, you will need a Kubernetes cluster. To setup a Kubernetes cluster on your laptop, you can download the [Minikube](https://minikube.sigs.k8s.io) on your PC and make sure you have [Docker](https://www.docker.com/) up and running on you PC.
+####  1.2.3. <a name='Step'></a> Step
+`Step` is the central block for formulating rules of data flows. A step is the result of instantiating an OP template, where values of all input parameters and sources of all input artifacts declared in the OP template must be specified here. The input parameters/artifacts of a step may be either static at the time of submission, or dynamically from outputs of another step.
 
-After downloading, you can initiate the Kubernetes cluster using: 
-```
-minikube start 
-```
-###  2.2. <a name='SetupArgoWorkflows'></a> Setup [Argo Workflows](https://argoproj.github.io/argo-workflows/quick-start/)
-To get started quickly, you can use the quick start manifest. It will install Argo Workflow as well as some commonly used components:
-```
-kubectl create ns argo
-kubectl apply -n argo -f https://raw.githubusercontent.com/deepmodeling/dflow/master/manifests/quick-start-postgres.yaml
-```
-If you are running Argo Workflows locally (e.g. using Minikube or Docker for Desktop), open a port-forward so you can access the namespace:
-```
-kubectl -n argo port-forward deployment/argo-server 2746:2746 --address 0.0.0.0
-```
-This will serve the user interface on https://localhost:2746
+```python
+from dflow import Step
 
-For access to the minio object storage, open a port-forward for minio
+simple_example_step = Step(
+    name="step0",
+    template=simple_example_templ,
+    parameters={"msg": "HelloWorld!"},
+    artifacts={"inp_art": foo},
+)
+``` 
+
+Note that `foo` here is an artifact either uploaded from local or output of another step.
+
+
+####  1.2.4. <a name='Workflow'></a> Workflow
+`Workflow` connects blocks together to build a workflow. A simple serial workflow is created by adding steps in sequence. Adding a list of steps to a workflow means these steps running in parallel.
+
+```python
+from dflow import Workflow
+
+wf = Workflow(name="hello-world")
+wf.add(simple_example_step)
 ```
-kubectl -n argo port-forward deployment/minio 9000:9000 --address 0.0.0.0
+
+Submit a workflow by
+
+```python
+wf.submit()
 ```
 
-###  2.3. <a name='Installdflow'></a> Install dflow
+An example is here
+- [Workflow example](examples/test_steps.py)
+
+
+##  2. <a name='QuickStart'></a> Quick Start
+
+###  2.1. <a name='SetupArgoServer'></a> Setup Argo Server
+
+If you have an Argo server already, you can skip this step. Otherwise you can follow the [installation guide](tutorials/readme.md).
+
+###  2.2. <a name='Installdflow'></a> Install dflow
 Make sure your Python version is not less than 3.6 and install dflow
+
 ```
 pip install pydflow
 ```
 
-###  2.4. <a name='Runanexample'></a> Run an example
-Submit a simple workflow
+###  2.3. <a name='Runanexample'></a> Run an example
+There are several [notebook tutorials](tutorials/readme.md) that can help you start to use dflow. Besides, you can submit a simple workflow from the terminal
+
 ```
-python examples/test_steps.py
+python examples/test_python.py
 ```
-Then you can check the submitted workflow through argo's UI.
+
+Then you can check the submitted workflow through [argo's UI](https://127.0.0.1:2746).
 
 ##  3. <a name='UserGuide'></a> User Guide ([dflow-doc](https://deepmodeling.com/dflow/dflow.html))
-###  3.1. <a name='Commonlayer-1'></a> Common layer
+###  3.1. <a name='Commonlayer'></a> Common layer
 
 ####  3.1.1. <a name='Workflowmanagement'></a> Workflow management
 After submitting a workflow by `wf.submit()`, or getting a history workflow by `wf = Workflow(id="xxx")`, one can track its real-time status with APIs
 
 - `wf.id`: workflow ID in argo
 - `wf.query_status()`: query workflow status, return `"Pending"`, `"Running"`, `"Succeeded"`, etc.
 - `wf.query_step(name=None)`: query step by name (support for regex), return a list of argo step objects
     - `step.phase`: phase of a step, `"Pending"`, `"Running"`, `Succeeded`, etc.
     - `step.outputs.parameters`: a dictionary of output parameters
     - `step.outputs.artifacts`: a dictionary of output artifacts
 
 ####  3.1.2. <a name='Uploaddownloadartifact'></a> Upload/download artifact
-Dflow offers tools for uploading files to Minio and downloading files from Minio (default object storage in the quick start). User can upload a list of files or directories and get an artifact object, which can be used as argument of a step
+Dflow offers tools for uploading files to the artifact repository and downloading files from it (default artifact repository is Minio set up in the quick start). User can upload a file/directory, a list of files/directories or a dictionary of files/directories and get an artifact object, which can be used as argument of a step
+
 ```python
 artifact = upload_artifact([path1, path2])
 step = Step(
     ...
     artifacts={"foo": artifact}
 )
 ```
+
 User can also download the output artifact of a step queried from a workflow (to current directory for default)
+
 ```python
 step = wf.query_step(name="hello")
 download_artifact(step.outputs.artifacts["bar"])
 ```
-Modify `dflow.s3_config` to configure S3 globally.
+
+Modify `dflow.s3_config` to configure artifact repository settings globally.
 
 Note: dflow retains the relative path of the uploaded file/directory with respect to the current directory during uploading. If file/directory outside current directory is uploaded, its absolute path is used as the relative path in the artifact. If you want a different directory structure in the artifact with the local one, you can make soft links and then upload.
 
 ####  3.1.3. <a name='Steps'></a> Steps
-`Steps` is another kind of OP template which is defined by its constituent `step`s instead of a container. It can be seen as a sub-workflow or a super OP template consisting of some smaller OPs. `Steps` is a sequential array of concurrent `Step`. A simple example goes like `[[s00,s01],[s10,s11,s12]]`, where inner array represent concurrent tasks while outer array is sequential. Add a `step` to a `steps` just like for a `workflow`
+`Steps` is another kind of OP template which is defined by its constituent steps instead of a container. It can be seen as a sub-workflow or a super OP template consisting of some smaller OPs. A `steps` includes an array of arrays of `step`s, e.g. `[[s00,s01],[s10,s11,s12]]`, where inner array represent concurrent steps while outer array is sequential. One can declare input/output parameters/artifacts for a steps by
+
+```python
+steps.inputs.parameters["msg"] = InputParameter()
+steps.inputs.artifacts["foo"] = InputArtifact()
+steps.outputs.parameters["msg"] = OutputParameter()
+steps.outputs.parameters["bar"] = OutputArtifact()
+```
+
+
+Add a `step` to a `steps` just like for a `workflow`
+
 ```python
 steps.add(step)
 ```
-`Steps` can be used as the template to define a bigger `step`. Thus one can construct complex workflows of nested structure. One is also allowed to recursively use a `Steps` as the template of a building bloack inside it self to achieve dynamic loop.
+
+`steps` can be used as the template to instantiate a bigger `step` just like script OP templates. Thus one can construct complex workflows of nested structure. One is also allowed to recursively use a `steps` as the template of a building bloack inside it self to achieve dynamic loop.
+
+The output parameter of a `steps` can be set to come from a step of it by
+
+```python
+steps.outputs.parameters["msg"].value_from_parameter = step.outputs.parameters["msg"]
+```
+
+Here, `step` must be contained in `steps`. For assigning output artifact for a `steps`, use
+
+```python
+steps.outputs.artifacts["foo"]._from = step.outputs.parameters["foo"]
+```
 
 - [Recursive example](examples/test_recurse.py)
 
 ####  3.1.4. <a name='DAG'></a> DAG
-`DAG` is another kind of OP template which is defined by its constituent `task`s and their dependencies. The usage of `DAG` is similar to that of `steps`. To add a `task` to a `DAG`, use
+`DAG` is another kind of OP template which is defined by its constituent tasks and their dependencies. The usage of `DAG` is similar to that of `Steps`. To add a `task` to a `dag`, use
+
 ```python
 dag.add(task)
 ```
-The usage of `task` is also similar to that of `step`. Dflow will automatically detect dependencies among `task`s of a `DAG` (from input/output relations). Additional dependencies can be declared by
+
+The usage of `task` is also similar to that of `step`. Dflow will automatically detect dependencies among tasks of a `dag` (from input/output relations). Additional dependencies can be declared by
+
 ```python
 task_3 = Task(..., dependencies=[task_1, task_2])
 ```
 
 - [DAG example](examples/test_dag.py)
 
-####  3.1.5. <a name='OutputparametersandartifactsofSteps'></a> Output parameters and artifacts of Steps
-The output parameter of a `Steps` can be set to come from a step of it by `steps.outputs.parameters["msg"].value_from_parameter = step.outputs.parameters["msg"]`. Here, `step` must be contained in `steps`. For assigning output artifact for a `Steps`, use `steps.outputs.artifacts["foo"]._from = step.outputs.parameters["foo"]`.
+####  3.1.5. <a name='Conditionalstepparametersandartifacts'></a> Conditional step, parameters and artifacts
+Set a step to be conditional by `Step(..., when=expr)` where `expr` is an boolean expression in string format. Such as `"%s < %s" % (par1, par2)`. The step will be performed if the expression is evalutated to be true, otherwise skipped. The `when` argument is often used as the breaking condition of recursive steps. The output parameter of a `steps` (similar to `dag`) can be assigned as conditional by
 
-####  3.1.6. <a name='Conditionalstepparametersandartifacts'></a> Conditional step, parameters and artifacts
-Set a step to be conditional by `Step(..., when=expr)` where `expr` is an boolean expression in string format. Such as `"%s < %s" % (par1, par2)`. The `when` argument is often used as the breaking condition of recursive steps. The output parameter of a `Steps` can be assigned as optional by
 ```python
 steps.outputs.parameters["msg"].value_from_expression = if_expression(
     _if=par1 < par2,
     _then=par3,
     _else=par4
 )
 ```
-Similarly, the output artifact of a `Steps` can be assigned as optional by
+
+Similarly, the output artifact of a `steps` can be assigned as conditional by
+
 ```python
 steps.outputs.artifacts["foo"].from_expression = if_expression(
     _if=par1 < par2,
     _then=art1,
     _else=art2
 )
 ```
 
 - [Conditional outputs example](examples/test_conditional_outputs.py)
 
-####  3.1.7. <a name='Produceparallelstepsusingloop'></a> Produce parallel steps using loop
-`with_param` and `with_sequence` are 2 arguments of `Step` for automatically generating a list of parallel steps. These steps share a common OP template, and only differ in the input parameters.
+####  3.1.6. <a name='Produceparallelstepsusingloop'></a> Produce parallel steps using loop
+In scientific computing, it is often required to produce a list of parallel steps which share a common OP template, and only differ in the input parameters. `with_param` and `with_sequence` are 2 arguments of `Step` for automatically generating a list of parallel steps. These steps share a common OP template, and only differ in the input parameters.
 
 A step using `with_param` option generates parallel steps on a list (either a constant list or referring to another parameter, e.g. an output parameter of another step or an input parameter of the `steps` or `DAG` context), the parallelism equals to the length of the list. Each parallel step picks an item from the list by `"{{item}}"`, such as
+
 ```python
 step = Step(
     ...
     parameters={"msg": "{{item}}"},
     with_param=steps.inputs.parameters["msg_list"]
 )
 ```
+
 A step using `with_sequence` option generates parallel steps on a numeric sequence. `with_sequence` is usually used in coordination with `argo_sequence` which returns an Argo's sequence. For `argo_sequence`, the number at which to start the sequence is specified by `start` (default: 0). One can either specify the number of elements in the sequence by `count` or the number at which to end the sequence by `end`. The printf format string can be specified by `format` to format the value in the sequence. Each argument can be passed with a parameter, `argo_len` which returns the length of a list may be useful. Each parallel step picks an element from the sequence by `"{{item}}"`, such as
+
 ```python
 step = Step(
     ...
     parameters={"i": "{{item}}"},
     with_sequence=argo_sequence(argo_len(steps.inputs.parameters["msg_list"]))
 )
 ```
 
-####  3.1.8. <a name='Timeout'></a> Timeout
+####  3.1.7. <a name='Timeout'></a> Timeout
 Set the timeout of a step by `Step(..., timeout=t)`. The unit is second.
 
 - [Timeout example](examples/test_error_handling.py)
 
-####  3.1.9. <a name='Continueonfailed'></a> Continue on failed
+####  3.1.8. <a name='Continueonfailed'></a> Continue on failed
 Set the workflow to continue when a step fails by `Step(..., continue_on_failed=True)`.
 
 - [Continue on failed example](examples/test_error_handling.py)
 
-####  3.1.10. <a name='Continueonsuccessnumberratioofparallelsteps'></a> Continue on success number/ratio of parallel steps
-Set the workflow to continue when certain number/ratio of parallel steps succeed by `Step(..., continue_on_num_success=n)` or `Step(..., continue_on_success_ratio=r)`.
+####  3.1.9. <a name='Continueonsuccessnumberratioofparallelsteps'></a> Continue on success number/ratio of parallel steps
+For a group of parallel steps generated by `with_param` or `with_sequence`, set the workflow to continue when certain number/ratio of parallel steps succeed by `Step(..., continue_on_num_success=n)` or `Step(..., continue_on_success_ratio=r)`.
 
 - [Continue on success ratio example](examples/test_success_ratio.py)
 
-####  3.1.11. <a name='Optionalinputartifacts'></a> Optional input artifacts
+####  3.1.10. <a name='Optionalinputartifacts'></a> Optional input artifacts
 Set an input artifact to be optional by `op_template.inputs.artifacts["foo"].optional = True`.
 
-####  3.1.12. <a name='Defaultvalueforoutputparameters'></a> Default value for output parameters
+####  3.1.11. <a name='Defaultvalueforoutputparameters'></a> Default value for output parameters
 Set default value for an output parameter by `op_template.outputs.parameters["msg"].default = default_value`. The default value will be used when the expression in `value_from_expression` fails or the step is skipped.
 
-####  3.1.13. <a name='Keyofastep'></a> Key of a step
-You can set a key for a step by `Step(..., key="some-key")` for the convenience of locating the step. The key can be regarded as an input parameter which may contain reference of other parameters. For instance, the key of a step can change with iterations of a dynamic loop. Once key is assigned to a step, the step can be query by `wf.query_step(key="some-key")`. If the key is unique within the workflow, the `query_step` method returns a list consist of only one element.
+####  3.1.12. <a name='Keyofastep'></a> Key of a step
+One can assign a key for a step by `Step(..., key="some-key")` for the convenience of locating the step. The key can be regarded as an input parameter which may contain reference of other parameters. For instance, the key of a step can change with iterations of a dynamic loop. Once key is assigned to a step, the step can be query by `wf.query_step(key="some-key")`. If the key is unique within the workflow, the `query_step` method returns a list consist of only one element.
 
 - [Key of step example](examples/test_reuse.py)
 
-####  3.1.14. <a name='Resubmitaworkflow'></a> Resubmit a workflow
+####  3.1.13. <a name='Resubmitaworkflow'></a> Resubmit a workflow
 Workflows often have some steps that are expensive to compute. The outputs of previously run steps can be reused for submitting a new workflow. E.g. a failed workflow can be restarted from a certain point after some modification of the workflow template or even outputs of completed steps. For example, submit a workflow with reused steps by `wf.submit(reuse_step=[step0, step1])`. Here, `step0` and `step1` are previously run steps returned by `query_step` method. Before the new workflow runs a step, it will detect if there exists a reused step whose key matches that of the step about to run. If hit, the workflow will skip the step and set its outputs as those of the reused step. To modify outputs of a step before reusing, use `step0.modify_output_parameter(par_name, value)` for parameters and `step0.modify_output_artifact(art_name, artifact)` for artifacts.
 
 - [Reuse step example](examples/test_reuse.py)
 
-####  3.1.15. <a name='Executor'></a> Executor
-By default, for a "script step" (a step whose template is a script OP template), the Shell script or Python script runs in the container directly. Alternatively, one can modify the executor to run the script. Dflow offers an extension point for "script step" `Step(..., executor=my_executor)`. Here, `my_executor` should be an instance of class derived from `Executor`. A `Executor`-derived class should implement a method `render` which converts original template to a new template.
+####  3.1.14. <a name='Executor'></a> Executor
+For a "script step" (a step whose template is a script OP template), by default the Shell script or Python script runs in the container directly. Alternatively, one can modify the executor to run the script. Dflow offers an extension point for "script step" `Step(..., executor=my_executor)`. Here, `my_executor` should be an instance of class derived from the abstract class `Executor`. An implementation class of `Executor` should implement a method `render` which converts original template to a new template.
+
 ```python
-class Executor(object):
+class Executor(ABC):
+    @abc.abstractmethod
     def render(self, template):
         pass
 ```
-A context is similar to an executor, but assigned to a workflow `Workflow(context=...)` and affect every step.
-
-####  3.1.16. <a name='SubmitSlurmjobviaslurmexecutor'></a> Submit Slurm job via slurm executor
 
-`SlurmRemoteExecutor` is provided as an example of executor. The executor submits a slurm job to a remote host and synchronize its status and logs to the dflow step. The central logic of the executor is implemented in the Golang project [Dflow-extender](https://github.com/dptech-corp/dflow-extender). If you want to run a step on a slurm cluster remotely, do something like
-```python
-Step(
-    ...,
-    executor=SlurmRemoteExecutor(host="1.2.3.4",
-        username="myuser",
-        header="""#!/bin/bash
-                  #SBATCH -N 1
-                  #SBATCH -n 1
-                  #SBATCH -p cpu""")
-)
-```
-There are 3 options for SSH authentication, using password, specify path of private key file locally, or upload authorized private key to each node (or equivalently add each node to the authorized host list).
+A context is similar to an executor, but assigned to a workflow `Workflow(context=...)` and affect every step.
 
-- [Slurm executor example](examples/test_slurm.py)
+####  3.1.15. <a name='SubmitHPCBohriumjobviadispatcherplugin'></a> Submit HPC/Bohrium job via dispatcher plugin
 
-####  3.1.17. <a name='SubmitHPCjobviadispatcherplugin'></a> Submit HPC job via dispatcher plugin
+[DPDispatcher](https://github.com/deepmodeling/dpdispatcher) is a python package used to generate HPC scheduler systems (Slurm/PBS/LSF) or [Bohrium](https://bohrium.dp.tech) jobs input scripts and submit these scripts and poke until they finish. Dflow provides simple interface to invoke dispatcher as executor to complete script steps. E.g.
 
-[DPDispatcher](https://github.com/deepmodeling/dpdispatcher) is a python package used to generate HPC scheduler systems (Slurm/PBS/LSF) jobs input scripts and submit these scripts to HPC systems and poke until they finish. Dflow provides simple interface to invoke dispatcher as executor to complete script steps. E.g.
 ```python
 from dflow.plugins.dispatcher import DispatcherExecutor
 Step(
     ...,
     executor=DispatcherExecutor(host="1.2.3.4",
         username="myuser",
         queue_name="V100")
 )
 ```
+
 For SSH authentication, one can either specify path of private key file locally, or upload authorized private key to each node (or equivalently add each node to the authorized host list). For configuring extra [machine, resources or task parameters for dispatcher](https://docs.deepmodeling.com/projects/dpdispatcher/en/latest/), use `DispatcherExecutor(..., machine_dict=m, resources_dict=r, task_dict=t)`.
 
 - [Dispatcher executor example](examples/test_dispatcher.py)
 
-####  3.1.18. <a name='SubmitSlurmjobviavirtualnode'></a> Submit Slurm job via virtual node
+####  3.1.16. <a name='SubmitSlurmjobviavirtualnode'></a> Submit Slurm job via virtual node
 
 Following the installation steps in the [wlm-operator](https://github.com/dptech-corp/wlm-operator) project to add Slurm partitions as virtual nodes to Kubernetes (use manifests [configurator.yaml](manifests/configurator.yaml), [operator-rbac.yaml](manifests/operator-rbac.yaml), [operator.yaml](manifests/operator.yaml) in this project which modified some RBAC configurations)
 ```
 $ kubectl get nodes
 NAME                            STATUS   ROLES                  AGE    VERSION
 minikube                        Ready    control-plane,master   49d    v1.22.3
 slurm-minikube-cpu              Ready    agent                  131m   v1.13.1-vk-N/A
 slurm-minikube-dplc-ai-v100x8   Ready    agent                  131m   v1.13.1-vk-N/A
 slurm-minikube-v100             Ready    agent                  131m   v1.13.1-vk-N/A
 ```
 Then you can assign a step to be executed on a virtual node (i.e. submit a Slurm job to the corresponding partition to complete the step)
+
 ```python
 step = Step(
     ...
     executor=SlurmJobTemplate(
         header="#!/bin/sh\n#SBATCH --nodes=1",
         node_selector={"kubernetes.io/hostname": "slurm-minikube-v100"}
     )
 )
 ```
 
-####  3.1.19. <a name='UseresourcesinKubernetes'></a> Use resources in Kubernetes
+####  3.1.17. <a name='UseresourcesinKubernetes'></a> Use resources in Kubernetes
 
 A step can also be completed by a Kubernetes resource (e.g. Job or custom resources). At the beginning, a manifest is applied to Kubernetes. Then the status of the resource is monitered until the success condition or the failure condition is satisfied.
+
 ```python
-class Resource(object):
+class Resource(ABC):
     action = None
     success_condition = None
     failure_condition = None
-    def get_manifest(self, template):
+    @abc.abstractmethod
         pass
 ```
 
 - [Wlm example](examples/test_wlm.py)
 
-####  3.1.20. <a name='Importantnotevariablenames'></a> Important note: variable names
+####  3.1.18. <a name='Importantnotevariablenames'></a> Important note: variable names
 
 Dflow has following restrictions on variable names.
 
 | Variable name | Static/Dynamic | Restrictions | Example |
 | :------------ | -------------- | ------------ | ------- |
 | Workflow/OP template name | Static | Lowercase RFC 1123 subdomain (must consist of lower case alphanumeric characters, '-' or '.', and must start and end with an alphanumeric character | my-name |
 | Step/Task name | Static | Must consist of alpha-numeric characters or '-', and must start with an alpha-numeric character | My-name1-2, 123-NAME |
 | Parameter/Artifact name | Static | Must consist of alpha-numeric characters, '_' or '-' | my_param_1, MY-PARAM-1 |
 | Key name | Dynamic | Lowercase RFC 1123 subdomain (must consist of lower case alphanumeric characters, '-' or '.', and must start and end with an alphanumeric character | my-name |
 
-#### 3.1.21. <a name='DebugmodeDflowindependentofKubernetes'></a> Debug mode: dflow independent of Kubernetes
+####  3.1.19. <a name='DebugmodedflowindependentofKubernetes'></a> Debug mode: dflow independent of Kubernetes
 
 The debug mode is enabled by setting
+
 ```python
 from dflow import config
 config["mode"] = "debug"
 ```
+
 Before running a workflow locally, make sure that the dependencies of all OPs in the workflow are well-configured in the locally environment, unless the dispatcher executor is employed to submit jobs to some remote environments. The debug mode uses the current directory as the working directory by default. Each workflow will create a new directory there, whose structure will be like
 ```
 python-lsev6
 ├── status
 └── step-penf5
     ├── inputs
     │   ├── artifacts
@@ -545,18 +495,42 @@
     └── workdir
         ├── ...
 ```
 The top level contains the status and all steps of the workflow. The directory name for each step will be its key if provided, or generated from its name otherwise. The step directory contains the input/output parameters/artifacts, the type and the phase of the step. For a step of type "Pod", its directory also includes the script, the log file and the working directory for the step.
 
 - [Debug mode examples](examples/debug)
 
-###  3.2. <a name='Interfacelayer-1'></a> Interface layer
+####  3.1.20. <a name='Artifactstorageplugins'></a>Artifact storage plugins
+
+The default storage for artifacts in dflow is a Minio deployment in the Kubernetes cluster. While other artifact storages are supported (e.g. Aliyun OSS, Azure blob storage (ABS), Google cloud storage(GCS)). Dflow provides an extension point to use customized storage in the artifact management. A storage client is a class implementing 5 abstract methods, `upload`, `download`, `list`, `copy` and `get_md5` (optional), which offer the functionality of uploading file, downloading file, listing files with a particular prefix, copying file on the server side and getting the MD5 sum of file, respectively. Use a custom storage client object by configuring s3_config["storage_client"].
+
+```python
+class StorageClient(ABC):
+    @abc.abstractmethod
+    def upload(self, key: str, path: str) -> None:
+        pass
+    @abc.abstractmethod
+    def download(self, key: str, path: str) -> None:
+        pass
+    @abc.abstractmethod
+    def list(self, prefix: str, recursive: bool = False) -> List[str]:
+        pass
+    @abc.abstractmethod
+    def copy(self, src: str, dst: str) -> None:
+        pass
+    @abc.abstractmethod
+    def get_md5(self, key: str) -> str:
+        pass
+```
+
+###  3.2. <a name='Interfacelayer'></a> Interface layer
 
 ####  3.2.1. <a name='Slices'></a> Slices
-`Slices` helps user to slice input parameters/artifacts (which must be lists) to feed parallel steps and stack their output parameters/artifacts to lists in the same pattern. For example,
+In coordination with [parallel steps](#Produceparallelstepsusingloop), `Slices` helps user to slice input parameters/artifacts (which must be lists) to feed parallel steps and stack their output parameters/artifacts to lists in the same pattern. The Python OP only need to handle one slice. For example,
+
 ```python
 step = Step(name="parallel-tasks",
     template=PythonOPTemplate(
         ...,
         slices=Slices("{{item}}",
             input_parameter=["msg"],
             input_artifact=["data"],
@@ -567,19 +541,21 @@
     },
     artifacts={
         "data": data_list
     },
     with_param=argo_range(5)
 )
 ```
+
 In this example, each item in `msg_list` is passed to a parallel step as the input parameter `msg`, each part in `data_list` is passed to a parallel step as the input artifact `data`. Finally, the output artifacts `log` of all parallel steps are collected to one artifact `step.outputs.artifacts["log"]`.
 
 - [Slices example](examples/test_slices.py)
 
 It should be noticed that this feature by default passes full input artifacts to each parallel step which may only use some slices of these artifacts. In comparison, the subpath mode of slices only passes one single slice of the input artifacts to each parallel step. To use the subpath mode of slices,
+
 ```python
 step = Step(name="parallel-tasks",
     template=PythonOPTemplate(
         ...,
         slices=Slices(sub_path=True,
             input_parameter=["msg"],
             input_artifact=["data"],
@@ -588,36 +564,39 @@
     parameters = {
         "msg": msg_list
     },
     artifacts={
         "data": data_list
     })
 ```
+
 Here, the slice pattern (`{{item}}`) of `PythonOPTemplate` and the `with_param` argument of the `Step` need not to be set, because they are fixed in this mode. Each input parameter and artifact to be sliced must be of the same length, and the parallelism equals to this length. Another noticeable point is that in order to use the subpath of the artifacts, these artifacts must be saved without compression when they are generated. E.g. declare `Artifact(..., archive=None)` in the output signs of Python OP, or specify `upload_artifact(..., archive=None)` while uploading artifacts. Besides, one can use `dflow.config["archive_mode"] = None` to set default archive mode to no compression globally.
 
 - [Subpath mode of slices example](examples/test_subpath_slices.py)
 
 ####  3.2.2. <a name='Retryanderrorhandling'></a> Retry and error handling
-Dflow catches `TransientError` and `FatalError` thrown from `OP`. User can set maximum number of retries on `TransientError` by `PythonOPTemplate(..., retry_on_transient_error=n)`. Timeout error is regarded as fatal error for default. To treat timeout error as transient error, set `PythonOPTemplate(..., timeout_as_transient_error=True)`.
+Dflow catches `TransientError` and `FatalError` thrown from `OP`. User can set maximum number of retries on `TransientError` by `PythonOPTemplate(..., retry_on_transient_error=n)`. Timeout error is regarded as fatal error for default. To treat timeout error as transient error, set `PythonOPTemplate(..., timeout_as_transient_error=True)`. When a fatal error is raised or the retries on transient error reaches maximum retries, the step is considered as failed.
 
 - [Retry example](examples/test_error_handling.py)
 
 ####  3.2.3. <a name='Progress'></a> Progress
 A `OP` can update progress in the runtime so that user can track its real-time progress
+
 ```python
 class Progress(OP):
     progress_total = 100
     ...
     def execute(op_in):
         for i in range(10):
             self.progress_current = 10 * (i + 1)
             ...
 ```
 
 - [Progress example](examples/test_progress.py)
 
 ####  3.2.4. <a name='Uploadpythonpackagesfordevelopment'></a> Upload python packages for development
 To avoid frequently making image during development, dflow offers an interface to upload local packages into container and add them to `$PYTHONPATH`, such as `PythonOPTemplate(..., python_packages=["/opt/anaconda3/lib/python3.9/site-packages/numpy"])`. One can also globally specify packages to be uploaded, which will affect all `OP`s
+
 ```python
 from dflow.python import upload_packages
 upload_packages.append("/opt/anaconda3/lib/python3.9/site-packages/numpy")
 ```
```

### Comparing `pydflow-1.6.99/README.md` & `pydflow-1.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,181 +1,108 @@
+Metadata-Version: 2.1
+Name: pydflow
+Version: 1.7.0
+Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
+Home-page: https://github.com/deepmodeling/dflow
+Author: Xinzijian Liu
+Author-email: liuxzj@dp.tech
+License: LGPLv3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # DFLOW
 
 [Dflow](https://deepmodeling.com/dflow/dflow.html) is a Python framework for constructing scientific computing workflows (e.g. concurrent learning workflows) employing [Argo Workflows](https://argoproj.github.io/) as the workflow engine.
 
 For dflow's users (e.g. ML application developers), dflow offers user-friendly functional programming interfaces for building their own workflows. Users need not be concerned with process control, task scheduling, observability and disaster tolerance. Users can track workflow status and handle exceptions by APIs as well as from frontend UI. Thereby users are enabled to concentrate on implementing operations (OPs) and orchestrating workflows.
 
-For dflow's developers, dflow wraps on argo SDK, keeps details of computing and storage resources from users, and provides extension abilities. While argo is a cloud-native workflow engine, dflow uses containers to decouple computing logic and scheduling logic, and uses Kubernetes to make workflows observable, reproducible and robust. Dflow is designed to be based on a distributed, heterogeneous infrastructure. The most common computing resources in scientific computing may be HPC clusters. User can either use executor to manage HPC jobs within dflow ([dflow-extender](https://github.com/dptech-corp/dflow-extender)) or using [DPDispatcher](https://github.com/deepmodeling/dpdispatcher) plugin, or use virtual node technique to uniformly manage HPC resources in the framework of Kubernetes ([wlm-operator](https://github.com/dptech-corp/wlm-operator)).
+For dflow's developers, dflow wraps on argo SDK, keeps details of computing and storage resources from users, and provides extension abilities. While argo is a cloud-native workflow engine, dflow uses containers to decouple computing logic and scheduling logic, and uses Kubernetes to make workflows observable, reproducible and robust. Dflow is designed to be based on a distributed, heterogeneous infrastructure. The most common computing resources in scientific computing may be HPC clusters. User can either use executor to manage HPC jobs using [DPDispatcher](https://github.com/deepmodeling/dpdispatcher) plugin, or use virtual node technique to uniformly manage HPC resources in the framework of Kubernetes ([wlm-operator](https://github.com/dptech-corp/wlm-operator)).
 
-Dflow's OPs can be reused among workflows and shared among users. Dflow provides a cookie cutter recipe [dflow-op-cutter](https://github.com/deepmodeling/dflow-op-cutter) for template a new OP package. Start developing an OP package at once from
+OP template (abbr. OP) in dflow can be reused among workflows and shared among users. Dflow provides a cookie cutter recipe [dflow-op-cutter](https://github.com/deepmodeling/dflow-op-cutter) for template a new OP package. Start developing an OP package at once from
 ```python
 pip install cookiecutter
 cookiecutter https://github.com/deepmodeling/dflow-op-cutter.git
 ```
 
 Dflow provides a debug mode for running workflows bare-metally whose backend is implemented in dflow in pure Python, independent of Argo/Kubernetes. The debug mode uses local environment to execute OPs instead of containers. It implements most APIs of the default mode in order to provide an identical user experience. The debug mode offer convenience for debugging or testing without container. For the clusters having problem deploying docker and Kubernetes and difficult to access from outside, the debug mode may also be used for production, despite less robustness and observability.
 
 <!-- vscode-markdown-toc -->
 * 1. [ Overview](#Overview)
 	* 1.1. [ Architecture](#Architecture)
-	* 1.2. [ Common layer](#Commonlayer)
+	* 1.2. [ Basics](#Basics)
 		* 1.2.1. [ Parameters and artifacts](#Parametersandartifacts)
 		* 1.2.2. [ OP template](#OPtemplate)
 		* 1.2.3. [ Step](#Step)
 		* 1.2.4. [ Workflow](#Workflow)
-	* 1.3. [ Interface layer](#Interfacelayer)
-		* 1.3.1. [ Python OP](#PythonOP)
 * 2. [ Quick Start](#QuickStart)
-	* 2.1. [ Prepare Kubernetes cluster](#PrepareKubernetescluster)
-	* 2.2. [ Setup Argo Workflows](#SetupArgoWorkflows)
-	* 2.3. [ Install dflow](#Installdflow)
-	* 2.4. [ Run an example](#Runanexample)
-* 3. [ User Guide (dflow-doc)](#UserGuide)
-	* 3.1. [ Common layer](#Commonlayer-1)
+	* 2.1. [ Setup Argo Server](#SetupArgoServer)
+	* 2.2. [ Install dflow](#Installdflow)
+	* 2.3. [ Run an example](#Runanexample)
+* 3. [ User Guide](#UserGuide)
+	* 3.1. [ Common layer](#Commonlayer)
 		* 3.1.1. [ Workflow management](#Workflowmanagement)
 		* 3.1.2. [ Upload/download artifact](#Uploaddownloadartifact)
 		* 3.1.3. [ Steps](#Steps)
 		* 3.1.4. [ DAG](#DAG)
-		* 3.1.5. [ Output parameters and artifacts of Steps](#OutputparametersandartifactsofSteps)
-		* 3.1.6. [ Conditional step, parameters and artifacts](#Conditionalstepparametersandartifacts)
-		* 3.1.7. [ Produce parallel steps using loop](#Produceparallelstepsusingloop)
-		* 3.1.8. [ Timeout](#Timeout)
-		* 3.1.9. [ Continue on failed](#Continueonfailed)
-		* 3.1.10. [ Continue on success number/ratio of parallel steps](#Continueonsuccessnumberratioofparallelsteps)
-		* 3.1.11. [ Optional input artifacts](#Optionalinputartifacts)
-		* 3.1.12. [ Default value for output parameters](#Defaultvalueforoutputparameters)
-		* 3.1.13. [ Key of a step](#Keyofastep)
-		* 3.1.14. [ Resubmit a workflow](#Resubmitaworkflow)
-		* 3.1.15. [ Executor](#Executor)
-		* 3.1.16. [ Submit Slurm job via slurm executor](#SubmitSlurmjobviaslurmexecutor)
-		* 3.1.17. [ Submit HPC job via dispatcher plugin](#SubmitHPCjobviadispatcherplugin)
-		* 3.1.18. [ Submit Slurm job via virtual node](#SubmitSlurmjobviavirtualnode)
-		* 3.1.19. [ Use resources in Kubernetes](#UseresourcesinKubernetes)
-		* 3.1.20. [ Important note: variable names](#Importantnotevariablenames)
-        * 3.1.21. [ Debug mode: dflow independent of Kubernetes](#DebugmodeDflowindependentofKubernetes)
-	* 3.2. [ Interface layer](#Interfacelayer-1)
+		* 3.1.5. [ Conditional step, parameters and artifacts](#Conditionalstepparametersandartifacts)
+		* 3.1.6. [ Produce parallel steps using loop](#Produceparallelstepsusingloop)
+		* 3.1.7. [ Timeout](#Timeout)
+		* 3.1.8. [ Continue on failed](#Continueonfailed)
+		* 3.1.9. [ Continue on success number/ratio of parallel steps](#Continueonsuccessnumberratioofparallelsteps)
+		* 3.1.10. [ Optional input artifacts](#Optionalinputartifacts)
+		* 3.1.11. [ Default value for output parameters](#Defaultvalueforoutputparameters)
+		* 3.1.12. [ Key of a step](#Keyofastep)
+		* 3.1.13. [ Resubmit a workflow](#Resubmitaworkflow)
+		* 3.1.14. [ Executor](#Executor)
+		* 3.1.15. [ Submit HPC/Bohrium job via dispatcher plugin](#SubmitHPCBohriumjobviadispatcherplugin)
+		* 3.1.16. [ Submit Slurm job via virtual node](#SubmitSlurmjobviavirtualnode)
+		* 3.1.17. [ Use resources in Kubernetes](#UseresourcesinKubernetes)
+		* 3.1.18. [ Important note: variable names](#Importantnotevariablenames)
+		* 3.1.19. [ Debug mode: dflow independent of Kubernetes](#DebugmodedflowindependentofKubernetes)
+		* 3.1.20. [Artifact storage plugins](#Artifactstorageplugins)
+	* 3.2. [ Interface layer](#Interfacelayer)
 		* 3.2.1. [ Slices](#Slices)
 		* 3.2.2. [ Retry and error handling](#Retryanderrorhandling)
 		* 3.2.3. [ Progress](#Progress)
 		* 3.2.4. [ Upload python packages for development](#Uploadpythonpackagesfordevelopment)
 
 <!-- vscode-markdown-toc-config
 	numbering=true
 	autoSave=true
 	/vscode-markdown-toc-config -->
 <!-- /vscode-markdown-toc -->
 
 ##  1. <a name='Overview'></a> Overview
 ###  1.1. <a name='Architecture'></a> Architecture
-The dflow consists of a **common layer** and an **interface layer**.  Interface layer takes various OP templates from users, usually in the form of python classes, and transforms them into base OP templates that common layer can handle.
+The dflow consists of a **common layer** and an **interface layer**.  Interface layer takes various OP templates from users, usually in the form of python classes or functions, and transforms them into base OP templates that common layer can handle.
 
 <p align="center">
 <img src="./docs/imgs/dflow_architecture.png" alt="dflow_architecture" width="400"/>
 </p>
 <!-- <style>
 img {
   display: block;
   margin-left: auto;
   margin-right: auto;
 }
 </style> -->
 
-###  1.2. <a name='Commonlayer'></a> Common layer
-Common layer is an extension over argo client which provides functionalities such as file processing, computing resources management, workflow submission and management, etc.
+###  1.2. <a name='Basics'></a> Basics
+
 ####  1.2.1. <a name='Parametersandartifacts'></a> Parameters and artifacts
-Parameters and artifacts are data stored by the workflow and passed within the workflow. Parameters are saved as strings which can be displayed in the UI, while artifacts are saved as files.
+Parameters and artifacts are data stored by the workflow and passed within the workflow. Parameters are saved as text which can be displayed in the UI, while artifacts are saved as files. Parameters are passed to an OP with their values, while artifacts are passed as paths.
 
 ####  1.2.2. <a name='OPtemplate'></a> OP template
-OP template (shown as base OP in the figure above) is the fundamental building block of a workflow. It defines an operation to be executed given the input and output. Both the input and output can be parameters and/or artifacts. The most common OP template is the container OP template. Necessary arguments to be defined for the operation are the container image and scripts to be executed. Currently, two types of container OP templates are supported: `ShellOPTemplate`, `PythonScriptOPTemplate`. Shell OP template (`ShellOPTemplate`) defines an operation by a shell script and Python script OP template (`PythonScriptOPTemplate`) defines an operation by a Python script.
-
-To use the `ShellOPTemplate`:
-
-```python
-from dflow import ShellOPTemplate
-
-simple_example_templ = ShellOPTemplate(
-    name="Hello",
-    image="alpine:latest",
-    script="cp /tmp/foo.txt /tmp/bar.txt && echo {{inputs.parameters.msg}} > /tmp/msg.txt",
-)
-```
-The above example defines a `ShellOPTemplate` with `name = "Hello"` and container image `alpine:latest`. The operation is to copy `/tmp/foo.txt` (input artifacts) to `/tmp/bar.txt` (output artifacts) and printout the properties of the parameters with name `msg` (input parameters) and redirect it to `/tmp/msg.txt` (value in the file is the properties of the output parameters). 
-<!-- 
-Parameters and artifacts can be defined as the following:
-- Input/output parameters: a dictionary that maps the parameter name to its properties.
-- Input/output artifacts: a dictionary that maps the artifact name to its properties. -->
-
-To define the parameters and artifacts of this OPTemplate: 
-
-```python
-from dflow import InputParameter, InputArtifact, OutputParameter, OutputArtifact
-
-# define input
-simple_example_templ.inputs.parameters = {"msg": InputParameter()}
-simple_example_templ.inputs.artifacts = {"inp_art": InputArtifact(path="/tmp/foo.txt")}
-# define output
-simple_example_templ.outputs.parameters = {
-    "msg": OutputParameter(value_from_path="/tmp/msg.txt")
-}
-simple_example_templ.outputs.artifacts = {
-    "out_art": OutputArtifact(path="/tmp/bar.txt")
-}
-```
-
-In the above example, there are three things to clarify. 
-1. The value of the input parameter is optional for the OP template, if provided, it will be regarded as the default value which can be overridden at run time. 
-2. For the output parameter, the source where its value comes from should be specified. For the container OP template, the value may come from a certain file generated in the container (`value_from_path`). 
-3. The paths to the input and output artifact in the container are required to be specified.
-
-On the same level, one can also define a `PythonScriptOPTemplate` to achieve the same operation. 
-
-####  1.2.3. <a name='Step'></a> Step
-`Step` is the central block for building a workflow. A `step` is created by instantiating an OP template. When a `step` is initialized, values of all input parameters and sources of all input artifacts declared in the OP template must be specified.
-<!-- `Steps` is a sequential array of concurrent `Step`'s. A simple example goes like `[[s00, s01],  [s10, s11, s12]]`, where inner array represent concurrent tasks while outer array is sequential. (this part can be put in the User Guide-->
-```python
-from dflow import Step
-
-simple_example_step = Step(
-    name="step0",
-    template=simple_example_templ,
-    parameters={"msg": "HelloWorld!"},
-    artifacts={"inp_art": foo},
-)
-``` 
-This step will instantiate the OP template created in [1.2.2](#122-a-nameoptemplatea-op-template). Note that foo is an artifact either uploaded from local or output of another step.
+OP template (abbr. OP) is a fundamental building block of a workflow. It defines a particular operation to be executed given the input and the expected output. Both the input and output can be parameters and/or artifacts. The most common OP template is the container OP template. Two types of container OP templates are supported: `ShellOPTemplate`, `PythonScriptOPTemplate`. `ShellOPTemplate` defines an operation by shell script and a container image where the script runs. `PythonScriptOPTemplate` defines an operation by Python script and a container image.
 
+As a more Python-native category of OP templates, `PythonOPTemplate` defines OPs in the form of Python classes or Python functions (called class OP or function OP correspondingly). As Python is a weak typed
+language, we impose strict type checking to Python OPs to alleviate ambiguity and unexpected behaviors.
 
-####  1.2.4. <a name='Workflow'></a> Workflow
-`Workflow` is the connecting block for building a workflow. A `workflow` is created by adding `step`s together.
-```python
-from dflow import Workflow
-
-wf = Workflow(name="hello-world")
-wf.add(simple_example_step)
-```
-Submit a workflow by
-```python
-wf.submit()
-```
-One can also add a list of `step`s to a workflow to make them run in parallel
-```python
-wf.add([hello2, hello3])
-```
-An example using all the elements discussed in [1.2](#12-a-namecommonlayera-common-layer) is shown here:
-- [ShellOP example](examples/test_steps.py)
-
-###  1.3. <a name='Interfacelayer'></a> Interface layer
-Interface layer handles more Python-native OPs defined in the form of class.
-####  1.3.1. <a name='PythonOP'></a> Python OP
-`PythonOPTemplate` is another kind of OP template. It inherits from `PythonScriptOPTemplate` but allows users to define operation (OP) in the form of a Python class. As Python is a weak typed language, we impose strict type checking to `PythonOP` to alleviate ambiguity and unexpected behaviors.
-
-The structures of the inputs and outputs of a `PythonOP` are defined in the static methods `get_input_sign` and `get_output_sign`. Each of them returns a `OPIOSign` object, which is a dictionary mapping from the name of a parameter/artifact to its sign. 
-<!-- For a parameter, its sign is its variable type, such as `str`, `float`, `list`, or any user-defined Python class. Since argo only accept string as parameter value, dflow encodes all parameters to json (except string type parameters) before passing them to argo, and decodes argo parameters from json (except string type parameters). For an artifact, its sign must be an instance of `Artifact`. `Artifact` receives the type of the path variable as the constructor argument, only `str`, `pathlib.Path`, `typing.Set[str]`, `typing.Set[pathlib.Path]`, `typing.List[str]`, `typing.List[pathlib.Path]` are supported. If a `OP` returns a list of path as an artifact, dflow not only collects files or directories in the returned list of path, and package them in an artifact, but also records their relative path in the artifact. Thus dflow can unpack the artifact to a list of path again before passing to the next `OP`. When no file or directory exists, dflow regards it as `None`. -->
-
-The execution of the `PythonOP` is defined in the `execute` method. The `execute` method receives a `OPIO` object as input and outputs a `OPIO` object. `OPIO` is a dictionary mapping from the name of a parameter/artifact to its value/path. The type of the parameter value or the artifact path should be in accord with that declared in the sign. Type checking is implemented before and after the `execute` method.
+For an class OP, the structures of the inputs and outputs of an OP are declared in the static methods `get_input_sign` and `get_output_sign`. Each of them returns a dictionary mapping from the name of a parameter/artifact to its type. The execution of the OP is defined in the `execute` method. The types of the parameter values passed in and out should be in accord with those declared in the sign. Type checking is implemented before and after the `execute` method. For an input/output artifact, its sign should be like `Artifact(type)` where `type` can be `Path`, `List[Path]`, `Dict[str, Path]` or `dflow.python.NestedDict[Path]`. For input artifact, the `execute` method will receive a path, a list of paths or a dictionary of paths according to its sign . OP developer can directly process the file or directory at the path. For output artifact, the `execute` method should also return a path, a list of paths or a dictionary of paths according to its sign.
 
 ```python
 from dflow.python import OP, OPIO, OPIOSign, Artifact
 from pathlib import Path
 import shutil
 
 
@@ -184,335 +111,380 @@
         pass
 
     @classmethod
     def get_input_sign(cls):
         return OPIOSign(
             {
                 "msg": str,
-                "inp_art": Artifact(Path),
+                "foo": Artifact(Path),
             }
         )
 
     @classmethod
     def get_output_sign(cls):
         return OPIOSign(
             {
                 "msg": str,
-                "out_art": Artifact(Path),
+                "bar": Artifact(Path),
             }
         )
 
     @OP.exec_sign_check
     def execute(
         self,
         op_in: OPIO,
     ) -> OPIO:
-        shutil.copy(op_in["inp_art"], "bar.txt")
+        shutil.copy(op_in["foo"], "bar.txt")
         out_msg = op_in["msg"]
         op_out = OPIO(
             {
                 "msg": out_msg,
-                "out_art": Path("bar.txt"),
+                "bar": Path("bar.txt"),
             }
         )
         return op_out
 ```
-The above example defines an OP `SimpleExample`. The operation is to copy `foo.txt` to `bar.txt` and write the properties of the parameters with name msg to `msg.txt`. 
 
-One may also define OP using decorator `@OP.function` and Python Annotation as:
+The above example defines an OP `SimpleExample`. The operation is to copy the input artifact `foo` to output artifact `bar` and to copy the input parameter `msg` to output parameter `msg`.
+
+For an function OP, the structure of the inputs and outputs are declared in the type annotations more compactly and execution is defined in the function body. Type checking is implemented before and after the function as well. We recommend `python>=3.9` to use this syntax sugar. See more about Python Annotation at [Python official howtos](https://docs.python.org/3/howto/annotations.html).
 
 ```python
 from dflow.python import OP, Artifact
 from pathlib import Path
 import shutil
 
 @OP.function
 def SimpleExample(
 		msg: str,
-		inp_art: Artifact(Path),
-)->{"msg": str, "out_art": Artifact(Path),}:
-    shutil.copy(inp_art, "bar.txt")
+		foo: Artifact(Path),
+) -> {"msg": str, "bar": Artifact(Path)}:
+    shutil.copy(foo, "bar.txt")
     out_msg = msg
-    return {"msg": out_msg, "out_art": Path("bar.txt"),}
+    return {"msg": out_msg, "bar": Path("bar.txt")}
 ```
 
-We recommend `python>=3.9` to use this syntax sugar.
-See more about Python Annotation at [Python official howtos](https://docs.python.org/3/howto/annotations.html).
+To define an OP template from the above class or function, we need to specify the container image and other optional arguments to `PythonOPTemplate`. `pydflow` need not to be installed in this image because local `pydflow` package will be uploaded into the container by default
 
-To use the above class as a PythonOPTemplate, we need to pass the above class to `PythonOPTemplate` and specify the container image. Note that `pydflow` must be installed in this image
 ```python
 from dflow.python import PythonOPTemplate
 
 simple_example_templ = PythonOPTemplate(SimpleExample, image="python:3.8")
 ```
 
-An example using all the elements discussed in [1.3](#12-a-namecommonlayera-common-layer)  is shown here:
-- [PythonOP example](examples/test_python.py)
+An example is here
+- [Python OP example](examples/test_python.py)
 
-##  2. <a name='QuickStart'></a> Quick Start
-###  2.1. <a name='PrepareKubernetescluster'></a> Prepare Kubernetes cluster
-Firstly, you will need a Kubernetes cluster. To setup a Kubernetes cluster on your laptop, you can download the [Minikube](https://minikube.sigs.k8s.io) on your PC and make sure you have [Docker](https://www.docker.com/) up and running on you PC.
+####  1.2.3. <a name='Step'></a> Step
+`Step` is the central block for formulating rules of data flows. A step is the result of instantiating an OP template, where values of all input parameters and sources of all input artifacts declared in the OP template must be specified here. The input parameters/artifacts of a step may be either static at the time of submission, or dynamically from outputs of another step.
 
-After downloading, you can initiate the Kubernetes cluster using: 
-```
-minikube start 
-```
-###  2.2. <a name='SetupArgoWorkflows'></a> Setup [Argo Workflows](https://argoproj.github.io/argo-workflows/quick-start/)
-To get started quickly, you can use the quick start manifest. It will install Argo Workflow as well as some commonly used components:
-```
-kubectl create ns argo
-kubectl apply -n argo -f https://raw.githubusercontent.com/deepmodeling/dflow/master/manifests/quick-start-postgres.yaml
-```
-If you are running Argo Workflows locally (e.g. using Minikube or Docker for Desktop), open a port-forward so you can access the namespace:
-```
-kubectl -n argo port-forward deployment/argo-server 2746:2746 --address 0.0.0.0
-```
-This will serve the user interface on https://localhost:2746
+```python
+from dflow import Step
 
-For access to the minio object storage, open a port-forward for minio
+simple_example_step = Step(
+    name="step0",
+    template=simple_example_templ,
+    parameters={"msg": "HelloWorld!"},
+    artifacts={"inp_art": foo},
+)
+``` 
+
+Note that `foo` here is an artifact either uploaded from local or output of another step.
+
+
+####  1.2.4. <a name='Workflow'></a> Workflow
+`Workflow` connects blocks together to build a workflow. A simple serial workflow is created by adding steps in sequence. Adding a list of steps to a workflow means these steps running in parallel.
+
+```python
+from dflow import Workflow
+
+wf = Workflow(name="hello-world")
+wf.add(simple_example_step)
 ```
-kubectl -n argo port-forward deployment/minio 9000:9000 --address 0.0.0.0
+
+Submit a workflow by
+
+```python
+wf.submit()
 ```
 
-###  2.3. <a name='Installdflow'></a> Install dflow
+An example is here
+- [Workflow example](examples/test_steps.py)
+
+
+##  2. <a name='QuickStart'></a> Quick Start
+
+###  2.1. <a name='SetupArgoServer'></a> Setup Argo Server
+
+If you have an Argo server already, you can skip this step. Otherwise you can follow the [installation guide](tutorials/readme.md).
+
+###  2.2. <a name='Installdflow'></a> Install dflow
 Make sure your Python version is not less than 3.6 and install dflow
+
 ```
 pip install pydflow
 ```
 
-###  2.4. <a name='Runanexample'></a> Run an example
-Submit a simple workflow
+###  2.3. <a name='Runanexample'></a> Run an example
+There are several [notebook tutorials](tutorials/readme.md) that can help you start to use dflow. Besides, you can submit a simple workflow from the terminal
+
 ```
-python examples/test_steps.py
+python examples/test_python.py
 ```
-Then you can check the submitted workflow through argo's UI.
+
+Then you can check the submitted workflow through [argo's UI](https://127.0.0.1:2746).
 
 ##  3. <a name='UserGuide'></a> User Guide ([dflow-doc](https://deepmodeling.com/dflow/dflow.html))
-###  3.1. <a name='Commonlayer-1'></a> Common layer
+###  3.1. <a name='Commonlayer'></a> Common layer
 
 ####  3.1.1. <a name='Workflowmanagement'></a> Workflow management
 After submitting a workflow by `wf.submit()`, or getting a history workflow by `wf = Workflow(id="xxx")`, one can track its real-time status with APIs
 
 - `wf.id`: workflow ID in argo
 - `wf.query_status()`: query workflow status, return `"Pending"`, `"Running"`, `"Succeeded"`, etc.
 - `wf.query_step(name=None)`: query step by name (support for regex), return a list of argo step objects
     - `step.phase`: phase of a step, `"Pending"`, `"Running"`, `Succeeded`, etc.
     - `step.outputs.parameters`: a dictionary of output parameters
     - `step.outputs.artifacts`: a dictionary of output artifacts
 
 ####  3.1.2. <a name='Uploaddownloadartifact'></a> Upload/download artifact
-Dflow offers tools for uploading files to Minio and downloading files from Minio (default object storage in the quick start). User can upload a list of files or directories and get an artifact object, which can be used as argument of a step
+Dflow offers tools for uploading files to the artifact repository and downloading files from it (default artifact repository is Minio set up in the quick start). User can upload a file/directory, a list of files/directories or a dictionary of files/directories and get an artifact object, which can be used as argument of a step
+
 ```python
 artifact = upload_artifact([path1, path2])
 step = Step(
     ...
     artifacts={"foo": artifact}
 )
 ```
+
 User can also download the output artifact of a step queried from a workflow (to current directory for default)
+
 ```python
 step = wf.query_step(name="hello")
 download_artifact(step.outputs.artifacts["bar"])
 ```
-Modify `dflow.s3_config` to configure S3 globally.
+
+Modify `dflow.s3_config` to configure artifact repository settings globally.
 
 Note: dflow retains the relative path of the uploaded file/directory with respect to the current directory during uploading. If file/directory outside current directory is uploaded, its absolute path is used as the relative path in the artifact. If you want a different directory structure in the artifact with the local one, you can make soft links and then upload.
 
 ####  3.1.3. <a name='Steps'></a> Steps
-`Steps` is another kind of OP template which is defined by its constituent `step`s instead of a container. It can be seen as a sub-workflow or a super OP template consisting of some smaller OPs. `Steps` is a sequential array of concurrent `Step`. A simple example goes like `[[s00,s01],[s10,s11,s12]]`, where inner array represent concurrent tasks while outer array is sequential. Add a `step` to a `steps` just like for a `workflow`
+`Steps` is another kind of OP template which is defined by its constituent steps instead of a container. It can be seen as a sub-workflow or a super OP template consisting of some smaller OPs. A `steps` includes an array of arrays of `step`s, e.g. `[[s00,s01],[s10,s11,s12]]`, where inner array represent concurrent steps while outer array is sequential. One can declare input/output parameters/artifacts for a steps by
+
+```python
+steps.inputs.parameters["msg"] = InputParameter()
+steps.inputs.artifacts["foo"] = InputArtifact()
+steps.outputs.parameters["msg"] = OutputParameter()
+steps.outputs.parameters["bar"] = OutputArtifact()
+```
+
+
+Add a `step` to a `steps` just like for a `workflow`
+
 ```python
 steps.add(step)
 ```
-`Steps` can be used as the template to define a bigger `step`. Thus one can construct complex workflows of nested structure. One is also allowed to recursively use a `Steps` as the template of a building bloack inside it self to achieve dynamic loop.
+
+`steps` can be used as the template to instantiate a bigger `step` just like script OP templates. Thus one can construct complex workflows of nested structure. One is also allowed to recursively use a `steps` as the template of a building bloack inside it self to achieve dynamic loop.
+
+The output parameter of a `steps` can be set to come from a step of it by
+
+```python
+steps.outputs.parameters["msg"].value_from_parameter = step.outputs.parameters["msg"]
+```
+
+Here, `step` must be contained in `steps`. For assigning output artifact for a `steps`, use
+
+```python
+steps.outputs.artifacts["foo"]._from = step.outputs.parameters["foo"]
+```
 
 - [Recursive example](examples/test_recurse.py)
 
 ####  3.1.4. <a name='DAG'></a> DAG
-`DAG` is another kind of OP template which is defined by its constituent `task`s and their dependencies. The usage of `DAG` is similar to that of `steps`. To add a `task` to a `DAG`, use
+`DAG` is another kind of OP template which is defined by its constituent tasks and their dependencies. The usage of `DAG` is similar to that of `Steps`. To add a `task` to a `dag`, use
+
 ```python
 dag.add(task)
 ```
-The usage of `task` is also similar to that of `step`. Dflow will automatically detect dependencies among `task`s of a `DAG` (from input/output relations). Additional dependencies can be declared by
+
+The usage of `task` is also similar to that of `step`. Dflow will automatically detect dependencies among tasks of a `dag` (from input/output relations). Additional dependencies can be declared by
+
 ```python
 task_3 = Task(..., dependencies=[task_1, task_2])
 ```
 
 - [DAG example](examples/test_dag.py)
 
-####  3.1.5. <a name='OutputparametersandartifactsofSteps'></a> Output parameters and artifacts of Steps
-The output parameter of a `Steps` can be set to come from a step of it by `steps.outputs.parameters["msg"].value_from_parameter = step.outputs.parameters["msg"]`. Here, `step` must be contained in `steps`. For assigning output artifact for a `Steps`, use `steps.outputs.artifacts["foo"]._from = step.outputs.parameters["foo"]`.
+####  3.1.5. <a name='Conditionalstepparametersandartifacts'></a> Conditional step, parameters and artifacts
+Set a step to be conditional by `Step(..., when=expr)` where `expr` is an boolean expression in string format. Such as `"%s < %s" % (par1, par2)`. The step will be performed if the expression is evalutated to be true, otherwise skipped. The `when` argument is often used as the breaking condition of recursive steps. The output parameter of a `steps` (similar to `dag`) can be assigned as conditional by
 
-####  3.1.6. <a name='Conditionalstepparametersandartifacts'></a> Conditional step, parameters and artifacts
-Set a step to be conditional by `Step(..., when=expr)` where `expr` is an boolean expression in string format. Such as `"%s < %s" % (par1, par2)`. The `when` argument is often used as the breaking condition of recursive steps. The output parameter of a `Steps` can be assigned as optional by
 ```python
 steps.outputs.parameters["msg"].value_from_expression = if_expression(
     _if=par1 < par2,
     _then=par3,
     _else=par4
 )
 ```
-Similarly, the output artifact of a `Steps` can be assigned as optional by
+
+Similarly, the output artifact of a `steps` can be assigned as conditional by
+
 ```python
 steps.outputs.artifacts["foo"].from_expression = if_expression(
     _if=par1 < par2,
     _then=art1,
     _else=art2
 )
 ```
 
 - [Conditional outputs example](examples/test_conditional_outputs.py)
 
-####  3.1.7. <a name='Produceparallelstepsusingloop'></a> Produce parallel steps using loop
-`with_param` and `with_sequence` are 2 arguments of `Step` for automatically generating a list of parallel steps. These steps share a common OP template, and only differ in the input parameters.
+####  3.1.6. <a name='Produceparallelstepsusingloop'></a> Produce parallel steps using loop
+In scientific computing, it is often required to produce a list of parallel steps which share a common OP template, and only differ in the input parameters. `with_param` and `with_sequence` are 2 arguments of `Step` for automatically generating a list of parallel steps. These steps share a common OP template, and only differ in the input parameters.
 
 A step using `with_param` option generates parallel steps on a list (either a constant list or referring to another parameter, e.g. an output parameter of another step or an input parameter of the `steps` or `DAG` context), the parallelism equals to the length of the list. Each parallel step picks an item from the list by `"{{item}}"`, such as
+
 ```python
 step = Step(
     ...
     parameters={"msg": "{{item}}"},
     with_param=steps.inputs.parameters["msg_list"]
 )
 ```
+
 A step using `with_sequence` option generates parallel steps on a numeric sequence. `with_sequence` is usually used in coordination with `argo_sequence` which returns an Argo's sequence. For `argo_sequence`, the number at which to start the sequence is specified by `start` (default: 0). One can either specify the number of elements in the sequence by `count` or the number at which to end the sequence by `end`. The printf format string can be specified by `format` to format the value in the sequence. Each argument can be passed with a parameter, `argo_len` which returns the length of a list may be useful. Each parallel step picks an element from the sequence by `"{{item}}"`, such as
+
 ```python
 step = Step(
     ...
     parameters={"i": "{{item}}"},
     with_sequence=argo_sequence(argo_len(steps.inputs.parameters["msg_list"]))
 )
 ```
 
-####  3.1.8. <a name='Timeout'></a> Timeout
+####  3.1.7. <a name='Timeout'></a> Timeout
 Set the timeout of a step by `Step(..., timeout=t)`. The unit is second.
 
 - [Timeout example](examples/test_error_handling.py)
 
-####  3.1.9. <a name='Continueonfailed'></a> Continue on failed
+####  3.1.8. <a name='Continueonfailed'></a> Continue on failed
 Set the workflow to continue when a step fails by `Step(..., continue_on_failed=True)`.
 
 - [Continue on failed example](examples/test_error_handling.py)
 
-####  3.1.10. <a name='Continueonsuccessnumberratioofparallelsteps'></a> Continue on success number/ratio of parallel steps
-Set the workflow to continue when certain number/ratio of parallel steps succeed by `Step(..., continue_on_num_success=n)` or `Step(..., continue_on_success_ratio=r)`.
+####  3.1.9. <a name='Continueonsuccessnumberratioofparallelsteps'></a> Continue on success number/ratio of parallel steps
+For a group of parallel steps generated by `with_param` or `with_sequence`, set the workflow to continue when certain number/ratio of parallel steps succeed by `Step(..., continue_on_num_success=n)` or `Step(..., continue_on_success_ratio=r)`.
 
 - [Continue on success ratio example](examples/test_success_ratio.py)
 
-####  3.1.11. <a name='Optionalinputartifacts'></a> Optional input artifacts
+####  3.1.10. <a name='Optionalinputartifacts'></a> Optional input artifacts
 Set an input artifact to be optional by `op_template.inputs.artifacts["foo"].optional = True`.
 
-####  3.1.12. <a name='Defaultvalueforoutputparameters'></a> Default value for output parameters
+####  3.1.11. <a name='Defaultvalueforoutputparameters'></a> Default value for output parameters
 Set default value for an output parameter by `op_template.outputs.parameters["msg"].default = default_value`. The default value will be used when the expression in `value_from_expression` fails or the step is skipped.
 
-####  3.1.13. <a name='Keyofastep'></a> Key of a step
-You can set a key for a step by `Step(..., key="some-key")` for the convenience of locating the step. The key can be regarded as an input parameter which may contain reference of other parameters. For instance, the key of a step can change with iterations of a dynamic loop. Once key is assigned to a step, the step can be query by `wf.query_step(key="some-key")`. If the key is unique within the workflow, the `query_step` method returns a list consist of only one element.
+####  3.1.12. <a name='Keyofastep'></a> Key of a step
+One can assign a key for a step by `Step(..., key="some-key")` for the convenience of locating the step. The key can be regarded as an input parameter which may contain reference of other parameters. For instance, the key of a step can change with iterations of a dynamic loop. Once key is assigned to a step, the step can be query by `wf.query_step(key="some-key")`. If the key is unique within the workflow, the `query_step` method returns a list consist of only one element.
 
 - [Key of step example](examples/test_reuse.py)
 
-####  3.1.14. <a name='Resubmitaworkflow'></a> Resubmit a workflow
+####  3.1.13. <a name='Resubmitaworkflow'></a> Resubmit a workflow
 Workflows often have some steps that are expensive to compute. The outputs of previously run steps can be reused for submitting a new workflow. E.g. a failed workflow can be restarted from a certain point after some modification of the workflow template or even outputs of completed steps. For example, submit a workflow with reused steps by `wf.submit(reuse_step=[step0, step1])`. Here, `step0` and `step1` are previously run steps returned by `query_step` method. Before the new workflow runs a step, it will detect if there exists a reused step whose key matches that of the step about to run. If hit, the workflow will skip the step and set its outputs as those of the reused step. To modify outputs of a step before reusing, use `step0.modify_output_parameter(par_name, value)` for parameters and `step0.modify_output_artifact(art_name, artifact)` for artifacts.
 
 - [Reuse step example](examples/test_reuse.py)
 
-####  3.1.15. <a name='Executor'></a> Executor
-By default, for a "script step" (a step whose template is a script OP template), the Shell script or Python script runs in the container directly. Alternatively, one can modify the executor to run the script. Dflow offers an extension point for "script step" `Step(..., executor=my_executor)`. Here, `my_executor` should be an instance of class derived from `Executor`. A `Executor`-derived class should implement a method `render` which converts original template to a new template.
+####  3.1.14. <a name='Executor'></a> Executor
+For a "script step" (a step whose template is a script OP template), by default the Shell script or Python script runs in the container directly. Alternatively, one can modify the executor to run the script. Dflow offers an extension point for "script step" `Step(..., executor=my_executor)`. Here, `my_executor` should be an instance of class derived from the abstract class `Executor`. An implementation class of `Executor` should implement a method `render` which converts original template to a new template.
+
 ```python
-class Executor(object):
+class Executor(ABC):
+    @abc.abstractmethod
     def render(self, template):
         pass
 ```
-A context is similar to an executor, but assigned to a workflow `Workflow(context=...)` and affect every step.
-
-####  3.1.16. <a name='SubmitSlurmjobviaslurmexecutor'></a> Submit Slurm job via slurm executor
 
-`SlurmRemoteExecutor` is provided as an example of executor. The executor submits a slurm job to a remote host and synchronize its status and logs to the dflow step. The central logic of the executor is implemented in the Golang project [Dflow-extender](https://github.com/dptech-corp/dflow-extender). If you want to run a step on a slurm cluster remotely, do something like
-```python
-Step(
-    ...,
-    executor=SlurmRemoteExecutor(host="1.2.3.4",
-        username="myuser",
-        header="""#!/bin/bash
-                  #SBATCH -N 1
-                  #SBATCH -n 1
-                  #SBATCH -p cpu""")
-)
-```
-There are 3 options for SSH authentication, using password, specify path of private key file locally, or upload authorized private key to each node (or equivalently add each node to the authorized host list).
+A context is similar to an executor, but assigned to a workflow `Workflow(context=...)` and affect every step.
 
-- [Slurm executor example](examples/test_slurm.py)
+####  3.1.15. <a name='SubmitHPCBohriumjobviadispatcherplugin'></a> Submit HPC/Bohrium job via dispatcher plugin
 
-####  3.1.17. <a name='SubmitHPCjobviadispatcherplugin'></a> Submit HPC job via dispatcher plugin
+[DPDispatcher](https://github.com/deepmodeling/dpdispatcher) is a python package used to generate HPC scheduler systems (Slurm/PBS/LSF) or [Bohrium](https://bohrium.dp.tech) jobs input scripts and submit these scripts and poke until they finish. Dflow provides simple interface to invoke dispatcher as executor to complete script steps. E.g.
 
-[DPDispatcher](https://github.com/deepmodeling/dpdispatcher) is a python package used to generate HPC scheduler systems (Slurm/PBS/LSF) jobs input scripts and submit these scripts to HPC systems and poke until they finish. Dflow provides simple interface to invoke dispatcher as executor to complete script steps. E.g.
 ```python
 from dflow.plugins.dispatcher import DispatcherExecutor
 Step(
     ...,
     executor=DispatcherExecutor(host="1.2.3.4",
         username="myuser",
         queue_name="V100")
 )
 ```
+
 For SSH authentication, one can either specify path of private key file locally, or upload authorized private key to each node (or equivalently add each node to the authorized host list). For configuring extra [machine, resources or task parameters for dispatcher](https://docs.deepmodeling.com/projects/dpdispatcher/en/latest/), use `DispatcherExecutor(..., machine_dict=m, resources_dict=r, task_dict=t)`.
 
 - [Dispatcher executor example](examples/test_dispatcher.py)
 
-####  3.1.18. <a name='SubmitSlurmjobviavirtualnode'></a> Submit Slurm job via virtual node
+####  3.1.16. <a name='SubmitSlurmjobviavirtualnode'></a> Submit Slurm job via virtual node
 
 Following the installation steps in the [wlm-operator](https://github.com/dptech-corp/wlm-operator) project to add Slurm partitions as virtual nodes to Kubernetes (use manifests [configurator.yaml](manifests/configurator.yaml), [operator-rbac.yaml](manifests/operator-rbac.yaml), [operator.yaml](manifests/operator.yaml) in this project which modified some RBAC configurations)
 ```
 $ kubectl get nodes
 NAME                            STATUS   ROLES                  AGE    VERSION
 minikube                        Ready    control-plane,master   49d    v1.22.3
 slurm-minikube-cpu              Ready    agent                  131m   v1.13.1-vk-N/A
 slurm-minikube-dplc-ai-v100x8   Ready    agent                  131m   v1.13.1-vk-N/A
 slurm-minikube-v100             Ready    agent                  131m   v1.13.1-vk-N/A
 ```
 Then you can assign a step to be executed on a virtual node (i.e. submit a Slurm job to the corresponding partition to complete the step)
+
 ```python
 step = Step(
     ...
     executor=SlurmJobTemplate(
         header="#!/bin/sh\n#SBATCH --nodes=1",
         node_selector={"kubernetes.io/hostname": "slurm-minikube-v100"}
     )
 )
 ```
 
-####  3.1.19. <a name='UseresourcesinKubernetes'></a> Use resources in Kubernetes
+####  3.1.17. <a name='UseresourcesinKubernetes'></a> Use resources in Kubernetes
 
 A step can also be completed by a Kubernetes resource (e.g. Job or custom resources). At the beginning, a manifest is applied to Kubernetes. Then the status of the resource is monitered until the success condition or the failure condition is satisfied.
+
 ```python
-class Resource(object):
+class Resource(ABC):
     action = None
     success_condition = None
     failure_condition = None
-    def get_manifest(self, template):
+    @abc.abstractmethod
         pass
 ```
 
 - [Wlm example](examples/test_wlm.py)
 
-####  3.1.20. <a name='Importantnotevariablenames'></a> Important note: variable names
+####  3.1.18. <a name='Importantnotevariablenames'></a> Important note: variable names
 
 Dflow has following restrictions on variable names.
 
 | Variable name | Static/Dynamic | Restrictions | Example |
 | :------------ | -------------- | ------------ | ------- |
 | Workflow/OP template name | Static | Lowercase RFC 1123 subdomain (must consist of lower case alphanumeric characters, '-' or '.', and must start and end with an alphanumeric character | my-name |
 | Step/Task name | Static | Must consist of alpha-numeric characters or '-', and must start with an alpha-numeric character | My-name1-2, 123-NAME |
 | Parameter/Artifact name | Static | Must consist of alpha-numeric characters, '_' or '-' | my_param_1, MY-PARAM-1 |
 | Key name | Dynamic | Lowercase RFC 1123 subdomain (must consist of lower case alphanumeric characters, '-' or '.', and must start and end with an alphanumeric character | my-name |
 
-#### 3.1.21. <a name='DebugmodeDflowindependentofKubernetes'></a> Debug mode: dflow independent of Kubernetes
+####  3.1.19. <a name='DebugmodedflowindependentofKubernetes'></a> Debug mode: dflow independent of Kubernetes
 
 The debug mode is enabled by setting
+
 ```python
 from dflow import config
 config["mode"] = "debug"
 ```
+
 Before running a workflow locally, make sure that the dependencies of all OPs in the workflow are well-configured in the locally environment, unless the dispatcher executor is employed to submit jobs to some remote environments. The debug mode uses the current directory as the working directory by default. Each workflow will create a new directory there, whose structure will be like
 ```
 python-lsev6
 ├── status
 └── step-penf5
     ├── inputs
     │   ├── artifacts
@@ -535,18 +507,42 @@
     └── workdir
         ├── ...
 ```
 The top level contains the status and all steps of the workflow. The directory name for each step will be its key if provided, or generated from its name otherwise. The step directory contains the input/output parameters/artifacts, the type and the phase of the step. For a step of type "Pod", its directory also includes the script, the log file and the working directory for the step.
 
 - [Debug mode examples](examples/debug)
 
-###  3.2. <a name='Interfacelayer-1'></a> Interface layer
+####  3.1.20. <a name='Artifactstorageplugins'></a>Artifact storage plugins
+
+The default storage for artifacts in dflow is a Minio deployment in the Kubernetes cluster. While other artifact storages are supported (e.g. Aliyun OSS, Azure blob storage (ABS), Google cloud storage(GCS)). Dflow provides an extension point to use customized storage in the artifact management. A storage client is a class implementing 5 abstract methods, `upload`, `download`, `list`, `copy` and `get_md5` (optional), which offer the functionality of uploading file, downloading file, listing files with a particular prefix, copying file on the server side and getting the MD5 sum of file, respectively. Use a custom storage client object by configuring s3_config["storage_client"].
+
+```python
+class StorageClient(ABC):
+    @abc.abstractmethod
+    def upload(self, key: str, path: str) -> None:
+        pass
+    @abc.abstractmethod
+    def download(self, key: str, path: str) -> None:
+        pass
+    @abc.abstractmethod
+    def list(self, prefix: str, recursive: bool = False) -> List[str]:
+        pass
+    @abc.abstractmethod
+    def copy(self, src: str, dst: str) -> None:
+        pass
+    @abc.abstractmethod
+    def get_md5(self, key: str) -> str:
+        pass
+```
+
+###  3.2. <a name='Interfacelayer'></a> Interface layer
 
 ####  3.2.1. <a name='Slices'></a> Slices
-`Slices` helps user to slice input parameters/artifacts (which must be lists) to feed parallel steps and stack their output parameters/artifacts to lists in the same pattern. For example,
+In coordination with [parallel steps](#Produceparallelstepsusingloop), `Slices` helps user to slice input parameters/artifacts (which must be lists) to feed parallel steps and stack their output parameters/artifacts to lists in the same pattern. The Python OP only need to handle one slice. For example,
+
 ```python
 step = Step(name="parallel-tasks",
     template=PythonOPTemplate(
         ...,
         slices=Slices("{{item}}",
             input_parameter=["msg"],
             input_artifact=["data"],
@@ -557,19 +553,21 @@
     },
     artifacts={
         "data": data_list
     },
     with_param=argo_range(5)
 )
 ```
+
 In this example, each item in `msg_list` is passed to a parallel step as the input parameter `msg`, each part in `data_list` is passed to a parallel step as the input artifact `data`. Finally, the output artifacts `log` of all parallel steps are collected to one artifact `step.outputs.artifacts["log"]`.
 
 - [Slices example](examples/test_slices.py)
 
 It should be noticed that this feature by default passes full input artifacts to each parallel step which may only use some slices of these artifacts. In comparison, the subpath mode of slices only passes one single slice of the input artifacts to each parallel step. To use the subpath mode of slices,
+
 ```python
 step = Step(name="parallel-tasks",
     template=PythonOPTemplate(
         ...,
         slices=Slices(sub_path=True,
             input_parameter=["msg"],
             input_artifact=["data"],
@@ -578,36 +576,39 @@
     parameters = {
         "msg": msg_list
     },
     artifacts={
         "data": data_list
     })
 ```
+
 Here, the slice pattern (`{{item}}`) of `PythonOPTemplate` and the `with_param` argument of the `Step` need not to be set, because they are fixed in this mode. Each input parameter and artifact to be sliced must be of the same length, and the parallelism equals to this length. Another noticeable point is that in order to use the subpath of the artifacts, these artifacts must be saved without compression when they are generated. E.g. declare `Artifact(..., archive=None)` in the output signs of Python OP, or specify `upload_artifact(..., archive=None)` while uploading artifacts. Besides, one can use `dflow.config["archive_mode"] = None` to set default archive mode to no compression globally.
 
 - [Subpath mode of slices example](examples/test_subpath_slices.py)
 
 ####  3.2.2. <a name='Retryanderrorhandling'></a> Retry and error handling
-Dflow catches `TransientError` and `FatalError` thrown from `OP`. User can set maximum number of retries on `TransientError` by `PythonOPTemplate(..., retry_on_transient_error=n)`. Timeout error is regarded as fatal error for default. To treat timeout error as transient error, set `PythonOPTemplate(..., timeout_as_transient_error=True)`.
+Dflow catches `TransientError` and `FatalError` thrown from `OP`. User can set maximum number of retries on `TransientError` by `PythonOPTemplate(..., retry_on_transient_error=n)`. Timeout error is regarded as fatal error for default. To treat timeout error as transient error, set `PythonOPTemplate(..., timeout_as_transient_error=True)`. When a fatal error is raised or the retries on transient error reaches maximum retries, the step is considered as failed.
 
 - [Retry example](examples/test_error_handling.py)
 
 ####  3.2.3. <a name='Progress'></a> Progress
 A `OP` can update progress in the runtime so that user can track its real-time progress
+
 ```python
 class Progress(OP):
     progress_total = 100
     ...
     def execute(op_in):
         for i in range(10):
             self.progress_current = 10 * (i + 1)
             ...
 ```
 
 - [Progress example](examples/test_progress.py)
 
 ####  3.2.4. <a name='Uploadpythonpackagesfordevelopment'></a> Upload python packages for development
 To avoid frequently making image during development, dflow offers an interface to upload local packages into container and add them to `$PYTHONPATH`, such as `PythonOPTemplate(..., python_packages=["/opt/anaconda3/lib/python3.9/site-packages/numpy"])`. One can also globally specify packages to be uploaded, which will affect all `OP`s
+
 ```python
 from dflow.python import upload_packages
 upload_packages.append("/opt/anaconda3/lib/python3.9/site-packages/numpy")
 ```
```

### Comparing `pydflow-1.6.99/setup.py` & `pydflow-1.7.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,34 +10,38 @@
     name='pydflow',
     version=VERSION,
     description='Dflow is a Python framework for constructing scientific '
     'computing workflows employing Argo Workflows as the workflow engine.',
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author="Xinzijian Liu",
+    author_email="liuxzj@dp.tech",
+    url="https://github.com/deepmodeling/dflow",
     license="LGPLv3",
     package_dir={'': 'src'},
     packages=[
         "dflow",
         "dflow/python",
         "dflow/client",
         "dflow/plugins",
     ],
+    include_package_data=True,
     python_requires='>=3.6',
     install_requires=[
         "six",
         "python-dateutil",
         "urllib3",
         "certifi",
         "typeguard<3",
         "argo-workflows==5.0.0",
         "jsonpickle",
         "minio",
         "kubernetes",
         "pyyaml",
         "cloudpickle==2.2.0",
         "requests",
+        "tqdm",
     ],
     entry_points={
         'console_scripts': ['dflow=dflow.main:main'],
     },
 )
```

### Comparing `pydflow-1.6.99/src/dflow/__init__.py` & `pydflow-1.7.0/src/dflow/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 import os
+import logging
 from importlib import import_module
 
+from .argo_objects import ArgoStep, ArgoWorkflow
 from .common import LineageClient, LocalArtifact, S3Artifact
 from .config import config, s3_config, set_config, set_s3_config
 from .context import Context
 from .dag import DAG
-from .executor import Executor, RemoteExecutor
+from .executor import ContainerExecutor, Executor, RemoteExecutor
 from .io import (AutonamedDict, IfExpression, InputArtifact, InputParameter,
                  Inputs, OutputArtifact, OutputParameter, Outputs,
                  if_expression)
 from .op_template import (OPTemplate, PythonScriptOPTemplate, Secret,
                           ShellOPTemplate)
 from .resource import Resource
 from .slurm import SlurmJob, SlurmJobTemplate, SlurmRemoteExecutor
-from .step import (Step, argo_concat, argo_len, argo_range, argo_sequence,
-                   argo_sum)
+from .step import (Step, argo_concat, argo_enumerate, argo_len, argo_range,
+                   argo_sequence, argo_sum)
 from .steps import Steps
 from .task import Task
 from .utils import (copy_artifact, copy_s3, download_artifact, download_s3,
                     path_list_of_artifact, randstr, upload_artifact, upload_s3)
-from .workflow import (DockerSecret, Workflow, query_archived_workflows,
-                       query_workflows)
+from .workflow import (DockerSecret, Workflow, parse_repo,
+                       query_archived_workflows, query_workflows)
+
+log_level = os.environ.get('LOG_LEVEL')
+if log_level:
+    logging.basicConfig(level=getattr(logging, log_level.upper(), None))
 
 __all__ = ["S3Artifact", "DAG", "Executor", "RemoteExecutor", "AutonamedDict",
            "IfExpression", "InputArtifact", "InputParameter", "Inputs",
            "OutputArtifact", "OutputParameter", "Outputs",
            "if_expression", "OPTemplate", "PythonScriptOPTemplate",
            "ShellOPTemplate", "Resource", "SlurmJob", "SlurmJobTemplate",
            "SlurmRemoteExecutor", "Step", "argo_len", "argo_range",
            "argo_sequence", "Steps", "Task", "copy_artifact", "copy_s3",
            "download_artifact", "download_s3", "path_list_of_artifact",
            "s3_config", "upload_artifact", "upload_s3", "Workflow", "config",
            "Context", "randstr", "LocalArtifact", "set_config",
            "set_s3_config", "DockerSecret", "argo_sum", "argo_concat",
            "LineageClient", "Secret", "query_workflows",
-           "query_archived_workflows"]
+           "query_archived_workflows", "ContainerExecutor", "ArgoStep",
+           "ArgoWorkflow", "argo_enumerate"]
 
 
 def import_func(s):
     fields = s.split(".")
     if fields[0] == __name__ or fields[0] == "":
         fields[0] = ""
         mod = import_module(".".join(fields[:-1]), package=__name__)
@@ -48,7 +55,8 @@
 
 
 if os.environ.get("DFLOW_LINEAGE"):
     config["lineage"] = import_func(os.environ.get("DFLOW_LINEAGE"))()
 if os.environ.get("DFLOW_S3_STORAGE_CLIENT"):
     s3_config["storage_client"] = import_func(os.environ.get(
         "DFLOW_S3_STORAGE_CLIENT"))()
+parse_repo()
```

### Comparing `pydflow-1.6.99/src/dflow/argo_objects.py` & `pydflow-1.7.0/src/dflow/argo_objects.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/src/dflow/client/v1alpha1_artifact.py` & `pydflow-1.7.0/src/dflow/client/v1alpha1_artifact.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/src/dflow/client/v1alpha1_parameter.py` & `pydflow-1.7.0/src/dflow/client/v1alpha1_parameter.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/src/dflow/client/v1alpha1_retry_strategy.py` & `pydflow-1.7.0/src/dflow/client/v1alpha1_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/src/dflow/client/v1alpha1_sequence.py` & `pydflow-1.7.0/src/dflow/client/v1alpha1_sequence.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/src/dflow/client/v1alpha1_value_from.py` & `pydflow-1.7.0/src/dflow/client/v1alpha1_value_from.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/src/dflow/common.py` & `pydflow-1.7.0/src/dflow/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import abc
 import logging
+import os
+import shutil
 from abc import ABC
 from copy import copy, deepcopy
 from typing import Any, Dict, List, Union
 
 from .config import config as global_config
 from .config import s3_config
 
@@ -103,14 +105,30 @@
         if art.slice is None:
             art.slice = key
         else:
             art.slice = "%s.%s" % (art.slice, key)
         return art
 
 
+class HTTPArtifact:
+    def __init__(self, url):
+        self.url = url
+
+    def download(self, path="."):
+        os.makedirs(path, exist_ok=True)
+        file_path = os.path.join(path, os.path.basename(self.url))
+        import requests
+        sess = requests.session()
+        with sess.get(self.url, stream=True, verify=False) as req:
+            req.raise_for_status()
+            with open(file_path, 'w') as f:
+                shutil.copyfileobj(req.raw, f.buffer)
+        return file_path
+
+
 class LineageClient(ABC):
     @abc.abstractmethod
     def register_workflow(
             self,
             workflow_name: str) -> str:
         pass
 
@@ -131,7 +149,23 @@
             output_uris: Dict[str, str],
             workflow_urn: str) -> Dict[str, str]:
         pass
 
     @abc.abstractmethod
     def get_artifact_metadata(self, urn: str) -> object:
         pass
+
+
+class CustomArtifact(ABC):
+    @abc.abstractmethod
+    def get_urn(self) -> str:
+        pass
+
+    def __repr__(self):
+        return self.get_urn()
+
+    @abc.abstractmethod
+    def download(self, name: str, path: str):
+        pass
+
+    def render(self, template, name: str):
+        return template
```

### Comparing `pydflow-1.6.99/src/dflow/config.py` & `pydflow-1.7.0/src/dflow/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     "lineage": None,
     "register_tasks": boolize(os.environ.get("DFLOW_REGISTER_TASKS", False)),
     "http_headers": split_headers(os.environ.get("DFLOW_HTTP_HEADERS", {})),
     "workflow_annotations": json.loads(os.environ.get(
         "DFLOW_WORKFLOW_ANNOTATIONS", "{}")),
     "overwrite_reused_artifact": boolize(os.environ.get(
         "DFLOW_OVERWRITE_REUSED_ARTIFACT", True)),
+    "detach": boolize(os.environ.get("DFLOW_DETACH", False)),
 }
 
 
 def set_config(
     **kwargs,
 ) -> None:
     """
```

### Comparing `pydflow-1.6.99/src/dflow/context_syntax.py` & `pydflow-1.7.0/src/dflow/context_syntax.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/src/dflow/dag.py` & `pydflow-1.7.0/src/dflow/dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Optional, Dict, List, Union
 
 from .config import config, s3_config
 from .io import Inputs, Outputs
 from .op_template import OPTemplate
+from .step import add_slices
 from .task import Task
 
 try:
     from argo.workflows.client import (V1alpha1DAGTemplate, V1alpha1Metadata,
                                        V1alpha1Template)
 except Exception:
     pass
@@ -146,7 +147,10 @@
             else:
                 self.tasks[j].outputs = deepcopy(t.outputs)
             self.running.remove(self.tasks[j])
             self.finished.append(self.tasks[j])
             self.resolve()
 
         assert len(self.finished) == len(self.tasks), "cyclic graph"
+
+    def add_slices(self, slices, input_artifact_prefix=None):
+        add_slices(self, slices, input_artifact_prefix)
```

### Comparing `pydflow-1.6.99/src/dflow/executor.py` & `pydflow-1.7.0/src/dflow/executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,64 @@
+import abc
 import os
+from abc import ABC
 from copy import deepcopy
 from typing import List, Optional, Union
 
 from .common import S3Artifact
 from .config import config
 from .io import InputArtifact
-from .op_template import OPTemplate
+from .op_template import OPTemplate, ScriptOPTemplate
 from .utils import randstr, upload_s3
 
 try:
     from argo.workflows.client import (V1HostPathVolumeSource, V1Volume,
                                        V1VolumeMount)
 except Exception:
     pass
 
 
-class Executor(object):
+class Executor(ABC):
     """
     Executor
     """
-
+    @abc.abstractmethod
     def render(
             self,
             template: OPTemplate,
     ) -> OPTemplate:
         """
         render original template and return a new template, do not modify
         self in this method to make the executor reusable
         """
         raise NotImplementedError()
 
 
-def run_script(image, cmd, docker=None, singularity=None, podman=None):
+def run_script(image, cmd, docker=None, singularity=None, podman=None,
+               image_pull_policy=None):
     if docker is not None:
-        return "%s pull %s && %s run -v$(pwd)/tmp:/tmp "\
+        if image_pull_policy is None:
+            if image.split(":")[-1] == "latest":
+                image_pull_policy = "Always"
+            else:
+                image_pull_policy = "IfNotPresent"
+        script = ""
+        if image_pull_policy == "Always":
+            script += "%s pull %s && " % (docker, image)
+        elif image_pull_policy == "IfNotPresent":
+            script += "if [ $(docker images %s | wc -l) -lt 2 ]; " % image
+            script += "then %s pull %s; fi && " % (docker, image)
+        return script + "%s run -v$(pwd)/tmp:/tmp "\
             "-v$(pwd)/script:/script %s %s /script" % (
-                docker, image, docker, image, " ".join(cmd))
+                docker, image, " ".join(cmd))
     elif singularity is not None:
-        return "%s pull image.sif %s && %s run -B$(pwd)/tmp:/tmp "\
+        return "if [ -f %s ]; then rm -f image.sif && ln -s %s image.sif; "\
+            "else %s pull image.sif %s; fi && %s run -B$(pwd)/tmp:/tmp "\
             "-B$(pwd)/script:/script image.sif %s /script && rm image.sif" % (
-                singularity, image, singularity, " ".join(cmd))
+                image, image, singularity, image, singularity, " ".join(cmd))
     elif podman is not None:
         return "%s pull %s && %s run -v$(pwd)/tmp:/tmp "\
             "-v$(pwd)/script:/script %s %s /script" % (
                 podman, image, podman, image, " ".join(cmd))
     else:
         return "%s script" % " ".join(cmd)
 
@@ -54,14 +69,59 @@
         tmp_template.tmp_root = tmp_root
         tmp_template.render_script()
         return tmp_template.script
     else:
         return template.script.replace("/tmp", tmp_root)
 
 
+class ContainerExecutor(Executor):
+    def __init__(
+            self,
+            docker: Optional[str] = None,
+            singularity: Optional[str] = None,
+            podman: Optional[str] = None,
+            image_pull_policy: Optional[str] = None,
+    ):
+        self.docker = docker
+        self.singularity = singularity
+        self.podman = podman
+        self.image_pull_policy = image_pull_policy
+
+    def render(self, template):
+        if not isinstance(template, ScriptOPTemplate):
+            return template
+
+        new_template = deepcopy(template)
+        new_template.name += "-" + randstr()
+        script = "cat <<'EOF'> script\n" + template.script + "\nEOF\n"
+        prep_script = "import os, shutil\n"
+        prep_script += "for dn, ds, fs in os.walk('tmp'):\n"
+        prep_script += "    for d in ds:\n"
+        prep_script += "        d = os.path.join(dn, d)\n"
+        prep_script += "        if os.path.islink(d):\n"
+        prep_script += "            src = os.path.realpath(d)\n"
+        prep_script += "            os.remove(d)\n"
+        prep_script += "            shutil.copytree(src, d, copy_function="\
+            "os.link)\n"
+        prep_script += "    for f in fs:\n"
+        prep_script += "        f = os.path.join(dn, f)\n"
+        prep_script += "        if os.path.islink(f):\n"
+        prep_script += "            src = os.path.realpath(f)\n"
+        prep_script += "            os.remove(f)\n"
+        prep_script += "            os.link(src, f)\n"
+        script += "cat <<'EOF' | python3\n" + prep_script + "\nEOF\n"
+        script += run_script(template.image, template.command, self.docker,
+                             self.singularity, self.podman,
+                             self.image_pull_policy)
+        new_template.command = ["sh"]
+        new_template.script = script
+        new_template.script_rendered = True
+        return new_template
+
+
 class RemoteExecutor(Executor):
     def __init__(
             self,
             host: str,
             port: int = 22,
             username: str = "root",
             password: Optional[str] = None,
@@ -220,8 +280,9 @@
                 source=private_key_artifact, mode=0o600)
         else:
             new_template.volumes.append(V1Volume(
                 name="dflow-private-key", host_path=V1HostPathVolumeSource(
                     path=config["private_key_host_path"])))
             new_template.mounts.append(V1VolumeMount(
                 name="dflow-private-key", mount_path="/root/.ssh"))
+        new_template.script_rendered = True
         return new_template
```

### Comparing `pydflow-1.6.99/src/dflow/io.py` & `pydflow-1.7.0/src/dflow/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import tempfile
 from collections import UserDict
 from copy import copy, deepcopy
 from typing import Any, Dict, List, Optional, Union
 
 import jsonpickle
 
-from .common import S3Artifact
+from .common import CustomArtifact, S3Artifact
 from .config import config
 from .utils import randstr, s3_config, upload_s3
 
 try:
     from argo.workflows.client import (V1alpha1ArchiveStrategy, V1alpha1Inputs,
                                        V1alpha1Outputs, V1alpha1RawArtifact)
 
@@ -262,20 +262,43 @@
         if config["mode"] == "debug":
             return ArgoVar("%s >= %s" % (self.expr, to_expr(other)))
         if isinstance(other, ArgoVar):
             other = "asFloat(%s)" % other.expr
         return ArgoVar("asFloat(%s) >= %s" % (self.expr, other))
 
     def __add__(self, other):
+        if isinstance(other, str):
+            return ArgoVar("%s + '%s'" % (self.expr, other))
         if config["mode"] == "debug":
             return ArgoVar("%s + %s" % (self.expr, to_expr(other)))
         if isinstance(other, ArgoVar):
             other = "asFloat(%s)" % other.expr
         return ArgoVar("asFloat(%s) + %s" % (self.expr, other))
 
+    def __sub__(self, other):
+        if config["mode"] == "debug":
+            return ArgoVar("%s - %s" % (self.expr, to_expr(other)))
+        if isinstance(other, ArgoVar):
+            other = "asFloat(%s)" % other.expr
+        return ArgoVar("asFloat(%s) - %s" % (self.expr, other))
+
+    def __mul__(self, other):
+        if config["mode"] == "debug":
+            return ArgoVar("%s * %s" % (self.expr, to_expr(other)))
+        if isinstance(other, ArgoVar):
+            other = "asFloat(%s)" % other.expr
+        return ArgoVar("asFloat(%s) * %s" % (self.expr, other))
+
+    def __truediv__(self, other):
+        if config["mode"] == "debug":
+            return ArgoVar("%s / %s" % (self.expr, to_expr(other)))
+        if isinstance(other, ArgoVar):
+            other = "asFloat(%s)" % other.expr
+        return ArgoVar("asFloat(%s) / %s" % (self.expr, other))
+
 
 class IfExpression(ArgoVar, Expression):
     def __init__(
             self,
             _if: Union[str, ArgoVar],
             _then: Union[str, ArgoVar],
             _else: Union[str, ArgoVar],
@@ -336,33 +359,34 @@
         self.access_modes = access_modes
 
 
 def convert_value_to_str(value):
     if isinstance(value, str):
         return value
 
-    s = jsonpickle.dumps(value)
-
     def handle(obj):
-        nonlocal s
-        if isinstance(obj, dict):
-            if "py/object" in obj and obj["py/object"] == "dflow.io.ArgoVar":
-                s = s.replace(json.dumps(obj), "{{=%s}}" % obj["expr"])
-                return
-            for v in obj.values():
-                if isinstance(v, (dict, list)):
-                    handle(v)
-        elif isinstance(obj, list):
-            for v in obj:
-                if isinstance(v, (dict, list)):
+        # TODO: Only support dict and list
+        if isinstance(obj, (dict, list)):
+            for i, v in obj.items() if isinstance(obj, dict) \
+                    else enumerate(obj):
+                if isinstance(v, ArgoVar):
+                    obj[i] = "dflow_placeholder_%s" % len(vars)
+                    if (hasattr(v, "type") and v.type == str) or (
+                            hasattr(v, "value") and isinstance(v.value, str)):
+                        vars.append("\"{{=%s}}\"" % v.expr)
+                    else:
+                        vars.append("{{=%s}}" % v.expr)
+                elif isinstance(v, (dict, list)):
                     handle(v)
 
-    if "dflow.io.ArgoVar" in s:
-        d = json.loads(s)
-        handle(d)
+    vars = []
+    handle(value)
+    s = jsonpickle.dumps(value)
+    for i, var in enumerate(vars):
+        s = s.replace("\"dflow_placeholder_%s\"" % i, var)
 
     return s
 
 
 class InputParameter(ArgoVar):
     """
     Input parameter for OP template
@@ -392,14 +416,16 @@
         if "value" in kwargs:
             self.value = kwargs["value"]
         self.save_as_artifact = save_as_artifact
         if config["mode"] == "debug":
             self.save_as_artifact = False
         self.path = path
         self.source = source
+        for k, v in kwargs.items():
+            self.__setattr__(k, v)
 
     @classmethod
     def from_dict(cls, d):
         kwargs = {
             "name": d.get("name", None),
             "type": str if json.loads(d.get("description", "{}")).get(
                 "type", str(str)) == str(str) else None,
@@ -529,43 +555,48 @@
             optional: bool = False,
             type: Optional[Any] = None,
             source: Union[str, "InputArtifact",
                           "OutputArtifact", S3Artifact] = None,
             mode: Optional[int] = None,
             sub_path: Optional[str] = None,
             archive: str = "default",
+            save_as_parameter: bool = False,
+            **kwargs,
     ) -> None:
         self.path = path
         self.name = name
         self.step = step
         self.template = template
         self.optional = optional
         self.type = type
         self.source = source
         self._sub_path = None
         self.mode = mode
-        self.sub_path = sub_path
+        self.sp = sub_path
         self.archive = archive
         self.slice = None
         self.parent = None
+        self.save_as_parameter = save_as_parameter
+        for k, v in kwargs.items():
+            self.__setattr__(k, v)
 
     @classmethod
     def from_dict(cls, d):
         kwargs = {
             "name": d.get("name", None),
             "path": d.get("path", None),
             "optional": d.get("optional", None),
             "mode": d.get("mode", None),
             "sub_path": d.get("subPath", None),
             "archive": None if "none" in d.get("archive", {}) else "tar",
         }
         if "s3" in d:
             kwargs["source"] = S3Artifact(key=d["s3"]["key"])
         if "oss" in d:
-            kwargs["source"] = S3Artifact(key=d["oss"]["key"]).oss()
+            kwargs["source"] = S3Artifact(key=d["oss"]["key"])
         return cls(**kwargs)
 
     def __getitem__(self, key):
         art = copy(self)
         art.parent = self
         if art.slice is None:
             art.slice = key
@@ -586,66 +617,92 @@
                             (self.step.id, self.name)
                 return "inputs.artifacts['%s']" % self.name
             return ""
         return super().__getattr__(key)
 
     def __repr__(self):
         from .task import Task
+        if self.save_as_parameter:
+            if self.name is not None:
+                if self.step is not None:
+                    if isinstance(self.step, Task):
+                        return "{{tasks.%s.inputs.parameters.dflow_art_%s}}"\
+                            % (self.step.id, self.name)
+                    else:
+                        return "{{steps.%s.inputs.artifacts.dflow_art_%s}}"\
+                            % (self.step.id, self.name)
+                return "{{inputs.artifacts.dflow_art_%s}}" % self.name
+            return ""
         if self.name is not None:
             if self.step is not None:
                 if isinstance(self.step, Task):
                     return "{{tasks.%s.inputs.artifacts.%s}}" % (self.step.id,
                                                                  self.name)
                 else:
                     return "{{steps.%s.inputs.artifacts.%s}}" % (self.step.id,
                                                                  self.name)
             return "{{inputs.artifacts.%s}}" % self.name
         return ""
 
     def sub_path(self, path):
         artifact = deepcopy(self)
-        artifact._sub_path = path
+        if artifact._sub_path is None:
+            artifact._sub_path = path
+        else:
+            artifact._sub_path += "/" + path
         return artifact
 
     def get_path_list_parameter(self):
         return self.template.inputs.parameters["dflow_%s_path_list" %
                                                self.name]
 
     def get_urn_parameter(self):
         return self.template.inputs.parameters["dflow_%s_urn" % self.name]
 
     def convert_to_argo(self):
+        if self.save_as_parameter:
+            if self.source is None:
+                return V1alpha1Parameter(name="dflow_art_%s" % self.name)
+            elif isinstance(self.source, CustomArtifact):
+                return V1alpha1Parameter(name="dflow_art_%s" % self.name,
+                                         value=jsonpickle.dumps(self.source))
+            else:
+                return V1alpha1Parameter(name="dflow_art_%s" % self.name,
+                                         value=str(self.source))
+
         archive = None
         if self.archive is None:
             archive = V1alpha1ArchiveStrategy(_none={})
         if self.path in NotAllowedInputArtifactPath:
             raise RuntimeError(
                 "Path [%s] is not allowed for input artifact" % self.path)
         if self.source is None:
             return V1alpha1Artifact(name=self.name, path=self.path,
                                     optional=self.optional, mode=self.mode,
                                     archive=archive)
         if isinstance(self.source, (InputArtifact, OutputArtifact)):
-            sub_path = self.sub_path if self.sub_path is not None else \
+            sub_path = self.sp if self.sp is not None else \
                 self.source._sub_path
+            if isinstance(sub_path, ArgoVar):
+                sub_path = "{{=%s}}" % sub_path.expr
             return V1alpha1Artifact(name=self.name, path=self.path,
                                     optional=self.optional,
                                     _from=str(self.source), sub_path=sub_path,
                                     mode=self.mode, archive=archive)
         elif isinstance(self.source, S3Artifact):
             if s3_config["repo_type"] == "s3":
                 return V1alpha1Artifact(name=self.name, path=self.path,
                                         optional=self.optional, s3=self.source,
-                                        sub_path=self.sub_path, mode=self.mode,
+                                        sub_path=self.sp, mode=self.mode,
                                         archive=archive)
             else:
                 return V1alpha1Artifact(name=self.name, path=self.path,
                                         optional=self.optional,
                                         oss=self.source.oss(),
-                                        sub_path=self.sub_path, mode=self.mode,
+                                        sub_path=self.sp, mode=self.mode,
                                         archive=archive)
         elif isinstance(self.source, str):
             return V1alpha1Artifact(name=self.name, path=self.path,
                                     optional=self.optional,
                                     raw=V1alpha1RawArtifact(data=self.source),
                                     mode=self.mode, archive=archive)
         else:
@@ -968,15 +1025,18 @@
             art.slice = key
         else:
             art.slice = "%s.%s" % (art.slice, key)
         return art
 
     def sub_path(self, path):
         artifact = deepcopy(self)
-        artifact._sub_path = path
+        if artifact._sub_path is None:
+            artifact._sub_path = path
+        else:
+            artifact._sub_path += "/" + path
         return artifact
 
     def __getattr__(self, key):
         from .task import Task
         if key == "expr":
             if self.redirect is not None:
                 return self.redirect.expr
@@ -1172,15 +1232,18 @@
         artifacts = []
         for par in self.parameters.values():
             if par.save_as_artifact:
                 artifacts.append(par.convert_to_argo())
             else:
                 parameters.append(par.convert_to_argo())
         for art in self.artifacts.values():
-            artifacts.append(art.convert_to_argo())
+            if art.save_as_parameter:
+                parameters.append(art.convert_to_argo())
+            else:
+                artifacts.append(art.convert_to_argo())
         return V1alpha1Inputs(parameters=parameters, artifacts=artifacts)
 
 
 class Outputs:
     """
     Outputs for OP template
```

### Comparing `pydflow-1.6.99/src/dflow/main.py` & `pydflow-1.7.0/src/dflow/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import datetime
 from typing import List, Optional
 
-from dflow import (S3Artifact, Workflow, download_artifact, query_workflows,
-                   upload_artifact)
+from dflow import (S3Artifact, Workflow, config, download_artifact,
+                   query_workflows, upload_artifact)
 
 
 def main_parser():
     parser = argparse.ArgumentParser(
         description="dflow: a Python framework for constructing scientific "
         "computing workflows",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -224,14 +224,20 @@
 
     parser_submit = subparsers.add_parser(
         "submit",
         help="Submit a workflow from a YAML file",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser_submit.add_argument("FILE", help="the YAML file")
+    parser_submit.add_argument(
+        "-d",
+        "--detach",
+        action="store_true",
+        help="detach mode for running workflow",
+    )
     return parser
 
 
 def parse_args(args: Optional[List[str]] = None):
     """Commandline options argument parsing.
 
     Parameters
@@ -433,12 +439,14 @@
             description=args.description, tags=tags, properties=properties)
         print("Storage key: %s" % art.key)
         if art.urn:
             print("Dataset URN: %s" % art.urn)
     elif args.command == "submit":
         with open(args.FILE, "r") as f:
             wf = Workflow.from_yaml(f.read())
+        if args.detach:
+            config["detach"] = True
         wf.submit()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pydflow-1.6.99/src/dflow/op_template.py` & `pydflow-1.7.0/src/dflow/op_template.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from copy import deepcopy
 from typing import Dict, List, Optional, Union
 
 from .config import config as global_config
 from .config import s3_config
 from .io import PVC, InputParameter, Inputs, OutputParameter, Outputs
 from .utils import randstr
@@ -216,14 +217,15 @@
             retry_strategy: Optional[V1alpha1RetryStrategy] = None,
             resource: Optional[V1alpha1ResourceTemplate] = None,
             image_pull_policy: Optional[str] = None,
             requests: Dict[str, str] = None,
             limits: Dict[str, str] = None,
             envs: Dict[str, Union[str, Secret, V1EnvVarSource]] = None,
             init_containers: Optional[List[V1alpha1UserContainer]] = None,
+            sidecars: Optional[List[V1alpha1UserContainer]] = None,
     ) -> None:
         super().__init__(name=name, inputs=inputs, outputs=outputs,
                          memoize_key=memoize_key, pvcs=pvcs,
                          annotations=annotations)
         self.image = image
         if isinstance(command, str):
             command = [command]
@@ -239,15 +241,21 @@
         self.timeout = timeout
         self.retry_strategy = retry_strategy
         self.resource = resource
         self.image_pull_policy = image_pull_policy
         self.requests = requests
         self.limits = limits
         self.envs = envs
+        if init_containers is None:
+            init_containers = []
         self.init_containers = init_containers
+        if sidecars is None:
+            sidecars = []
+        self.sidecars = sidecars
+        self.script_rendered = False
 
     @classmethod
     def from_dict(cls, d):
         kwargs = {
             "name": d.get("name", None),
             "inputs": Inputs.from_dict(d.get("inputs", {})),
             "outputs": Outputs.from_dict(d.get("outputs", {})),
@@ -268,15 +276,48 @@
             "requests": d.get("script", {}).get("resources", {}).get(
                 "requests", None),
             "limits": d.get("script", {}).get("resources", {}).get(
                 "limits", None),
             "envs": {env.name: env.value for env in d.get("script", {}).get(
                 "env", [])},
             "init_containers": d.get("initContainers", None),
+            "sidecars": d.get("sidecars", None),
         }
+        engine = d.get("metadata", {}).get("annotations", {}).get(
+            "workflow.dp.tech/container_engine")
+        docker = "docker" if engine == "docker" else None
+        singularity = "singularity" if engine == "singularity" else None
+        podman = "podman" if engine == "podman" else None
+        if d.get("metadata", {}).get("annotations", {}).get(
+                "workflow.dp.tech/executor") == "dispatcher":
+            host = kwargs["annotations"].get("workflow.dp.tech/host")
+            port = kwargs["annotations"].get("workflow.dp.tech/port", 22)
+            username = kwargs["annotations"].get(
+                "workflow.dp.tech/username", "root")
+            password = kwargs["annotations"].get("workflow.dp.tech/password")
+            queue_name = kwargs["annotations"].get(
+                "workflow.dp.tech/queue_name")
+            extras = kwargs["annotations"].get("workflow.dp.tech/extras")
+            extras = json.loads(extras) if extras else {}
+            machine = extras.get("machine", None)
+            resources = extras.get("resources", None)
+            task = extras.get("task", None)
+            clean = extras.get("clean", True)
+            from .plugins.dispatcher import DispatcherExecutor
+            executor = DispatcherExecutor(
+                host, queue_name, port, username, password,
+                machine_dict=machine, resources_dict=resources,
+                task_dict=task, docker_executable=docker,
+                singularity_executable=singularity, podman_executable=podman,
+                clean=clean)
+            return executor.render(cls(**kwargs))
+        elif engine:
+            from .executor import ContainerExecutor
+            executor = ContainerExecutor(docker, singularity, podman)
+            return executor.render(cls(**kwargs))
         return cls(**kwargs)
 
     def convert_to_argo(self, memoize_prefix=None,
                         memoize_configmap="dflow"):
         self.handle_key(memoize_prefix, memoize_configmap)
         self.annotations["workflows.argoproj.io/progress"] = self.init_progress
         if self.resource is not None:
@@ -287,14 +328,15 @@
                                     outputs=self.outputs.convert_to_argo(),
                                     timeout=self.timeout,
                                     retry_strategy=self.retry_strategy,
                                     memoize=self.memoize,
                                     volumes=self.volumes,
                                     resource=self.resource,
                                     init_containers=self.init_containers,
+                                    sidecars=self.sidecars,
                                     )
         else:
             if self.envs is not None:
                 env = []
                 for k, v in self.envs.items():
                     if isinstance(v, V1EnvVarSource):
                         env.append(V1EnvVar(name=k, value_from=v))
@@ -329,14 +371,15 @@
                                      command=self.command, source=self.script,
                                      volume_mounts=self.mounts,
                                      resources=V1ResourceRequirements(
                                          limits=self.limits,
                                          requests=self.requests),
                                      env=env),
                                  init_containers=self.init_containers,
+                                 sidecars=self.sidecars,
                                  archive_location=loc,
                                  )
 
 
 class ShellOPTemplate(ScriptOPTemplate):
     """
     Shell script OP template
@@ -357,14 +400,15 @@
         pvcs: PVCs need to be declared
         image_pull_policy: Always, IfNotPresent, Never
         annotations: annotations for the OP template
         requests: a dict of resource requests
         limits: a dict of resource limits
         envs: environment variables
         init_containers: init containers before the template runs
+        sidecars: sidecar containers
     """
 
     def __init__(
         self,
         name: Optional[str] = None,
         inputs: Optional[Inputs] = None,
         outputs: Optional[Outputs] = None,
@@ -380,25 +424,26 @@
         timeout: Optional[str] = None,
         retry_strategy: Optional[V1alpha1RetryStrategy] = None,
         image_pull_policy: Optional[str] = None,
         requests: Dict[str, str] = None,
         limits: Dict[str, str] = None,
         envs: Dict[str, str] = None,
         init_containers: Optional[List[V1alpha1UserContainer]] = None,
+        sidecars: Optional[List[V1alpha1UserContainer]] = None,
     ) -> None:
         if command is None:
             command = ["sh"]
         super().__init__(
             name=name, inputs=inputs, outputs=outputs, image=image,
             command=command, script=script, volumes=volumes, mounts=mounts,
             init_progress=init_progress, timeout=timeout,
             retry_strategy=retry_strategy, memoize_key=memoize_key, pvcs=pvcs,
             image_pull_policy=image_pull_policy, annotations=annotations,
             requests=requests, limits=limits, envs=envs,
-            init_containers=init_containers,
+            init_containers=init_containers, sidecars=sidecars,
         )
 
 
 class PythonScriptOPTemplate(ScriptOPTemplate):
     """
     Python script OP template
 
@@ -418,14 +463,15 @@
         pvcs: PVCs need to be declared
         image_pull_policy: Always, IfNotPresent, Never
         annotations: annotations for the OP template
         requests: a dict of resource requests
         limits: a dict of resource limits
         envs: environment variables
         init_containers: init containers before the template runs
+        sidecars: sidecar containers
     """
 
     def __init__(
         self,
         name: Optional[str] = None,
         inputs: Optional[Inputs] = None,
         outputs: Optional[Outputs] = None,
@@ -441,25 +487,26 @@
         timeout: Optional[str] = None,
         retry_strategy: Optional[V1alpha1RetryStrategy] = None,
         image_pull_policy: Optional[str] = None,
         requests: Dict[str, str] = None,
         limits: Dict[str, str] = None,
         envs: Dict[str, str] = None,
         init_containers: Optional[List[V1alpha1UserContainer]] = None,
+        sidecars: Optional[List[V1alpha1UserContainer]] = None,
     ) -> None:
         if command is None:
             command = ["python3"]
         super().__init__(
             name=name, inputs=inputs, outputs=outputs, image=image,
             command=command, script=script, volumes=volumes, mounts=mounts,
             init_progress=init_progress, timeout=timeout,
             retry_strategy=retry_strategy, memoize_key=memoize_key, pvcs=pvcs,
             image_pull_policy=image_pull_policy, annotations=annotations,
             requests=requests, limits=limits, envs=envs,
-            init_containers=init_containers,
+            init_containers=init_containers, sidecars=sidecars,
         )
 
 
 class ContainerOPTemplate(ScriptOPTemplate):
     def __init__(
             self,
             command: Union[str, List[str]] = "",
@@ -497,9 +544,10 @@
             "requests": d.get("container", {}).get("resources", {}).get(
                 "requests", None),
             "limits": d.get("container", {}).get("resources", {}).get(
                 "limits", None),
             "envs": {env.name: env.value for env in d.get("container", {}).get(
                 "env", [])},
             "init_containers": d.get("initContainers", None),
+            "sidecars": d.get("sidecars", None),
         }
         return cls(**kwargs)
```

### Comparing `pydflow-1.6.99/src/dflow/plugins/bohrium.py` & `pydflow-1.7.0/src/dflow/plugins/bohrium.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,15 @@
         new_template.script = render_script_with_tmp_root(template,
                                                           "$(pwd)/tmp")
         if isinstance(template, ShellOPTemplate):
             new_template.script = "mkdir -p tmp\n" + new_template.script
         if isinstance(template, PythonScriptOPTemplate):
             new_template.script = "import os\nos.makedirs('tmp', "\
                 "exist_ok=True)\n" + new_template.script
+        new_template.script_rendered = True
         return new_template
 
 
 class BohriumContext(Context):
     """
     Bohrium context
 
@@ -203,14 +204,15 @@
                                                                   "$(pwd)/tmp")
                 if isinstance(template, ShellOPTemplate):
                     new_template.script = "mkdir -p tmp\n" + \
                         new_template.script
                 if isinstance(template, PythonScriptOPTemplate):
                     new_template.script = "import os\nos.makedirs('tmp', "\
                         "exist_ok=True)\n" + new_template.script
+                new_template.script_rendered = True
             return new_template
 
         return template
 
 
 class TiefblueClient(StorageClient):
     def __init__(
```

### Comparing `pydflow-1.6.99/src/dflow/plugins/dispatcher.py` & `pydflow-1.7.0/src/dflow/plugins/dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import abc
 import json
 import os
+from abc import ABC
 from copy import deepcopy
+from getpass import getpass
 from typing import List, Optional, Union
 
-from ..common import S3Artifact
+from ..common import CustomArtifact, S3Artifact
 from ..config import config
 from ..executor import Executor, render_script_with_tmp_root, run_script
 from ..io import InputArtifact, InputParameter
 from ..op_template import ScriptOPTemplate
+from ..python import PythonOPTemplate
 from ..utils import randstr, upload_s3
 from . import bohrium
 
 try:
     from argo.workflows.client import (V1HostPathVolumeSource, V1Volume,
                                        V1VolumeMount)
 except Exception:
@@ -47,15 +51,15 @@
         task_dict: task config for dispatcher
         json_file: JSON file containing machine and resources config
         docker_executable: docker executable to run remotely
         singularity_executable: singularity executable to run remotely
         podman_executable: podman executable to run remotely
         remote_root: remote root path for working
         retry_on_submission_error: max retries on submission error
-        merge_sliced_step: handle multi slices in one dispatcher job
+        merge_sliced_step: handle multi slices in a single dispatcher job
     """
 
     def __init__(self,
                  host: Optional[str] = None,
                  queue_name: Optional[str] = None,
                  port: int = 22,
                  username: str = "root",
@@ -72,14 +76,17 @@
                  json_file: Optional[os.PathLike] = None,
                  docker_executable: Optional[str] = None,
                  singularity_executable: Optional[str] = None,
                  podman_executable: Optional[str] = None,
                  remote_root: Optional[str] = None,
                  retry_on_submission_error: Optional[int] = None,
                  merge_sliced_step: bool = False,
+                 pre_script: str = "",
+                 post_script: str = "",
+                 clean: bool = True,
                  ) -> None:
         self.host = host
         self.queue_name = queue_name
         self.port = port
         self.username = username
         self.password = password
         self.private_key_file = private_key_file
@@ -106,14 +113,17 @@
         if config["mode"] == "debug":
             self.work_root = "."
         else:
             self.work_root = "/"
         self.remote_root = remote_root
         self.retry_on_submission_error = retry_on_submission_error
         self.merge_sliced_step = merge_sliced_step
+        self.pre_script = pre_script
+        self.post_script = post_script
+        self.clean = clean
 
         conf = {}
         if json_file is not None:
             with open(json_file, "r") as f:
                 conf = json.load(f)
 
         self.machine_dict = {
@@ -128,39 +138,51 @@
             }
         }
         if self.password is not None:
             self.machine_dict["remote_profile"]["password"] = self.password
         if self.remote_root is not None:
             self.machine_dict["remote_root"] = self.remote_root
         else:
-            self.machine_dict["remote_root"] = "/home/%s/dflow/workflows" % \
-                self.username
+            if self.username == "root":
+                self.machine_dict["remote_root"] = "/root/dflow/workflows"
+            else:
+                self.machine_dict["remote_root"] = "/home/%s/dflow/workflows"\
+                    % self.username
         if self.private_key_file is not None:
             self.machine_dict["remote_profile"]["key_filename"] = \
                 "/root/.ssh/" + os.path.basename(self.private_key_file)
         if "machine" in conf:
             update_dict(self.machine_dict, conf["machine"])
         if machine_dict is not None:
             update_dict(self.machine_dict, machine_dict)
 
         if self.machine_dict["context_type"] == "Bohrium":
             if "batch_type" not in self.machine_dict:
                 self.machine_dict["batch_type"] = "Bohrium"
-            if "email" not in self.machine_dict["remote_profile"] and \
-                    bohrium.config["username"] is not None:
-                self.machine_dict["remote_profile"]["email"] = \
-                    bohrium.config["username"]
-            if "password" not in self.machine_dict["remote_profile"] and \
-                    bohrium.config["password"] is not None:
-                self.machine_dict["remote_profile"]["password"] = \
-                    bohrium.config["password"]
-            if "program_id" not in self.machine_dict["remote_profile"] and \
-                    bohrium.config["project_id"] is not None:
-                self.machine_dict["remote_profile"]["program_id"] = int(
-                    bohrium.config["project_id"])
+            if "email" not in self.machine_dict["remote_profile"]:
+                if bohrium.config["username"] is not None:
+                    self.machine_dict["remote_profile"]["email"] = \
+                        bohrium.config["username"]
+                else:
+                    self.machine_dict["remote_profile"]["email"] = input(
+                        "Bohrium email: ")
+            if "password" not in self.machine_dict["remote_profile"]:
+                if bohrium.config["password"] is not None:
+                    self.machine_dict["remote_profile"]["password"] = \
+                        bohrium.config["password"]
+                else:
+                    self.machine_dict["remote_profile"]["password"] = getpass(
+                        "Bohrium password: ")
+            if "program_id" not in self.machine_dict["remote_profile"]:
+                if bohrium.config["project_id"] is not None:
+                    self.machine_dict["remote_profile"]["program_id"] = int(
+                        bohrium.config["project_id"])
+                else:
+                    self.machine_dict["remote_profile"]["program_id"] = int(
+                        input("Bohrium program ID: "))
             if "input_data" not in self.machine_dict["remote_profile"]:
                 self.machine_dict["remote_profile"]["input_data"] = {}
             input_data = self.machine_dict["remote_profile"]["input_data"]
             input_data["log_file"] = "log"
             if "job_type" not in input_data:
                 input_data["job_type"] = "container"
             if "platform" not in input_data:
@@ -175,15 +197,16 @@
         # set env to prevent dispatcher from considering different tasks as one
         self.resources_dict = {
             "number_node": 1,
             "cpu_per_node": 1,
             "group_size": 5,
             "envs": {
                 "DFLOW_WORKFLOW": "{{workflow.name}}",
-                "DFLOW_POD": "{{pod.name}}"
+                "DFLOW_POD": "{{pod.name}}",
+                "PYTHONUNBUFFERED": "true",
             }
         }
         if self.queue_name is not None:
             self.resources_dict["queue_name"] = self.queue_name
         if "resources" in conf:
             update_dict(self.resources_dict, conf["resources"])
         if resources_dict is not None:
@@ -207,15 +230,15 @@
         new_template.image_pull_policy = self.image_pull_policy
         new_template.command = self.command
 
         remote_command = template.command if self.remote_command is None \
             else self.remote_command
         cmd = ""
         if self.map_tmp_dir:
-            cmd += "sed -i \\\"s#\\\\$(pwd)#$(pwd)#g\\\" script && "
+            cmd += "sed -i \"s#\\$(pwd)#$(pwd)#g\" script && "
 
         cmd += run_script(template.image, remote_command,
                           self.docker_executable, self.singularity_executable,
                           self.podman_executable)
         self.task_dict["command"] = cmd
         self.task_dict["forward_files"] = ["script"]
         for art in template.inputs.artifacts.values():
@@ -237,46 +260,72 @@
                 self.task_dict["backward_files"].append(
                     "./" + par.value_from_path)
             elif par.value_from_path is not None and not (
                     merge and sliced_output_parameters):
                 self.task_dict["backward_files"].append(
                     "./" + par.value_from_path)
 
-        new_template.script = "import os\n"
+        new_template.script = self.pre_script
+        new_template.script += "import os\n"
         new_template.script += "os.chdir('%s')\n" % self.work_root
+        if any([art.save_as_parameter for art in
+                template.inputs.artifacts.values()]) and \
+                isinstance(template, PythonOPTemplate):
+            template = deepcopy(template)
+            if self.machine_dict["context_type"] == "Bohrium":
+                template.download_method = "bohrium_download"
+            elif self.machine_dict["context_type"] == "SSHContext":
+                template.download_method = "remote_download"
+            template.render_script()
+            new_template.volumes = [v for v in new_template.volumes
+                                    if v.name not in ["launching", "dev-fuse"]]
+            new_template.mounts = [m for m in new_template.mounts
+                                   if m.name != "launching"]
+            new_template.sidecars = [s for s in new_template.sidecars
+                                     if not s.name.startswith("rclone-")]
+
         new_template.script += "with open('script', 'w') as f:\n"
         new_template.script += "    f.write(r\"\"\"\n"
         if self.map_tmp_dir:
-            new_template.script += render_script_with_tmp_root(template,
-                                                               "$(pwd)/tmp")
+            script = render_script_with_tmp_root(template, "$(pwd)/tmp")
         else:
-            new_template.script += template.script
+            script = template.script
+        # keep the script human-readable
+        script = script.replace("\"\"\"", "'''")
+        new_template.script += script
         new_template.script += "\"\"\")\n"
 
         if self.machine_dict["context_type"] == "Bohrium":
             if "image_name" not in self.machine_dict["remote_profile"][
                     "input_data"]:
                 self.machine_dict["remote_profile"]["input_data"][
                     "image_name"] = template.image
 
         self.machine_dict["local_root"] = self.work_root
         new_template.script += "import json, shlex\n"
         new_template.script += "from dpdispatcher import Machine, Resources,"\
             " Task, Submission\n"
         new_template.script += "machine = Machine.load_from_dict(json.loads("\
-            "'%s'))\n" % json.dumps(self.machine_dict)
+            "r'%s'))\n" % json.dumps(self.machine_dict)
+        for name, art in template.inputs.artifacts.items():
+            if self.machine_dict["context_type"] == "Bohrium" and \
+                    art.save_as_parameter:
+                new_template.script += "machine.input_data['job_resources']"\
+                    " = machine.input_data.get('job_resources', []) + ['%s']"\
+                    "\n" % art.source.get_bohrium_urn(name)
+
         new_template.script += "resources = Resources.load_from_dict(json."\
-            "loads('%s'))\n" % json.dumps(self.resources_dict)
+            "loads(r'%s'))\n" % json.dumps(self.resources_dict)
         if new_template.envs is not None:
             for k in new_template.envs.keys():
                 new_template.script += "resources.envs['%s'] = "\
                     "os.environ.get('%s')\n" % (k, k)
         new_template.script += "resources.envs['ARGO_TEMPLATE'] = "\
             "shlex.quote(os.environ.get('ARGO_TEMPLATE'))\n"
-        new_template.script += "task = Task.load_from_dict(json.loads('%s'))"\
+        new_template.script += "task = Task.load_from_dict(json.loads(r'%s'))"\
             "\n" % json.dumps(self.task_dict)
         new_template.script += "task.forward_files = list(filter("\
             "os.path.exists, task.forward_files))\n"
         new_template.script += "for f in task.backward_files:\n"
         new_template.script += "    os.makedirs(os.path.dirname(f), "\
             "exist_ok=True)\n"
         if merge:
@@ -363,51 +412,69 @@
             new_template.script += "submission = Submission(work_base='.', "\
                 "machine=machine, resources=resources, task_list=[task])\n"
         if self.retry_on_submission_error:
             new_template.script += "for retry in range(%s):\n" % \
                 self.retry_on_submission_error
             new_template.script += "    try:\n"
             new_template.script += "        print('retry ' + str(retry))\n"
-            new_template.script += "        submission.run_submission()\n"
+            new_template.script += "        submission.run_submission(clean="\
+                "%s)\n" % self.clean
             new_template.script += "        break\n"
             new_template.script += "    except Exception:\n"
             new_template.script += "        import traceback\n"
             new_template.script += "        traceback.print_exc()\n"
             new_template.script += "        import time\n"
             new_template.script += "        time.sleep(2**retry)\n"
         else:
-            new_template.script += "submission.run_submission()\n"
+            new_template.script += "submission.run_submission(clean=%s)\n" % \
+                self.clean
         if merge:
             for name in sliced_output_parameters:
                 path = template.outputs.parameters[name].value_from_path
                 new_template.script += "res = []\n"
                 new_template.script += "for i in range(len(item_list)):\n"
                 new_template.script += "    fname = './%s_' + str(i)\n" % path
                 new_template.script += "    if os.path.isfile(fname):\n"
                 new_template.script += "        with open(fname, 'r') as f:\n"
                 new_template.script += "            res.append(f.read())\n"
                 new_template.script += "with open('./%s', 'w') as f:\n" % path
                 new_template.script += "    f.write(json.dumps(res))\n"
+        new_template.script_rendered = True
 
         # workaround for unavailable exit code of Bohrium job
         # check output files explicitly
         for art in template.outputs.artifacts.values():
             new_template.script += "assert os.path.exists('./%s')\n" % art.path
         for par in template.outputs.parameters.values():
             if par.save_as_artifact or (par.value_from_path is not None and
                                         not hasattr(par, "default")):
                 new_template.script += "assert os.path.exists('./%s')\n" % \
                     par.value_from_path
 
+        new_template.script += self.post_script
         if self.private_key_file is not None:
             key = upload_s3(self.private_key_file)
             private_key_artifact = S3Artifact(key=key)
             new_template.inputs.artifacts["dflow_private_key"] = InputArtifact(
                 path="/root/.ssh/" + os.path.basename(self.private_key_file),
                 source=private_key_artifact, mode=0o600)
         else:
             new_template.volumes.append(V1Volume(
                 name="dflow-private-key", host_path=V1HostPathVolumeSource(
                     path=config["private_key_host_path"])))
             new_template.mounts.append(V1VolumeMount(
                 name="dflow-private-key", mount_path="/root/.ssh"))
         return new_template
+
+
+class DispatcherArtifact(CustomArtifact, ABC):
+    @abc.abstractmethod
+    def get_bohrium_urn(self, name: str) -> str:
+        pass
+
+    @abc.abstractmethod
+    def remote_download(self, name: str, path: str):
+        pass
+
+    @abc.abstractmethod
+    def bohrium_download(self, name: str, path: str):
+        pass
```

### Comparing `pydflow-1.6.99/src/dflow/plugins/lebesgue.py` & `pydflow-1.7.0/src/dflow/plugins/lebesgue.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/src/dflow/plugins/metadata.py` & `pydflow-1.7.0/src/dflow/plugins/metadata.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/src/dflow/plugins/oss.py` & `pydflow-1.7.0/src/dflow/plugins/oss.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from typing import Optional
 
 import oss2
 
+from ..config import s3_config
 from ..utils import StorageClient
 
 
 class OSSClient(StorageClient):
     def __init__(
             self,
             endpoint: Optional[str] = None,
@@ -26,48 +27,64 @@
         self.bucket_name = bucket_name
         self.access_key_id = access_key_id
         self.access_key_secret = access_key_secret
         auth = oss2.Auth(access_key_id, access_key_secret)
         bucket = oss2.Bucket(auth, endpoint, bucket_name)
         self.bucket = bucket
 
+    def to_dict(self):
+        retained_keys = ["endpoint", "bucket_name"]
+        return {k: self.__dict__[k] for k in retained_keys}
+
+    def prefixing(self, key):
+        if not key.startswith(s3_config["repo_prefix"]):
+            return s3_config["repo_prefix"] + key
+        return key
+
+    def unprefixing(self, key):
+        if key.startswith(s3_config["repo_prefix"]):
+            return key[len(s3_config["repo_prefix"]):]
+        return key
+
     def upload(self, key, path):
-        self.bucket.put_object_from_file(key, path)
+        self.bucket.put_object_from_file(self.prefixing(key), path)
 
     def download(self, key, path):
         if os.path.dirname(path):
             os.makedirs(os.path.dirname(path), exist_ok=True)
-        self.bucket.get_object_to_file(key, path)
+        self.bucket.get_object_to_file(self.prefixing(key), path)
 
     def list(self, prefix, recursive=False):
+        prefix = self.prefixing(prefix)
         keys = []
         if recursive:
             marker = ""
             while True:
                 r = self.bucket.list_objects(prefix, marker=marker)
                 for obj in r.object_list:
                     if not obj.key.endswith("/"):
-                        keys.append(obj.key)
+                        keys.append(self.unprefixing(obj.key))
                 if not r.is_truncated:
                     break
                 marker = r.next_marker
         else:
             marker = ""
             while True:
                 r = self.bucket.list_objects(prefix, delimiter="/",
                                              marker=marker)
                 for obj in r.object_list:
                     if obj.key == prefix and obj.key.endswith("/"):
                         continue
-                    keys.append(obj.key)
+                    keys.append(self.unprefixing(obj.key))
                 for key in r.prefix_list:
-                    keys.append(key)
+                    keys.append(self.unprefixing(key))
                 if not r.is_truncated:
                     break
                 marker = r.next_marker
         return keys
 
     def copy(self, src, dst):
-        self.bucket.copy_object(self.bucket_name, src, dst)
+        self.bucket.copy_object(self.bucket_name, self.prefixing(src),
+                                self.prefixing(dst))
 
     def get_md5(self, key):
-        return self.bucket.get_object_meta(key).etag
+        return self.bucket.get_object_meta(self.prefixing(key).etag)
```

### Comparing `pydflow-1.6.99/src/dflow/plugins/ray.py` & `pydflow-1.7.0/src/dflow/plugins/ray.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/src/dflow/python/op.py` & `pydflow-1.7.0/src/dflow/python/op.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 from ..argo_objects import ArgoObjectDict
 from ..config import config
 from ..utils import get_key, s3_config
 from .opio import (OPIO, Artifact, BigParameter, OPIOSign, Parameter,
                    type_to_str)
 
+iwd = os.getcwd()
+
 
 class OP(ABC):
     """
     Python class OP
 
     Args:
         progress_total: an int representing total progress
@@ -106,14 +108,15 @@
             self,
             op_in: OPIO,
     ) -> OPIO:
         """Run the OP
         """
         raise NotImplementedError
 
+    @staticmethod
     def exec_sign_check(func):
         @functools.wraps(func)
         def wrapper_exec(self, op_in):
             OP._check_signature(op_in, self.get_input_sign(), True)
             op_out = func(self, op_in)
             OP._check_signature(op_out, self.get_output_sign(), False)
             return op_out
```

### Comparing `pydflow-1.6.99/src/dflow/python/opio.py` & `pydflow-1.7.0/src/dflow/python/opio.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,23 +59,26 @@
             self,
             type: Any,
             archive: str = "default",
             save: List[Union[PVC, S3Artifact]] = None,
             optional: bool = False,
             global_name: Optional[str] = None,
             sub_path: bool = True,
+            **kwargs,
     ) -> None:
         self.type = type
         if archive == "default":
             archive = config["archive_mode"]
         self.archive = archive
         self.save = save
         self.optional = optional
         self.global_name = global_name
         self.sub_path = sub_path
+        for k, v in kwargs.items():
+            self.__setattr__(k, v)
 
     def __setattr__(self, key, value):
         if key == "type":
             assert (value in ArtifactAllowedTypes), "%s is not allowed" \
                                                     "artifact type, only %s " \
                                                     "are allowed." % (
                                                         value,
@@ -103,14 +106,16 @@
             global_name: Optional[str] = None,
             **kwargs,
     ) -> None:
         self.type = type
         self.global_name = global_name
         if "default" in kwargs:
             self.default = kwargs["default"]
+        for k, v in kwargs.items():
+            self.__setattr__(k, v)
 
     def to_str(self):
         default = ""
         if hasattr(self, "default"):
             try:
                 default = ", default=%s" % json.dumps(self.default)
             except Exception:
@@ -131,14 +136,16 @@
             self,
             type: Any,
             **kwargs,
     ) -> None:
         self.type = type
         if "default" in kwargs:
             self.default = kwargs["default"]
+        for k, v in kwargs.items():
+            self.__setattr__(k, v)
 
     def to_str(self):
         default = ""
         if hasattr(self, "default"):
             try:
                 default = ", default=%s" % json.dumps(self.default)
             except Exception:
```

### Comparing `pydflow-1.6.99/src/dflow/python/python_op_template.py` & `pydflow-1.7.0/src/dflow/python/python_op_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import inspect
+import logging
 import os
+import sys
 from pathlib import Path
-from typing import Optional, Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Type, Union
 
 import jsonpickle
 import typeguard
 
 from .. import __path__
 from ..common import S3Artifact
 from ..config import config
 from ..io import (PVC, InputArtifact, InputParameter, Inputs, OutputArtifact,
                   OutputParameter, Outputs)
 from ..op_template import PythonScriptOPTemplate
-from ..utils import s3_config, randstr
-from .op import OP
+from ..utils import add_prefix_to_slice, randstr, s3_config
+from .op import OP, iwd
 from .opio import Artifact, BigParameter, Parameter
 
 try:
     from argo.workflows.client import (V1alpha1UserContainer, V1Volume,
                                        V1VolumeMount)
 
     from ..client import V1alpha1RetryStrategy
@@ -50,14 +52,16 @@
             slices: Optional[str] = None,
             input_parameter: Optional[List[str]] = None,
             input_artifact: Optional[List[str]] = None,
             output_parameter: Optional[List[str]] = None,
             output_artifact: Optional[List[str]] = None,
             sub_path: bool = False,
             group_size: Optional[int] = None,
+            shuffle: bool = False,
+            random_seed: int = 0,
             pool_size: Optional[int] = None,
             register_first_only: bool = False,
     ) -> None:
         self.input_parameter = input_parameter if input_parameter is not \
             None else []
         self.input_artifact = input_artifact if input_artifact is not None \
             else []
@@ -69,26 +73,46 @@
         if slices is not None:
             self.slices = slices
         elif self.sub_path:
             self.slices = "{{item.order}}"
         else:
             self.slices = "{{item}}"
         self.group_size = group_size
+        self.shuffle = shuffle
+        self.random_seed = random_seed
         self.pool_size = pool_size
         self.register_first_only = register_first_only
 
 
 def get_source_code(o):
     source_lines, start_line = inspect.getsourcelines(o)
-    with open(inspect.getsourcefile(o), "r",
-              encoding="utf-8") as fd:
+    if sys.version_info.minor >= 9:
+        source_file = inspect.getsourcefile(o)
+    else:
+        source_file = os.path.join(iwd, inspect.getsourcefile(o))
+    with open(source_file, "r", encoding="utf-8") as fd:
         pre_lines = fd.readlines()[:start_line-1]
     return "".join(pre_lines + source_lines) + "\n"
 
 
+def handle_packages_script(package_root):
+    script = "import os, sys, json\n"
+    script += "package_root = r'%s'\n" % package_root
+    script += "catalog_dir = os.path.join(package_root, "\
+        "'%s')\n" % config['catalog_dir_name']
+    script += "if os.path.exists(catalog_dir):\n"
+    script += "    for f in os.listdir(catalog_dir):\n"
+    script += "        with open(os.path.join(catalog_dir, f), 'r')"\
+        " as fd:\n"
+    script += "            for item in json.load(fd)['path_list']:\n"
+    script += "                sys.path.insert(0, os.path.join("\
+        "package_root, os.path.dirname(item['dflow_list_item'])))\n"
+    return script
+
+
 class PythonOPTemplate(PythonScriptOPTemplate):
     """
     Convert from Python class OP to OP template
 
     Args:
         op_class: Python class OP
         image: image of the OP template
@@ -120,24 +144,25 @@
         volumes: volumes to use in the OP template
         mounts: volumes to mount in the OP template
         image_pull_policy: Always, IfNotPresent, Never
         requests: a dict of resource requests
         limits: a dict of resource limits
         envs: environment variables
         init_containers: init containers before the template runs
+        sidecars: sidecar containers
     """
 
     def __init__(self,
-                 op_class: OP,
+                 op_class: Union[Type[OP], OP],
                  image: Optional[str] = None,
                  command: Union[str, List[str]] = None,
                  output_artifact_save: Dict[str,
                                             List[Union[PVC, S3Artifact]]]
                  = None,
-                 output_artifact_archive: Dict[str, str] = None,
+                 output_artifact_archive: Dict[str, Optional[str]] = None,
                  output_parameter_default: Dict[str, Any] = None,
                  input_artifact_slices: Dict[str, str] = None,
                  input_parameter_slices: Dict[str, str] = None,
                  output_artifact_slices: Dict[str, str] = None,
                  output_parameter_slices: Dict[str, str] = None,
                  output_artifact_global_name: Dict[str, str] = None,
                  output_parameter_global_name: Dict[str, str] = None,
@@ -151,19 +176,21 @@
                  mounts: Optional[List[V1VolumeMount]] = None,
                  image_pull_policy: Optional[str] = None,
                  requests: Dict[str, str] = None,
                  limits: Dict[str, str] = None,
                  upload_dflow: bool = True,
                  envs: Dict[str, str] = None,
                  init_containers: Optional[List[V1alpha1UserContainer]] = None,
+                 sidecars: Optional[List[V1alpha1UserContainer]] = None,
                  tmp_root: str = "/tmp",
                  pre_script: str = "",
                  post_script: str = "",
                  ) -> None:
         self.n_parts = {}
+        self.keys_of_parts = {}
         self.op_class = op_class
         op = None
         if isinstance(op_class, OP):
             op = op_class
             op_class = op.__class__
         class_name = op_class.__name__
         input_sign = op_class.get_input_sign()
@@ -177,26 +204,21 @@
         if output_artifact_global_name is not None:
             for name, global_name in output_artifact_global_name.items():
                 output_sign[name].global_name = global_name
         super().__init__(
             name="%s-%s" % (class_name, randstr()), inputs=Inputs(),
             outputs=Outputs(), volumes=volumes, mounts=mounts,
             requests=requests, limits=limits, envs=envs,
-            init_containers=init_containers)
+            init_containers=init_containers, sidecars=sidecars)
         self.pre_script = pre_script
         self.post_script = post_script
         if timeout is not None:
             self.timeout = "%ss" % timeout
-        if retry_on_transient_error is not None:
-            if timeout_as_transient_error:
-                expr = "asInt(lastRetry.exitCode) != 2"
-            else:
-                expr = "asInt(lastRetry.exitCode) == 1"
-            self.retry_strategy = V1alpha1RetryStrategy(
-                limit=retry_on_transient_error, expression=expr)
+        self.retry_on_transient_error = retry_on_transient_error
+        self.timeout_as_transient_error = timeout_as_transient_error
         self.dflow_vars = {}
         self.tmp_root = tmp_root
         for name, sign in input_sign.items():
             if isinstance(sign, Artifact):
                 self.inputs.artifacts[name] = InputArtifact(
                     path="%s/inputs/artifacts/" % self.tmp_root + name,
                     optional=sign.optional, type=sign.type,
@@ -311,96 +333,92 @@
             else input_artifact_slices
         self.input_parameter_slices = {} if input_parameter_slices is None \
             else input_parameter_slices
         self.output_artifact_slices = {} if output_artifact_slices is None \
             else output_artifact_slices
         self.output_parameter_slices = {} if output_parameter_slices is None \
             else output_parameter_slices
-        self.slices = slices
-
-    def __setattr__(self, key, value):
-        super().__setattr__(key, value)
-        if key == "slices":
-            self.init_slices(value)
-            self.render_script()
+        self.set_slices(slices)
+        self.download_method = "download"
 
-    def init_slices(self, slices):
+    def set_slices(self, slices, input_artifact_prefix=None):
+        self.slices = slices
         self.input_artifact_slices = {}
         self.input_parameter_slices = {}
         self.output_artifact_slices = {}
         self.output_parameter_slices = {}
-        self.add_slices(slices)
-
-    def add_slices(self, slices):
         if slices is not None:
-            assert isinstance(slices, Slices)
-            if slices.input_artifact and not slices.sub_path:
-                for name in slices.input_artifact:
+            self.add_slices(slices, input_artifact_prefix)
+        else:
+            self.render_script()
+
+    def add_slices(self, slices: Slices, input_artifact_prefix=None):
+        if input_artifact_prefix is None:
+            input_artifact_prefix = {}
+        if slices.input_artifact and not slices.sub_path:
+            for name in slices.input_artifact:
+                if name in input_artifact_prefix:
+                    self.input_artifact_slices[name] = add_prefix_to_slice(
+                        input_artifact_prefix[name], slices.slices)
+                else:
                     self.input_artifact_slices[name] = slices.slices
-            if slices.input_parameter:
-                for name in slices.input_parameter:
-                    self.input_parameter_slices[name] = slices.slices
-            if slices.output_artifact:
-                self.output_artifact_slices = {}
-                for name in slices.output_artifact:
-                    self.output_artifact_slices[name] = slices.slices
-                    self.outputs.artifacts[name].archive = None  # no archive
-            if slices.output_parameter:
-                for name in slices.output_parameter:
-                    self.output_parameter_slices[name] = slices.slices
-
-            if slices.sub_path:
-                for name in slices.input_artifact:
-                    self.inputs.parameters["dflow_%s_sub_path" %
-                                           name] = InputParameter(value=".")
-                    sign = self.input_sign[name]
-                    self.inputs.artifacts[name] = InputArtifact(
-                        path="%s/inputs/artifacts/%s/{{inputs.parameters."
-                        "dflow_%s_sub_path}}" % (self.tmp_root, name, name),
-                        optional=sign.optional, type=sign.type)
+        if slices.input_parameter:
+            for name in slices.input_parameter:
+                self.input_parameter_slices[name] = slices.slices
+        if slices.output_artifact:
+            self.output_artifact_slices = {}
+            for name in slices.output_artifact:
+                self.output_artifact_slices[name] = slices.slices
+                self.outputs.artifacts[name].archive = None  # no archive
+        if slices.output_parameter:
+            for name in slices.output_parameter:
+                self.output_parameter_slices[name] = slices.slices
+
+        if slices.sub_path:
+            for name in slices.input_artifact:
+                self.inputs.parameters["dflow_%s_sub_path" %
+                                       name] = InputParameter(value=".")
+                sign = self.input_sign[name]
+                self.inputs.artifacts[name] = InputArtifact(
+                    path="%s/inputs/artifacts/%s/{{inputs.parameters."
+                    "dflow_%s_sub_path}}" % (self.tmp_root, name, name),
+                    optional=sign.optional, type=sign.type)
+        self.render_script()
 
     def render_script(self):
         op_class = self.op_class
         class_name = op_class.__name__
         op = self.op
         input_sign = self.input_sign
         output_sign = self.output_sign
         input_artifact_slices = self.input_artifact_slices
         input_parameter_slices = self.input_parameter_slices
         output_artifact_slices = self.output_artifact_slices
         output_parameter_slices = self.output_parameter_slices
 
         script = self.pre_script.format(**{"tmp_root": self.tmp_root})
         if self.python_packages:
-            script += "import os, sys, json\n"
-            script += "package_root = r'%s/inputs/artifacts/"\
-                "dflow_python_packages'\n" % self.tmp_root
-            script += "catalog_dir = os.path.join(package_root, "\
-                "'%s')\n" % config['catalog_dir_name']
-            script += "if os.path.exists(catalog_dir):\n"
-            script += "    for f in os.listdir(catalog_dir):\n"
-            script += "        with open(os.path.join(catalog_dir, f), 'r')"\
-                " as fd:\n"
-            script += "            for item in json.load(fd)['path_list']:\n"
-            script += "                sys.path.insert(0, os.path.join("\
-                "package_root, os.path.dirname(item['dflow_list_item'])))\n"
+            script += handle_packages_script(
+                "%s/inputs/artifacts/dflow_python_packages" % self.tmp_root)
 
         script += "import json, jsonpickle\n"
         script += "from dflow import config, s3_config\n"
         script += "config.update(jsonpickle.loads(r'''%s'''))\n" % \
             jsonpickle.dumps(config)
         script += "s3_config.update(jsonpickle.loads(r'''%s'''))\n" % \
             jsonpickle.dumps(s3_config)
         if op_class.__module__ in ["__main__", "__mp_main__"]:
             try:
                 if hasattr(op_class, "func"):
                     script += get_source_code(op_class.func)
                 else:
                     script += get_source_code(op_class)
             except Exception:
+                logging.info("Failed to get source code of OP, "
+                             "use cloudpickle instead", exc_info=True)
                 import cloudpickle
                 if self.python_packages:
                     self.python_packages.update(cloudpickle.__path__)
                 else:
                     self.python_packages = set(cloudpickle.__path__)
 
                 script += "import cloudpickle\n"
@@ -446,28 +464,38 @@
                 if isinstance(input_sign[name], Artifact):
                     if input_sign[name].type == str:
                         script += "    input_sign['%s'].type = List[str]\n" % \
                             name
                     elif input_sign[name].type == Path:
                         script += "    input_sign['%s'].type = List[Path]\n" %\
                             name
+        if any([art.save_as_parameter
+                for art in self.inputs.artifacts.values()]):
+            script += "    pids = []\n"
         for name, sign in input_sign.items():
             if isinstance(sign, Artifact):
+                if self.inputs.artifacts[name].save_as_parameter:
+                    script += "    pids.append(jsonpickle.loads('{{inputs."\
+                        "parameters.dflow_art_%s}}').%s('%s', '%s/inputs/"\
+                        "artifacts/%s'))\n" % (name, self.download_method,
+                                               name, self.tmp_root, name)
                 slices = self.get_slices(input_artifact_slices, name)
                 if self.slices is not None and self.slices.sub_path and \
                         name in self.slices.input_artifact:
                     script += "    input['%s'] = handle_input_artifact('%s', "\
                         "input_sign['%s'], %s, r'%s', '{{inputs.parameters."\
                         "dflow_%s_sub_path}}', None)\n" % (
                             name, name, name, slices, self.tmp_root, name)
                 else:
                     script += "    input['%s'] = handle_input_artifact('%s', "\
-                        "input_sign['%s'], %s, r'%s', None, %s)\n" \
-                        % (name, name, name, slices, self.tmp_root,
-                           self.n_parts.get(name, None))
+                        "input_sign['%s'], %s, r'%s', None, %s, "\
+                        "keys_of_parts=%s)\n" % (
+                            name, name, name, slices, self.tmp_root,
+                            self.n_parts.get(name, None),
+                            self.keys_of_parts.get(name, None))
             else:
                 slices = self.get_slices(input_parameter_slices, name)
                 if isinstance(sign, BigParameter) and \
                         config["mode"] != "debug":
                     script += "    input['%s'] = handle_input_parameter('%s',"\
                         " '', input_sign['%s'], %s, r'%s')\n" \
                         % (name, name, name, slices, self.tmp_root)
@@ -584,14 +612,21 @@
             script += "                raise error\n"
             script += "    except TransientError:\n"
             script += "        sys.exit(1)\n"
             script += "    except FatalError:\n"
             script += "        sys.exit(2)\n"
 
         script += self.post_script.format(**{"tmp_root": self.tmp_root})
+
+        if any([art.save_as_parameter
+                for art in self.inputs.artifacts.values()]):
+            script += "    import signal\n"
+            script += "    [os.killpg(os.getpgid(pid), signal.SIGTERM)"\
+                " for pid in pids if pid is not None]\n"
+
         self.script = script
 
     def get_slices(self, slices_dict, name):
         slices = None
         if slices_dict is not None:
             slices = self.render_slices(slices_dict.get(name, None))
         return slices
@@ -610,14 +645,24 @@
                 self.dflow_vars[var] = var_name
             else:
                 var_name = self.dflow_vars[var]
             slices = slices.replace(var, "{{inputs.parameters.%s}}" % var_name)
             i = slices.find("{{item")
         return slices
 
+    def convert_to_argo(self, memoize_prefix=None, memoize_configmap="dflow"):
+        if self.retry_on_transient_error is not None:
+            if self.timeout_as_transient_error:
+                expr = "asInt(lastRetry.exitCode) != 2"
+            else:
+                expr = "asInt(lastRetry.exitCode) == 1"
+            self.retry_strategy = V1alpha1RetryStrategy(
+                limit=self.retry_on_transient_error, expression=expr)
+        return super().convert_to_argo(memoize_prefix, memoize_configmap)
+
 
 class TransientError(Exception):
     pass
 
 
 class FatalError(Exception):
     pass
```

### Comparing `pydflow-1.6.99/src/dflow/python/utils.py` & `pydflow-1.7.0/src/dflow/python/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from pathlib import Path
 from typing import Dict, List, Set
 
 import jsonpickle
 
 from ..config import config
 from ..utils import (assemble_path_list, assemble_path_nested_dict,
-                     convert_dflow_list, copy_file, remove_empty_dir_tag)
+                     convert_dflow_list, copy_file, expand, flatten,
+                     remove_empty_dir_tag)
 from .opio import Artifact, BigParameter, NestedDict, Parameter
 
 
 def get_slices(path_list, path_dict, slices):
     if slices is not None:
         slices = slices if isinstance(slices, list) else [slices]
         new_path_list = []
@@ -36,15 +37,16 @@
         else:
             path_list = new_path_list
             path_dict = path_list
     return path_list, path_dict
 
 
 def handle_input_artifact(name, sign, slices=None, data_root="/tmp",
-                          sub_path=None, n_parts=None):
+                          sub_path=None, n_parts=None, keys_of_parts=None,
+                          path=None):
     require_dict = sign.type in [
         Dict[str, str], Dict[str, Path], NestedDict[str], NestedDict[Path]] \
         or slices is not None
 
     if n_parts is not None:
         path_list = []
         path_dict = []
@@ -52,25 +54,46 @@
             art_path = '%s/inputs/artifacts/dflow_%s_%s' % (data_root, name, i)
             remove_empty_dir_tag(art_path)
             pl = assemble_path_list(art_path)
             if require_dict:
                 pd = assemble_path_nested_dict(art_path)
                 if slices is not None:
                     pl, pd = get_slices(pl, pd, slices[i])
-                path_dict.append(pd)
+                if isinstance(pd, list) and len(pd) == 1:
+                    path_dict.append(pd[0])
+                else:
+                    path_dict.append(pd)
             if pl:
                 path_list += pl
             else:
                 path_list.append(art_path)
+    elif keys_of_parts is not None:
+        path_list = []
+        path_dict = {}
+        for i in keys_of_parts:
+            art_path = '%s/inputs/artifacts/dflow_%s_%s' % (data_root, name, i)
+            remove_empty_dir_tag(art_path)
+            pl = assemble_path_list(art_path)
+            pd = assemble_path_nested_dict(art_path)
+            if slices is not None:
+                pl, pd = get_slices(pl, pd, slices[i])
+            if isinstance(pd, list) and len(pd) == 1:
+                path_dict[i] = pd[0]
+            else:
+                path_dict[i] = pd
+            if pl:
+                path_list += pl
+            else:
+                path_list.append(art_path)
+        path_dict = expand(path_dict)
     else:
-        if sub_path is None:
-            art_path = '%s/inputs/artifacts/%s' % (data_root, name)
-        else:
-            art_path = '%s/inputs/artifacts/%s/%s' % (data_root, name,
-                                                      sub_path)
+        art_path = '%s/inputs/artifacts/%s' % (data_root, name) \
+            if path is None else path
+        if sub_path is not None:
+            art_path = os.path.join(art_path, sub_path)
         if not os.path.exists(art_path):  # for optional artifact
             return None
         remove_empty_dir_tag(art_path)
         path_list = assemble_path_list(art_path)
         if require_dict:
             path_dict = assemble_path_nested_dict(art_path)
             path_list, path_dict = get_slices(path_list, path_dict, slices)
@@ -182,34 +205,17 @@
     elif sign.type in [Dict[str, str], Dict[str, Path]]:
         os.makedirs(data_root + '/outputs/artifacts/' + name, exist_ok=True)
         for s, path in value.items():
             path_list.append(copy_results_and_return_path_item(
                 path, name, s, data_root))
     elif sign.type in [NestedDict[str], NestedDict[Path]]:
         os.makedirs(data_root + '/outputs/artifacts/' + name, exist_ok=True)
-
-        def handle(obj, prefix):
-            if isinstance(obj, dict):
-                for k, v in obj.items():
-                    key = prefix + "." + k if prefix else k
-                    if isinstance(v, (list, dict)):
-                        handle(v, key)
-                    elif isinstance(v, (str, Path)):
-                        path_list.append(copy_results_and_return_path_item(
-                            v, name, key, data_root))
-            elif isinstance(obj, list):
-                for i, v in enumerate(obj):
-                    key = prefix + "." + str(i) if prefix else str(i)
-                    if isinstance(v, (list, dict)):
-                        handle(v, key)
-                    elif isinstance(v, (str, Path)):
-                        path_list.append(copy_results_and_return_path_item(
-                            v, name, key, data_root))
-
-        handle(value, "")
+        for s, path in flatten(value).items():
+            path_list.append(copy_results_and_return_path_item(
+                path, name, s, data_root))
 
     os.makedirs(data_root + "/outputs/artifacts/%s/%s" % (name, config[
         "catalog_dir_name"]), exist_ok=True)
     with open(data_root + "/outputs/artifacts/%s/%s/%s" % (name, config[
             "catalog_dir_name"], uuid.uuid4()), "w") as f:
         f.write(jsonpickle.dumps({"path_list": path_list}))
     handle_empty_dir(data_root + "/outputs/artifacts/%s" % name)
```

### Comparing `pydflow-1.6.99/src/dflow/resource.py` & `pydflow-1.7.0/src/dflow/resource.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+import abc
+from abc import ABC
 from typing import Optional
 
 from .op_template import OPTemplate
 
 
-class Resource(object):
+class Resource(ABC):
     """
     Resource
 
     Args:
         action: action on the Kubernetes resource
         success_condition: expression representing success
         failure_condition: expression representing failure
     """
     action: Optional[str] = None
     success_condition: Optional[str] = None
     failure_condition: Optional[str] = None
 
+    @abc.abstractmethod
     def get_manifest(
             self,
             template: OPTemplate,
     ) -> OPTemplate:
         """
         The method to get the manifest (str)
         """
```

### Comparing `pydflow-1.6.99/src/dflow/slurm.py` & `pydflow-1.7.0/src/dflow/slurm.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/src/dflow/step.py` & `pydflow-1.7.0/src/dflow/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,44 @@
+import json
 import logging
 import os
 import re
 import sys
 from copy import deepcopy
 from typing import Any, Dict, List, Optional, Union
 
 import jsonpickle
 
-from .common import LocalArtifact, S3Artifact
+from .common import CustomArtifact, HTTPArtifact, LocalArtifact, S3Artifact
 from .config import config, s3_config
 from .context_syntax import GLOBAL_CONTEXT
 from .executor import Executor
 from .io import (PVC, ArgoVar, Expression, InputArtifact, InputParameter,
                  OutputArtifact, OutputParameter, if_expression, to_expr)
 from .op_template import (OPTemplate, PythonScriptOPTemplate, ScriptOPTemplate,
                           ShellOPTemplate)
 from .python import Slices
 from .resource import Resource
 from .util_ops import CheckNumSuccess, CheckSuccessRatio, InitArtifactForSlices
-from .utils import catalog_of_artifact, merge_dir, randstr, upload_artifact
+from .utils import (add_prefix_to_slice, catalog_of_artifact, flatten,
+                    merge_dir, randstr, upload_artifact)
 
 try:
     from argo.workflows.client import (V1alpha1Arguments, V1alpha1ContinueOn,
                                        V1alpha1ResourceTemplate,
                                        V1alpha1WorkflowStep, V1VolumeMount)
 
     from .client import V1alpha1Sequence
 except Exception:
     V1alpha1Sequence = object
 
 
 uploaded_python_packages = []
 
 
-def add_prefix_to_slices(prefix, slices):
-    return "(lambda x: ['%s.' + str(i) for i in x] "\
-        "if isinstance(x, list) else '%s.' + str(x))(%s)" % (
-            prefix, prefix, slices)
-
-
 class ArgoRange(ArgoVar):
     def __init__(self, end, start=0, step=1):
         self.end = end
         self.start = start
         self.step = step
         if isinstance(start, (InputParameter, OutputParameter)):
             start = "sprig.atoi(%s)" % start.expr
@@ -177,14 +173,41 @@
         param: the Argo parameter which is a list
     """
     if config["mode"] == "debug":
         return Expression("len(%s)" % to_expr(param))
     return ArgoLen(param)
 
 
+class ArgoEnumerate(ArgoVar):
+    def __init__(self, param: ArgoVar):
+        super().__init__(
+            "toJson(map(sprig.untilStep(0, len(sprig.fromJson(%s)), 1),"
+            " { {'order': #, 'value': jsonpath(%s, '$')[#]} }))" % (
+                param.expr, param.expr))
+
+
+def argo_enumerate(
+        param,
+) -> ArgoVar:
+    """
+    Return the enumeration of a list which is an Argo parameter
+
+    Args:
+        param: the Argo parameter which is a list
+    """
+    if config["mode"] == "debug":
+        return Expression("[{'order': i, 'value': v} for i, v in "
+                          "enumerate(%s)]" % to_expr(param))
+    if isinstance(param, ArgoVar):
+        return ArgoEnumerate(param)
+    else:
+        return json.dumps([{'order': i, 'value': v} for i, v in
+                           enumerate(param)])
+
+
 class ArgoSum:
     def __init__(self, param):
         self.param = param
         self.expr = "sum(%s)" % param
 
 
 def argo_sum(
@@ -247,16 +270,16 @@
     """
 
     def __init__(
             self,
             name: str,
             template: OPTemplate,
             parameters: Dict[str, Any] = None,
-            artifacts: Dict[str, Union[S3Artifact,
-                                       InputArtifact, OutputArtifact]] = None,
+            artifacts: Dict[str, Optional[Union[
+                S3Artifact, InputArtifact, OutputArtifact]]] = None,
             when: Optional[str] = None,
             with_param: Union[str, list,
                               InputParameter, OutputParameter] = None,
             continue_on_failed: bool = False,
             continue_on_error: bool = False,
             continue_on_num_success: Optional[int] = None,
             continue_on_success_ratio: Optional[float] = None,
@@ -328,115 +351,20 @@
 
         if slices is not None:
             self.template = self.template.copy()
             self.template.slices = slices
             for name, par in self.template.inputs.parameters.items():
                 if name not in self.inputs.parameters:
                     self.inputs.parameters[name] = deepcopy(par)
-
-            self.template.inputs.parameters["dflow_slice"] = InputParameter(
-                value=slices.slices)
-            self.inputs.parameters["dflow_slice"] = InputParameter(
-                value=slices.slices)
-            for name in slices.input_parameter:
-                for step in (self.template if hasattr(
-                        self.template, "__iter__") else []):
-                    for par in list(step.inputs.parameters.values()):
-                        # input parameter referring to sliced input parameter
-                        if par.value is self.template.inputs.parameters[name]:
-                            step.template.inputs.parameters["dflow_slice"] = \
-                                InputParameter()
-                            step.template.add_slices(Slices(
-                                "{{inputs.parameters.dflow_slice}}",
-                                input_parameter=[par.name],
-                                sub_path=slices.sub_path,
-                                pool_size=slices.pool_size))
-                            step.template.render_script()
-                            step.inputs.parameters["dflow_slice"] = \
-                                InputParameter(
-                                    value="{{inputs.parameters.dflow_slice}}")
-
-            for name in slices.input_artifact:
-                for step in (self.template if hasattr(
-                        self.template, "__iter__") else []):
-                    for art in list(step.inputs.artifacts.values()):
-                        # input artifact referring to sliced input artifact
-                        if art.source is self.template.inputs.artifacts[name]:
-                            if name in self.input_artifact_slices:
-                                slice = self.input_artifact_slices[name]
-                                pattern = add_prefix_to_slices(
-                                    slice, "{{inputs.parameters.dflow_slice}}")
-                            else:
-                                pattern = "{{inputs.parameters.dflow_slice}}"
-                            step.template.inputs.parameters["dflow_slice"] = \
-                                InputParameter()
-                            step.template.add_slices(Slices(
-                                pattern,
-                                input_artifact=[art.name],
-                                sub_path=slices.sub_path,
-                                pool_size=slices.pool_size))
-                            step.template.render_script()
-                            step.inputs.parameters["dflow_slice"] = \
-                                InputParameter(
-                                    value="{{inputs.parameters.dflow_slice}}")
-
-            def stack_output_parameter(par):
-                if isinstance(par, OutputParameter):
-                    step = par.step
-                    step.template.inputs.parameters["dflow_slice"] = \
-                        InputParameter()
-                    step.template.add_slices(Slices(
-                        "{{inputs.parameters.dflow_slice}}",
-                        output_parameter=[par.name],
-                        sub_path=slices.sub_path,
-                        pool_size=slices.pool_size))
-                    step.template.render_script()
-                    step.inputs.parameters["dflow_slice"] = \
-                        InputParameter(
-                            value="{{inputs.parameters.dflow_slice}}")
-
-            for name in slices.output_parameter:
-                # sliced output parameter from
-                if self.template.outputs.parameters[name].value_from_parameter\
-                        is not None:
-                    stack_output_parameter(self.template.outputs.parameters[
-                        name].value_from_parameter)
-                elif self.template.outputs.parameters[name].\
-                        value_from_expression is not None:
-                    stack_output_parameter(self.template.outputs.parameters[
-                        name].value_from_expression._then)
-                    stack_output_parameter(self.template.outputs.parameters[
-                        name].value_from_expression._else)
-
-            def stack_output_artifact(art):
-                if isinstance(art, OutputArtifact):
-                    step = art.step
-                    step.template.inputs.parameters["dflow_slice"] = \
-                        InputParameter()
-                    step.template.add_slices(Slices(
-                        "{{inputs.parameters.dflow_slice}}",
-                        output_artifact=[art.name],
-                        sub_path=slices.sub_path,
-                        pool_size=slices.pool_size))
-                    step.template.render_script()
-                    step.inputs.parameters["dflow_slice"] = \
-                        InputParameter(
-                            value="{{inputs.parameters.dflow_slice}}")
-
-            for name in slices.output_artifact:
-                # sliced output artifact from
-                if self.template.outputs.artifacts[name]._from is not None:
-                    stack_output_artifact(
-                        self.template.outputs.artifacts[name]._from)
-                elif self.template.outputs.artifacts[name].from_expression is \
-                        not None:
-                    stack_output_artifact(self.template.outputs.artifacts[
-                        name].from_expression._then)
-                    stack_output_artifact(self.template.outputs.artifacts[
-                        name].from_expression._else)
+            self.template.add_slices(slices, self.input_artifact_slices)
+            from .dag import DAG
+            from .steps import Steps
+            if isinstance(self.template, (DAG, Steps)):
+                self.inputs.parameters["dflow_slice"] = InputParameter(
+                    value=slices.slices)
 
         sum_var = None
         if isinstance(self.with_param, ArgoRange) and \
                 isinstance(self.with_param.end, ArgoSum):
             sum_var = self.with_param.end.param
 
         if self.with_sequence is not None and \
@@ -455,38 +383,74 @@
             concat_var = self.with_sequence.count.param.param
 
         if hasattr(self.template, "slices") and self.template.slices is not \
                 None and self.template.slices.group_size is not None:
             self.template = self.template.copy()
             group_size = self.template.slices.group_size
             self.template.inputs.parameters["dflow_nslices"] = InputParameter()
-            if self.with_param is not None:
+            if self.template.slices.shuffle:
+                self.template.pre_script += "import random\n"
+                self.template.pre_script += "random.seed(%s)\n" % \
+                    self.template.slices.random_seed
+                # pre script is formatted
+                self.template.pre_script += "shuffled = "\
+                    "list(range({{{{inputs.parameters.dflow_nslices}}}}))\n"
+                self.template.pre_script += "random.shuffle(shuffled)\n"
+                self.template.pre_script += "random.seed()\n"  # unset seed
+            if isinstance(self.with_param, ArgoRange):
+                self.template.inputs.parameters["dflow_range_end"] = \
+                    InputParameter()
+                self.inputs.parameters["dflow_range_end"] = \
+                    InputParameter(value=self.with_param.end)
+                self.template.inputs.parameters["dflow_range_start"] = \
+                    InputParameter()
+                self.inputs.parameters["dflow_range_start"] = \
+                    InputParameter(value=self.with_param.start)
+                self.template.inputs.parameters["dflow_range_step"] = \
+                    InputParameter()
+                self.inputs.parameters["dflow_range_step"] = \
+                    InputParameter(value=self.with_param.step)
+                nslices = argo_len(self.with_param)
+                old_slices = self.template.slices.slices
+                self.template.slices.slices = \
+                    "[range({{inputs.parameters.dflow_range_start}}, "\
+                    "{{inputs.parameters.dflow_range_end}}, "\
+                    "{{inputs.parameters.dflow_range_step}})"\
+                    "[%s] for i in range({{item}}*%s, min(({{item}}+1)*%s"\
+                    ", {{inputs.parameters.dflow_nslices}}))]" % (
+                        old_slices.replace("{{item}}", "shuffled[i]"
+                                           if self.template.slices.shuffle
+                                           else "i"), group_size, group_size)
+                # re-render the script
+                self.template.set_slices(self.template.slices,
+                                         self.input_artifact_slices)
+                self.with_param = argo_range(if_expression(
+                    "%s %% %s > 0" % (nslices, group_size),
+                    "%s/%s + 1" % (nslices, group_size),
+                    "%s/%s" % (nslices, group_size)))
+            elif self.with_param is not None:
                 self.template.inputs.parameters["dflow_with_param"] = \
                     InputParameter()
                 self.inputs.parameters["dflow_with_param"] = \
                     InputParameter(value=self.with_param)
                 if hasattr(self.with_param, "__len__"):
                     nslices = len(self.with_param)
                 else:
                     nslices = argo_len(self.with_param)
                 old_slices = self.template.slices.slices
                 self.template.slices.slices = \
                     "[json.loads(r'''{{inputs.parameters.dflow_with_param}}"\
                     "''')[%s] for i in range({{item}}*%s, min(({{item}}+1)*%s"\
                     ", {{inputs.parameters.dflow_nslices}}))]" % (
-                        old_slices.replace("{{item}}", "i"), group_size,
-                        group_size)
+                        old_slices.replace("{{item}}", "shuffled[i]"
+                                           if self.template.slices.shuffle
+                                           else "i"), group_size, group_size)
                 # re-render the script
-                self.template.slices = self.template.slices
-                for k, slice in self.input_artifact_slices.items():
-                    if k in self.template.input_artifact_slices:
-                        old = self.template.input_artifact_slices[k]
-                        self.template.input_artifact_slices[k] = \
-                            add_prefix_to_slices(slice, old)
-                        self.template.render_script()
+                self.template.set_slices(self.template.slices,
+                                         self.input_artifact_slices)
                 self.with_param = argo_range(if_expression(
                     "%s %% %s > 0" % (nslices, group_size),
                     "%s/%s + 1" % (nslices, group_size),
                     "%s/%s" % (nslices, group_size)))
             if self.with_sequence is not None:
                 self.template.inputs.parameters["dflow_sequence_start"] = \
                     InputParameter()
@@ -522,29 +486,25 @@
                     "dflow_sequence_count}}' != 'null' else range(int('{{"\
                     "inputs.parameters.dflow_sequence_start}}'), int('{{"\
                     "inputs.parameters.dflow_sequence_end}}') + 1) if int('{{"\
                     "inputs.parameters.dflow_sequence_end}}') > int('{{"\
                     "inputs.parameters.dflow_sequence_start}}') else range("\
                     "int('{{inputs.parameters.dflow_sequence_start}}'), "\
                     "int('{{inputs.parameters.dflow_sequence_end}}') - 1, -1)"\
-                    ")][i] for i in range(int('{{item}}')*%s, min((int('{{"\
+                    ")][%s] for i in range(int('{{item}}')*%s, min((int('{{"\
                     "item}}')+1)*%s, {{inputs.parameters.dflow_nslices}}))]"\
                     % (old_slices.replace(
                         "'{{item}}'", "('%s' %% j)" % format)
                         if format is not None
                         else old_slices.replace("{{item}}", "j"),
+                        "shuffled[i]" if self.template.slices.shuffle else "i",
                         group_size, group_size)
                 # re-render the script
-                self.template.slices = self.template.slices
-                for k, slice in self.input_artifact_slices.items():
-                    if k in self.template.input_artifact_slices:
-                        old = self.template.input_artifact_slices[k]
-                        self.template.input_artifact_slices[k] = \
-                            add_prefix_to_slices(slice, old)
-                        self.template.render_script()
+                self.template.set_slices(self.template.slices,
+                                         self.input_artifact_slices)
                 self.with_sequence = argo_sequence(
                     count=if_expression(
                         "%s %% %s > 0" % (nslices, group_size),
                         "%s/%s + 1" % (nslices, group_size),
                         "%s/%s" % (nslices, group_size)), format=format)
 
             self.inputs.parameters["dflow_nslices"] = InputParameter(
@@ -559,88 +519,88 @@
             self.template.slices is not None and \
             self.template.slices.sub_path else []
 
         if sliced_output_artifact or sliced_input_artifact or \
                 sum_var is not None or concat_var is not None:
             self.template = self.template.copy()
             init_template = InitArtifactForSlices(
-                self.template.name, self.util_image, self.util_command,
+                self.template, self.util_image, self.util_command,
                 self.util_image_pull_policy, self.key, sliced_output_artifact,
                 sliced_input_artifact, sum_var, concat_var)
             if self.key is not None:
                 self.template.inputs.parameters["dflow_group_key"] = \
                     InputParameter(value="")
                 self.inputs.parameters["dflow_group_key"] = InputParameter(
                     value=re.sub("{{=?item.*}}", "group", str(self.key)))
                 self.template.inputs.parameters["dflow_artifact_key"] = \
                     InputParameter(value="")
                 # For the case of reusing sliced steps, ensure that the output
                 # artifacts are reused
                 for name in sliced_output_artifact:
-                    self.template.outputs.artifacts[name].save.append(
-                        S3Artifact(key="{{inputs.parameters."
-                                   "dflow_artifact_key}}/%s" % name))
-
-                    def merge_output_artifact(art):
+                    def merge_step_output_artifact(art):
                         step = art.step
                         template = step.template
                         template.inputs.parameters["dflow_group_key"] = \
                             InputParameter()
                         step.inputs.parameters["dflow_group_key"] = \
                             InputParameter(
                                 value="{{inputs.parameters.dflow_group_key}}")
                         template.inputs.parameters["dflow_artifact_key"] = \
                             InputParameter()
                         step.inputs.parameters["dflow_artifact_key"] = \
                             InputParameter(value="{{inputs.parameters."
                                            "dflow_artifact_key}}")
-                        template.outputs.artifacts[art.name].save.append(
-                            S3Artifact(key="{{inputs.parameters."
-                                       "dflow_artifact_key}}/%s" % name))
-
-                    if self.template.outputs.artifacts[name]._from is not \
-                            None:
                         merge_output_artifact(
-                            self.template.outputs.artifacts[name]._from)
-                    elif self.template.outputs.artifacts[name].\
-                            from_expression is not None:
-                        merge_output_artifact(self.template.outputs.artifacts[
-                            name].from_expression._then)
-                        merge_output_artifact(self.template.outputs.artifacts[
-                            name].from_expression._else)
+                            template.outputs.artifacts[art.name])
+
+                    def merge_output_artifact(art):
+                        if art._from is not None:
+                            merge_step_output_artifact(art._from)
+                        elif art.from_expression is not None:
+                            merge_step_output_artifact(
+                                art.from_expression._then)
+                            merge_step_output_artifact(
+                                art.from_expression._else)
+                        else:
+                            art.save.append(S3Artifact(
+                                key="{{inputs.parameters.dflow_artifact_key}}"
+                                "/%s" % name))
+
+                    merge_output_artifact(
+                        self.template.outputs.artifacts[name])
             else:
                 self.template.inputs.parameters["dflow_artifact_key"] = \
                     InputParameter(value="")
                 for name in sliced_output_artifact:
-                    self.template.outputs.artifacts[name].save.append(
-                        S3Artifact(key="{{inputs.parameters."
-                                   "dflow_artifact_key}}/%s" % name))
-
-                    def merge_output_artifact(art):
+                    def merge_step_output_artifact(art):
                         step = art.step
                         template = step.template
                         template.inputs.parameters["dflow_artifact_key"] = \
                             InputParameter()
                         step.inputs.parameters["dflow_artifact_key"] = \
                             InputParameter(value="{{inputs.parameters."
                                            "dflow_artifact_key}}")
-                        template.outputs.artifacts[art.name].save.append(
-                            S3Artifact(key="{{inputs.parameters."
-                                       "dflow_artifact_key}}/%s" % name))
-
-                    if self.template.outputs.artifacts[name]._from is not \
-                            None:
                         merge_output_artifact(
-                            self.template.outputs.artifacts[name]._from)
-                    elif self.template.outputs.artifacts[name].\
-                            from_expression is not None:
-                        merge_output_artifact(self.template.outputs.artifacts[
-                            name].from_expression._then)
-                        merge_output_artifact(self.template.outputs.artifacts[
-                            name].from_expression._else)
+                            template.outputs.artifacts[art.name])
+
+                    def merge_output_artifact(art):
+                        if art._from is not None:
+                            merge_step_output_artifact(art._from)
+                        elif art.from_expression is not None:
+                            merge_step_output_artifact(
+                                art.from_expression._then)
+                            merge_step_output_artifact(
+                                art.from_expression._else)
+                        else:
+                            art.save.append(S3Artifact(
+                                key="{{inputs.parameters.dflow_artifact_key}}"
+                                "/%s" % name))
+
+                    merge_output_artifact(
+                        self.template.outputs.artifacts[name])
 
             if self.key is not None:
                 group_key = re.sub("{{=?item.*}}", "group", str(self.key))
                 self.prepare_step = self.__class__(
                     name="%s-init-artifact" % self.name,
                     template=init_template,
                     parameters={"dflow_group_key": group_key})
@@ -652,14 +612,17 @@
                     name="%s-init-artifact" % self.name,
                     template=init_template)
                 self.inputs.parameters["dflow_artifact_key"] = InputParameter(
                     value=self.prepare_step.outputs.parameters[
                         "dflow_artifact_key"])
 
             if sliced_input_artifact:
+                if self.key is not None:
+                    self.prepare_step.inputs.parameters["dflow_key"].value = \
+                        "%s-init-artifact" % group_key
                 for name in sliced_input_artifact:
                     self.inputs.parameters["dflow_%s_sub_path" %
                                            name].value = "{{item.%s}}" % name
                     # step cannot resolve
                     # {{inputs.parameters.dflow_%s_sub_path}}
                     self.inputs.artifacts[name].path = None
                     v = self.inputs.artifacts[name].source
@@ -667,16 +630,15 @@
                         self.prepare_step.inputs.artifacts[name].source = \
                             v.sub_path(config["catalog_dir_name"])
                         self.inputs.artifacts[name].source = \
                             v.sub_path("{{item.%s}}" % name)
                     elif isinstance(v, (InputArtifact, OutputArtifact,
                                         LocalArtifact)):
                         self.prepare_step.inputs.artifacts[name].source = v
-                        self.inputs.artifacts[name].sub_path = \
-                            "{{item.%s}}" % name
+                        self.inputs.artifacts[name].sp = "{{item.%s}}" % name
                 self.with_param = self.prepare_step.outputs.parameters[
                     "dflow_slices_path"]
 
             for name in sliced_output_artifact:
                 self.outputs.artifacts[name].redirect = \
                     self.prepare_step.outputs.artifacts[name]
 
@@ -940,15 +902,15 @@
                 if name[:6] == "dflow_" and name[-9:] == "_sub_path" or \
                         name[:10] == "dflow_var_":
                     del steps.inputs.parameters[name]
                     del self.inputs.parameters[name]
                 else:
                     step.set_parameters({name: steps.inputs.parameters[name]})
             for name, art in list(self.inputs.artifacts.items()):
-                art.sub_path = None
+                art.sp = None
                 if isinstance(art.source, S3Artifact):
                     del steps.inputs.artifacts[name]
                     del self.inputs.artifacts[name]
                 else:
                     step.set_artifacts({name: steps.inputs.artifacts[name]})
             if self.prepare_step is not None:
                 for name in list(self.prepare_step.inputs.parameters.keys()):
@@ -1067,18 +1029,21 @@
             elif "s3" in art:
                 kwargs["artifacts"][name] = S3Artifact(key=art["s3"]["key"])
                 if "subPath" in art:
                     kwargs["artifacts"][name] = kwargs["artifacts"][
                         name].sub_path(art["subPath"])
             elif "oss" in art:
                 kwargs["artifacts"][name] = S3Artifact(
-                    key=art["oss"]["key"]).oss()
+                    key=art["oss"]["key"])
                 if "subPath" in art:
                     kwargs["artifacts"][name] = kwargs["artifacts"][
                         name].sub_path(art["subPath"])
+            elif "http" in art:
+                kwargs["artifacts"][name] = HTTPArtifact(
+                    url=art["http"]["url"])
         kwargs["key"] = kwargs["parameters"].get("dflow_key", None)
         return cls(**kwargs)
 
     def __repr__(self):
         return self.id
 
     def set_parameters(self, parameters):
@@ -1117,30 +1082,46 @@
             self.inputs.parameters[k].value = v
 
     def set_artifacts(self, artifacts):
         for k, v in artifacts.items():
             if v is None:
                 del self.inputs.artifacts[k]
                 self.template.inputs.artifacts[k].optional = True
+            elif isinstance(v, CustomArtifact):
+                self.inputs.artifacts[k].source = v
+                self.inputs.artifacts[k].save_as_parameter = True
+                self.template = deepcopy(self.template)
+                self.template.inputs.artifacts[k].source = v
+                self.template.inputs.artifacts[k].save_as_parameter = True
+                from .python import PythonOPTemplate
+                if isinstance(self.template, PythonOPTemplate):
+                    self.template = v.render(self.template, k)
+                from .dag import DAG
+                from .steps import Steps
+                if isinstance(self.template, (Steps, DAG)):
+                    for step in self.template:
+                        for name, art in step.inputs.artifacts.items():
+                            if art.source is self.template.inputs.artifacts[k]:
+                                step.set_artifacts({name: v})
             elif isinstance(v, (list, tuple)):
                 self.template = self.template.copy()
                 slices = []
                 for i, a in enumerate(v):
                     vn = "dflow_%s_%s" % (k, i)
                     self.template.inputs.artifacts[vn] = deepcopy(
                         self.template.inputs.artifacts[k])
                     self.inputs.artifacts[vn] = deepcopy(
                         self.template.inputs.artifacts[vn])
                     self.inputs.artifacts[vn].source = a
                     if hasattr(a, "slice") and a.slice is not None:
                         slices.append(a.slice)
                     else:
                         slices.append(None)
-                from .steps import Steps
                 from .dag import DAG
+                from .steps import Steps
                 if isinstance(self.template, (Steps, DAG)):
                     for step in self.template:
                         for name, art in list(step.inputs.artifacts.items()):
                             if art.source is self.template.inputs.artifacts[k]:
                                 step.set_artifacts({name: [
                                     self.template.inputs.artifacts[
                                         "dflow_%s_%s" % (k, i)]
@@ -1156,28 +1137,68 @@
                                                         vn)
                     if any(map(lambda x: x is not None, slices)):
                         self.template.input_artifact_slices[k] = slices
                     self.template.n_parts[k] = len(v)
                     self.template.render_script()
                 del self.template.inputs.artifacts[k]
                 del self.inputs.artifacts[k]
+            elif isinstance(v, dict):
+                self.template = self.template.copy()
+                slices = {}
+                flat_v = flatten(v)
+                for i, a in flat_v.items():
+                    vn = "dflow_%s_%s" % (k, i)
+                    self.template.inputs.artifacts[vn] = deepcopy(
+                        self.template.inputs.artifacts[k])
+                    self.inputs.artifacts[vn] = deepcopy(
+                        self.template.inputs.artifacts[vn])
+                    self.inputs.artifacts[vn].source = a
+                    if hasattr(a, "slice") and a.slice is not None:
+                        slices[i] = a.slice
+                    else:
+                        slices[i] = None
+                from .dag import DAG
+                from .steps import Steps
+                if isinstance(self.template, (Steps, DAG)):
+                    for step in self.template:
+                        for name, art in list(step.inputs.artifacts.items()):
+                            if art.source is self.template.inputs.artifacts[k]:
+                                step.set_artifacts({name: {
+                                    i: self.template.inputs.artifacts[
+                                        "dflow_%s_%s" % (k, i)]
+                                    if slice is None else
+                                    self.template.inputs.artifacts[
+                                        "dflow_%s_%s" % (k, i)][slice]
+                                    for i, slice in slices.items()}})
+                else:
+                    for i, a in flat_v.items():
+                        vn = "dflow_%s_%s" % (k, i)
+                        self.template.inputs.artifacts[vn].path = \
+                            "%s/inputs/artifacts/%s" % (self.template.tmp_root,
+                                                        vn)
+                    if any(map(lambda x: x is not None, slices.values())):
+                        self.template.input_artifact_slices[k] = slices
+                    self.template.keys_of_parts[k] = list(v.keys())
+                    self.template.render_script()
+                del self.template.inputs.artifacts[k]
+                del self.inputs.artifacts[k]
             else:
                 self.inputs.artifacts[k].source = v
                 if hasattr(v, "slice") and v.slice is not None:
                     self.input_artifact_slices[k] = v.slice
                     self.template = self.template.copy()
                     if isinstance(v.slice, (InputParameter, OutputParameter)):
                         self.template.inputs.parameters[
                             "dflow_%s" % v.slice.name] = InputParameter()
                         self.inputs.parameters["dflow_%s" % v.slice.name] = \
                             InputParameter(value=v.slice)
                         v.slice = "{{inputs.parameters.dflow_%s}}" % \
                             v.slice.name
-                    from .steps import Steps
                     from .dag import DAG
+                    from .steps import Steps
                     if isinstance(self.template, (Steps, DAG)):
                         for step in self.template:
                             for name, art in step.inputs.artifacts.items():
                                 if art.source is \
                                         self.template.inputs.artifacts[k] or \
                                         hasattr(art.source, "parent") and \
                                         art.source.parent is \
@@ -1191,15 +1212,15 @@
                                     step.set_artifacts({
                                         name: self.template.inputs.artifacts[
                                             k][slice]})
                     else:
                         if k in self.template.input_artifact_slices:
                             old = self.template.input_artifact_slices[k]
                             self.template.input_artifact_slices[k] = \
-                                add_prefix_to_slices(v.slice, old)
+                                add_prefix_to_slice(v.slice, old)
                         else:
                             self.template.input_artifact_slices[k] = v.slice \
                                 if isinstance(v.slice, int) \
                                 else "'%s'" % v.slice
                         self.template.render_script()
                 if config["save_path_as_parameter"]:
                     if isinstance(v, S3Artifact) and v.path_list is not None:
@@ -1303,14 +1324,16 @@
                 self.argo_parameters.append(par.convert_to_argo())
 
         for art in self.inputs.artifacts.values():
             if isinstance(art.source, PVC):
                 pass
             elif art.source is None and art.optional:
                 pass
+            elif art.save_as_parameter:
+                self.argo_parameters.append(art.convert_to_argo())
             else:
                 self.argo_artifacts.append(art.convert_to_argo())
 
         if self.use_resource is not None:
             self.template.resource = V1alpha1ResourceTemplate(
                 action=self.use_resource.action,
                 success_condition=self.use_resource.success_condition,
@@ -1426,14 +1449,18 @@
                     fs = os.listdir(path)
                     if len(fs) == 1 and os.path.isfile(os.path.join(path,
                                                                     fs[0])):
                         os.rename(os.path.join(path, fs[0]), path + ".bk")
                         os.rmdir(path)
                         os.rename(path + ".bk", path)
                     art.source.local_path = path
+                elif isinstance(art.source, HTTPArtifact) and not hasattr(
+                        art.source, "local_path"):
+                    path = os.path.abspath("download/%s" % randstr())
+                    art.source.local_path = art.source.download(path=path)
                 if not hasattr(art.source, "local_path") and art.optional:
                     continue
                 steps.inputs.artifacts[name].local_path = art.source.local_path
 
             if "dflow_key" in steps.inputs.parameters and \
                     steps.inputs.parameters["dflow_key"].value:
                 step_id = steps.inputs.parameters["dflow_key"].value
@@ -1445,15 +1472,16 @@
                                                self.outputs.artifacts)
                     with open(os.path.join(stepdir, "phase"), "r") as f:
                         self.phase = f.read()
                     return
                 os.makedirs(stepdir)
             else:
                 while True:
-                    step_id = self.name + "-" + randstr()
+                    step_id = "%s-%s-%s" % (scope.workflow_id, self.name,
+                                            randstr())
                     stepdir = os.path.abspath(step_id)
                     if not os.path.exists(stepdir):
                         os.makedirs(stepdir)
                         break
 
             with open(os.path.join(stepdir, "type"), "w") as f:
                 if isinstance(self.template, Steps):
@@ -1636,33 +1664,38 @@
                                ignore_nonexist=False):
         os.makedirs(os.path.join(stepdir, "inputs/artifacts"), exist_ok=True)
         for name, art in artifacts.items():
             art_path = os.path.join(stepdir, "inputs/artifacts/%s" % name)
             if isinstance(art.source, str) and art.source.startswith("{{"):
                 if "/" in art.source:
                     i = art.source.find("}}")
-                    art.sub_path = art.source[i+3:]
+                    art.sp = art.source[i+3:]
                     art.source = art.source[:i+2]
                 art.source = get_var(art.source, scope)
             if isinstance(art.source, S3Artifact) and not hasattr(
                     art.source, "local_path"):
                 path = os.path.abspath("download/%s" % randstr())
                 art.source.download(path=path, debug_download=True,
                                     remove_catalog=False)
                 fs = os.listdir(path)
                 if len(fs) == 1 and os.path.isfile(os.path.join(path,
                                                                 fs[0])):
                     os.rename(os.path.join(path, fs[0]), path + ".bk")
                     os.rmdir(path)
                     os.rename(path + ".bk", path)
                 art.source.local_path = path
-            if isinstance(art.source, (InputArtifact, OutputArtifact,
-                                       LocalArtifact, S3Artifact)):
-                if art.sub_path is not None:
-                    sub_path = art.sub_path
+            elif isinstance(art.source, HTTPArtifact) and not hasattr(
+                    art.source, "local_path"):
+                path = os.path.abspath("download/%s" % randstr())
+                art.source.local_path = art.source.download(path=path)
+            if isinstance(
+                art.source, (InputArtifact, OutputArtifact, LocalArtifact,
+                             S3Artifact, HTTPArtifact)):
+                if art.sp is not None:
+                    sub_path = art.sp
                     if item is not None:
                         sub_path = render_item(sub_path, item)
                     os.symlink(os.path.join(art.source.local_path, sub_path),
                                art_path)
                 elif isinstance(
                         art.source,
                         InputArtifact) and art.optional and not hasattr(
@@ -1709,17 +1742,20 @@
             art_path = os.path.join(stepdir, "outputs/artifacts/%s" % name)
             os.symlink(art.local_path, art_path)
             if art.global_name is not None:
                 os.makedirs(os.path.join(stepdir, "../outputs/artifacts"),
                             exist_ok=True)
                 global_art_path = os.path.join(
                     stepdir, "../outputs/artifacts/%s" % art.global_name)
-                if os.path.exists(global_art_path):
-                    os.remove(global_art_path)
-                os.symlink(art_path, global_art_path)
+                while True:
+                    try:
+                        os.symlink(art_path, global_art_path)
+                        break
+                    except FileExistsError:
+                        os.remove(global_art_path)
 
     def load_output_parameters(self, stepdir, parameters):
         for name, par in parameters.items():
             par_path = os.path.join(stepdir,
                                     "outputs/parameters/%s" % name)
             with open(par_path, "r") as f:
                 if par.type is None or par.type == str:
@@ -1749,14 +1785,19 @@
         self.phase = "Running"
 
         # render item
         if item is not None:
             for name, par in parameters.items():
                 if isinstance(par.value, str):
                     par.value = render_item(par.value, item)
+            for name, art in self.inputs.artifacts.items():
+                if isinstance(art.source, S3Artifact):
+                    art.source.key = render_item(art.source.key, item)
+                elif isinstance(art.source, HTTPArtifact):
+                    art.source.url = render_item(art.source.url, item)
 
         import os
         cwd = os.getcwd()
         if "dflow_key" in parameters:
             step_id = parameters["dflow_key"].value
             stepdir = os.path.abspath(step_id)
             if os.path.exists(stepdir):
@@ -1768,15 +1809,16 @@
                 os.chdir(cwd)
                 with open(os.path.join(stepdir, "phase"), "r") as f:
                     self.phase = f.read()
                 return
             os.makedirs(stepdir)
         else:
             while True:
-                step_id = self.name + "-" + randstr()
+                step_id = "%s-%s-%s" % (scope.workflow_id, self.name,
+                                        randstr())
                 stepdir = os.path.abspath(step_id)
                 if not os.path.exists(stepdir):
                     os.makedirs(stepdir)
                     break
 
         self.stepdir = stepdir
         with open(os.path.join(stepdir, "type"), "w") as f:
@@ -1805,23 +1847,17 @@
             if isinstance(
                     art.source,
                     InputArtifact) and art.source is None and art.optional:
                 pass
             else:
                 os.symlink(art_path, path)
 
-        # clean output path
-        for art in self.outputs.artifacts.values():
-            path = art.path
-            path = "%s/%s" % (workdir, path)
-            backup(path)
-
         # render variables in the script
         script = self.template.script
-        if self.executor is None:
+        if not self.template.script_rendered:
             if hasattr(self.template, "tmp_root"):
                 # do not modify self.template
                 template = deepcopy(self.template)
                 template.tmp_root = "%s%s" % (workdir, template.tmp_root)
                 template.render_script()
                 script = template.script
             else:
@@ -1844,14 +1880,16 @@
                 while line:
                     sys.stdout.write(line)
                     f.write(line)
                     line = p.stdout.readline().decode(sys.stdout.encoding)
             p.wait()
             ret_code = p.poll()
         if ret_code != 0:
+            with open(os.path.join(stepdir, "phase"), "w") as f:
+                f.write("Failed")
             raise RuntimeError("Run %s failed" % args)
 
         # generate output parameters
         for name, par in self.outputs.parameters.items():
             path = par.value_from_path
             if path is not None:
                 path = "%s/%s" % (workdir, path)
@@ -2054,7 +2092,98 @@
     expr = expr.replace("sprig.untilStep",
                         "(lambda *x: list(range(*list(map(int, x)))))")
     expr = expr.replace("sprig.atoi", "int")
     expr = expr.replace(" ? ", " and ")
     expr = expr.replace(" : ", " or ")
     expr = expr.replace("asFloat", "float")
     return expr
+
+
+def add_slices(templ: OPTemplate, slices: Slices, input_artifact_prefix=None):
+    if input_artifact_prefix is None:
+        input_artifact_prefix = {}
+    templ.inputs.parameters["dflow_slice"] = InputParameter(
+        value=slices.slices)
+
+    for name in slices.input_parameter:
+        for step in templ:
+            for par in list(step.inputs.parameters.values()):
+                # input parameter referring to sliced input parameter
+                if par.value is templ.inputs.parameters[name]:
+                    step.template.inputs.parameters["dflow_slice"] = \
+                        InputParameter()
+                    step.template.add_slices(Slices(
+                        "{{inputs.parameters.dflow_slice}}",
+                        input_parameter=[par.name],
+                        sub_path=slices.sub_path,
+                        pool_size=slices.pool_size))
+                    step.inputs.parameters["dflow_slice"] = InputParameter(
+                        value="{{inputs.parameters.dflow_slice}}")
+
+    for name in slices.input_artifact:
+        for step in templ:
+            for art in list(step.inputs.artifacts.values()):
+                print(art.source, art.source is templ.inputs.artifacts[name])
+                # input artifact referring to sliced input artifact
+                if art.source is templ.inputs.artifacts[name] or getattr(
+                    art.source, "parent", None) is \
+                        templ.inputs.artifacts[name]:
+                    if name in input_artifact_prefix:
+                        slice = input_artifact_prefix[name]
+                        pattern = add_prefix_to_slice(
+                            slice, "{{inputs.parameters.dflow_slice}}")
+                    else:
+                        pattern = "{{inputs.parameters.dflow_slice}}"
+                    step.template.inputs.parameters["dflow_slice"] = \
+                        InputParameter()
+                    step.template.add_slices(Slices(
+                        pattern,
+                        input_artifact=[art.name],
+                        sub_path=slices.sub_path,
+                        pool_size=slices.pool_size))
+                    step.inputs.parameters["dflow_slice"] = InputParameter(
+                        value="{{inputs.parameters.dflow_slice}}")
+
+    def stack_output_parameter(par):
+        if isinstance(par, OutputParameter):
+            step = par.step
+            step.template.inputs.parameters["dflow_slice"] = InputParameter()
+            step.template.add_slices(Slices(
+                "{{inputs.parameters.dflow_slice}}",
+                output_parameter=[par.name],
+                sub_path=slices.sub_path,
+                pool_size=slices.pool_size))
+            step.inputs.parameters["dflow_slice"] = InputParameter(
+                value="{{inputs.parameters.dflow_slice}}")
+
+    for name in slices.output_parameter:
+        # sliced output parameter from
+        if templ.outputs.parameters[name].value_from_parameter is not None:
+            stack_output_parameter(
+                templ.outputs.parameters[name].value_from_parameter)
+        elif templ.outputs.parameters[name].value_from_expression is not None:
+            stack_output_parameter(
+                templ.outputs.parameters[name].value_from_expression._then)
+            stack_output_parameter(
+                templ.outputs.parameters[name].value_from_expression._else)
+
+    def stack_output_artifact(art):
+        if isinstance(art, OutputArtifact):
+            step = art.step
+            step.template.inputs.parameters["dflow_slice"] = InputParameter()
+            step.template.add_slices(Slices(
+                "{{inputs.parameters.dflow_slice}}",
+                output_artifact=[art.name],
+                sub_path=slices.sub_path,
+                pool_size=slices.pool_size))
+            step.inputs.parameters["dflow_slice"] = InputParameter(
+                value="{{inputs.parameters.dflow_slice}}")
+
+    for name in slices.output_artifact:
+        # sliced output artifact from
+        if templ.outputs.artifacts[name]._from is not None:
+            stack_output_artifact(templ.outputs.artifacts[name]._from)
+        elif templ.outputs.artifacts[name].from_expression is not None:
+            stack_output_artifact(
+                templ.outputs.artifacts[name].from_expression._then)
+            stack_output_artifact(
+                templ.outputs.artifacts[name].from_expression._else)
```

### Comparing `pydflow-1.6.99/src/dflow/steps.py` & `pydflow-1.7.0/src/dflow/steps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from copy import deepcopy
-from typing import Optional, Dict, List, Union
+from typing import Dict, List, Optional, Union
 
 from .config import config, s3_config
 from .io import Inputs, Outputs
 from .op_template import OPTemplate
-from .step import Step
+from .step import Step, add_slices
 
 try:
     from argo.workflows.client import V1alpha1Metadata, V1alpha1Template
 except Exception:
     pass
 
 
@@ -143,7 +143,10 @@
                         step[j].phase = "Failed"
                         if not step[j].continue_on_failed:
                             raise RuntimeError("Step %s failed" % step[j])
                     else:
                         step[j].outputs = deepcopy(ps.outputs)
             else:
                 step.run(self, context)
+
+    def add_slices(self, slices, input_artifact_prefix=None):
+        add_slices(self, slices, input_artifact_prefix)
```

### Comparing `pydflow-1.6.99/src/dflow/task.py` & `pydflow-1.7.0/src/dflow/task.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import Optional, List
+from typing import List, Optional, Union
 
 from .io import OutputArtifact, OutputParameter
 from .op_template import OPTemplate
 from .step import Step
 
 try:
-    from argo.workflows.client import (V1alpha1Arguments, V1alpha1ContinueOn,
-                                       V1alpha1DAGTask)
+    from argo.workflows.client import V1alpha1Arguments, V1alpha1DAGTask
 except Exception:
     pass
 
 
 class Task(Step):
     """
     Task
@@ -38,15 +37,15 @@
         dependencies: extra dependencies of the task
     """
 
     def __init__(
             self,
             name: str,
             template: OPTemplate,
-            dependencies: Optional[List["Task"]] = None,
+            dependencies: Optional[List[Union["Task", str]]] = None,
             **kwargs,
     ) -> None:
         if dependencies is None:
             dependencies = []
         self.dependencies = dependencies
         super().__init__(name=name, template=template, **kwargs)
         if self.prepare_step is not None:
@@ -58,31 +57,46 @@
     def from_dict(cls, d, templates):
         task = super().from_dict(d, templates)
         task.dependencies = d.get("dependencies", [])
         return task
 
     def set_parameters(self, parameters):
         super().set_parameters(parameters)
-        for v in parameters.values():
-            if isinstance(v, (OutputParameter, OutputArtifact)) and v.step \
-                    not in self.dependencies:
-                self.dependencies.append(v.step)
+        for v in self.inputs.parameters.values():
+            if hasattr(v, "value"):
+                def handle(obj):
+                    # TODO: Only support output parameter, dict and list
+                    if isinstance(obj, OutputParameter):
+                        if obj.step not in self.dependencies:
+                            self.dependencies.append(obj.step)
+                    elif isinstance(obj, dict):
+                        for v in obj.values():
+                            handle(v)
+                    elif isinstance(obj, list):
+                        for v in obj:
+                            handle(v)
+                handle(v.value)
 
     def set_artifacts(self, artifacts):
         super().set_artifacts(artifacts)
-        for v in artifacts.values():
-            if isinstance(v, OutputArtifact) and v.step not in \
+        for v in self.inputs.artifacts.values():
+            if isinstance(v.source, OutputArtifact) and v.source.step not in \
                     self.dependencies:
-                self.dependencies.append(v.step)
+                self.dependencies.append(v.source.step)
 
     def convert_to_argo(self, context=None):
         self.prepare_argo_arguments(context)
+        depends = []
+        for task in self.dependencies:
+            if isinstance(task, Task):
+                depends.append("(%s.Succeeded)" % task)
+            else:
+                depends.append("(%s)" % task)
         return V1alpha1DAGTask(
             name=self.name, template=self.template.name,
             arguments=V1alpha1Arguments(
                 parameters=self.argo_parameters,
                 artifacts=self.argo_artifacts
             ), when=self.when, with_param=self.with_param,
             with_sequence=self.with_sequence,
-            continue_on=V1alpha1ContinueOn(failed=self.continue_on_failed),
-            dependencies=[task.name for task in self.dependencies],
+            depends=" && ".join(depends),
         )
```

### Comparing `pydflow-1.6.99/src/dflow/util_ops.py` & `pydflow-1.7.0/src/dflow/util_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 from .config import config
 from .io import (InputArtifact, InputParameter, Inputs, OutputArtifact,
                  OutputParameter)
 from .op_template import PythonScriptOPTemplate, ShellOPTemplate
 
 
 class InitArtifactForSlices(PythonScriptOPTemplate):
-    def __init__(self, name, image, command, image_pull_policy, key,
+    def __init__(self, template, image, command, image_pull_policy, key,
                  sliced_output_artifact, sliced_input_artifact, sum_var,
                  concat_var, tmp_root="/tmp"):
+        name = template.name
         super().__init__(name="%s-init-artifact" % name, image=image,
                          command=command, image_pull_policy=image_pull_policy)
+        self.origin = template
         self.key = key
         self.sliced_output_artifact = sliced_output_artifact
         self.sliced_input_artifact = sliced_input_artifact
         self.sum_var = sum_var
         self.concat_var = concat_var
         self.tmp_root = tmp_root
 
@@ -38,14 +40,20 @@
                 self.outputs.artifacts[name] = OutputArtifact(
                     path="%s/outputs/artifacts/%s" % (self.tmp_root, name),
                     save=S3Artifact(key="{{workflow.name}}/{{pod.name}}/%s"
                                     % name),
                     archive=None)
 
         if self.sliced_input_artifact:
+            if self.key is not None:
+                self.inputs.parameters["dflow_key"] = InputParameter()
+                self.outputs.parameters["dflow_global"] = OutputParameter(
+                    value="{{pod.name}}",
+                    global_name="{{inputs.parameters.dflow_key}}",
+                )
             for name in self.sliced_input_artifact:
                 self.inputs.artifacts[name] = InputArtifact(
                     path="%s/inputs/artifacts/%s" % (self.tmp_root, name),
                     optional=True, sub_path=config["catalog_dir_name"])
                 self.outputs.parameters["dflow_slices_path"] = OutputParameter(
                     value_from_path="%s/outputs/parameters/dflow_slices_path"
                     % self.tmp_root, type=dict)
@@ -74,38 +82,42 @@
                                       config["catalog_dir_name"])
             script += "with open(r'%s/outputs/artifacts/%s/%s/init',"\
                 " 'w') as f:\n" % (self.tmp_root, name,
                                    config["catalog_dir_name"])
             script += "    json.dump({'path_list': []}, f)\n"
 
         if self.sliced_input_artifact:
+            required = []
             for i, name in enumerate(self.sliced_input_artifact):
                 script += "path_list_%s = []\n" % i
                 script += "path = r'%s/inputs/artifacts/%s'\n" % \
                     (self.tmp_root, name)
                 script += "if os.path.exists(path):\n"
                 script += "    for f in os.listdir(path):\n"
                 script += "        with open(os.path.join(path, f), 'r')"\
                     " as fd:\n"
-                script += "            path_list_%s += json.load(fd)"\
-                    "['path_list']\n" % i
+                script += "            for i in json.load(fd)['path_list']:\n"
+                script += "                if i not in path_list_%s:\n" % i
+                script += "                    path_list_%s.append(i)\n" % i
                 script += "path_list_%s.sort(key=lambda x: x['order'])\n" \
                     % i
+                if not self.origin.inputs.artifacts[name].optional:
+                    required.append(i)
 
-            n_arts = len(self.sliced_input_artifact)
-            if n_arts > 1:
+            if len(required) > 1:
                 script += "assert " + " == ".join(
-                    ["len(path_list_%s)" % i for i in range(n_arts)]) + "\n"
+                    ["len(path_list_%s)" % i for i in required]) + "\n"
 
             script += "slices_path = []\n"
-            script += "for i in range(len(path_list_0)):\n"
+            script += "for i in range(len(path_list_%s)):\n" % required[0]
             script += "    item = {'order': i}\n"
             for i, name in enumerate(self.sliced_input_artifact):
                 script += "    item['%s'] = path_list_%s[i]"\
-                    "['dflow_list_item']\n" % (name, i)
+                    "['dflow_list_item'] if path_list_%s else None\n" % (
+                        name, i, i)
             script += "    slices_path.append(item)\n"
             script += "os.makedirs(r'%s/outputs/parameters', exist_ok=True)\n"\
                 % self.tmp_root
             script += "with open(r'%s/outputs/parameters/dflow_slices_path',"\
                 " 'w') as f:\n" % self.tmp_root
             script += "    json.dump(slices_path, f)\n"
```

### Comparing `pydflow-1.6.99/src/dflow/utils.py` & `pydflow-1.7.0/src/dflow/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,14 +92,16 @@
         linktree(artifact.local_path, path)
         return assemble_path_list(path, remove=remove_catalog)
 
     key = get_key(artifact)
 
     if slice is not None:
         sub_path = path_list_of_artifact(artifact)[slice]
+
+    if sub_path is not None:
         key = key + "/" + sub_path
         path = os.path.join(path, os.path.dirname(sub_path))
         download_s3(key=key, recursive=True, path=path, keep_dir=True,
                     **kwargs)
         path = os.path.join(path, os.path.basename(sub_path))
         remove_empty_dir_tag(path)
         return path
@@ -123,14 +125,67 @@
             else:
                 merge_dir(tmpdir, path)
 
     remove_empty_dir_tag(path)
     return assemble_path_list(path, remove=remove_catalog)
 
 
+def flatten(d: Union[list, dict]) -> dict:
+    def handle(obj, prefix):
+        if isinstance(obj, dict):
+            for k, v in obj.items():
+                key = prefix + "." + k if prefix else k
+                if isinstance(v, (list, dict)):
+                    handle(v, key)
+                else:
+                    flat[key] = v
+        elif isinstance(obj, list):
+            for i, v in enumerate(obj):
+                key = prefix + "." + str(i) if prefix else str(i)
+                if isinstance(v, (list, dict)):
+                    handle(v, key)
+                else:
+                    flat[key] = v
+    flat = {}
+    handle(d, "")
+    return flat
+
+
+def dict2list(d: dict):
+    for k, v in d.items():
+        if isinstance(v, dict):
+            d[k] = dict2list(v)
+    try:
+        lst = []
+        for k, v in d.items():
+            i = int(k)
+            if i < len(lst):
+                lst[i] = v
+            else:
+                lst += [None] * (i - len(lst)) + [v]
+        return lst
+    except Exception:
+        return d
+
+
+def expand(d: dict) -> Union[list, dict]:
+    exp = {}
+    for k, v in d.items():
+        fields = str(k).split(".")
+        tmp = exp
+        for field in fields[:-1]:
+            if field not in tmp:
+                tmp[field] = {}
+            tmp = tmp[field]
+        field = fields[-1]
+        tmp[field] = v
+    exp = dict2list(exp)
+    return exp
+
+
 def upload_artifact(
         path: Union[os.PathLike, List[os.PathLike], Set[os.PathLike],
                     Dict[str, os.PathLike], list, dict],
         archive: str = "default",
         namespace: Optional[str] = None,
         dataset_name: Optional[str] = None,
         **kwargs,
@@ -147,39 +202,21 @@
         secure: secure or not for Minio
         bucket_name: bucket name for Minio
     """
     if archive == "default":
         archive = config["archive_mode"]
     cwd = os.getcwd()
     with tempfile.TemporaryDirectory() as tmpdir:
-        path_list = []
-        pairs = []
-
-        def handle(obj, prefix):
-            if isinstance(obj, dict):
-                for k, v in obj.items():
-                    key = prefix + "." + k if prefix else k
-                    if isinstance(v, (list, dict)):
-                        handle(v, key)
-                    elif isinstance(v, (str, Path)):
-                        pairs.append((key, v))
-            elif isinstance(obj, list):
-                for i, v in enumerate(obj):
-                    key = prefix + "." + str(i) if prefix else str(i)
-                    if isinstance(v, (list, dict)):
-                        handle(v, key)
-                    elif isinstance(v, (str, Path)):
-                        pairs.append((key, v))
-
         if isinstance(path, dict):
-            handle(path, "")
+            pairs = flatten(path).items()
         elif isinstance(path, (list, set)):
             pairs = enumerate(path)
         else:
             pairs = [(0, path)]
+        path_list = []
         for i, p in pairs:
             logging.debug("upload artifact: handle path: %s" % p)
             if p is None:
                 continue
             if not os.path.exists(p):
                 raise RuntimeError("File or directory %s not found" % p)
             abspath = os.path.abspath(p)
@@ -286,15 +323,16 @@
         **kwargs,
 ) -> str:
     if s3_config["storage_client"] is not None:
         client = s3_config["storage_client"]
     else:
         client = MinioClient(**kwargs)
     if recursive:
-        for obj in client.list(prefix=key, recursive=True):
+        from tqdm import tqdm
+        for obj in tqdm(client.list(prefix=key, recursive=True)):
             rel_path = obj[len(key):]
             if rel_path[:1] == "/":
                 rel_path = rel_path[1:]
             if rel_path == "":
                 file_path = os.path.join(path, os.path.basename(key))
             elif keep_dir:
                 file_path = os.path.join(path, os.path.basename(key), rel_path)
@@ -494,60 +532,16 @@
                     path_dict[item["order"]] = None
                 else:
                     path_dict[item["order"]] = os.path.join(
                         art_path, item["dflow_list_item"])
     return path_dict
 
 
-def dict2list(d: dict):
-    for k, v in d.items():
-        if isinstance(v, dict):
-            d[k] = dict2list(v)
-    try:
-        lst = []
-        for k, v in d.items():
-            i = int(k)
-            if i < len(lst):
-                lst[i] = v
-            else:
-                lst += [None] * (i - len(lst)) + [v]
-        return lst
-    except Exception:
-        return d
-
-
 def assemble_path_nested_dict(art_path, remove=False):
-    path_dict = {}
-    if os.path.isdir(art_path):
-        dflow_list = []
-        catalog_dir = os.path.join(art_path, config["catalog_dir_name"])
-        if os.path.exists(catalog_dir):
-            for f in os.listdir(catalog_dir):
-                with open(os.path.join(catalog_dir, f), 'r') as fd:
-                    for item in jsonpickle.loads(fd.read())['path_list']:
-                        if item not in dflow_list:
-                            dflow_list.append(item)  # remove duplicate
-            if remove:
-                shutil.rmtree(catalog_dir)
-        if len(dflow_list) > 0:
-            for item in dflow_list:
-                fields = str(item["order"]).split(".")
-                tmp = path_dict
-                for field in fields[:-1]:
-                    if field not in tmp:
-                        tmp[field] = {}
-                    tmp = tmp[field]
-                field = fields[-1]
-                if item["dflow_list_item"] is None:
-                    tmp[field] = None
-                else:
-                    tmp[field] = os.path.join(
-                        art_path, item["dflow_list_item"])
-            path_dict = dict2list(path_dict)
-    return path_dict
+    return expand(assemble_path_dict(art_path, remove))
 
 
 def remove_empty_dir_tag(path):
     for dn, ds, fs in os.walk(path, followlinks=True):
         if ".empty_dir" in fs:
             os.remove(os.path.join(dn, ".empty_dir"))
 
@@ -644,14 +638,15 @@
         stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         **kwargs,
     ) as sub:
         if input is not None:
             sub.stdin.write(bytes(input, encoding=sys.stdout.encoding))
+            sub.stdin.close()
         if print_oe:
             out = ""
             err = ""
             sel = selectors.DefaultSelector()
             sel.register(sub.stdout, selectors.EVENT_READ)
             sel.register(sub.stderr, selectors.EVENT_READ)
             ok = True
@@ -780,7 +775,13 @@
     def copy(self, src: str, dst: str) -> None:
         self.client.copy_object(self.bucket_name, dst,
                                 CopySource(self.bucket_name, src))
 
     def get_md5(self, key: str) -> str:
         return self.client.stat_object(bucket_name=self.bucket_name,
                                        object_name=key).etag
+
+
+def add_prefix_to_slice(prefix, slices):
+    return "(lambda x: ['%s.' + str(i) for i in x] "\
+        "if isinstance(x, list) else '%s.' + str(x))(%s)" % (
+            prefix, prefix, slices)
```

### Comparing `pydflow-1.6.99/src/dflow/workflow.py` & `pydflow-1.7.0/src/dflow/workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 import os
+import sys
 import time
 from copy import deepcopy
 from typing import Any, Dict, List, Optional, Union
 
 import jsonpickle
 
 from .argo_objects import ArgoStep, ArgoWorkflow
@@ -103,16 +104,16 @@
             k8s_config_file: Optional[os.PathLike] = None,
             k8s_api_server: Optional[str] = None,
             context: Optional[Union[Context, Executor]] = None,
             annotations: Dict[str, str] = None,
             labels: Dict[str, str] = None,
             parallelism: Optional[int] = None,
             pod_gc_strategy: Optional[str] = None,
-            image_pull_secrets: Union[str, DockerSecret,
-                                      List[Union[str, DockerSecret]]] = None,
+            image_pull_secrets: Optional[Union[
+                str, DockerSecret, List[Union[str, DockerSecret]]]] = None,
             artifact_repo_key: Optional[str] = None,
             parameters: Optional[Dict[str, Any]] = None,
     ) -> None:
         self.host = host if host is not None else config["host"]
         self.token = token if token is not None else config["token"]
         self.k8s_config_file = k8s_config_file if k8s_config_file is not None \
             else config["k8s_config_file"]
@@ -154,31 +155,17 @@
         self.templates = {}
         self.argo_templates = {}
         self.pvcs = {}
         if parameters is None:
             parameters = {}
         self.parameters = parameters
         self.k8s_client = None
-
-        if self.artifact_repo_key is not None:
-            core_v1_api = self.get_k8s_core_v1_api()
-            cm = core_v1_api.read_namespaced_config_map(
-                namespace=self.namespace, name="artifact-repositories")
-            repo = yaml.full_load(cm.data[self.artifact_repo_key])
-            s3_config["repo"] = repo
-            if "s3" in repo:
-                s3_config["repo_type"] = "s3"
-                s3 = repo["s3"]
-            elif "oss" in repo:
-                s3_config["repo_type"] = "oss"
-                s3 = repo["oss"]
-            if "keyFormat" in s3:
-                t = "{{workflow.name}}/{{pod.name}}"
-                if s3["keyFormat"].endswith(t):
-                    s3_config["repo_prefix"] = s3["keyFormat"][:-len(t)]
+        parse_repo(self.artifact_repo_key, self.namespace,
+                   k8s_api_server=self.k8s_api_server, token=self.token,
+                   k8s_config_file=self.k8s_config_file)
 
     def get_k8s_core_v1_api(self):
         if self.k8s_client is None:
             self.k8s_client = get_k8s_client(self.k8s_api_server, self.token,
                                              self.k8s_config_file)
         return kubernetes.client.CoreV1Api(self.k8s_client)
 
@@ -221,14 +208,17 @@
             if self.id is None:
                 while True:
                     self.id = self.name + "-" + randstr()
                     wfdir = os.path.abspath(self.id)
                     if not os.path.exists(wfdir):
                         os.makedirs(wfdir)
                         break
+            else:
+                wfdir = os.path.abspath(self.id)
+                os.makedirs(wfdir, exist_ok=True)
 
             if reuse_step is not None:
                 for step in reuse_step:
                     if step.key is None:
                         continue
                     stepdir = os.path.join(wfdir, step.key)
                     os.makedirs(stepdir, exist_ok=True)
@@ -288,29 +278,39 @@
                                     stepdir, io, "artifacts", name))
 
             cwd = os.getcwd()
             os.chdir(wfdir)
             print("Workflow is running locally (ID: %s)" % self.id)
             with open(os.path.join(wfdir, "status"), "w") as f:
                 f.write("Running")
+            if config["detach"]:
+                pid = os.fork()
+                if pid != 0:
+                    os.chdir(cwd)
+                    return ArgoWorkflow({"id": self.id})
+                flog = open(os.path.join(wfdir, "log.txt"), "w")
+                os.dup2(flog.fileno(), sys.stdout.fileno())
+                os.dup2(flog.fileno(), sys.stderr.fileno())
             try:
                 entrypoint = deepcopy(self.entrypoint)
                 entrypoint.orig_template = self.entrypoint
                 entrypoint.run(self.id, self.context)
                 with open(os.path.join(wfdir, "status"), "w") as f:
                     f.write("Succeeded")
             except Exception:
                 import traceback
                 traceback.print_exc()
                 with open(os.path.join(wfdir, "status"), "w") as f:
                     f.write("Failed")
+            if config["detach"]:
+                flog.close()
+                exit()
             os.chdir(cwd)
             return ArgoWorkflow({"id": self.id})
 
-        assert self.id is None, "Do not submit a workflow repeatedly"
         manifest = self.convert_to_argo(reuse_step=reuse_step)
 
         logger.debug("submit manifest:\n%s" % manifest)
         response = self.api_instance.api_client.call_api(
             '/api/v1/workflows/%s' % self.namespace, 'POST',
             body=V1alpha1WorkflowCreateRequest(workflow=manifest),
             response_type=object,
@@ -372,14 +372,16 @@
         art_key_prefix = art_key
         if art_key_prefix.startswith(s3_config["prefix"]):
             art_key_prefix = art_key_prefix[len(s3_config["prefix"]):]
         if art_key_prefix.endswith(name):
             art_key_prefix = art_key_prefix[:-len(name)-1]
 
         group_key = step.inputs.parameters["dflow_group_key"].value
+        if "%s-init-artifact" % group_key in self.reused_keys:
+            return
         memoize_key = "%s-%s-init-artifact" % (self.id, group_key)
         if memoize_key not in self.memoize_map:
             self.memoize_map[memoize_key] = {
                 "nodeID": "dflow-%s" % randstr(10),
                 "outputs": {
                     "parameters": [{
                         "name": "dflow_artifact_key",
@@ -419,15 +421,18 @@
     def convert_to_argo(self, reuse_step=None):
         if self.context is not None:
             assert isinstance(self.context, (Context, Executor))
             self = self.context.render(self)
 
         status = None
         if reuse_step is not None:
-            self.id = self.name + "-" + randstr()
+            self.reused_keys = [step.key for step in reuse_step
+                                if step.key is not None]
+            if self.id is None:
+                self.id = self.name + "-" + randstr()
             self.copied_keys = []
             self.memoize_map = {}
             key2id = {}
             for step in reuse_step:
                 data = {}
                 if step.key is None:
                     continue
@@ -589,14 +594,44 @@
             step = Step("main", entrypoint,
                         parameters=kwargs.pop("parameters"))
             kwargs["steps"].add(step)
         elif isinstance(entrypoint, Steps):
             kwargs["steps"] = entrypoint
         elif isinstance(entrypoint, DAG):
             kwargs["dag"] = entrypoint
+        engine = d.get("metadata", {}).get("annotations", {}).get(
+            "workflow.dp.tech/container_engine")
+        docker = "docker" if engine == "docker" else None
+        singularity = "singularity" if engine == "singularity" else None
+        podman = "podman" if engine == "podman" else None
+        if d.get("metadata", {}).get("annotations", {}).get(
+                "workflow.dp.tech/executor") == "dispatcher":
+            host = kwargs["annotations"].get("workflow.dp.tech/host")
+            port = int(kwargs["annotations"].get("workflow.dp.tech/port", 22))
+            username = kwargs["annotations"].get(
+                "workflow.dp.tech/username", "root")
+            password = kwargs["annotations"].get("workflow.dp.tech/password")
+            queue_name = kwargs["annotations"].get(
+                "workflow.dp.tech/queue_name")
+            extras = kwargs["annotations"].get("workflow.dp.tech/extras")
+            extras = json.loads(extras) if extras else {}
+            machine = extras.get("machine", None)
+            resources = extras.get("resources", None)
+            task = extras.get("task", None)
+            clean = extras.get("clean", True)
+            from .plugins.dispatcher import DispatcherExecutor
+            kwargs["context"] = DispatcherExecutor(
+                host, queue_name, port, username, password,
+                machine_dict=machine, resources_dict=resources,
+                task_dict=task, docker_executable=docker,
+                singularity_executable=singularity, podman_executable=podman,
+                clean=clean)
+        elif engine:
+            from .executor import ContainerExecutor
+            kwargs["context"] = ContainerExecutor(docker, singularity, podman)
         return cls(**kwargs)
 
     def handle_template(self, template, memoize_prefix=None,
                         memoize_configmap="dflow"):
         if template.name in self.templates:
             assert template == self.templates[template.name], \
                 "Duplication of template name: %s" % template.name
@@ -660,15 +695,15 @@
 
         Returns:
             Pending, Running, Succeeded, Failed, Error, etc
         """
         if config["mode"] == "debug":
             with open("%s/status" % self.id, "r") as f:
                 return f.read()
-        workflow = self.query(fields=["status"])
+        workflow = self.query(fields=["status.phase"])
 
         if "phase" not in workflow.status:
             return "Pending"
         else:
             return workflow.status.phase
 
     def query_step(
@@ -702,15 +737,15 @@
             if key is not None and not isinstance(key, list):
                 key = [key]
             step_list = []
             for s in os.listdir(self.id):
                 stepdir = os.path.join(self.id, s)
                 if not os.path.isdir(stepdir):
                     continue
-                if name is not None and not s[:len(name)] == name:
+                if name is not None and not s.startswith(self.id + "-" + name):
                     continue
                 if key is not None and s not in key:
                     continue
                 if not os.path.exists(os.path.join(stepdir, "type")):
                     continue
                 with open(os.path.join(stepdir, "type"), "r") as f:
                     _type = f.read()
@@ -991,7 +1026,31 @@
         res = api_client.call_api(
             '/api/v1/archived-workflows',
             'GET', response_type='object',
             header_params=config["http_headers"],
             query_params=query_params,
             _return_http_data_only=True)
     return [ArgoWorkflow(w) for w in res["items"]] if res["items"] else []
+
+
+def parse_repo(repo_key=None, namespace=None, **kwargs):
+    if repo_key is None:
+        repo_key = s3_config["repo_key"]
+    if namespace is None:
+        namespace = config["namespace"]
+    if repo_key is not None and s3_config["repo"] is None:
+        with get_k8s_client(**kwargs) as k8s_client:
+            core_v1_api = kubernetes.client.CoreV1Api(k8s_client)
+            cm = core_v1_api.read_namespaced_config_map(
+                namespace=namespace, name="artifact-repositories")
+            repo = yaml.full_load(cm.data[repo_key])
+            s3_config["repo"] = repo
+            if "s3" in repo:
+                s3_config["repo_type"] = "s3"
+                s3 = repo["s3"]
+            elif "oss" in repo:
+                s3_config["repo_type"] = "oss"
+                s3 = repo["oss"]
+            if "keyFormat" in s3:
+                t = "{{workflow.name}}/{{pod.name}}"
+                if s3["keyFormat"].endswith(t):
+                    s3_config["repo_prefix"] = s3["keyFormat"][:-len(t)]
```

### Comparing `pydflow-1.6.99/src/pydflow.egg-info/PKG-INFO` & `pydflow-1.7.0/src/pydflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,191 +1,108 @@
 Metadata-Version: 2.1
 Name: pydflow
-Version: 1.6.99
+Version: 1.7.0
 Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
+Home-page: https://github.com/deepmodeling/dflow
 Author: Xinzijian Liu
+Author-email: liuxzj@dp.tech
 License: LGPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DFLOW
 
 [Dflow](https://deepmodeling.com/dflow/dflow.html) is a Python framework for constructing scientific computing workflows (e.g. concurrent learning workflows) employing [Argo Workflows](https://argoproj.github.io/) as the workflow engine.
 
 For dflow's users (e.g. ML application developers), dflow offers user-friendly functional programming interfaces for building their own workflows. Users need not be concerned with process control, task scheduling, observability and disaster tolerance. Users can track workflow status and handle exceptions by APIs as well as from frontend UI. Thereby users are enabled to concentrate on implementing operations (OPs) and orchestrating workflows.
 
-For dflow's developers, dflow wraps on argo SDK, keeps details of computing and storage resources from users, and provides extension abilities. While argo is a cloud-native workflow engine, dflow uses containers to decouple computing logic and scheduling logic, and uses Kubernetes to make workflows observable, reproducible and robust. Dflow is designed to be based on a distributed, heterogeneous infrastructure. The most common computing resources in scientific computing may be HPC clusters. User can either use executor to manage HPC jobs within dflow ([dflow-extender](https://github.com/dptech-corp/dflow-extender)) or using [DPDispatcher](https://github.com/deepmodeling/dpdispatcher) plugin, or use virtual node technique to uniformly manage HPC resources in the framework of Kubernetes ([wlm-operator](https://github.com/dptech-corp/wlm-operator)).
+For dflow's developers, dflow wraps on argo SDK, keeps details of computing and storage resources from users, and provides extension abilities. While argo is a cloud-native workflow engine, dflow uses containers to decouple computing logic and scheduling logic, and uses Kubernetes to make workflows observable, reproducible and robust. Dflow is designed to be based on a distributed, heterogeneous infrastructure. The most common computing resources in scientific computing may be HPC clusters. User can either use executor to manage HPC jobs using [DPDispatcher](https://github.com/deepmodeling/dpdispatcher) plugin, or use virtual node technique to uniformly manage HPC resources in the framework of Kubernetes ([wlm-operator](https://github.com/dptech-corp/wlm-operator)).
 
-Dflow's OPs can be reused among workflows and shared among users. Dflow provides a cookie cutter recipe [dflow-op-cutter](https://github.com/deepmodeling/dflow-op-cutter) for template a new OP package. Start developing an OP package at once from
+OP template (abbr. OP) in dflow can be reused among workflows and shared among users. Dflow provides a cookie cutter recipe [dflow-op-cutter](https://github.com/deepmodeling/dflow-op-cutter) for template a new OP package. Start developing an OP package at once from
 ```python
 pip install cookiecutter
 cookiecutter https://github.com/deepmodeling/dflow-op-cutter.git
 ```
 
 Dflow provides a debug mode for running workflows bare-metally whose backend is implemented in dflow in pure Python, independent of Argo/Kubernetes. The debug mode uses local environment to execute OPs instead of containers. It implements most APIs of the default mode in order to provide an identical user experience. The debug mode offer convenience for debugging or testing without container. For the clusters having problem deploying docker and Kubernetes and difficult to access from outside, the debug mode may also be used for production, despite less robustness and observability.
 
 <!-- vscode-markdown-toc -->
 * 1. [ Overview](#Overview)
 	* 1.1. [ Architecture](#Architecture)
-	* 1.2. [ Common layer](#Commonlayer)
+	* 1.2. [ Basics](#Basics)
 		* 1.2.1. [ Parameters and artifacts](#Parametersandartifacts)
 		* 1.2.2. [ OP template](#OPtemplate)
 		* 1.2.3. [ Step](#Step)
 		* 1.2.4. [ Workflow](#Workflow)
-	* 1.3. [ Interface layer](#Interfacelayer)
-		* 1.3.1. [ Python OP](#PythonOP)
 * 2. [ Quick Start](#QuickStart)
-	* 2.1. [ Prepare Kubernetes cluster](#PrepareKubernetescluster)
-	* 2.2. [ Setup Argo Workflows](#SetupArgoWorkflows)
-	* 2.3. [ Install dflow](#Installdflow)
-	* 2.4. [ Run an example](#Runanexample)
-* 3. [ User Guide (dflow-doc)](#UserGuide)
-	* 3.1. [ Common layer](#Commonlayer-1)
+	* 2.1. [ Setup Argo Server](#SetupArgoServer)
+	* 2.2. [ Install dflow](#Installdflow)
+	* 2.3. [ Run an example](#Runanexample)
+* 3. [ User Guide](#UserGuide)
+	* 3.1. [ Common layer](#Commonlayer)
 		* 3.1.1. [ Workflow management](#Workflowmanagement)
 		* 3.1.2. [ Upload/download artifact](#Uploaddownloadartifact)
 		* 3.1.3. [ Steps](#Steps)
 		* 3.1.4. [ DAG](#DAG)
-		* 3.1.5. [ Output parameters and artifacts of Steps](#OutputparametersandartifactsofSteps)
-		* 3.1.6. [ Conditional step, parameters and artifacts](#Conditionalstepparametersandartifacts)
-		* 3.1.7. [ Produce parallel steps using loop](#Produceparallelstepsusingloop)
-		* 3.1.8. [ Timeout](#Timeout)
-		* 3.1.9. [ Continue on failed](#Continueonfailed)
-		* 3.1.10. [ Continue on success number/ratio of parallel steps](#Continueonsuccessnumberratioofparallelsteps)
-		* 3.1.11. [ Optional input artifacts](#Optionalinputartifacts)
-		* 3.1.12. [ Default value for output parameters](#Defaultvalueforoutputparameters)
-		* 3.1.13. [ Key of a step](#Keyofastep)
-		* 3.1.14. [ Resubmit a workflow](#Resubmitaworkflow)
-		* 3.1.15. [ Executor](#Executor)
-		* 3.1.16. [ Submit Slurm job via slurm executor](#SubmitSlurmjobviaslurmexecutor)
-		* 3.1.17. [ Submit HPC job via dispatcher plugin](#SubmitHPCjobviadispatcherplugin)
-		* 3.1.18. [ Submit Slurm job via virtual node](#SubmitSlurmjobviavirtualnode)
-		* 3.1.19. [ Use resources in Kubernetes](#UseresourcesinKubernetes)
-		* 3.1.20. [ Important note: variable names](#Importantnotevariablenames)
-        * 3.1.21. [ Debug mode: dflow independent of Kubernetes](#DebugmodeDflowindependentofKubernetes)
-	* 3.2. [ Interface layer](#Interfacelayer-1)
+		* 3.1.5. [ Conditional step, parameters and artifacts](#Conditionalstepparametersandartifacts)
+		* 3.1.6. [ Produce parallel steps using loop](#Produceparallelstepsusingloop)
+		* 3.1.7. [ Timeout](#Timeout)
+		* 3.1.8. [ Continue on failed](#Continueonfailed)
+		* 3.1.9. [ Continue on success number/ratio of parallel steps](#Continueonsuccessnumberratioofparallelsteps)
+		* 3.1.10. [ Optional input artifacts](#Optionalinputartifacts)
+		* 3.1.11. [ Default value for output parameters](#Defaultvalueforoutputparameters)
+		* 3.1.12. [ Key of a step](#Keyofastep)
+		* 3.1.13. [ Resubmit a workflow](#Resubmitaworkflow)
+		* 3.1.14. [ Executor](#Executor)
+		* 3.1.15. [ Submit HPC/Bohrium job via dispatcher plugin](#SubmitHPCBohriumjobviadispatcherplugin)
+		* 3.1.16. [ Submit Slurm job via virtual node](#SubmitSlurmjobviavirtualnode)
+		* 3.1.17. [ Use resources in Kubernetes](#UseresourcesinKubernetes)
+		* 3.1.18. [ Important note: variable names](#Importantnotevariablenames)
+		* 3.1.19. [ Debug mode: dflow independent of Kubernetes](#DebugmodedflowindependentofKubernetes)
+		* 3.1.20. [Artifact storage plugins](#Artifactstorageplugins)
+	* 3.2. [ Interface layer](#Interfacelayer)
 		* 3.2.1. [ Slices](#Slices)
 		* 3.2.2. [ Retry and error handling](#Retryanderrorhandling)
 		* 3.2.3. [ Progress](#Progress)
 		* 3.2.4. [ Upload python packages for development](#Uploadpythonpackagesfordevelopment)
 
 <!-- vscode-markdown-toc-config
 	numbering=true
 	autoSave=true
 	/vscode-markdown-toc-config -->
 <!-- /vscode-markdown-toc -->
 
 ##  1. <a name='Overview'></a> Overview
 ###  1.1. <a name='Architecture'></a> Architecture
-The dflow consists of a **common layer** and an **interface layer**.  Interface layer takes various OP templates from users, usually in the form of python classes, and transforms them into base OP templates that common layer can handle.
+The dflow consists of a **common layer** and an **interface layer**.  Interface layer takes various OP templates from users, usually in the form of python classes or functions, and transforms them into base OP templates that common layer can handle.
 
 <p align="center">
 <img src="./docs/imgs/dflow_architecture.png" alt="dflow_architecture" width="400"/>
 </p>
 <!-- <style>
 img {
   display: block;
   margin-left: auto;
   margin-right: auto;
 }
 </style> -->
 
-###  1.2. <a name='Commonlayer'></a> Common layer
-Common layer is an extension over argo client which provides functionalities such as file processing, computing resources management, workflow submission and management, etc.
+###  1.2. <a name='Basics'></a> Basics
+
 ####  1.2.1. <a name='Parametersandartifacts'></a> Parameters and artifacts
-Parameters and artifacts are data stored by the workflow and passed within the workflow. Parameters are saved as strings which can be displayed in the UI, while artifacts are saved as files.
+Parameters and artifacts are data stored by the workflow and passed within the workflow. Parameters are saved as text which can be displayed in the UI, while artifacts are saved as files. Parameters are passed to an OP with their values, while artifacts are passed as paths.
 
 ####  1.2.2. <a name='OPtemplate'></a> OP template
-OP template (shown as base OP in the figure above) is the fundamental building block of a workflow. It defines an operation to be executed given the input and output. Both the input and output can be parameters and/or artifacts. The most common OP template is the container OP template. Necessary arguments to be defined for the operation are the container image and scripts to be executed. Currently, two types of container OP templates are supported: `ShellOPTemplate`, `PythonScriptOPTemplate`. Shell OP template (`ShellOPTemplate`) defines an operation by a shell script and Python script OP template (`PythonScriptOPTemplate`) defines an operation by a Python script.
-
-To use the `ShellOPTemplate`:
-
-```python
-from dflow import ShellOPTemplate
-
-simple_example_templ = ShellOPTemplate(
-    name="Hello",
-    image="alpine:latest",
-    script="cp /tmp/foo.txt /tmp/bar.txt && echo {{inputs.parameters.msg}} > /tmp/msg.txt",
-)
-```
-The above example defines a `ShellOPTemplate` with `name = "Hello"` and container image `alpine:latest`. The operation is to copy `/tmp/foo.txt` (input artifacts) to `/tmp/bar.txt` (output artifacts) and printout the properties of the parameters with name `msg` (input parameters) and redirect it to `/tmp/msg.txt` (value in the file is the properties of the output parameters). 
-<!-- 
-Parameters and artifacts can be defined as the following:
-- Input/output parameters: a dictionary that maps the parameter name to its properties.
-- Input/output artifacts: a dictionary that maps the artifact name to its properties. -->
-
-To define the parameters and artifacts of this OPTemplate: 
-
-```python
-from dflow import InputParameter, InputArtifact, OutputParameter, OutputArtifact
-
-# define input
-simple_example_templ.inputs.parameters = {"msg": InputParameter()}
-simple_example_templ.inputs.artifacts = {"inp_art": InputArtifact(path="/tmp/foo.txt")}
-# define output
-simple_example_templ.outputs.parameters = {
-    "msg": OutputParameter(value_from_path="/tmp/msg.txt")
-}
-simple_example_templ.outputs.artifacts = {
-    "out_art": OutputArtifact(path="/tmp/bar.txt")
-}
-```
-
-In the above example, there are three things to clarify. 
-1. The value of the input parameter is optional for the OP template, if provided, it will be regarded as the default value which can be overridden at run time. 
-2. For the output parameter, the source where its value comes from should be specified. For the container OP template, the value may come from a certain file generated in the container (`value_from_path`). 
-3. The paths to the input and output artifact in the container are required to be specified.
-
-On the same level, one can also define a `PythonScriptOPTemplate` to achieve the same operation. 
-
-####  1.2.3. <a name='Step'></a> Step
-`Step` is the central block for building a workflow. A `step` is created by instantiating an OP template. When a `step` is initialized, values of all input parameters and sources of all input artifacts declared in the OP template must be specified.
-<!-- `Steps` is a sequential array of concurrent `Step`'s. A simple example goes like `[[s00, s01],  [s10, s11, s12]]`, where inner array represent concurrent tasks while outer array is sequential. (this part can be put in the User Guide-->
-```python
-from dflow import Step
-
-simple_example_step = Step(
-    name="step0",
-    template=simple_example_templ,
-    parameters={"msg": "HelloWorld!"},
-    artifacts={"inp_art": foo},
-)
-``` 
-This step will instantiate the OP template created in [1.2.2](#122-a-nameoptemplatea-op-template). Note that foo is an artifact either uploaded from local or output of another step.
-
-
-####  1.2.4. <a name='Workflow'></a> Workflow
-`Workflow` is the connecting block for building a workflow. A `workflow` is created by adding `step`s together.
-```python
-from dflow import Workflow
-
-wf = Workflow(name="hello-world")
-wf.add(simple_example_step)
-```
-Submit a workflow by
-```python
-wf.submit()
-```
-One can also add a list of `step`s to a workflow to make them run in parallel
-```python
-wf.add([hello2, hello3])
-```
-An example using all the elements discussed in [1.2](#12-a-namecommonlayera-common-layer) is shown here:
-- [ShellOP example](examples/test_steps.py)
-
-###  1.3. <a name='Interfacelayer'></a> Interface layer
-Interface layer handles more Python-native OPs defined in the form of class.
-####  1.3.1. <a name='PythonOP'></a> Python OP
-`PythonOPTemplate` is another kind of OP template. It inherits from `PythonScriptOPTemplate` but allows users to define operation (OP) in the form of a Python class. As Python is a weak typed language, we impose strict type checking to `PythonOP` to alleviate ambiguity and unexpected behaviors.
+OP template (abbr. OP) is a fundamental building block of a workflow. It defines a particular operation to be executed given the input and the expected output. Both the input and output can be parameters and/or artifacts. The most common OP template is the container OP template. Two types of container OP templates are supported: `ShellOPTemplate`, `PythonScriptOPTemplate`. `ShellOPTemplate` defines an operation by shell script and a container image where the script runs. `PythonScriptOPTemplate` defines an operation by Python script and a container image.
 
-The structures of the inputs and outputs of a `PythonOP` are defined in the static methods `get_input_sign` and `get_output_sign`. Each of them returns a `OPIOSign` object, which is a dictionary mapping from the name of a parameter/artifact to its sign. 
-<!-- For a parameter, its sign is its variable type, such as `str`, `float`, `list`, or any user-defined Python class. Since argo only accept string as parameter value, dflow encodes all parameters to json (except string type parameters) before passing them to argo, and decodes argo parameters from json (except string type parameters). For an artifact, its sign must be an instance of `Artifact`. `Artifact` receives the type of the path variable as the constructor argument, only `str`, `pathlib.Path`, `typing.Set[str]`, `typing.Set[pathlib.Path]`, `typing.List[str]`, `typing.List[pathlib.Path]` are supported. If a `OP` returns a list of path as an artifact, dflow not only collects files or directories in the returned list of path, and package them in an artifact, but also records their relative path in the artifact. Thus dflow can unpack the artifact to a list of path again before passing to the next `OP`. When no file or directory exists, dflow regards it as `None`. -->
+As a more Python-native category of OP templates, `PythonOPTemplate` defines OPs in the form of Python classes or Python functions (called class OP or function OP correspondingly). As Python is a weak typed
+language, we impose strict type checking to Python OPs to alleviate ambiguity and unexpected behaviors.
 
-The execution of the `PythonOP` is defined in the `execute` method. The `execute` method receives a `OPIO` object as input and outputs a `OPIO` object. `OPIO` is a dictionary mapping from the name of a parameter/artifact to its value/path. The type of the parameter value or the artifact path should be in accord with that declared in the sign. Type checking is implemented before and after the `execute` method.
+For an class OP, the structures of the inputs and outputs of an OP are declared in the static methods `get_input_sign` and `get_output_sign`. Each of them returns a dictionary mapping from the name of a parameter/artifact to its type. The execution of the OP is defined in the `execute` method. The types of the parameter values passed in and out should be in accord with those declared in the sign. Type checking is implemented before and after the `execute` method. For an input/output artifact, its sign should be like `Artifact(type)` where `type` can be `Path`, `List[Path]`, `Dict[str, Path]` or `dflow.python.NestedDict[Path]`. For input artifact, the `execute` method will receive a path, a list of paths or a dictionary of paths according to its sign . OP developer can directly process the file or directory at the path. For output artifact, the `execute` method should also return a path, a list of paths or a dictionary of paths according to its sign.
 
 ```python
 from dflow.python import OP, OPIO, OPIOSign, Artifact
 from pathlib import Path
 import shutil
 
 
@@ -194,335 +111,380 @@
         pass
 
     @classmethod
     def get_input_sign(cls):
         return OPIOSign(
             {
                 "msg": str,
-                "inp_art": Artifact(Path),
+                "foo": Artifact(Path),
             }
         )
 
     @classmethod
     def get_output_sign(cls):
         return OPIOSign(
             {
                 "msg": str,
-                "out_art": Artifact(Path),
+                "bar": Artifact(Path),
             }
         )
 
     @OP.exec_sign_check
     def execute(
         self,
         op_in: OPIO,
     ) -> OPIO:
-        shutil.copy(op_in["inp_art"], "bar.txt")
+        shutil.copy(op_in["foo"], "bar.txt")
         out_msg = op_in["msg"]
         op_out = OPIO(
             {
                 "msg": out_msg,
-                "out_art": Path("bar.txt"),
+                "bar": Path("bar.txt"),
             }
         )
         return op_out
 ```
-The above example defines an OP `SimpleExample`. The operation is to copy `foo.txt` to `bar.txt` and write the properties of the parameters with name msg to `msg.txt`. 
 
-One may also define OP using decorator `@OP.function` and Python Annotation as:
+The above example defines an OP `SimpleExample`. The operation is to copy the input artifact `foo` to output artifact `bar` and to copy the input parameter `msg` to output parameter `msg`.
+
+For an function OP, the structure of the inputs and outputs are declared in the type annotations more compactly and execution is defined in the function body. Type checking is implemented before and after the function as well. We recommend `python>=3.9` to use this syntax sugar. See more about Python Annotation at [Python official howtos](https://docs.python.org/3/howto/annotations.html).
 
 ```python
 from dflow.python import OP, Artifact
 from pathlib import Path
 import shutil
 
 @OP.function
 def SimpleExample(
 		msg: str,
-		inp_art: Artifact(Path),
-)->{"msg": str, "out_art": Artifact(Path),}:
-    shutil.copy(inp_art, "bar.txt")
+		foo: Artifact(Path),
+) -> {"msg": str, "bar": Artifact(Path)}:
+    shutil.copy(foo, "bar.txt")
     out_msg = msg
-    return {"msg": out_msg, "out_art": Path("bar.txt"),}
+    return {"msg": out_msg, "bar": Path("bar.txt")}
 ```
 
-We recommend `python>=3.9` to use this syntax sugar.
-See more about Python Annotation at [Python official howtos](https://docs.python.org/3/howto/annotations.html).
+To define an OP template from the above class or function, we need to specify the container image and other optional arguments to `PythonOPTemplate`. `pydflow` need not to be installed in this image because local `pydflow` package will be uploaded into the container by default
 
-To use the above class as a PythonOPTemplate, we need to pass the above class to `PythonOPTemplate` and specify the container image. Note that `pydflow` must be installed in this image
 ```python
 from dflow.python import PythonOPTemplate
 
 simple_example_templ = PythonOPTemplate(SimpleExample, image="python:3.8")
 ```
 
-An example using all the elements discussed in [1.3](#12-a-namecommonlayera-common-layer)  is shown here:
-- [PythonOP example](examples/test_python.py)
+An example is here
+- [Python OP example](examples/test_python.py)
 
-##  2. <a name='QuickStart'></a> Quick Start
-###  2.1. <a name='PrepareKubernetescluster'></a> Prepare Kubernetes cluster
-Firstly, you will need a Kubernetes cluster. To setup a Kubernetes cluster on your laptop, you can download the [Minikube](https://minikube.sigs.k8s.io) on your PC and make sure you have [Docker](https://www.docker.com/) up and running on you PC.
+####  1.2.3. <a name='Step'></a> Step
+`Step` is the central block for formulating rules of data flows. A step is the result of instantiating an OP template, where values of all input parameters and sources of all input artifacts declared in the OP template must be specified here. The input parameters/artifacts of a step may be either static at the time of submission, or dynamically from outputs of another step.
 
-After downloading, you can initiate the Kubernetes cluster using: 
-```
-minikube start 
-```
-###  2.2. <a name='SetupArgoWorkflows'></a> Setup [Argo Workflows](https://argoproj.github.io/argo-workflows/quick-start/)
-To get started quickly, you can use the quick start manifest. It will install Argo Workflow as well as some commonly used components:
-```
-kubectl create ns argo
-kubectl apply -n argo -f https://raw.githubusercontent.com/deepmodeling/dflow/master/manifests/quick-start-postgres.yaml
-```
-If you are running Argo Workflows locally (e.g. using Minikube or Docker for Desktop), open a port-forward so you can access the namespace:
-```
-kubectl -n argo port-forward deployment/argo-server 2746:2746 --address 0.0.0.0
-```
-This will serve the user interface on https://localhost:2746
+```python
+from dflow import Step
 
-For access to the minio object storage, open a port-forward for minio
+simple_example_step = Step(
+    name="step0",
+    template=simple_example_templ,
+    parameters={"msg": "HelloWorld!"},
+    artifacts={"inp_art": foo},
+)
+``` 
+
+Note that `foo` here is an artifact either uploaded from local or output of another step.
+
+
+####  1.2.4. <a name='Workflow'></a> Workflow
+`Workflow` connects blocks together to build a workflow. A simple serial workflow is created by adding steps in sequence. Adding a list of steps to a workflow means these steps running in parallel.
+
+```python
+from dflow import Workflow
+
+wf = Workflow(name="hello-world")
+wf.add(simple_example_step)
 ```
-kubectl -n argo port-forward deployment/minio 9000:9000 --address 0.0.0.0
+
+Submit a workflow by
+
+```python
+wf.submit()
 ```
 
-###  2.3. <a name='Installdflow'></a> Install dflow
+An example is here
+- [Workflow example](examples/test_steps.py)
+
+
+##  2. <a name='QuickStart'></a> Quick Start
+
+###  2.1. <a name='SetupArgoServer'></a> Setup Argo Server
+
+If you have an Argo server already, you can skip this step. Otherwise you can follow the [installation guide](tutorials/readme.md).
+
+###  2.2. <a name='Installdflow'></a> Install dflow
 Make sure your Python version is not less than 3.6 and install dflow
+
 ```
 pip install pydflow
 ```
 
-###  2.4. <a name='Runanexample'></a> Run an example
-Submit a simple workflow
+###  2.3. <a name='Runanexample'></a> Run an example
+There are several [notebook tutorials](tutorials/readme.md) that can help you start to use dflow. Besides, you can submit a simple workflow from the terminal
+
 ```
-python examples/test_steps.py
+python examples/test_python.py
 ```
-Then you can check the submitted workflow through argo's UI.
+
+Then you can check the submitted workflow through [argo's UI](https://127.0.0.1:2746).
 
 ##  3. <a name='UserGuide'></a> User Guide ([dflow-doc](https://deepmodeling.com/dflow/dflow.html))
-###  3.1. <a name='Commonlayer-1'></a> Common layer
+###  3.1. <a name='Commonlayer'></a> Common layer
 
 ####  3.1.1. <a name='Workflowmanagement'></a> Workflow management
 After submitting a workflow by `wf.submit()`, or getting a history workflow by `wf = Workflow(id="xxx")`, one can track its real-time status with APIs
 
 - `wf.id`: workflow ID in argo
 - `wf.query_status()`: query workflow status, return `"Pending"`, `"Running"`, `"Succeeded"`, etc.
 - `wf.query_step(name=None)`: query step by name (support for regex), return a list of argo step objects
     - `step.phase`: phase of a step, `"Pending"`, `"Running"`, `Succeeded`, etc.
     - `step.outputs.parameters`: a dictionary of output parameters
     - `step.outputs.artifacts`: a dictionary of output artifacts
 
 ####  3.1.2. <a name='Uploaddownloadartifact'></a> Upload/download artifact
-Dflow offers tools for uploading files to Minio and downloading files from Minio (default object storage in the quick start). User can upload a list of files or directories and get an artifact object, which can be used as argument of a step
+Dflow offers tools for uploading files to the artifact repository and downloading files from it (default artifact repository is Minio set up in the quick start). User can upload a file/directory, a list of files/directories or a dictionary of files/directories and get an artifact object, which can be used as argument of a step
+
 ```python
 artifact = upload_artifact([path1, path2])
 step = Step(
     ...
     artifacts={"foo": artifact}
 )
 ```
+
 User can also download the output artifact of a step queried from a workflow (to current directory for default)
+
 ```python
 step = wf.query_step(name="hello")
 download_artifact(step.outputs.artifacts["bar"])
 ```
-Modify `dflow.s3_config` to configure S3 globally.
+
+Modify `dflow.s3_config` to configure artifact repository settings globally.
 
 Note: dflow retains the relative path of the uploaded file/directory with respect to the current directory during uploading. If file/directory outside current directory is uploaded, its absolute path is used as the relative path in the artifact. If you want a different directory structure in the artifact with the local one, you can make soft links and then upload.
 
 ####  3.1.3. <a name='Steps'></a> Steps
-`Steps` is another kind of OP template which is defined by its constituent `step`s instead of a container. It can be seen as a sub-workflow or a super OP template consisting of some smaller OPs. `Steps` is a sequential array of concurrent `Step`. A simple example goes like `[[s00,s01],[s10,s11,s12]]`, where inner array represent concurrent tasks while outer array is sequential. Add a `step` to a `steps` just like for a `workflow`
+`Steps` is another kind of OP template which is defined by its constituent steps instead of a container. It can be seen as a sub-workflow or a super OP template consisting of some smaller OPs. A `steps` includes an array of arrays of `step`s, e.g. `[[s00,s01],[s10,s11,s12]]`, where inner array represent concurrent steps while outer array is sequential. One can declare input/output parameters/artifacts for a steps by
+
+```python
+steps.inputs.parameters["msg"] = InputParameter()
+steps.inputs.artifacts["foo"] = InputArtifact()
+steps.outputs.parameters["msg"] = OutputParameter()
+steps.outputs.parameters["bar"] = OutputArtifact()
+```
+
+
+Add a `step` to a `steps` just like for a `workflow`
+
 ```python
 steps.add(step)
 ```
-`Steps` can be used as the template to define a bigger `step`. Thus one can construct complex workflows of nested structure. One is also allowed to recursively use a `Steps` as the template of a building bloack inside it self to achieve dynamic loop.
+
+`steps` can be used as the template to instantiate a bigger `step` just like script OP templates. Thus one can construct complex workflows of nested structure. One is also allowed to recursively use a `steps` as the template of a building bloack inside it self to achieve dynamic loop.
+
+The output parameter of a `steps` can be set to come from a step of it by
+
+```python
+steps.outputs.parameters["msg"].value_from_parameter = step.outputs.parameters["msg"]
+```
+
+Here, `step` must be contained in `steps`. For assigning output artifact for a `steps`, use
+
+```python
+steps.outputs.artifacts["foo"]._from = step.outputs.parameters["foo"]
+```
 
 - [Recursive example](examples/test_recurse.py)
 
 ####  3.1.4. <a name='DAG'></a> DAG
-`DAG` is another kind of OP template which is defined by its constituent `task`s and their dependencies. The usage of `DAG` is similar to that of `steps`. To add a `task` to a `DAG`, use
+`DAG` is another kind of OP template which is defined by its constituent tasks and their dependencies. The usage of `DAG` is similar to that of `Steps`. To add a `task` to a `dag`, use
+
 ```python
 dag.add(task)
 ```
-The usage of `task` is also similar to that of `step`. Dflow will automatically detect dependencies among `task`s of a `DAG` (from input/output relations). Additional dependencies can be declared by
+
+The usage of `task` is also similar to that of `step`. Dflow will automatically detect dependencies among tasks of a `dag` (from input/output relations). Additional dependencies can be declared by
+
 ```python
 task_3 = Task(..., dependencies=[task_1, task_2])
 ```
 
 - [DAG example](examples/test_dag.py)
 
-####  3.1.5. <a name='OutputparametersandartifactsofSteps'></a> Output parameters and artifacts of Steps
-The output parameter of a `Steps` can be set to come from a step of it by `steps.outputs.parameters["msg"].value_from_parameter = step.outputs.parameters["msg"]`. Here, `step` must be contained in `steps`. For assigning output artifact for a `Steps`, use `steps.outputs.artifacts["foo"]._from = step.outputs.parameters["foo"]`.
+####  3.1.5. <a name='Conditionalstepparametersandartifacts'></a> Conditional step, parameters and artifacts
+Set a step to be conditional by `Step(..., when=expr)` where `expr` is an boolean expression in string format. Such as `"%s < %s" % (par1, par2)`. The step will be performed if the expression is evalutated to be true, otherwise skipped. The `when` argument is often used as the breaking condition of recursive steps. The output parameter of a `steps` (similar to `dag`) can be assigned as conditional by
 
-####  3.1.6. <a name='Conditionalstepparametersandartifacts'></a> Conditional step, parameters and artifacts
-Set a step to be conditional by `Step(..., when=expr)` where `expr` is an boolean expression in string format. Such as `"%s < %s" % (par1, par2)`. The `when` argument is often used as the breaking condition of recursive steps. The output parameter of a `Steps` can be assigned as optional by
 ```python
 steps.outputs.parameters["msg"].value_from_expression = if_expression(
     _if=par1 < par2,
     _then=par3,
     _else=par4
 )
 ```
-Similarly, the output artifact of a `Steps` can be assigned as optional by
+
+Similarly, the output artifact of a `steps` can be assigned as conditional by
+
 ```python
 steps.outputs.artifacts["foo"].from_expression = if_expression(
     _if=par1 < par2,
     _then=art1,
     _else=art2
 )
 ```
 
 - [Conditional outputs example](examples/test_conditional_outputs.py)
 
-####  3.1.7. <a name='Produceparallelstepsusingloop'></a> Produce parallel steps using loop
-`with_param` and `with_sequence` are 2 arguments of `Step` for automatically generating a list of parallel steps. These steps share a common OP template, and only differ in the input parameters.
+####  3.1.6. <a name='Produceparallelstepsusingloop'></a> Produce parallel steps using loop
+In scientific computing, it is often required to produce a list of parallel steps which share a common OP template, and only differ in the input parameters. `with_param` and `with_sequence` are 2 arguments of `Step` for automatically generating a list of parallel steps. These steps share a common OP template, and only differ in the input parameters.
 
 A step using `with_param` option generates parallel steps on a list (either a constant list or referring to another parameter, e.g. an output parameter of another step or an input parameter of the `steps` or `DAG` context), the parallelism equals to the length of the list. Each parallel step picks an item from the list by `"{{item}}"`, such as
+
 ```python
 step = Step(
     ...
     parameters={"msg": "{{item}}"},
     with_param=steps.inputs.parameters["msg_list"]
 )
 ```
+
 A step using `with_sequence` option generates parallel steps on a numeric sequence. `with_sequence` is usually used in coordination with `argo_sequence` which returns an Argo's sequence. For `argo_sequence`, the number at which to start the sequence is specified by `start` (default: 0). One can either specify the number of elements in the sequence by `count` or the number at which to end the sequence by `end`. The printf format string can be specified by `format` to format the value in the sequence. Each argument can be passed with a parameter, `argo_len` which returns the length of a list may be useful. Each parallel step picks an element from the sequence by `"{{item}}"`, such as
+
 ```python
 step = Step(
     ...
     parameters={"i": "{{item}}"},
     with_sequence=argo_sequence(argo_len(steps.inputs.parameters["msg_list"]))
 )
 ```
 
-####  3.1.8. <a name='Timeout'></a> Timeout
+####  3.1.7. <a name='Timeout'></a> Timeout
 Set the timeout of a step by `Step(..., timeout=t)`. The unit is second.
 
 - [Timeout example](examples/test_error_handling.py)
 
-####  3.1.9. <a name='Continueonfailed'></a> Continue on failed
+####  3.1.8. <a name='Continueonfailed'></a> Continue on failed
 Set the workflow to continue when a step fails by `Step(..., continue_on_failed=True)`.
 
 - [Continue on failed example](examples/test_error_handling.py)
 
-####  3.1.10. <a name='Continueonsuccessnumberratioofparallelsteps'></a> Continue on success number/ratio of parallel steps
-Set the workflow to continue when certain number/ratio of parallel steps succeed by `Step(..., continue_on_num_success=n)` or `Step(..., continue_on_success_ratio=r)`.
+####  3.1.9. <a name='Continueonsuccessnumberratioofparallelsteps'></a> Continue on success number/ratio of parallel steps
+For a group of parallel steps generated by `with_param` or `with_sequence`, set the workflow to continue when certain number/ratio of parallel steps succeed by `Step(..., continue_on_num_success=n)` or `Step(..., continue_on_success_ratio=r)`.
 
 - [Continue on success ratio example](examples/test_success_ratio.py)
 
-####  3.1.11. <a name='Optionalinputartifacts'></a> Optional input artifacts
+####  3.1.10. <a name='Optionalinputartifacts'></a> Optional input artifacts
 Set an input artifact to be optional by `op_template.inputs.artifacts["foo"].optional = True`.
 
-####  3.1.12. <a name='Defaultvalueforoutputparameters'></a> Default value for output parameters
+####  3.1.11. <a name='Defaultvalueforoutputparameters'></a> Default value for output parameters
 Set default value for an output parameter by `op_template.outputs.parameters["msg"].default = default_value`. The default value will be used when the expression in `value_from_expression` fails or the step is skipped.
 
-####  3.1.13. <a name='Keyofastep'></a> Key of a step
-You can set a key for a step by `Step(..., key="some-key")` for the convenience of locating the step. The key can be regarded as an input parameter which may contain reference of other parameters. For instance, the key of a step can change with iterations of a dynamic loop. Once key is assigned to a step, the step can be query by `wf.query_step(key="some-key")`. If the key is unique within the workflow, the `query_step` method returns a list consist of only one element.
+####  3.1.12. <a name='Keyofastep'></a> Key of a step
+One can assign a key for a step by `Step(..., key="some-key")` for the convenience of locating the step. The key can be regarded as an input parameter which may contain reference of other parameters. For instance, the key of a step can change with iterations of a dynamic loop. Once key is assigned to a step, the step can be query by `wf.query_step(key="some-key")`. If the key is unique within the workflow, the `query_step` method returns a list consist of only one element.
 
 - [Key of step example](examples/test_reuse.py)
 
-####  3.1.14. <a name='Resubmitaworkflow'></a> Resubmit a workflow
+####  3.1.13. <a name='Resubmitaworkflow'></a> Resubmit a workflow
 Workflows often have some steps that are expensive to compute. The outputs of previously run steps can be reused for submitting a new workflow. E.g. a failed workflow can be restarted from a certain point after some modification of the workflow template or even outputs of completed steps. For example, submit a workflow with reused steps by `wf.submit(reuse_step=[step0, step1])`. Here, `step0` and `step1` are previously run steps returned by `query_step` method. Before the new workflow runs a step, it will detect if there exists a reused step whose key matches that of the step about to run. If hit, the workflow will skip the step and set its outputs as those of the reused step. To modify outputs of a step before reusing, use `step0.modify_output_parameter(par_name, value)` for parameters and `step0.modify_output_artifact(art_name, artifact)` for artifacts.
 
 - [Reuse step example](examples/test_reuse.py)
 
-####  3.1.15. <a name='Executor'></a> Executor
-By default, for a "script step" (a step whose template is a script OP template), the Shell script or Python script runs in the container directly. Alternatively, one can modify the executor to run the script. Dflow offers an extension point for "script step" `Step(..., executor=my_executor)`. Here, `my_executor` should be an instance of class derived from `Executor`. A `Executor`-derived class should implement a method `render` which converts original template to a new template.
+####  3.1.14. <a name='Executor'></a> Executor
+For a "script step" (a step whose template is a script OP template), by default the Shell script or Python script runs in the container directly. Alternatively, one can modify the executor to run the script. Dflow offers an extension point for "script step" `Step(..., executor=my_executor)`. Here, `my_executor` should be an instance of class derived from the abstract class `Executor`. An implementation class of `Executor` should implement a method `render` which converts original template to a new template.
+
 ```python
-class Executor(object):
+class Executor(ABC):
+    @abc.abstractmethod
     def render(self, template):
         pass
 ```
-A context is similar to an executor, but assigned to a workflow `Workflow(context=...)` and affect every step.
-
-####  3.1.16. <a name='SubmitSlurmjobviaslurmexecutor'></a> Submit Slurm job via slurm executor
 
-`SlurmRemoteExecutor` is provided as an example of executor. The executor submits a slurm job to a remote host and synchronize its status and logs to the dflow step. The central logic of the executor is implemented in the Golang project [Dflow-extender](https://github.com/dptech-corp/dflow-extender). If you want to run a step on a slurm cluster remotely, do something like
-```python
-Step(
-    ...,
-    executor=SlurmRemoteExecutor(host="1.2.3.4",
-        username="myuser",
-        header="""#!/bin/bash
-                  #SBATCH -N 1
-                  #SBATCH -n 1
-                  #SBATCH -p cpu""")
-)
-```
-There are 3 options for SSH authentication, using password, specify path of private key file locally, or upload authorized private key to each node (or equivalently add each node to the authorized host list).
+A context is similar to an executor, but assigned to a workflow `Workflow(context=...)` and affect every step.
 
-- [Slurm executor example](examples/test_slurm.py)
+####  3.1.15. <a name='SubmitHPCBohriumjobviadispatcherplugin'></a> Submit HPC/Bohrium job via dispatcher plugin
 
-####  3.1.17. <a name='SubmitHPCjobviadispatcherplugin'></a> Submit HPC job via dispatcher plugin
+[DPDispatcher](https://github.com/deepmodeling/dpdispatcher) is a python package used to generate HPC scheduler systems (Slurm/PBS/LSF) or [Bohrium](https://bohrium.dp.tech) jobs input scripts and submit these scripts and poke until they finish. Dflow provides simple interface to invoke dispatcher as executor to complete script steps. E.g.
 
-[DPDispatcher](https://github.com/deepmodeling/dpdispatcher) is a python package used to generate HPC scheduler systems (Slurm/PBS/LSF) jobs input scripts and submit these scripts to HPC systems and poke until they finish. Dflow provides simple interface to invoke dispatcher as executor to complete script steps. E.g.
 ```python
 from dflow.plugins.dispatcher import DispatcherExecutor
 Step(
     ...,
     executor=DispatcherExecutor(host="1.2.3.4",
         username="myuser",
         queue_name="V100")
 )
 ```
+
 For SSH authentication, one can either specify path of private key file locally, or upload authorized private key to each node (or equivalently add each node to the authorized host list). For configuring extra [machine, resources or task parameters for dispatcher](https://docs.deepmodeling.com/projects/dpdispatcher/en/latest/), use `DispatcherExecutor(..., machine_dict=m, resources_dict=r, task_dict=t)`.
 
 - [Dispatcher executor example](examples/test_dispatcher.py)
 
-####  3.1.18. <a name='SubmitSlurmjobviavirtualnode'></a> Submit Slurm job via virtual node
+####  3.1.16. <a name='SubmitSlurmjobviavirtualnode'></a> Submit Slurm job via virtual node
 
 Following the installation steps in the [wlm-operator](https://github.com/dptech-corp/wlm-operator) project to add Slurm partitions as virtual nodes to Kubernetes (use manifests [configurator.yaml](manifests/configurator.yaml), [operator-rbac.yaml](manifests/operator-rbac.yaml), [operator.yaml](manifests/operator.yaml) in this project which modified some RBAC configurations)
 ```
 $ kubectl get nodes
 NAME                            STATUS   ROLES                  AGE    VERSION
 minikube                        Ready    control-plane,master   49d    v1.22.3
 slurm-minikube-cpu              Ready    agent                  131m   v1.13.1-vk-N/A
 slurm-minikube-dplc-ai-v100x8   Ready    agent                  131m   v1.13.1-vk-N/A
 slurm-minikube-v100             Ready    agent                  131m   v1.13.1-vk-N/A
 ```
 Then you can assign a step to be executed on a virtual node (i.e. submit a Slurm job to the corresponding partition to complete the step)
+
 ```python
 step = Step(
     ...
     executor=SlurmJobTemplate(
         header="#!/bin/sh\n#SBATCH --nodes=1",
         node_selector={"kubernetes.io/hostname": "slurm-minikube-v100"}
     )
 )
 ```
 
-####  3.1.19. <a name='UseresourcesinKubernetes'></a> Use resources in Kubernetes
+####  3.1.17. <a name='UseresourcesinKubernetes'></a> Use resources in Kubernetes
 
 A step can also be completed by a Kubernetes resource (e.g. Job or custom resources). At the beginning, a manifest is applied to Kubernetes. Then the status of the resource is monitered until the success condition or the failure condition is satisfied.
+
 ```python
-class Resource(object):
+class Resource(ABC):
     action = None
     success_condition = None
     failure_condition = None
-    def get_manifest(self, template):
+    @abc.abstractmethod
         pass
 ```
 
 - [Wlm example](examples/test_wlm.py)
 
-####  3.1.20. <a name='Importantnotevariablenames'></a> Important note: variable names
+####  3.1.18. <a name='Importantnotevariablenames'></a> Important note: variable names
 
 Dflow has following restrictions on variable names.
 
 | Variable name | Static/Dynamic | Restrictions | Example |
 | :------------ | -------------- | ------------ | ------- |
 | Workflow/OP template name | Static | Lowercase RFC 1123 subdomain (must consist of lower case alphanumeric characters, '-' or '.', and must start and end with an alphanumeric character | my-name |
 | Step/Task name | Static | Must consist of alpha-numeric characters or '-', and must start with an alpha-numeric character | My-name1-2, 123-NAME |
 | Parameter/Artifact name | Static | Must consist of alpha-numeric characters, '_' or '-' | my_param_1, MY-PARAM-1 |
 | Key name | Dynamic | Lowercase RFC 1123 subdomain (must consist of lower case alphanumeric characters, '-' or '.', and must start and end with an alphanumeric character | my-name |
 
-#### 3.1.21. <a name='DebugmodeDflowindependentofKubernetes'></a> Debug mode: dflow independent of Kubernetes
+####  3.1.19. <a name='DebugmodedflowindependentofKubernetes'></a> Debug mode: dflow independent of Kubernetes
 
 The debug mode is enabled by setting
+
 ```python
 from dflow import config
 config["mode"] = "debug"
 ```
+
 Before running a workflow locally, make sure that the dependencies of all OPs in the workflow are well-configured in the locally environment, unless the dispatcher executor is employed to submit jobs to some remote environments. The debug mode uses the current directory as the working directory by default. Each workflow will create a new directory there, whose structure will be like
 ```
 python-lsev6
 ├── status
 └── step-penf5
     ├── inputs
     │   ├── artifacts
@@ -545,18 +507,42 @@
     └── workdir
         ├── ...
 ```
 The top level contains the status and all steps of the workflow. The directory name for each step will be its key if provided, or generated from its name otherwise. The step directory contains the input/output parameters/artifacts, the type and the phase of the step. For a step of type "Pod", its directory also includes the script, the log file and the working directory for the step.
 
 - [Debug mode examples](examples/debug)
 
-###  3.2. <a name='Interfacelayer-1'></a> Interface layer
+####  3.1.20. <a name='Artifactstorageplugins'></a>Artifact storage plugins
+
+The default storage for artifacts in dflow is a Minio deployment in the Kubernetes cluster. While other artifact storages are supported (e.g. Aliyun OSS, Azure blob storage (ABS), Google cloud storage(GCS)). Dflow provides an extension point to use customized storage in the artifact management. A storage client is a class implementing 5 abstract methods, `upload`, `download`, `list`, `copy` and `get_md5` (optional), which offer the functionality of uploading file, downloading file, listing files with a particular prefix, copying file on the server side and getting the MD5 sum of file, respectively. Use a custom storage client object by configuring s3_config["storage_client"].
+
+```python
+class StorageClient(ABC):
+    @abc.abstractmethod
+    def upload(self, key: str, path: str) -> None:
+        pass
+    @abc.abstractmethod
+    def download(self, key: str, path: str) -> None:
+        pass
+    @abc.abstractmethod
+    def list(self, prefix: str, recursive: bool = False) -> List[str]:
+        pass
+    @abc.abstractmethod
+    def copy(self, src: str, dst: str) -> None:
+        pass
+    @abc.abstractmethod
+    def get_md5(self, key: str) -> str:
+        pass
+```
+
+###  3.2. <a name='Interfacelayer'></a> Interface layer
 
 ####  3.2.1. <a name='Slices'></a> Slices
-`Slices` helps user to slice input parameters/artifacts (which must be lists) to feed parallel steps and stack their output parameters/artifacts to lists in the same pattern. For example,
+In coordination with [parallel steps](#Produceparallelstepsusingloop), `Slices` helps user to slice input parameters/artifacts (which must be lists) to feed parallel steps and stack their output parameters/artifacts to lists in the same pattern. The Python OP only need to handle one slice. For example,
+
 ```python
 step = Step(name="parallel-tasks",
     template=PythonOPTemplate(
         ...,
         slices=Slices("{{item}}",
             input_parameter=["msg"],
             input_artifact=["data"],
@@ -567,19 +553,21 @@
     },
     artifacts={
         "data": data_list
     },
     with_param=argo_range(5)
 )
 ```
+
 In this example, each item in `msg_list` is passed to a parallel step as the input parameter `msg`, each part in `data_list` is passed to a parallel step as the input artifact `data`. Finally, the output artifacts `log` of all parallel steps are collected to one artifact `step.outputs.artifacts["log"]`.
 
 - [Slices example](examples/test_slices.py)
 
 It should be noticed that this feature by default passes full input artifacts to each parallel step which may only use some slices of these artifacts. In comparison, the subpath mode of slices only passes one single slice of the input artifacts to each parallel step. To use the subpath mode of slices,
+
 ```python
 step = Step(name="parallel-tasks",
     template=PythonOPTemplate(
         ...,
         slices=Slices(sub_path=True,
             input_parameter=["msg"],
             input_artifact=["data"],
@@ -588,36 +576,39 @@
     parameters = {
         "msg": msg_list
     },
     artifacts={
         "data": data_list
     })
 ```
+
 Here, the slice pattern (`{{item}}`) of `PythonOPTemplate` and the `with_param` argument of the `Step` need not to be set, because they are fixed in this mode. Each input parameter and artifact to be sliced must be of the same length, and the parallelism equals to this length. Another noticeable point is that in order to use the subpath of the artifacts, these artifacts must be saved without compression when they are generated. E.g. declare `Artifact(..., archive=None)` in the output signs of Python OP, or specify `upload_artifact(..., archive=None)` while uploading artifacts. Besides, one can use `dflow.config["archive_mode"] = None` to set default archive mode to no compression globally.
 
 - [Subpath mode of slices example](examples/test_subpath_slices.py)
 
 ####  3.2.2. <a name='Retryanderrorhandling'></a> Retry and error handling
-Dflow catches `TransientError` and `FatalError` thrown from `OP`. User can set maximum number of retries on `TransientError` by `PythonOPTemplate(..., retry_on_transient_error=n)`. Timeout error is regarded as fatal error for default. To treat timeout error as transient error, set `PythonOPTemplate(..., timeout_as_transient_error=True)`.
+Dflow catches `TransientError` and `FatalError` thrown from `OP`. User can set maximum number of retries on `TransientError` by `PythonOPTemplate(..., retry_on_transient_error=n)`. Timeout error is regarded as fatal error for default. To treat timeout error as transient error, set `PythonOPTemplate(..., timeout_as_transient_error=True)`. When a fatal error is raised or the retries on transient error reaches maximum retries, the step is considered as failed.
 
 - [Retry example](examples/test_error_handling.py)
 
 ####  3.2.3. <a name='Progress'></a> Progress
 A `OP` can update progress in the runtime so that user can track its real-time progress
+
 ```python
 class Progress(OP):
     progress_total = 100
     ...
     def execute(op_in):
         for i in range(10):
             self.progress_current = 10 * (i + 1)
             ...
 ```
 
 - [Progress example](examples/test_progress.py)
 
 ####  3.2.4. <a name='Uploadpythonpackagesfordevelopment'></a> Upload python packages for development
 To avoid frequently making image during development, dflow offers an interface to upload local packages into container and add them to `$PYTHONPATH`, such as `PythonOPTemplate(..., python_packages=["/opt/anaconda3/lib/python3.9/site-packages/numpy"])`. One can also globally specify packages to be uploaded, which will affect all `OP`s
+
 ```python
 from dflow.python import upload_packages
 upload_packages.append("/opt/anaconda3/lib/python3.9/site-packages/numpy")
 ```
```

### Comparing `pydflow-1.6.99/src/pydflow.egg-info/SOURCES.txt` & `pydflow-1.7.0/src/pydflow.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
+VERSION
 setup.py
 src/dflow/__init__.py
 src/dflow/__main__.py
 src/dflow/argo_objects.py
 src/dflow/common.py
 src/dflow/config.py
 src/dflow/context.py
@@ -25,15 +27,17 @@
 src/dflow/client/v1alpha1_artifact.py
 src/dflow/client/v1alpha1_parameter.py
 src/dflow/client/v1alpha1_retry_strategy.py
 src/dflow/client/v1alpha1_sequence.py
 src/dflow/client/v1alpha1_value_from.py
 src/dflow/plugins/__init__.py
 src/dflow/plugins/bohrium.py
+src/dflow/plugins/datasets.py
 src/dflow/plugins/dispatcher.py
+src/dflow/plugins/launching.py
 src/dflow/plugins/lebesgue.py
 src/dflow/plugins/metadata.py
 src/dflow/plugins/oss.py
 src/dflow/plugins/ray.py
 src/dflow/python/__init__.py
 src/dflow/python/op.py
 src/dflow/python/opio.py
```

### Comparing `pydflow-1.6.99/tests/test_big_parameter.py` & `pydflow-1.7.0/tests/test_big_parameter.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,14 @@
     wf.add(big_step)
     wf.submit()
 
     while wf.query_status() in ["Pending", "Running"]:
         time.sleep(1)
 
     assert(wf.query_status() == "Succeeded")
-    step = wf.query_step(name="step1")[0]
+    step = wf.query_step(key="step1")[0]
     assert(step.phase == "Succeeded")
     assert(isinstance(step.outputs.parameters["foo"].value, Hello))
 
 
 if __name__ == "__main__":
     test_big_parameter()
```

### Comparing `pydflow-1.6.99/tests/test_conditional_outputs.py` & `pydflow-1.7.0/tests/test_conditional_outputs.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/tests/test_dag.py` & `pydflow-1.7.0/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/tests/test_group_size.py` & `pydflow-1.7.0/tests/test_group_size.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/tests/test_makevasp.py` & `pydflow-1.7.0/tests/test_makevasp.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/tests/test_python.py` & `pydflow-1.7.0/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/tests/test_recurse.py` & `pydflow-1.7.0/tests/test_recurse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/tests/test_reuse.py` & `pydflow-1.7.0/tests/test_reuse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/tests/test_slices.py` & `pydflow-1.7.0/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.6.99/tests/test_subpath_slices.py` & `pydflow-1.7.0/tests/test_subpath_slices.py`

 * *Files identical despite different names*

