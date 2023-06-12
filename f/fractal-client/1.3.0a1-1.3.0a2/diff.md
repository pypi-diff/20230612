# Comparing `tmp/fractal_client-1.3.0a1.tar.gz` & `tmp/fractal_client-1.3.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_client-1.3.0a1.tar", max compression
+gzip compressed data, was "fractal_client-1.3.0a2.tar", max compression
```

## Comparing `fractal_client-1.3.0a1.tar` & `fractal_client-1.3.0a2.tar`

### file list

```diff
@@ -1,96 +1,106 @@
--rw-r--r--   0        0        0     1576 2023-05-09 19:58:57.312677 fractal_client-1.3.0a1/LICENSE
--rw-r--r--   0        0        0     2619 2023-05-09 19:58:57.312677 fractal_client-1.3.0a1/README.md
--rw-r--r--   0        0        0       24 2023-06-12 06:40:22.416526 fractal_client-1.3.0a1/fractal/__init__.py
--rw-r--r--   0        0        0      124 2023-05-26 13:31:24.681931 fractal_client-1.3.0a1/fractal/__main__.py
--rw-r--r--   0        0        0     3448 2023-05-26 13:44:53.339222 fractal_client-1.3.0a1/fractal/authclient.py
--rw-r--r--   0        0        0     3773 2023-05-30 07:19:20.910204 fractal_client-1.3.0a1/fractal/client.py
--rw-r--r--   0        0        0    12249 2023-06-12 06:40:09.560661 fractal_client-1.3.0a1/fractal/cmd/__init__.py
--rw-r--r--   0        0        0     6863 2023-06-05 08:33:35.839631 fractal_client-1.3.0a1/fractal/cmd/_aux_task_caching.py
--rw-r--r--   0        0        0     5795 2023-06-06 12:51:00.225986 fractal_client-1.3.0a1/fractal/cmd/_dataset.py
--rw-r--r--   0        0        0     5115 2023-06-06 12:51:00.229986 fractal_client-1.3.0a1/fractal/cmd/_job.py
--rw-r--r--   0        0        0     4031 2023-06-06 12:51:00.229986 fractal_client-1.3.0a1/fractal/cmd/_project.py
--rw-r--r--   0        0        0     5954 2023-06-12 06:40:09.560661 fractal_client-1.3.0a1/fractal/cmd/_task.py
--rw-r--r--   0        0        0     4620 2023-06-06 12:51:00.229986 fractal_client-1.3.0a1/fractal/cmd/_user.py
--rw-r--r--   0        0        0     9027 2023-06-12 06:40:09.560661 fractal_client-1.3.0a1/fractal/cmd/_workflow.py
--rw-r--r--   0        0        0       42 2023-02-21 08:49:25.750218 fractal_client-1.3.0a1/fractal/common/.git
--rw-r--r--   0        0        0      717 2023-03-06 13:52:20.997699 fractal_client-1.3.0a1/fractal/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-21 08:49:27.594201 fractal_client-1.3.0a1/fractal/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-03-06 13:52:21.001699 fractal_client-1.3.0a1/fractal/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-21 08:49:27.594201 fractal_client-1.3.0a1/fractal/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-03-06 13:52:21.001699 fractal_client-1.3.0a1/fractal/common/README.md
--rw-r--r--   0        0        0        0 2023-02-21 08:49:27.594201 fractal_client-1.3.0a1/fractal/common/__init__.py
--rw-r--r--   0        0        0      149 2023-02-21 10:13:04.505672 fractal_client-1.3.0a1/fractal/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      147 2023-03-16 09:04:47.705157 fractal_client-1.3.0a1/fractal/common/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       57 2023-05-26 06:48:59.488787 fractal_client-1.3.0a1/fractal/common/requirements.txt
--rw-r--r--   0        0        0      614 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/schemas/__init__.py
--rw-r--r--   0        0        0      411 2023-05-25 12:32:05.945818 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      372 2023-03-16 09:04:47.705157 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      490 2023-03-03 14:13:42.839064 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1753 2023-04-20 07:56:22.895496 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1251 2023-03-16 09:04:47.793156 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc
--rw-r--r--   0        0        0     1610 2023-05-26 06:49:58.096032 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2027 2023-03-16 09:04:47.705157 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc
--rw-r--r--   0        0        0     3459 2023-05-25 12:32:06.081816 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     3515 2023-03-16 09:04:47.797156 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc
--rw-r--r--   0        0        0     3537 2023-05-26 06:49:58.132032 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     3711 2023-03-16 09:04:47.797156 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/project.cpython-39.pyc
--rw-r--r--   0        0        0     1165 2023-05-26 06:49:58.136032 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1185 2023-03-16 09:04:47.801156 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/state.cpython-39.pyc
--rw-r--r--   0        0        0     3109 2023-05-26 06:49:58.136032 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     4994 2023-03-16 09:04:47.805156 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/task.cpython-39.pyc
--rw-r--r--   0        0        0     3098 2023-05-25 12:32:06.097816 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc
--rw-r--r--   0        0        0     1202 2023-05-25 12:32:06.097816 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1024 2023-03-16 09:04:47.809156 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/user.cpython-39.pyc
--rw-r--r--   0        0        0     3882 2023-05-26 06:49:58.328029 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     1616 2023-04-06 11:30:39.096144 fractal_client-1.3.0a1/fractal/common/schemas/_validators.py
--rw-r--r--   0        0        0     1117 2023-05-26 06:48:59.488787 fractal_client-1.3.0a1/fractal/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     2769 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/schemas/manifest.py
--rw-r--r--   0        0        0     2483 2023-05-26 06:48:59.488787 fractal_client-1.3.0a1/fractal/common/schemas/project.py
--rw-r--r--   0        0        0      673 2023-05-26 06:48:59.488787 fractal_client-1.3.0a1/fractal/common/schemas/state.py
--rw-r--r--   0        0        0     2872 2023-05-26 06:48:59.488787 fractal_client-1.3.0a1/fractal/common/schemas/task.py
--rw-r--r--   0        0        0     2741 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/schemas/task_collection.py
--rw-r--r--   0        0        0     1216 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/schemas/user.py
--rw-r--r--   0        0        0     2457 2023-05-26 06:48:59.488787 fractal_client-1.3.0a1/fractal/common/schemas/workflow.py
--rw-r--r--   0        0        0      415 2023-03-06 13:52:30.189594 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      415 2023-03-07 09:47:31.002846 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      415 2023-04-20 07:57:03.191274 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1578 2023-03-06 13:52:30.221594 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1578 2023-03-07 09:47:31.038845 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      606 2023-05-15 11:49:28.546463 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3382 2023-03-15 10:53:32.644401 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3382 2023-04-20 07:57:03.471272 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      859 2023-03-06 13:52:30.469591 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      859 2023-03-07 09:47:31.354842 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      859 2023-04-20 07:57:03.471272 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-06 13:52:30.469591 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1164 2023-04-20 07:56:23.111495 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1164 2023-04-20 07:57:03.471272 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1763 2023-03-06 14:08:06.438014 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1763 2023-03-07 09:47:31.358842 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1763 2023-04-20 07:57:03.471272 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2222 2023-03-06 13:52:30.473591 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2222 2023-03-07 09:47:31.358842 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2792 2023-05-25 12:32:06.297813 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1224 2023-05-25 12:32:06.297813 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1317 2023-03-06 13:52:30.473591 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2213 2023-04-20 07:56:23.115495 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2671 2023-05-25 12:32:06.301813 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2579 2023-03-06 14:43:41.164713 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3032 2023-04-20 07:56:23.115495 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2911 2023-05-15 11:49:28.882460 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-03-06 13:52:21.001699 fractal_client-1.3.0a1/fractal/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-05-11 16:07:56.531485 fractal_client-1.3.0a1/fractal/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-03-14 13:42:31.592919 fractal_client-1.3.0a1/fractal/common/tests/test_dataset.py
--rw-r--r--   0        0        0      541 2023-03-06 13:52:21.001699 fractal_client-1.3.0a1/fractal/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-04-06 11:30:39.096144 fractal_client-1.3.0a1/fractal/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-03-06 14:07:44.150418 fractal_client-1.3.0a1/fractal/common/tests/test_state.py
--rw-r--r--   0        0        0     1190 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/tests/test_task.py
--rw-r--r--   0        0        0      773 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/tests/test_task_collection.py
--rw-r--r--   0        0        0     1499 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-05-11 16:07:56.531485 fractal_client-1.3.0a1/fractal/common/tests/test_workflow.py
--rw-r--r--   0        0        0     1285 2023-05-12 13:33:57.004876 fractal_client-1.3.0a1/fractal/config.py
--rw-r--r--   0        0        0     1609 2023-05-09 19:58:57.316677 fractal_client-1.3.0a1/fractal/interface.py
--rw-r--r--   0        0        0    23230 2023-06-12 06:40:09.560661 fractal_client-1.3.0a1/fractal/parser.py
--rw-r--r--   0        0        0     1265 2023-05-09 19:58:57.316677 fractal_client-1.3.0a1/fractal/response.py
--rw-r--r--   0        0        0     1825 2023-06-12 06:40:22.416526 fractal_client-1.3.0a1/pyproject.toml
--rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 fractal_client-1.3.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1576 2023-05-09 19:58:57.312677 fractal_client-1.3.0a2/LICENSE
+-rw-r--r--   0        0        0     2484 2023-06-12 14:10:42.230233 fractal_client-1.3.0a2/README.md
+-rw-r--r--   0        0        0       24 2023-06-12 14:15:35.227390 fractal_client-1.3.0a2/fractal/__init__.py
+-rw-r--r--   0        0        0      124 2023-05-26 13:31:24.681931 fractal_client-1.3.0a2/fractal/__main__.py
+-rw-r--r--   0        0        0     3448 2023-05-26 13:44:53.339222 fractal_client-1.3.0a2/fractal/authclient.py
+-rw-r--r--   0        0        0     3773 2023-05-30 07:19:20.910204 fractal_client-1.3.0a2/fractal/client.py
+-rw-r--r--   0        0        0    12216 2023-06-12 14:05:40.809583 fractal_client-1.3.0a2/fractal/cmd/__init__.py
+-rw-r--r--   0        0        0     6863 2023-06-05 08:33:35.839631 fractal_client-1.3.0a2/fractal/cmd/_aux_task_caching.py
+-rw-r--r--   0        0        0     5795 2023-06-06 12:51:00.225986 fractal_client-1.3.0a2/fractal/cmd/_dataset.py
+-rw-r--r--   0        0        0     5115 2023-06-06 12:51:00.229986 fractal_client-1.3.0a2/fractal/cmd/_job.py
+-rw-r--r--   0        0        0     4031 2023-06-06 12:51:00.229986 fractal_client-1.3.0a2/fractal/cmd/_project.py
+-rw-r--r--   0        0        0     6139 2023-06-12 14:05:40.809583 fractal_client-1.3.0a2/fractal/cmd/_task.py
+-rw-r--r--   0        0        0     4620 2023-06-06 12:51:00.229986 fractal_client-1.3.0a2/fractal/cmd/_user.py
+-rw-r--r--   0        0        0     9027 2023-06-12 06:40:09.560661 fractal_client-1.3.0a2/fractal/cmd/_workflow.py
+-rw-r--r--   0        0        0       42 2023-02-21 08:49:25.750218 fractal_client-1.3.0a2/fractal/common/.git
+-rw-r--r--   0        0        0      717 2023-03-06 13:52:20.997699 fractal_client-1.3.0a2/fractal/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-21 08:49:27.594201 fractal_client-1.3.0a2/fractal/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-03-06 13:52:21.001699 fractal_client-1.3.0a2/fractal/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-21 08:49:27.594201 fractal_client-1.3.0a2/fractal/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-03-06 13:52:21.001699 fractal_client-1.3.0a2/fractal/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-21 08:49:27.594201 fractal_client-1.3.0a2/fractal/common/__init__.py
+-rw-r--r--   0        0        0      149 2023-02-21 10:13:04.505672 fractal_client-1.3.0a2/fractal/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      147 2023-03-16 09:04:47.705157 fractal_client-1.3.0a2/fractal/common/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0       57 2023-05-26 06:48:59.488787 fractal_client-1.3.0a2/fractal/common/requirements.txt
+-rw-r--r--   0        0        0      614 2023-05-25 12:31:57.653940 fractal_client-1.3.0a2/fractal/common/schemas/__init__.py
+-rw-r--r--   0        0        0      411 2023-05-25 12:32:05.945818 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      372 2023-03-16 09:04:47.705157 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      490 2023-03-03 14:13:42.839064 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1753 2023-04-20 07:56:22.895496 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1251 2023-03-16 09:04:47.793156 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc
+-rw-r--r--   0        0        0     1610 2023-05-26 06:49:58.096032 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2027 2023-03-16 09:04:47.705157 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc
+-rw-r--r--   0        0        0     4068 2023-06-12 13:01:03.378002 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     3515 2023-03-16 09:04:47.797156 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc
+-rw-r--r--   0        0        0     3537 2023-05-26 06:49:58.132032 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     3711 2023-03-16 09:04:47.797156 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/project.cpython-39.pyc
+-rw-r--r--   0        0        0     1165 2023-05-26 06:49:58.136032 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1185 2023-03-16 09:04:47.801156 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/state.cpython-39.pyc
+-rw-r--r--   0        0        0     2705 2023-06-12 13:01:03.386002 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     4994 2023-03-16 09:04:47.805156 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/task.cpython-39.pyc
+-rw-r--r--   0        0        0     3292 2023-06-12 13:01:03.390002 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1202 2023-05-25 12:32:06.097816 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1024 2023-03-16 09:04:47.809156 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/user.cpython-39.pyc
+-rw-r--r--   0        0        0     3882 2023-05-26 06:49:58.328029 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     1616 2023-04-06 11:30:39.096144 fractal_client-1.3.0a2/fractal/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1117 2023-05-26 06:48:59.488787 fractal_client-1.3.0a2/fractal/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     3479 2023-06-12 10:22:50.369047 fractal_client-1.3.0a2/fractal/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2483 2023-05-26 06:48:59.488787 fractal_client-1.3.0a2/fractal/common/schemas/project.py
+-rw-r--r--   0        0        0      673 2023-05-26 06:48:59.488787 fractal_client-1.3.0a2/fractal/common/schemas/state.py
+-rw-r--r--   0        0        0     2578 2023-06-12 10:22:50.369047 fractal_client-1.3.0a2/fractal/common/schemas/task.py
+-rw-r--r--   0        0        0     2935 2023-06-12 10:22:50.369047 fractal_client-1.3.0a2/fractal/common/schemas/task_collection.py
+-rw-r--r--   0        0        0     1216 2023-05-25 12:31:57.653940 fractal_client-1.3.0a2/fractal/common/schemas/user.py
+-rw-r--r--   0        0        0     2457 2023-05-26 06:48:59.488787 fractal_client-1.3.0a2/fractal/common/schemas/workflow.py
+-rw-r--r--   0        0        0      415 2023-03-06 13:52:30.189594 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      415 2023-03-07 09:47:31.002846 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      415 2023-04-20 07:57:03.191274 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      415 2023-06-12 13:01:14.929878 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     1578 2023-03-06 13:52:30.221594 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1578 2023-03-07 09:47:31.038845 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      606 2023-05-15 11:49:28.546463 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      606 2023-06-12 13:01:14.961878 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     3382 2023-03-15 10:53:32.644401 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3382 2023-04-20 07:57:03.471272 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3382 2023-06-12 13:01:15.169875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0      859 2023-03-06 13:52:30.469591 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      859 2023-03-07 09:47:31.354842 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1241 2023-06-12 13:01:03.562000 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1241 2023-06-12 13:01:15.169875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     2236 2023-03-06 13:52:30.469591 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1164 2023-04-20 07:56:23.111495 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1164 2023-04-20 07:57:03.471272 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1164 2023-06-12 13:01:15.169875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     1763 2023-03-06 14:08:06.438014 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1763 2023-03-07 09:47:31.358842 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1763 2023-04-20 07:57:03.471272 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1763 2023-06-12 13:01:15.173875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     2222 2023-03-06 13:52:30.473591 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2222 2023-03-07 09:47:31.358842 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2792 2023-05-25 12:32:06.297813 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2792 2023-06-12 13:01:15.173875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     1335 2023-06-12 13:01:03.566000 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1335 2023-06-12 13:01:15.177875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     1317 2023-03-06 13:52:30.473591 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2213 2023-04-20 07:56:23.115495 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2671 2023-05-25 12:32:06.301813 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2671 2023-06-12 13:01:15.177875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     2579 2023-03-06 14:43:41.164713 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3032 2023-04-20 07:56:23.115495 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2911 2023-05-15 11:49:28.882460 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2911 2023-06-12 13:01:15.177875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0      139 2023-03-06 13:52:21.001699 fractal_client-1.3.0a2/fractal/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-05-11 16:07:56.531485 fractal_client-1.3.0a2/fractal/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-03-14 13:42:31.592919 fractal_client-1.3.0a2/fractal/common/tests/test_dataset.py
+-rw-r--r--   0        0        0     1420 2023-06-12 10:22:50.369047 fractal_client-1.3.0a2/fractal/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-04-06 11:30:39.096144 fractal_client-1.3.0a2/fractal/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-03-06 14:07:44.150418 fractal_client-1.3.0a2/fractal/common/tests/test_state.py
+-rw-r--r--   0        0        0     1190 2023-05-25 12:31:57.653940 fractal_client-1.3.0a2/fractal/common/tests/test_task.py
+-rw-r--r--   0        0        0      968 2023-06-12 10:22:50.369047 fractal_client-1.3.0a2/fractal/common/tests/test_task_collection.py
+-rw-r--r--   0        0        0     1499 2023-05-25 12:31:57.653940 fractal_client-1.3.0a2/fractal/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-05-11 16:07:56.531485 fractal_client-1.3.0a2/fractal/common/tests/test_workflow.py
+-rw-r--r--   0        0        0     1285 2023-05-12 13:33:57.004876 fractal_client-1.3.0a2/fractal/config.py
+-rw-r--r--   0        0        0     1609 2023-05-09 19:58:57.316677 fractal_client-1.3.0a2/fractal/interface.py
+-rw-r--r--   0        0        0    23055 2023-06-12 14:05:40.809583 fractal_client-1.3.0a2/fractal/parser.py
+-rw-r--r--   0        0        0     1265 2023-05-09 19:58:57.316677 fractal_client-1.3.0a2/fractal/response.py
+-rw-r--r--   0        0        0     1851 2023-06-12 14:15:35.227390 fractal_client-1.3.0a2/pyproject.toml
+-rw-r--r--   0        0        0     3329 1970-01-01 00:00:00.000000 fractal_client-1.3.0a2/PKG-INFO
```

### Comparing `fractal_client-1.3.0a1/LICENSE` & `fractal_client-1.3.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/README.md` & `fractal_client-1.3.0a2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
 See https://fractal-analytics-platform.github.io/fractal.
 
 # Contributors and license
 
 Unless otherwise stated in each individual module, all Fractal components are released according to a BSD 3-Clause License, and Copyright is with Friedrich Miescher Institute for Biomedical Research and University of Zurich.
 
-Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa) & [@jacopo-exact](https://github.com/jacopo-exact) from [eXact lab S.r.l.](exact-lab.it).
+Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [eXact lab S.r.l.](exact-lab.it).
```

### Comparing `fractal_client-1.3.0a1/fractal/authclient.py` & `fractal_client-1.3.0a2/fractal/authclient.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/client.py` & `fractal_client-1.3.0a2/fractal/client.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/cmd/__init__.py` & `fractal_client-1.3.0a2/fractal/cmd/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,15 @@
         iface = await get_task_list(client)
     elif subcmd == "collect":
         parameters = [
             "package",
             "package_version",
             "python_version",
             "package_extras",
+            "pinned_dependency",
         ]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = await task_collect_pip(client, batch=batch, **function_kwargs)
     elif subcmd == "check-collection":
         parameters = ["state_id", "include_logs", "do_not_separate_logs"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = await task_collection_check(client, **function_kwargs)
@@ -158,30 +159,28 @@
         parameters = [
             "name",
             "command",
             "source",
             "input_type",
             "output_type",
             "version",
-            "default_args_file",
             "meta_file",
         ]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = await post_task(client, batch=batch, **function_kwargs)
     elif subcmd == "edit":
         parameters = [
             "id",
             "name",
             "version",
             "new_name",
             "new_command",
             "new_input_type",
             "new_output_type",
             "new_version",
-            "default_args_file",
             "meta_file",
         ]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = await patch_task(client, **function_kwargs)
     elif subcmd == "delete":
         parameters = ["id", "name", "version"]
         function_kwargs = get_kwargs(parameters, kwargs)
```

### Comparing `fractal_client-1.3.0a1/fractal/cmd/_aux_task_caching.py` & `fractal_client-1.3.0a2/fractal/cmd/_aux_task_caching.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/cmd/_dataset.py` & `fractal_client-1.3.0a2/fractal/cmd/_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/cmd/_job.py` & `fractal_client-1.3.0a2/fractal/cmd/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/cmd/_project.py` & `fractal_client-1.3.0a2/fractal/cmd/_project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/cmd/_task.py` & `fractal_client-1.3.0a2/fractal/cmd/_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,25 +27,38 @@
 async def task_collect_pip(
     client: AuthClient,
     *,
     package: str,
     package_version: Optional[str] = None,
     python_version: Optional[str] = None,
     package_extras: Optional[str] = None,
+    pinned_dependency: Optional[list[str]] = None,
     batch: bool = False,
 ) -> BaseInterface:
 
     # Construct TaskCollectPip object
     attributes = dict(package=package)
     if package_version:
         attributes["package_version"] = package_version
     if python_version:
         attributes["python_version"] = python_version
     if package_extras:
         attributes["package_extras"] = package_extras
+    if pinned_dependency:
+        for pin in pinned_dependency:
+            if len(pin.split("=")) != 2:
+                logging.error(
+                    f"Invalid pin: {pin}.\nPins must be written as "
+                    "'--pinned-dependency PACKAGE_NAME=PACKAGE_VERSION'"
+                )
+                sys.exit(1)
+        attributes["pinned_package_versions"] = {
+            _name: _version
+            for _name, _version in (p.split("=") for p in pinned_dependency)
+        }
     task_collect = TaskCollectPip(**attributes)
 
     res = await client.post(
         f"{settings.BASE_URL}/task/collect/pip/",
         json=task_collect.dict(exclude_unset=True),
     )
 
@@ -61,15 +74,14 @@
 
 async def task_collection_check(
     client: AuthClient,
     *,
     state_id: int,
     include_logs: bool,
     do_not_separate_logs: bool = False,
-    **kwargs,
 ) -> BaseInterface:
 
     res = await client.get(
         f"{settings.BASE_URL}/task/collect/{state_id}?verbose={include_logs}"
     )
     state = check_response(res, expected_status_code=200, coerce=StateRead)
 
@@ -95,24 +107,20 @@
     *,
     name: str,
     command: str,
     source: str,
     input_type: str = "Any",
     output_type: str = "Any",
     version: Optional[str] = None,
-    default_args_file: Optional[str] = None,
     meta_file: Optional[str] = None,
     batch: bool = False,
 ) -> BaseInterface:
     optionals = {}
     if version:
         optionals["version"] = version
-    if default_args_file:
-        with open(default_args_file, "r") as f:
-            optionals["default_args"] = json.load(f)
     if meta_file:
         with open(meta_file, "r") as f:
             optionals["meta"] = json.load(f)
     payload = TaskCreate(
         name=name,
         command=command,
         source=source,
@@ -136,15 +144,14 @@
     name: Optional[str] = None,
     version: Optional[str] = None,
     new_name: Optional[str] = None,
     new_command: Optional[str] = None,
     new_input_type: Optional[str] = None,
     new_output_type: Optional[str] = None,
     new_version: Optional[str] = None,
-    default_args_file: Optional[str] = None,
     meta_file: Optional[str] = None,
 ) -> BaseInterface:
 
     if id:
         if version:
             logging.error(
                 "Too many arguments: cannot provide both `id` and `version`."
@@ -158,25 +165,22 @@
         except FractalCacheError as e:
             print(e)
             sys.exit(1)
 
     update = {}
     if new_name:
         update["name"] = new_name
-    if new_command:
-        update["command"] = new_command
-    if new_version:
-        update["version"] = new_version
     if new_input_type:
         update["input_type"] = new_input_type
     if new_output_type:
         update["output_type"] = new_output_type
-    if default_args_file:
-        with open(default_args_file, "r") as f:
-            update["default_args"] = json.load(f)
+    if new_command:
+        update["command"] = new_command
+    if new_version:
+        update["version"] = new_version
     if meta_file:
         with open(meta_file, "r") as f:
             update["meta"] = json.load(f)
 
     task_update = TaskUpdate(**update)
     payload = task_update.dict(exclude_unset=True)
     if not payload:
```

### Comparing `fractal_client-1.3.0a1/fractal/cmd/_user.py` & `fractal_client-1.3.0a2/fractal/cmd/_user.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/cmd/_workflow.py` & `fractal_client-1.3.0a2/fractal/cmd/_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/.github/workflows/ci.yml` & `fractal_client-1.3.0a2/fractal/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/.pre-commit-config.yaml` & `fractal_client-1.3.0a2/fractal/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/README.md` & `fractal_client-1.3.0a2/fractal/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__init__.py` & `fractal_client-1.3.0a2/fractal/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 25 12:31:57 2023 UTC, .py size: 2769 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,217 +1,220 @@
-00000000: 6f0d 0d0a 0000 0000 3d55 6f64 d10a 0000  o.......=Uod....
+00000000: 610d 0d0a 0000 0000 9785 f463 010b 0000  a..........c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c02 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c06 6d07 5a07 0100 6400 6406 6c06  d.l.m.Z...d.d.l.
-00000070: 6d08 5a08 0100 6400 6407 6c06 6d09 5a09  m.Z...d.d.l.m.Z.
-00000080: 0100 6408 5a0a 4700 6409 640a 8400 640a  ..d.Z.G.d.d...d.
-00000090: 6507 8303 5a0b 6505 640b 650b 640c 8d02  e...Z.e.d.e.d...
-000000a0: 5a0c 4700 640d 640e 8400 640e 6507 8303  Z.G.d.d...d.e...
-000000b0: 5a0d 4700 640f 6410 8400 6410 650b 8303  Z.G.d.d...d.e...
-000000c0: 5a0e 4700 6411 6412 8400 6412 650d 8303  Z.G.d.d...d.e...
-000000d0: 5a0f 6413 5300 2914 e900 0000 0029 01da  Z.d.S.)......)..
-000000e0: 0450 6174 6829 01da 0341 6e79 2901 da08  .Path)...Any)...
-000000f0: 4f70 7469 6f6e 616c 2901 da07 5479 7065  Optional)...Type
-00000100: 5661 7229 01da 0942 6173 654d 6f64 656c  Var)...BaseModel
-00000110: 2901 da05 4669 656c 6429 01da 0976 616c  )...Field)...val
-00000120: 6964 6174 6f72 2902 da0e 5461 736b 4d61  idator)...TaskMa
-00000130: 6e69 6665 7374 5631 da0a 4d61 6e69 6665  nifestV1..Manife
-00000140: 7374 5631 6300 0000 0000 0000 0000 0000  stV1c...........
-00000150: 0000 0000 0004 0000 0040 0000 0073 6e00  .........@...sn.
-00000160: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-00000170: 6504 6505 6402 3c00 6506 6505 6403 3c00  e.e.d.<.e.e.d.<.
-00000180: 6504 6505 6404 3c00 6504 6505 6405 3c00  e.e.d.<.e.e.d.<.
-00000190: 6507 6508 6406 8d01 5a09 650a 6508 6504  e.e.d...Z.e.e.e.
-000001a0: 650b 6602 1900 1900 6505 6407 3c00 6507  e.f.....e.d.<.e.
-000001b0: 6508 6406 8d01 5a0c 650a 6508 6504 650b  e.d...Z.e.e.e.e.
-000001c0: 6602 1900 1900 6505 6408 3c00 6409 5300  f.....e.d.<.d.S.
-000001d0: 290a da11 5f54 6173 6b4d 616e 6966 6573  )..._TaskManifes
-000001e0: 7442 6173 6561 a503 0000 0a20 2020 2042  tBasea.....    B
-000001f0: 6173 6520 636c 6173 7320 666f 7220 5461  ase class for Ta
-00000200: 736b 4d61 6e69 6665 7374 0a0a 2020 2020  skManifest..    
-00000210: 5265 7072 6573 656e 7473 2061 2074 6173  Represents a tas
-00000220: 6b20 7769 7468 696e 2061 206d 616e 6665  k within a manfe
-00000230: 7374 0a0a 2020 2020 4174 7472 6962 7574  st..    Attribut
-00000240: 6573 3a0a 2020 2020 2020 2020 6e61 6d65  es:.        name
-00000250: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
-00000260: 6520 7461 736b 206e 616d 650a 2020 2020  e task name.    
-00000270: 2020 2020 6578 6563 7574 6162 6c65 3a0a      executable:.
-00000280: 2020 2020 2020 2020 2020 2020 5061 7468              Path
-00000290: 2074 6f20 7468 6520 6578 6563 7574 6162   to the executab
-000002a0: 6c65 2072 656c 6174 6976 6520 746f 2074  le relative to t
-000002b0: 6865 2070 6163 6b61 6765 2072 6f6f 740a  he package root.
-000002c0: 0a20 2020 2020 2020 2020 2020 204e 6f74  .            Not
-000002d0: 653a 2062 7920 7061 636b 6167 6520 726f  e: by package ro
-000002e0: 6f74 2077 6520 6d65 616e 2022 6173 2069  ot we mean "as i
-000002f0: 7420 7769 6c6c 2062 6520 696e 7374 616c  t will be instal
-00000300: 6c65 6422 2e20 4966 2061 0a20 2020 2020  led". If a.     
-00000310: 2020 2020 2020 2070 6163 6b61 6765 2060         package `
-00000320: 506b 6760 2069 6e73 7461 6c6c 7320 696e  Pkg` installs in
-00000330: 2074 6865 2066 6f6c 6465 7220 6070 6b67   the folder `pkg
-00000340: 6020 7468 6520 6578 6563 7574 6162 6c65  ` the executable
-00000350: 0a20 2020 2020 2020 2020 2020 2060 706b  .            `pk
-00000360: 672f 6578 6563 7574 6162 6c65 2e70 7960  g/executable.py`
-00000370: 2c20 7468 6973 2061 7474 7269 6275 7465  , this attribute
-00000380: 206d 7573 7420 636f 6e74 6169 6e20 6f6e   must contain on
-00000390: 6c79 0a20 2020 2020 2020 2020 2020 2060  ly.            `
-000003a0: 6578 6563 7574 6162 6c65 2e70 7960 2e0a  executable.py`..
-000003b0: 2020 2020 2020 2020 696e 7075 745f 7479          input_ty
-000003c0: 7065 3a0a 2020 2020 2020 2020 2020 2020  pe:.            
-000003d0: 5468 6520 696e 7075 7420 7479 7065 2061  The input type a
-000003e0: 6363 6570 7465 6420 6279 2074 6865 2074  ccepted by the t
-000003f0: 6173 6b0a 2020 2020 2020 2020 6f75 7470  ask.        outp
-00000400: 7574 5f74 7970 653a 0a20 2020 2020 2020  ut_type:.       
-00000410: 2020 2020 2054 6865 206f 7574 7075 7420       The output 
-00000420: 7479 7065 2072 6574 7572 6e65 6420 6279  type returned by
-00000430: 2074 6865 2074 6173 6b0a 2020 2020 2020   the task.      
-00000440: 2020 6465 6661 756c 745f 6172 6773 3a0a    default_args:.
-00000450: 2020 2020 2020 2020 2020 2020 416e 2061              An a
-00000460: 7262 6974 7261 7279 2c20 4a53 4f4e 2d73  rbitrary, JSON-s
-00000470: 6572 6961 6c69 7a61 626c 6520 6469 6374  erializable dict
-00000480: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
-00000490: 6720 7468 6520 6465 6661 756c 740a 2020  g the default.  
-000004a0: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
-000004b0: 7465 7273 2074 6861 7420 7769 6c6c 2062  ters that will b
-000004c0: 6520 7061 7373 6564 2074 6f20 7468 6520  e passed to the 
-000004d0: 7461 736b 0a20 2020 2020 2020 206d 6574  task.        met
-000004e0: 613a 0a20 2020 2020 2020 2020 2020 2041  a:.            A
-000004f0: 6464 6974 696f 6e61 6c20 696e 666f 726d  dditional inform
-00000500: 6174 696f 6e20 6162 6f75 7420 7468 6520  ation about the 
-00000510: 7061 636b 6167 652c 2073 7563 6820 6173  package, such as
-00000520: 2068 6173 6820 6f66 2074 6865 0a20 2020   hash of the.   
-00000530: 2020 2020 2020 2020 2065 7865 6375 7461           executa
-00000540: 626c 652c 2073 7065 6369 6669 6320 7275  ble, specific ru
-00000550: 6e74 696d 6520 7265 7175 6972 656d 656e  ntime requiremen
-00000560: 7473 2028 652e 672e 2c20 6e65 6564 5f67  ts (e.g., need_g
-00000570: 7075 3d54 7275 6529 2c0a 2020 2020 2020  pu=True),.      
-00000580: 2020 2020 2020 6574 632e 0a20 2020 20da        etc..    .
-00000590: 046e 616d 65da 0a65 7865 6375 7461 626c  .name..executabl
-000005a0: 65da 0a69 6e70 7574 5f74 7970 65da 0b6f  e..input_type..o
-000005b0: 7574 7075 745f 7479 7065 2901 da0f 6465  utput_type)...de
-000005c0: 6661 756c 745f 6661 6374 6f72 79da 0c64  fault_factory..d
-000005d0: 6566 6175 6c74 5f61 7267 73da 046d 6574  efault_args..met
-000005e0: 614e 290d da08 5f5f 6e61 6d65 5f5f da0a  aN)...__name__..
-000005f0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000600: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00000610: 5fda 0373 7472 da0f 5f5f 616e 6e6f 7461  _..str..__annota
-00000620: 7469 6f6e 735f 5f72 0200 0000 7207 0000  tions__r....r...
-00000630: 00da 0464 6963 7472 1100 0000 7204 0000  ...dictr....r...
-00000640: 0072 0300 0000 7212 0000 00a9 0072 1a00  .r....r......r..
-00000650: 0000 721a 0000 00fa 402f 686f 6d65 2f74  ..r.....@/home/t
-00000660: 6f6d 6d61 736f 2f46 7261 6374 616c 2f66  ommaso/Fractal/f
-00000670: 7261 6374 616c 2f66 7261 6374 616c 2f63  ractal/fractal/c
-00000680: 6f6d 6d6f 6e2f 7363 6865 6d61 732f 6d61  ommon/schemas/ma
-00000690: 6e69 6665 7374 2e70 7972 0b00 0000 0e00  nifest.pyr......
-000006a0: 0000 7310 0000 000a 0004 0108 1c08 0108  ..s.............
-000006b0: 0108 011e 0122 0172 0b00 0000 da10 5461  .....".r......Ta
-000006c0: 736b 4d61 6e69 6665 7374 5479 7065 2901  skManifestType).
-000006d0: da05 626f 756e 6463 0000 0000 0000 0000  ..boundc........
-000006e0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-000006f0: 7326 0000 0065 005a 0164 005a 0255 0064  s&...e.Z.d.Z.U.d
-00000700: 015a 0365 0465 0564 023c 0065 0665 0719  .Z.e.e.d.<.e.e..
-00000710: 0065 0564 033c 0064 0453 0029 05da 0d5f  .e.d.<.d.S.)..._
-00000720: 4d61 6e69 6665 7374 4261 7365 6128 0300  ManifestBasea(..
-00000730: 000a 2020 2020 4d61 6e69 6665 7374 2062  ..    Manifest b
-00000740: 6173 6520 636c 6173 730a 0a20 2020 2050  ase class..    P
-00000750: 6163 6b61 6765 7320 636f 6e74 6169 6e69  ackages containi
-00000760: 6e67 2074 6173 6b73 2061 7265 2072 6571  ng tasks are req
-00000770: 7569 7265 6420 746f 2069 6e63 6c75 6465  uired to include
-00000780: 2061 2073 7065 6369 616c 2066 696c 650a   a special file.
-00000790: 2020 2020 605f 5f46 5241 4354 414c 5f4d      `__FRACTAL_M
-000007a0: 414e 4946 4553 545f 5f2e 6a73 6f6e 6020  ANIFEST__.json` 
-000007b0: 696e 206f 7264 6572 2074 6f20 6265 2064  in order to be d
-000007c0: 6973 636f 7665 7265 6420 616e 6420 7573  iscovered and us
-000007d0: 6564 2062 7920 4672 6163 7461 6c2e 0a0a  ed by Fractal...
-000007e0: 2020 2020 5468 6973 206d 6f64 656c 2063      This model c
-000007f0: 6c61 7373 2061 6e64 2074 6865 206d 6f64  lass and the mod
-00000800: 656c 2063 6c61 7373 6573 2069 7420 6465  el classes it de
-00000810: 7065 6e64 7320 6f6e 2070 726f 7669 6465  pends on provide
-00000820: 2074 6865 2062 6173 650a 2020 2020 7363   the base.    sc
-00000830: 6865 6d61 2074 6f20 7265 6164 2c20 7772  hema to read, wr
-00000840: 6974 6520 616e 6420 7661 6c69 6461 7465  ite and validate
-00000850: 206d 616e 6966 6573 7473 2e0a 0a20 2020   manifests...   
-00000860: 2041 7474 7269 6275 7465 733a 0a20 2020   Attributes:.   
-00000870: 2020 2020 206d 616e 6966 6573 745f 7665       manifest_ve
-00000880: 7273 696f 6e3a 0a20 2020 2020 2020 2020  rsion:.         
-00000890: 2020 2041 2076 6572 7369 6f6e 2073 7472     A version str
-000008a0: 696e 6720 7468 6174 2070 726f 7669 6465  ing that provide
-000008b0: 7320 696e 6469 6361 7469 6f6e 2066 6f72  s indication for
-000008c0: 2063 6f6d 7061 7469 6269 6c69 7479 2062   compatibility b
-000008d0: 6574 7765 656e 0a20 2020 2020 2020 2020  etween.         
-000008e0: 2020 206d 616e 6966 6573 7473 2061 7320     manifests as 
-000008f0: 7468 6520 7363 6865 6d61 2065 766f 6c76  the schema evolv
-00000900: 6573 2e20 5468 6973 2069 7320 666f 7220  es. This is for 
-00000910: 696e 7374 616e 6365 2075 7365 6420 6279  instance used by
-00000920: 0a20 2020 2020 2020 2020 2020 2046 7261  .            Fra
-00000930: 6374 616c 2074 6f20 6465 7465 726d 696e  ctal to determin
-00000940: 6520 7768 6963 6820 7375 6263 6c61 7373  e which subclass
-00000950: 206f 6620 7468 6520 7072 6573 656e 7420   of the present 
-00000960: 6261 7365 2063 6c61 7373 206e 6565 6473  base class needs
-00000970: 0a20 2020 2020 2020 2020 2020 2062 6520  .            be 
-00000980: 7573 6564 2074 6f20 7265 6164 2061 6e64  used to read and
-00000990: 2076 616c 6964 6174 6520 7468 6520 696e   validate the in
-000009a0: 7075 742e 0a20 2020 2020 2020 2074 6173  put..        tas
-000009b0: 6b5f 6c69 7374 203a 206c 6973 745b 5461  k_list : list[Ta
-000009c0: 736b 4d61 6e69 6665 7374 5479 7065 5d0a  skManifestType].
-000009d0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-000009e0: 6c69 7374 206f 6620 7461 736b 732c 2072  list of tasks, r
-000009f0: 6570 7265 7365 6e74 6564 2061 7320 7370  epresented as sp
-00000a00: 6563 6966 6965 6420 6279 2073 7562 636c  ecified by subcl
-00000a10: 6173 7365 7320 6f66 2074 6865 0a20 2020  asses of the.   
-00000a20: 2020 2020 2020 2020 205f 5461 736b 4d61           _TaskMa
-00000a30: 6e69 6665 7374 4261 7365 2028 612e 6b2e  nifestBase (a.k.
-00000a40: 612e 2054 6173 6b4d 616e 6966 6573 7454  a. TaskManifestT
-00000a50: 7970 6529 0a20 2020 20da 106d 616e 6966  ype).    ..manif
-00000a60: 6573 745f 7665 7273 696f 6eda 0974 6173  est_version..tas
-00000a70: 6b5f 6c69 7374 4e29 0872 1300 0000 7214  k_listN).r....r.
-00000a80: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
-00000a90: 0000 7218 0000 00da 046c 6973 7472 1c00  ..r......listr..
-00000aa0: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
-00000ab0: 0072 1b00 0000 721e 0000 0036 0000 0073  .r....r....6...s
-00000ac0: 0800 0000 0a00 0401 0814 1001 721e 0000  ............r...
-00000ad0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000ae0: 0000 0100 0000 4000 0000 730c 0000 0065  ......@...s....e
-00000af0: 005a 0164 005a 0264 0153 0029 0272 0900  .Z.d.Z.d.S.).r..
-00000b00: 0000 4e29 0372 1300 0000 7214 0000 0072  ..N).r....r....r
-00000b10: 1500 0000 721a 0000 0072 1a00 0000 721a  ....r....r....r.
-00000b20: 0000 0072 1b00 0000 7209 0000 004f 0000  ...r....r....O..
-00000b30: 0073 0400 0000 0800 0401 7209 0000 0063  .s........r....c
-00000b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b50: 0300 0000 4000 0000 732e 0000 0065 005a  ....@...s....e.Z
-00000b60: 0164 005a 0255 0064 015a 0365 0465 0519  .d.Z.U.d.Z.e.e..
-00000b70: 0065 0664 023c 0065 0764 0383 0164 0464  .e.d.<.e.d...d.d
-00000b80: 0584 0083 015a 0864 0653 0029 0772 0a00  .....Z.d.S.).r..
-00000b90: 0000 7a23 0a20 2020 204d 616e 6966 6573  ..z#.    Manifes
-00000ba0: 7420 7363 6865 6d61 2076 6572 7369 6f6e  t schema version
-00000bb0: 2031 0a20 2020 2072 2000 0000 721f 0000   1.    r ...r...
-00000bc0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-00000bd0: 0000 0200 0000 4300 0000 7314 0000 007c  ......C...s....|
-00000be0: 0164 016b 0372 0874 0064 0283 0182 0164  .d.k.r.t.d.....d
-00000bf0: 0053 0029 034e da01 317a 1657 726f 6e67  .S.).N..1z.Wrong
-00000c00: 206d 616e 6966 6573 7420 7665 7273 696f   manifest versio
-00000c10: 6e29 01da 0a56 616c 7565 4572 726f 7229  n)...ValueError)
-00000c20: 02da 0363 6c73 da05 7661 6c75 6572 1a00  ...cls..valuer..
-00000c30: 0000 721a 0000 0072 1b00 0000 da12 6d61  ..r....r......ma
-00000c40: 6e69 6665 7374 5f76 6572 7369 6f6e 5f31  nifest_version_1
-00000c50: 5a00 0000 7306 0000 0008 0208 0104 ff7a  Z...s..........z
-00000c60: 1d4d 616e 6966 6573 7456 312e 6d61 6e69  .ManifestV1.mani
-00000c70: 6665 7374 5f76 6572 7369 6f6e 5f31 4e29  fest_version_1N)
-00000c80: 0972 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
-00000c90: 7216 0000 0072 2100 0000 7209 0000 0072  r....r!...r....r
-00000ca0: 1800 0000 7208 0000 0072 2600 0000 721a  ....r....r&...r.
-00000cb0: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
-00000cc0: 0000 720a 0000 0053 0000 0073 0a00 0000  ..r....S...s....
-00000cd0: 0a00 0401 0c04 0602 0e01 720a 0000 004e  ..........r....N
-00000ce0: 2910 da07 7061 7468 6c69 6272 0200 0000  )...pathlibr....
-00000cf0: da06 7479 7069 6e67 7203 0000 0072 0400  ..typingr....r..
-00000d00: 0000 7205 0000 00da 0870 7964 616e 7469  ..r......pydanti
-00000d10: 6372 0600 0000 7207 0000 0072 0800 0000  cr....r....r....
-00000d20: da07 5f5f 616c 6c5f 5f72 0b00 0000 721c  ..__all__r....r.
-00000d30: 0000 0072 1e00 0000 7209 0000 0072 0a00  ...r....r....r..
-00000d40: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
-00000d50: 0072 1b00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000d60: 0100 0000 731a 0000 000c 000c 010c 010c  ....s...........
-00000d70: 010c 020c 010c 0104 0310 030c 2510 0310  ............%...
-00000d80: 1914 04                                  ...
+00000060: 6405 6c02 6d06 5a06 0100 6400 6406 6c02  d.l.m.Z...d.d.l.
+00000070: 6d07 5a07 0100 6400 6407 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
+00000080: 0100 6400 6408 6c08 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
+00000090: 6409 6c0b 6d0c 5a0c 0100 640a 5a0d 4700  d.l.m.Z...d.Z.G.
+000000a0: 640b 640c 8400 640c 6509 8303 5a0e 6507  d.d...d.e...Z.e.
+000000b0: 640d 650e 640e 8d02 5a0f 4700 640f 6410  d.e.d...Z.G.d.d.
+000000c0: 8400 6410 6509 8303 5a10 4700 6411 6412  ..d.e...Z.G.d.d.
+000000d0: 8400 6412 650e 8303 5a11 4700 6413 6414  ..d.e...Z.G.d.d.
+000000e0: 8400 6414 6510 8303 5a12 6415 5300 2916  ..d.e...Z.d.S.).
+000000f0: e900 0000 0029 01da 0450 6174 6829 01da  .....)...Path)..
+00000100: 0341 6e79 2901 da04 4469 6374 2901 da04  .Any)...Dict)...
+00000110: 4c69 7374 2901 da08 4f70 7469 6f6e 616c  List)...Optional
+00000120: 2901 da07 5479 7065 5661 7229 01da 0942  )...TypeVar)...B
+00000130: 6173 654d 6f64 656c 2901 da09 7661 6c69  aseModel)...vali
+00000140: 6461 746f 7229 01da 0546 6965 6c64 2902  dator)...Field).
+00000150: da0e 5461 736b 4d61 6e69 6665 7374 5631  ..TaskManifestV1
+00000160: da0a 4d61 6e69 6665 7374 5631 6300 0000  ..ManifestV1c...
+00000170: 0000 0000 0000 0000 0000 0000 0004 0000  ................
+00000180: 0040 0000 0073 6e00 0000 6500 5a01 6400  .@...sn...e.Z.d.
+00000190: 5a02 5500 6401 5a03 6504 6505 6402 3c00  Z.U.d.Z.e.e.d.<.
+000001a0: 6506 6505 6403 3c00 6504 6505 6404 3c00  e.e.d.<.e.e.d.<.
+000001b0: 6504 6505 6405 3c00 6507 6508 6406 8d01  e.e.d.<.e.e.d...
+000001c0: 5a09 650a 650b 6504 650c 6602 1900 1900  Z.e.e.e.e.f.....
+000001d0: 6505 6407 3c00 6507 6508 6406 8d01 5a0d  e.d.<.e.e.d...Z.
+000001e0: 650a 650b 6504 650c 6602 1900 1900 6505  e.e.e.e.f.....e.
+000001f0: 6408 3c00 6409 5300 290a da11 5f54 6173  d.<.d.S.)..._Tas
+00000200: 6b4d 616e 6966 6573 7442 6173 6561 a503  kManifestBasea..
+00000210: 0000 0a20 2020 2042 6173 6520 636c 6173  ...    Base clas
+00000220: 7320 666f 7220 5461 736b 4d61 6e69 6665  s for TaskManife
+00000230: 7374 0a0a 2020 2020 5265 7072 6573 656e  st..    Represen
+00000240: 7473 2061 2074 6173 6b20 7769 7468 696e  ts a task within
+00000250: 2061 206d 616e 6665 7374 0a0a 2020 2020   a manfest..    
+00000260: 4174 7472 6962 7574 6573 3a0a 2020 2020  Attributes:.    
+00000270: 2020 2020 6e61 6d65 3a0a 2020 2020 2020      name:.      
+00000280: 2020 2020 2020 5468 6520 7461 736b 206e        The task n
+00000290: 616d 650a 2020 2020 2020 2020 6578 6563  ame.        exec
+000002a0: 7574 6162 6c65 3a0a 2020 2020 2020 2020  utable:.        
+000002b0: 2020 2020 5061 7468 2074 6f20 7468 6520      Path to the 
+000002c0: 6578 6563 7574 6162 6c65 2072 656c 6174  executable relat
+000002d0: 6976 6520 746f 2074 6865 2070 6163 6b61  ive to the packa
+000002e0: 6765 2072 6f6f 740a 0a20 2020 2020 2020  ge root..       
+000002f0: 2020 2020 204e 6f74 653a 2062 7920 7061       Note: by pa
+00000300: 636b 6167 6520 726f 6f74 2077 6520 6d65  ckage root we me
+00000310: 616e 2022 6173 2069 7420 7769 6c6c 2062  an "as it will b
+00000320: 6520 696e 7374 616c 6c65 6422 2e20 4966  e installed". If
+00000330: 2061 0a20 2020 2020 2020 2020 2020 2070   a.            p
+00000340: 6163 6b61 6765 2060 506b 6760 2069 6e73  ackage `Pkg` ins
+00000350: 7461 6c6c 7320 696e 2074 6865 2066 6f6c  talls in the fol
+00000360: 6465 7220 6070 6b67 6020 7468 6520 6578  der `pkg` the ex
+00000370: 6563 7574 6162 6c65 0a20 2020 2020 2020  ecutable.       
+00000380: 2020 2020 2060 706b 672f 6578 6563 7574       `pkg/execut
+00000390: 6162 6c65 2e70 7960 2c20 7468 6973 2061  able.py`, this a
+000003a0: 7474 7269 6275 7465 206d 7573 7420 636f  ttribute must co
+000003b0: 6e74 6169 6e20 6f6e 6c79 0a20 2020 2020  ntain only.     
+000003c0: 2020 2020 2020 2060 6578 6563 7574 6162         `executab
+000003d0: 6c65 2e70 7960 2e0a 2020 2020 2020 2020  le.py`..        
+000003e0: 696e 7075 745f 7479 7065 3a0a 2020 2020  input_type:.    
+000003f0: 2020 2020 2020 2020 5468 6520 696e 7075          The inpu
+00000400: 7420 7479 7065 2061 6363 6570 7465 6420  t type accepted 
+00000410: 6279 2074 6865 2074 6173 6b0a 2020 2020  by the task.    
+00000420: 2020 2020 6f75 7470 7574 5f74 7970 653a      output_type:
+00000430: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00000440: 206f 7574 7075 7420 7479 7065 2072 6574   output type ret
+00000450: 7572 6e65 6420 6279 2074 6865 2074 6173  urned by the tas
+00000460: 6b0a 2020 2020 2020 2020 6465 6661 756c  k.        defaul
+00000470: 745f 6172 6773 3a0a 2020 2020 2020 2020  t_args:.        
+00000480: 2020 2020 416e 2061 7262 6974 7261 7279      An arbitrary
+00000490: 2c20 4a53 4f4e 2d73 6572 6961 6c69 7a61  , JSON-serializa
+000004a0: 626c 6520 6469 6374 696f 6e61 7279 2063  ble dictionary c
+000004b0: 6f6e 7461 696e 696e 6720 7468 6520 6465  ontaining the de
+000004c0: 6661 756c 740a 2020 2020 2020 2020 2020  fault.          
+000004d0: 2020 7061 7261 6d65 7465 7273 2074 6861    parameters tha
+000004e0: 7420 7769 6c6c 2062 6520 7061 7373 6564  t will be passed
+000004f0: 2074 6f20 7468 6520 7461 736b 0a20 2020   to the task.   
+00000500: 2020 2020 206d 6574 613a 0a20 2020 2020       meta:.     
+00000510: 2020 2020 2020 2041 6464 6974 696f 6e61         Additiona
+00000520: 6c20 696e 666f 726d 6174 696f 6e20 6162  l information ab
+00000530: 6f75 7420 7468 6520 7061 636b 6167 652c  out the package,
+00000540: 2073 7563 6820 6173 2068 6173 6820 6f66   such as hash of
+00000550: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00000560: 2065 7865 6375 7461 626c 652c 2073 7065   executable, spe
+00000570: 6369 6669 6320 7275 6e74 696d 6520 7265  cific runtime re
+00000580: 7175 6972 656d 656e 7473 2028 652e 672e  quirements (e.g.
+00000590: 2c20 6e65 6564 5f67 7075 3d54 7275 6529  , need_gpu=True)
+000005a0: 2c0a 2020 2020 2020 2020 2020 2020 6574  ,.            et
+000005b0: 632e 0a20 2020 20da 046e 616d 65da 0a65  c..    ..name..e
+000005c0: 7865 6375 7461 626c 655a 0a69 6e70 7574  xecutableZ.input
+000005d0: 5f74 7970 65da 0b6f 7574 7075 745f 7479  _type..output_ty
+000005e0: 7065 2901 da0f 6465 6661 756c 745f 6661  pe)...default_fa
+000005f0: 6374 6f72 79da 0c64 6566 6175 6c74 5f61  ctory..default_a
+00000600: 7267 73da 046d 6574 614e 290e da08 5f5f  rgs..metaN)...__
+00000610: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000620: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000630: da07 5f5f 646f 635f 5fda 0373 7472 da0f  ..__doc__..str..
+00000640: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
+00000650: 0200 0000 720a 0000 00da 0464 6963 7472  ....r......dictr
+00000660: 1200 0000 7206 0000 0072 0400 0000 7203  ....r....r....r.
+00000670: 0000 0072 1300 0000 a900 721b 0000 0072  ...r......r....r
+00000680: 1b00 0000 fa40 2f68 6f6d 652f 746f 6d6d  .....@/home/tomm
+00000690: 6173 6f2f 4672 6163 7461 6c2f 6672 6163  aso/Fractal/frac
+000006a0: 7461 6c2f 6672 6163 7461 6c2f 636f 6d6d  tal/fractal/comm
+000006b0: 6f6e 2f73 6368 656d 6173 2f6d 616e 6966  on/schemas/manif
+000006c0: 6573 742e 7079 720d 0000 0010 0000 0073  est.pyr........s
+000006d0: 0e00 0000 0a01 041c 0801 0801 0801 0801  ................
+000006e0: 1e01 720d 0000 00da 1054 6173 6b4d 616e  ..r......TaskMan
+000006f0: 6966 6573 7454 7970 6529 01da 0562 6f75  ifestType)...bou
+00000700: 6e64 6300 0000 0000 0000 0000 0000 0000  ndc.............
+00000710: 0000 0003 0000 0040 0000 0073 2600 0000  .......@...s&...
+00000720: 6500 5a01 6400 5a02 5500 6401 5a03 6504  e.Z.d.Z.U.d.Z.e.
+00000730: 6505 6402 3c00 6506 6507 1900 6505 6403  e.d.<.e.e...e.d.
+00000740: 3c00 6404 5300 2905 da0d 5f4d 616e 6966  <.d.S.)..._Manif
+00000750: 6573 7442 6173 6561 2803 0000 0a20 2020  estBasea(....   
+00000760: 204d 616e 6966 6573 7420 6261 7365 2063   Manifest base c
+00000770: 6c61 7373 0a0a 2020 2020 5061 636b 6167  lass..    Packag
+00000780: 6573 2063 6f6e 7461 696e 696e 6720 7461  es containing ta
+00000790: 736b 7320 6172 6520 7265 7175 6972 6564  sks are required
+000007a0: 2074 6f20 696e 636c 7564 6520 6120 7370   to include a sp
+000007b0: 6563 6961 6c20 6669 6c65 0a20 2020 2060  ecial file.    `
+000007c0: 5f5f 4652 4143 5441 4c5f 4d41 4e49 4645  __FRACTAL_MANIFE
+000007d0: 5354 5f5f 2e6a 736f 6e60 2069 6e20 6f72  ST__.json` in or
+000007e0: 6465 7220 746f 2062 6520 6469 7363 6f76  der to be discov
+000007f0: 6572 6564 2061 6e64 2075 7365 6420 6279  ered and used by
+00000800: 2046 7261 6374 616c 2e0a 0a20 2020 2054   Fractal...    T
+00000810: 6869 7320 6d6f 6465 6c20 636c 6173 7320  his model class 
+00000820: 616e 6420 7468 6520 6d6f 6465 6c20 636c  and the model cl
+00000830: 6173 7365 7320 6974 2064 6570 656e 6473  asses it depends
+00000840: 206f 6e20 7072 6f76 6964 6520 7468 6520   on provide the 
+00000850: 6261 7365 0a20 2020 2073 6368 656d 6120  base.    schema 
+00000860: 746f 2072 6561 642c 2077 7269 7465 2061  to read, write a
+00000870: 6e64 2076 616c 6964 6174 6520 6d61 6e69  nd validate mani
+00000880: 6665 7374 732e 0a0a 2020 2020 4174 7472  fests...    Attr
+00000890: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
+000008a0: 6d61 6e69 6665 7374 5f76 6572 7369 6f6e  manifest_version
+000008b0: 3a0a 2020 2020 2020 2020 2020 2020 4120  :.            A 
+000008c0: 7665 7273 696f 6e20 7374 7269 6e67 2074  version string t
+000008d0: 6861 7420 7072 6f76 6964 6573 2069 6e64  hat provides ind
+000008e0: 6963 6174 696f 6e20 666f 7220 636f 6d70  ication for comp
+000008f0: 6174 6962 696c 6974 7920 6265 7477 6565  atibility betwee
+00000900: 6e0a 2020 2020 2020 2020 2020 2020 6d61  n.            ma
+00000910: 6e69 6665 7374 7320 6173 2074 6865 2073  nifests as the s
+00000920: 6368 656d 6120 6576 6f6c 7665 732e 2054  chema evolves. T
+00000930: 6869 7320 6973 2066 6f72 2069 6e73 7461  his is for insta
+00000940: 6e63 6520 7573 6564 2062 790a 2020 2020  nce used by.    
+00000950: 2020 2020 2020 2020 4672 6163 7461 6c20          Fractal 
+00000960: 746f 2064 6574 6572 6d69 6e65 2077 6869  to determine whi
+00000970: 6368 2073 7562 636c 6173 7320 6f66 2074  ch subclass of t
+00000980: 6865 2070 7265 7365 6e74 2062 6173 6520  he present base 
+00000990: 636c 6173 7320 6e65 6564 730a 2020 2020  class needs.    
+000009a0: 2020 2020 2020 2020 6265 2075 7365 6420          be used 
+000009b0: 746f 2072 6561 6420 616e 6420 7661 6c69  to read and vali
+000009c0: 6461 7465 2074 6865 2069 6e70 7574 2e0a  date the input..
+000009d0: 2020 2020 2020 2020 7461 736b 5f6c 6973          task_lis
+000009e0: 7420 3a20 4c69 7374 5b54 6173 6b4d 616e  t : List[TaskMan
+000009f0: 6966 6573 7454 7970 655d 0a20 2020 2020  ifestType].     
+00000a00: 2020 2020 2020 2054 6865 206c 6973 7420         The list 
+00000a10: 6f66 2074 6173 6b73 2c20 7265 7072 6573  of tasks, repres
+00000a20: 656e 7465 6420 6173 2073 7065 6369 6669  ented as specifi
+00000a30: 6564 2062 7920 7375 6263 6c61 7373 6573  ed by subclasses
+00000a40: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
+00000a50: 2020 2020 5f54 6173 6b4d 616e 6966 6573      _TaskManifes
+00000a60: 7442 6173 6520 2861 2e6b 2e61 2e20 5461  tBase (a.k.a. Ta
+00000a70: 736b 4d61 6e69 6665 7374 5479 7065 290a  skManifestType).
+00000a80: 2020 2020 da10 6d61 6e69 6665 7374 5f76      ..manifest_v
+00000a90: 6572 7369 6f6e da09 7461 736b 5f6c 6973  ersion..task_lis
+00000aa0: 744e 2908 7214 0000 0072 1500 0000 7216  tN).r....r....r.
+00000ab0: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
+00000ac0: 0000 7205 0000 0072 1d00 0000 721b 0000  ..r....r....r...
+00000ad0: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00000ae0: 721f 0000 0038 0000 0073 0600 0000 0a01  r....8...s......
+00000af0: 0414 0801 721f 0000 0063 0000 0000 0000  ....r....c......
+00000b00: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+00000b10: 0000 730c 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00000b20: 0153 0029 0272 0b00 0000 4e29 0372 1400  .S.).r....N).r..
+00000b30: 0000 7215 0000 0072 1600 0000 721b 0000  ..r....r....r...
+00000b40: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00000b50: 720b 0000 0051 0000 0073 0200 0000 0801  r....Q...s......
+00000b60: 720b 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000b70: 0000 0000 0000 0300 0000 4000 0000 732e  ..........@...s.
+00000b80: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
+00000b90: 0365 0465 0519 0065 0664 023c 0065 0764  .e.e...e.d.<.e.d
+00000ba0: 0383 0164 0464 0584 0083 015a 0864 0653  ...d.d.....Z.d.S
+00000bb0: 0029 0772 0c00 0000 7a23 0a20 2020 204d  .).r....z#.    M
+00000bc0: 616e 6966 6573 7420 7363 6865 6d61 2076  anifest schema v
+00000bd0: 6572 7369 6f6e 2031 0a20 2020 2072 2100  ersion 1.    r!.
+00000be0: 0000 7220 0000 0063 0200 0000 0000 0000  ..r ...c........
+00000bf0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00000c00: 7314 0000 007c 0164 016b 0372 1074 0064  s....|.d.k.r.t.d
+00000c10: 0283 0182 0164 0053 0029 034e da01 317a  .....d.S.).N..1z
+00000c20: 1657 726f 6e67 206d 616e 6966 6573 7420  .Wrong manifest 
+00000c30: 7665 7273 696f 6e29 01da 0a56 616c 7565  version)...Value
+00000c40: 4572 726f 7229 02da 0363 6c73 da05 7661  Error)...cls..va
+00000c50: 6c75 6572 1b00 0000 721b 0000 0072 1c00  luer....r....r..
+00000c60: 0000 da12 6d61 6e69 6665 7374 5f76 6572  ....manifest_ver
+00000c70: 7369 6f6e 5f31 5c00 0000 7304 0000 0000  sion_1\...s.....
+00000c80: 0208 017a 1d4d 616e 6966 6573 7456 312e  ...z.ManifestV1.
+00000c90: 6d61 6e69 6665 7374 5f76 6572 7369 6f6e  manifest_version
+00000ca0: 5f31 4e29 0972 1400 0000 7215 0000 0072  _1N).r....r....r
+00000cb0: 1600 0000 7217 0000 0072 0500 0000 720b  ....r....r....r.
+00000cc0: 0000 0072 1900 0000 7209 0000 0072 2600  ...r....r....r&.
+00000cd0: 0000 721b 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+00000ce0: 0072 1c00 0000 720c 0000 0055 0000 0073  .r....r....U...s
+00000cf0: 0800 0000 0a01 0404 0c02 0601 720c 0000  ............r...
+00000d00: 004e 2913 da07 7061 7468 6c69 6272 0200  .N)...pathlibr..
+00000d10: 0000 da06 7479 7069 6e67 7203 0000 0072  ....typingr....r
+00000d20: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
+00000d30: 0000 00da 0870 7964 616e 7469 6372 0800  .....pydanticr..
+00000d40: 0000 7209 0000 00da 0873 716c 6d6f 6465  ..r......sqlmode
+00000d50: 6c72 0a00 0000 da07 5f5f 616c 6c5f 5f72  lr......__all__r
+00000d60: 0d00 0000 721d 0000 0072 1f00 0000 720b  ....r....r....r.
+00000d70: 0000 0072 0c00 0000 721b 0000 0072 1b00  ...r....r....r..
+00000d80: 0000 721b 0000 0072 1c00 0000 da08 3c6d  ..r....r......<m
+00000d90: 6f64 756c 653e 0100 0000 731c 0000 000c  odule>....s.....
+00000da0: 010c 010c 010c 010c 010c 020c 010c 010c  ................
+00000db0: 0304 0310 250c 0310 1910 04              ....%......
```

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Feb 21 08:49:27 2023 UTC, .py size: 2817 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,220 +1,255 @@
-00000000: 610d 0d0a 0000 0000 9785 f463 010b 0000  a..........c....
+00000000: 6f0d 0d0a 0000 0000 faf1 8664 970d 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c02 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c02 6d06 5a06 0100 6400 6406 6c02  d.l.m.Z...d.d.l.
-00000070: 6d07 5a07 0100 6400 6407 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000080: 0100 6400 6408 6c08 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
-00000090: 6409 6c0b 6d0c 5a0c 0100 640a 5a0d 4700  d.l.m.Z...d.Z.G.
-000000a0: 640b 640c 8400 640c 6509 8303 5a0e 6507  d.d...d.e...Z.e.
-000000b0: 640d 650e 640e 8d02 5a0f 4700 640f 6410  d.e.d...Z.G.d.d.
-000000c0: 8400 6410 6509 8303 5a10 4700 6411 6412  ..d.e...Z.G.d.d.
-000000d0: 8400 6412 650e 8303 5a11 4700 6413 6414  ..d.e...Z.G.d.d.
-000000e0: 8400 6414 6510 8303 5a12 6415 5300 2916  ..d.e...Z.d.S.).
-000000f0: e900 0000 0029 01da 0450 6174 6829 01da  .....)...Path)..
-00000100: 0341 6e79 2901 da04 4469 6374 2901 da04  .Any)...Dict)...
-00000110: 4c69 7374 2901 da08 4f70 7469 6f6e 616c  List)...Optional
-00000120: 2901 da07 5479 7065 5661 7229 01da 0942  )...TypeVar)...B
-00000130: 6173 654d 6f64 656c 2901 da09 7661 6c69  aseModel)...vali
-00000140: 6461 746f 7229 01da 0546 6965 6c64 2902  dator)...Field).
-00000150: da0e 5461 736b 4d61 6e69 6665 7374 5631  ..TaskManifestV1
-00000160: da0a 4d61 6e69 6665 7374 5631 6300 0000  ..ManifestV1c...
-00000170: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-00000180: 0040 0000 0073 6e00 0000 6500 5a01 6400  .@...sn...e.Z.d.
-00000190: 5a02 5500 6401 5a03 6504 6505 6402 3c00  Z.U.d.Z.e.e.d.<.
-000001a0: 6506 6505 6403 3c00 6504 6505 6404 3c00  e.e.d.<.e.e.d.<.
-000001b0: 6504 6505 6405 3c00 6507 6508 6406 8d01  e.e.d.<.e.e.d...
-000001c0: 5a09 650a 650b 6504 650c 6602 1900 1900  Z.e.e.e.e.f.....
-000001d0: 6505 6407 3c00 6507 6508 6406 8d01 5a0d  e.d.<.e.e.d...Z.
-000001e0: 650a 650b 6504 650c 6602 1900 1900 6505  e.e.e.e.f.....e.
-000001f0: 6408 3c00 6409 5300 290a da11 5f54 6173  d.<.d.S.)..._Tas
-00000200: 6b4d 616e 6966 6573 7442 6173 6561 a503  kManifestBasea..
-00000210: 0000 0a20 2020 2042 6173 6520 636c 6173  ...    Base clas
-00000220: 7320 666f 7220 5461 736b 4d61 6e69 6665  s for TaskManife
-00000230: 7374 0a0a 2020 2020 5265 7072 6573 656e  st..    Represen
-00000240: 7473 2061 2074 6173 6b20 7769 7468 696e  ts a task within
-00000250: 2061 206d 616e 6665 7374 0a0a 2020 2020   a manfest..    
-00000260: 4174 7472 6962 7574 6573 3a0a 2020 2020  Attributes:.    
-00000270: 2020 2020 6e61 6d65 3a0a 2020 2020 2020      name:.      
-00000280: 2020 2020 2020 5468 6520 7461 736b 206e        The task n
-00000290: 616d 650a 2020 2020 2020 2020 6578 6563  ame.        exec
-000002a0: 7574 6162 6c65 3a0a 2020 2020 2020 2020  utable:.        
-000002b0: 2020 2020 5061 7468 2074 6f20 7468 6520      Path to the 
-000002c0: 6578 6563 7574 6162 6c65 2072 656c 6174  executable relat
-000002d0: 6976 6520 746f 2074 6865 2070 6163 6b61  ive to the packa
-000002e0: 6765 2072 6f6f 740a 0a20 2020 2020 2020  ge root..       
-000002f0: 2020 2020 204e 6f74 653a 2062 7920 7061       Note: by pa
-00000300: 636b 6167 6520 726f 6f74 2077 6520 6d65  ckage root we me
-00000310: 616e 2022 6173 2069 7420 7769 6c6c 2062  an "as it will b
-00000320: 6520 696e 7374 616c 6c65 6422 2e20 4966  e installed". If
-00000330: 2061 0a20 2020 2020 2020 2020 2020 2070   a.            p
-00000340: 6163 6b61 6765 2060 506b 6760 2069 6e73  ackage `Pkg` ins
-00000350: 7461 6c6c 7320 696e 2074 6865 2066 6f6c  talls in the fol
-00000360: 6465 7220 6070 6b67 6020 7468 6520 6578  der `pkg` the ex
-00000370: 6563 7574 6162 6c65 0a20 2020 2020 2020  ecutable.       
-00000380: 2020 2020 2060 706b 672f 6578 6563 7574       `pkg/execut
-00000390: 6162 6c65 2e70 7960 2c20 7468 6973 2061  able.py`, this a
-000003a0: 7474 7269 6275 7465 206d 7573 7420 636f  ttribute must co
-000003b0: 6e74 6169 6e20 6f6e 6c79 0a20 2020 2020  ntain only.     
-000003c0: 2020 2020 2020 2060 6578 6563 7574 6162         `executab
-000003d0: 6c65 2e70 7960 2e0a 2020 2020 2020 2020  le.py`..        
-000003e0: 696e 7075 745f 7479 7065 3a0a 2020 2020  input_type:.    
-000003f0: 2020 2020 2020 2020 5468 6520 696e 7075          The inpu
-00000400: 7420 7479 7065 2061 6363 6570 7465 6420  t type accepted 
-00000410: 6279 2074 6865 2074 6173 6b0a 2020 2020  by the task.    
-00000420: 2020 2020 6f75 7470 7574 5f74 7970 653a      output_type:
-00000430: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00000440: 206f 7574 7075 7420 7479 7065 2072 6574   output type ret
-00000450: 7572 6e65 6420 6279 2074 6865 2074 6173  urned by the tas
-00000460: 6b0a 2020 2020 2020 2020 6465 6661 756c  k.        defaul
-00000470: 745f 6172 6773 3a0a 2020 2020 2020 2020  t_args:.        
-00000480: 2020 2020 416e 2061 7262 6974 7261 7279      An arbitrary
-00000490: 2c20 4a53 4f4e 2d73 6572 6961 6c69 7a61  , JSON-serializa
-000004a0: 626c 6520 6469 6374 696f 6e61 7279 2063  ble dictionary c
-000004b0: 6f6e 7461 696e 696e 6720 7468 6520 6465  ontaining the de
-000004c0: 6661 756c 740a 2020 2020 2020 2020 2020  fault.          
-000004d0: 2020 7061 7261 6d65 7465 7273 2074 6861    parameters tha
-000004e0: 7420 7769 6c6c 2062 6520 7061 7373 6564  t will be passed
-000004f0: 2074 6f20 7468 6520 7461 736b 0a20 2020   to the task.   
-00000500: 2020 2020 206d 6574 613a 0a20 2020 2020       meta:.     
-00000510: 2020 2020 2020 2041 6464 6974 696f 6e61         Additiona
-00000520: 6c20 696e 666f 726d 6174 696f 6e20 6162  l information ab
-00000530: 6f75 7420 7468 6520 7061 636b 6167 652c  out the package,
-00000540: 2073 7563 6820 6173 2068 6173 6820 6f66   such as hash of
-00000550: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-00000560: 2065 7865 6375 7461 626c 652c 2073 7065   executable, spe
-00000570: 6369 6669 6320 7275 6e74 696d 6520 7265  cific runtime re
-00000580: 7175 6972 656d 656e 7473 2028 652e 672e  quirements (e.g.
-00000590: 2c20 6e65 6564 5f67 7075 3d54 7275 6529  , need_gpu=True)
-000005a0: 2c0a 2020 2020 2020 2020 2020 2020 6574  ,.            et
-000005b0: 632e 0a20 2020 20da 046e 616d 65da 0a65  c..    ..name..e
-000005c0: 7865 6375 7461 626c 655a 0a69 6e70 7574  xecutableZ.input
-000005d0: 5f74 7970 65da 0b6f 7574 7075 745f 7479  _type..output_ty
-000005e0: 7065 2901 da0f 6465 6661 756c 745f 6661  pe)...default_fa
-000005f0: 6374 6f72 79da 0c64 6566 6175 6c74 5f61  ctory..default_a
-00000600: 7267 73da 046d 6574 614e 290e da08 5f5f  rgs..metaN)...__
-00000610: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000620: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000630: da07 5f5f 646f 635f 5fda 0373 7472 da0f  ..__doc__..str..
-00000640: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
-00000650: 0200 0000 720a 0000 00da 0464 6963 7472  ....r......dictr
-00000660: 1200 0000 7206 0000 0072 0400 0000 7203  ....r....r....r.
-00000670: 0000 0072 1300 0000 a900 721b 0000 0072  ...r......r....r
-00000680: 1b00 0000 fa40 2f68 6f6d 652f 746f 6d6d  .....@/home/tomm
-00000690: 6173 6f2f 4672 6163 7461 6c2f 6672 6163  aso/Fractal/frac
-000006a0: 7461 6c2f 6672 6163 7461 6c2f 636f 6d6d  tal/fractal/comm
-000006b0: 6f6e 2f73 6368 656d 6173 2f6d 616e 6966  on/schemas/manif
-000006c0: 6573 742e 7079 720d 0000 0010 0000 0073  est.pyr........s
-000006d0: 0e00 0000 0a01 041c 0801 0801 0801 0801  ................
-000006e0: 1e01 720d 0000 00da 1054 6173 6b4d 616e  ..r......TaskMan
-000006f0: 6966 6573 7454 7970 6529 01da 0562 6f75  ifestType)...bou
-00000700: 6e64 6300 0000 0000 0000 0000 0000 0000  ndc.............
-00000710: 0000 0003 0000 0040 0000 0073 2600 0000  .......@...s&...
-00000720: 6500 5a01 6400 5a02 5500 6401 5a03 6504  e.Z.d.Z.U.d.Z.e.
-00000730: 6505 6402 3c00 6506 6507 1900 6505 6403  e.d.<.e.e...e.d.
-00000740: 3c00 6404 5300 2905 da0d 5f4d 616e 6966  <.d.S.)..._Manif
-00000750: 6573 7442 6173 6561 2803 0000 0a20 2020  estBasea(....   
-00000760: 204d 616e 6966 6573 7420 6261 7365 2063   Manifest base c
-00000770: 6c61 7373 0a0a 2020 2020 5061 636b 6167  lass..    Packag
-00000780: 6573 2063 6f6e 7461 696e 696e 6720 7461  es containing ta
-00000790: 736b 7320 6172 6520 7265 7175 6972 6564  sks are required
-000007a0: 2074 6f20 696e 636c 7564 6520 6120 7370   to include a sp
-000007b0: 6563 6961 6c20 6669 6c65 0a20 2020 2060  ecial file.    `
-000007c0: 5f5f 4652 4143 5441 4c5f 4d41 4e49 4645  __FRACTAL_MANIFE
-000007d0: 5354 5f5f 2e6a 736f 6e60 2069 6e20 6f72  ST__.json` in or
-000007e0: 6465 7220 746f 2062 6520 6469 7363 6f76  der to be discov
-000007f0: 6572 6564 2061 6e64 2075 7365 6420 6279  ered and used by
-00000800: 2046 7261 6374 616c 2e0a 0a20 2020 2054   Fractal...    T
-00000810: 6869 7320 6d6f 6465 6c20 636c 6173 7320  his model class 
-00000820: 616e 6420 7468 6520 6d6f 6465 6c20 636c  and the model cl
-00000830: 6173 7365 7320 6974 2064 6570 656e 6473  asses it depends
-00000840: 206f 6e20 7072 6f76 6964 6520 7468 6520   on provide the 
-00000850: 6261 7365 0a20 2020 2073 6368 656d 6120  base.    schema 
-00000860: 746f 2072 6561 642c 2077 7269 7465 2061  to read, write a
-00000870: 6e64 2076 616c 6964 6174 6520 6d61 6e69  nd validate mani
-00000880: 6665 7374 732e 0a0a 2020 2020 4174 7472  fests...    Attr
-00000890: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
-000008a0: 6d61 6e69 6665 7374 5f76 6572 7369 6f6e  manifest_version
-000008b0: 3a0a 2020 2020 2020 2020 2020 2020 4120  :.            A 
-000008c0: 7665 7273 696f 6e20 7374 7269 6e67 2074  version string t
-000008d0: 6861 7420 7072 6f76 6964 6573 2069 6e64  hat provides ind
-000008e0: 6963 6174 696f 6e20 666f 7220 636f 6d70  ication for comp
-000008f0: 6174 6962 696c 6974 7920 6265 7477 6565  atibility betwee
-00000900: 6e0a 2020 2020 2020 2020 2020 2020 6d61  n.            ma
-00000910: 6e69 6665 7374 7320 6173 2074 6865 2073  nifests as the s
-00000920: 6368 656d 6120 6576 6f6c 7665 732e 2054  chema evolves. T
-00000930: 6869 7320 6973 2066 6f72 2069 6e73 7461  his is for insta
-00000940: 6e63 6520 7573 6564 2062 790a 2020 2020  nce used by.    
-00000950: 2020 2020 2020 2020 4672 6163 7461 6c20          Fractal 
-00000960: 746f 2064 6574 6572 6d69 6e65 2077 6869  to determine whi
-00000970: 6368 2073 7562 636c 6173 7320 6f66 2074  ch subclass of t
-00000980: 6865 2070 7265 7365 6e74 2062 6173 6520  he present base 
-00000990: 636c 6173 7320 6e65 6564 730a 2020 2020  class needs.    
-000009a0: 2020 2020 2020 2020 6265 2075 7365 6420          be used 
-000009b0: 746f 2072 6561 6420 616e 6420 7661 6c69  to read and vali
-000009c0: 6461 7465 2074 6865 2069 6e70 7574 2e0a  date the input..
-000009d0: 2020 2020 2020 2020 7461 736b 5f6c 6973          task_lis
-000009e0: 7420 3a20 4c69 7374 5b54 6173 6b4d 616e  t : List[TaskMan
-000009f0: 6966 6573 7454 7970 655d 0a20 2020 2020  ifestType].     
-00000a00: 2020 2020 2020 2054 6865 206c 6973 7420         The list 
-00000a10: 6f66 2074 6173 6b73 2c20 7265 7072 6573  of tasks, repres
-00000a20: 656e 7465 6420 6173 2073 7065 6369 6669  ented as specifi
-00000a30: 6564 2062 7920 7375 6263 6c61 7373 6573  ed by subclasses
-00000a40: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
-00000a50: 2020 2020 5f54 6173 6b4d 616e 6966 6573      _TaskManifes
-00000a60: 7442 6173 6520 2861 2e6b 2e61 2e20 5461  tBase (a.k.a. Ta
-00000a70: 736b 4d61 6e69 6665 7374 5479 7065 290a  skManifestType).
-00000a80: 2020 2020 da10 6d61 6e69 6665 7374 5f76      ..manifest_v
-00000a90: 6572 7369 6f6e da09 7461 736b 5f6c 6973  ersion..task_lis
-00000aa0: 744e 2908 7214 0000 0072 1500 0000 7216  tN).r....r....r.
-00000ab0: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
-00000ac0: 0000 7205 0000 0072 1d00 0000 721b 0000  ..r....r....r...
-00000ad0: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000ae0: 721f 0000 0038 0000 0073 0600 0000 0a01  r....8...s......
-00000af0: 0414 0801 721f 0000 0063 0000 0000 0000  ....r....c......
-00000b00: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-00000b10: 0000 730c 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00000b20: 0153 0029 0272 0b00 0000 4e29 0372 1400  .S.).r....N).r..
-00000b30: 0000 7215 0000 0072 1600 0000 721b 0000  ..r....r....r...
-00000b40: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000b50: 720b 0000 0051 0000 0073 0200 0000 0801  r....Q...s......
-00000b60: 720b 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000b70: 0000 0000 0000 0300 0000 4000 0000 732e  ..........@...s.
-00000b80: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
-00000b90: 0365 0465 0519 0065 0664 023c 0065 0764  .e.e...e.d.<.e.d
-00000ba0: 0383 0164 0464 0584 0083 015a 0864 0653  ...d.d.....Z.d.S
-00000bb0: 0029 0772 0c00 0000 7a23 0a20 2020 204d  .).r....z#.    M
-00000bc0: 616e 6966 6573 7420 7363 6865 6d61 2076  anifest schema v
-00000bd0: 6572 7369 6f6e 2031 0a20 2020 2072 2100  ersion 1.    r!.
-00000be0: 0000 7220 0000 0063 0200 0000 0000 0000  ..r ...c........
-00000bf0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-00000c00: 7314 0000 007c 0164 016b 0372 1074 0064  s....|.d.k.r.t.d
-00000c10: 0283 0182 0164 0053 0029 034e da01 317a  .....d.S.).N..1z
-00000c20: 1657 726f 6e67 206d 616e 6966 6573 7420  .Wrong manifest 
-00000c30: 7665 7273 696f 6e29 01da 0a56 616c 7565  version)...Value
-00000c40: 4572 726f 7229 02da 0363 6c73 da05 7661  Error)...cls..va
-00000c50: 6c75 6572 1b00 0000 721b 0000 0072 1c00  luer....r....r..
-00000c60: 0000 da12 6d61 6e69 6665 7374 5f76 6572  ....manifest_ver
-00000c70: 7369 6f6e 5f31 5c00 0000 7304 0000 0000  sion_1\...s.....
-00000c80: 0208 017a 1d4d 616e 6966 6573 7456 312e  ...z.ManifestV1.
-00000c90: 6d61 6e69 6665 7374 5f76 6572 7369 6f6e  manifest_version
-00000ca0: 5f31 4e29 0972 1400 0000 7215 0000 0072  _1N).r....r....r
-00000cb0: 1600 0000 7217 0000 0072 0500 0000 720b  ....r....r....r.
-00000cc0: 0000 0072 1900 0000 7209 0000 0072 2600  ...r....r....r&.
-00000cd0: 0000 721b 0000 0072 1b00 0000 721b 0000  ..r....r....r...
-00000ce0: 0072 1c00 0000 720c 0000 0055 0000 0073  .r....r....U...s
-00000cf0: 0800 0000 0a01 0404 0c02 0601 720c 0000  ............r...
-00000d00: 004e 2913 da07 7061 7468 6c69 6272 0200  .N)...pathlibr..
-00000d10: 0000 da06 7479 7069 6e67 7203 0000 0072  ....typingr....r
-00000d20: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-00000d30: 0000 00da 0870 7964 616e 7469 6372 0800  .....pydanticr..
-00000d40: 0000 7209 0000 00da 0873 716c 6d6f 6465  ..r......sqlmode
-00000d50: 6c72 0a00 0000 da07 5f5f 616c 6c5f 5f72  lr......__all__r
-00000d60: 0d00 0000 721d 0000 0072 1f00 0000 720b  ....r....r....r.
-00000d70: 0000 0072 0c00 0000 721b 0000 0072 1b00  ...r....r....r..
-00000d80: 0000 721b 0000 0072 1c00 0000 da08 3c6d  ..r....r......<m
-00000d90: 6f64 756c 653e 0100 0000 731c 0000 000c  odule>....s.....
-00000da0: 010c 010c 010c 010c 010c 020c 010c 010c  ................
-00000db0: 0304 0310 250c 0310 1910 04              ....%......
+00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
+00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6404 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6405 6c04 6d06 5a06 0100 6400 6406 6c04  d.l.m.Z...d.d.l.
+00000070: 6d07 5a07 0100 6400 6407 6c04 6d08 5a08  m.Z...d.d.l.m.Z.
+00000080: 0100 6408 5a09 4700 6409 640a 8400 640a  ..d.Z.G.d.d...d.
+00000090: 6505 8303 5a0a 6503 640b 650a 640c 8d02  e...Z.e.d.e.d...
+000000a0: 5a0b 4700 640d 640e 8400 640e 6505 8303  Z.G.d.d...d.e...
+000000b0: 5a0c 4700 640f 6410 8400 6410 650a 8303  Z.G.d.d...d.e...
+000000c0: 5a0d 4700 6411 6412 8400 6412 650c 8303  Z.G.d.d...d.e...
+000000d0: 5a0e 6413 5300 2914 e900 0000 0029 01da  Z.d.S.)......)..
+000000e0: 0341 6e79 2901 da08 4f70 7469 6f6e 616c  .Any)...Optional
+000000f0: 2901 da07 5479 7065 5661 7229 01da 0942  )...TypeVar)...B
+00000100: 6173 654d 6f64 656c 2901 da05 4669 656c  aseModel)...Fiel
+00000110: 6429 01da 0e72 6f6f 745f 7661 6c69 6461  d)...root_valida
+00000120: 746f 7229 01da 0976 616c 6964 6174 6f72  tor)...validator
+00000130: 2902 da0e 5461 736b 4d61 6e69 6665 7374  )...TaskManifest
+00000140: 5631 da0a 4d61 6e69 6665 7374 5631 6300  V1..ManifestV1c.
+00000150: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+00000160: 0000 0040 0000 0073 6400 0000 6500 5a01  ...@...sd...e.Z.
+00000170: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
+00000180: 3c00 6504 6505 6403 3c00 6504 6505 6404  <.e.e.d.<.e.e.d.
+00000190: 3c00 6504 6505 6405 3c00 6506 6507 6406  <.e.e.d.<.e.e.d.
+000001a0: 8d01 5a08 6509 6507 6504 650a 6602 1900  ..Z.e.e.e.e.f...
+000001b0: 1900 6505 6407 3c00 6509 6507 6504 650a  ..e.d.<.e.e.e.e.
+000001c0: 6602 1900 1900 6505 6408 3c00 6409 5300  f.....e.d.<.d.S.
+000001d0: 290a da11 5f54 6173 6b4d 616e 6966 6573  )..._TaskManifes
+000001e0: 7442 6173 6561 4c03 0000 0a20 2020 2042  tBaseaL....    B
+000001f0: 6173 6520 636c 6173 7320 666f 7220 6054  ase class for `T
+00000200: 6173 6b4d 616e 6966 6573 7460 0a0a 2020  askManifest`..  
+00000210: 2020 5265 7072 6573 656e 7473 2061 2074    Represents a t
+00000220: 6173 6b20 7769 7468 696e 2061 206d 616e  ask within a man
+00000230: 6665 7374 0a0a 2020 2020 4174 7472 6962  fest..    Attrib
+00000240: 7574 6573 3a0a 2020 2020 2020 2020 6e61  utes:.        na
+00000250: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
+00000260: 5468 6520 7461 736b 206e 616d 650a 2020  The task name.  
+00000270: 2020 2020 2020 6578 6563 7574 6162 6c65        executable
+00000280: 3a0a 2020 2020 2020 2020 2020 2020 5061  :.            Pa
+00000290: 7468 2074 6f20 7468 6520 6578 6563 7574  th to the execut
+000002a0: 6162 6c65 2072 656c 6174 6976 6520 746f  able relative to
+000002b0: 2074 6865 2070 6163 6b61 6765 2072 6f6f   the package roo
+000002c0: 740a 0a20 2020 2020 2020 2020 2020 204e  t..            N
+000002d0: 6f74 653a 2062 7920 7061 636b 6167 6520  ote: by package 
+000002e0: 726f 6f74 2077 6520 6d65 616e 2022 6173  root we mean "as
+000002f0: 2069 7420 7769 6c6c 2062 6520 696e 7374   it will be inst
+00000300: 616c 6c65 6422 2e20 4966 2061 0a20 2020  alled". If a.   
+00000310: 2020 2020 2020 2020 2070 6163 6b61 6765           package
+00000320: 2060 506b 6760 2069 6e73 7461 6c6c 7320   `Pkg` installs 
+00000330: 696e 2074 6865 2066 6f6c 6465 7220 6070  in the folder `p
+00000340: 6b67 6020 7468 6520 6578 6563 7574 6162  kg` the executab
+00000350: 6c65 0a20 2020 2020 2020 2020 2020 2060  le.            `
+00000360: 706b 672f 6578 6563 7574 6162 6c65 2e70  pkg/executable.p
+00000370: 7960 2c20 7468 6973 2061 7474 7269 6275  y`, this attribu
+00000380: 7465 206d 7573 7420 636f 6e74 6169 6e20  te must contain 
+00000390: 6f6e 6c79 0a20 2020 2020 2020 2020 2020  only.           
+000003a0: 2060 6578 6563 7574 6162 6c65 2e70 7960   `executable.py`
+000003b0: 2e0a 2020 2020 2020 2020 696e 7075 745f  ..        input_
+000003c0: 7479 7065 3a0a 2020 2020 2020 2020 2020  type:.          
+000003d0: 2020 5468 6520 696e 7075 7420 7479 7065    The input type
+000003e0: 2061 6363 6570 7465 6420 6279 2074 6865   accepted by the
+000003f0: 2074 6173 6b0a 2020 2020 2020 2020 6f75   task.        ou
+00000400: 7470 7574 5f74 7970 653a 0a20 2020 2020  tput_type:.     
+00000410: 2020 2020 2020 2054 6865 206f 7574 7075         The outpu
+00000420: 7420 7479 7065 2072 6574 7572 6e65 6420  t type returned 
+00000430: 6279 2074 6865 2074 6173 6b0a 2020 2020  by the task.    
+00000440: 2020 2020 6d65 7461 3a0a 2020 2020 2020      meta:.      
+00000450: 2020 2020 2020 4164 6469 7469 6f6e 616c        Additional
+00000460: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
+00000470: 7574 2074 6865 2070 6163 6b61 6765 2c20  ut the package, 
+00000480: 7375 6368 2061 7320 6861 7368 206f 6620  such as hash of 
+00000490: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+000004a0: 6578 6563 7574 6162 6c65 2c20 7370 6563  executable, spec
+000004b0: 6966 6963 2072 756e 7469 6d65 2072 6571  ific runtime req
+000004c0: 7569 7265 6d65 6e74 7320 2865 2e67 2e2c  uirements (e.g.,
+000004d0: 206e 6565 645f 6770 753d 5472 7565 292c   need_gpu=True),
+000004e0: 0a20 2020 2020 2020 2020 2020 2065 7463  .            etc
+000004f0: 2e0a 2020 2020 2020 2020 6172 6773 5f73  ..        args_s
+00000500: 6368 656d 613a 0a20 2020 2020 2020 2020  chema:.         
+00000510: 2020 204a 534f 4e20 5363 6865 6d61 2066     JSON Schema f
+00000520: 6f72 2074 6173 6b20 6172 6775 6d65 6e74  or task argument
+00000530: 730a 2020 2020 da04 6e61 6d65 da0a 6578  s.    ..name..ex
+00000540: 6563 7574 6162 6c65 da0a 696e 7075 745f  ecutable..input_
+00000550: 7479 7065 da0b 6f75 7470 7574 5f74 7970  type..output_typ
+00000560: 6529 01da 0f64 6566 6175 6c74 5f66 6163  e)...default_fac
+00000570: 746f 7279 da04 6d65 7461 da0b 6172 6773  tory..meta..args
+00000580: 5f73 6368 656d 614e 290b da08 5f5f 6e61  _schemaN)...__na
+00000590: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+000005a0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+000005b0: 5f5f 646f 635f 5fda 0373 7472 da0f 5f5f  __doc__..str..__
+000005c0: 616e 6e6f 7461 7469 6f6e 735f 5f72 0600  annotations__r..
+000005d0: 0000 da04 6469 6374 7211 0000 0072 0300  ....dictr....r..
+000005e0: 0000 7202 0000 00a9 0072 1a00 0000 721a  ..r......r....r.
+000005f0: 0000 00fa 402f 686f 6d65 2f74 6f6d 6d61  ....@/home/tomma
+00000600: 736f 2f46 7261 6374 616c 2f66 7261 6374  so/Fractal/fract
+00000610: 616c 2f66 7261 6374 616c 2f63 6f6d 6d6f  al/fractal/commo
+00000620: 6e2f 7363 6865 6d61 732f 6d61 6e69 6665  n/schemas/manife
+00000630: 7374 2e70 7972 0b00 0000 0e00 0000 7310  st.pyr........s.
+00000640: 0000 000a 0004 0108 1b08 0108 0108 011e  ................
+00000650: 0118 0172 0b00 0000 da10 5461 736b 4d61  ...r......TaskMa
+00000660: 6e69 6665 7374 5479 7065 2901 da05 626f  nifestType)...bo
+00000670: 756e 6463 0000 0000 0000 0000 0000 0000  undc............
+00000680: 0000 0000 0300 0000 4000 0000 734c 0000  ........@...sL..
+00000690: 0065 005a 0164 005a 0255 0064 015a 0365  .e.Z.d.Z.U.d.Z.e
+000006a0: 0465 0564 023c 0065 0665 0719 0065 0564  .e.d.<.e.e...e.d
+000006b0: 033c 0064 045a 0865 0965 0564 053c 0065  .<.d.Z.e.e.d.<.e
+000006c0: 0a65 0419 0065 0564 063c 0065 0b83 0064  .e...e.d.<.e...d
+000006d0: 0764 0884 0083 015a 0c64 0953 0029 0ada  .d.....Z.d.S.)..
+000006e0: 0d5f 4d61 6e69 6665 7374 4261 7365 6111  ._ManifestBasea.
+000006f0: 0400 000a 2020 2020 4d61 6e69 6665 7374  ....    Manifest
+00000700: 2062 6173 6520 636c 6173 730a 0a20 2020   base class..   
+00000710: 2050 6163 6b61 6765 7320 636f 6e74 6169   Packages contai
+00000720: 6e69 6e67 2074 6173 6b73 2061 7265 2072  ning tasks are r
+00000730: 6571 7569 7265 6420 746f 2069 6e63 6c75  equired to inclu
+00000740: 6465 2061 2073 7065 6369 616c 2066 696c  de a special fil
+00000750: 650a 2020 2020 605f 5f46 5241 4354 414c  e.    `__FRACTAL
+00000760: 5f4d 414e 4946 4553 545f 5f2e 6a73 6f6e  _MANIFEST__.json
+00000770: 6020 696e 206f 7264 6572 2074 6f20 6265  ` in order to be
+00000780: 2064 6973 636f 7665 7265 6420 616e 6420   discovered and 
+00000790: 7573 6564 2062 7920 4672 6163 7461 6c2e  used by Fractal.
+000007a0: 0a0a 2020 2020 5468 6973 206d 6f64 656c  ..    This model
+000007b0: 2063 6c61 7373 2061 6e64 2074 6865 206d   class and the m
+000007c0: 6f64 656c 2063 6c61 7373 6573 2069 7420  odel classes it 
+000007d0: 6465 7065 6e64 7320 6f6e 2070 726f 7669  depends on provi
+000007e0: 6465 2074 6865 2062 6173 650a 2020 2020  de the base.    
+000007f0: 7363 6865 6d61 2074 6f20 7265 6164 2c20  schema to read, 
+00000800: 7772 6974 6520 616e 6420 7661 6c69 6461  write and valida
+00000810: 7465 206d 616e 6966 6573 7473 2e0a 0a20  te manifests... 
+00000820: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
+00000830: 2020 2020 2020 206d 616e 6966 6573 745f         manifest_
+00000840: 7665 7273 696f 6e3a 0a20 2020 2020 2020  version:.       
+00000850: 2020 2020 2041 2076 6572 7369 6f6e 2073       A version s
+00000860: 7472 696e 6720 7468 6174 2070 726f 7669  tring that provi
+00000870: 6465 7320 696e 6469 6361 7469 6f6e 2066  des indication f
+00000880: 6f72 2063 6f6d 7061 7469 6269 6c69 7479  or compatibility
+00000890: 2062 6574 7765 656e 0a20 2020 2020 2020   between.       
+000008a0: 2020 2020 206d 616e 6966 6573 7473 2061       manifests a
+000008b0: 7320 7468 6520 7363 6865 6d61 2065 766f  s the schema evo
+000008c0: 6c76 6573 2e20 5468 6973 2069 7320 666f  lves. This is fo
+000008d0: 7220 696e 7374 616e 6365 2075 7365 6420  r instance used 
+000008e0: 6279 0a20 2020 2020 2020 2020 2020 2046  by.            F
+000008f0: 7261 6374 616c 2074 6f20 6465 7465 726d  ractal to determ
+00000900: 696e 6520 7768 6963 6820 7375 6263 6c61  ine which subcla
+00000910: 7373 206f 6620 7468 6520 7072 6573 656e  ss of the presen
+00000920: 7420 6261 7365 2063 6c61 7373 206e 6565  t base class nee
+00000930: 6473 0a20 2020 2020 2020 2020 2020 2062  ds.            b
+00000940: 6520 7573 6564 2074 6f20 7265 6164 2061  e used to read a
+00000950: 6e64 2076 616c 6964 6174 6520 7468 6520  nd validate the 
+00000960: 696e 7075 742e 0a20 2020 2020 2020 2074  input..        t
+00000970: 6173 6b5f 6c69 7374 203a 206c 6973 745b  ask_list : list[
+00000980: 5461 736b 4d61 6e69 6665 7374 5479 7065  TaskManifestType
+00000990: 5d0a 2020 2020 2020 2020 2020 2020 5468  ].            Th
+000009a0: 6520 6c69 7374 206f 6620 7461 736b 732c  e list of tasks,
+000009b0: 2072 6570 7265 7365 6e74 6564 2061 7320   represented as 
+000009c0: 7370 6563 6966 6965 6420 6279 2073 7562  specified by sub
+000009d0: 636c 6173 7365 7320 6f66 2074 6865 0a20  classes of the. 
+000009e0: 2020 2020 2020 2020 2020 205f 5461 736b             _Task
+000009f0: 4d61 6e69 6665 7374 4261 7365 2028 612e  ManifestBase (a.
+00000a00: 6b2e 612e 2054 6173 6b4d 616e 6966 6573  k.a. TaskManifes
+00000a10: 7454 7970 6529 0a20 2020 2020 2020 2068  tType).        h
+00000a20: 6173 5f61 7267 735f 7363 6865 6d61 733a  as_args_schemas:
+00000a30: 0a20 2020 2020 2020 2020 2020 2060 5472  .            `Tr
+00000a40: 7565 6020 6966 2074 6865 206d 616e 6966  ue` if the manif
+00000a50: 6573 7420 696e 636c 6475 6573 204a 534f  est incldues JSO
+00000a60: 4e20 5363 6865 6d61 7320 666f 7220 7468  N Schemas for th
+00000a70: 6520 6172 6775 6d65 6e74 7320 6f66 0a20  e arguments of. 
+00000a80: 2020 2020 2020 2020 2020 2065 6163 6820             each 
+00000a90: 7461 736b 2e0a 2020 2020 2020 2020 6172  task..        ar
+00000aa0: 6773 5f73 6368 656d 615f 7665 7273 696f  gs_schema_versio
+00000ab0: 6e3a 0a20 2020 2020 2020 2020 2020 204c  n:.            L
+00000ac0: 6162 656c 206f 6620 686f 7720 6061 7267  abel of how `arg
+00000ad0: 735f 7363 6865 6d61 6073 2077 6572 6520  s_schema`s were 
+00000ae0: 6765 6e65 7261 7465 6420 2865 2e67 2e20  generated (e.g. 
+00000af0: 6070 7964 616e 7469 635f 7631 6029 2e0a  `pydantic_v1`)..
+00000b00: 2020 2020 da10 6d61 6e69 6665 7374 5f76      ..manifest_v
+00000b10: 6572 7369 6f6e da09 7461 736b 5f6c 6973  ersion..task_lis
+00000b20: 7446 da10 6861 735f 6172 6773 5f73 6368  tF..has_args_sch
+00000b30: 656d 6173 da13 6172 6773 5f73 6368 656d  emas..args_schem
+00000b40: 615f 7665 7273 696f 6e63 0200 0000 0000  a_versionc......
+00000b50: 0000 0000 0000 0500 0000 0900 0000 4300  ..............C.
+00000b60: 0000 734c 0000 007c 0164 0119 007d 027c  ..sL...|.d...}.|
+00000b70: 0164 0219 007d 037c 0272 247c 0344 005d  .d...}.|.r$|.D.]
+00000b80: 177d 047c 046a 0064 0075 0072 2374 0164  .}.|.j.d.u.r#t.d
+00000b90: 037c 029b 0064 047c 046a 029b 0064 057c  .|...d.|.j...d.|
+00000ba0: 046a 009b 0064 069d 0783 0182 0171 0c7c  .j...d.......q.|
+00000bb0: 0153 0029 074e 7221 0000 0072 2000 0000  .S.).Nr!...r ...
+00000bc0: 7a11 6861 735f 6172 6773 5f73 6368 656d  z.has_args_schem
+00000bd0: 6173 3d7a 0b20 6275 7420 7461 736b 2022  as=z. but task "
+00000be0: 7a12 2220 6861 7320 6172 6773 5f73 6368  z." has args_sch
+00000bf0: 656d 613d da01 2e29 0372 1200 0000 da0a  ema=...).r......
+00000c00: 5661 6c75 6545 7272 6f72 720c 0000 0029  ValueErrorr....)
+00000c10: 05da 0363 6c73 da06 7661 6c75 6573 7221  ...cls..valuesr!
+00000c20: 0000 0072 2000 0000 da04 7461 736b 721a  ...r .....taskr.
+00000c30: 0000 0072 1a00 0000 721b 0000 00da 1f5f  ...r....r......_
+00000c40: 6368 6563 6b5f 6172 6773 5f73 6368 656d  check_args_schem
+00000c50: 6173 5f61 7265 5f70 7265 7365 6e74 5400  as_are_presentT.
+00000c60: 0000 731c 0000 0008 0208 0104 0108 010a  ..s.............
+00000c70: 0102 0108 0104 0104 ff04 0106 ff04 ff02  ................
+00000c80: ff04 057a 2d5f 4d61 6e69 6665 7374 4261  ...z-_ManifestBa
+00000c90: 7365 2e5f 6368 6563 6b5f 6172 6773 5f73  se._check_args_s
+00000ca0: 6368 656d 6173 5f61 7265 5f70 7265 7365  chemas_are_prese
+00000cb0: 6e74 4e29 0d72 1300 0000 7214 0000 0072  ntN).r....r....r
+00000cc0: 1500 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
+00000cd0: 0000 00da 046c 6973 7472 1c00 0000 7221  .....listr....r!
+00000ce0: 0000 00da 0462 6f6f 6c72 0300 0000 7207  .....boolr....r.
+00000cf0: 0000 0072 2800 0000 721a 0000 0072 1a00  ...r(...r....r..
+00000d00: 0000 721a 0000 0072 1b00 0000 721e 0000  ..r....r....r...
+00000d10: 0035 0000 0073 1000 0000 0a00 0401 0819  .5...s..........
+00000d20: 0c01 0c01 0c01 0402 0e01 721e 0000 0063  ..........r....c
+00000d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000d40: 0100 0000 4000 0000 730c 0000 0065 005a  ....@...s....e.Z
+00000d50: 0164 005a 0264 0153 0029 0272 0900 0000  .d.Z.d.S.).r....
+00000d60: 4e29 0372 1300 0000 7214 0000 0072 1500  N).r....r....r..
+00000d70: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+00000d80: 0072 1b00 0000 7209 0000 0062 0000 0073  .r....r....b...s
+00000d90: 0400 0000 0800 0401 7209 0000 0063 0000  ........r....c..
+00000da0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00000db0: 0000 4000 0000 732e 0000 0065 005a 0164  ..@...s....e.Z.d
+00000dc0: 005a 0255 0064 015a 0365 0465 0519 0065  .Z.U.d.Z.e.e...e
+00000dd0: 0664 023c 0065 0764 0383 0164 0464 0584  .d.<.e.d...d.d..
+00000de0: 0083 015a 0864 0653 0029 0772 0a00 0000  ...Z.d.S.).r....
+00000df0: 7a23 0a20 2020 204d 616e 6966 6573 7420  z#.    Manifest 
+00000e00: 7363 6865 6d61 2076 6572 7369 6f6e 2031  schema version 1
+00000e10: 0a20 2020 2072 2000 0000 721f 0000 0063  .    r ...r....c
+00000e20: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000e30: 0400 0000 4300 0000 731c 0000 007c 0164  ....C...s....|.d
+00000e40: 016b 0372 0c74 0064 027c 019b 0064 039d  .k.r.t.d.|...d..
+00000e50: 0383 0182 0164 0053 0029 044e da01 317a  .....d.S.).N..1z
+00000e60: 1e57 726f 6e67 206d 616e 6966 6573 7420  .Wrong manifest 
+00000e70: 7665 7273 696f 6e20 2867 6976 656e 20fa  version (given .
+00000e80: 0129 2901 7224 0000 0029 0272 2500 0000  .)).r$...).r%...
+00000e90: da05 7661 6c75 6572 1a00 0000 721a 0000  ..valuer....r...
+00000ea0: 0072 1b00 0000 da12 6d61 6e69 6665 7374  .r......manifest
+00000eb0: 5f76 6572 7369 6f6e 5f31 6d00 0000 7306  _version_1m...s.
+00000ec0: 0000 0008 0210 0104 ff7a 1d4d 616e 6966  .........z.Manif
+00000ed0: 6573 7456 312e 6d61 6e69 6665 7374 5f76  estV1.manifest_v
+00000ee0: 6572 7369 6f6e 5f31 4e29 0972 1300 0000  ersion_1N).r....
+00000ef0: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00000f00: 2900 0000 7209 0000 0072 1800 0000 7208  )...r....r....r.
+00000f10: 0000 0072 2e00 0000 721a 0000 0072 1a00  ...r....r....r..
+00000f20: 0000 721a 0000 0072 1b00 0000 720a 0000  ..r....r....r...
+00000f30: 0066 0000 0073 0a00 0000 0a00 0401 0c04  .f...s..........
+00000f40: 0602 0e01 720a 0000 004e 290f da06 7479  ....r....N)...ty
+00000f50: 7069 6e67 7202 0000 0072 0300 0000 7204  pingr....r....r.
+00000f60: 0000 00da 0870 7964 616e 7469 6372 0500  .....pydanticr..
+00000f70: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
+00000f80: 00da 075f 5f61 6c6c 5f5f 720b 0000 0072  ...__all__r....r
+00000f90: 1c00 0000 721e 0000 0072 0900 0000 720a  ....r....r....r.
+00000fa0: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+00000fb0: 0000 721b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000fc0: 3e01 0000 0073 1a00 0000 0c00 0c01 0c01  >....s..........
+00000fd0: 0c02 0c01 0c01 0c01 0403 1003 0c24 1003  .............$..
+00000fe0: 102d 1404                                .-..
```

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/project.cpython-39.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/project.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/state.cpython-39.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 26 06:48:59 2023 UTC, .py size: 2872 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5b56 7064 380b 0000  o.......[Vpd8...
+00000000: 6f0d 0d0a 0000 0000 faf1 8664 120a 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c03 6d06 5a06 0100 6406 6407 6c07  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6408 5a09 4700 6409 640a  m.Z...d.Z.G.d.d.
@@ -21,175 +21,150 @@
 00000140: 6461 7465 da08 5461 736b 5265 6164 da0a  date..TaskRead..
 00000150: 5461 736b 496d 706f 7274 da0a 5461 736b  TaskImport..Task
 00000160: 4578 706f 7274 6300 0000 0000 0000 0000  Exportc.........
 00000170: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
 00000180: 2e00 0000 6500 5a01 6400 5a02 5500 6401  ....e.Z.d.Z.U.d.
 00000190: 5a03 6504 6505 6402 3c00 6506 6402 6403  Z.e.e.d.<.e.d.d.
 000001a0: 6404 8d02 6507 6402 8301 8301 5a08 6405  d...e.d.....Z.d.
-000001b0: 5300 2906 da09 5f54 6173 6b42 6173 6561  S.)..._TaskBasea
-000001c0: e002 0000 2320 544f 444f 2066 6978 206d  ....# TODO fix m
-000001d0: 650a 2020 2020 5461 736b 2062 6173 6520  e.    Task base 
-000001e0: 636c 6173 730a 0a20 2020 2041 2054 6173  class..    A Tas
-000001f0: 6b20 6973 2074 6865 2065 6c65 6d65 6e74  k is the element
-00000200: 616c 2075 6e69 7420 6f66 2061 2077 6f72  al unit of a wor
-00000210: 6b66 6c6f 772c 2061 6e64 206d 7573 7420  kflow, and must 
-00000220: 6265 2061 2073 656c 662d 7374 616e 6469  be a self-standi
-00000230: 6e67 0a20 2020 2065 7865 6375 7461 626c  ng.    executabl
-00000240: 652e 0a0a 2020 2020 4174 7472 6962 7574  e...    Attribut
-00000250: 6573 0a20 2020 2020 2020 206e 616d 653a  es.        name:
-00000260: 0a20 2020 2020 2020 2020 2020 2041 2068  .            A h
-00000270: 756d 616e 2072 6561 6461 626c 6520 6e61  uman readable na
-00000280: 6d65 2066 6f72 2074 6865 2074 6173 6b0a  me for the task.
-00000290: 2020 2020 2020 2020 636f 6d6d 616e 643a          command:
-000002a0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-000002b0: 2063 6f6d 6d61 6e64 2873 2920 7468 6174   command(s) that
-000002c0: 2065 7865 6375 7465 7320 7468 6520 7461   executes the ta
-000002d0: 736b 0a20 2020 2020 2020 2073 6f75 7263  sk.        sourc
-000002e0: 653a 0a20 2020 2020 2020 2020 2020 2050  e:.            P
-000002f0: 6174 6820 6f72 2075 726c 2074 6f20 7461  ath or url to ta
-00000300: 736b 2073 6f75 7263 652e 2054 6869 7320  sk source. This 
-00000310: 6973 2074 6865 2069 6e66 6f72 6d61 7469  is the informati
-00000320: 6f6e 2069 7320 7573 6564 2074 6f0a 2020  on is used to.  
-00000330: 2020 2020 2020 2020 2020 6d61 7463 6820            match 
-00000340: 7461 736b 7320 6163 726f 7373 2066 7261  tasks across fra
-00000350: 6374 616c 2069 6e73 7461 6c6c 6174 696f  ctal installatio
-00000360: 6e73 2077 6865 6e20 6120 776f 726b 666c  ns when a workfl
-00000370: 6f77 2069 730a 2020 2020 2020 2020 2020  ow is.          
-00000380: 2020 696d 706f 7274 6564 2e0a 2020 2020    imported..    
-00000390: 2020 2020 696e 7075 745f 7479 7065 3a0a      input_type:.
-000003a0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-000003b0: 7479 7065 206f 6620 6461 7461 2074 6865  type of data the
-000003c0: 2074 6173 6b20 6578 7065 6374 7320 6173   task expects as
-000003d0: 2069 6e70 7574 0a20 2020 2020 2020 206f   input.        o
-000003e0: 7574 7075 745f 7479 7065 3a0a 2020 2020  utput_type:.    
-000003f0: 2020 2020 2020 2020 5468 6520 7479 7065          The type
-00000400: 206f 6620 6461 7461 2074 6865 2074 6173   of data the tas
-00000410: 6b20 6578 7065 6374 7320 6173 206f 7574  k expects as out
-00000420: 7075 740a 2020 2020 2020 2020 6465 6661  put.        defa
-00000430: 756c 745f 6172 6773 3a20 4f70 7469 6f6e  ult_args: Option
-00000440: 616c 5b64 6963 745b 7374 722c 2041 6e79  al[dict[str, Any
-00000450: 5d5d 0a20 2020 2020 2020 2020 2020 2064  ]].            d
-00000460: 6963 7469 6f6e 6172 7920 2873 6176 6564  ictionary (saved
-00000470: 2061 7320 4a53 4f4e 2920 6f66 2074 6865   as JSON) of the
-00000480: 2064 6566 6175 6c74 2070 6172 616d 6574   default paramet
-00000490: 6572 7320 6f66 2074 6865 2074 6173 6b0a  ers of the task.
-000004a0: 2020 2020 da06 736f 7572 6365 54a9 01da      ..sourceT...
-000004b0: 0b61 6c6c 6f77 5f72 6575 7365 4e29 09da  .allow_reuseN)..
-000004c0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000004d0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000004e0: 655f 5fda 075f 5f64 6f63 5f5f da03 7374  e__..__doc__..st
-000004f0: 72da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  r..__annotations
-00000500: 5f5f 7206 0000 0072 0800 0000 da07 5f73  __r....r......_s
-00000510: 6f75 7263 65a9 0072 1900 0000 7219 0000  ource..r....r...
-00000520: 00fa 3c2f 686f 6d65 2f74 6f6d 6d61 736f  ..</home/tommaso
-00000530: 2f46 7261 6374 616c 2f66 7261 6374 616c  /Fractal/fractal
-00000540: 2f66 7261 6374 616c 2f63 6f6d 6d6f 6e2f  /fractal/common/
-00000550: 7363 6865 6d61 732f 7461 736b 2e70 7972  schemas/task.pyr
-00000560: 0e00 0000 1300 0000 7308 0000 000a 0004  ........s.......
-00000570: 0108 1718 0172 0e00 0000 6300 0000 0000  .....r....c.....
-00000580: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
-00000590: 0000 0073 e200 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-000005a0: 5500 6503 6504 1900 6505 6401 3c00 6503  U.e.e...e.d.<.e.
-000005b0: 6504 1900 6505 6402 3c00 6503 6504 1900  e...e.d.<.e.e...
-000005c0: 6505 6403 3c00 6503 6504 1900 6505 6404  e.d.<.e.e...e.d.
-000005d0: 3c00 6503 6504 1900 6505 6405 3c00 6503  <.e.e...e.d.<.e.
-000005e0: 6506 6504 6507 6602 1900 1900 6505 6406  e.e.e.f.....e.d.
-000005f0: 3c00 6503 6506 6504 6507 6602 1900 1900  <.e.e.e.e.f.....
-00000600: 6505 6407 3c00 6503 6504 1900 6505 6408  e.d.<.e.e...e.d.
-00000610: 3c00 6508 6401 6409 640a 8d02 6509 6401  <.e.d.d.d...e.d.
-00000620: 8301 8301 5a0a 6508 6402 6409 640a 8d02  ....Z.e.d.d.d...
-00000630: 6509 6402 8301 8301 5a0b 6508 6403 6409  e.d.....Z.e.d.d.
-00000640: 640a 8d02 6509 6403 8301 8301 5a0c 6508  d...e.d.....Z.e.
-00000650: 6404 6409 640a 8d02 6509 6404 8301 8301  d.d.d...e.d.....
-00000660: 5a0d 6508 6408 6409 640a 8d02 6509 6408  Z.e.d.d.d...e.d.
-00000670: 8301 8301 5a0e 640b 5300 290c 720a 0000  ....Z.d.S.).r...
-00000680: 00da 046e 616d 65da 0a69 6e70 7574 5f74  ...name..input_t
-00000690: 7970 65da 0b6f 7574 7075 745f 7479 7065  ype..output_type
-000006a0: da07 636f 6d6d 616e 6472 0f00 0000 da0c  ..commandr......
-000006b0: 6465 6661 756c 745f 6172 6773 da04 6d65  default_args..me
-000006c0: 7461 da07 7665 7273 696f 6e54 7210 0000  ta..versionTr...
-000006d0: 004e 290f 7212 0000 0072 1300 0000 7214  .N).r....r....r.
-000006e0: 0000 0072 0300 0000 7216 0000 0072 1700  ...r....r....r..
-000006f0: 0000 da04 6469 6374 7202 0000 0072 0600  ....dictr....r..
-00000700: 0000 7208 0000 00da 055f 6e61 6d65 da0b  ..r......_name..
-00000710: 5f69 6e70 7574 5f74 7970 65da 0c5f 6f75  _input_type.._ou
-00000720: 7470 7574 5f74 7970 65da 085f 636f 6d6d  tput_type.._comm
-00000730: 616e 64da 085f 7665 7273 696f 6e72 1900  and.._versionr..
-00000740: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000750: 0072 0a00 0000 2f00 0000 7324 0000 000a  .r..../...s$....
-00000760: 000c 010c 010c 010c 010c 0114 0114 010c  ................
-00000770: 0114 030a 0106 0104 ff0a 0306 0104 ff14  ................
-00000780: 0318 0172 0a00 0000 6300 0000 0000 0000  ...r....c.......
-00000790: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-000007a0: 00f3 0c00 0000 6500 5a01 6400 5a02 6401  ......e.Z.d.Z.d.
-000007b0: 5300 2902 720c 0000 004e a903 7212 0000  S.).r....N..r...
-000007c0: 0072 1300 0000 7214 0000 0072 1900 0000  .r....r....r....
-000007d0: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-000007e0: 0c00 0000 4500 0000 f304 0000 0008 0004  ....E...........
-000007f0: 0172 0c00 0000 6300 0000 0000 0000 0000  .r....c.........
-00000800: 0000 0000 0000 0001 0000 0040 0000 0072  ...........@...r
-00000810: 2800 0000 2902 720d 0000 004e 7229 0000  (...).r....Nr)..
-00000820: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
-00000830: 721a 0000 0072 0d00 0000 4900 0000 722a  r....r....I...r*
-00000840: 0000 0072 0d00 0000 6300 0000 0000 0000  ...r....c.......
-00000850: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000860: 0073 8a00 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
-00000870: 6503 6504 6401 3c00 6505 6504 6402 3c00  e.e.d.<.e.e.d.<.
-00000880: 6505 6504 6403 3c00 6505 6504 6404 3c00  e.e.d.<.e.e.d.<.
-00000890: 6505 6504 6405 3c00 6506 6900 6406 8d01  e.e.d.<.e.i.d...
-000008a0: 5a07 6508 6509 6505 650a 6602 1900 1900  Z.e.e.e.e.f.....
-000008b0: 6504 6407 3c00 6506 6900 6406 8d01 5a0b  e.d.<.e.i.d...Z.
-000008c0: 6508 6509 6505 650a 6602 1900 1900 6504  e.e.e.e.f.....e.
-000008d0: 6408 3c00 6508 6505 1900 6504 6409 3c00  d.<.e.e...e.d.<.
-000008e0: 6508 6505 1900 6504 640a 3c00 640b 5300  e.e...e.d.<.d.S.
-000008f0: 290c 720b 0000 00da 0269 6472 1b00 0000  ).r......idr....
-00000900: 721e 0000 0072 1c00 0000 721d 0000 00a9  r....r....r.....
-00000910: 01da 0764 6566 6175 6c74 721f 0000 0072  ...defaultr....r
-00000920: 2000 0000 da05 6f77 6e65 7272 2100 0000   .....ownerr!...
-00000930: 4e29 0c72 1200 0000 7213 0000 0072 1400  N).r....r....r..
-00000940: 0000 da03 696e 7472 1700 0000 7216 0000  ....intr....r...
-00000950: 0072 0500 0000 721f 0000 0072 0300 0000  .r....r....r....
-00000960: 7222 0000 0072 0200 0000 7220 0000 0072  r"...r....r ...r
-00000970: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
-00000980: 0000 0072 0b00 0000 4d00 0000 7314 0000  ...r....M...s...
-00000990: 000a 0008 0108 0108 0108 0108 011e 011e  ................
-000009a0: 010c 0110 0172 0b00 0000 6300 0000 0000  .....r....c.....
-000009b0: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
-000009c0: 0000 0073 da00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-000009d0: 5500 6503 6504 6401 3c00 6503 6504 6402  U.e.e.d.<.e.e.d.
-000009e0: 3c00 6503 6504 6403 3c00 6503 6504 6404  <.e.e.d.<.e.e.d.
-000009f0: 3c00 6505 6900 6405 8d01 5a06 6507 6508  <.e.i.d...Z.e.e.
-00000a00: 6503 6509 6602 1900 1900 6504 6406 3c00  e.e.f.....e.d.<.
-00000a10: 6505 6900 6405 8d01 5a0a 6507 6508 6503  e.i.d...Z.e.e.e.
-00000a20: 6509 6602 1900 1900 6504 6407 3c00 6507  e.f.....e.d.<.e.
-00000a30: 6503 1900 6504 6408 3c00 650b 6401 6409  e...e.d.<.e.d.d.
-00000a40: 640a 8d02 650c 6401 8301 8301 5a0d 650b  d...e.d.....Z.e.
-00000a50: 6403 6409 640a 8d02 650c 6403 8301 8301  d.d.d...e.d.....
-00000a60: 5a0e 650b 6404 6409 640a 8d02 650c 6404  Z.e.d.d.d...e.d.
-00000a70: 8301 8301 5a0f 650b 6402 6409 640a 8d02  ....Z.e.d.d.d...
-00000a80: 650c 6402 8301 8301 5a10 650b 6408 6409  e.d.....Z.e.d.d.
-00000a90: 640a 8d02 650c 6408 8301 8301 5a11 640b  d...e.d.....Z.d.
-00000aa0: 5300 290c 7209 0000 0072 1b00 0000 721e  S.).r....r....r.
-00000ab0: 0000 0072 1c00 0000 721d 0000 0072 2c00  ...r....r....r,.
-00000ac0: 0000 721f 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
-00000ad0: 0054 7210 0000 004e 2912 7212 0000 0072  .Tr....N).r....r
-00000ae0: 1300 0000 7214 0000 0072 1600 0000 7217  ....r....r....r.
-00000af0: 0000 0072 0500 0000 721f 0000 0072 0300  ...r....r....r..
-00000b00: 0000 7222 0000 0072 0200 0000 7220 0000  ..r"...r....r ..
-00000b10: 0072 0600 0000 7208 0000 0072 2300 0000  .r....r....r#...
-00000b20: 7224 0000 0072 2500 0000 7226 0000 0072  r$...r%...r&...r
-00000b30: 2700 0000 7219 0000 0072 1900 0000 7219  '...r....r....r.
-00000b40: 0000 0072 1a00 0000 7209 0000 0059 0000  ...r....r....Y..
-00000b50: 0073 2200 0000 0a00 0801 0801 0801 0801  .s".............
-00000b60: 1e01 1e01 0c01 1403 0a01 0601 04ff 0a03  ................
-00000b70: 0601 04ff 1403 1801 7209 0000 004e 2910  ........r....N).
-00000b80: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
-00000b90: 0000 da08 7079 6461 6e74 6963 7204 0000  ....pydanticr...
-00000ba0: 0072 0500 0000 7206 0000 00da 0b5f 7661  .r....r......_va
-00000bb0: 6c69 6461 746f 7273 7208 0000 00da 075f  lidatorsr......_
-00000bc0: 5f61 6c6c 5f5f 720e 0000 0072 0a00 0000  _all__r....r....
-00000bd0: 720c 0000 0072 0d00 0000 720b 0000 0072  r....r....r....r
-00000be0: 0900 0000 7219 0000 0072 1900 0000 7219  ....r....r....r.
-00000bf0: 0000 0072 1a00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000c00: 653e 0100 0000 731a 0000 000c 000c 010c  e>....s.........
-00000c10: 020c 010c 010c 0204 0210 0910 1c10 1610  ................
-00000c20: 0410 0414 0c                             .....
+000001b0: 5300 2906 da09 5f54 6173 6b42 6173 657a  S.)..._TaskBasez
+000001c0: f50a 0a20 2020 2042 6173 6520 636c 6173  ...    Base clas
+000001d0: 7320 666f 7220 6054 6173 6b60 2061 6e64  s for `Task` and
+000001e0: 2060 5461 736b 7b43 7265 6174 652c 5265   `Task{Create,Re
+000001f0: 6164 2c55 7064 6174 652c 496d 706f 7274  ad,Update,Import
+00000200: 2c45 7870 6f72 747d 6020 6d6f 6465 6c73  ,Export}` models
+00000210: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
+00000220: 0a20 2020 2020 2020 2073 6f75 7263 653a  .        source:
+00000230: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
+00000240: 7320 6973 2074 6865 2069 6e66 6f72 6d61  s is the informa
+00000250: 7469 6f6e 2069 7320 7573 6564 2074 6f20  tion is used to 
+00000260: 6d61 7463 6820 7461 736b 7320 6163 726f  match tasks acro
+00000270: 7373 2066 7261 6374 616c 0a20 2020 2020  ss fractal.     
+00000280: 2020 2020 2020 2069 6e73 7461 6c6c 6174         installat
+00000290: 696f 6e73 2077 6865 6e20 6120 776f 726b  ions when a work
+000002a0: 666c 6f77 2069 7320 696d 706f 7274 6564  flow is imported
+000002b0: 2e0a 2020 2020 da06 736f 7572 6365 54a9  ..    ..sourceT.
+000002c0: 01da 0b61 6c6c 6f77 5f72 6575 7365 4e29  ...allow_reuseN)
+000002d0: 09da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000002e0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000002f0: 616d 655f 5fda 075f 5f64 6f63 5f5f da03  ame__..__doc__..
+00000300: 7374 72da 0f5f 5f61 6e6e 6f74 6174 696f  str..__annotatio
+00000310: 6e73 5f5f 7206 0000 0072 0800 0000 da07  ns__r....r......
+00000320: 5f73 6f75 7263 65a9 0072 1900 0000 7219  _source..r....r.
+00000330: 0000 00fa 3c2f 686f 6d65 2f74 6f6d 6d61  ....</home/tomma
+00000340: 736f 2f46 7261 6374 616c 2f66 7261 6374  so/Fractal/fract
+00000350: 616c 2f66 7261 6374 616c 2f63 6f6d 6d6f  al/fractal/commo
+00000360: 6e2f 7363 6865 6d61 732f 7461 736b 2e70  n/schemas/task.p
+00000370: 7972 0e00 0000 1300 0000 7308 0000 000a  yr........s.....
+00000380: 0004 0108 0a18 0172 0e00 0000 6300 0000  .......r....c...
+00000390: 0000 0000 0000 0000 0000 0000 0004 0000  ................
+000003a0: 0040 0000 0073 ee00 0000 6500 5a01 6400  .@...s....e.Z.d.
+000003b0: 5a02 5500 6503 6504 1900 6505 6401 3c00  Z.U.e.e...e.d.<.
+000003c0: 6503 6504 1900 6505 6402 3c00 6503 6504  e.e...e.d.<.e.e.
+000003d0: 1900 6505 6403 3c00 6503 6504 1900 6505  ..e.d.<.e.e...e.
+000003e0: 6404 3c00 6503 6504 1900 6505 6405 3c00  d.<.e.e...e.d.<.
+000003f0: 6503 6506 6504 6507 6602 1900 1900 6505  e.e.e.e.f.....e.
+00000400: 6406 3c00 6503 6504 1900 6505 6407 3c00  d.<.e.e...e.d.<.
+00000410: 6503 6506 6504 6507 6602 1900 1900 6505  e.e.e.e.f.....e.
+00000420: 6408 3c00 6503 6504 1900 6505 6409 3c00  d.<.e.e...e.d.<.
+00000430: 6508 6401 640a 640b 8d02 6509 6401 8301  e.d.d.d...e.d...
+00000440: 8301 5a0a 6508 6402 640a 640b 8d02 6509  ..Z.e.d.d.d...e.
+00000450: 6402 8301 8301 5a0b 6508 6403 640a 640b  d.....Z.e.d.d.d.
+00000460: 8d02 6509 6403 8301 8301 5a0c 6508 6404  ..e.d.....Z.e.d.
+00000470: 640a 640b 8d02 6509 6404 8301 8301 5a0d  d.d...e.d.....Z.
+00000480: 6508 6407 640a 640b 8d02 6509 6407 8301  e.d.d.d...e.d...
+00000490: 8301 5a0e 640c 5300 290d 720a 0000 00da  ..Z.d.S.).r.....
+000004a0: 046e 616d 65da 0a69 6e70 7574 5f74 7970  .name..input_typ
+000004b0: 65da 0b6f 7574 7075 745f 7479 7065 da07  e..output_type..
+000004c0: 636f 6d6d 616e 6472 0f00 0000 da04 6d65  commandr......me
+000004d0: 7461 da07 7665 7273 696f 6eda 0b61 7267  ta..version..arg
+000004e0: 735f 7363 6865 6d61 da13 6172 6773 5f73  s_schema..args_s
+000004f0: 6368 656d 615f 7665 7273 696f 6e54 7210  chema_versionTr.
+00000500: 0000 004e 290f 7212 0000 0072 1300 0000  ...N).r....r....
+00000510: 7214 0000 0072 0300 0000 7216 0000 0072  r....r....r....r
+00000520: 1700 0000 da04 6469 6374 7202 0000 0072  ......dictr....r
+00000530: 0600 0000 7208 0000 00da 055f 6e61 6d65  ....r......_name
+00000540: da0b 5f69 6e70 7574 5f74 7970 65da 0c5f  .._input_type.._
+00000550: 6f75 7470 7574 5f74 7970 65da 085f 636f  output_type.._co
+00000560: 6d6d 616e 64da 085f 7665 7273 696f 6e72  mmand.._versionr
+00000570: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
+00000580: 0000 0072 0a00 0000 2200 0000 7326 0000  ...r...."...s&..
+00000590: 000a 000c 010c 010c 010c 010c 0114 010c  ................
+000005a0: 0114 010c 0114 030a 0106 0104 ff0a 0306  ................
+000005b0: 0104 ff14 0318 0172 0a00 0000 6300 0000  .......r....c...
+000005c0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+000005d0: 0040 0000 00f3 0c00 0000 6500 5a01 6400  .@........e.Z.d.
+000005e0: 5a02 6401 5300 2902 720c 0000 004e a903  Z.d.S.).r....N..
+000005f0: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000600: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
+00000610: 0000 0072 0c00 0000 3900 0000 f304 0000  ...r....9.......
+00000620: 0008 0004 0172 0c00 0000 6300 0000 0000  .....r....c.....
+00000630: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+00000640: 0000 0072 2900 0000 2902 720d 0000 004e  ...r)...).r....N
+00000650: 722a 0000 0072 1900 0000 7219 0000 0072  r*...r....r....r
+00000660: 1900 0000 721a 0000 0072 0d00 0000 3d00  ....r....r....=.
+00000670: 0000 722b 0000 0072 0d00 0000 6300 0000  ..r+...r....c...
+00000680: 0000 0000 0000 0000 0000 0000 0004 0000  ................
+00000690: 0040 0000 0073 8c00 0000 6500 5a01 6400  .@...s....e.Z.d.
+000006a0: 5a02 5500 6503 6504 6401 3c00 6505 6504  Z.U.e.e.d.<.e.e.
+000006b0: 6402 3c00 6505 6504 6403 3c00 6505 6504  d.<.e.e.d.<.e.e.
+000006c0: 6404 3c00 6505 6504 6405 3c00 6506 6900  d.<.e.e.d.<.e.i.
+000006d0: 6406 8d01 5a07 6508 6509 6505 650a 6602  d...Z.e.e.e.e.f.
+000006e0: 1900 1900 6504 6407 3c00 6508 6505 1900  ....e.d.<.e.e...
+000006f0: 6504 6408 3c00 6508 6505 1900 6504 6409  e.d.<.e.e...e.d.
+00000700: 3c00 6508 6509 6505 650a 6602 1900 1900  <.e.e.e.e.f.....
+00000710: 6504 640a 3c00 6508 6505 1900 6504 640b  e.d.<.e.e...e.d.
+00000720: 3c00 640c 5300 290d 720b 0000 00da 0269  <.d.S.).r......i
+00000730: 6472 1b00 0000 721e 0000 0072 1c00 0000  dr....r....r....
+00000740: 721d 0000 00a9 01da 0764 6566 6175 6c74  r........default
+00000750: 721f 0000 00da 056f 776e 6572 7220 0000  r......ownerr ..
+00000760: 0072 2100 0000 7222 0000 004e 290b 7212  .r!...r"...N).r.
+00000770: 0000 0072 1300 0000 7214 0000 00da 0369  ...r....r......i
+00000780: 6e74 7217 0000 0072 1600 0000 7205 0000  ntr....r....r...
+00000790: 0072 1f00 0000 7203 0000 0072 2300 0000  .r....r....r#...
+000007a0: 7202 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+000007b0: 1900 0000 721a 0000 0072 0b00 0000 4100  ....r....r....A.
+000007c0: 0000 7316 0000 000a 0008 0108 0108 0108  ..s.............
+000007d0: 0108 011e 010c 010c 0114 0110 0172 0b00  .............r..
+000007e0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000007f0: 0000 0004 0000 0040 0000 0073 f000 0000  .......@...s....
+00000800: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
+00000810: 3c00 6503 6504 6402 3c00 6503 6504 6403  <.e.e.d.<.e.e.d.
+00000820: 3c00 6503 6504 6404 3c00 6505 6900 6405  <.e.e.d.<.e.i.d.
+00000830: 8d01 5a06 6507 6508 6503 6509 6602 1900  ..Z.e.e.e.e.f...
+00000840: 1900 6504 6406 3c00 6507 6503 1900 6504  ..e.d.<.e.e...e.
+00000850: 6407 3c00 6507 6508 6503 6509 6602 1900  d.<.e.e.e.e.f...
+00000860: 1900 6504 6408 3c00 6507 6503 1900 6504  ..e.d.<.e.e...e.
+00000870: 6409 3c00 650a 6401 640a 640b 8d02 650b  d.<.e.d.d.d...e.
+00000880: 6401 8301 8301 5a0c 650a 6403 640a 640b  d.....Z.e.d.d.d.
+00000890: 8d02 650b 6403 8301 8301 5a0d 650a 6404  ..e.d.....Z.e.d.
+000008a0: 640a 640b 8d02 650b 6404 8301 8301 5a0e  d.d...e.d.....Z.
+000008b0: 650a 6402 640a 640b 8d02 650b 6402 8301  e.d.d.d...e.d...
+000008c0: 8301 5a0f 650a 6407 640a 640b 8d02 650b  ..Z.e.d.d.d...e.
+000008d0: 6407 8301 8301 5a10 650a 6409 640a 640b  d.....Z.e.d.d.d.
+000008e0: 8d02 650b 6409 8301 8301 5a11 640c 5300  ..e.d.....Z.d.S.
+000008f0: 290d 7209 0000 0072 1b00 0000 721e 0000  ).r....r....r...
+00000900: 0072 1c00 0000 721d 0000 0072 2d00 0000  .r....r....r-...
+00000910: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
+00000920: 2200 0000 5472 1000 0000 4e29 1272 1200  "...Tr....N).r..
+00000930: 0000 7213 0000 0072 1400 0000 7216 0000  ..r....r....r...
+00000940: 0072 1700 0000 7205 0000 0072 1f00 0000  .r....r....r....
+00000950: 7203 0000 0072 2300 0000 7202 0000 0072  r....r#...r....r
+00000960: 0600 0000 7208 0000 0072 2400 0000 7225  ....r....r$...r%
+00000970: 0000 0072 2600 0000 7227 0000 0072 2800  ...r&...r'...r(.
+00000980: 0000 da14 5f61 7267 735f 7363 6865 6d61  ...._args_schema
+00000990: 5f76 6572 7369 6f6e 7219 0000 0072 1900  _versionr....r..
+000009a0: 0000 7219 0000 0072 1a00 0000 7209 0000  ..r....r....r...
+000009b0: 004e 0000 0073 2a00 0000 0a00 0801 0801  .N...s*.........
+000009c0: 0801 0801 1e01 0c01 1401 0c01 1403 0a01  ................
+000009d0: 0601 04ff 0a03 0601 04ff 1403 1401 0a01  ................
+000009e0: 0601 08ff 7209 0000 004e 2910 da06 7479  ....r....N)...ty
+000009f0: 7069 6e67 7202 0000 0072 0300 0000 da08  pingr....r......
+00000a00: 7079 6461 6e74 6963 7204 0000 0072 0500  pydanticr....r..
+00000a10: 0000 7206 0000 00da 0b5f 7661 6c69 6461  ..r......_valida
+00000a20: 746f 7273 7208 0000 00da 075f 5f61 6c6c  torsr......__all
+00000a30: 5f5f 720e 0000 0072 0a00 0000 720c 0000  __r....r....r...
+00000a40: 0072 0d00 0000 720b 0000 0072 0900 0000  .r....r....r....
+00000a50: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00000a60: 1a00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000a70: 0000 731a 0000 000c 000c 010c 020c 010c  ..s.............
+00000a80: 010c 0204 0210 0910 0f10 1710 0410 0414  ................
+00000a90: 0d                                       .
```

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/task.cpython-39.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/task.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 25 12:31:57 2023 UTC, .py size: 2741 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3d55 6f64 b50a 0000  o.......=Uod....
+00000000: 6f0d 0d0a 0000 0000 faf1 8664 770b 0000  o..........dw...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c05 6d07 5a07 0100 6400 6406 6c05  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6407 6408 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
@@ -29,166 +29,178 @@
 000001c0: fa47 2f68 6f6d 652f 746f 6d6d 6173 6f2f  .G/home/tommaso/
 000001d0: 4672 6163 7461 6c2f 6672 6163 7461 6c2f  Fractal/fractal/
 000001e0: 6672 6163 7461 6c2f 636f 6d6d 6f6e 2f73  fractal/common/s
 000001f0: 6368 656d 6173 2f74 6173 6b5f 636f 6c6c  chemas/task_coll
 00000200: 6563 7469 6f6e 2e70 7972 0d00 0000 1200  ection.pyr......
 00000210: 0000 7304 0000 0008 0004 0172 0d00 0000  ..s........r....
 00000220: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000230: 0004 0000 0040 0000 0073 9600 0000 6500  .....@...s....e.
+00000230: 0004 0000 0040 0000 0073 ae00 0000 6500  .....@...s....e.
 00000240: 5a01 6400 5a02 5500 6401 5a03 6504 6505  Z.d.Z.U.d.Z.e.e.
 00000250: 6402 3c00 6403 5a06 6507 6504 1900 6505  d.<.d.Z.e.e...e.
 00000260: 6404 3c00 6403 5a08 6507 6504 1900 6505  d.<.d.Z.e.e...e.
 00000270: 6405 3c00 6403 5a09 6507 6504 1900 6505  d.<.d.Z.e.e...e.
-00000280: 6406 3c00 650a 6404 6407 6408 8d02 650b  d.<.e.d.d.d...e.
-00000290: 6404 8301 8301 5a0c 650a 6405 6407 6408  d.....Z.e.d.d.d.
-000002a0: 8d02 650b 6405 8301 8301 5a0d 650a 6406  ..e.d.....Z.e.d.
-000002b0: 6407 6408 8d02 650b 6406 8301 8301 5a0e  d.d...e.d.....Z.
-000002c0: 650a 6402 8301 6409 640a 8400 8301 5a0f  e.d...d.d.....Z.
-000002d0: 6403 5300 290b 720b 0000 0061 e002 0000  d.S.).r....a....
-000002e0: 0a20 2020 2054 6173 6b43 6f6c 6c65 6374  .    TaskCollect
-000002f0: 5069 7020 636c 6173 730a 0a20 2020 2054  Pip class..    T
-00000300: 6869 7320 636c 6173 7320 6f6e 6c79 2065  his class only e
-00000310: 6e63 6f64 6573 2074 6865 2061 7474 7269  ncodes the attri
-00000320: 6275 7465 7320 7265 7175 6972 6564 2074  butes required t
-00000330: 6f20 7472 6967 6765 7220 610a 2020 2020  o trigger a.    
-00000340: 7461 736b 2d63 6f6c 6c65 6374 696f 6e20  task-collection 
-00000350: 6f70 6572 6174 696f 6e2e 204f 7468 6572  operation. Other
-00000360: 2061 7474 7269 6275 7465 7320 2874 6861   attributes (tha
-00000370: 7420 6172 6520 6173 7369 676e 6564 202a  t are assigned *
-00000380: 6475 7269 6e67 2a0a 2020 2020 7461 736b  during*.    task
-00000390: 2063 6f6c 6c65 6374 696f 6e29 2061 7265   collection) are
-000003a0: 2064 6566 696e 6564 2061 7320 7061 7274   defined as part
-000003b0: 206f 6620 6672 6163 7461 6c2d 7365 7276   of fractal-serv
-000003c0: 6572 2e0a 0a20 2020 2054 776f 2063 6173  er...    Two cas
-000003d0: 6573 2061 7265 2073 7570 706f 7274 6564  es are supported
-000003e0: 3a0a 0a20 2020 2020 2020 2031 2e20 6070  :..        1. `p
-000003f0: 6163 6b61 6765 6020 6973 2074 6865 2070  ackage` is the p
-00000400: 6174 6820 6f66 2061 206c 6f63 616c 2077  ath of a local w
-00000410: 6865 656c 2066 696c 653b 0a20 2020 2020  heel file;.     
-00000420: 2020 2032 2e20 6070 6163 6b61 6765 6020     2. `package` 
-00000430: 6973 2074 6865 206e 616d 6520 6f66 2061  is the name of a
-00000440: 2070 6163 6b61 6765 2074 6861 7420 6361   package that ca
-00000450: 6e20 6265 2069 6e73 7461 6c6c 6564 2076  n be installed v
-00000460: 6961 2060 7069 7060 2e0a 0a0a 2020 2020  ia `pip`....    
-00000470: 4174 7472 6962 7574 6573 3a0a 2020 2020  Attributes:.    
-00000480: 2020 2020 7061 636b 6167 653a 0a20 2020      package:.   
-00000490: 2020 2020 2020 2020 2054 6865 206e 616d           The nam
-000004a0: 6520 6f66 2061 2060 7069 7060 2d69 6e73  e of a `pip`-ins
-000004b0: 7461 6c6c 6162 6c65 2070 6163 6b61 6765  tallable package
-000004c0: 2c20 6f72 2074 6865 2070 6174 6820 746f  , or the path to
-000004d0: 2061 206c 6f63 616c 0a20 2020 2020 2020   a local.       
-000004e0: 2020 2020 2077 6865 656c 2066 696c 652e       wheel file.
-000004f0: 0a20 2020 2020 2020 2070 6163 6b61 6765  .        package
-00000500: 5f76 6572 7369 6f6e 3a20 5665 7273 696f  _version: Versio
-00000510: 6e20 6f66 2074 6865 2070 6163 6b61 6765  n of the package
-00000520: 0a20 2020 2020 2020 2070 6163 6b61 6765  .        package
-00000530: 5f65 7874 7261 733a 2050 6163 6b61 6765  _extras: Package
-00000540: 2065 7874 7261 7320 746f 2069 6e63 6c75   extras to inclu
-00000550: 6465 2069 6e20 7468 6520 6070 6970 2069  de in the `pip i
-00000560: 6e73 7461 6c6c 6020 636f 6d6d 616e 640a  nstall` command.
-00000570: 2020 2020 2020 2020 7079 7468 6f6e 5f76          python_v
-00000580: 6572 7369 6f6e 3a20 5079 7468 6f6e 2076  ersion: Python v
-00000590: 6572 7369 6f6e 2074 6f20 696e 7374 616c  ersion to instal
-000005a0: 6c20 616e 6420 7275 6e20 7468 6520 7061  l and run the pa
-000005b0: 636b 6167 6520 7461 736b 730a 2020 2020  ckage tasks.    
-000005c0: da07 7061 636b 6167 654e da0f 7061 636b  ..packageN..pack
-000005d0: 6167 655f 7665 7273 696f 6eda 0e70 6163  age_version..pac
-000005e0: 6b61 6765 5f65 7874 7261 73da 0e70 7974  kage_extras..pyt
-000005f0: 686f 6e5f 7665 7273 696f 6e54 2901 da0b  hon_versionT)...
-00000600: 616c 6c6f 775f 7265 7573 6563 0200 0000  allow_reusec....
-00000610: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000620: 4300 0000 7342 0000 0064 017c 0176 0072  C...sB...d.|.v.r
-00000630: 1f7c 01a0 0064 02a1 0173 1174 0164 037c  .|...d...s.t.d.|
-00000640: 019b 0064 049d 0383 0182 0174 027c 0183  ...d.......t.|..
-00000650: 01a0 03a1 0073 1f74 0164 057c 019b 0064  .....s.t.d.|...d
-00000660: 049d 0383 0182 017c 0153 0029 064e fa01  .......|.S.).N..
-00000670: 2f7a 042e 7768 6c7a 2f4c 6f63 616c 2d70  /z..whlz/Local-p
-00000680: 6163 6b61 6765 2070 6174 6820 6d75 7374  ackage path must
-00000690: 2062 6520 6120 7768 6565 6c20 6669 6c65   be a wheel file
-000006a0: 2028 6769 7665 6e20 7a02 292e 7a2c 4c6f   (given z.).z,Lo
-000006b0: 6361 6c2d 7061 636b 6167 6520 7061 7468  cal-package path
-000006c0: 206d 7573 7420 6265 2061 6273 6f6c 7574   must be absolut
-000006d0: 653a 2028 6769 7665 6e20 2904 da08 656e  e: (given )...en
-000006e0: 6473 7769 7468 da0a 5661 6c75 6545 7272  dswith..ValueErr
-000006f0: 6f72 7202 0000 00da 0b69 735f 6162 736f  orr......is_abso
-00000700: 6c75 7465 2902 da03 636c 73da 0576 616c  lute)...cls..val
-00000710: 7565 7211 0000 0072 1100 0000 7212 0000  uer....r....r...
-00000720: 00da 1170 6163 6b61 6765 5f76 616c 6964  ...package_valid
-00000730: 6174 6f72 3c00 0000 7318 0000 0008 020a  ator<...s.......
-00000740: 0102 0102 0102 0106 ff04 ff0c 0402 010a  ................
-00000750: 0104 ff04 037a 2054 6173 6b43 6f6c 6c65  .....z TaskColle
-00000760: 6374 5069 702e 7061 636b 6167 655f 7661  ctPip.package_va
-00000770: 6c69 6461 746f 7229 1072 0e00 0000 720f  lidator).r....r.
-00000780: 0000 0072 1000 0000 da07 5f5f 646f 635f  ...r......__doc_
-00000790: 5fda 0373 7472 da0f 5f5f 616e 6e6f 7461  _..str..__annota
-000007a0: 7469 6f6e 735f 5f72 1400 0000 7204 0000  tions__r....r...
-000007b0: 0072 1500 0000 7216 0000 0072 0700 0000  .r....r....r....
-000007c0: 7209 0000 00da 105f 7061 636b 6167 655f  r......_package_
-000007d0: 7665 7273 696f 6eda 0f5f 7061 636b 6167  version.._packag
-000007e0: 655f 6578 7472 6173 da0f 5f70 7974 686f  e_extras.._pytho
-000007f0: 6e5f 7665 7273 696f 6e72 1e00 0000 7211  n_versionr....r.
-00000800: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-00000810: 0000 720b 0000 0016 0000 0073 2200 0000  ..r........s"...
-00000820: 0a00 0401 0816 1001 1001 1001 0a02 0601  ................
-00000830: 04ff 0a03 0601 04ff 0a03 0601 04ff 0604  ................
-00000840: 0e01 720b 0000 0063 0000 0000 0000 0000  ..r....c........
-00000850: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000860: 7368 0000 0065 005a 0164 005a 0255 0064  sh...e.Z.d.Z.U.d
-00000870: 015a 0365 0464 0219 0065 0564 033c 0065  .Z.e.d...e.d.<.e
-00000880: 0665 0564 043c 0065 0765 0564 053c 0065  .e.d.<.e.e.d.<.e
-00000890: 0867 0064 068d 015a 0965 0a65 0b65 0c19  .g.d...Z.e.e.e..
-000008a0: 0019 0065 0564 073c 0065 0a65 0619 0065  ...e.d.<.e.e...e
-000008b0: 0564 083c 0065 0a65 0619 0065 0564 093c  .d.<.e.e...e.d.<
-000008c0: 0064 0a64 0b84 005a 0d64 0c53 0029 0d72  .d.d...Z.d.S.).r
-000008d0: 0c00 0000 7aac 0a20 2020 2054 6173 6b43  ....z..    TaskC
-000008e0: 6f6c 6c65 6374 5374 6174 7573 2063 6c61  ollectStatus cla
-000008f0: 7373 0a0a 2020 2020 4174 7472 6962 7574  ss..    Attribut
-00000900: 6573 3a0a 2020 2020 2020 2020 7374 6174  es:.        stat
-00000910: 7573 3a20 5442 440a 2020 2020 2020 2020  us: TBD.        
-00000920: 7061 636b 6167 653a 2054 4244 0a20 2020  package: TBD.   
-00000930: 2020 2020 2076 656e 765f 7061 7468 3a20       venv_path: 
-00000940: 5442 440a 2020 2020 2020 2020 7461 736b  TBD.        task
-00000950: 5f6c 6973 743a 2054 4244 0a20 2020 2020  _list: TBD.     
-00000960: 2020 206c 6f67 3a20 5442 440a 2020 2020     log: TBD.    
-00000970: 2020 2020 696e 666f 3a20 5442 440a 2020      info: TBD.  
-00000980: 2020 2905 da07 7065 6e64 696e 67da 0a69    )...pending..i
-00000990: 6e73 7461 6c6c 696e 67da 0a63 6f6c 6c65  nstalling..colle
-000009a0: 6374 696e 67da 0466 6169 6cda 024f 4bda  cting..fail..OK.
-000009b0: 0673 7461 7475 7372 1300 0000 da09 7665  .statusr......ve
-000009c0: 6e76 5f70 6174 6829 01da 0764 6566 6175  nv_path)...defau
-000009d0: 6c74 da09 7461 736b 5f6c 6973 74da 036c  lt..task_list..l
-000009e0: 6f67 da04 696e 666f 6301 0000 0000 0000  og..infoc.......
-000009f0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00000a00: 0073 1a00 0000 7c00 a000 a100 7d01 7401  .s....|.....}.t.
-00000a10: 7c00 6a02 8301 7c01 6401 3c00 7c01 5300  |.j...|.d.<.|.S.
-00000a20: 2902 7a51 0a20 2020 2020 2020 2052 6574  ).zQ.        Ret
-00000a30: 7572 6e20 6073 656c 662e 6469 6374 2829  urn `self.dict()
-00000a40: 6020 6166 7465 7220 6361 7374 696e 6720  ` after casting 
-00000a50: 6073 656c 662e 7665 6e76 5f70 6174 6860  `self.venv_path`
-00000a60: 2074 6f20 6120 7374 7269 6e67 0a20 2020   to a string.   
-00000a70: 2020 2020 2072 2b00 0000 2903 da04 6469       r+...)...di
-00000a80: 6374 7220 0000 0072 2b00 0000 2902 da04  ctr ...r+...)...
-00000a90: 7365 6c66 da01 6472 1100 0000 7211 0000  self..dr....r...
-00000aa0: 0072 1200 0000 da0e 7361 6e69 7469 7365  .r......sanitise
-00000ab0: 645f 6469 6374 5f00 0000 7306 0000 0008  d_dict_...s.....
-00000ac0: 040e 0104 017a 2054 6173 6b43 6f6c 6c65  .....z TaskColle
-00000ad0: 6374 5374 6174 7573 2e73 616e 6974 6973  ctStatus.sanitis
-00000ae0: 6564 5f64 6963 744e 290e 720e 0000 0072  ed_dictN).r....r
-00000af0: 0f00 0000 7210 0000 0072 1f00 0000 7203  ....r....r....r.
-00000b00: 0000 0072 2100 0000 7220 0000 0072 0200  ...r!...r ...r..
-00000b10: 0000 7206 0000 0072 2d00 0000 7204 0000  ..r....r-...r...
-00000b20: 00da 046c 6973 7472 0a00 0000 7233 0000  ...listr....r3..
-00000b30: 0072 1100 0000 7211 0000 0072 1100 0000  .r....r....r....
-00000b40: 7212 0000 0072 0c00 0000 4b00 0000 7312  r....r....K...s.
-00000b50: 0000 000a 0004 010c 0c08 0108 011a 010c  ................
-00000b60: 010c 010c 0272 0c00 0000 4e29 11da 0770  .....r....N)...p
-00000b70: 6174 686c 6962 7202 0000 00da 0674 7970  athlibr......typ
-00000b80: 696e 6772 0300 0000 7204 0000 00da 0870  ingr....r......p
-00000b90: 7964 616e 7469 6372 0500 0000 7206 0000  ydanticr....r...
-00000ba0: 0072 0700 0000 da0b 5f76 616c 6964 6174  .r......_validat
-00000bb0: 6f72 7372 0900 0000 da04 7461 736b 720a  orsr......taskr.
-00000bc0: 0000 00da 075f 5f61 6c6c 5f5f 720d 0000  .....__all__r...
-00000bd0: 0072 0b00 0000 720c 0000 0072 1100 0000  .r....r....r....
-00000be0: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00000bf0: 083c 6d6f 6475 6c65 3e01 0000 0073 1800  .<module>....s..
-00000c00: 0000 0c00 0c01 0c01 0c02 0c01 0c01 0c02  ................
-00000c10: 0c01 0402 1006 1004 1435                 .........5
+00000280: 6406 3c00 6403 5a0a 6507 650b 6504 6504  d.<.d.Z.e.e.e.e.
+00000290: 6602 1900 1900 6505 6407 3c00 650c 6404  f.....e.d.<.e.d.
+000002a0: 6408 6409 8d02 650d 6404 8301 8301 5a0e  d.d...e.d.....Z.
+000002b0: 650c 6405 6408 6409 8d02 650d 6405 8301  e.d.d.d...e.d...
+000002c0: 8301 5a0f 650c 6406 6408 6409 8d02 650d  ..Z.e.d.d.d...e.
+000002d0: 6406 8301 8301 5a10 650c 6402 8301 640a  d.....Z.e.d...d.
+000002e0: 640b 8400 8301 5a11 6403 5300 290c 720b  d.....Z.d.S.).r.
+000002f0: 0000 0061 6503 0000 0a20 2020 2054 6173  ...ae....    Tas
+00000300: 6b43 6f6c 6c65 6374 5069 7020 636c 6173  kCollectPip clas
+00000310: 730a 0a20 2020 2054 6869 7320 636c 6173  s..    This clas
+00000320: 7320 6f6e 6c79 2065 6e63 6f64 6573 2074  s only encodes t
+00000330: 6865 2061 7474 7269 6275 7465 7320 7265  he attributes re
+00000340: 7175 6972 6564 2074 6f20 7472 6967 6765  quired to trigge
+00000350: 7220 610a 2020 2020 7461 736b 2d63 6f6c  r a.    task-col
+00000360: 6c65 6374 696f 6e20 6f70 6572 6174 696f  lection operatio
+00000370: 6e2e 204f 7468 6572 2061 7474 7269 6275  n. Other attribu
+00000380: 7465 7320 2874 6861 7420 6172 6520 6173  tes (that are as
+00000390: 7369 676e 6564 202a 6475 7269 6e67 2a0a  signed *during*.
+000003a0: 2020 2020 7461 736b 2063 6f6c 6c65 6374      task collect
+000003b0: 696f 6e29 2061 7265 2064 6566 696e 6564  ion) are defined
+000003c0: 2061 7320 7061 7274 206f 6620 6672 6163   as part of frac
+000003d0: 7461 6c2d 7365 7276 6572 2e0a 0a20 2020  tal-server...   
+000003e0: 2054 776f 2063 6173 6573 2061 7265 2073   Two cases are s
+000003f0: 7570 706f 7274 6564 3a0a 0a20 2020 2020  upported:..     
+00000400: 2020 2031 2e20 6070 6163 6b61 6765 6020     1. `package` 
+00000410: 6973 2074 6865 2070 6174 6820 6f66 2061  is the path of a
+00000420: 206c 6f63 616c 2077 6865 656c 2066 696c   local wheel fil
+00000430: 653b 0a20 2020 2020 2020 2032 2e20 6070  e;.        2. `p
+00000440: 6163 6b61 6765 6020 6973 2074 6865 206e  ackage` is the n
+00000450: 616d 6520 6f66 2061 2070 6163 6b61 6765  ame of a package
+00000460: 2074 6861 7420 6361 6e20 6265 2069 6e73   that can be ins
+00000470: 7461 6c6c 6564 2076 6961 2060 7069 7060  talled via `pip`
+00000480: 2e0a 0a0a 2020 2020 4174 7472 6962 7574  ....    Attribut
+00000490: 6573 3a0a 2020 2020 2020 2020 7061 636b  es:.        pack
+000004a0: 6167 653a 0a20 2020 2020 2020 2020 2020  age:.           
+000004b0: 2054 6865 206e 616d 6520 6f66 2061 2060   The name of a `
+000004c0: 7069 7060 2d69 6e73 7461 6c6c 6162 6c65  pip`-installable
+000004d0: 2070 6163 6b61 6765 2c20 6f72 2074 6865   package, or the
+000004e0: 2070 6174 6820 746f 2061 206c 6f63 616c   path to a local
+000004f0: 0a20 2020 2020 2020 2020 2020 2077 6865  .            whe
+00000500: 656c 2066 696c 652e 0a20 2020 2020 2020  el file..       
+00000510: 2070 6163 6b61 6765 5f76 6572 7369 6f6e   package_version
+00000520: 3a20 5665 7273 696f 6e20 6f66 2074 6865  : Version of the
+00000530: 2070 6163 6b61 6765 0a20 2020 2020 2020   package.       
+00000540: 2070 6163 6b61 6765 5f65 7874 7261 733a   package_extras:
+00000550: 2050 6163 6b61 6765 2065 7874 7261 7320   Package extras 
+00000560: 746f 2069 6e63 6c75 6465 2069 6e20 7468  to include in th
+00000570: 6520 6070 6970 2069 6e73 7461 6c6c 6020  e `pip install` 
+00000580: 636f 6d6d 616e 640a 2020 2020 2020 2020  command.        
+00000590: 7079 7468 6f6e 5f76 6572 7369 6f6e 3a20  python_version: 
+000005a0: 5079 7468 6f6e 2076 6572 7369 6f6e 2074  Python version t
+000005b0: 6f20 696e 7374 616c 6c20 616e 6420 7275  o install and ru
+000005c0: 6e20 7468 6520 7061 636b 6167 6520 7461  n the package ta
+000005d0: 736b 730a 2020 2020 2020 2020 7069 6e6e  sks.        pinn
+000005e0: 6564 5f70 6163 6b61 6765 5f76 6572 7369  ed_package_versi
+000005f0: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
+00000600: 2064 6963 7469 6f6e 6172 7920 2770 6163   dictionary 'pac
+00000610: 6b61 6765 273a 2776 6572 7369 6f6e 2720  kage':'version' 
+00000620: 7573 6564 2074 6f20 7069 6e20 7665 7273  used to pin vers
+00000630: 696f 6e73 2066 6f72 2073 7065 6369 6669  ions for specifi
+00000640: 630a 2020 2020 2020 2020 2020 2020 7061  c.            pa
+00000650: 636b 6167 6573 2e0a 0a20 2020 20da 0770  ckages...    ..p
+00000660: 6163 6b61 6765 4eda 0f70 6163 6b61 6765  ackageN..package
+00000670: 5f76 6572 7369 6f6e da0e 7061 636b 6167  _version..packag
+00000680: 655f 6578 7472 6173 da0e 7079 7468 6f6e  e_extras..python
+00000690: 5f76 6572 7369 6f6e da17 7069 6e6e 6564  _version..pinned
+000006a0: 5f70 6163 6b61 6765 5f76 6572 7369 6f6e  _package_version
+000006b0: 7354 2901 da0b 616c 6c6f 775f 7265 7573  sT)...allow_reus
+000006c0: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
+000006d0: 0000 0400 0000 4300 0000 7342 0000 0064  ......C...sB...d
+000006e0: 017c 0176 0072 1f7c 01a0 0064 02a1 0173  .|.v.r.|...d...s
+000006f0: 1174 0164 037c 019b 0064 049d 0383 0182  .t.d.|...d......
+00000700: 0174 027c 0183 01a0 03a1 0073 1f74 0164  .t.|.......s.t.d
+00000710: 057c 019b 0064 049d 0383 0182 017c 0153  .|...d.......|.S
+00000720: 0029 064e fa01 2f7a 042e 7768 6c7a 2f4c  .).N../z..whlz/L
+00000730: 6f63 616c 2d70 6163 6b61 6765 2070 6174  ocal-package pat
+00000740: 6820 6d75 7374 2062 6520 6120 7768 6565  h must be a whee
+00000750: 6c20 6669 6c65 2028 6769 7665 6e20 7a02  l file (given z.
+00000760: 292e 7a2c 4c6f 6361 6c2d 7061 636b 6167  ).z,Local-packag
+00000770: 6520 7061 7468 206d 7573 7420 6265 2061  e path must be a
+00000780: 6273 6f6c 7574 653a 2028 6769 7665 6e20  bsolute: (given 
+00000790: 2904 da08 656e 6473 7769 7468 da0a 5661  )...endswith..Va
+000007a0: 6c75 6545 7272 6f72 7202 0000 00da 0b69  lueErrorr......i
+000007b0: 735f 6162 736f 6c75 7465 2902 da03 636c  s_absolute)...cl
+000007c0: 73da 0576 616c 7565 7211 0000 0072 1100  s..valuer....r..
+000007d0: 0000 7212 0000 00da 1170 6163 6b61 6765  ..r......package
+000007e0: 5f76 616c 6964 6174 6f72 4100 0000 7318  _validatorA...s.
+000007f0: 0000 0008 020a 0102 0102 0102 0106 ff04  ................
+00000800: ff0c 0402 010a 0104 ff04 037a 2054 6173  ...........z Tas
+00000810: 6b43 6f6c 6c65 6374 5069 702e 7061 636b  kCollectPip.pack
+00000820: 6167 655f 7661 6c69 6461 746f 7229 1272  age_validator).r
+00000830: 0e00 0000 720f 0000 0072 1000 0000 da07  ....r....r......
+00000840: 5f5f 646f 635f 5fda 0373 7472 da0f 5f5f  __doc__..str..__
+00000850: 616e 6e6f 7461 7469 6f6e 735f 5f72 1400  annotations__r..
+00000860: 0000 7204 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00000870: 0072 1700 0000 da04 6469 6374 7207 0000  .r......dictr...
+00000880: 0072 0900 0000 da10 5f70 6163 6b61 6765  .r......_package
+00000890: 5f76 6572 7369 6f6e da0f 5f70 6163 6b61  _version.._packa
+000008a0: 6765 5f65 7874 7261 73da 0f5f 7079 7468  ge_extras.._pyth
+000008b0: 6f6e 5f76 6572 7369 6f6e 721f 0000 0072  on_versionr....r
+000008c0: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
+000008d0: 0000 0072 0b00 0000 1600 0000 7324 0000  ...r........s$..
+000008e0: 000a 0004 0108 1a10 0110 0110 0118 010a  ................
+000008f0: 0206 0104 ff0a 0306 0104 ff0a 0306 0104  ................
+00000900: ff06 040e 0172 0b00 0000 6300 0000 0000  .....r....c.....
+00000910: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00000920: 0000 0073 6800 0000 6500 5a01 6400 5a02  ...sh...e.Z.d.Z.
+00000930: 5500 6401 5a03 6504 6402 1900 6505 6403  U.d.Z.e.d...e.d.
+00000940: 3c00 6506 6505 6404 3c00 6507 6505 6405  <.e.e.d.<.e.e.d.
+00000950: 3c00 6508 6700 6406 8d01 5a09 650a 650b  <.e.g.d...Z.e.e.
+00000960: 650c 1900 1900 6505 6407 3c00 650a 6506  e.....e.d.<.e.e.
+00000970: 1900 6505 6408 3c00 650a 6506 1900 6505  ..e.d.<.e.e...e.
+00000980: 6409 3c00 640a 640b 8400 5a0d 640c 5300  d.<.d.d...Z.d.S.
+00000990: 290d 720c 0000 007a ac0a 2020 2020 5461  ).r....z..    Ta
+000009a0: 736b 436f 6c6c 6563 7453 7461 7475 7320  skCollectStatus 
+000009b0: 636c 6173 730a 0a20 2020 2041 7474 7269  class..    Attri
+000009c0: 6275 7465 733a 0a20 2020 2020 2020 2073  butes:.        s
+000009d0: 7461 7475 733a 2054 4244 0a20 2020 2020  tatus: TBD.     
+000009e0: 2020 2070 6163 6b61 6765 3a20 5442 440a     package: TBD.
+000009f0: 2020 2020 2020 2020 7665 6e76 5f70 6174          venv_pat
+00000a00: 683a 2054 4244 0a20 2020 2020 2020 2074  h: TBD.        t
+00000a10: 6173 6b5f 6c69 7374 3a20 5442 440a 2020  ask_list: TBD.  
+00000a20: 2020 2020 2020 6c6f 673a 2054 4244 0a20        log: TBD. 
+00000a30: 2020 2020 2020 2069 6e66 6f3a 2054 4244         info: TBD
+00000a40: 0a20 2020 2029 05da 0770 656e 6469 6e67  .    )...pending
+00000a50: da0a 696e 7374 616c 6c69 6e67 da0a 636f  ..installing..co
+00000a60: 6c6c 6563 7469 6e67 da04 6661 696c da02  llecting..fail..
+00000a70: 4f4b da06 7374 6174 7573 7213 0000 00da  OK..statusr.....
+00000a80: 0976 656e 765f 7061 7468 2901 da07 6465  .venv_path)...de
+00000a90: 6661 756c 74da 0974 6173 6b5f 6c69 7374  fault..task_list
+00000aa0: da03 6c6f 67da 0469 6e66 6f63 0100 0000  ..log..infoc....
+00000ab0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000ac0: 4300 0000 731a 0000 007c 00a0 00a1 007d  C...s....|.....}
+00000ad0: 0174 017c 006a 0283 017c 0164 013c 007c  .t.|.j...|.d.<.|
+00000ae0: 0153 0029 027a 510a 2020 2020 2020 2020  .S.).zQ.        
+00000af0: 5265 7475 726e 2060 7365 6c66 2e64 6963  Return `self.dic
+00000b00: 7428 2960 2061 6674 6572 2063 6173 7469  t()` after casti
+00000b10: 6e67 2060 7365 6c66 2e76 656e 765f 7061  ng `self.venv_pa
+00000b20: 7468 6020 746f 2061 2073 7472 696e 670a  th` to a string.
+00000b30: 2020 2020 2020 2020 722d 0000 0029 0372          r-...).r
+00000b40: 2300 0000 7221 0000 0072 2d00 0000 2902  #...r!...r-...).
+00000b50: da04 7365 6c66 da01 6472 1100 0000 7211  ..self..dr....r.
+00000b60: 0000 0072 1200 0000 da0e 7361 6e69 7469  ...r......saniti
+00000b70: 7365 645f 6469 6374 6400 0000 7306 0000  sed_dictd...s...
+00000b80: 0008 040e 0104 017a 2054 6173 6b43 6f6c  .......z TaskCol
+00000b90: 6c65 6374 5374 6174 7573 2e73 616e 6974  lectStatus.sanit
+00000ba0: 6973 6564 5f64 6963 744e 290e 720e 0000  ised_dictN).r...
+00000bb0: 0072 0f00 0000 7210 0000 0072 2000 0000  .r....r....r ...
+00000bc0: 7203 0000 0072 2200 0000 7221 0000 0072  r....r"...r!...r
+00000bd0: 0200 0000 7206 0000 0072 2f00 0000 7204  ....r....r/...r.
+00000be0: 0000 00da 046c 6973 7472 0a00 0000 7234  .....listr....r4
+00000bf0: 0000 0072 1100 0000 7211 0000 0072 1100  ...r....r....r..
+00000c00: 0000 7212 0000 0072 0c00 0000 5000 0000  ..r....r....P...
+00000c10: 7312 0000 000a 0004 010c 0c08 0108 011a  s...............
+00000c20: 010c 010c 010c 0272 0c00 0000 4e29 11da  .......r....N)..
+00000c30: 0770 6174 686c 6962 7202 0000 00da 0674  .pathlibr......t
+00000c40: 7970 696e 6772 0300 0000 7204 0000 00da  ypingr....r.....
+00000c50: 0870 7964 616e 7469 6372 0500 0000 7206  .pydanticr....r.
+00000c60: 0000 0072 0700 0000 da0b 5f76 616c 6964  ...r......_valid
+00000c70: 6174 6f72 7372 0900 0000 da04 7461 736b  atorsr......task
+00000c80: 720a 0000 00da 075f 5f61 6c6c 5f5f 720d  r......__all__r.
+00000c90: 0000 0072 0b00 0000 720c 0000 0072 1100  ...r....r....r..
+00000ca0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00000cb0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000cc0: 1800 0000 0c00 0c01 0c01 0c02 0c01 0c01  ................
+00000cd0: 0c02 0c01 0402 1006 1004 143a            ...........:
```

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/user.cpython-39.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/user.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/_validators.py` & `fractal_client-1.3.0a2/fractal/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/applyworkflow.py` & `fractal_client-1.3.0a2/fractal/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/manifest.py` & `fractal_client-1.3.0a2/fractal/common/schemas/manifest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from pathlib import Path
 from typing import Any
 from typing import Optional
 from typing import TypeVar
 
 from pydantic import BaseModel
 from pydantic import Field
+from pydantic import root_validator
 from pydantic import validator
 
 
 __all__ = ("TaskManifestV1", "ManifestV1")
 
 
 class _TaskManifestBase(BaseModel):
     """
-    Base class for TaskManifest
+    Base class for `TaskManifest`
 
     Represents a task within a manfest
 
     Attributes:
         name:
             The task name
         executable:
@@ -27,29 +27,28 @@
             package `Pkg` installs in the folder `pkg` the executable
             `pkg/executable.py`, this attribute must contain only
             `executable.py`.
         input_type:
             The input type accepted by the task
         output_type:
             The output type returned by the task
-        default_args:
-            An arbitrary, JSON-serializable dictionary containing the default
-            parameters that will be passed to the task
         meta:
             Additional information about the package, such as hash of the
             executable, specific runtime requirements (e.g., need_gpu=True),
             etc.
+        args_schema:
+            JSON Schema for task arguments
     """
 
     name: str
-    executable: Path
+    executable: str
     input_type: str
     output_type: str
-    default_args: Optional[dict[str, Any]] = Field(default_factory=dict)
     meta: Optional[dict[str, Any]] = Field(default_factory=dict)
+    args_schema: Optional[dict[str, Any]]
 
 
 TaskManifestType = TypeVar("TaskManifestType", bound=_TaskManifestBase)
 
 
 class _ManifestBase(BaseModel):
     """
@@ -66,18 +65,38 @@
             A version string that provides indication for compatibility between
             manifests as the schema evolves. This is for instance used by
             Fractal to determine which subclass of the present base class needs
             be used to read and validate the input.
         task_list : list[TaskManifestType]
             The list of tasks, represented as specified by subclasses of the
             _TaskManifestBase (a.k.a. TaskManifestType)
+        has_args_schemas:
+            `True` if the manifest incldues JSON Schemas for the arguments of
+            each task.
+        args_schema_version:
+            Label of how `args_schema`s were generated (e.g. `pydantic_v1`).
     """
 
     manifest_version: str
-    task_list: list[TaskManifestType]  # type: ignore
+    task_list: list[TaskManifestType]
+    has_args_schemas: bool = False
+    args_schema_version: Optional[str]
+
+    @root_validator()
+    def _check_args_schemas_are_present(cls, values):
+        has_args_schemas = values["has_args_schemas"]
+        task_list = values["task_list"]
+        if has_args_schemas:
+            for task in task_list:
+                if task.args_schema is None:
+                    raise ValueError(
+                        f'has_args_schemas={has_args_schemas} but task "'
+                        f'{task.name}" has args_schema={task.args_schema}.'
+                    )
+        return values
 
 
 class TaskManifestV1(_TaskManifestBase):
     pass
 
 
 class ManifestV1(_ManifestBase):
@@ -86,8 +105,8 @@
     """
 
     task_list: list[TaskManifestV1]
 
     @validator("manifest_version")
     def manifest_version_1(cls, value):
         if value != "1":
-            raise ValueError("Wrong manifest version")
+            raise ValueError(f"Wrong manifest version (given {value})")
```

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/project.py` & `fractal_client-1.3.0a2/fractal/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/state.py` & `fractal_client-1.3.0a2/fractal/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/task_collection.py` & `fractal_client-1.3.0a2/fractal/common/schemas/task_collection.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,20 +36,25 @@
     Attributes:
         package:
             The name of a `pip`-installable package, or the path to a local
             wheel file.
         package_version: Version of the package
         package_extras: Package extras to include in the `pip install` command
         python_version: Python version to install and run the package tasks
+        pinned_package_versions:
+            dictionary 'package':'version' used to pin versions for specific
+            packages.
+
     """
 
     package: str
     package_version: Optional[str] = None
     package_extras: Optional[str] = None
     python_version: Optional[str] = None
+    pinned_package_versions: Optional[dict[str, str]] = None
 
     _package_version = validator("package_version", allow_reuse=True)(
         valstr("package_version")
     )
     _package_extras = validator("package_extras", allow_reuse=True)(
         valstr("package_extras")
     )
```

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/user.py` & `fractal_client-1.3.0a2/fractal/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/schemas/workflow.py` & `fractal_client-1.3.0a2/fractal/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 25 12:31:57 2023 UTC, .py size: 773 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-00000000: 6f0d 0d0a 0000 0000 3d55 6f64 0503 0000  o.......=Uod....
+00000000: 6f0d 0d0a 0000 0000 faf1 8664 c803 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6405 6406 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
 00000080: 2907 e900 0000 004e 2901 da05 6465 6275  )......N)...debu
 00000090: 6729 01da 0f56 616c 6964 6174 696f 6e45  g)...ValidationE
 000000a0: 7272 6f72 2901 da0e 5461 736b 436f 6c6c  rror)...TaskColl
 000000b0: 6563 7450 6970 6300 0000 0000 0000 0000  ectPipc.........
 000000c0: 0000 0002 0000 0008 0000 0043 0000 0073  ...........C...s
-000000d0: 7a01 0000 7400 6401 6402 8d01 7d00 7401  z...t.d.d...}.t.
+000000d0: bc01 0000 7400 6401 6402 8d01 7d00 7401  ....t.d.d...}.t.
 000000e0: 7c00 8301 0100 7c00 7328 6403 6404 6405  |.....|.s(d.d.d.
 000000f0: 7402 a003 a100 7600 7318 7404 a005 7c00  t.....v.s.t...|.
 00000100: a101 721d 7404 a006 7c00 a101 6e01 6405  ..r.t...|...n.d.
 00000110: 6901 1600 7d01 7407 7404 a008 7c01 a101  i...}.t.t...|...
 00000120: 8301 8201 7400 6406 6402 8d01 7d00 7401  ....t.d.d...}.t.
 00000130: 7c00 8301 0100 7c00 7350 6403 6404 6405  |.....|.sPd.d.d.
 00000140: 7402 a003 a100 7600 7340 7404 a005 7c00  t.....v.s@t...|.
@@ -27,51 +27,58 @@
 000001a0: 0100 0100 5900 0100 7409 a00a 740b a101  ....Y...t...t...
 000001b0: 8f0d 0100 7400 6408 6402 8d01 7d00 5700  ....t.d.d...}.W.
 000001c0: 6400 0400 0400 8303 0100 6e08 3100 737f  d.........n.1.s.
 000001d0: 7701 0100 0100 0100 5900 0100 7409 a00a  w.......Y...t...
 000001e0: 740b a101 8f0e 0100 7400 6401 6409 640a  t.......t.d.d.d.
 000001f0: 8d02 7d00 5700 6400 0400 0400 8303 0100  ..}.W.d.........
 00000200: 6e08 3100 739a 7701 0100 0100 0100 5900  n.1.s.w.......Y.
-00000210: 0100 7409 a00a 740b a101 8f0f 0100 7400  ..t...t.......t.
+00000210: 0100 7409 a00a 740b a101 8f0e 0100 7400  ..t...t.......t.
 00000220: 6401 6400 640a 8d02 7d00 5700 6400 0400  d.d.d...}.W.d...
-00000230: 0400 8303 0100 6400 5300 3100 73b6 7701  ......d.S.1.s.w.
-00000240: 0100 0100 0100 5900 0100 6400 5300 290b  ......Y...d.S.).
-00000250: 4e7a 0c73 6f6d 652d 7061 636b 6167 6529  Nz.some-package)
-00000260: 01da 0770 6163 6b61 6765 7a0e 6173 7365  ...packagez.asse
-00000270: 7274 2025 2870 7930 2973 da03 7079 30da  rt %(py0)s..py0.
-00000280: 0163 7a11 2f73 6f6d 652f 7061 636b 6167  .cz./some/packag
-00000290: 652e 7768 6c7a 0c73 6f6d 652f 7061 636b  e.whlz.some/pack
-000002a0: 6167 657a 142f 736f 6d65 2f70 6163 6b61  agez./some/packa
-000002b0: 6765 2e74 6172 2e67 7ada 0029 0272 0500  ge.tar.gz..).r..
-000002c0: 0000 da0e 7061 636b 6167 655f 6578 7472  ....package_extr
-000002d0: 6173 290c 7204 0000 0072 0200 0000 da0c  as).r....r......
-000002e0: 4070 795f 6275 696c 7469 6e73 da06 6c6f  @py_builtins..lo
-000002f0: 6361 6c73 da0a 4070 7974 6573 745f 6172  cals..@pytest_ar
-00000300: da18 5f73 686f 756c 645f 7265 7072 5f67  .._should_repr_g
-00000310: 6c6f 6261 6c5f 6e61 6d65 da09 5f73 6166  lobal_name.._saf
-00000320: 6572 6570 72da 0e41 7373 6572 7469 6f6e  erepr..Assertion
-00000330: 4572 726f 72da 135f 666f 726d 6174 5f65  Error.._format_e
-00000340: 7870 6c61 6e61 7469 6f6e da06 7079 7465  xplanation..pyte
-00000350: 7374 da06 7261 6973 6573 7203 0000 0029  st..raisesr....)
-00000360: 0272 0700 0000 da0b 4070 795f 666f 726d  .r......@py_form
-00000370: 6174 31a9 0072 1400 0000 fa4a 2f68 6f6d  at1..r.....J/hom
-00000380: 652f 746f 6d6d 6173 6f2f 4672 6163 7461  e/tommaso/Fracta
-00000390: 6c2f 6672 6163 7461 6c2f 6672 6163 7461  l/fractal/fracta
-000003a0: 6c2f 636f 6d6d 6f6e 2f74 6573 7473 2f74  l/common/tests/t
-000003b0: 6573 745f 7461 736b 5f63 6f6c 6c65 6374  est_task_collect
-000003c0: 696f 6e2e 7079 da13 7465 7374 5f54 6173  ion.py..test_Tas
-000003d0: 6b43 6f6c 6c65 6374 5069 7008 0000 0073  kCollectPip....s
-000003e0: 2400 0000 0a02 0801 3e01 0a01 0801 3e01  $.......>.....>.
-000003f0: 0c02 0c01 1cff 0c02 0c01 1cff 0c02 0e01  ................
-00000400: 1cff 0c02 0e01 22ff 7216 0000 0029 0eda  ......".r....)..
-00000410: 0862 7569 6c74 696e 7372 0a00 0000 da19  .builtinsr......
-00000420: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
-00000430: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
-00000440: 7469 6f6e da07 7265 7772 6974 6572 0c00  tion..rewriter..
-00000450: 0000 7211 0000 00da 0864 6576 746f 6f6c  ..r......devtool
-00000460: 7372 0200 0000 da17 7079 6461 6e74 6963  sr......pydantic
-00000470: 2e65 7272 6f72 5f77 7261 7070 6572 7372  .error_wrappersr
-00000480: 0300 0000 da07 7363 6865 6d61 7372 0400  ......schemasr..
-00000490: 0000 7216 0000 0072 1400 0000 7214 0000  ..r....r....r...
-000004a0: 0072 1400 0000 7215 0000 00da 083c 6d6f  .r....r......<mo
-000004b0: 6475 6c65 3e01 0000 0073 0a00 0000 2200  dule>....s....".
-000004c0: 0c01 0c01 0c02 0c03                      ........
+00000230: 0400 8303 0100 6e08 3100 73b5 7701 0100  ......n.1.s.w...
+00000240: 0100 0100 5900 0100 7400 6401 6900 640b  ....Y...t.d.i.d.
+00000250: 8d02 7d00 7409 a00a 740b a101 8f0f 0100  ..}.t...t.......
+00000260: 7400 6401 640c 640b 8d02 7d00 5700 6400  t.d.d.d...}.W.d.
+00000270: 0400 0400 8303 0100 6400 5300 3100 73d7  ........d.S.1.s.
+00000280: 7701 0100 0100 0100 5900 0100 6400 5300  w.......Y...d.S.
+00000290: 290d 4e7a 0c73 6f6d 652d 7061 636b 6167  ).Nz.some-packag
+000002a0: 6529 01da 0770 6163 6b61 6765 7a0e 6173  e)...packagez.as
+000002b0: 7365 7274 2025 2870 7930 2973 da03 7079  sert %(py0)s..py
+000002c0: 30da 0163 7a11 2f73 6f6d 652f 7061 636b  0..cz./some/pack
+000002d0: 6167 652e 7768 6c7a 0c73 6f6d 652f 7061  age.whlz.some/pa
+000002e0: 636b 6167 657a 142f 736f 6d65 2f70 6163  ckagez./some/pac
+000002f0: 6b61 6765 2e74 6172 2e67 7ada 0029 0272  kage.tar.gz..).r
+00000300: 0500 0000 da0e 7061 636b 6167 655f 6578  ......package_ex
+00000310: 7472 6173 2902 7205 0000 00da 1770 696e  tras).r......pin
+00000320: 6e65 645f 7061 636b 6167 655f 7665 7273  ned_package_vers
+00000330: 696f 6e73 e901 0000 0029 0c72 0400 0000  ions.....).r....
+00000340: 7202 0000 00da 0c40 7079 5f62 7569 6c74  r......@py_built
+00000350: 696e 73da 066c 6f63 616c 73da 0a40 7079  ins..locals..@py
+00000360: 7465 7374 5f61 72da 185f 7368 6f75 6c64  test_ar.._should
+00000370: 5f72 6570 725f 676c 6f62 616c 5f6e 616d  _repr_global_nam
+00000380: 65da 095f 7361 6665 7265 7072 da0e 4173  e.._saferepr..As
+00000390: 7365 7274 696f 6e45 7272 6f72 da13 5f66  sertionError.._f
+000003a0: 6f72 6d61 745f 6578 706c 616e 6174 696f  ormat_explanatio
+000003b0: 6eda 0670 7974 6573 74da 0672 6169 7365  n..pytest..raise
+000003c0: 7372 0300 0000 2902 7207 0000 00da 0b40  sr....).r......@
+000003d0: 7079 5f66 6f72 6d61 7431 a900 7216 0000  py_format1..r...
+000003e0: 00fa 4a2f 686f 6d65 2f74 6f6d 6d61 736f  ..J/home/tommaso
+000003f0: 2f46 7261 6374 616c 2f66 7261 6374 616c  /Fractal/fractal
+00000400: 2f66 7261 6374 616c 2f63 6f6d 6d6f 6e2f  /fractal/common/
+00000410: 7465 7374 732f 7465 7374 5f74 6173 6b5f  tests/test_task_
+00000420: 636f 6c6c 6563 7469 6f6e 2e70 79da 1374  collection.py..t
+00000430: 6573 745f 5461 736b 436f 6c6c 6563 7450  est_TaskCollectP
+00000440: 6970 0800 0000 732c 0000 000a 0208 013e  ip....s,.......>
+00000450: 010a 0108 013e 010c 020c 011c ff0c 020c  .....>..........
+00000460: 011c ff0c 020e 011c ff0c 020e 011c ff0c  ................
+00000470: 030c 010e 0122 ff72 1800 0000 290e da08  .....".r....)...
+00000480: 6275 696c 7469 6e73 720c 0000 00da 195f  builtinsr......_
+00000490: 7079 7465 7374 2e61 7373 6572 7469 6f6e  pytest.assertion
+000004a0: 2e72 6577 7269 7465 da09 6173 7365 7274  .rewrite..assert
+000004b0: 696f 6eda 0772 6577 7269 7465 720e 0000  ion..rewriter...
+000004c0: 0072 1300 0000 da08 6465 7674 6f6f 6c73  .r......devtools
+000004d0: 7202 0000 00da 1770 7964 616e 7469 632e  r......pydantic.
+000004e0: 6572 726f 725f 7772 6170 7065 7273 7203  error_wrappersr.
+000004f0: 0000 00da 0773 6368 656d 6173 7204 0000  .....schemasr...
+00000500: 0072 1800 0000 7216 0000 0072 1600 0000  .r....r....r....
+00000510: 7216 0000 0072 1700 0000 da08 3c6d 6f64  r....r......<mod
+00000520: 756c 653e 0100 0000 730a 0000 0022 000c  ule>....s...."..
+00000530: 010c 010c 020c 03                        .......
```

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/test_dataset.py` & `fractal_client-1.3.0a2/fractal/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/test_project.py` & `fractal_client-1.3.0a2/fractal/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/test_state.py` & `fractal_client-1.3.0a2/fractal/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/test_task.py` & `fractal_client-1.3.0a2/fractal/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/test_task_collection.py` & `fractal_client-1.3.0a2/fractal/common/tests/test_task_collection.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,7 +18,11 @@
         c = TaskCollectPip(package="some/package")
     with pytest.raises(ValidationError):
         c = TaskCollectPip(package="/some/package.tar.gz")
     with pytest.raises(ValidationError):
         c = TaskCollectPip(package="some-package", package_extras="")
     with pytest.raises(ValidationError):
         c = TaskCollectPip(package="some-package", package_extras=None)
+
+    c = TaskCollectPip(package="some-package", pinned_package_versions={})
+    with pytest.raises(ValidationError):
+        c = TaskCollectPip(package="some-package", pinned_package_versions=1)
```

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/test_user.py` & `fractal_client-1.3.0a2/fractal/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/common/tests/test_workflow.py` & `fractal_client-1.3.0a2/fractal/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/config.py` & `fractal_client-1.3.0a2/fractal/config.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/interface.py` & `fractal_client-1.3.0a2/fractal/interface.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/fractal/parser.py` & `fractal_client-1.3.0a2/fractal/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,14 +291,19 @@
     help=(
         "Comma separated list of extra components for the package to be "
         "installed, e.g., `collect fractal-tasks-core "
         "--package-extras=torch,tensorflow` will trigger the installation of "
         "`fractal-tasks-core[torch,tensorflow]`"
     ),
 )
+task_collect_parser.add_argument(
+    "--pinned-dependency",
+    action="append",
+    help="List of 'package_name:package_version' to be pinned",  # FIXME
+)
 
 # task check-collection
 task_check_collection_parser = task_subparsers.add_parser(
     "check-collection",
     description="Check status of background task collection processes",
     allow_abbrev=False,
 )
@@ -352,19 +357,14 @@
 )
 task_new_parser.add_argument(
     "--version",
     type=str,
     help="Task version",
 )
 task_new_parser.add_argument(
-    "--default-args-file",
-    help="Path to JSON file with default task arguments",
-    type=str,
-)
-task_new_parser.add_argument(
     "--meta-file",
     help="Path to JSON file with additional parameters useful for execution",
     type=str,
 )
 
 # task edit
 task_edit_parser = task_subparsers.add_parser(
@@ -403,22 +403,14 @@
 )
 task_edit_parser.add_argument(
     "--new-output-type",
     type=str,
     help="New output type",
 )
 task_edit_parser.add_argument(
-    "--default-args-file",
-    type=str,
-    help=(
-        "Path to JSON serialised file containing updates to the current"
-        "`default_args` dictionary"
-    ),
-)
-task_edit_parser.add_argument(
     "--meta-file",
     type=str,
     help=(
         "Path to JSON serialised file containing updates to the current "
         "`meta` dictionary"
     ),
 )
```

### Comparing `fractal_client-1.3.0a1/fractal/response.py` & `fractal_client-1.3.0a2/fractal/response.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a1/pyproject.toml` & `fractal_client-1.3.0a2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-client"
-version = "1.3.0a1"
+version = "1.3.0a2"
 description = "Client component of the Fractal analytics platform"
 authors = [
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
 readme = "README.md"
@@ -43,15 +43,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.bumpver]
-current_version = "1.3.0a1"
+current_version = "1.3.0a2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
@@ -70,8 +70,8 @@
 fractal_old = "fractal.old:run"
 fractal_new = "fractal.new:run"
 
 [tool.coverage.run]
 branch = true
 parallel = true
 relative_files = true
-omit = ["tests/*"]
+omit = ["tests/*", "fractal/common/tests/*"]
```

### Comparing `fractal_client-1.3.0a1/PKG-INFO` & `fractal_client-1.3.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-client
-Version: 1.3.0a1
+Version: 1.3.0a2
 Summary: Client component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal
 License: BSD-3-Clause
 Author: Tommaso Comparin
 Author-email: tommaso.comparin@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -40,9 +40,9 @@
 
 See https://fractal-analytics-platform.github.io/fractal.
 
 # Contributors and license
 
 Unless otherwise stated in each individual module, all Fractal components are released according to a BSD 3-Clause License, and Copyright is with Friedrich Miescher Institute for Biomedical Research and University of Zurich.
 
-Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa) & [@jacopo-exact](https://github.com/jacopo-exact) from [eXact lab S.r.l.](exact-lab.it).
+Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [eXact lab S.r.l.](exact-lab.it).
```

