# Comparing `tmp/genv-0.9.0.tar.gz` & `tmp/genv-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genv-0.9.0.tar", last modified: Mon May  1 06:07:49 2023, max compression
+gzip compressed data, was "genv-1.0.0.tar", last modified: Mon Jun 12 08:06:42 2023, max compression
```

## Comparing `genv-0.9.0.tar` & `genv-1.0.0.tar`

### file list

```diff
@@ -1,61 +1,121 @@
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.421188 genv-0.9.0/
--rw-r--r--   0 raz       (1001) raz       (1001)     4737 2023-05-01 06:07:49.421188 genv-0.9.0/PKG-INFO
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.417188 genv-0.9.0/genv/
--rw-r--r--   0 raz       (1001) raz       (1001)      268 2023-04-30 14:04:42.000000 genv-0.9.0/genv/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     8607 2023-04-30 14:04:42.000000 genv-0.9.0/genv/devices.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.418188 genv-0.9.0/genv/enforce/
--rw-r--r--   0 raz       (1001) raz       (1001)      103 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1311 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/execute.py
--rw-r--r--   0 raz       (1001) raz       (1001)      298 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/report.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.418188 genv-0.9.0/genv/enforce/rules/
--rw-r--r--   0 raz       (1001) raz       (1001)      176 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/rules/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      851 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/rules/env_devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1379 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/rules/env_memory.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1342 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/rules/max_devices_per_user.py
--rw-r--r--   0 raz       (1001) raz       (1001)      629 2023-04-13 08:09:45.000000 genv-0.9.0/genv/enforce/rules/non_env_processes.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1136 2023-02-19 16:28:43.000000 genv-0.9.0/genv/enforce/survey.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.418188 genv-0.9.0/genv/env/
--rw-r--r--   0 raz       (1001) raz       (1001)      227 2023-04-30 14:04:42.000000 genv-0.9.0/genv/env/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      995 2023-04-30 14:04:42.000000 genv-0.9.0/genv/env/devices.py
--rw-r--r--   0 raz       (1001) raz       (1001)     6009 2023-04-13 08:09:45.000000 genv-0.9.0/genv/envs.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1348 2023-04-30 14:04:42.000000 genv-0.9.0/genv/json_.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.419188 genv-0.9.0/genv/metrics/
--rw-r--r--   0 raz       (1001) raz       (1001)      184 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3109 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/collection.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1797 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/metric.py
--rw-r--r--   0 raz       (1001) raz       (1001)     2663 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/publisher.py
--rw-r--r--   0 raz       (1001) raz       (1001)      443 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/spec.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3605 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/specs.py
--rw-r--r--   0 raz       (1001) raz       (1001)      157 2023-04-04 06:42:45.000000 genv-0.9.0/genv/metrics/type.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1438 2023-04-04 06:42:45.000000 genv-0.9.0/genv/nvidia_smi.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4311 2023-04-30 14:04:44.000000 genv-0.9.0/genv/os_.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1253 2023-04-17 10:27:35.000000 genv-0.9.0/genv/poll.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4347 2023-04-03 12:05:14.000000 genv-0.9.0/genv/processes.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.420188 genv-0.9.0/genv/remote/
--rw-r--r--   0 raz       (1001) raz       (1001)      162 2023-03-30 12:58:17.000000 genv-0.9.0/genv/remote/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      379 2023-02-19 16:28:43.000000 genv-0.9.0/genv/remote/devices.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.420188 genv-0.9.0/genv/remote/enforce/
--rw-r--r--   0 raz       (1001) raz       (1001)       29 2023-02-13 23:02:53.000000 genv-0.9.0/genv/remote/enforce/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      640 2023-02-19 16:28:43.000000 genv-0.9.0/genv/remote/enforce/execute.py
--rw-r--r--   0 raz       (1001) raz       (1001)      378 2023-02-19 16:28:43.000000 genv-0.9.0/genv/remote/envs.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.420188 genv-0.9.0/genv/remote/metrics/
--rw-r--r--   0 raz       (1001) raz       (1001)       35 2023-04-04 06:42:45.000000 genv-0.9.0/genv/remote/metrics/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1730 2023-04-04 06:42:45.000000 genv-0.9.0/genv/remote/metrics/collection.py
--rw-r--r--   0 raz       (1001) raz       (1001)      383 2023-02-19 16:28:43.000000 genv-0.9.0/genv/remote/processes.py
--rw-r--r--   0 raz       (1001) raz       (1001)      825 2023-03-30 12:58:17.000000 genv-0.9.0/genv/remote/snapshot.py
--rw-r--r--   0 raz       (1001) raz       (1001)     3179 2023-04-04 06:42:45.000000 genv-0.9.0/genv/remote/ssh.py
--rw-r--r--   0 raz       (1001) raz       (1001)      515 2023-02-19 16:28:43.000000 genv-0.9.0/genv/remote/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.421188 genv-0.9.0/genv/runners/
--rw-r--r--   0 raz       (1001) raz       (1001)       59 2023-04-04 06:42:45.000000 genv-0.9.0/genv/runners/__init__.py
--rw-r--r--   0 raz       (1001) raz       (1001)      687 2023-04-04 06:42:45.000000 genv-0.9.0/genv/runners/local.py
--rw-r--r--   0 raz       (1001) raz       (1001)     2046 2023-04-04 06:42:45.000000 genv-0.9.0/genv/runners/runner.py
--rw-r--r--   0 raz       (1001) raz       (1001)     2425 2023-04-04 06:42:45.000000 genv-0.9.0/genv/runners/ssh.py
--rw-r--r--   0 raz       (1001) raz       (1001)     1499 2023-04-04 06:42:45.000000 genv-0.9.0/genv/snapshot.py
--rw-r--r--   0 raz       (1001) raz       (1001)     4069 2023-04-30 14:04:42.000000 genv-0.9.0/genv/utils.py
-drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-05-01 06:07:49.417188 genv-0.9.0/genv.egg-info/
--rw-r--r--   0 raz       (1001) raz       (1001)     4737 2023-05-01 06:07:49.000000 genv-0.9.0/genv.egg-info/PKG-INFO
--rw-r--r--   0 raz       (1001) raz       (1001)     1130 2023-05-01 06:07:49.000000 genv-0.9.0/genv.egg-info/SOURCES.txt
--rw-r--r--   0 raz       (1001) raz       (1001)        1 2023-05-01 06:07:49.000000 genv-0.9.0/genv.egg-info/dependency_links.txt
--rw-r--r--   0 raz       (1001) raz       (1001)        5 2023-05-01 06:07:49.000000 genv-0.9.0/genv.egg-info/top_level.txt
--rw-r--r--   0 raz       (1001) raz       (1001)       38 2023-05-01 06:07:49.421188 genv-0.9.0/setup.cfg
--rw-r--r--   0 raz       (1001) raz       (1001)      622 2023-05-01 06:01:25.000000 genv-0.9.0/setup.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.061021 genv-1.0.0/
+-rw-r--r--   0 raz       (1001) raz       (1001)    34523 2022-12-27 17:45:39.000000 genv-1.0.0/LICENSE
+-rw-r--r--   0 raz       (1001) raz       (1001)     4060 2023-06-12 08:06:42.061021 genv-1.0.0/PKG-INFO
+-rw-r--r--   0 raz       (1001) raz       (1001)     3394 2023-06-12 08:06:16.000000 genv-1.0.0/README.md
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.052021 genv-1.0.0/genv/
+-rw-r--r--   0 raz       (1001) raz       (1001)      306 2023-06-12 07:39:27.000000 genv-1.0.0/genv/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.054021 genv-1.0.0/genv/cli/
+-rw-r--r--   0 raz       (1001) raz       (1001)        0 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5007 2023-06-12 08:06:16.000000 genv-1.0.0/genv/cli/__main__.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     2755 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/activate.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     1358 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/attach.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     2295 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/config.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)      738 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/deactivate.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)      465 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/detach.py
+-rw-r--r--   0 raz       (1001) raz       (1001)    10817 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     2565 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/enforce.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     9382 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/envs.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)      656 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/home.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)      610 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/lock.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     1945 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/monitor.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)    15306 2023-06-12 08:06:16.000000 genv-1.0.0/genv/cli/remote.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5133 2023-06-12 08:06:16.000000 genv-1.0.0/genv/cli/shell.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      892 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/status.py
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     1986 2023-06-12 07:39:27.000000 genv-1.0.0/genv/cli/usage.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.055021 genv-1.0.0/genv/core/
+-rw-r--r--   0 raz       (1001) raz       (1001)      116 2023-06-12 07:39:27.000000 genv-1.0.0/genv/core/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5677 2023-06-12 07:39:27.000000 genv-1.0.0/genv/core/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3703 2023-06-12 07:39:27.000000 genv-1.0.0/genv/core/envs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      894 2023-06-12 07:39:27.000000 genv-1.0.0/genv/core/processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      379 2023-06-12 07:39:27.000000 genv-1.0.0/genv/core/snapshot.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1424 2023-06-12 07:39:27.000000 genv-1.0.0/genv/core/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.056021 genv-1.0.0/genv/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)       49 2023-06-12 07:39:27.000000 genv-1.0.0/genv/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1288 2023-06-12 07:39:27.000000 genv-1.0.0/genv/enforce/execute.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.056021 genv-1.0.0/genv/enforce/rules/
+-rw-r--r--   0 raz       (1001) raz       (1001)      176 2023-06-12 07:39:27.000000 genv-1.0.0/genv/enforce/rules/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      864 2023-06-12 07:39:27.000000 genv-1.0.0/genv/enforce/rules/env_devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1394 2023-06-12 07:39:27.000000 genv-1.0.0/genv/enforce/rules/env_memory.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1355 2023-06-12 07:39:27.000000 genv-1.0.0/genv/enforce/rules/max_devices_per_user.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      642 2023-06-12 07:39:27.000000 genv-1.0.0/genv/enforce/rules/non_env_processes.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.056021 genv-1.0.0/genv/entities/
+-rw-r--r--   0 raz       (1001) raz       (1001)      111 2023-06-12 07:39:27.000000 genv-1.0.0/genv/entities/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.057021 genv-1.0.0/genv/entities/core/
+-rw-r--r--   0 raz       (1001) raz       (1001)      138 2023-06-12 07:39:27.000000 genv-1.0.0/genv/entities/core/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     7231 2023-06-12 07:39:27.000000 genv-1.0.0/genv/entities/core/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     5875 2023-06-12 07:39:27.000000 genv-1.0.0/genv/entities/core/envs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3484 2023-06-12 07:39:27.000000 genv-1.0.0/genv/entities/core/processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      982 2023-06-12 07:39:27.000000 genv-1.0.0/genv/entities/core/snapshot.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.057021 genv-1.0.0/genv/entities/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)       54 2023-06-12 07:39:27.000000 genv-1.0.0/genv/entities/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      270 2023-06-12 07:39:27.000000 genv-1.0.0/genv/entities/enforce/report.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1126 2023-06-12 07:39:27.000000 genv-1.0.0/genv/entities/enforce/survey.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.057021 genv-1.0.0/genv/metrics/
+-rw-r--r--   0 raz       (1001) raz       (1001)      184 2023-06-12 07:39:27.000000 genv-1.0.0/genv/metrics/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3074 2023-06-12 07:39:27.000000 genv-1.0.0/genv/metrics/collection.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.051021 genv-1.0.0/genv/metrics/export/
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.058021 genv-1.0.0/genv/metrics/export/grafana/
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.058021 genv-1.0.0/genv/metrics/export/grafana/dashboards/
+-rw-r--r--   0 raz       (1001) raz       (1001)     9965 2023-06-12 07:39:27.000000 genv-1.0.0/genv/metrics/export/grafana/dashboards/overview.json
+-rw-r--r--   0 raz       (1001) raz       (1001)      182 2023-06-12 07:39:27.000000 genv-1.0.0/genv/metrics/export/grafana/grafana.ini
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.051021 genv-1.0.0/genv/metrics/export/grafana/provisioning/
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.058021 genv-1.0.0/genv/metrics/export/grafana/provisioning/dashboards/
+-rw-r--r--   0 raz       (1001) raz       (1001)      114 2023-06-12 07:39:27.000000 genv-1.0.0/genv/metrics/export/grafana/provisioning/dashboards/default.yml
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.058021 genv-1.0.0/genv/metrics/export/grafana/provisioning/datasources/
+-rw-r--r--   0 raz       (1001) raz       (1001)      134 2023-06-12 07:39:27.000000 genv-1.0.0/genv/metrics/export/grafana/provisioning/datasources/default.yml
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.058021 genv-1.0.0/genv/metrics/export/prometheus/
+-rw-r--r--   0 raz       (1001) raz       (1001)      155 2023-06-12 07:39:27.000000 genv-1.0.0/genv/metrics/export/prometheus/prometheus.yml
+-rw-r--r--   0 raz       (1001) raz       (1001)     1786 2023-06-12 07:39:27.000000 genv-1.0.0/genv/metrics/metric.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     2663 2023-06-12 07:39:27.000000 genv-1.0.0/genv/metrics/publisher.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      431 2023-06-12 07:39:27.000000 genv-1.0.0/genv/metrics/spec.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3593 2023-06-12 07:39:27.000000 genv-1.0.0/genv/metrics/specs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      157 2023-06-12 07:39:27.000000 genv-1.0.0/genv/metrics/type.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.058021 genv-1.0.0/genv/remote/
+-rw-r--r--   0 raz       (1001) raz       (1001)       87 2023-06-12 07:39:27.000000 genv-1.0.0/genv/remote/__init__.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.058021 genv-1.0.0/genv/remote/core/
+-rw-r--r--   0 raz       (1001) raz       (1001)       96 2023-06-12 07:39:27.000000 genv-1.0.0/genv/remote/core/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      381 2023-06-12 07:39:27.000000 genv-1.0.0/genv/remote/core/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      377 2023-06-12 07:39:27.000000 genv-1.0.0/genv/remote/core/envs.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      387 2023-06-12 07:39:27.000000 genv-1.0.0/genv/remote/core/processes.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      834 2023-06-12 07:39:27.000000 genv-1.0.0/genv/remote/core/snapshot.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.059021 genv-1.0.0/genv/remote/enforce/
+-rw-r--r--   0 raz       (1001) raz       (1001)       29 2023-06-12 07:39:27.000000 genv-1.0.0/genv/remote/enforce/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      637 2023-06-12 07:39:27.000000 genv-1.0.0/genv/remote/enforce/execute.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.059021 genv-1.0.0/genv/remote/metrics/
+-rw-r--r--   0 raz       (1001) raz       (1001)       35 2023-06-12 07:39:27.000000 genv-1.0.0/genv/remote/metrics/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1683 2023-06-12 07:39:27.000000 genv-1.0.0/genv/remote/metrics/collection.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.059021 genv-1.0.0/genv/remote/utils/
+-rw-r--r--   0 raz       (1001) raz       (1001)       40 2023-06-12 07:39:27.000000 genv-1.0.0/genv/remote/utils/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3110 2023-06-12 07:39:27.000000 genv-1.0.0/genv/remote/utils/ssh.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      515 2023-06-12 07:39:27.000000 genv-1.0.0/genv/remote/utils/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.059021 genv-1.0.0/genv/sdk/
+-rw-r--r--   0 raz       (1001) raz       (1001)      272 2023-06-12 07:39:27.000000 genv-1.0.0/genv/sdk/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4132 2023-06-12 08:06:16.000000 genv-1.0.0/genv/sdk/devices.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     4280 2023-06-12 08:06:16.000000 genv-1.0.0/genv/sdk/env.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1300 2023-06-12 07:39:27.000000 genv-1.0.0/genv/sdk/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.060021 genv-1.0.0/genv/serialization/
+-rw-r--r--   0 raz       (1001) raz       (1001)       44 2023-06-12 07:39:27.000000 genv-1.0.0/genv/serialization/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1803 2023-06-12 07:39:27.000000 genv-1.0.0/genv/serialization/json_.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.060021 genv-1.0.0/genv/shims/
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     2750 2023-06-10 15:50:03.000000 genv-1.0.0/genv/shims/docker
+-rwxr-xr-x   0 raz       (1001) raz       (1001)     7030 2023-05-07 09:36:08.000000 genv-1.0.0/genv/shims/nvidia-smi
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.060021 genv-1.0.0/genv/utils/
+-rw-r--r--   0 raz       (1001) raz       (1001)      107 2023-06-12 07:39:27.000000 genv-1.0.0/genv/utils/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1393 2023-06-12 07:39:27.000000 genv-1.0.0/genv/utils/nvidia_smi.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3144 2023-06-12 08:06:16.000000 genv-1.0.0/genv/utils/os_.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     1253 2023-06-12 07:39:27.000000 genv-1.0.0/genv/utils/poll.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.061021 genv-1.0.0/genv/utils/runners/
+-rw-r--r--   0 raz       (1001) raz       (1001)       93 2023-06-12 07:39:27.000000 genv-1.0.0/genv/utils/runners/__init__.py
+-rw-r--r--   0 raz       (1001) raz       (1001)      688 2023-06-12 07:39:27.000000 genv-1.0.0/genv/utils/runners/local.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     2046 2023-06-12 07:39:27.000000 genv-1.0.0/genv/utils/runners/runner.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     2113 2023-06-12 07:39:27.000000 genv-1.0.0/genv/utils/runners/ssh.py
+-rw-r--r--   0 raz       (1001) raz       (1001)     3446 2023-06-12 07:39:27.000000 genv-1.0.0/genv/utils/utils.py
+drwxr-xr-x   0 raz       (1001) raz       (1001)        0 2023-06-12 08:06:42.053021 genv-1.0.0/genv.egg-info/
+-rw-r--r--   0 raz       (1001) raz       (1001)     4060 2023-06-12 08:06:41.000000 genv-1.0.0/genv.egg-info/PKG-INFO
+-rw-r--r--   0 raz       (1001) raz       (1001)     2373 2023-06-12 08:06:42.000000 genv-1.0.0/genv.egg-info/SOURCES.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)        1 2023-06-12 08:06:41.000000 genv-1.0.0/genv.egg-info/dependency_links.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)       48 2023-06-12 08:06:41.000000 genv-1.0.0/genv.egg-info/entry_points.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)       29 2023-06-12 08:06:41.000000 genv-1.0.0/genv.egg-info/requires.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)        5 2023-06-12 08:06:41.000000 genv-1.0.0/genv.egg-info/top_level.txt
+-rw-r--r--   0 raz       (1001) raz       (1001)       38 2023-06-12 08:06:42.061021 genv-1.0.0/setup.cfg
+-rw-r--r--   0 raz       (1001) raz       (1001)     1079 2023-06-12 08:00:56.000000 genv-1.0.0/setup.py
```

### Comparing `genv-0.9.0/PKG-INFO` & `genv-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 Metadata-Version: 2.1
 Name: genv
-Version: 0.9.0
-Summary: GPU Environment Management
+Version: 1.0.0
+Summary: GPU environment and cluster management
 Home-page: https://github.com/run-ai/genv
-Author: Run:AI
+Author: Run.ai
 Author-email: pypi@run.ai
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: GPU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: Terminals
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: monitor
+License-File: LICENSE
 
 <p align="center">
   <img src="images/genv blade landscape black@4x.png#gh-light-mode-only" width="600" alt="genv"/>
   <img src="images/genv blade landscape white@4x.png#gh-dark-mode-only" width="600" alt="genv"/>
 </p>
 
 # Genv (GPU Environment Management) [![Join the community at (https://discord.gg/zN3Q9pQAuT)](https://img.shields.io/badge/Discord-genv-7289da?logo=discord)](https://discord.gg/zN3Q9pQAuT)
@@ -73,37 +81,7 @@
 
 
 ## License
 The Genv software is Copyright 2022 [Run.ai Labs, Ltd.].
 The software is licensed by Run.ai under the AGPLv3 license.
 Please note that Run.ai’s intention in licensing the software are that the obligations of licensee pursuant to the AGPLv3 license should be interpreted broadly.
 For example, Run.ai’s intention is that the terms “work based on the Program” in Section 0 of the AGPLv3 license, and “Corresponding Source” in Section 1 of the AGPLv3 license, should be interpreted as broadly as possible to the extent permitted under applicable law.
-
-Genv Remote vs. Run.ai
-----------------------
-1. containers vs environments
-2. SSH vs k8s
-3. interception- vs monitoring-based enfircements
-4. non-centralized (no load balancing)
-5. no advanced user roles (everyone can list envs and devices)
-6. shim-based visualization vs. interception-based virtualization
-7. environment must fit in a node vs. multi-node workload
-8. no compute mgmt
-
-
-QUOTA:
------
-system:
-    [V] (nvidia-smi)      non env processes
-    [V] (nvidia-smi)      processes from envs on non-attached devices
-    [ ] (envs.json)       timeout
-
-resources:
-    [V] (devices.json)    num of attached devices
-
-    (later...)
-    [ ] (nvidia-smi)      num of processes (as an alternative to compute mgmt)
-    [ ] (envs.json)       num of active envs
-    [ ] (envs.json)       num of machines with active envs
-    [ ] (nvidia-smi)      amount of GPU memory (per device/total)
-
-https://grafana.com/docs/grafana/latest/cli/#override-homepath-value
```

### Comparing `genv-0.9.0/genv/devices.py` & `genv-1.0.0/genv/entities/core/devices.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,12 @@
-from contextlib import contextmanager
 from dataclasses import dataclass
 from datetime import datetime
-import subprocess
 from typing import Callable, Iterable, Optional, Union
 
-from genv.os_ import access_lock, create_lock
-from genv.utils import get_temp_file_path, memory_to_bytes, DATETIME_FMT
-
-# NOTE(raz): This should be the layer that queries and controls the state of Genv regarding devices.
-# Currently, it relies on executing the device manager executable of Genv, as this is where the logic is implemented.
-# This however should be done oppositely.
-# The entire logic that queries and controls devices.json should be implemented here, and the device manager executable
-# should use methods from here.
-# It should take the Genv lock for the atomicity of the transaction, and print output as needed.
-# The current architecture has an inherent potential deadlock because each manager locks a different lock, and might
-# call the other manager.
+from genv.utils import DATETIME_FMT, memory_to_bytes
 
 
 @dataclass
 class Device:
     @dataclass
     class Attachement:
         eid: str
@@ -95,17 +83,17 @@
         """
         for index, attachment in enumerate(self.attachments):
             if attachment.eid == eid:
                 del self.attachments[index]
 
 
 @dataclass
-class Snapshot:
+class Devices:
     """
-    A snapshot of devices.
+    A collection of devices.
     """
 
     devices: Iterable[Device]
 
     @property
     def indices(self) -> Iterable[int]:
         return [device.index for device in self.devices]
@@ -115,27 +103,30 @@
 
     def __len__(self):
         return self.devices.__len__()
 
     def __getitem__(self, index: int) -> Device:
         return next(device for device in self.devices if device.index == index)
 
+    def __contains__(self, index: int) -> bool:
+        return index in self.indices
+
     def filter(
         self,
         deep: bool = True,
         *,
         indices: Optional[Iterable[int]] = None,
         not_indices: Optional[Iterable[int]] = None,
         eid: Optional[str] = None,
         eids: Optional[Iterable[str]] = None,
         attached: Optional[bool] = None,
         function: Optional[Callable[[Device], bool]] = None,
     ):
         """
-        Returns a new filtered snapshot.
+        Returns a new filtered collection.
 
         :param deep: Perform deep filtering
         :param indices: Device indices to keep
         :param not_indices: Device indices to remove
         :param eid: Environment identifier to keep
         :param eids: Environment identifiers to keep
         :param attached: Keep only devices with environments attached or not
@@ -173,15 +164,15 @@
                 devices = [device for device in devices if device.attached]
             else:
                 devices = [device for device in devices if device.detached]
 
         if function is not None:
             devices = [device for device in devices if function(device)]
 
-        return Snapshot(devices)
+        return Devices(devices)
 
     def attach(
         self, eid: str, indices: Union[Iterable[int], int], gpu_memory: Optional[str]
     ) -> None:
         """
         Attaches devices to an environment.
         """
@@ -190,107 +181,62 @@
             indices = [indices]
 
         time = datetime.now().strftime(DATETIME_FMT)
 
         for index in indices:
             self.devices[index].attach(eid, gpu_memory, time)
 
+    def detach(self, eid: str, index: Optional[int] = None) -> None:
+        """Detaches an environment"""
 
-def snapshot() -> Snapshot:
-    """
-    Returns a devices snapshot.
-    """
+        if index is not None:
+            self.devices[index].detach(eid)
+        else:
+            for device in self.devices:
+                device.detach(eid)
 
-    lines = (
-        subprocess.check_output(
-            "genv exec devices query --query index total_memory attachments", shell=True
-        )
-        .decode("utf-8")
-        .strip()
-        .splitlines()
-    )
-
-    def parse_attachment(s: str) -> Device.Attachement:
-        eid, gpu_memory, time = s.split("+")
-
-        return Device.Attachement(
-            eid,
-            gpu_memory or None,
-            time.replace("_", " "),
-        )
-
-    def parse_device(s: str) -> Device:
-        index, total_memory, attachments = s.split(",")
-
-        return Device(
-            int(index),
-            total_memory,
-            [parse_attachment(attachment) for attachment in attachments.split(" ")]
-            if attachments
-            else [],
-        )
-
-    return Snapshot([parse_device(line) for line in lines])
+    def cleanup(
+        self,
+        *,
+        poll_eid: Optional[Callable[[str], bool]] = None,
+    ):
+        """
+        Cleans up the collection in place.
+        """
+        for device in self.devices:
+            for eid in device.eids:
+                if (poll_eid is not None) and (not poll_eid(eid)):
+                    device.detach(eid)
 
+    def find_available_devices(
+        self, count: int, gpu_memory: Optional[str], allow_over_subscription: bool
+    ) -> Iterable[int]:
+        """
+        Finds available devices with respect to the optionally specified memory request.
+        When thare are not enough devices available, non available devices are also used if
+        over-subscription is allowed. Otherwise, RuntimeError is raised.
 
-def attach(eid: str) -> Iterable[int]:
-    """
-    Attaches an environment to devices.
+        :param count: Amount of devices to find
+        :param gpu_memory: Optional memory request
+        :param allow_over_subscription: Use non available devices if needed
 
-    :param eid: Environment identifier
-    :return: Attached device indices
-    """
-    output = (
-        subprocess.check_output(
-            f"genv exec devices attach --eid {eid}",
-            shell=True,
+        :return: A list of device indices
+        """
+        available_devices = self.filter(
+            function=lambda device: device.available(gpu_memory)
         )
-        .decode("utf-8")
-        .strip()
-    )
 
-    return [int(index) for index in output.split(",") if index]
+        indices = available_devices.indices
 
+        if allow_over_subscription and len(indices) < count:
+            not_available_devices = self.filter(not_indices=available_devices.indices)
 
-def detach(eid: str, index: int) -> None:
-    """
-    Detaches an environment from a device.
-
-    :param eid: Environment identifier
-    :param index: Device index
-    :return: None
-    """
-    # TODO(raz): support detaching from multiple devices at the same time
-    subprocess.check_call(
-        f"genv exec devices detach --quiet --eid {eid} --index {index}", shell=True
-    )
-
-
-def get_lock_path(index: int, create: bool = False) -> str:
-    """
-    Returns the path of a device lock file.
-    Creates the file if requested and it does not exist.
-    """
-
-    path = get_temp_file_path(f"devices/{index}.lock")
-
-    if create:
-        create_lock(path)
-
-    return path
-
+            # we sort in order to use the least populated devices first
+            indices += sorted(
+                not_available_devices.indices,
+                key=lambda index: len(self[index].eids),
+            )
 
-@contextmanager
-def lock(index: int) -> None:
-    """
-    Obtain exclusive access to a device.
-    """
-    path = get_lock_path(index)
+        if len(indices) < count:
+            raise RuntimeError("No available devices")
 
-    # NOTE(raz): currently, we wait on the lock even if it is already taken by our environment.
-    # we should think if this is the desired behavior and if it's possible to lock once per environment.
-    with access_lock(path):
-        yield
-
-    # TODO(raz): currently we wait for the entire device to become available.
-    # we should support fractional usage and allow multiple environments to
-    # access the device if the sum of their memory capacity fits.
+        return indices[:count]
```

### Comparing `genv-0.9.0/genv/enforce/execute.py` & `genv-1.0.0/genv/enforce/execute.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 import sys
 from typing import Dict
 
-from .. import os_
-from .. import devices
-from .. import envs
-from .. import processes
+import genv.utils
+from genv.entities import Envs, Processes, Report
+import genv.core.devices
 
-from .report import Report
 
-
-def _terminate(processes: processes.Snapshot) -> None:
+def _terminate(processes: Processes) -> None:
     for process in processes:
         try:
             print(
                 f"Terminating process {process.pid} from environment {process.eid or 'N/A'} that is running on GPU(s) {','.join([str(index) for index in process.indices])}"
             )
 
-            os_.terminate(process.pid)
+            genv.utils.terminate(process.pid)
         except PermissionError:
             print(
                 f"[ERROR] Not enough permissions to terminate process {process.pid}",
                 file=sys.stderr,
             )
         except ProcessLookupError:
             print(f"[DEBUG] Process {process.pid} already terminated", file=sys.stderr)
 
 
-def _detach(envs: Dict[int, envs.Snapshot]) -> None:
+def _detach(envs: Dict[int, Envs]) -> None:
     for index, envs in envs.items():
         for env in envs:
             print(
                 f"Detaching environment {env.eid} of user {env.username or 'N/A'} from device {index}"
             )
 
-            devices.detach(env.eid, index)
+            genv.core.devices.detach(env.eid, index)
 
 
 def execute(report: Report) -> None:
     """
     Terminates processes and detaches environments from devices according to the given report.
     """
     _terminate(report.terminate)
```

### Comparing `genv-0.9.0/genv/enforce/rules/env_devices.py` & `genv-1.0.0/genv/enforce/rules/env_devices.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..survey import Survey
+from genv.entities.enforce import Survey
 
 
 def env_devices(*surveys: Survey) -> None:
     """
     Terminates processes on devices not attached to their environments.
     """
     for survey in surveys:
```

### Comparing `genv-0.9.0/genv/enforce/rules/env_memory.py` & `genv-1.0.0/genv/enforce/rules/env_memory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from ...utils import memory_to_bytes, bytes_to_memory
+from genv.utils import memory_to_bytes, bytes_to_memory
 
-from ..survey import Survey
+from genv.entities.enforce import Survey
 
 
 def env_memory(*surveys: Survey) -> None:
     """
     Terminates processes from environments that exceed their memory capacity.
     """
     for survey in surveys:
```

### Comparing `genv-0.9.0/genv/enforce/rules/max_devices_per_user.py` & `genv-1.0.0/genv/enforce/rules/max_devices_per_user.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..survey import Survey
+from genv.entities.enforce import Survey
 
 
 def max_devices_per_user(*surveys: Survey, maximum: int) -> None:
     """
     Enforce maximum devices per user.
     """
     usernames = set(
```

### Comparing `genv-0.9.0/genv/enforce/rules/non_env_processes.py` & `genv-1.0.0/genv/enforce/rules/non_env_processes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..survey import Survey
+from genv.entities.enforce import Survey
 
 
 def non_env_processes(*surveys: Survey) -> None:
     """
     Terminates processes that are not running in environments.
     """
     for survey in surveys:
```

### Comparing `genv-0.9.0/genv/enforce/survey.py` & `genv-1.0.0/genv/entities/enforce/survey.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Dict, Optional, Set
 
-from ..snapshot import Snapshot
+from ..core import Snapshot
 
-from .report import Report
+from . import Report
 
 
 @dataclass
 class Survey:
     snapshot: Snapshot
     hostname: Optional[str] = None
```

### Comparing `genv-0.9.0/genv/envs.py` & `genv-1.0.0/genv/entities/core/envs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,104 @@
 from dataclasses import dataclass
-import subprocess
-from typing import Any, Dict, Iterable, Optional, Union
+from datetime import datetime
+from pathlib import Path
+from typing import Any, Callable, Iterable, Optional, Type, Union
 
-from . import utils
-
-# NOTE(raz): This should be the layer that queries and controls the state of Genv regarding active environments.
-# Currently, it relies on executing the environment manager executable of Genv, as this is where the logic is implemented.
-# This however should be done oppositely.
-# The entire logic that queries and controls envs.json should be implemented here, and the environment manager executable
-# should use methods from here.
-# It should take the Genv lock for the atomicity of the transaction, and print output as needed.
-# The current architecture has an inherent potential deadlock because each manager locks a different lock, and might
-# call the other manager.
+import genv.utils
 
 
 @dataclass
 class Env:
+    @dataclass
+    class Config:
+        name: Optional[str] = None
+        gpu_memory: Optional[str] = None
+        gpus: Optional[int] = None
+
+        def load(self, path: Union[str, Path]) -> None:
+            """Loads from disk"""
+
+            def _load_field(basename: str, type: Type = str) -> None:
+                file = Path(path).joinpath(basename)
+
+                if file.is_file():
+                    return type(file.read_text().strip())
+
+            self.name = _load_field("name")
+            self.gpu_memory = _load_field("gpu-memory")
+            self.gpus = _load_field("gpus", int)
+
+        def save(self, path: Union[str, Path]) -> None:
+            """Saves to disk"""
+
+            def _save_field(basename: str, value: Optional[Any]) -> None:
+                file = Path(path).joinpath(basename)
+
+                if value is not None:
+                    file.write_text(str(value))
+                else:
+                    file.unlink(missing_ok=True)
+
+            _save_field("name", self.name)
+            _save_field("gpu-memory", self.gpu_memory)
+            _save_field("gpus", self.gpus)
+
     eid: str
     uid: int
     creation: str
     username: Optional[str]
-
-    @dataclass
-    class Config:
-        name: Optional[str]
-        gpu_memory: Optional[str]
-
     config: Config
+    pids: Iterable[int]
+    kernel_ids: Iterable[str]
 
     @property
     def time_since(self) -> str:
-        return utils.time_since(self.creation)
+        return genv.utils.time_since(self.creation)
+
+    @property
+    def active(self) -> bool:
+        return len(self.pids) > 0 or len(self.kernel_ids) > 0
 
     def __hash__(self) -> int:
         return self.eid.__hash__()
 
+    def cleanup(
+        self,
+        *,
+        poll_pid: Callable[[int], bool] = None,
+        poll_kernel: Callable[[str], bool] = None,
+    ):
+        """
+        Cleans up in place.
+        """
+        if poll_pid is not None:
+            self.pids = [pid for pid in self.pids if poll_pid(pid)]
+
+        if poll_kernel is not None:
+            self.kernel_ids = [
+                kernel_id for kernel_id in self.kernel_ids if poll_kernel(kernel_id)
+            ]
+
+    def attach(
+        self, *, pid: Optional[int] = None, kernel_id: Optional[str] = None
+    ) -> None:
+        """
+        Attaches a process or a Jupyter kernel to an environment.
+        """
+        if pid is not None:
+            self.pids.append(pid)
+
+        if kernel_id is not None:
+            self.kernel_ids.append(kernel_id)
+
 
 @dataclass
-class Snapshot:
+class Envs:
     """
-    A snapshot of active environments.
+    A collection of environments.
     """
 
     envs: Iterable[Env]
 
     @property
     def eids(self) -> Iterable[str]:
         return [env.eid for env in self.envs]
@@ -57,24 +112,48 @@
 
     def __len__(self):
         return self.envs.__len__()
 
     def __getitem__(self, eid: str) -> Env:
         return next(env for env in self.envs if env.eid == eid)
 
+    def __contains__(self, eid: str) -> bool:
+        return any(env.eid == eid for env in self.envs)
+
+    def activate(
+        self,
+        eid: str,
+        uid: int,
+        username: Optional[str] = None,
+    ) -> None:
+        """
+        Activates a new environment.
+        """
+        self.envs.append(
+            Env(
+                eid=eid,
+                uid=uid,
+                creation=datetime.now().strftime(genv.utils.DATETIME_FMT),
+                username=username,
+                config=Env.Config(name=None, gpu_memory=None, gpus=None),
+                pids=[],
+                kernel_ids=[],
+            )
+        )
+
     def filter(
         self,
         deep: bool = True,
         *,
         eid: Optional[str] = None,
         eids: Optional[Iterable[str]] = None,
         username: Optional[str] = None,
     ):
         """
-        Returns a new filtered snapshot.
+        Returns a new filtered collection.
 
         :param deep: Perform deep filtering
         :param eid: Environment identifier to keep
         :param eids: Environment identifiers to keep
         :param username: Username to keep
         """
         if eids:
@@ -90,134 +169,56 @@
 
         if eids is not None:
             envs = [env for env in envs if env.eid in eids]
 
         if username is not None:
             envs = [env for env in envs if env.username == username]
 
-        return Snapshot(envs)
-
-
-def snapshot() -> Snapshot:
-    return Snapshot(
-        [
-            Env(
-                eid,
-                int(uid),
-                creation,
-                username or None,
-                Env.Config(name or None, gpu_memory or None),
-            )
-            for eid, uid, creation, username, name, gpu_memory in query(
-                "eid", "uid", "creation", "username", "config.name", "config.gpu_memory"
-            )
-        ]
-    )
+        return Envs(envs)
 
+    def cleanup(
+        self,
+        *,
+        eid: Optional[str] = None,
+        eids: Optional[Iterable[str]] = None,
+        poll_pid: Callable[[int], bool] = None,
+        poll_kernel: Callable[[str], bool] = None,
+    ):
+        """Cleans up the collection in place.
 
-def query(
-    *properties: str, eid: Optional[str] = None, eids: bool = False
-) -> Union[
-    str,
-    Iterable[str],
-    Iterable[Iterable[str]],
-    Dict[str, str],
-    Dict[str, Iterable[str]],
-]:
-    """
-    Queries the environment manager about all active environments or a specific one.
-    Returns a query result per environment.
-    A query result can be a single string if only a single property was queried,
-    or a list of strings if multiple properties were queried.
-
-    :param properties: Environment properties to query
-    :param eid: Identifier of a specific environment to query
-    :param eids: Return a mapping between environment identifiers to query results
-    """
-    if len(properties) == 0:
-        raise RuntimeError("At least one query property must be provided")
-
-    command = "genv exec envs query"
-
-    if eid:
-        command = f"{command} --eid {eid}"
-    else:
-        properties = ("eid", *properties)
-
-    command = f"{command} --query {' '.join(properties)}"
-
-    output = subprocess.check_output(command, shell=True).decode("utf-8").strip()
-
-    if eid:
-        return output if len(properties) == 1 else output.split(",")
-    else:
-        result = dict()
-
-        for line in output.splitlines():
-            eid, line = line.split(",", 1)
-            result[eid] = line if (len(properties) - 1) == 1 else line.split(",")
-
-        return result if eids else list(result.values())
-
-
-def eids() -> Iterable[str]:
-    """
-    Returns the identifiers of all active environments.
-
-    :return: Identifiers of all active environments.
-    """
-    return query("eid")
-
-
-def names() -> Dict[str, Optional[str]]:
-    """
-    Returns the names of all active environments.
-
-    :return: A mapping from environment identifier to its configured name or None if not configured.
-    """
-    return {
-        eid: (name or None) for eid, name in query("config.name", eids=True).items()
-    }
-
-
-def gpus(eid: str) -> Optional[int]:
-    """
-    Returns the configured device count an environment.
-    """
-    s = query("config.gpus", eid=eid)
-
-    return int(s) if s else None
+        Cleans only the specified environments when passing identifiers.
+        """
+        if eids:
+            eids = set(eids)
 
+        if eid:
+            if not eids:
+                eids = set()
 
-def gpu_memory(eid: str) -> Optional[str]:
-    """
-    Returns the configured amount of GPU memory of an environment.
+            eids.add(eid)
 
-    :param eid: Environment to query
-    :return: The configured amount of GPU memory or None if not configured
-    """
-    return query("config.gpu_memory", eid=eid) or None
+        for env in self.envs:
+            if eids is not None:
+                if env.eid not in eids:
+                    continue
+
+            env.cleanup(poll_pid=poll_pid, poll_kernel=poll_kernel)
+
+        self.envs = [env for env in self.envs if env.active]
+
+    def find(
+        self, *, pid: Optional[int] = None, kernel_id: Optional[str] = None
+    ) -> Iterable[Env]:
+        """
+        Returns the environments of the given process or kernel.
+        """
 
+        def _pred(env: Env) -> bool:
+            if (pid is not None) and (pid in env.pids):
+                return True
 
-def activate(eid: str, uid: int, pid: int) -> None:
-    """
-    Activates an environment.
-    """
-    subprocess.check_output(
-        f"genv exec envs activate --eid {eid} --uid {uid} --pid {pid}",
-        shell=True,
-    )
+            if (kernel_id is not None) and (kernel_id in env.kernel_ids):
+                return True
 
+            return False
 
-def configure(eid: str, command: str, value: Any) -> None:
-    """
-    Configures an environment.
-    """
-    ARGUMENTS = {
-        "gpus": "--count",
-        "gpu-memory": "--gpu-memory",
-    }
-
-    subprocess.check_output(
-        f"genv exec envs config --eid {eid} {command} {ARGUMENTS[command]} {str(value)}",
-        shell=True,
-    )
+        return [env for env in self.envs if _pred(env)]
```

### Comparing `genv-0.9.0/genv/metrics/collection.py` & `genv-1.0.0/genv/metrics/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Iterable
 
-from genv.metrics.metric import Metric
-from genv.metrics.spec import Spec
-from genv.metrics.type import Type
-from genv.snapshot import Snapshot
+from genv.entities import Snapshot
+
+from .metric import Metric
+from .spec import Spec
+from .type import Type
 
 
 class Collection:
     """
     A metric collection.
     """
```

### Comparing `genv-0.9.0/genv/metrics/metric.py` & `genv-1.0.0/genv/metrics/metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Callable, Iterable, Optional
 
 import prometheus_client
 
-from genv.snapshot import Snapshot
-from genv.metrics.spec import Type
+from genv.entities import Snapshot
+
+from .spec import Type
 
 
 class Metric(prometheus_client.Gauge):
     """
     A Genv metric.
     """
```

### Comparing `genv-0.9.0/genv/metrics/publisher.py` & `genv-1.0.0/genv/metrics/publisher.py`

 * *Files identical despite different names*

### Comparing `genv-0.9.0/genv/metrics/specs.py` & `genv-1.0.0/genv/metrics/specs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 import sys
 
-from genv.metrics.spec import Spec, Type
+from .spec import Spec, Type
 
 
 def Device(*args, **kwargs) -> Spec:
     """
     Returns a per-device metric specification.
     """
     labelnames = kwargs.pop("labelnames", tuple())
```

### Comparing `genv-0.9.0/genv/nvidia_smi.py` & `genv-1.0.0/genv/utils/nvidia_smi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from typing import Dict, Iterable
 
-from .runners.runner import Runner
-from .runners.local import LocalRunner
+from .runners import Runner, Local
 
 DEFAULT_NVIDIA_SMI_ENV_VARS = {"GENV_BYPASS": "1", **os.environ}
-DEFAULT_LOCAL_RUNNER = LocalRunner(DEFAULT_NVIDIA_SMI_ENV_VARS)
+DEFAULT_LOCAL_RUNNER = Local(DEFAULT_NVIDIA_SMI_ENV_VARS)
 
 NVIDIA_SMI = "nvidia-smi"
 CSV_FORMAT_PARAM = "--format=csv,noheader,nounits"
 NVIDIA_CSV_SPLITTER = ", "
 
 
 async def device_uuids(runner: Runner = DEFAULT_LOCAL_RUNNER) -> Dict[str, int]:
```

### Comparing `genv-0.9.0/genv/poll.py` & `genv-1.0.0/genv/utils/poll.py`

 * *Files identical despite different names*

### Comparing `genv-0.9.0/genv/processes.py` & `genv-1.0.0/genv/entities/core/processes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-import asyncio
 from dataclasses import dataclass
 import sys
 from typing import Iterable, Optional
 
-from . import nvidia_smi
-from . import os_
-from . import utils
+import genv.utils
 
 
 @dataclass
 class Process:
     """
-    A compute running process either from an environment or not.
+    A compute running process.
     """
 
     @dataclass
     class Usage:
         """
         The GPU index and amount of GPU memory used by the process.
         """
 
         index: int
         gpu_memory: str
 
         @property
         def bytes(self) -> int:
-            return utils.memory_to_bytes(self.gpu_memory)
+            return genv.utils.memory_to_bytes(self.gpu_memory)
 
     pid: int
     used_gpu_memory: Iterable[Usage]
     eid: Optional[str]
 
     @property
     def indices(self) -> Iterable[int]:
@@ -55,28 +52,28 @@
     @staticmethod
     def eid(pid: int) -> Optional[str]:
         """
         Returns the environment identifier of the process with the given pid.
         Returns None if the process is not running in an environment or if it could not be queried.
         """
         try:
-            return os_.get_process_environ(pid).get("GENV_ENVIRONMENT_ID")
+            return genv.utils.get_process_environ(pid).get("GENV_ENVIRONMENT_ID")
         except PermissionError:
             print(
                 f"[WARNING] Not enough permissions to query environment of process {pid}",
                 file=sys.stderr,
             )
         except FileNotFoundError:
             print(f"[DEBUG] Process {pid} already terminated", file=sys.stderr)
 
 
 @dataclass
-class Snapshot:
+class Processes:
     """
-    A snapshot of running processes.
+    A collection of processes.
     """
 
     processes: Iterable[Process]
 
     @property
     def pids(self) -> Iterable[int]:
         return [process.pid for process in self.processes]
@@ -96,15 +93,15 @@
         *,
         pids: Optional[Iterable[int]] = None,
         eid: Optional[str] = None,
         eids: Optional[Iterable[str]] = None,
         index: Optional[int] = None,
     ):
         """
-        Returns a new filtered snapshot.
+        Returns a new filtered collection.
 
         :param deep: Perform deep filtering
         :param pids: Process identifiers to keep
         :param eid: Environment identifier to keep
         :param eids: Environment identifiers to keep
         :param username: Username to keep
         """
@@ -127,38 +124,8 @@
 
         if index is not None:
             if deep:
                 processes = [process.filter(index=index) for process in processes]
 
             processes = [process for process in processes if index in process.indices]
 
-        return Snapshot(processes)
-
-
-async def snapshot() -> Snapshot:
-    """
-    Returns a snapshot of all running compute processes.
-    """
-    uuids, apps = await asyncio.gather(
-        nvidia_smi.device_uuids(), nvidia_smi.compute_apps()
-    )
-
-    pid_to_apps = {
-        pid: [app for app in apps if app["pid"] == pid]
-        for pid in set(app["pid"] for app in apps)
-    }
-
-    return Snapshot(
-        [
-            Process(
-                pid=pid,
-                used_gpu_memory=[
-                    Process.Usage(
-                        index=uuids[app["gpu_uuid"]], gpu_memory=app["used_gpu_memory"]
-                    )
-                    for app in apps
-                ],
-                eid=Process.eid(pid),
-            )
-            for pid, apps in pid_to_apps.items()
-        ]
-    )
+        return Processes(processes)
```

### Comparing `genv-0.9.0/genv/remote/enforce/execute.py` & `genv-1.0.0/genv/remote/enforce/execute.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import json
 from typing import Iterable
 
-from ...json_ import JSONEncoder
-from ...enforce import Report
+from genv.entities.enforce import Report
 
-from ..utils import reprint
-from ..ssh import run, Config, Command
+from genv.serialization import JSONEncoder
+
+from ..utils import reprint, run, Config, Command
 
 
 async def execute(config: Config, reports: Iterable[Report]) -> None:
     """
     Executes reports on multiple hosts.
 
     :param reports: Reports to execute on each host
 
     :return: None
     """
-    command = Command(["exec", "usage", "execute"], sudo=True)
+    command = Command(["usage", "execute"], sudo=True)
 
     hosts, stdouts = await run(
         config,
         command,
         stdins=[json.dumps(report, cls=JSONEncoder) for report in reports],
     )
```

### Comparing `genv-0.9.0/genv/remote/snapshot.py` & `genv-1.0.0/genv/remote/core/snapshot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 from typing import Iterable, Optional, Tuple
 
-from ..snapshot import Snapshot
-from ..json_ import JSONDecoder
+from genv.entities import Snapshot
+from genv.serialization import JSONDecoder
 
-from .ssh import run, Host, Config, Command
+from ..utils import run, Host, Config, Command
 
 # TODO(raz): should we support cases where 'sudo' is not an option?
 
 
 async def exec(config: Config, *, type: Optional[str], sudo: bool):
-    args = ["exec", "usage", "snapshot"]
+    args = ["usage", "snapshot"]
 
     if type:
         args.append(f"--type {type}")
 
     command = Command(args, sudo)
 
     hosts, stdouts = await run(config, command)
```

### Comparing `genv-0.9.0/genv/remote/ssh.py` & `genv-1.0.0/genv/remote/utils/ssh.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import asyncio
 from dataclasses import dataclass
 import sys
 from typing import Any, Callable, Iterable, Optional, Tuple
 
+from genv.utils.runners import SSH as Runner
+
 from .utils import reprint
-from ..runners.ssh import SshRunner
 
 
 @dataclass
 class Host:
     """
     Host configuration.
 
     :param hostname: Hostname or IP address
-    :param root: Genv installation directory
     :param timeout: SSH connection timeout
     """
 
     hostname: str
-    root: str
     timeout: Optional[int]
 
 
 @dataclass
 class Config:
     """
     Execution configuration.
@@ -32,14 +31,15 @@
     :param quiet: Ignore SSH errors
     """
 
     hosts: Iterable[Host]
     throw_on_error: bool
     quiet: bool
 
+
 @dataclass
 class Command:
     """
     Genv command specification.
 
     :param args: Genv command arguments
     :param sudo: Run command as root using sudo
@@ -61,15 +61,18 @@
     :param command: Genv command specification
     :param stdins: Input to send per host
 
     :return: Returns the hosts that succeeded and their standard outputs
     """
     ssh_runners_and_inputs = []
     for host, stdin in zip(config.hosts, stdins or [None for _ in config.hosts]):
-        ssh_runner = SshRunner(host.hostname, host.timeout, {'PATH': SshRunner.calc_remote_path_env(host.root)})
+        ssh_runner = Runner(
+            host.hostname,
+            host.timeout,
+        )
         ssh_runners_and_inputs.append((ssh_runner, stdin))
 
     ssh_outputs = await asyncio.gather(
         *(
             ssh_runner.run("genv", *command.args, stdin=stdin, sudo=command.sudo)
             for ssh_runner, stdin in ssh_runners_and_inputs
         )
```

### Comparing `genv-0.9.0/genv/remote/utils.py` & `genv-1.0.0/genv/remote/utils/utils.py`

 * *Files identical despite different names*

### Comparing `genv-0.9.0/genv/runners/local.py` & `genv-1.0.0/genv/utils/runners/local.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from asyncio.subprocess import Process
 
-from .runner import Runner
+from .runner import Runner as Base
 
 
-class LocalRunner(Runner):
+class Runner(Base):
     def name(self) -> str:
         return "local"
 
     async def _open_process(self, *args: str, stdin_fd: int, sudo: bool) -> Process:
         if sudo:
             args = ["sudo", *args]
```

### Comparing `genv-0.9.0/genv/runners/runner.py` & `genv-1.0.0/genv/utils/runners/runner.py`

 * *Files identical despite different names*

### Comparing `genv-0.9.0/genv.egg-info/PKG-INFO` & `genv-1.0.0/genv.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 Metadata-Version: 2.1
 Name: genv
-Version: 0.9.0
-Summary: GPU Environment Management
+Version: 1.0.0
+Summary: GPU environment and cluster management
 Home-page: https://github.com/run-ai/genv
-Author: Run:AI
+Author: Run.ai
 Author-email: pypi@run.ai
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: GPU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: Terminals
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: monitor
+License-File: LICENSE
 
 <p align="center">
   <img src="images/genv blade landscape black@4x.png#gh-light-mode-only" width="600" alt="genv"/>
   <img src="images/genv blade landscape white@4x.png#gh-dark-mode-only" width="600" alt="genv"/>
 </p>
 
 # Genv (GPU Environment Management) [![Join the community at (https://discord.gg/zN3Q9pQAuT)](https://img.shields.io/badge/Discord-genv-7289da?logo=discord)](https://discord.gg/zN3Q9pQAuT)
@@ -73,37 +81,7 @@
 
 
 ## License
 The Genv software is Copyright 2022 [Run.ai Labs, Ltd.].
 The software is licensed by Run.ai under the AGPLv3 license.
 Please note that Run.ai’s intention in licensing the software are that the obligations of licensee pursuant to the AGPLv3 license should be interpreted broadly.
 For example, Run.ai’s intention is that the terms “work based on the Program” in Section 0 of the AGPLv3 license, and “Corresponding Source” in Section 1 of the AGPLv3 license, should be interpreted as broadly as possible to the extent permitted under applicable law.
-
-Genv Remote vs. Run.ai
-----------------------
-1. containers vs environments
-2. SSH vs k8s
-3. interception- vs monitoring-based enfircements
-4. non-centralized (no load balancing)
-5. no advanced user roles (everyone can list envs and devices)
-6. shim-based visualization vs. interception-based virtualization
-7. environment must fit in a node vs. multi-node workload
-8. no compute mgmt
-
-
-QUOTA:
------
-system:
-    [V] (nvidia-smi)      non env processes
-    [V] (nvidia-smi)      processes from envs on non-attached devices
-    [ ] (envs.json)       timeout
-
-resources:
-    [V] (devices.json)    num of attached devices
-
-    (later...)
-    [ ] (nvidia-smi)      num of processes (as an alternative to compute mgmt)
-    [ ] (envs.json)       num of active envs
-    [ ] (envs.json)       num of machines with active envs
-    [ ] (nvidia-smi)      amount of GPU memory (per device/total)
-
-https://grafana.com/docs/grafana/latest/cli/#override-homepath-value
```

