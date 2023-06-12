# Comparing `tmp/pulumiverse_exoscale-0.48.0.tar.gz` & `tmp/pulumiverse_exoscale-0.49.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_exoscale-0.48.0.tar", last modified: Fri May 19 21:04:18 2023, max compression
+gzip compressed data, was "pulumiverse_exoscale-0.49.0.tar", last modified: Mon Jun 12 08:57:37 2023, max compression
```

## Comparing `pulumiverse_exoscale-0.48.0.tar` & `pulumiverse_exoscale-0.49.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:04:18.410469 pulumiverse_exoscale-0.48.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-19 21:04:18.410469 pulumiverse_exoscale-0.48.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:04:18.410469 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51270 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    59349 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    50320 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/compute_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:04:18.410469 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    40713 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    18856 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_instance_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_instance_pool_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_nlb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    19159 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    18631 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_cluster_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_nodepool_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/iam_access_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    53079 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    37973 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/nic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/nlb.py
--rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/nlb_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    90177 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    16432 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/secondary_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    39602 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/security_group_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/security_group_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    39936 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/sks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/sks_kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    41557 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/sks_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/ssh_keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:04:18.410469 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:04:18.410469 pulumiverse_exoscale-0.48.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:57:37.173968 pulumiverse_exoscale-0.49.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-12 08:57:37.173968 pulumiverse_exoscale-0.49.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:57:37.169968 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51270 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59349 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50320 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/compute_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:57:37.173968 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39665 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18856 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_instance_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_database_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_instance_pool_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_nlb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19402 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18631 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_cluster_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_nodepool_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/iam_access_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53079 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37973 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/nic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/nlb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/nlb_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90177 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16360 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/secondary_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39602 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/security_group_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/security_group_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40583 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/sks_kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41557 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/ssh_keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:57:37.173968 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-12 08:57:37.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-12 08:57:37.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:57:37.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:57:37.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 08:57:37.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 08:57:37.000000 pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 08:57:37.173968 pulumiverse_exoscale-0.49.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-12 08:57:36.000000 pulumiverse_exoscale-0.49.0/setup.py
```

### Comparing `pulumiverse_exoscale-0.48.0/PKG-INFO` & `pulumiverse_exoscale-0.49.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_exoscale
-Version: 0.48.0
+Version: 0.49.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_exoscale-0.48.0/README.md` & `pulumiverse_exoscale-0.49.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/__init__.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .get_affinity import *
 from .get_anti_affinity_group import *
 from .get_compute import *
 from .get_compute_instance import *
 from .get_compute_instance_list import *
 from .get_compute_ip_address import *
 from .get_compute_template import *
+from .get_database_uri import *
 from .get_domain import *
 from .get_domain_record import *
 from .get_elastic_ip import *
 from .get_instance_pool import *
 from .get_instance_pool_list import *
 from .get_network import *
 from .get_nlb import *
```

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/_inputs.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/_utilities.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/affinity.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/affinity.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/anti_affinity_group.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/anti_affinity_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/compute.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/compute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/compute_instance.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/compute_instance.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/config/vars.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/database.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,14 @@
                  pg: Optional[pulumi.Input['DatabasePgArgs']] = None,
                  plan: Optional[pulumi.Input[str]] = None,
                  redis: Optional[pulumi.Input['DatabaseRedisArgs']] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  termination_protection: Optional[pulumi.Input[bool]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  updated_at: Optional[pulumi.Input[str]] = None,
-                 uri: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Database resources.
         :param pulumi.Input[str] ca_certificate: CA Certificate required to reach a DBaaS service through a TLS-protected connection.
         :param pulumi.Input[str] created_at: The creation date of the database service.
         :param pulumi.Input[int] disk_size: The disk size of the database service.
         :param pulumi.Input['DatabaseKafkaArgs'] kafka: *kafka* database service type specific arguments.
@@ -257,15 +256,14 @@
         :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
                <TYPE>` - for reference).
         :param pulumi.Input['DatabaseRedisArgs'] redis: *redis* database service type specific arguments. Structure is documented below.
         :param pulumi.Input[str] state: The current state of the database service.
         :param pulumi.Input[bool] termination_protection: The database service protection boolean flag against termination/power-off.
         :param pulumi.Input[str] type: The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
         :param pulumi.Input[str] updated_at: The date of the latest database service update.
-        :param pulumi.Input[str] uri: The database service connection URI.
         :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if ca_certificate is not None:
             pulumi.set(__self__, "ca_certificate", ca_certificate)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if disk_size is not None:
@@ -298,16 +296,14 @@
             pulumi.set(__self__, "state", state)
         if termination_protection is not None:
             pulumi.set(__self__, "termination_protection", termination_protection)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if updated_at is not None:
             pulumi.set(__self__, "updated_at", updated_at)
-        if uri is not None:
-            pulumi.set(__self__, "uri", uri)
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="caCertificate")
     def ca_certificate(self) -> Optional[pulumi.Input[str]]:
         """
@@ -535,26 +531,14 @@
 
     @updated_at.setter
     def updated_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "updated_at", value)
 
     @property
     @pulumi.getter
-    def uri(self) -> Optional[pulumi.Input[str]]:
-        """
-        The database service connection URI.
-        """
-        return pulumi.get(self, "uri")
-
-    @uri.setter
-    def uri(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "uri", value)
-
-    @property
-    @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
         The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
@@ -687,17 +671,14 @@
             __props__.__dict__["created_at"] = None
             __props__.__dict__["disk_size"] = None
             __props__.__dict__["node_cpus"] = None
             __props__.__dict__["node_memory"] = None
             __props__.__dict__["nodes"] = None
             __props__.__dict__["state"] = None
             __props__.__dict__["updated_at"] = None
-            __props__.__dict__["uri"] = None
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["uri"])
-        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Database, __self__).__init__(
             'exoscale:index/database:Database',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -719,15 +700,14 @@
             pg: Optional[pulumi.Input[pulumi.InputType['DatabasePgArgs']]] = None,
             plan: Optional[pulumi.Input[str]] = None,
             redis: Optional[pulumi.Input[pulumi.InputType['DatabaseRedisArgs']]] = None,
             state: Optional[pulumi.Input[str]] = None,
             termination_protection: Optional[pulumi.Input[bool]] = None,
             type: Optional[pulumi.Input[str]] = None,
             updated_at: Optional[pulumi.Input[str]] = None,
-            uri: Optional[pulumi.Input[str]] = None,
             zone: Optional[pulumi.Input[str]] = None) -> 'Database':
         """
         Get an existing Database resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
@@ -749,15 +729,14 @@
         :param pulumi.Input[str] plan: The plan of the database service (use the [Exoscale CLI](https://github.com/exoscale/cli/) - `exo dbaas type show
                <TYPE>` - for reference).
         :param pulumi.Input[pulumi.InputType['DatabaseRedisArgs']] redis: *redis* database service type specific arguments. Structure is documented below.
         :param pulumi.Input[str] state: The current state of the database service.
         :param pulumi.Input[bool] termination_protection: The database service protection boolean flag against termination/power-off.
         :param pulumi.Input[str] type: The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
         :param pulumi.Input[str] updated_at: The date of the latest database service update.
-        :param pulumi.Input[str] uri: The database service connection URI.
         :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DatabaseState.__new__(_DatabaseState)
 
         __props__.__dict__["ca_certificate"] = ca_certificate
@@ -775,15 +754,14 @@
         __props__.__dict__["pg"] = pg
         __props__.__dict__["plan"] = plan
         __props__.__dict__["redis"] = redis
         __props__.__dict__["state"] = state
         __props__.__dict__["termination_protection"] = termination_protection
         __props__.__dict__["type"] = type
         __props__.__dict__["updated_at"] = updated_at
-        __props__.__dict__["uri"] = uri
         __props__.__dict__["zone"] = zone
         return Database(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="caCertificate")
     def ca_certificate(self) -> pulumi.Output[str]:
         """
@@ -935,21 +913,13 @@
         """
         The date of the latest database service update.
         """
         return pulumi.get(self, "updated_at")
 
     @property
     @pulumi.getter
-    def uri(self) -> pulumi.Output[str]:
-        """
-        The database service connection URI.
-        """
-        return pulumi.get(self, "uri")
-
-    @property
-    @pulumi.getter
     def zone(self) -> pulumi.Output[str]:
         """
         The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         return pulumi.get(self, "zone")
```

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/domain.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/domain.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/domain_record.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/elastic_ip.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/elastic_ip.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_affinity.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_affinity.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_anti_affinity_group.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_anti_affinity_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_instance.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_instance.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_instance_list.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_instance_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_ip_address.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_template.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_compute_template.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_domain.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_domain_record.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_elastic_ip.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_elastic_ip.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_instance_pool.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_instance_pool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_instance_pool_list.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_instance_pool_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_network.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_nlb.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_nlb.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_private_network.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_private_network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_security_group.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_security_group.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,23 +17,34 @@
 ]
 
 @pulumi.output_type
 class GetSecurityGroupResult:
     """
     A collection of values returned by getSecurityGroup.
     """
-    def __init__(__self__, id=None, name=None):
+    def __init__(__self__, external_sources=None, id=None, name=None):
+        if external_sources and not isinstance(external_sources, list):
+            raise TypeError("Expected argument 'external_sources' to be a list")
+        pulumi.set(__self__, "external_sources", external_sources)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
 
     @property
+    @pulumi.getter(name="externalSources")
+    def external_sources(self) -> Sequence[str]:
+        """
+        The list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
+        """
+        return pulumi.get(self, "external_sources")
+
+    @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         The security group ID to match (conflicts with `name`)
         """
         return pulumi.get(self, "id")
 
@@ -48,14 +59,15 @@
 
 class AwaitableGetSecurityGroupResult(GetSecurityGroupResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetSecurityGroupResult(
+            external_sources=self.external_sources,
             id=self.id,
             name=self.name)
 
 
 def get_security_group(id: Optional[str] = None,
                        name: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSecurityGroupResult:
@@ -68,14 +80,15 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getSecurityGroup:getSecurityGroup', __args__, opts=opts, typ=GetSecurityGroupResult).value
 
     return AwaitableGetSecurityGroupResult(
+        external_sources=__ret__.external_sources,
         id=__ret__.id,
         name=__ret__.name)
 
 
 @_utilities.lift_output_func(get_security_group)
 def get_security_group_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                               name: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_cluster.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,17 @@
         Enable automatic upgrading of the control plane version.
         """
         return pulumi.get(self, "auto_upgrade")
 
     @property
     @pulumi.getter
     def cni(self) -> Optional[str]:
+        """
+        The CNI plugin that is to be used. Defaults to "calico".
+        """
         return pulumi.get(self, "cni")
 
     @property
     @pulumi.getter(name="controlPlaneCa")
     def control_plane_ca(self) -> str:
         """
         The CA certificate (in PEM format) for TLS communications between control plane components.
@@ -288,14 +291,15 @@
                     zone: Optional[str] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSKSClusterResult:
     """
     Use this data source to access information about an existing resource.
 
     :param str aggregation_ca: The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g. `metrics-server`).
     :param bool auto_upgrade: Enable automatic upgrading of the control plane version.
+    :param str cni: The CNI plugin that is to be used. Defaults to "calico".
     :param str control_plane_ca: The CA certificate (in PEM format) for TLS communications between control plane components.
     :param str created_at: The cluster creation date.
     :param str description: A free-form text describing the cluster.
     :param str endpoint: The cluster API endpoint.
     :param bool exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
     :param str id: The ID of this resource.
     :param str kubelet_ca: The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
@@ -377,14 +381,15 @@
                            zone: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSKSClusterResult]:
     """
     Use this data source to access information about an existing resource.
 
     :param str aggregation_ca: The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g. `metrics-server`).
     :param bool auto_upgrade: Enable automatic upgrading of the control plane version.
+    :param str cni: The CNI plugin that is to be used. Defaults to "calico".
     :param str control_plane_ca: The CA certificate (in PEM format) for TLS communications between control plane components.
     :param str created_at: The cluster creation date.
     :param str description: A free-form text describing the cluster.
     :param str endpoint: The cluster API endpoint.
     :param bool exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
     :param str id: The ID of this resource.
     :param str kubelet_ca: The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
```

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_cluster_list.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_cluster_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_nodepool.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_nodepool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_nodepool_list.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_sks_nodepool_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_template.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/iam_access_key.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/iam_access_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/instance_pool.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/instance_pool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/ip_address.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/network.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/nic.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/nic.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/nlb.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/nlb.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/nlb_service.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/nlb_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/outputs.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/private_network.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/private_network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/provider.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,48 +10,48 @@
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
-                 dns_endpoint: pulumi.Input[str],
-                 timeout: pulumi.Input[int],
                  compute_endpoint: Optional[pulumi.Input[str]] = None,
                  config: Optional[pulumi.Input[str]] = None,
                  delay: Optional[pulumi.Input[int]] = None,
+                 dns_endpoint: Optional[pulumi.Input[str]] = None,
                  environment: Optional[pulumi.Input[str]] = None,
                  gzip_user_data: Optional[pulumi.Input[bool]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  profile: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
+                 timeout: Optional[pulumi.Input[int]] = None,
                  token: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
-        :param pulumi.Input[str] dns_endpoint: Exoscale DNS API endpoint (by default: https://api.exoscale.com/dns)
-        :param pulumi.Input[int] timeout: Timeout in seconds for waiting on compute resources to become available (by default: 300)
         :param pulumi.Input[str] compute_endpoint: Exoscale CloudStack API endpoint (by default: https://api.exoscale.com/v1)
         :param pulumi.Input[str] config: CloudStack ini configuration filename (by default: cloudstack.ini)
+        :param pulumi.Input[str] dns_endpoint: Exoscale DNS API endpoint (by default: https://api.exoscale.com/dns)
         :param pulumi.Input[bool] gzip_user_data: Defines if the user-data of compute instances should be gzipped (by default: true)
         :param pulumi.Input[str] key: Exoscale API key
         :param pulumi.Input[str] region: CloudStack ini configuration section name (by default: cloudstack)
         :param pulumi.Input[str] secret: Exoscale API secret
+        :param pulumi.Input[int] timeout: Timeout in seconds for waiting on compute resources to become available (by default: 300)
         """
-        pulumi.set(__self__, "dns_endpoint", dns_endpoint)
-        pulumi.set(__self__, "timeout", timeout)
         if compute_endpoint is not None:
             pulumi.set(__self__, "compute_endpoint", compute_endpoint)
         if config is not None:
             pulumi.set(__self__, "config", config)
         if delay is not None:
             warnings.warn("""Does nothing""", DeprecationWarning)
             pulumi.log.warn("""delay is deprecated: Does nothing""")
         if delay is not None:
             pulumi.set(__self__, "delay", delay)
+        if dns_endpoint is not None:
+            pulumi.set(__self__, "dns_endpoint", dns_endpoint)
         if environment is not None:
             pulumi.set(__self__, "environment", environment)
         if gzip_user_data is not None:
             pulumi.set(__self__, "gzip_user_data", gzip_user_data)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if profile is not None:
@@ -59,45 +59,23 @@
             pulumi.log.warn("""profile is deprecated: Use region instead""")
         if profile is not None:
             pulumi.set(__self__, "profile", profile)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if secret is not None:
             pulumi.set(__self__, "secret", secret)
+        if timeout is not None:
+            pulumi.set(__self__, "timeout", timeout)
         if token is not None:
             warnings.warn("""Use key instead""", DeprecationWarning)
             pulumi.log.warn("""token is deprecated: Use key instead""")
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
-    @pulumi.getter(name="dnsEndpoint")
-    def dns_endpoint(self) -> pulumi.Input[str]:
-        """
-        Exoscale DNS API endpoint (by default: https://api.exoscale.com/dns)
-        """
-        return pulumi.get(self, "dns_endpoint")
-
-    @dns_endpoint.setter
-    def dns_endpoint(self, value: pulumi.Input[str]):
-        pulumi.set(self, "dns_endpoint", value)
-
-    @property
-    @pulumi.getter
-    def timeout(self) -> pulumi.Input[int]:
-        """
-        Timeout in seconds for waiting on compute resources to become available (by default: 300)
-        """
-        return pulumi.get(self, "timeout")
-
-    @timeout.setter
-    def timeout(self, value: pulumi.Input[int]):
-        pulumi.set(self, "timeout", value)
-
-    @property
     @pulumi.getter(name="computeEndpoint")
     def compute_endpoint(self) -> Optional[pulumi.Input[str]]:
         """
         Exoscale CloudStack API endpoint (by default: https://api.exoscale.com/v1)
         """
         return pulumi.get(self, "compute_endpoint")
 
@@ -123,14 +101,26 @@
         return pulumi.get(self, "delay")
 
     @delay.setter
     def delay(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "delay", value)
 
     @property
+    @pulumi.getter(name="dnsEndpoint")
+    def dns_endpoint(self) -> Optional[pulumi.Input[str]]:
+        """
+        Exoscale DNS API endpoint (by default: https://api.exoscale.com/dns)
+        """
+        return pulumi.get(self, "dns_endpoint")
+
+    @dns_endpoint.setter
+    def dns_endpoint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "dns_endpoint", value)
+
+    @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "environment")
 
     @environment.setter
     def environment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "environment", value)
@@ -190,14 +180,26 @@
 
     @secret.setter
     def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
     @property
     @pulumi.getter
+    def timeout(self) -> Optional[pulumi.Input[int]]:
+        """
+        Timeout in seconds for waiting on compute resources to become available (by default: 300)
+        """
+        return pulumi.get(self, "timeout")
+
+    @timeout.setter
+    def timeout(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "timeout", value)
+
+    @property
+    @pulumi.getter
     def token(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "token", value)
 
@@ -237,15 +239,15 @@
         :param pulumi.Input[str] secret: Exoscale API secret
         :param pulumi.Input[int] timeout: Timeout in seconds for waiting on compute resources to become available (by default: 300)
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ProviderArgs,
+                 args: Optional[ProviderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The provider type for the exoscale package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
@@ -287,28 +289,24 @@
 
             __props__.__dict__["compute_endpoint"] = compute_endpoint
             __props__.__dict__["config"] = config
             if delay is not None and not opts.urn:
                 warnings.warn("""Does nothing""", DeprecationWarning)
                 pulumi.log.warn("""delay is deprecated: Does nothing""")
             __props__.__dict__["delay"] = pulumi.Output.from_input(delay).apply(pulumi.runtime.to_json) if delay is not None else None
-            if dns_endpoint is None and not opts.urn:
-                raise TypeError("Missing required property 'dns_endpoint'")
             __props__.__dict__["dns_endpoint"] = dns_endpoint
             __props__.__dict__["environment"] = environment
             __props__.__dict__["gzip_user_data"] = pulumi.Output.from_input(gzip_user_data).apply(pulumi.runtime.to_json) if gzip_user_data is not None else None
             __props__.__dict__["key"] = key
             if profile is not None and not opts.urn:
                 warnings.warn("""Use region instead""", DeprecationWarning)
                 pulumi.log.warn("""profile is deprecated: Use region instead""")
             __props__.__dict__["profile"] = profile
             __props__.__dict__["region"] = region
             __props__.__dict__["secret"] = None if secret is None else pulumi.Output.secret(secret)
-            if timeout is None and not opts.urn:
-                raise TypeError("Missing required property 'timeout'")
             __props__.__dict__["timeout"] = pulumi.Output.from_input(timeout).apply(pulumi.runtime.to_json) if timeout is not None else None
             if token is not None and not opts.urn:
                 warnings.warn("""Use key instead""", DeprecationWarning)
                 pulumi.log.warn("""token is deprecated: Use key instead""")
             __props__.__dict__["token"] = token
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["secret"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
@@ -332,15 +330,15 @@
         """
         CloudStack ini configuration filename (by default: cloudstack.ini)
         """
         return pulumi.get(self, "config")
 
     @property
     @pulumi.getter(name="dnsEndpoint")
-    def dns_endpoint(self) -> pulumi.Output[str]:
+    def dns_endpoint(self) -> pulumi.Output[Optional[str]]:
         """
         Exoscale DNS API endpoint (by default: https://api.exoscale.com/dns)
         """
         return pulumi.get(self, "dns_endpoint")
 
     @property
     @pulumi.getter
```

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/secondary_ip_address.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/secondary_ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/security_group.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/security_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/security_group_rule.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/security_group_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/security_group_rules.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/security_group_rules.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/sks_cluster.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/sks_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
                  oidc: Optional[pulumi.Input['SKSClusterOidcArgs']] = None,
                  service_level: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SKSCluster resource.
         :param pulumi.Input[str] zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
+        :param pulumi.Input[str] cni: The CNI plugin that is to be used. Defaults to "calico".
         :param pulumi.Input[str] description: A free-form text describing the cluster.
         :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
                control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
                (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
@@ -104,14 +105,17 @@
     @auto_upgrade.setter
     def auto_upgrade(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "auto_upgrade", value)
 
     @property
     @pulumi.getter
     def cni(self) -> Optional[pulumi.Input[str]]:
+        """
+        The CNI plugin that is to be used. Defaults to "calico".
+        """
         return pulumi.get(self, "cni")
 
     @cni.setter
     def cni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cni", value)
 
     @property
@@ -238,14 +242,15 @@
                  version: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SKSCluster resources.
         :param pulumi.Input[str] aggregation_ca: The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g.
                `metrics-server`).
         :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
+        :param pulumi.Input[str] cni: The CNI plugin that is to be used. Defaults to "calico".
         :param pulumi.Input[str] control_plane_ca: The CA certificate (in PEM format) for TLS communications between control plane components.
         :param pulumi.Input[str] created_at: The cluster creation date.
         :param pulumi.Input[str] description: A free-form text describing the cluster.
         :param pulumi.Input[str] endpoint: The cluster API endpoint.
         :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
                control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] kubelet_ca: The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
@@ -337,14 +342,17 @@
     @auto_upgrade.setter
     def auto_upgrade(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "auto_upgrade", value)
 
     @property
     @pulumi.getter
     def cni(self) -> Optional[pulumi.Input[str]]:
+        """
+        The CNI plugin that is to be used. Defaults to "calico".
+        """
         return pulumi.get(self, "cni")
 
     @cni.setter
     def cni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cni", value)
 
     @property
@@ -562,14 +570,15 @@
          exoscale_sks_cluster.my_sks_cluster \\
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
+        :param pulumi.Input[str] cni: The CNI plugin that is to be used. Defaults to "calico".
         :param pulumi.Input[str] description: A free-form text describing the cluster.
         :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
                control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane
                (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
@@ -694,14 +703,15 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] aggregation_ca: The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g.
                `metrics-server`).
         :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
+        :param pulumi.Input[str] cni: The CNI plugin that is to be used. Defaults to "calico".
         :param pulumi.Input[str] control_plane_ca: The CA certificate (in PEM format) for TLS communications between control plane components.
         :param pulumi.Input[str] created_at: The cluster creation date.
         :param pulumi.Input[str] description: A free-form text describing the cluster.
         :param pulumi.Input[str] endpoint: The cluster API endpoint.
         :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the
                control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] kubelet_ca: The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
@@ -764,14 +774,17 @@
         Enable automatic upgrading of the control plane version.
         """
         return pulumi.get(self, "auto_upgrade")
 
     @property
     @pulumi.getter
     def cni(self) -> pulumi.Output[Optional[str]]:
+        """
+        The CNI plugin that is to be used. Defaults to "calico".
+        """
         return pulumi.get(self, "cni")
 
     @property
     @pulumi.getter(name="controlPlaneCa")
     def control_plane_ca(self) -> pulumi.Output[str]:
         """
         The CA certificate (in PEM format) for TLS communications between control plane components.
```

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/sks_kubeconfig.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/sks_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/sks_nodepool.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/sks_nodepool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/ssh_key.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/ssh_keypair.py` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale/ssh_keypair.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/PKG-INFO` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-exoscale
-Version: 0.48.0
+Version: 0.49.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/SOURCES.txt` & `pulumiverse_exoscale-0.49.0/pulumiverse_exoscale.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 pulumiverse_exoscale/get_affinity.py
 pulumiverse_exoscale/get_anti_affinity_group.py
 pulumiverse_exoscale/get_compute.py
 pulumiverse_exoscale/get_compute_instance.py
 pulumiverse_exoscale/get_compute_instance_list.py
 pulumiverse_exoscale/get_compute_ip_address.py
 pulumiverse_exoscale/get_compute_template.py
+pulumiverse_exoscale/get_database_uri.py
 pulumiverse_exoscale/get_domain.py
 pulumiverse_exoscale/get_domain_record.py
 pulumiverse_exoscale/get_elastic_ip.py
 pulumiverse_exoscale/get_instance_pool.py
 pulumiverse_exoscale/get_instance_pool_list.py
 pulumiverse_exoscale/get_network.py
 pulumiverse_exoscale/get_nlb.py
```

### Comparing `pulumiverse_exoscale-0.48.0/setup.py` & `pulumiverse_exoscale-0.49.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.48.0"
-PLUGIN_VERSION = "0.48.0"
+VERSION = "0.49.0"
+PLUGIN_VERSION = "0.49.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'exoscale', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-exoscale'])
         except OSError as error:
```

