# Comparing `tmp/remoulade-1.2.2.tar.gz` & `tmp/remoulade-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remoulade-1.2.2.tar", last modified: Tue May 23 15:41:08 2023, max compression
+gzip compressed data, was "remoulade-1.2.3.tar", last modified: Mon Jun 12 08:35:43 2023, max compression
```

## Comparing `remoulade-1.2.2.tar` & `remoulade-1.2.3.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.409070 remoulade-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-23 15:40:52.000000 remoulade-1.2.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-05-23 15:40:52.000000 remoulade-1.2.2/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-23 15:40:52.000000 remoulade-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-23 15:41:08.409070 remoulade-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-23 15:40:52.000000 remoulade-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.389070 remoulade-1.2.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      275 2023-05-23 15:40:52.000000 remoulade-1.2.2/bin/remoulade-gevent
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-23 15:40:52.000000 remoulade-1.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.393070 remoulade-1.2.2/remoulade/
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.397070 remoulade-1.2.2/remoulade/api/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/api/apispec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/api/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/api/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    17143 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.397070 remoulade-1.2.2/remoulade/brokers/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/brokers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/brokers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/brokers/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/brokers/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.397070 remoulade-1.2.2/remoulade/cancel/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/cancel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/cancel/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.397070 remoulade-1.2.2/remoulade/cancel/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/cancel/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/cancel/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/cancel/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/cancel/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/cancel/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.401070 remoulade-1.2.2/remoulade/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/cli/remoulade_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/cli/remoulade_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/cli/remoulade_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/collection_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.401070 remoulade-1.2.2/remoulade/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/helpers/actor_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/helpers/backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/helpers/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/helpers/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.405070 remoulade-1.2.2/remoulade/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/age_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/catch_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/current_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/logging_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/max_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/max_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/retries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/middleware/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.405070 remoulade-1.2.2/remoulade/rate_limits/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/rate_limits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/rate_limits/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.405070 remoulade-1.2.2/remoulade/rate_limits/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/rate_limits/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/rate_limits/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/rate_limits/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/rate_limits/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/rate_limits/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/rate_limits/rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/rate_limits/window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.405070 remoulade-1.2.2/remoulade/results/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/results/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.405070 remoulade-1.2.2/remoulade/results/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/results/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/results/backends/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/results/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/results/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/results/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/results/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.405070 remoulade-1.2.2/remoulade/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.409070 remoulade-1.2.2/remoulade/state/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/state/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.409070 remoulade-1.2.2/remoulade/state/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/state/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/state/backends/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/state/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/state/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/state/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/state/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-05-23 15:40:52.000000 remoulade-1.2.2/remoulade/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:41:08.397070 remoulade-1.2.2/remoulade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-23 15:41:08.000000 remoulade-1.2.2/remoulade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-23 15:41:08.000000 remoulade-1.2.2/remoulade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:41:08.000000 remoulade-1.2.2/remoulade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-23 15:41:08.000000 remoulade-1.2.2/remoulade.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-23 15:41:08.000000 remoulade-1.2.2/remoulade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 15:41:08.000000 remoulade-1.2.2/remoulade.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-23 15:41:08.409070 remoulade-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-23 15:40:52.000000 remoulade-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.430018 remoulade-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-12 08:35:34.000000 remoulade-1.2.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-12 08:35:34.000000 remoulade-1.2.3/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-12 08:35:34.000000 remoulade-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-12 08:35:43.430018 remoulade-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-12 08:35:34.000000 remoulade-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.422018 remoulade-1.2.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      275 2023-06-12 08:35:34.000000 remoulade-1.2.3/bin/remoulade-gevent
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-12 08:35:34.000000 remoulade-1.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.422018 remoulade-1.2.3/remoulade/
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.422018 remoulade-1.2.3/remoulade/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/api/apispec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/api/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/api/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17143 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.426018 remoulade-1.2.3/remoulade/brokers/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/brokers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/brokers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/brokers/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/brokers/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.426018 remoulade-1.2.3/remoulade/cancel/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/cancel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/cancel/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.426018 remoulade-1.2.3/remoulade/cancel/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/cancel/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/cancel/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/cancel/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/cancel/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/cancel/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.426018 remoulade-1.2.3/remoulade/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/cli/remoulade_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/cli/remoulade_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/cli/remoulade_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/collection_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.426018 remoulade-1.2.3/remoulade/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/helpers/actor_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/helpers/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/helpers/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/helpers/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.426018 remoulade-1.2.3/remoulade/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/age_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/catch_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/current_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/logging_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/max_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/max_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/middleware/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.426018 remoulade-1.2.3/remoulade/rate_limits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/rate_limits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/rate_limits/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.426018 remoulade-1.2.3/remoulade/rate_limits/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/rate_limits/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/rate_limits/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/rate_limits/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/rate_limits/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/rate_limits/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/rate_limits/rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/rate_limits/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.426018 remoulade-1.2.3/remoulade/results/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/results/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.426018 remoulade-1.2.3/remoulade/results/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/results/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/results/backends/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/results/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/results/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/results/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/results/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.430018 remoulade-1.2.3/remoulade/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.430018 remoulade-1.2.3/remoulade/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/state/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.430018 remoulade-1.2.3/remoulade/state/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/state/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/state/backends/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/state/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/state/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/state/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/state/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-06-12 08:35:34.000000 remoulade-1.2.3/remoulade/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:35:43.422018 remoulade-1.2.3/remoulade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-12 08:35:43.000000 remoulade-1.2.3/remoulade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-12 08:35:43.000000 remoulade-1.2.3/remoulade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:35:43.000000 remoulade-1.2.3/remoulade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-12 08:35:43.000000 remoulade-1.2.3/remoulade.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-12 08:35:43.000000 remoulade-1.2.3/remoulade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 08:35:43.000000 remoulade-1.2.3/remoulade.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-12 08:35:43.430018 remoulade-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-12 08:35:34.000000 remoulade-1.2.3/setup.py
```

### Comparing `remoulade-1.2.2/COPYING` & `remoulade-1.2.3/COPYING`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/COPYING.LESSER` & `remoulade-1.2.3/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/PKG-INFO` & `remoulade-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remoulade
-Version: 1.2.2
+Version: 1.2.3
 Summary: Background Processing for Python 3.
 Author: Wiremind
 Author-email: dev@wiremind.io
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `remoulade-1.2.2/README.md` & `remoulade-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/__init__.py` & `remoulade-1.2.3/remoulade/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,8 +86,8 @@
     # Workers
     "Worker",
     # Scheduler
     "get_scheduler",
     "set_scheduler",
 ]
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
```

### Comparing `remoulade-1.2.2/remoulade/__main__.py` & `remoulade-1.2.3/remoulade/__main__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/actor.py` & `remoulade-1.2.3/remoulade/actor.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/api/apispec.py` & `remoulade-1.2.3/remoulade/api/apispec.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/api/main.py` & `remoulade-1.2.3/remoulade/api/main.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/api/scheduler.py` & `remoulade-1.2.3/remoulade/api/scheduler.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/api/state.py` & `remoulade-1.2.3/remoulade/api/state.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/broker.py` & `remoulade-1.2.3/remoulade/broker.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/brokers/__init__.py` & `remoulade-1.2.3/remoulade/brokers/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/brokers/local.py` & `remoulade-1.2.3/remoulade/brokers/local.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/brokers/rabbitmq.py` & `remoulade-1.2.3/remoulade/brokers/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/brokers/stub.py` & `remoulade-1.2.3/remoulade/brokers/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/cancel/__init__.py` & `remoulade-1.2.3/remoulade/cancel/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/cancel/backend.py` & `remoulade-1.2.3/remoulade/cancel/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/cancel/backends/__init__.py` & `remoulade-1.2.3/remoulade/cancel/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/cancel/backends/redis.py` & `remoulade-1.2.3/remoulade/cancel/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/cancel/backends/stub.py` & `remoulade-1.2.3/remoulade/cancel/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/cancel/errors.py` & `remoulade-1.2.3/remoulade/cancel/errors.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/cancel/middleware.py` & `remoulade-1.2.3/remoulade/cancel/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/cli/remoulade_ls.py` & `remoulade-1.2.3/remoulade/cli/remoulade_ls.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/cli/remoulade_run.py` & `remoulade-1.2.3/remoulade/cli/remoulade_run.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/cli/remoulade_scheduler.py` & `remoulade-1.2.3/remoulade/cli/remoulade_scheduler.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/collection_results.py` & `remoulade-1.2.3/remoulade/collection_results.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/common.py` & `remoulade-1.2.3/remoulade/common.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/composition.py` & `remoulade-1.2.3/remoulade/composition.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/encoder.py` & `remoulade-1.2.3/remoulade/encoder.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/errors.py` & `remoulade-1.2.3/remoulade/errors.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/generic.py` & `remoulade-1.2.3/remoulade/generic.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/helpers/__init__.py` & `remoulade-1.2.3/remoulade/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/helpers/actor_arguments.py` & `remoulade-1.2.3/remoulade/helpers/actor_arguments.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/helpers/backoff.py` & `remoulade-1.2.3/remoulade/helpers/backoff.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/helpers/queues.py` & `remoulade-1.2.3/remoulade/helpers/queues.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/helpers/reduce.py` & `remoulade-1.2.3/remoulade/helpers/reduce.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/logging.py` & `remoulade-1.2.3/remoulade/logging.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/message.py` & `remoulade-1.2.3/remoulade/message.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/__init__.py` & `remoulade-1.2.3/remoulade/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/age_limit.py` & `remoulade-1.2.3/remoulade/middleware/age_limit.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/catch_error.py` & `remoulade-1.2.3/remoulade/middleware/catch_error.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/current_message.py` & `remoulade-1.2.3/remoulade/middleware/current_message.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/logging_metadata.py` & `remoulade-1.2.3/remoulade/middleware/logging_metadata.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/max_memory.py` & `remoulade-1.2.3/remoulade/middleware/max_memory.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/max_tasks.py` & `remoulade-1.2.3/remoulade/middleware/max_tasks.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/middleware.py` & `remoulade-1.2.3/remoulade/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/pipelines.py` & `remoulade-1.2.3/remoulade/middleware/pipelines.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/prometheus.py` & `remoulade-1.2.3/remoulade/middleware/prometheus.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/retries.py` & `remoulade-1.2.3/remoulade/middleware/retries.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/shutdown.py` & `remoulade-1.2.3/remoulade/middleware/shutdown.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/threading.py` & `remoulade-1.2.3/remoulade/middleware/threading.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/middleware/time_limit.py` & `remoulade-1.2.3/remoulade/middleware/time_limit.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/rate_limits/__init__.py` & `remoulade-1.2.3/remoulade/rate_limits/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/rate_limits/backend.py` & `remoulade-1.2.3/remoulade/rate_limits/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/rate_limits/backends/__init__.py` & `remoulade-1.2.3/remoulade/rate_limits/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/rate_limits/backends/redis.py` & `remoulade-1.2.3/remoulade/rate_limits/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/rate_limits/backends/stub.py` & `remoulade-1.2.3/remoulade/rate_limits/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/rate_limits/bucket.py` & `remoulade-1.2.3/remoulade/rate_limits/bucket.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/rate_limits/concurrent.py` & `remoulade-1.2.3/remoulade/rate_limits/concurrent.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/rate_limits/rate_limiter.py` & `remoulade-1.2.3/remoulade/rate_limits/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/rate_limits/window.py` & `remoulade-1.2.3/remoulade/rate_limits/window.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/result.py` & `remoulade-1.2.3/remoulade/result.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/results/__init__.py` & `remoulade-1.2.3/remoulade/results/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/results/backend.py` & `remoulade-1.2.3/remoulade/results/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/results/backends/__init__.py` & `remoulade-1.2.3/remoulade/results/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/results/backends/local.py` & `remoulade-1.2.3/remoulade/results/backends/local.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/results/backends/redis.py` & `remoulade-1.2.3/remoulade/results/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/results/backends/stub.py` & `remoulade-1.2.3/remoulade/results/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/results/errors.py` & `remoulade-1.2.3/remoulade/results/errors.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/results/middleware.py` & `remoulade-1.2.3/remoulade/results/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/scheduler/__init__.py` & `remoulade-1.2.3/remoulade/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/scheduler/scheduler.py` & `remoulade-1.2.3/remoulade/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/state/backend.py` & `remoulade-1.2.3/remoulade/state/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/state/backends/__init__.py` & `remoulade-1.2.3/remoulade/state/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/state/backends/postgres.py` & `remoulade-1.2.3/remoulade/state/backends/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         encoder: Optional[Encoder] = None,
         client: Optional[sessionmaker] = None,
         max_size: int = 2000000,
         url: Optional[str] = None,
     ):
         self.url = url or os.getenv("REMOULADE_POSTGRESQL_URL") or DEFAULT_POSTGRES_URI
         super().__init__(namespace=namespace, encoder=encoder)
-        self.client = client or sessionmaker(create_engine(self.url))
+        self.client = client or sessionmaker(create_engine(self.url, pool_pre_ping=True))
         self.init_db()
         self.max_size = max_size
         self.lock = threading.Lock()
 
     def init_db(self):
         with self.client.begin() as session:
             bind = session.get_bind()
```

### Comparing `remoulade-1.2.2/remoulade/state/backends/redis.py` & `remoulade-1.2.3/remoulade/state/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/state/backends/stub.py` & `remoulade-1.2.3/remoulade/state/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/state/middleware.py` & `remoulade-1.2.3/remoulade/state/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/utils.py` & `remoulade-1.2.3/remoulade/utils.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade/worker.py` & `remoulade-1.2.3/remoulade/worker.py`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/remoulade.egg-info/PKG-INFO` & `remoulade-1.2.3/remoulade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remoulade
-Version: 1.2.2
+Version: 1.2.3
 Summary: Background Processing for Python 3.
 Author: Wiremind
 Author-email: dev@wiremind.io
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `remoulade-1.2.2/remoulade.egg-info/SOURCES.txt` & `remoulade-1.2.3/remoulade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/setup.cfg` & `remoulade-1.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `remoulade-1.2.2/setup.py` & `remoulade-1.2.3/setup.py`

 * *Files identical despite different names*

