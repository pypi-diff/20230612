# Comparing `tmp/bluepysnap-1.0.5.tar.gz` & `tmp/bluepysnap-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepysnap-1.0.5.tar", last modified: Tue Mar 21 10:39:31 2023, max compression
+gzip compressed data, was "bluepysnap-1.0.6.tar", last modified: Mon Jun 12 09:38:23 2023, max compression
```

## Comparing `bluepysnap-1.0.5.tar` & `bluepysnap-1.0.6.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:39:31.535021 bluepysnap-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-03-21 10:39:31.535021 bluepysnap-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:39:31.531021 bluepysnap-1.0.5/bluepysnap/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/_doctools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14706 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/bbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/circuit_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    20974 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/circuit_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:39:31.531021 bluepysnap-1.0.5/bluepysnap/edges/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/edges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/edges/edge_population.py
--rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/edges/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/frame_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/morph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/neuron_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/node_sets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:39:31.531021 bluepysnap-1.0.5/bluepysnap/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25165 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/nodes/node_population.py
--rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/nodes/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:39:31.531021 bluepysnap-1.0.5/bluepysnap/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/circuit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:39:31.531021 bluepysnap-1.0.5/bluepysnap/schemas/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/definitions/datatypes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/definitions/edge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/definitions/node.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:39:31.535021 bluepysnap-1.0.5/bluepysnap/schemas/edge/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/edge/chemical.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/edge/chemical_virtual.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/edge/electrical.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/edge/endfoot.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/edge/glialglial.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/edge/neuromodulatory.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/edge/synapse_astrocyte.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:39:31.535021 bluepysnap-1.0.5/bluepysnap/schemas/node/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/node/astrocyte.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/node/biophysical.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/node/vasculature.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/node/virtual.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/schemas/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/sonata_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/spike_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/bluepysnap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 10:39:31.531021 bluepysnap-1.0.5/bluepysnap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-03-21 10:39:31.000000 bluepysnap-1.0.5/bluepysnap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-21 10:39:31.000000 bluepysnap-1.0.5/bluepysnap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 10:39:31.000000 bluepysnap-1.0.5/bluepysnap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-21 10:39:31.000000 bluepysnap-1.0.5/bluepysnap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-21 10:39:31.000000 bluepysnap-1.0.5/bluepysnap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-21 10:39:31.000000 bluepysnap-1.0.5/bluepysnap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 10:39:31.535021 bluepysnap-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-03-21 10:39:20.000000 bluepysnap-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.024181 bluepysnap-1.0.6/bluepysnap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/_doctools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 09:38:22.000000 bluepysnap-1.0.6/bluepysnap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/bbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/circuit_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21388 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/circuit_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.024181 bluepysnap-1.0.6/bluepysnap/edges/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/edges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24870 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/edges/edge_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/edges/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/frame_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/morph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/neuron_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/node_sets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.024181 bluepysnap-1.0.6/bluepysnap/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28955 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/nodes/node_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/nodes/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/bluepysnap/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/circuit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/bluepysnap/schemas/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/definitions/datatypes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/definitions/edge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/definitions/node.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/bluepysnap/schemas/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/chemical.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/chemical_virtual.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/electrical.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/endfoot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/glialglial.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/neuromodulatory.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/edge/synapse_astrocyte.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/bluepysnap/schemas/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/node/astrocyte.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/node/biophysical.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/node/vasculature.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/node/virtual.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/schemas/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/sonata_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/spike_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/bluepysnap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:23.024181 bluepysnap-1.0.6/bluepysnap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-12 09:38:22.000000 bluepysnap-1.0.6/bluepysnap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-12 09:38:23.000000 bluepysnap-1.0.6/bluepysnap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:38:22.000000 bluepysnap-1.0.6/bluepysnap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 09:38:22.000000 bluepysnap-1.0.6/bluepysnap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-12 09:38:22.000000 bluepysnap-1.0.6/bluepysnap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 09:38:22.000000 bluepysnap-1.0.6/bluepysnap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:38:23.028181 bluepysnap-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-12 09:38:17.000000 bluepysnap-1.0.6/setup.py
```

### Comparing `bluepysnap-1.0.5/COPYING` & `bluepysnap-1.0.6/COPYING`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/COPYING.LESSER` & `bluepysnap-1.0.6/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/PKG-INFO` & `bluepysnap-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: bluepysnap
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simulation and Neural network Analysis Productivity layer
 Home-page: https://github.com/BlueBrain/snap
 Author: Blue Brain Project, EPFL
 License: LGPLv3
 Keywords: SONATA,BlueBrainProject
 Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: plots
 Provides-Extra: spatial-index
 License-File: COPYING
 License-File: COPYING.LESSER
 License-File: AUTHORS.txt
```

### Comparing `bluepysnap-1.0.5/README.rst` & `bluepysnap-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/__init__.py` & `bluepysnap-1.0.6/bluepysnap/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,7 +17,12 @@
 
 """Simulation and Neural network Analysis Productivity layer."""
 
 from bluepysnap.circuit import Circuit
 from bluepysnap.config import Config
 from bluepysnap.exceptions import BluepySnapError
 from bluepysnap.simulation import Simulation
+
+try:
+    from bluepysnap._version import version as __version__
+except ImportError:  # pragma: no cover
+    __version__ = "unknown"
```

### Comparing `bluepysnap-1.0.5/bluepysnap/_doctools.py` & `bluepysnap-1.0.6/bluepysnap/_doctools.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/_plotting.py` & `bluepysnap-1.0.6/bluepysnap/_plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,42 +58,37 @@
         then a default layout is set using pyplot.gca().
     """
     # pylint: disable=too-many-locals
     plt = _get_pyplot()
     if time_binsize is not None and time_binsize <= 0:
         raise BluepySnapError(f"Invalid time_binsize = {time_binsize}. Should be > 0.")
 
-    spike_report = filtered_report.spike_report
-
-    times = filtered_report.report.index
-    node_count = filtered_report.report[["ids", "population"]].drop_duplicates().shape[0]
-
-    if len(times) == 0:
-        raise BluepySnapError(
-            "No data to display. You should check your " f"'group' query: {spike_report.group}."
-        )
-
-    time_start = np.min(times)
-    time_stop = np.max(times)
-
-    if time_binsize is None:
-        # heuristic for a nice bin size (~100 spikes per bin on average)
-        time_binsize = min(50.0, (time_stop - time_start) / ((len(times) / 100.0) + 1.0))
-
-    bins = np.append(np.arange(time_start, time_stop, time_binsize), time_stop)
-    hist, bin_edges = np.histogram(times, bins=bins)
-    freq = 1.0 * hist / node_count / (0.001 * time_binsize)
-
     if ax is None:
         ax = plt.gca()
         ax.set_xlabel("Time [ms]")
         ax.set_ylabel("PSTH [Hz]")
 
-    # use the middle of the bins instead of the start of the bin
-    ax.plot(0.5 * (bin_edges[1:] + bin_edges[:-1]), freq, label="PSTH", drawstyle="steps-mid")
+    times = filtered_report.report.index
+
+    if len(times) > 0:
+        time_start = np.min(times)
+        time_stop = np.max(times)
+
+        if time_binsize is None:
+            # heuristic for a nice bin size (~100 spikes per bin on average)
+            time_binsize = min(50.0, (time_stop - time_start) / ((len(times) / 100.0) + 1.0))
+
+        bins = np.append(np.arange(time_start, time_stop, time_binsize), time_stop)
+        hist, bin_edges = np.histogram(times, bins=bins)
+        node_count = filtered_report.report[["ids", "population"]].drop_duplicates().shape[0]
+        freq = 1.0 * hist / node_count / (0.001 * time_binsize)
+
+        # use the middle of the bins instead of the start of the bin
+        ax.plot(0.5 * (bin_edges[1:] + bin_edges[:-1]), freq, label="PSTH", drawstyle="steps-mid")
+
     return ax
 
 
 def spike_raster(filtered_report, y_axis=None, ax=None):  # pragma: no cover
     """Spike raster plot.
 
     Shows a global overview of the circuit's firing nodes. The y axis can project either the
@@ -210,16 +205,15 @@
         raise BluepySnapError(f"Invalid binsize = {binsize}. Should be > 0.")
 
     gb = filtered_report.report.groupby(["ids", "population"])
     values = np.concatenate([np.diff(node_spikes.index.to_numpy()) for _, node_spikes in gb])
 
     if len(values) == 0:
         raise BluepySnapError(
-            "No data to display. You should check your "
-            f"'group' query: {filtered_report.spike_report.group}."
+            f"No data to display. You should check your 'group' query: {filtered_report.group}."
         )
     if use_frequency:
         values = values[values > 0]  # filter out zero intervals
         values = 1000.0 / values
 
     if binsize is None:
         bins = "auto"
```

### Comparing `bluepysnap-1.0.5/bluepysnap/bbp.py` & `bluepysnap-1.0.6/bluepysnap/bbp.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/circuit.py` & `bluepysnap-1.0.6/bluepysnap/circuit.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,23 +12,26 @@
 # details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 """Access to circuit data."""
+import logging
 
 from cached_property import cached_property
 
-from bluepysnap.config import CircuitConfig
+from bluepysnap.config import CircuitConfig, CircuitConfigStatus
 from bluepysnap.edges import Edges
 from bluepysnap.exceptions import BluepySnapError
 from bluepysnap.node_sets import NodeSets
 from bluepysnap.nodes import Nodes
 
+L = logging.getLogger(__name__)
+
 
 class Circuit:
     """Access to circuit data."""
 
     def __init__(self, config):
         """Initializes a circuit object from a SONATA config file.
 
@@ -37,14 +40,20 @@
 
         Returns:
             Circuit: A Circuit object.
         """
         self._circuit_config_path = config
         self._config = CircuitConfig.from_config(config)
 
+        if self.partial_config:
+            L.info(
+                "Loaded PARTIAL circuit config. Functionality may be limited. "
+                "It is up to the user to be diligent when accessing properties."
+            )
+
     @property
     def to_libsonata(self):
         """Libsonata instance of the circuit."""
         return self._config.to_libsonata
 
     @property
     def config(self):
@@ -78,14 +87,19 @@
         return Nodes(self)
 
     @cached_property
     def edges(self):
         """Access to edge population(s). See :py:class:`~bluepysnap.edges.Edges`."""
         return Edges(self)
 
+    @cached_property
+    def partial_config(self):
+        """Check partiality of the config."""
+        return self._config.status == CircuitConfigStatus.partial
+
     def __getstate__(self):
         """Make Circuits pickle-able, without storing state of caches."""
         return self._circuit_config_path
 
     def __setstate__(self, state):
         """Load from pickle state."""
         self.__init__(state)
```

### Comparing `bluepysnap-1.0.5/bluepysnap/circuit_ids.py` & `bluepysnap-1.0.6/bluepysnap/circuit_ids.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/circuit_validation.py` & `bluepysnap-1.0.6/bluepysnap/circuit_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,18 @@
 
     Returns:
         Error: Error with level FATAL
     """
     return Error(Error.FATAL, message)
 
 
+def _check_partial_circuit_config(config):
+    return config.get("metadata", {}).get("status") == "partial"
+
+
 def _check_components_dir(name, components):
     """Checks existence of directory within Sonata config 'components'.
 
     Args:
         name (str): components directory name
         components (dict): ref to config's components
 
@@ -615,14 +619,22 @@
     """
     config = Parser.parse(load_json(config_file), str(Path(config_file).parent))
     errors = schemas.validate_circuit_schema(config_file, config)
 
     if "networks" in config:
         errors += validate_networks(config, skip_slow)
 
+    if _check_partial_circuit_config(config):
+        message = (
+            "The Circuit config is partial. Validity cannot be established "
+            "for partial configs as it depends on the intended use. "
+        )
+        L.warning(message)
+        errors.append(Error(Error.WARNING, message))
+
     if only_errors:
         errors = [e for e in errors if e.level == Error.FATAL]
 
     if print_errors:
         _print_errors(errors)
 
     return set(errors)
```

### Comparing `bluepysnap-1.0.5/bluepysnap/cli.py` & `bluepysnap-1.0.6/bluepysnap/cli.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/config.py` & `bluepysnap-1.0.6/bluepysnap/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 import copy
 import json
 from collections.abc import Iterable, Mapping
 from pathlib import Path
 
 import libsonata
+from libsonata import CircuitConfigStatus
 
 from bluepysnap.exceptions import BluepySnapError
 
 # List of keys which are expected to have paths
 EXPECTED_PATH_KEYS = {
     "morphologies_dir",
     "biophysical_neuron_models_dir",
@@ -61,16 +62,16 @@
             config (dict): Dict containing the config.
             config_dir(str):  Path to the directory containing the config file.
 
         Returns:
              Parser: A Parser object.
         """
         content = config.copy()
-
-        self.manifest = Parser._resolve_manifest(content.pop("manifest", {}), config_dir)
+        manifest = content.pop("manifest", None) or {}
+        self.manifest = Parser._resolve_manifest(manifest, config_dir)
         self.content = content
 
     @staticmethod
     def _resolve_manifest(manifest, configdir):
         result = manifest.copy()
 
         for k, v in result.items():
@@ -180,14 +181,19 @@
         return self._populations["nodes"]
 
     @property
     def edge_populations(self):
         """Access edge population configs."""
         return self._populations["edges"]
 
+    @property
+    def status(self) -> CircuitConfigStatus:
+        """Return status of the config."""
+        return self._libsonata.config_status
+
     @staticmethod
     def _resolve_population_configs(config):
         """Resolves population configs for the node and edge populations."""
         networks = config.get("networks") or {}
         components = config.get("components") or {}
 
         def resolve_network_populations(element_type):
```

### Comparing `bluepysnap-1.0.5/bluepysnap/edges/edge_population.py` & `bluepysnap-1.0.6/bluepysnap/edges/edge_population.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,25 @@
 
         Returns:
             EdgePopulation: An EdgePopulation object.
         """
         self._circuit = circuit
         self.name = population_name
 
-    @property
+    @cached_property
     def _properties(self):
+        """Edge population properties."""
         return self._circuit.to_libsonata.edge_population_properties(self.name)
 
     @property
     def _population(self):
+        """Libsonata edge population.
+
+        Not cached because it would keep the hdf5 file open.
+        """
         return self._circuit.to_libsonata.edge_population(self.name)
 
     @staticmethod
     def _resolve_node_ids(nodes, group):
         """Node IDs corresponding to node group filter."""
         if group is None:
             return None
@@ -586,18 +591,18 @@
             raise BluepySnapError(
                 (
                     "Spatial index is for now only available internally to BBP. "
                     "It requires `spatial_index`, an internal package."
                 )
             ) from e
 
-        properties = self._circuit.to_libsonata.edge_population_properties(self.name)
-        if not properties.spatial_synapse_index_dir:
+        index_dir = self._properties.spatial_synapse_index_dir
+        if not index_dir:
             raise BluepySnapError(f"It appears {self.name} does not have synapse indices")
-        return open_index(properties.spatial_synapse_index_dir)
+        return open_index(index_dir)
 
     def __getstate__(self):
         """Make EdgePopulation pickle-able, without storing state of caches."""
         return self._circuit, self.name
 
     def __setstate__(self, state):
         """Load from pickle state."""
```

### Comparing `bluepysnap-1.0.5/bluepysnap/edges/edges.py` & `bluepysnap-1.0.6/bluepysnap/edges/edges.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/exceptions.py` & `bluepysnap-1.0.6/bluepysnap/exceptions.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/frame_report.py` & `bluepysnap-1.0.6/bluepysnap/frame_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,28 +72,39 @@
         raise NotImplementedError
 
     @staticmethod
     def _wrap_columns(columns):
         """Allows to change the columns names if needed."""
         return columns
 
-    def get(self, group=None, t_start=None, t_stop=None):
+    def get(self, group=None, t_start=None, t_stop=None, t_step=None):
         """Fetch data from the report.
 
         Args:
             group (None/int/list/np.array/dict): Get frames filtered by :ref:`Group Concept`.
             t_start (float): Include only frames occurring at or after this time.
             t_stop (float): Include only frames occurring at or before this time.
+            t_step (float): Optional time step, useful to reduce the number of samples.
+                It should be a multiple of the report time step dt, and it's equal to dt by default.
+                If the given t_step isn't an exact multiple, it's rounded to the closer multiple.
+                Only the samples at t = t0 + k * t_step, for k = 0, 1... are returned,
+                where t0 is the first sample time >= t_start.
 
         Returns:
             pandas.DataFrame: frame as columns indexed by timestamps.
         """
+        t_stride = round(t_step / self.frame_report.dt) if t_step is not None else 1
+        if t_stride < 1:
+            msg = f"Invalid {t_step=}. It should be None or a multiple of {self.frame_report.dt}."
+            raise BluepySnapError(msg)
         ids = self._resolve(group).tolist()
         try:
-            view = self._frame_population.get(node_ids=ids, tstart=t_start, tstop=t_stop)
+            view = self._frame_population.get(
+                node_ids=ids, tstart=t_start, tstop=t_stop, tstride=t_stride
+            )
         except SonataError as e:
             raise BluepySnapError(e) from e
 
         if len(view.ids) == 0:
             return pd.DataFrame()
 
         # cell ids and section ids in the columns are enforced to be int64
```

### Comparing `bluepysnap-1.0.5/bluepysnap/morph.py` & `bluepysnap-1.0.6/bluepysnap/morph.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/network.py` & `bluepysnap-1.0.6/bluepysnap/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,17 @@
             limit (int): If specified, return the first ``limit`` number of
                 IDs from the match result. If limit is greater than the size of all the population
                 then all IDs are returned.
 
         Returns:
             CircuitNodeIds/CircuitEdgeIds: containing the IDs and the populations.
         """
+        if not self.population_names:
+            raise BluepySnapError("Cannot create CircuitIds for empty population.")
+
         str_type = f"<U{max(len(pop) for pop in self.population_names)}"
         ids = []
         populations = []
         for pop in self.values():
             pop_ids, name_ids = fun_to_apply(pop)
             pops = np.full_like(pop_ids, fill_value=name_ids, dtype=str_type)
             ids.append(pop_ids)
```

### Comparing `bluepysnap-1.0.5/bluepysnap/neuron_models.py` & `bluepysnap-1.0.6/bluepysnap/neuron_models.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/node_sets.py` & `bluepysnap-1.0.6/bluepysnap/node_sets.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/nodes/node_population.py` & `bluepysnap-1.0.6/bluepysnap/nodes/node_population.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
     See more examples in ``NodePopulation::get``
 """
 import inspect
 from collections.abc import Mapping, Sequence
 from copy import deepcopy
 
+import libsonata
 import numpy as np
 import pandas as pd
 from cached_property import cached_property
 from more_itertools import first
 
 from bluepysnap import query, utils
 from bluepysnap.circuit_ids import CircuitNodeId, CircuitNodeIds
@@ -90,44 +91,118 @@
 
     @property
     def _node_sets(self):
         """Node sets defined for this node population."""
         return self._circuit.node_sets
 
     @cached_property
-    def _data(self):
-        """Collect data for the node population as a pandas.DataFrame."""
-        nodes = self._population
-        categoricals = nodes.enumeration_names
-
-        _all = nodes.select_all()
-        result = pd.DataFrame(index=np.arange(_all.flat_size))
-
-        for attr in sorted(nodes.attribute_names):
-            if attr in categoricals:
-                enumeration = np.asarray(nodes.get_enumeration(attr, _all))
-                values = np.asarray(nodes.enumeration_values(attr))
-                # if the size of `values` is large enough compared to `enumeration`, not using
-                # categorical reduces the memory usage.
-                if values.shape[0] < 0.5 * enumeration.shape[0]:
-                    result[attr] = pd.Categorical.from_codes(enumeration, categories=values)
-                else:
-                    result[attr] = values[enumeration]
-            else:
-                result[attr] = nodes.get_attribute(attr, _all)
-        for attr in sorted(utils.add_dynamic_prefix(nodes.dynamics_attribute_names)):
-            result[attr] = nodes.get_dynamics_attribute(attr.split(DYNAMICS_PREFIX)[1], _all)
+    def _cache(self):
+        """Cached DataFrame of nodes, to be accessed through _get_data()."""
+        return pd.DataFrame(index=pd.RangeIndex(self.size, name="node_ids"))
+
+    def _get_libsonata_selection(self, node_ids):
+        """Return a libsonata Selection from the given node_ids."""
+        if node_ids is None:
+            return libsonata.Selection([(0, self.size)])
+        return libsonata.Selection(node_ids)
+
+    def _get_values_from_sonata(self, nodes, attr, node_ids):
+        """Return the selected values as np.ndarray or pd.Categorical."""
+        selection = self._get_libsonata_selection(node_ids)
+        if attr in nodes.enumeration_names:
+            enumeration = np.asarray(nodes.get_enumeration(attr, selection))
+            values = np.asarray(nodes.enumeration_values(attr))
+            # if the size of `values` is large enough compared to `enumeration`, not using
+            # categorical reduces the memory usage.
+            # We compare with nodes.size instead of len(enumeration) to not depend on the selection.
+            if len(values) < 0.5 * nodes.size:
+                return pd.Categorical.from_codes(enumeration, categories=values)
+            return values[enumeration]
+        if attr in nodes.attribute_names:
+            return nodes.get_attribute(attr, selection)
+        if attr.startswith(DYNAMICS_PREFIX):
+            stripped = attr[len(DYNAMICS_PREFIX) :]
+            if stripped in nodes.dynamics_attribute_names:
+                return nodes.get_dynamics_attribute(stripped, selection)
+        raise BluepySnapError(f"Attribute not found in population {self.name}: {attr}")
+
+    def _iter_selected_properties(self, existing, desired):
+        """Yield ordered (idx, attr) for each attr in desired, and not in existing.
+
+        Called to ensure that the order of the columns of the cached DataFrame doesn't depend
+        on the order of the retrieved attributes, when _get_data is called multiple times
+        with different properties.
+
+        Args:
+            existing: existing attributes, that are going to be skipped.
+            desired: desired attributes, that are going to be yielded in order.
+        """
+        idx = 0
+        existing = set(existing)
+        desired = set(desired)
+        for attr in self._ordered_property_names:
+            if attr in existing:
+                idx += 1
+                continue
+            if attr not in desired:
+                continue
+            yield idx, attr
+
+    def _get_data(self, properties=None, node_ids=None):
+        """Collect data for the node population as a pandas.DataFrame.
+
+        Return a DataFrame with node_ids as index, loading the requested properties if needed.
+
+        The returned DataFrame isn't filtered by columns, so it may contain more properties than
+        requested, if they were loaded previously.
+
+        This is done for efficiency, since a copy of the data is not needed:
+        - in self.get(), the DataFrame is filtered by node_ids first, and by property later
+        - in self.property_dtypes(), all the properties are needed
+        - in self._node_ids_by_filter(), the required columns are selected if and when needed
+
+        Args:
+            properties (str|set|list|None): properties to load, or None to load all of them.
+            node_ids (list|np.ndarray|None): node ids to select.
+                If None, all the ids are selected, and the cache is read and updated if needed.
+                If not None, the cache is read and used if possible, but not updated.
+        """
+        result = self._cache
+        if properties is None:
+            properties_set = self.property_names
+        else:
+            properties_set = set(utils.ensure_list(properties))
+            self._check_properties(properties_set)
+        if node_ids is not None:
+            # Select the ids from the cached dataframe.
+            # The original dataframe won't be updated in this case.
+            result = result.loc[node_ids]
+        cached_columns = properties_set.intersection(result.columns)
+        if len(cached_columns) < len(properties_set):
+            # some requested properties miss from the cache
+            nodes = self._population
+            # insert columns at the correct position
+            for n, (loc, name) in enumerate(
+                self._iter_selected_properties(existing=result.columns, desired=properties_set)
+            ):
+                values = self._get_values_from_sonata(nodes=nodes, attr=name, node_ids=node_ids)
+                result.insert(n + loc, name, values)
         return result
 
-    @property
+    @cached_property
     def _properties(self):
+        """Node population properties."""
         return self._circuit.to_libsonata.node_population_properties(self.name)
 
     @property
     def _population(self):
+        """Libsonata node population.
+
+        Not cached because it would keep the hdf5 file open.
+        """
         return self._circuit.to_libsonata.node_population(self.name)
 
     @cached_property
     def size(self):
         """Node population size."""
         return self._population.size
 
@@ -140,14 +215,19 @@
     def _property_names(self):
         return set(self._population.attribute_names)
 
     @cached_property
     def _dynamics_params_names(self):
         return set(utils.add_dynamic_prefix(self._population.dynamics_attribute_names))
 
+    @cached_property
+    def _ordered_property_names(self):
+        """Similar to self.property_names, but as an ordered list."""
+        return sorted(self._property_names) + sorted(self._dynamics_params_names)
+
     def source_in_edges(self):
         """Set of edge population names that use this node population as source.
 
         Returns:
             set: a set containing the names of edge populations using this NodePopulation as
             source.
         """
@@ -232,42 +312,43 @@
     @cached_property
     def property_dtypes(self):
         """Returns the dtypes of all the properties.
 
         Returns:
             pandas.Series: series indexed by field name with the corresponding dtype as value.
         """
-        return self._data.dtypes.sort_index()
+        # read all the properties, without loading any node id
+        return self._get_data(properties=None, node_ids=[]).dtypes.sort_index()
 
     def _check_id(self, node_id):
         """Check that single node ID belongs to the circuit."""
-        if node_id not in self._data.index:
+        if node_id < 0 or node_id >= self.size:
             raise BluepySnapError(f"node ID not found: {node_id} in population '{self.name}'")
 
     def _check_ids(self, node_ids):
         """Check that node IDs belong to the circuit."""
         if len(node_ids) == 0:
             return
         # use the function with better performance for arrays or lists
         if isinstance(node_ids, np.ndarray):
             max_id = node_ids.max()
             min_id = node_ids.min()
         else:
             max_id = max(node_ids)
             min_id = min(node_ids)
-        if min_id < 0 or max_id >= self._data.index.shape[0]:
+        if min_id < 0 or max_id >= self.size:
             raise BluepySnapError(
-                f"All node IDs must be >= 0 and < {self._data.index.shape[0]} "
-                f"for population '{self.name}'"
+                f"All node IDs must be >= 0 and < {self.size} " f"for population '{self.name}'"
             )
 
-    def _check_property(self, prop):
-        """Check if a property exists inside the dataset."""
-        if prop not in self.property_names:
-            raise BluepySnapError(f"No such property: '{prop}'")
+    def _check_properties(self, properties):
+        """Check if the properties exist inside the dataset."""
+        unknown_props = properties - self.property_names
+        if unknown_props:
+            raise BluepySnapError(f"Unknown node properties: {sorted(unknown_props)}")
 
     def _get_node_set(self, node_set_name):
         """Returns the node set named 'node_set_name'."""
         if node_set_name not in self._node_sets:
             raise BluepySnapError(f"Undefined node set: '{node_set_name}'")
         return self._node_sets[node_set_name]
 
@@ -297,21 +378,21 @@
             >>> _node_ids_by_filter({ Node.X: (0, 1), Node.MTYPE: 'L1_SLAC' })
             >>> _node_ids_by_filter({ Node.LAYER: [2, 3] })
             >>> _node_ids_by_filter({'$or': [{ Node.LAYER: [2, 3]},
             >>>                              { Node.X: (0, 1), Node.MTYPE: 'L1_SLAC' }]})
 
         """
         queries = self._resolve_nodesets(queries)
+        properties = query.get_properties(queries)
         if raise_missing_prop:
-            properties = query.get_properties(queries)
-            if not properties.issubset(self._data.columns):
-                unknown_props = properties - set(self._data.columns)
-                raise BluepySnapError(f"Unknown node properties: {unknown_props}")
-        idx = query.resolve_ids(self._data, self.name, queries)
-        return self._data.index[idx].values
+            self._check_properties(properties)
+        # load all the properties needed to execute the query, excluding the unknown properties
+        data = self._get_data(properties & self.property_names)
+        idx = query.resolve_ids(data, self.name, queries)
+        return idx.nonzero()[0]
 
     def ids(self, group=None, limit=None, sample=None, raise_missing_property=True):
         """Node IDs corresponding to node ``group``.
 
         Args:
             group (int/CircuitNodeId/CircuitNodeIds/sequence/str/mapping/None):
                 See :ref:`Group Concept`
@@ -333,15 +414,15 @@
         preserve_order = False
         if isinstance(group, str):
             group = self._get_node_set(group)
         elif isinstance(group, CircuitNodeIds):
             group = group.filter_population(self.name).get_ids()
 
         if group is None:
-            result = self._data.index.values
+            result = np.arange(self.size)
         elif isinstance(group, Mapping):
             result = self._node_ids_by_filter(
                 queries=group, raise_missing_prop=raise_missing_property
             )
         elif isinstance(group, np.ndarray):
             result = group
             self._check_ids(result)
@@ -375,15 +456,15 @@
     def get(self, group=None, properties=None):
         """Node properties as a pandas Series or DataFrame.
 
         Args:
             group (int/CircuitNodeId/CircuitNodeIds/sequence/str/mapping/None):
                 see :ref:`Group Concept`
             properties (list|str|None): If specified, return only the properties in the list.
-                Otherwise return all properties.
+                Otherwise, return all the properties.
 
         Returns:
             value/pandas.Series/pandas.DataFrame:
                 The type of the returned object depends on the type of the input parameters,
                 see the Examples for an explanation of the different cases.
 
         Notes:
@@ -437,29 +518,25 @@
                 >>> type(result), result.shape
                 (pandas.core.frame.DataFrame, (3, 1))
 
                 >>> result = my_node_population.get(group=[0], properties=[Cell.MTYPE])
                 >>> type(result), result.shape
                 (pandas.core.frame.DataFrame, (1, 1))
         """
-        result = self._data
-        if properties is not None:
-            for p in utils.ensure_list(properties):
-                self._check_property(p)
-            result = result[properties]
-
         if group is not None:
             if isinstance(group, (int, np.integer)):
                 self._check_id(group)
             elif isinstance(group, CircuitNodeId):
                 group = self.ids(group)[0]
             else:
                 group = self.ids(group)
-            result = result.loc[group]
 
+        result = self._get_data(properties=properties)
+        result = result.loc[group] if group is not None else result
+        result = result[properties] if properties is not None else result
         return result
 
     def positions(self, group=None):
         """Node position(s) as pandas Series or DataFrame.
 
         Args:
             group (int/CircuitNodeId/CircuitNodeIds/sequence/str/mapping/None): Which nodes will
@@ -589,20 +666,18 @@
             raise BluepySnapError(
                 (
                     "Spatial index is for now only available internally to BBP. ",
                     "It requires `spatial_index`, an internal package.",
                 )
             ) from e
 
-        properties = self._circuit.to_libsonata.node_population_properties(self.name)
-
-        if not properties.spatial_segment_index_dir:
+        index_dir = self._properties.spatial_segment_index_dir
+        if not index_dir:
             raise BluepySnapError(f"It appears {self.name} does not have segment indices")
-
-        return open_index(properties.spatial_segment_index_dir)
+        return open_index(index_dir)
 
     def __getstate__(self):
         """Make NodePopulation pickle-able, without storing state of caches."""
         return (self._circuit, self.name)
 
     def __setstate__(self, state):
         """Load from pickle state."""
```

### Comparing `bluepysnap-1.0.5/bluepysnap/nodes/nodes.py` & `bluepysnap-1.0.6/bluepysnap/nodes/nodes.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/query.py` & `bluepysnap-1.0.6/bluepysnap/query.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/schemas/circuit.yaml` & `bluepysnap-1.0.6/bluepysnap/schemas/circuit.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/schemas/definitions/datatypes.yaml` & `bluepysnap-1.0.6/bluepysnap/schemas/definitions/datatypes.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/schemas/definitions/edge.yaml` & `bluepysnap-1.0.6/bluepysnap/schemas/definitions/edge.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/schemas/definitions/node.yaml` & `bluepysnap-1.0.6/bluepysnap/schemas/definitions/node.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/schemas/edge/chemical.yaml` & `bluepysnap-1.0.6/bluepysnap/schemas/edge/chemical.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/schemas/edge/chemical_virtual.yaml` & `bluepysnap-1.0.6/bluepysnap/schemas/edge/chemical_virtual.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/schemas/edge/electrical.yaml` & `bluepysnap-1.0.6/bluepysnap/schemas/edge/electrical.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/schemas/edge/endfoot.yaml` & `bluepysnap-1.0.6/bluepysnap/schemas/edge/endfoot.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/schemas/edge/glialglial.yaml` & `bluepysnap-1.0.6/bluepysnap/schemas/edge/glialglial.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/schemas/edge/synapse_astrocyte.yaml` & `bluepysnap-1.0.6/bluepysnap/schemas/edge/synapse_astrocyte.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/schemas/node/biophysical.yaml` & `bluepysnap-1.0.6/bluepysnap/schemas/node/biophysical.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/schemas/node/vasculature.yaml` & `bluepysnap-1.0.6/bluepysnap/schemas/node/vasculature.yaml`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/schemas/schemas.py` & `bluepysnap-1.0.6/bluepysnap/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/settings.py` & `bluepysnap-1.0.6/bluepysnap/settings.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/simulation.py` & `bluepysnap-1.0.6/bluepysnap/simulation.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/sonata_constants.py` & `bluepysnap-1.0.6/bluepysnap/sonata_constants.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap/spike_report.py` & `bluepysnap-1.0.6/bluepysnap/spike_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         Args:
             spike_report (SpikeReport): The SpikeReport to filter.
             group (None/int/list/np.array/dict): Get spikes filtered by group. See NodePopulation.
             t_start (float): Include only frames occurring at or after this time.
             t_stop (float): Include only frames occurring at or before this time.
 
         Returns:
-            FilteredSpikeReport: A FilteredFrameReport object.
+            FilteredSpikeReport: A FilteredSpikeReport object.
         """
         self.spike_report = spike_report
         self.group = group
         self.t_start = t_start
         self.t_stop = t_stop
 
     @cached_property
@@ -263,10 +263,10 @@
 
         Args:
             group (None/int/list/np.array/dict): Get spikes filtered by group. See NodePopulation.
             t_start (float): Include only frames occurring at or after this time.
             t_stop (float): Include only frames occurring at or before this time.
 
         Returns:
-            FilteredSpikeReport: A FilteredFrameReport object.
+            FilteredSpikeReport: A FilteredSpikeReport object.
         """
         return FilteredSpikeReport(self, group, t_start, t_stop)
```

### Comparing `bluepysnap-1.0.5/bluepysnap/utils.py` & `bluepysnap-1.0.6/bluepysnap/utils.py`

 * *Files identical despite different names*

### Comparing `bluepysnap-1.0.5/bluepysnap.egg-info/PKG-INFO` & `bluepysnap-1.0.6/bluepysnap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: bluepysnap
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simulation and Neural network Analysis Productivity layer
 Home-page: https://github.com/BlueBrain/snap
 Author: Blue Brain Project, EPFL
 License: LGPLv3
 Keywords: SONATA,BlueBrainProject
 Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: plots
 Provides-Extra: spatial-index
 License-File: COPYING
 License-File: COPYING.LESSER
 License-File: AUTHORS.txt
```

### Comparing `bluepysnap-1.0.5/bluepysnap.egg-info/SOURCES.txt` & `bluepysnap-1.0.6/bluepysnap.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.py
 bluepysnap/__init__.py
 bluepysnap/_doctools.py
 bluepysnap/_plotting.py
+bluepysnap/_version.py
 bluepysnap/bbp.py
 bluepysnap/circuit.py
 bluepysnap/circuit_ids.py
 bluepysnap/circuit_validation.py
 bluepysnap/cli.py
 bluepysnap/config.py
 bluepysnap/exceptions.py
```

### Comparing `bluepysnap-1.0.5/pyproject.toml` & `bluepysnap-1.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [tool.black]
 line-length  =  100
 target-version  =  [
-    'py37',
+    'py38',
 ]
 include  =  '(bluepysnap|tests)\/.*\.py|doc\/source\/conf\.py|setup\.py'
 
 [tool.isort]
 profile  =  'black'
 line_length  =  100
 known_local_folder  =  [
 'utils',
 'test_module',
 ]
 
+[tool.pylint.main]
+# Files or directories to be skipped. They should be base names, not paths.
+ignore = ["CVS", "_version.py"]
+
 [tool.pylint.messages_control]
 disable = [
     'fixme',
     'invalid-name',
     'len-as-condition',
     'no-else-return',
     'import-outside-toplevel',
```

### Comparing `bluepysnap-1.0.5/setup.py` & `bluepysnap-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,37 +37,39 @@
 
 
 with open("README.rst") as f:
     README = f.read()
 
 setup(
     name="bluepysnap",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
         "cached_property>=1.0",
         "h5py>=3.0.1,<4.0.0",
         "jsonschema>=4.0.0,<5.0.0",
-        "libsonata>=0.1.17,<1.0.0",
+        "libsonata>=0.1.20,<1.0.0",
         "morphio>=3.0.0,<4.0.0",
         "morph-tool>=2.4.3,<3.0.0",
         "numpy>=1.8",
         "pandas>=1.0.0",
         "click>=7.0",
         "more-itertools>=8.2.0",
     ],
     extras_require={
         "docs": ["sphinx", "sphinx-bluebrain-theme"],
         "plots": ["matplotlib>=3.0.0"],
-        "spatial-index": ["spatial-index>=1.2.1,<2.0"],
+        "spatial-index": ["spatial-index>=1.2.1"],
     },
     packages=find_packages(),
     package_data={
         "bluepysnap": ["schemas/*.yaml", "schemas/*/*.yaml"],
     },
-    use_scm_version=True,
+    use_scm_version={
+        "write_to": "bluepysnap/_version.py",
+    },
     setup_requires=[
         "setuptools_scm",
     ],
     cmdclass={
         "egg_info": EggInfo,
     },
     entry_points="""
@@ -79,17 +81,17 @@
     long_description=README,
     long_description_content_type="text/x-rst",
     license="LGPLv3",
     url="https://github.com/BlueBrain/snap",
     keywords=["SONATA", "BlueBrainProject"],
     classifiers=[
         "Development Status :: 3 - Alpha",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: POSIX",
         "Topic :: Scientific/Engineering",
         "Topic :: Utilities",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     ],
 )
```

