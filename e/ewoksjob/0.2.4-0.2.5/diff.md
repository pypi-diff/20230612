# Comparing `tmp/ewoksjob-0.2.4.tar.gz` & `tmp/ewoksjob-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksjob-0.2.4.tar", last modified: Thu Jun  1 11:56:32 2023, max compression
+gzip compressed data, was "dist/ewoksjob-0.2.5.tar", last modified: Mon Jun 12 16:36:17 2023, max compression
```

## Comparing `ewoksjob-0.2.4.tar` & `ewoksjob-0.2.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2627 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1698 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob/apps/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/apps/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/apps/ewoks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob/client/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob/client/celery/
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/client/celery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/client/celery/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/client/celery/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/client/dummy_workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob/client/local/
--rw-rw-rw-   0 root         (0) root         (0)      374 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/client/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4410 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/client/local/pool.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/client/local/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/client/local/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5172 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 11:56:26.000000 ewoksjob-0.2.4/src/ewoksjob/events/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob/events/handlers/
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/events/handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/events/handlers/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob/events/readers/
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/events/readers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5423 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/events/readers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/events/readers/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/events/readers/sqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 11:56:26.000000 ewoksjob-0.2.4/src/ewoksjob/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4472 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/tests/test_cancel.py
--rw-rw-rw-   0 root         (0) root         (0)     2391 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      665 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/tests/test_convert.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/tests/test_convert_and_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2617 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/tests/test_events.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/tests/test_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/tests/test_execute_and_upload.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/tests/test_feedback.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/tests/test_future.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/tests/test_futures.py
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/tests/test_task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob/worker/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/worker/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     5824 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/worker/options.py
--rw-rw-rw-   0 root         (0) root         (0)     7410 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/worker/process.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/worker/process_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/worker/slurm.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-06-01 11:50:24.000000 ewoksjob-0.2.4/src/ewoksjob/worker/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2627 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1708 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-01 11:56:32.000000 ewoksjob-0.2.4/src/ewoksjob.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1694 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-12 16:33:11.000000 ewoksjob-0.2.5/src/ewoksjob/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob/apps/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/apps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/apps/ewoks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob/client/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob/client/celery/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/client/celery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/client/celery/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/client/celery/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/client/dummy_workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob/client/local/
+-rw-rw-rw-   0 root         (0) root         (0)      374 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/client/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4410 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/client/local/pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/client/local/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/client/local/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5172 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 16:36:10.000000 ewoksjob-0.2.5/src/ewoksjob/events/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob/events/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/events/handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/events/handlers/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob/events/readers/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/events/readers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5423 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/events/readers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/events/readers/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/events/readers/sqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 16:36:11.000000 ewoksjob-0.2.5/src/ewoksjob/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4458 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/tests/test_cancel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2391 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/tests/test_convert.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/tests/test_convert_and_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/tests/test_events.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/tests/test_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/tests/test_execute_and_upload.py
+-rw-rw-rw-   0 root         (0) root         (0)     1800 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/tests/test_feedback.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/tests/test_future.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/tests/test_futures.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/tests/test_task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob/worker/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/worker/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5824 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/worker/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/worker/process.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/worker/process_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/worker/slurm.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-06-12 15:40:01.000000 ewoksjob-0.2.5/src/ewoksjob/worker/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      842 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-12 16:36:17.000000 ewoksjob-0.2.5/src/ewoksjob.egg-info/top_level.txt
```

### Comparing `ewoksjob-0.2.4/LICENSE.md` & `ewoksjob-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/PKG-INFO` & `ewoksjob-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksjob
-Version: 0.2.4
+Version: 0.2.5
 Summary: Asynchronous and distributed scheduling of Ewoks workflows from python
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
 Project-URL: Documentation, https://ewoksjob.readthedocs.io/
```

### Comparing `ewoksjob-0.2.4/README.md` & `ewoksjob-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/setup.cfg` & `ewoksjob-0.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 	ewoksutils >=0.1.1
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 worker = 
-	ewokscore >=0.3.2
-	ewoks >=0.1.5
+	ewokscore >=0.5
+	ewoks >=0.3
 redis = 
 	redis <5
 sql = 
 	sqlalchemy <2
 monitor = 
 	flower
 slurm =
```

### Comparing `ewoksjob-0.2.4/src/ewoksjob/__main__.py` & `ewoksjob-0.2.5/src/ewoksjob/__main__.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/apps/ewoks.py` & `ewoksjob-0.2.5/src/ewoksjob/apps/ewoks.py`

 * *Files 24% similar despite different names*

```diff
@@ -42,18 +42,25 @@
 
 @app.task()
 @worker_execute_wrapper
 def discover_tasks_from_modules(*args, **kwargs) -> List[dict]:
     return task_discovery.discover_tasks_from_modules(*args, **kwargs)
 
 
+@app.task()
+@worker_execute_wrapper
+def discover_all_tasks(*args, **kwargs) -> List[dict]:
+    return task_discovery.discover_all_tasks(*args, **kwargs)
+
+
 _TASK_MAPPING: Dict[Callable, Callable] = {
     "execute_graph": ewoks.execute_graph,
     "convert_graph": ewoks.convert_graph,
     "discover_tasks_from_modules": task_discovery.discover_tasks_from_modules,
+    "discover_all_tasks": task_discovery.discover_all_tasks,
 }
 
 _BOUND_TASKS = {"execute_graph"}
 
 
 def get_ewoks_task_from_celery_task(celery_task: Callable) -> Callable:
     return _TASK_MAPPING[celery_task.__name__]
```

### Comparing `ewoksjob-0.2.4/src/ewoksjob/client/celery/__init__.py` & `ewoksjob-0.2.5/src/ewoksjob/client/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/client/celery/tasks.py` & `ewoksjob-0.2.5/src/ewoksjob/client/celery/tasks.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from ..dummy_workflow import dummy_workflow
 
 __all__ = [
     "execute_graph",
     "execute_test_graph",
     "convert_workflow",
     "discover_tasks_from_modules",
+    "discover_all_tasks",
 ]
 
 
 def execute_graph(**kw) -> AsyncResult:
     return send_task("ewoksjob.apps.ewoks.execute_graph", **kw)
 
 
@@ -31,7 +32,11 @@
 
 def convert_workflow(**kw) -> AsyncResult:
     return send_task("ewoksjob.apps.ewoks.convert_graph", **kw)
 
 
 def discover_tasks_from_modules(**kw) -> AsyncResult:
     return send_task("ewoksjob.apps.ewoks.discover_tasks_from_modules", **kw)
+
+
+def discover_all_tasks(**kw) -> AsyncResult:
+    return send_task("ewoksjob.apps.ewoks.discover_all_tasks", **kw)
```

### Comparing `ewoksjob-0.2.4/src/ewoksjob/client/celery/utils.py` & `ewoksjob-0.2.5/src/ewoksjob/client/celery/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/client/dummy_workflow.py` & `ewoksjob-0.2.5/src/ewoksjob/client/dummy_workflow.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/client/local/pool.py` & `ewoksjob-0.2.5/src/ewoksjob/client/local/pool.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/client/local/tasks.py` & `ewoksjob-0.2.5/src/ewoksjob/client/local/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 __all__ = [
     "execute_graph",
     "execute_test_graph",
     "convert_workflow",
     "discover_tasks_from_modules",
+    "discover_all_tasks",
 ]
 
 
 def execute_graph(
     args: Optional[Tuple] = tuple(), kwargs: Optional[Mapping] = None
 ) -> Future:
     return _submit_with_jobid(ewoks.execute_graph, args=args, kwargs=kwargs)
@@ -48,14 +49,21 @@
 ) -> Future:
     pool = get_active_pool()
     return pool.submit(
         task_discovery.discover_tasks_from_modules, args=args, kwargs=kwargs
     )
 
 
+def discover_all_tasks(
+    args: Optional[Tuple] = tuple(), kwargs: Optional[Mapping] = None
+) -> Future:
+    pool = get_active_pool()
+    return pool.submit(task_discovery.discover_all_tasks, args=args, kwargs=kwargs)
+
+
 def _submit_with_jobid(
     func: Callable, args: Optional[Tuple] = tuple(), kwargs: Optional[Mapping] = None
 ) -> Future:
     pool = get_active_pool()
     if kwargs is None:
         kwargs = dict()
     execinfo = kwargs.setdefault("execinfo", dict())
```

### Comparing `ewoksjob-0.2.4/src/ewoksjob/client/local/utils.py` & `ewoksjob-0.2.5/src/ewoksjob/client/local/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/config.py` & `ewoksjob-0.2.5/src/ewoksjob/config.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/events/handlers/redis.py` & `ewoksjob-0.2.5/src/ewoksjob/events/handlers/redis.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/events/readers/__init__.py` & `ewoksjob-0.2.5/src/ewoksjob/events/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/events/readers/base.py` & `ewoksjob-0.2.5/src/ewoksjob/events/readers/base.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/events/readers/redis.py` & `ewoksjob-0.2.5/src/ewoksjob/events/readers/redis.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/events/readers/sqlite3.py` & `ewoksjob-0.2.5/src/ewoksjob/events/readers/sqlite3.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/tests/conftest.py` & `ewoksjob-0.2.5/src/ewoksjob/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 
 from ewokscore import events
 from ewokscore.events import cleanup
 from ewoksjob.events.readers import instantiate_reader
 from ewoksjob.worker import options as worker_options
 
-from .utils import has_redis_server
+from .utils import has_redis
 from ..client import local
 
 try:
     from pyslurmutils.tests.conftest import slurm_data_directory  # noqa F401
     from pyslurmutils.tests.conftest import slurm_log_directory  # noqa F401
     from pyslurmutils.tests.conftest import data_directory  # noqa F401
     from pyslurmutils.tests.conftest import log_directory  # noqa F401
@@ -20,15 +20,15 @@
 except ImportError:
 
     @pytest.fixture(scope="session")
     def slurm_config() -> None:
         pytest.skip("requires pyslurmutils")
 
 
-if has_redis_server():
+if has_redis():
     import redis
 
     @pytest.fixture(scope="session")
     def celery_config(redis_proc):
         url = f"redis://{redis_proc.host}:{redis_proc.port}"
         # celery -A ewoksjob.apps.ewoks --broker={url}/0 --result-backend={url}/1 inspect stats -t 5
         return {
```

### Comparing `ewoksjob-0.2.4/src/ewoksjob/tests/test_cancel.py` & `ewoksjob-0.2.5/src/ewoksjob/tests/test_cancel.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/tests/test_config.py` & `ewoksjob-0.2.5/src/ewoksjob/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/tests/test_convert.py` & `ewoksjob-0.2.5/src/ewoksjob/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/tests/test_convert_and_execute.py` & `ewoksjob-0.2.5/src/ewoksjob/tests/test_convert_and_execute.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/tests/test_events.py` & `ewoksjob-0.2.5/src/ewoksjob/tests/test_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pytest
 import datetime
 import threading
 from ewokscore import events
-from .utils import has_redis_server
+from .utils import has_redis
 
 
-@pytest.mark.skipif(not has_redis_server(), reason="redis-server not installed")
+@pytest.mark.skipif(not has_redis(), reason="redis-server not installed")
 def test_redis(redis_ewoks_events):
     handlers, reader = redis_ewoks_events
     assert_event_reader(handlers, reader)
 
 
 def test_sqlite3(sqlite3_ewoks_events):
     handlers, reader = sqlite3_ewoks_events
     assert_event_reader(handlers, reader)
 
 
-@pytest.mark.skipif(not has_redis_server(), reason="redis-server not installed")
+@pytest.mark.skipif(not has_redis(), reason="redis-server not installed")
 def test_redis_stop_wait_events(redis_ewoks_events):
     _, reader = redis_ewoks_events
     assert_stop_event(reader)
 
 
 def test_sqlite3_stop_wait_events(sqlite3_ewoks_events):
     _, reader = sqlite3_ewoks_events
```

### Comparing `ewoksjob-0.2.4/src/ewoksjob/tests/test_execute.py` & `ewoksjob-0.2.5/src/ewoksjob/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/tests/test_execute_and_upload.py` & `ewoksjob-0.2.5/src/ewoksjob/tests/test_execute_and_upload.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/tests/test_feedback.py` & `ewoksjob-0.2.5/src/ewoksjob/tests/test_feedback.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from ewokscore import Task
 from ewoksutils.import_utils import qualname
 from ewoks import execute_graph
-from .utils import has_redis_server
+from .utils import has_redis
 
 
 class AddNumbers(Task, input_names=["a", "b"], output_names=["sum"]):
     def run(self):
         self.outputs.sum = self.inputs.a + self.inputs.b
 
 
@@ -19,15 +19,15 @@
                 "task_identifier": qualname(AddNumbers),
                 "task_type": "class",
             }
         ],
     }
 
 
-@pytest.mark.skipif(not has_redis_server(), reason="redis-server not installed")
+@pytest.mark.skipif(not has_redis(), reason="redis-server not installed")
 @pytest.mark.parametrize("scheme", ("nexus", "json"))
 def test_redis(scheme, redis_ewoks_events, tmpdir):
     handlers, reader = redis_ewoks_events
     assert_feedback(scheme, handlers, reader, tmpdir)
 
 
 @pytest.mark.parametrize("scheme", ("nexus", "json"))
```

### Comparing `ewoksjob-0.2.4/src/ewoksjob/tests/test_future.py` & `ewoksjob-0.2.5/src/ewoksjob/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/tests/test_futures.py` & `ewoksjob-0.2.5/src/ewoksjob/tests/test_futures.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pytest
 from ..client import celery
 from ..client import local
 from .utils import wait_not_finished
-from .utils import has_redis_server
+from .utils import has_redis
 
 
 @pytest.mark.skip(reason="working in manual testing")
 @pytest.mark.skipif(
-    not has_redis_server(), reason="memory and sqlite do not support task monitoring"
+    not has_redis(), reason="memory and sqlite do not support task monitoring"
 )
 def test_futures(ewoks_worker):
     assert_futures(celery)
 
 
 def test_futures_local(local_ewoks_worker):
     assert_futures(local)
```

### Comparing `ewoksjob-0.2.4/src/ewoksjob/tests/utils.py` & `ewoksjob-0.2.5/src/ewoksjob/tests/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,29 +2,33 @@
 import time
 import logging
 from types import ModuleType
 
 logger = logging.getLogger(__name__)
 
 
-def has_redis_server():
+def has_redis() -> bool:
+    try:
+        import redis  # noqa F401
+    except ImportError:
+        return False
     with os.popen("redis-server --version") as output:
         return bool(output.read())
 
 
 def get_result(future, **kwargs):
     if hasattr(future, "get"):
         return future.get(**kwargs)
     else:
         return future.result(**kwargs)
 
 
 def wait_not_finished(mod: ModuleType, expected_task_ids: set, timeout=3):
     """Wait until all running task ID's are `expected_task_ids`"""
-    if mod.__name__.endswith("celery") and not has_redis_server():
+    if mod.__name__.endswith("celery") and not has_redis():
         time.sleep(0.1)
         logger.warning("memory and sqlite do not support task monitoring")
         return
     t0 = time.time()
     while True:
         task_ids = set(mod.get_not_finished_task_ids())
         if task_ids == expected_task_ids:
```

### Comparing `ewoksjob-0.2.4/src/ewoksjob/worker/errors.py` & `ewoksjob-0.2.5/src/ewoksjob/worker/errors.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/worker/options.py` & `ewoksjob-0.2.5/src/ewoksjob/worker/options.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/worker/process.py` & `ewoksjob-0.2.5/src/ewoksjob/worker/process.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/worker/slurm.py` & `ewoksjob-0.2.5/src/ewoksjob/worker/slurm.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob/worker/task.py` & `ewoksjob-0.2.5/src/ewoksjob/worker/task.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob.egg-info/PKG-INFO` & `ewoksjob-0.2.5/src/ewoksjob.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksjob
-Version: 0.2.4
+Version: 0.2.5
 Summary: Asynchronous and distributed scheduling of Ewoks workflows from python
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
 Project-URL: Documentation, https://ewoksjob.readthedocs.io/
```

### Comparing `ewoksjob-0.2.4/src/ewoksjob.egg-info/SOURCES.txt` & `ewoksjob-0.2.5/src/ewoksjob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.2.4/src/ewoksjob.egg-info/requires.txt` & `ewoksjob-0.2.5/src/ewoksjob.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 [:python_version < "3.8"]
 importlib-metadata<5.0
 
 [beacon]
 blissdata
 
 [blissworker]
-ewokscore>=0.3.2
-ewoks>=0.1.5
+ewokscore>=0.5
+ewoks>=0.3
 redis<5
 blissdata
 pyslurmutils>=0.1.0rc
 gevent
 flower
 ewoks[esrf-data-portal]
 
 [dev]
-ewokscore>=0.3.2
-ewoks>=0.1.5
+ewokscore>=0.5
+ewoks>=0.3
 redis<5
 blissdata
 pyslurmutils>=0.1.0rc
 gevent
 flower
 ewoks[esrf-data-portal]
 sqlalchemy<2
@@ -32,16 +32,16 @@
 pytest-celery
 pytest-redis
 pytest-mock
 black>=22
 flake8>=4
 
 [doc]
-ewokscore>=0.3.2
-ewoks>=0.1.5
+ewokscore>=0.5
+ewoks>=0.3
 redis<5
 sphinx>=4.5
 sphinx-autodoc-typehints>=1.16
 
 [monitor]
 flower
 
@@ -52,24 +52,24 @@
 pyslurmutils>=0.1.0rc
 gevent
 
 [sql]
 sqlalchemy<2
 
 [test]
-ewokscore>=0.3.2
-ewoks>=0.1.5
+ewokscore>=0.5
+ewoks>=0.3
 redis<5
 blissdata
 pyslurmutils>=0.1.0rc
 gevent
 flower
 ewoks[esrf-data-portal]
 sqlalchemy<2
 pytest>=7
 pytest-celery
 pytest-redis
 pytest-mock
 
 [worker]
-ewokscore>=0.3.2
-ewoks>=0.1.5
+ewokscore>=0.5
+ewoks>=0.3
```

