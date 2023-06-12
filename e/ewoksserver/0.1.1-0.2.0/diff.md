# Comparing `tmp/ewoksserver-0.1.1.tar.gz` & `tmp/ewoksserver-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksserver-0.1.1.tar", last modified: Fri Jun  9 17:42:18 2023, max compression
+gzip compressed data, was "dist/ewoksserver-0.2.0.tar", last modified: Mon Jun 12 17:22:04 2023, max compression
```

## Comparing `ewoksserver-0.1.1.tar` & `ewoksserver-0.2.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2198 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1468 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1445 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-09 17:39:50.000000 ewoksserver-0.1.1/src/ewoksserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 17:42:11.000000 ewoksserver-0.1.1/src/ewoksserver/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/events/ewoks_events.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/events/websocket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver/resources/
--rw-rw-rw-   0 root         (0) root         (0)      731 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9807 2023-06-09 17:28:45.000000 ewoksserver-0.1.1/src/ewoksserver/resources/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver/resources/binary/
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/binary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/binary/icons.py
--rw-rw-rw-   0 root         (0) root         (0)     3834 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/binary/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     3472 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/binary/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 17:42:11.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/icons/default.png
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/icons/graphInput.svg
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/icons/graphOutput.svg
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/icons/sum.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 17:42:11.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumlist.SumList.json
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumtask.SumTask.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 17:42:11.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12315 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/data/workflows/demo.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver/resources/events/
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/events/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver/resources/json/
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/json/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4691 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/json/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     3043 2023-06-09 17:28:45.000000 ewoksserver-0.1.1/src/ewoksserver/resources/json/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3332 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/json/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3371 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/json/workflows.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/resources/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6379 2023-06-09 17:41:02.000000 ewoksserver-0.1.1/src/ewoksserver/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 17:42:11.000000 ewoksserver-0.1.1/src/ewoksserver/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3053 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/tests/data/icon1.png
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/tests/data/icon1.svg
--rw-rw-rw-   0 root         (0) root         (0)     1698 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/tests/data/icon2.png
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/tests/data/icon2.svg
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/tests/dummy_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2040 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/tests/test_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3137 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/tests/test_events.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/tests/test_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2612 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/tests/test_icons.py
--rw-rw-rw-   0 root         (0) root         (0)     5797 2023-06-09 17:28:45.000000 ewoksserver-0.1.1/src/ewoksserver/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/tests/test_websocket_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     4013 2023-06-09 07:03:08.000000 ewoksserver-0.1.1/src/ewoksserver/tests/test_workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2198 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2221 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      360 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-09 17:42:17.000000 ewoksserver-0.1.1/src/ewoksserver.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1468 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-12 17:20:31.000000 ewoksserver-0.2.0/src/ewoksserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:21:58.000000 ewoksserver-0.2.0/src/ewoksserver/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/events/ewoks_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/events/websocket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9845 2023-06-12 15:39:48.000000 ewoksserver-0.2.0/src/ewoksserver/resources/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/binary/
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/binary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/binary/icons.py
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/binary/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3472 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/binary/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:21:58.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/default.png
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/graphInput.svg
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/graphOutput.svg
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/sum.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:21:58.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumlist.SumList.json
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/tasks/ewokscore.tests.examples.tasks.sumtask.SumTask.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:21:58.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12315 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/data/workflows/demo.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/events/
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/events/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/resources/json/
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/json/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4691 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/json/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     4256 2023-06-12 15:39:48.000000 ewoksserver-0.2.0/src/ewoksserver/resources/json/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3332 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/json/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3371 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/json/workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/resources/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7568 2023-06-12 15:39:48.000000 ewoksserver-0.2.0/src/ewoksserver/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:21:58.000000 ewoksserver-0.2.0/src/ewoksserver/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3053 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/data/icon1.png
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/data/icon1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/data/icon2.png
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/data/icon2.svg
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/dummy_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3137 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_icons.py
+-rw-rw-rw-   0 root         (0) root         (0)     5956 2023-06-12 15:39:48.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_websocket_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2023-06-12 07:03:10.000000 ewoksserver-0.2.0/src/ewoksserver/tests/test_workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2221 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 17:22:04.000000 ewoksserver-0.2.0/src/ewoksserver.egg-info/top_level.txt
```

### Comparing `ewoksserver-0.1.1/LICENSE.md` & `ewoksserver-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/PKG-INFO` & `ewoksserver-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksserver
-Version: 0.1.1
+Version: 0.2.0
 Summary: Backend for ewoksweb
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Author: ESRF
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Project-URL: Documentation, https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksserver
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver/issues
```

### Comparing `ewoksserver-0.1.1/README.md` & `ewoksserver-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/setup.cfg` & `ewoksserver-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 	flask
 	flask-restful
 	flask-cors
 	flask-socketio <=5.2
 	flask-apispec
 	werkzeug <2.3  # until flask-socketio issue #1982 is solved
 	simple-websocket
-	ewokscore >=0.4.3
-	ewoksjob[worker]
+	ewoksjob[worker] >=0.2.5
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = *.png, *.svg, *.json
 
@@ -45,14 +44,15 @@
 	pytest >=7
 	pytest-celery
 	sqlalchemy
 dev = 
 	%(test)s
 	black >=22
 	flake8 >=4
+	ewokscore >=0.5
 doc = 
 	%(test)s
 	sphinx >=4.5
 	sphinx-autodoc-typehints >=1.16
 	sphinxcontrib-redoc
 
 [options.entry_points]
```

### Comparing `ewoksserver-0.1.1/src/ewoksserver/events/ewoks_events.py` & `ewoksserver-0.2.0/src/ewoksserver/events/ewoks_events.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/events/websocket.py` & `ewoksserver-0.2.0/src/ewoksserver/events/websocket.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/resources/__init__.py` & `ewoksserver-0.2.0/src/ewoksserver/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/resources/api.py` & `ewoksserver-0.2.0/src/ewoksserver/resources/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 
 class EwoksTaskListSchema(Schema):
     items = fields.List(fields.Nested(EwoksTaskSchema()))
 
 
 class DiscoverSchema(Schema):
-    modules = fields.List(fields.Str)
+    modules = fields.List(fields.Str, dump_default=None, load_default=None)
 
 
 class EwoksEventSchema(Schema):
     host_name = fields.Str(required=True)
     process_id = fields.Int(required=True)
     user_name = fields.Str(required=True)
     job_id = fields.Str(required=True)
```

### Comparing `ewoksserver-0.1.1/src/ewoksserver/resources/binary/icons.py` & `ewoksserver-0.2.0/src/ewoksserver/resources/binary/icons.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/resources/binary/resource.py` & `ewoksserver-0.2.0/src/ewoksserver/resources/binary/resource.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/resources/binary/utils.py` & `ewoksserver-0.2.0/src/ewoksserver/resources/binary/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/resources/data/icons/default.png` & `ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/default.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/resources/data/icons/sum.png` & `ewoksserver-0.2.0/src/ewoksserver/resources/data/icons/sum.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/resources/data/workflows/demo.json` & `ewoksserver-0.2.0/src/ewoksserver/resources/data/workflows/demo.json`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/resources/events/resource.py` & `ewoksserver-0.2.0/src/ewoksserver/resources/events/resource.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/resources/json/__init__.py` & `ewoksserver-0.2.0/src/ewoksserver/resources/json/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/resources/json/resource.py` & `ewoksserver-0.2.0/src/ewoksserver/resources/json/resource.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/resources/json/utils.py` & `ewoksserver-0.2.0/src/ewoksserver/resources/json/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/resources/json/workflows.py` & `ewoksserver-0.2.0/src/ewoksserver/resources/json/workflows.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/server.py` & `ewoksserver-0.2.0/src/ewoksserver/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import sys
 import json
 from pprint import pformat
-from typing import Optional, Tuple
+from typing import Optional, Tuple, ContextManager, Dict
 
 import argparse
 import logging
-from contextlib import contextmanager
+from contextlib import contextmanager, ExitStack
 
 import flask
 from flask_cors import CORS
 from flask_socketio import SocketIO
 from flask_restful import Api
 from flask_apispec import FlaskApiSpec
 
@@ -26,16 +26,17 @@
 
 
 try:
     from ewoksweb.serverutils import get_test_config
 except ImportError:
     get_test_config = None
 
-
 from .resources import add_resources
+from .resources.json import utils as resource_utils
+from .resources.json.tasks import discover_tasks
 from .events.websocket import add_events
 
 
 def create_app(**config) -> Tuple[flask.Flask, Api, FlaskApiSpec]:
     app = flask.Flask(__name__, static_folder=get_static_root(), static_url_path="")
     CORS(app)
     configure_app(app, **config)
@@ -125,32 +126,52 @@
     if save_spec_dir:
         os.makedirs(save_spec_dir, exist_ok=True)
     with open(filename, "w") as f:
         json.dump(apidoc.spec.to_dict(), f)
 
 
 def run_app(
-    app: flask.Flask, socketio: Optional[SocketIO] = None, port: int = 5000
+    app: flask.Flask,
+    socketio: Optional[SocketIO] = None,
+    port: int = 5000,
+    init_context: Optional[ContextManager] = None,
 ) -> None:
-    with run_context(app):
+    with run_context(app, init_context=init_context):
         if socketio is None:
             app.run(port=port)
         else:
             # allow_unsafe_werkzeug=True, see MR1877
             socketio.run(app, port=port)
 
 
 @contextmanager
-def run_context(app: flask.Flask):
-    with app.app_context():
+def run_context(
+    app: flask.Flask,
+    init_context: Optional[ContextManager] = None,
+    local_pool_options: Optional[Dict] = None,
+):
+    with ExitStack() as stack:
+        ctx = app.app_context()
+        stack.enter_context(ctx)
         if app.config.get("CELERY") is None:
-            with pool_context():
-                yield
-        else:
-            yield
+            if local_pool_options is None:
+                local_pool_options = dict()
+            ctx = pool_context(**local_pool_options)
+            stack.enter_context(ctx)
+        if init_context is not None:
+            ctx = init_context(app)
+            stack.enter_context(ctx)
+        yield
+
+
+def rediscover_tasks(app: flask.Flask):
+    tasks = discover_tasks(app)
+    root_url = resource_utils.root_url(app.config.get("RESOURCE_DIRECTORY"), "tasks")
+    for resource in tasks:
+        resource_utils.save_resource(root_url, resource["task_identifier"], resource)
 
 
 def main(argv=None):
     if argv is None:
         argv = sys.argv
 
     parser = argparse.ArgumentParser(description="REST API for Ewoks")
@@ -200,14 +221,20 @@
         help="Without websocket events",
     )
     parser.add_argument(
         "--frontend-tests",
         action="store_true",
         help="Load frontend test configuration",
     )
+    parser.add_argument(
+        "-r",
+        "--rediscover-tasks",
+        action="store_true",
+        help="Run task discovery on start up",
+    )
 
     args = parser.parse_args(argv[1:])
     log_level = getattr(logging, args.log_level)
 
     if args.frontend_tests:
         if get_test_config is None:
             raise RuntimeError("ewoksweb is not installed")
@@ -215,20 +242,27 @@
 
     app, _, apidoc = create_app(
         configuration=args.configuration, resource_directory=args.resource_directory
     )
     if args.spec_filename:
         save_apidoc(apidoc, args.spec_filename)
         return
+
     if args.without_events:
         socketio = None
     else:
         socketio = add_socket(app)
     set_log_level(log_level=log_level)
 
+    @contextmanager
+    def init_context(app):
+        if args.rediscover_tasks:
+            rediscover_tasks(app)
+        yield
+
     print_config(app)
     print_serve_message(app, port=args.port)
-    run_app(app, socketio=socketio, port=args.port)
+    run_app(app, socketio=socketio, port=args.port, init_context=init_context)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `ewoksserver-0.1.1/src/ewoksserver/tests/conftest.py` & `ewoksserver-0.2.0/src/ewoksserver/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/tests/data/icon1.png` & `ewoksserver-0.2.0/src/ewoksserver/tests/data/icon1.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/tests/data/icon2.png` & `ewoksserver-0.2.0/src/ewoksserver/tests/data/icon2.png`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/tests/test_data.py` & `ewoksserver-0.2.0/src/ewoksserver/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/tests/test_events.py` & `ewoksserver-0.2.0/src/ewoksserver/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/tests/test_execute.py` & `ewoksserver-0.2.0/src/ewoksserver/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/tests/test_icons.py` & `ewoksserver-0.2.0/src/ewoksserver/tests/test_icons.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/tests/test_tasks.py` & `ewoksserver-0.2.0/src/ewoksserver/tests/test_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,19 @@
     assert response.status_code == 200, data
 
     response = rest_client.post("/tasks/discover", json={"modules": ["not_a_module"]})
     data = response.get_json()
     assert response.status_code == 404, data
     assert "No module named" in data["message"]
 
+    response = rest_client.post("/tasks/discover")
+    data = response.get_json()
+    assert response.status_code == 200, data
+    assert data["identifiers"]
+
 
 def test_task_descriptions(rest_client, default_task_identifiers):
     response = rest_client.get("/tasks/descriptions")
     data = response.get_json()
     assert response.status_code == 200
     default_descriptions = [
         desc
```

### Comparing `ewoksserver-0.1.1/src/ewoksserver/tests/test_websocket_connection.py` & `ewoksserver-0.2.0/src/ewoksserver/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver/tests/test_workflows.py` & `ewoksserver-0.2.0/src/ewoksserver/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `ewoksserver-0.1.1/src/ewoksserver.egg-info/PKG-INFO` & `ewoksserver-0.2.0/src/ewoksserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksserver
-Version: 0.1.1
+Version: 0.2.0
 Summary: Backend for ewoksweb
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Author: ESRF
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver
 Project-URL: Documentation, https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksserver
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoks/ewoksserver/issues
```

### Comparing `ewoksserver-0.1.1/src/ewoksserver.egg-info/SOURCES.txt` & `ewoksserver-0.2.0/src/ewoksserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

