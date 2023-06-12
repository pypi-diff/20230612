# Comparing `tmp/vgd_counterfactuals-0.3.1.tar.gz` & `tmp/vgd_counterfactuals-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vgd_counterfactuals-0.3.1.tar", max compression
+gzip compressed data, was "vgd_counterfactuals-0.3.2.tar", max compression
```

## Comparing `vgd_counterfactuals-0.3.1.tar` & `vgd_counterfactuals-0.3.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.3.1/LICENSE
--rwxr-xr-x   0        0        0     6577 2023-06-12 12:40:28.348441 vgd_counterfactuals-0.3.1/README.rst
--rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.3.1/banner.png
--rwxr-xr-x   0        0        0     1540 2023-06-12 12:40:28.340441 vgd_counterfactuals-0.3.1/pyproject.toml
--rwxr-xr-x   0        0        0        5 2023-06-12 12:40:28.348441 vgd_counterfactuals-0.3.1/vgd_counterfactuals/VERSION
--rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.3.1/vgd_counterfactuals/__init__.py
--rw-r--r--   0        0        0    12166 2023-06-01 10:10:57.254190 vgd_counterfactuals-0.3.1/vgd_counterfactuals/base.py
--rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.3.1/vgd_counterfactuals/cli.py
--rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/00_quickstart.py
--rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/01_visualization.py
--rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/README.rst
--rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/__init__.py
--rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
--rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
--rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
--rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
--rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
--rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
--rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
--rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
--rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
--rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
--rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
--rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
--rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
--rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
--rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
--rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
--rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
--rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
--rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
--rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
--rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
--rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
--rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
--rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
--rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
--rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
--rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/README.rst
--rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/results/README.rst
--rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/template_experiment.py
--rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/template_experiment_sub.py
--rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/__init__.py
--rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2667 2023-06-12 12:39:10.587919 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/__pycache__/colors.cpython-310.pyc
--rw-r--r--   0        0        0     9194 2023-06-01 10:01:20.429985 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
--rw-r--r--   0        0        0     3914 2023-06-12 12:39:09.739913 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/colors.py
--rw-r--r--   0        0        0    13613 2023-06-01 10:01:19.881981 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/molecules.py
--rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/smiles_one_step_changes.py
--rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.3.1/vgd_counterfactuals/templates/article.tex.j2
--rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.3.1/vgd_counterfactuals/testing.py
--rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.3.1/vgd_counterfactuals/utils.py
--rw-r--r--   0        0        0     3931 2023-06-01 08:03:40.743915 vgd_counterfactuals-0.3.1/vgd_counterfactuals/visualization.py
--rw-r--r--   0        0        0     7661 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.3.2/LICENSE
+-rwxr-xr-x   0        0        0     6577 2023-06-12 15:18:05.343575 vgd_counterfactuals-0.3.2/README.rst
+-rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.3.2/banner.png
+-rwxr-xr-x   0        0        0     1540 2023-06-12 15:18:29.648405 vgd_counterfactuals-0.3.2/pyproject.toml
+-rwxr-xr-x   0        0        0        5 2023-06-12 15:18:05.339575 vgd_counterfactuals-0.3.2/vgd_counterfactuals/VERSION
+-rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.3.2/vgd_counterfactuals/__init__.py
+-rw-r--r--   0        0        0    12166 2023-06-01 10:10:57.254190 vgd_counterfactuals-0.3.2/vgd_counterfactuals/base.py
+-rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.3.2/vgd_counterfactuals/cli.py
+-rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/00_quickstart.py
+-rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/01_visualization.py
+-rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/README.rst
+-rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/__init__.py
+-rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
+-rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
+-rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
+-rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
+-rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
+-rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
+-rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
+-rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
+-rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
+-rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
+-rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
+-rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
+-rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
+-rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
+-rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
+-rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
+-rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
+-rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
+-rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
+-rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
+-rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
+-rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
+-rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
+-rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
+-rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
+-rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
+-rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.3.2/vgd_counterfactuals/experiments/README.rst
+-rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.3.2/vgd_counterfactuals/experiments/results/README.rst
+-rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.3.2/vgd_counterfactuals/experiments/template_experiment.py
+-rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.3.2/vgd_counterfactuals/experiments/template_experiment_sub.py
+-rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.3.2/vgd_counterfactuals/generate/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.3.2/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2667 2023-06-12 15:17:30.262386 vgd_counterfactuals-0.3.2/vgd_counterfactuals/generate/__pycache__/colors.cpython-310.pyc
+-rw-r--r--   0        0        0     9194 2023-06-01 10:01:20.429985 vgd_counterfactuals-0.3.2/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
+-rw-r--r--   0        0        0     3913 2023-06-12 15:17:29.402357 vgd_counterfactuals-0.3.2/vgd_counterfactuals/generate/colors.py
+-rw-r--r--   0        0        0    13613 2023-06-01 10:01:19.881981 vgd_counterfactuals-0.3.2/vgd_counterfactuals/generate/molecules.py
+-rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.3.2/vgd_counterfactuals/generate/smiles_one_step_changes.py
+-rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.3.2/vgd_counterfactuals/templates/article.tex.j2
+-rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.3.2/vgd_counterfactuals/testing.py
+-rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.3.2/vgd_counterfactuals/utils.py
+-rw-r--r--   0        0        0     3931 2023-06-01 08:03:40.743915 vgd_counterfactuals-0.3.2/vgd_counterfactuals/visualization.py
+-rw-r--r--   0        0        0     7661 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.3.2/PKG-INFO
```

### Comparing `vgd_counterfactuals-0.3.1/LICENSE` & `vgd_counterfactuals-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/README.rst` & `vgd_counterfactuals-0.3.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.3.1-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.3.2-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

### Comparing `vgd_counterfactuals-0.3.1/banner.png` & `vgd_counterfactuals-0.3.2/banner.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/pyproject.toml` & `vgd_counterfactuals-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vgd_counterfactuals"
-version = "0.3.1"
+version = "0.3.2"
 description = "Counterfactual explanations for GNNs based on the visual graph dataset format"
 license = "MIT license"
 authors = ["Jonas Teufel <jonseb1998@gmail.com>"]
 maintainers = ["Jonas Teufel <jonseb1998@gmail.com>"]
 readme = "README.rst"
 keywords = ["graph neural networks", "counterfactuals", "explainable AI"]
 packages = [
@@ -33,15 +33,15 @@
 jinja2 = ">=3.0.3"
 matplotlib = ">=3.5.3"
 numpy = ">=1.23.2"
 python-decouple = ">=3.6"
 poetry-bumpversion = ">=0.3.0"
 rdkit = ">=2022.9.5"
 pycomex = ">=0.9.2"
-visual_graph_datasets = ">=0.13.1"
+visual_graph_datasets = ">=0.13.4"
 dimorphite-dl = ">=1.3.2"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.1.3"
 poetry-bumpversion = ">=0.3.0"
 
 [tool.poetry_bumpversion.file."vgd_counterfactuals/VERSION"]
```

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/base.py` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/base.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/cli.py` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/cli.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/00_quickstart.py` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/00_quickstart.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/01_visualization.py` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/01_visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/code.py` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/code.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/README.rst` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/experiments/README.rst`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/template_experiment.py` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/experiments/template_experiment.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/experiments/template_experiment_sub.py` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/experiments/template_experiment_sub.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/__pycache__/colors.cpython-310.pyc` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/generate/__pycache__/colors.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 12:39:09 2023 UTC, .py size: 3914 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ed11 8764 4a0f 0000  o..........dJ...
+00000000: 6f0d 0d0a 0000 0000 0937 8764 490f 0000  o........7.dI...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 f800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c04 6d00 5a05 0100 6400 6402 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6400 6403 6c06 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6400 6404 6c06 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -116,15 +116,15 @@
 00000730: 0000 0072 1400 0000 7210 0000 003c 0000  ...r....r....<..
 00000740: 0073 1c00 0000 0403 1001 0801 1001 0a01  .s..............
 00000750: 2009 0401 0201 0201 0601 0601 08fc 0280   ...............
 00000760: 0407 7210 0000 0063 0200 0000 0000 0000  ..r....c........
 00000770: 0000 0000 0700 0000 0900 0000 4300 0000  ............C...
 00000780: 7382 0000 0067 007d 0274 007c 0083 017d  s....g.}.t.|...}
 00000790: 037c 0064 0119 0044 005d 347d 047c 0064  .|.d...D.]4}.|.d
-000007a0: 0119 0044 005d 2d7d 057c 047c 056b 0372  ...D.]-}.|.|.k.r
+000007a0: 0119 0044 005d 2d7d 057c 047c 056b 0472  ...D.]-}.|.|.k.r
 000007b0: 3d7c 037c 047c 0566 0219 0073 3d74 017c  =|.|.|.f...s=t.|
 000007c0: 0083 017d 0674 027c 067c 047c 0564 0264  ...}.t.|.|.|.d.d
 000007d0: 0364 0467 0169 0164 058d 0501 007c 02a0  .d.g.i.d.....|..
 000007e0: 0364 067c 01a0 047c 06a1 017c 047c 0566  .d.|...|...|.|.f
 000007f0: 027c 047c 0566 0264 079c 04a1 0101 0071  .|.|.f.d.......q
 00000800: 1071 0a7c 0253 0029 084e 7216 0000 0046  .q.|.S.).Nr....F
 00000810: da0f 6564 6765 5f61 7474 7269 6275 7465  ..edge_attribute
```

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/colors.py` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/generate/colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 def get_valid_add_edge(graph: tv.GraphDict,
                        processing: ColorProcessing
                        ) -> t.List[dict]:
     results = []
     node_adjancency = graph_node_adjacency(graph)
     for i in graph['node_indices']:
         for j in graph['node_indices']:
-            if i != j and not node_adjancency[i, j]:
+            if i > j and not node_adjancency[i, j]:
                 new_graph = copy_graph_dict(graph)
                 graph_add_edge(
                     graph=new_graph, 
                     node_index_1=i, 
                     node_index_2=j, 
                     directed=False,
                     attributes={
```

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/molecules.py` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/generate/molecules.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/generate/smiles_one_step_changes.py` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/generate/smiles_one_step_changes.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/templates/article.tex.j2` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/templates/article.tex.j2`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/utils.py` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/utils.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/vgd_counterfactuals/visualization.py` & `vgd_counterfactuals-0.3.2/vgd_counterfactuals/visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.3.1/PKG-INFO` & `vgd_counterfactuals-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgd-counterfactuals
-Version: 0.3.1
+Version: 0.3.2
 Summary: Counterfactual explanations for GNNs based on the visual graph dataset format
 License: MIT
 Keywords: graph neural networks,counterfactuals,explainable AI
 Author: Jonas Teufel
 Author-email: jonseb1998@gmail.com
 Maintainer: Jonas Teufel
 Maintainer-email: jonseb1998@gmail.com
@@ -20,28 +20,28 @@
 Requires-Dist: jinja2 (>=3.0.3)
 Requires-Dist: matplotlib (>=3.5.3)
 Requires-Dist: numpy (>=1.23.2)
 Requires-Dist: poetry-bumpversion (>=0.3.0)
 Requires-Dist: pycomex (>=0.9.2)
 Requires-Dist: python-decouple (>=3.6)
 Requires-Dist: rdkit (>=2022.9.5)
-Requires-Dist: visual_graph_datasets (>=0.13.1)
+Requires-Dist: visual_graph_datasets (>=0.13.4)
 Description-Content-Type: text/x-rst
 
 |made-with-python| |python-version| |version|
 
 .. |made-with-python| image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.3.1-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.3.2-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

