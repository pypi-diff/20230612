# Comparing `tmp/vgd_counterfactuals-0.3.0.tar.gz` & `tmp/vgd_counterfactuals-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vgd_counterfactuals-0.3.0.tar", max compression
+gzip compressed data, was "vgd_counterfactuals-0.3.1.tar", max compression
```

## Comparing `vgd_counterfactuals-0.3.0.tar` & `vgd_counterfactuals-0.3.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.3.0/LICENSE
--rwxr-xr-x   0        0        0     6577 2023-06-12 09:05:41.163959 vgd_counterfactuals-0.3.0/README.rst
--rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.3.0/banner.png
--rwxr-xr-x   0        0        0     1540 2023-06-12 09:21:17.467943 vgd_counterfactuals-0.3.0/pyproject.toml
--rwxr-xr-x   0        0        0        5 2023-06-12 09:05:41.163959 vgd_counterfactuals-0.3.0/vgd_counterfactuals/VERSION
--rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.3.0/vgd_counterfactuals/__init__.py
--rw-r--r--   0        0        0    12166 2023-06-01 10:10:57.254190 vgd_counterfactuals-0.3.0/vgd_counterfactuals/base.py
--rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.3.0/vgd_counterfactuals/cli.py
--rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/00_quickstart.py
--rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/01_visualization.py
--rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/README.rst
--rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/__init__.py
--rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
--rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
--rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
--rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
--rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
--rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
--rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
--rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
--rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
--rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
--rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
--rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
--rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
--rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
--rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
--rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
--rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
--rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
--rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
--rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
--rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
--rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
--rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
--rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
--rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
--rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
--rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.3.0/vgd_counterfactuals/experiments/README.rst
--rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.3.0/vgd_counterfactuals/experiments/results/README.rst
--rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.3.0/vgd_counterfactuals/experiments/template_experiment.py
--rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.3.0/vgd_counterfactuals/experiments/template_experiment_sub.py
--rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.3.0/vgd_counterfactuals/generate/__init__.py
--rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.3.0/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2665 2023-06-12 08:05:30.105591 vgd_counterfactuals-0.3.0/vgd_counterfactuals/generate/__pycache__/colors.cpython-310.pyc
--rw-r--r--   0        0        0     9194 2023-06-01 10:01:20.429985 vgd_counterfactuals-0.3.0/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
--rw-r--r--   0        0        0     3912 2023-06-12 08:05:29.265620 vgd_counterfactuals-0.3.0/vgd_counterfactuals/generate/colors.py
--rw-r--r--   0        0        0    13613 2023-06-01 10:01:19.881981 vgd_counterfactuals-0.3.0/vgd_counterfactuals/generate/molecules.py
--rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.3.0/vgd_counterfactuals/generate/smiles_one_step_changes.py
--rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.3.0/vgd_counterfactuals/templates/article.tex.j2
--rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.3.0/vgd_counterfactuals/testing.py
--rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.3.0/vgd_counterfactuals/utils.py
--rw-r--r--   0        0        0     3931 2023-06-01 08:03:40.743915 vgd_counterfactuals-0.3.0/vgd_counterfactuals/visualization.py
--rw-r--r--   0        0        0     7661 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.3.1/LICENSE
+-rwxr-xr-x   0        0        0     6577 2023-06-12 12:40:28.348441 vgd_counterfactuals-0.3.1/README.rst
+-rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.3.1/banner.png
+-rwxr-xr-x   0        0        0     1540 2023-06-12 12:40:28.340441 vgd_counterfactuals-0.3.1/pyproject.toml
+-rwxr-xr-x   0        0        0        5 2023-06-12 12:40:28.348441 vgd_counterfactuals-0.3.1/vgd_counterfactuals/VERSION
+-rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.3.1/vgd_counterfactuals/__init__.py
+-rw-r--r--   0        0        0    12166 2023-06-01 10:10:57.254190 vgd_counterfactuals-0.3.1/vgd_counterfactuals/base.py
+-rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.3.1/vgd_counterfactuals/cli.py
+-rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/00_quickstart.py
+-rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/01_visualization.py
+-rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/README.rst
+-rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/__init__.py
+-rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
+-rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
+-rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
+-rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
+-rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
+-rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
+-rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
+-rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
+-rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
+-rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
+-rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
+-rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
+-rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
+-rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
+-rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
+-rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
+-rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
+-rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
+-rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
+-rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
+-rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
+-rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
+-rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
+-rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
+-rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
+-rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
+-rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/README.rst
+-rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/results/README.rst
+-rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/template_experiment.py
+-rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/template_experiment_sub.py
+-rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2667 2023-06-12 12:39:10.587919 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/__pycache__/colors.cpython-310.pyc
+-rw-r--r--   0        0        0     9194 2023-06-01 10:01:20.429985 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
+-rw-r--r--   0        0        0     3914 2023-06-12 12:39:09.739913 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/colors.py
+-rw-r--r--   0        0        0    13613 2023-06-01 10:01:19.881981 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/molecules.py
+-rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/smiles_one_step_changes.py
+-rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.3.1/vgd_counterfactuals/templates/article.tex.j2
+-rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.3.1/vgd_counterfactuals/testing.py
+-rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.3.1/vgd_counterfactuals/utils.py
+-rw-r--r--   0        0        0     3931 2023-06-01 08:03:40.743915 vgd_counterfactuals-0.3.1/vgd_counterfactuals/visualization.py
+-rw-r--r--   0        0        0     7661 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.3.1/PKG-INFO
```

### Comparing `vgd_counterfactuals-0.3.0/LICENSE` & `vgd_counterfactuals-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/README.rst` & `vgd_counterfactuals-0.3.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.3.0-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.3.1-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

### Comparing `vgd_counterfactuals-0.3.0/banner.png` & `vgd_counterfactuals-0.3.1/banner.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/pyproject.toml` & `vgd_counterfactuals-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vgd_counterfactuals"
-version = "0.3.0"
+version = "0.3.1"
 description = "Counterfactual explanations for GNNs based on the visual graph dataset format"
 license = "MIT license"
 authors = ["Jonas Teufel <jonseb1998@gmail.com>"]
 maintainers = ["Jonas Teufel <jonseb1998@gmail.com>"]
 readme = "README.rst"
 keywords = ["graph neural networks", "counterfactuals", "explainable AI"]
 packages = [
```

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/base.py` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/base.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/cli.py` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/cli.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/00_quickstart.py` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/00_quickstart.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/01_visualization.py` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/01_visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/code.py` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/code.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/experiments/README.rst` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/README.rst`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/experiments/template_experiment.py` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/template_experiment.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/experiments/template_experiment_sub.py` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/template_experiment_sub.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/generate/__pycache__/colors.cpython-310.pyc` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/__pycache__/colors.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 08:05:29 2023 UTC, .py size: 3912 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c9d1 8664 480f 0000  o..........dH...
+00000000: 6f0d 0d0a 0000 0000 ed11 8764 4a0f 0000  o..........dJ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 f800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c04 6d00 5a05 0100 6400 6402 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6400 6403 6c06 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6400 6404 6c06 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -114,54 +114,54 @@
 00000710: 0000 7212 0000 0072 2700 0000 da01 6a72  ..r....r'.....jr
 00000720: 2800 0000 7209 0000 0072 1300 0000 7213  (...r....r....r.
 00000730: 0000 0072 1400 0000 7210 0000 003c 0000  ...r....r....<..
 00000740: 0073 1c00 0000 0403 1001 0801 1001 0a01  .s..............
 00000750: 2009 0401 0201 0201 0601 0601 08fc 0280   ...............
 00000760: 0407 7210 0000 0063 0200 0000 0000 0000  ..r....c........
 00000770: 0000 0000 0700 0000 0900 0000 4300 0000  ............C...
-00000780: 7380 0000 0067 007d 0274 007c 0083 017d  s....g.}.t.|...}
-00000790: 037c 0064 0119 0044 005d 337d 047c 0064  .|.d...D.]3}.|.d
-000007a0: 0119 0044 005d 2c7d 057c 047c 056b 0372  ...D.],}.|.|.k.r
-000007b0: 3c7c 037c 047c 0566 0219 0073 3c74 017c  <|.|.|.f...s<t.|
+00000780: 7382 0000 0067 007d 0274 007c 0083 017d  s....g.}.t.|...}
+00000790: 037c 0064 0119 0044 005d 347d 047c 0064  .|.d...D.]4}.|.d
+000007a0: 0119 0044 005d 2d7d 057c 047c 056b 0372  ...D.]-}.|.|.k.r
+000007b0: 3d7c 037c 047c 0566 0219 0073 3d74 017c  =|.|.|.f...s=t.|
 000007c0: 0083 017d 0674 027c 067c 047c 0564 0264  ...}.t.|.|.|.d.d
-000007d0: 0364 0469 0164 058d 0501 007c 02a0 0364  .d.i.d.....|...d
-000007e0: 067c 01a0 047c 06a1 017c 047c 0566 027c  .|...|...|.|.f.|
-000007f0: 047c 0566 0264 079c 04a1 0101 0071 1071  .|.f.d.......q.q
-00000800: 0a7c 0253 0029 084e 7216 0000 0046 da0f  .|.S.).Nr....F..
-00000810: 6564 6765 5f61 7474 7269 6275 7465 7372  edge_attributesr
-00000820: 2c00 0000 2905 720d 0000 00da 0c6e 6f64  ,...).r......nod
-00000830: 655f 696e 6465 785f 31da 0c6e 6f64 655f  e_index_1..node_
-00000840: 696e 6465 785f 3272 2a00 0000 721e 0000  index_2r*...r...
-00000850: 00da 0861 6464 5f65 6467 6572 2100 0000  ...add_edger!...
-00000860: 2905 7204 0000 0072 0200 0000 7205 0000  ).r....r....r...
-00000870: 0072 2500 0000 7226 0000 0029 0772 0d00  .r%...r&...).r..
-00000880: 0000 720b 0000 0072 1200 0000 da0f 6e6f  ..r....r......no
-00000890: 6465 5f61 646a 616e 6365 6e63 7972 2700  de_adjancencyr'.
-000008a0: 0000 7231 0000 0072 2800 0000 7213 0000  ..r1...r(...r...
-000008b0: 0072 1300 0000 7214 0000 0072 1100 0000  .r....r....r....
-000008c0: 5700 0000 732e 0000 0004 0308 010c 010c  W...s...........
-000008d0: 0114 0108 0102 0102 0102 0102 0102 0104  ................
-000008e0: 0202 ff06 fb04 0a02 0108 0106 0106 0108  ................
-000008f0: fc02 8002 f304 1472 1100 0000 2919 da06  .......r....)...
-00000900: 7479 7069 6e67 da01 74da 056e 756d 7079  typing..t..numpy
-00000910: 7218 0000 00da 1c76 6973 7561 6c5f 6772  r......visual_gr
-00000920: 6170 685f 6461 7461 7365 7473 2e74 7970  aph_datasets.typ
-00000930: 696e 67da 0274 76da 1b76 6973 7561 6c5f  ing..tv..visual_
-00000940: 6772 6170 685f 6461 7461 7365 7473 2e67  graph_datasets.g
-00000950: 7261 7068 7202 0000 0072 0300 0000 7204  raphr....r....r.
-00000960: 0000 0072 0500 0000 7206 0000 00da 2776  ...r....r.....'v
-00000970: 6973 7561 6c5f 6772 6170 685f 6461 7461  isual_graph_data
-00000980: 7365 7473 2e67 656e 6572 6174 696f 6e2e  sets.generation.
-00000990: 636f 6c6f 7273 7207 0000 00da 2776 6973  colorsr.....'vis
-000009a0: 7561 6c5f 6772 6170 685f 6461 7461 7365  ual_graph_datase
-000009b0: 7473 2e70 726f 6365 7373 696e 672e 636f  ts.processing.co
-000009c0: 6c6f 7273 7208 0000 00da 0373 7472 da04  lorsr......str..
-000009d0: 4c69 7374 da04 6469 6374 7215 0000 00da  List..dictr.....
-000009e0: 0947 7261 7068 4469 6374 da03 416e 7972  .GraphDict..Anyr
-000009f0: 0f00 0000 7210 0000 0072 1100 0000 7213  ....r....r....r.
-00000a00: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-00000a10: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000a20: 7344 0000 0008 0008 020c 010c 0110 0110  sD..............
-00000a30: 010c 010c 0102 0504 0108 fe08 0102 ff02  ................
-00000a40: 0202 fe08 030a fd08 190a 0102 ff02 0202  ................
-00000a50: fe08 030a fd08 1602 0102 ff08 020a fe08  ................
-00000a60: 1b02 0102 ff08 020e fe                   .........
+000007d0: 0364 0467 0169 0164 058d 0501 007c 02a0  .d.g.i.d.....|..
+000007e0: 0364 067c 01a0 047c 06a1 017c 047c 0566  .d.|...|...|.|.f
+000007f0: 027c 047c 0566 0264 079c 04a1 0101 0071  .|.|.f.d.......q
+00000800: 1071 0a7c 0253 0029 084e 7216 0000 0046  .q.|.S.).Nr....F
+00000810: da0f 6564 6765 5f61 7474 7269 6275 7465  ..edge_attribute
+00000820: 7372 2c00 0000 2905 720d 0000 00da 0c6e  sr,...).r......n
+00000830: 6f64 655f 696e 6465 785f 31da 0c6e 6f64  ode_index_1..nod
+00000840: 655f 696e 6465 785f 3272 2a00 0000 721e  e_index_2r*...r.
+00000850: 0000 00da 0861 6464 5f65 6467 6572 2100  .....add_edger!.
+00000860: 0000 2905 7204 0000 0072 0200 0000 7205  ..).r....r....r.
+00000870: 0000 0072 2500 0000 7226 0000 0029 0772  ...r%...r&...).r
+00000880: 0d00 0000 720b 0000 0072 1200 0000 da0f  ....r....r......
+00000890: 6e6f 6465 5f61 646a 616e 6365 6e63 7972  node_adjancencyr
+000008a0: 2700 0000 7231 0000 0072 2800 0000 7213  '...r1...r(...r.
+000008b0: 0000 0072 1300 0000 7214 0000 0072 1100  ...r....r....r..
+000008c0: 0000 5700 0000 732e 0000 0004 0308 010c  ..W...s.........
+000008d0: 010c 0114 0108 0102 0102 0102 0102 0102  ................
+000008e0: 0106 0202 ff06 fb04 0a02 0108 0106 0106  ................
+000008f0: 0108 fc02 8002 f304 1472 1100 0000 2919  .........r....).
+00000900: da06 7479 7069 6e67 da01 74da 056e 756d  ..typing..t..num
+00000910: 7079 7218 0000 00da 1c76 6973 7561 6c5f  pyr......visual_
+00000920: 6772 6170 685f 6461 7461 7365 7473 2e74  graph_datasets.t
+00000930: 7970 696e 67da 0274 76da 1b76 6973 7561  yping..tv..visua
+00000940: 6c5f 6772 6170 685f 6461 7461 7365 7473  l_graph_datasets
+00000950: 2e67 7261 7068 7202 0000 0072 0300 0000  .graphr....r....
+00000960: 7204 0000 0072 0500 0000 7206 0000 00da  r....r....r.....
+00000970: 2776 6973 7561 6c5f 6772 6170 685f 6461  'visual_graph_da
+00000980: 7461 7365 7473 2e67 656e 6572 6174 696f  tasets.generatio
+00000990: 6e2e 636f 6c6f 7273 7207 0000 00da 2776  n.colorsr.....'v
+000009a0: 6973 7561 6c5f 6772 6170 685f 6461 7461  isual_graph_data
+000009b0: 7365 7473 2e70 726f 6365 7373 696e 672e  sets.processing.
+000009c0: 636f 6c6f 7273 7208 0000 00da 0373 7472  colorsr......str
+000009d0: da04 4c69 7374 da04 6469 6374 7215 0000  ..List..dictr...
+000009e0: 00da 0947 7261 7068 4469 6374 da03 416e  ...GraphDict..An
+000009f0: 7972 0f00 0000 7210 0000 0072 1100 0000  yr....r....r....
+00000a00: 7213 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
+00000a10: 1400 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000a20: 0000 7344 0000 0008 0008 020c 010c 0110  ..sD............
+00000a30: 0110 010c 010c 0102 0504 0108 fe08 0102  ................
+00000a40: ff02 0202 fe08 030a fd08 190a 0102 ff02  ................
+00000a50: 0202 fe08 030a fd08 1602 0102 ff08 020a  ................
+00000a60: fe08 1b02 0102 ff08 020e fe              ...........
```

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/generate/colors.py` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 new_graph = copy_graph_dict(graph)
                 graph_add_edge(
                     graph=new_graph, 
                     node_index_1=i, 
                     node_index_2=j, 
                     directed=False,
                     attributes={
-                        'edge_attributes': 1
+                        'edge_attributes': [1]
                     }
                 )
                 
                 results.append({
                     'type': 'add_edge',
                     'value': processing.unprocess(new_graph),
                     'org': (i, j),
```

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/generate/molecules.py` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/molecules.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/generate/smiles_one_step_changes.py` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/smiles_one_step_changes.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/templates/article.tex.j2` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/templates/article.tex.j2`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/utils.py` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/utils.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/vgd_counterfactuals/visualization.py` & `vgd_counterfactuals-0.3.1/vgd_counterfactuals/visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.0/PKG-INFO` & `vgd_counterfactuals-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgd-counterfactuals
-Version: 0.3.0
+Version: 0.3.1
 Summary: Counterfactual explanations for GNNs based on the visual graph dataset format
 License: MIT
 Keywords: graph neural networks,counterfactuals,explainable AI
 Author: Jonas Teufel
 Author-email: jonseb1998@gmail.com
 Maintainer: Jonas Teufel
 Maintainer-email: jonseb1998@gmail.com
@@ -33,15 +33,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.3.0-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.3.1-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

