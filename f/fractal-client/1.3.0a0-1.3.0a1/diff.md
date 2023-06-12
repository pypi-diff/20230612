# Comparing `tmp/fractal_client-1.3.0a0.tar.gz` & `tmp/fractal_client-1.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_client-1.3.0a0.tar", max compression
+gzip compressed data, was "fractal_client-1.3.0a1.tar", max compression
```

## Comparing `fractal_client-1.3.0a0.tar` & `fractal_client-1.3.0a1.tar`

### file list

```diff
@@ -1,93 +1,96 @@
--rw-r--r--   0        0        0     1576 2023-05-09 19:58:57.312677 fractal_client-1.3.0a0/LICENSE
--rw-r--r--   0        0        0     2619 2023-05-09 19:58:57.312677 fractal_client-1.3.0a0/README.md
--rw-r--r--   0        0        0       24 2023-05-15 12:57:11.406870 fractal_client-1.3.0a0/fractal/__init__.py
--rw-r--r--   0        0        0      124 2023-05-09 19:58:57.316677 fractal_client-1.3.0a0/fractal/__main__.py
--rw-r--r--   0        0        0     3448 2023-05-12 13:35:21.647646 fractal_client-1.3.0a0/fractal/authclient.py
--rw-r--r--   0        0        0     3607 2023-05-09 19:58:57.316677 fractal_client-1.3.0a0/fractal/client.py
--rw-r--r--   0        0        0     7424 2023-05-15 12:45:04.215004 fractal_client-1.3.0a0/fractal/cmd/__init__.py
--rw-r--r--   0        0        0     5846 2023-05-12 13:17:45.698886 fractal_client-1.3.0a0/fractal/cmd/_dataset.py
--rw-r--r--   0        0        0     5169 2023-05-15 12:45:04.215004 fractal_client-1.3.0a0/fractal/cmd/_job.py
--rw-r--r--   0        0        0     4116 2023-05-12 13:17:45.698886 fractal_client-1.3.0a0/fractal/cmd/_project.py
--rw-r--r--   0        0        0     5393 2023-05-12 13:17:45.698886 fractal_client-1.3.0a0/fractal/cmd/_task.py
--rw-r--r--   0        0        0     4463 2023-05-09 19:58:57.316677 fractal_client-1.3.0a0/fractal/cmd/_user.py
--rw-r--r--   0        0        0     8885 2023-05-12 13:18:41.370093 fractal_client-1.3.0a0/fractal/cmd/_workflow.py
--rw-r--r--   0        0        0     2413 2023-05-09 19:58:57.316677 fractal_client-1.3.0a0/fractal/cmd/utils.py
--rw-r--r--   0        0        0       42 2023-02-21 08:49:25.750218 fractal_client-1.3.0a0/fractal/common/.git
--rw-r--r--   0        0        0      717 2023-03-06 13:52:20.997699 fractal_client-1.3.0a0/fractal/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-21 08:49:27.594201 fractal_client-1.3.0a0/fractal/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-03-06 13:52:21.001699 fractal_client-1.3.0a0/fractal/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-21 08:49:27.594201 fractal_client-1.3.0a0/fractal/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-03-06 13:52:21.001699 fractal_client-1.3.0a0/fractal/common/README.md
--rw-r--r--   0        0        0        0 2023-02-21 08:49:27.594201 fractal_client-1.3.0a0/fractal/common/__init__.py
--rw-r--r--   0        0        0      149 2023-02-21 10:13:04.505672 fractal_client-1.3.0a0/fractal/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      147 2023-03-16 09:04:47.705157 fractal_client-1.3.0a0/fractal/common/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       48 2023-03-06 13:52:21.001699 fractal_client-1.3.0a0/fractal/common/requirements.txt
--rw-r--r--   0        0        0      525 2023-02-21 08:49:27.594201 fractal_client-1.3.0a0/fractal/common/schemas/__init__.py
--rw-r--r--   0        0        0      374 2023-02-21 10:13:04.505672 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      372 2023-03-16 09:04:47.705157 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      490 2023-03-03 14:13:42.839064 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1753 2023-04-20 07:56:22.895496 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1251 2023-03-16 09:04:47.793156 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc
--rw-r--r--   0        0        0     1589 2023-05-11 16:08:00.511429 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2027 2023-03-16 09:04:47.705157 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc
--rw-r--r--   0        0        0     3527 2023-02-21 10:13:04.645671 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     3515 2023-03-16 09:04:47.797156 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc
--rw-r--r--   0        0        0     3598 2023-04-20 07:56:22.903496 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     3711 2023-03-16 09:04:47.797156 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/project.cpython-39.pyc
--rw-r--r--   0        0        0     1191 2023-03-06 14:07:54.286234 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1185 2023-03-16 09:04:47.801156 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/state.cpython-39.pyc
--rw-r--r--   0        0        0     4929 2023-05-09 20:00:39.843482 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     4994 2023-03-16 09:04:47.805156 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/task.cpython-39.pyc
--rw-r--r--   0        0        0     1121 2023-05-11 16:08:00.523429 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1024 2023-03-16 09:04:47.809156 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/user.cpython-39.pyc
--rw-r--r--   0        0        0     3943 2023-05-11 16:08:00.527429 fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     1616 2023-04-06 11:30:39.096144 fractal_client-1.3.0a0/fractal/common/schemas/_validators.py
--rw-r--r--   0        0        0     1044 2023-05-11 16:07:56.531485 fractal_client-1.3.0a0/fractal/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     2817 2023-02-21 08:49:27.594201 fractal_client-1.3.0a0/fractal/common/schemas/manifest.py
--rw-r--r--   0        0        0     2527 2023-04-06 11:30:39.096144 fractal_client-1.3.0a0/fractal/common/schemas/project.py
--rw-r--r--   0        0        0      695 2023-03-06 14:07:44.150418 fractal_client-1.3.0a0/fractal/common/schemas/state.py
--rw-r--r--   0        0        0     4323 2023-05-09 20:00:26.031645 fractal_client-1.3.0a0/fractal/common/schemas/task.py
--rw-r--r--   0        0        0      980 2023-05-11 16:07:56.531485 fractal_client-1.3.0a0/fractal/common/schemas/user.py
--rw-r--r--   0        0        0     2502 2023-05-11 16:07:56.531485 fractal_client-1.3.0a0/fractal/common/schemas/workflow.py
--rw-r--r--   0        0        0      415 2023-03-06 13:52:30.189594 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      415 2023-03-07 09:47:31.002846 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      415 2023-04-20 07:57:03.191274 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1578 2023-03-06 13:52:30.221594 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1578 2023-03-07 09:47:31.038845 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      606 2023-05-15 11:49:28.546463 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3382 2023-03-15 10:53:32.644401 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3382 2023-04-20 07:57:03.471272 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      859 2023-03-06 13:52:30.469591 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      859 2023-03-07 09:47:31.354842 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      859 2023-04-20 07:57:03.471272 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-06 13:52:30.469591 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1164 2023-04-20 07:56:23.111495 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1164 2023-04-20 07:57:03.471272 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1763 2023-03-06 14:08:06.438014 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1763 2023-03-07 09:47:31.358842 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1763 2023-04-20 07:57:03.471272 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2222 2023-03-06 13:52:30.473591 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2222 2023-03-07 09:47:31.358842 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2222 2023-04-20 07:57:03.475272 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1317 2023-03-06 13:52:30.473591 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2213 2023-04-20 07:56:23.115495 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2213 2023-04-20 07:57:03.479272 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2579 2023-03-06 14:43:41.164713 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3032 2023-04-20 07:56:23.115495 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2911 2023-05-15 11:49:28.882460 fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-03-06 13:52:21.001699 fractal_client-1.3.0a0/fractal/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-05-11 16:07:56.531485 fractal_client-1.3.0a0/fractal/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-03-14 13:42:31.592919 fractal_client-1.3.0a0/fractal/common/tests/test_dataset.py
--rw-r--r--   0        0        0      541 2023-03-06 13:52:21.001699 fractal_client-1.3.0a0/fractal/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-04-06 11:30:39.096144 fractal_client-1.3.0a0/fractal/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-03-06 14:07:44.150418 fractal_client-1.3.0a0/fractal/common/tests/test_state.py
--rw-r--r--   0        0        0      748 2023-03-06 13:52:21.001699 fractal_client-1.3.0a0/fractal/common/tests/test_task.py
--rw-r--r--   0        0        0     1224 2023-04-06 11:30:39.096144 fractal_client-1.3.0a0/fractal/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-05-11 16:07:56.531485 fractal_client-1.3.0a0/fractal/common/tests/test_workflow.py
--rw-r--r--   0        0        0     1285 2023-05-12 13:33:57.004876 fractal_client-1.3.0a0/fractal/config.py
--rw-r--r--   0        0        0     1609 2023-05-09 19:58:57.316677 fractal_client-1.3.0a0/fractal/interface.py
--rw-r--r--   0        0        0    21649 2023-05-15 12:45:04.215004 fractal_client-1.3.0a0/fractal/parser.py
--rw-r--r--   0        0        0     1265 2023-05-09 19:58:57.316677 fractal_client-1.3.0a0/fractal/response.py
--rw-r--r--   0        0        0     1824 2023-05-15 12:57:11.406870 fractal_client-1.3.0a0/pyproject.toml
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 fractal_client-1.3.0a0/setup.py
--rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 fractal_client-1.3.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1576 2023-05-09 19:58:57.312677 fractal_client-1.3.0a1/LICENSE
+-rw-r--r--   0        0        0     2619 2023-05-09 19:58:57.312677 fractal_client-1.3.0a1/README.md
+-rw-r--r--   0        0        0       24 2023-06-12 06:40:22.416526 fractal_client-1.3.0a1/fractal/__init__.py
+-rw-r--r--   0        0        0      124 2023-05-26 13:31:24.681931 fractal_client-1.3.0a1/fractal/__main__.py
+-rw-r--r--   0        0        0     3448 2023-05-26 13:44:53.339222 fractal_client-1.3.0a1/fractal/authclient.py
+-rw-r--r--   0        0        0     3773 2023-05-30 07:19:20.910204 fractal_client-1.3.0a1/fractal/client.py
+-rw-r--r--   0        0        0    12249 2023-06-12 06:40:09.560661 fractal_client-1.3.0a1/fractal/cmd/__init__.py
+-rw-r--r--   0        0        0     6863 2023-06-05 08:33:35.839631 fractal_client-1.3.0a1/fractal/cmd/_aux_task_caching.py
+-rw-r--r--   0        0        0     5795 2023-06-06 12:51:00.225986 fractal_client-1.3.0a1/fractal/cmd/_dataset.py
+-rw-r--r--   0        0        0     5115 2023-06-06 12:51:00.229986 fractal_client-1.3.0a1/fractal/cmd/_job.py
+-rw-r--r--   0        0        0     4031 2023-06-06 12:51:00.229986 fractal_client-1.3.0a1/fractal/cmd/_project.py
+-rw-r--r--   0        0        0     5954 2023-06-12 06:40:09.560661 fractal_client-1.3.0a1/fractal/cmd/_task.py
+-rw-r--r--   0        0        0     4620 2023-06-06 12:51:00.229986 fractal_client-1.3.0a1/fractal/cmd/_user.py
+-rw-r--r--   0        0        0     9027 2023-06-12 06:40:09.560661 fractal_client-1.3.0a1/fractal/cmd/_workflow.py
+-rw-r--r--   0        0        0       42 2023-02-21 08:49:25.750218 fractal_client-1.3.0a1/fractal/common/.git
+-rw-r--r--   0        0        0      717 2023-03-06 13:52:20.997699 fractal_client-1.3.0a1/fractal/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-21 08:49:27.594201 fractal_client-1.3.0a1/fractal/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-03-06 13:52:21.001699 fractal_client-1.3.0a1/fractal/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-21 08:49:27.594201 fractal_client-1.3.0a1/fractal/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-03-06 13:52:21.001699 fractal_client-1.3.0a1/fractal/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-21 08:49:27.594201 fractal_client-1.3.0a1/fractal/common/__init__.py
+-rw-r--r--   0        0        0      149 2023-02-21 10:13:04.505672 fractal_client-1.3.0a1/fractal/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      147 2023-03-16 09:04:47.705157 fractal_client-1.3.0a1/fractal/common/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0       57 2023-05-26 06:48:59.488787 fractal_client-1.3.0a1/fractal/common/requirements.txt
+-rw-r--r--   0        0        0      614 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/schemas/__init__.py
+-rw-r--r--   0        0        0      411 2023-05-25 12:32:05.945818 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      372 2023-03-16 09:04:47.705157 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      490 2023-03-03 14:13:42.839064 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1753 2023-04-20 07:56:22.895496 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1251 2023-03-16 09:04:47.793156 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc
+-rw-r--r--   0        0        0     1610 2023-05-26 06:49:58.096032 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2027 2023-03-16 09:04:47.705157 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc
+-rw-r--r--   0        0        0     3459 2023-05-25 12:32:06.081816 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     3515 2023-03-16 09:04:47.797156 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc
+-rw-r--r--   0        0        0     3537 2023-05-26 06:49:58.132032 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     3711 2023-03-16 09:04:47.797156 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/project.cpython-39.pyc
+-rw-r--r--   0        0        0     1165 2023-05-26 06:49:58.136032 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1185 2023-03-16 09:04:47.801156 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/state.cpython-39.pyc
+-rw-r--r--   0        0        0     3109 2023-05-26 06:49:58.136032 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     4994 2023-03-16 09:04:47.805156 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/task.cpython-39.pyc
+-rw-r--r--   0        0        0     3098 2023-05-25 12:32:06.097816 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1202 2023-05-25 12:32:06.097816 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1024 2023-03-16 09:04:47.809156 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/user.cpython-39.pyc
+-rw-r--r--   0        0        0     3882 2023-05-26 06:49:58.328029 fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     1616 2023-04-06 11:30:39.096144 fractal_client-1.3.0a1/fractal/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1117 2023-05-26 06:48:59.488787 fractal_client-1.3.0a1/fractal/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     2769 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2483 2023-05-26 06:48:59.488787 fractal_client-1.3.0a1/fractal/common/schemas/project.py
+-rw-r--r--   0        0        0      673 2023-05-26 06:48:59.488787 fractal_client-1.3.0a1/fractal/common/schemas/state.py
+-rw-r--r--   0        0        0     2872 2023-05-26 06:48:59.488787 fractal_client-1.3.0a1/fractal/common/schemas/task.py
+-rw-r--r--   0        0        0     2741 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/schemas/task_collection.py
+-rw-r--r--   0        0        0     1216 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/schemas/user.py
+-rw-r--r--   0        0        0     2457 2023-05-26 06:48:59.488787 fractal_client-1.3.0a1/fractal/common/schemas/workflow.py
+-rw-r--r--   0        0        0      415 2023-03-06 13:52:30.189594 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      415 2023-03-07 09:47:31.002846 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      415 2023-04-20 07:57:03.191274 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1578 2023-03-06 13:52:30.221594 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1578 2023-03-07 09:47:31.038845 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      606 2023-05-15 11:49:28.546463 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3382 2023-03-15 10:53:32.644401 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3382 2023-04-20 07:57:03.471272 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      859 2023-03-06 13:52:30.469591 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      859 2023-03-07 09:47:31.354842 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      859 2023-04-20 07:57:03.471272 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-06 13:52:30.469591 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1164 2023-04-20 07:56:23.111495 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1164 2023-04-20 07:57:03.471272 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1763 2023-03-06 14:08:06.438014 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1763 2023-03-07 09:47:31.358842 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1763 2023-04-20 07:57:03.471272 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2222 2023-03-06 13:52:30.473591 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2222 2023-03-07 09:47:31.358842 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2792 2023-05-25 12:32:06.297813 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1224 2023-05-25 12:32:06.297813 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1317 2023-03-06 13:52:30.473591 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2213 2023-04-20 07:56:23.115495 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2671 2023-05-25 12:32:06.301813 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2579 2023-03-06 14:43:41.164713 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3032 2023-04-20 07:56:23.115495 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2911 2023-05-15 11:49:28.882460 fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      139 2023-03-06 13:52:21.001699 fractal_client-1.3.0a1/fractal/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-05-11 16:07:56.531485 fractal_client-1.3.0a1/fractal/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-03-14 13:42:31.592919 fractal_client-1.3.0a1/fractal/common/tests/test_dataset.py
+-rw-r--r--   0        0        0      541 2023-03-06 13:52:21.001699 fractal_client-1.3.0a1/fractal/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-04-06 11:30:39.096144 fractal_client-1.3.0a1/fractal/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-03-06 14:07:44.150418 fractal_client-1.3.0a1/fractal/common/tests/test_state.py
+-rw-r--r--   0        0        0     1190 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/tests/test_task.py
+-rw-r--r--   0        0        0      773 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/tests/test_task_collection.py
+-rw-r--r--   0        0        0     1499 2023-05-25 12:31:57.653940 fractal_client-1.3.0a1/fractal/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-05-11 16:07:56.531485 fractal_client-1.3.0a1/fractal/common/tests/test_workflow.py
+-rw-r--r--   0        0        0     1285 2023-05-12 13:33:57.004876 fractal_client-1.3.0a1/fractal/config.py
+-rw-r--r--   0        0        0     1609 2023-05-09 19:58:57.316677 fractal_client-1.3.0a1/fractal/interface.py
+-rw-r--r--   0        0        0    23230 2023-06-12 06:40:09.560661 fractal_client-1.3.0a1/fractal/parser.py
+-rw-r--r--   0        0        0     1265 2023-05-09 19:58:57.316677 fractal_client-1.3.0a1/fractal/response.py
+-rw-r--r--   0        0        0     1825 2023-06-12 06:40:22.416526 fractal_client-1.3.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 fractal_client-1.3.0a1/PKG-INFO
```

### Comparing `fractal_client-1.3.0a0/LICENSE` & `fractal_client-1.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/README.md` & `fractal_client-1.3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/authclient.py` & `fractal_client-1.3.0a1/fractal/authclient.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/client.py` & `fractal_client-1.3.0a1/fractal/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,15 +83,19 @@
         handler = getattr(cmd, args.cmd)
     else:
         # no command provided. Print help and exit 1
         parser_main.print_help()
         exit(1)
 
     try:
-        kwargs = vars(args)
+        # Make a copy of vars(args), and remove cmd (which is not a relevant
+        # argument for functions called with **kwargs)
+        kwargs = vars(args).copy()
+        kwargs.pop("cmd")
+
         if args.cmd == "version":
             async with AsyncClient() as client:
                 interface = await handler(client, **kwargs)
         else:
             # Extract (and remove) username/password for AuthClient from kwargs
             username = kwargs.pop("user") or settings.FRACTAL_USER
             password = kwargs.pop("password") or settings.FRACTAL_PASSWORD
```

### Comparing `fractal_client-1.3.0a0/fractal/cmd/_dataset.py` & `fractal_client-1.3.0a1/fractal/cmd/_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,26 +16,32 @@
 from ..interface import RichConsoleInterface
 from ..interface import RichJsonInterface
 from ..response import check_response
 
 
 async def post_dataset(
     client: AuthClient,
+    *,
     project_id: int,
     dataset_name: str,
-    metadata_filename: Optional[str] = None,
+    metadata: Optional[str] = None,
     type: Optional[str] = None,
     batch: bool = False,
-    **kwargs,
 ) -> RichJsonInterface:
-
-    if metadata_filename is None:
+    """
+    Arguments:
+        project_id: ID of project to add the new dataset to
+        dataset_name: Name of new dataset
+        metadata: Path to file containing dataset metadata in JSON format.
+        type: Dataset type.
+    """
+    if metadata is None:
         meta = {}
     else:
-        with open(metadata_filename, "r") as f:
+        with open(metadata, "r") as f:
             meta = json.load(f)
 
     dataset_dict = dict(name=dataset_name, meta=meta)
     if type:
         dataset_dict["type"] = type
     dataset = DatasetCreate(**dataset_dict)
 
@@ -51,19 +57,18 @@
     else:
         return RichJsonInterface(retcode=0, data=new_dataset.dict())
 
 
 async def post_resource(
     client: AuthClient,
     *,
-    batch: bool = False,
     project_id: int,
     dataset_id: int,
     path: str,
-    **kwargs,
+    batch: bool = False,
 ) -> BaseInterface:
 
     # Check that path is absolute, which is needed for when the server submits
     # tasks as a different user
     if not os.path.isabs(path):
         msg = f"{path=} is not an absolute path"
         raise ValueError(msg)
@@ -88,15 +93,14 @@
 
 async def delete_resource(
     client: AuthClient,
     *,
     project_id: int,
     dataset_id: int,
     resource_id: int,
-    **kwargs,
 ) -> BaseInterface:
     res = await client.delete(
         (
             f"{settings.BASE_URL}/project/{project_id}/"
             f"dataset/{dataset_id}/resource/{resource_id}"
         )
     )
@@ -110,15 +114,14 @@
     project_id: int,
     dataset_id: int,
     new_name: Optional[str] = None,
     new_type: Optional[str] = None,
     meta_file: Optional[str] = None,
     make_read_only: bool = False,
     remove_read_only: bool = False,
-    **kwargs,
 ) -> BaseInterface:
 
     # Prepare payload
     dataset_update_dict = {}
     if new_name:
         dataset_update_dict["name"] = new_name
     if new_type:
@@ -144,52 +147,49 @@
     new_dataset = check_response(
         res, expected_status_code=200, coerce=DatasetRead
     )
     return RichJsonInterface(retcode=0, data=new_dataset.dict())
 
 
 async def get_dataset(
-    client: AuthClient, *, project_id: int, dataset_id: int, **kwargs
+    client: AuthClient, *, project_id: int, dataset_id: int
 ) -> BaseInterface:
     res = await client.get(
         f"{settings.BASE_URL}/project/{project_id}/dataset/{dataset_id}"
     )
     from rich.console import Group
 
     dataset = check_response(res, expected_status_code=200, coerce=DatasetRead)
 
-    if kwargs.get("json", False):
-        return RichJsonInterface(retcode=0, data=dataset.dict())
-    else:
-        table = Table(title="Dataset")
-        table.add_column("ID", style="cyan", no_wrap=True)
-        table.add_column("Name", justify="right", style="green")
-        table.add_column("Type", style="white")
-        table.add_column("Meta", justify="center")
-        table.add_column("Read only", justify="center")
-
-        table.add_row(
-            str(dataset.id),
-            dataset.name,
-            dataset.type,
-            json.dumps(dataset.meta, indent=2),
-            "✅" if dataset.read_only else "❌",
-        )
-        table_res = Table(title="Resources")
-        table_res.add_column("Path", justify="center", style="yellow")
-        table_res.add_column("ID", justify="center", style="yellow")
-        table_res.add_column("Dataset ID", justify="center", style="yellow")
-        for r in dataset.resource_list:
-            table_res.add_row(r.path, str(r.id), str(r.dataset_id))
-        group = Group(table, table_res)
-        return RichConsoleInterface(retcode=0, data=group)
+    table = Table(title="Dataset")
+    table.add_column("ID", style="cyan", no_wrap=True)
+    table.add_column("Name", justify="right", style="green")
+    table.add_column("Type", style="white")
+    table.add_column("Meta", justify="center")
+    table.add_column("Read only", justify="center")
+
+    table.add_row(
+        str(dataset.id),
+        dataset.name,
+        dataset.type,
+        json.dumps(dataset.meta, indent=2),
+        "✅" if dataset.read_only else "❌",
+    )
+    table_res = Table(title="Resources")
+    table_res.add_column("Path", justify="center", style="yellow")
+    table_res.add_column("ID", justify="center", style="yellow")
+    table_res.add_column("Dataset ID", justify="center", style="yellow")
+    for r in dataset.resource_list:
+        table_res.add_row(r.path, str(r.id), str(r.dataset_id))
+    group = Group(table, table_res)
+    return RichConsoleInterface(retcode=0, data=group)
 
 
 async def delete_dataset(
-    client: AuthClient, project_id: int, dataset_id: int, **kwargs
+    client: AuthClient, *, project_id: int, dataset_id: int
 ) -> PrintInterface:
 
     res = await client.delete(
         f"{settings.BASE_URL}/project/{project_id}/dataset/{dataset_id}"
     )
     check_response(res, expected_status_code=204)
     return PrintInterface(retcode=0, data="")
```

### Comparing `fractal_client-1.3.0a0/fractal/cmd/_job.py` & `fractal_client-1.3.0a1/fractal/cmd/_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from ..interface import RichConsoleInterface
 from ..interface import RichJsonInterface
 from ..response import check_response
 
 
 async def get_job(
     client: AuthClient,
+    *,
     project_id: int,
     job_id: int,
-    batch: bool = False,
     do_not_separate_logs: bool = False,
-    **kwargs,
+    batch: bool = False,
 ) -> BaseInterface:
     """
     Query the status of a workflow-execution job
     """
 
     res = await client.get(
         f"{settings.BASE_URL}/project/{project_id}/job/{job_id}"
@@ -44,18 +44,15 @@
             extra_lines = ["\nThis is the job log:\n", log]
             return RichJsonInterface(
                 retcode=0, data=data, extra_lines=extra_lines
             )
 
 
 async def get_job_list(
-    client: AuthClient,
-    project_id: int,
-    batch: bool = False,
-    **kwargs,
+    client: AuthClient, *, project_id: int, batch: bool = False
 ) -> BaseInterface:
 
     res = await client.get(f"{settings.BASE_URL}/project/{project_id}/job/")
     jobs = check_response(res, expected_status_code=200)
 
     # Coerce to a list of ApplyWorkflowRead objects
     jobs = [ApplyWorkflowRead(**job) for job in jobs]
@@ -82,18 +79,18 @@
                 j.working_dir,
             )
         return RichConsoleInterface(retcode=0, data=table)
 
 
 async def get_job_logs(
     client: AuthClient,
+    *,
     project_id: int,
     job_id: int,
     output_folder: str,
-    **kwargs,
 ) -> BaseInterface:
 
     # Check that output_folder does not already exist
     if Path(output_folder).exists():
         return PrintInterface(
             retcode=1, data=f"ERROR: {output_folder=} already exists"
         )
@@ -149,18 +146,15 @@
 
     return PrintInterface(
         retcode=0, data=f"Logs downloaded to {output_folder=}"
     )
 
 
 async def stop_job(
-    client: AuthClient,
-    project_id: int,
-    job_id: int,
-    **kwargs,
+    client: AuthClient, *, project_id: int, job_id: int
 ) -> BaseInterface:
     """
     Stop a workflow-execution job
     """
 
     res = await client.get(
         f"{settings.BASE_URL}/project/{project_id}/job/{job_id}/stop/"
```

### Comparing `fractal_client-1.3.0a0/fractal/cmd/_project.py` & `fractal_client-1.3.0a1/fractal/cmd/_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 from typing import Optional
 from typing import Union
 
 from rich.table import Table
 
 from ..authclient import AuthClient
 from ..common.schemas import ProjectCreate
@@ -14,25 +13,24 @@
 from ..interface import RichConsoleInterface
 from ..interface import RichJsonInterface
 from ..response import check_response
 
 
 async def post_project(
     client: AuthClient,
+    *,
     name: str,
     dataset: Optional[str] = None,
     batch: bool = False,
-    **kwargs,
 ) -> BaseInterface:
     # Prepare a ProjectCreate request body
     project_dict = dict(name=name)
     if dataset:
         project_dict["default_dataset_name"] = dataset
     project = ProjectCreate(**project_dict)
-    logging.info(project)
     # Send API request
     res = await client.post(
         f"{settings.BASE_URL}/project/",
         json=project.dict(exclude_unset=True),
     )
     project = check_response(res, expected_status_code=201, coerce=ProjectRead)
     if batch:
@@ -44,17 +42,15 @@
             raise ValueError(msg)
         dataset_id = project.dataset_list[0].id
         return PrintInterface(retcode=0, data=f"{project.id} {dataset_id}")
     else:
         return RichJsonInterface(retcode=0, data=project.dict())
 
 
-async def get_project_list(
-    client: AuthClient, **kwargs
-) -> RichConsoleInterface:
+async def get_project_list(client: AuthClient) -> RichConsoleInterface:
 
     res = await client.get(f"{settings.BASE_URL}/project/")
     res = check_response(res, expected_status_code=200)
 
     projects = [ProjectRead(**item) for item in res]
 
     table = Table(title="Project List")
@@ -80,41 +76,41 @@
             read_only_icon,
         )
 
     return RichConsoleInterface(retcode=0, data=table)
 
 
 async def get_project(
-    client: AuthClient, project_id: int, **kwargs
+    client: AuthClient, *, project_id: int
 ) -> RichJsonInterface:
     res = await client.get(
         f"{settings.BASE_URL}/project/{project_id}",
     )
     project = check_response(res, expected_status_code=200, coerce=ProjectRead)
     return RichJsonInterface(retcode=0, data=project.dict())
 
 
 async def delete_project(
-    client: AuthClient, project_id: int, **kwargs
+    client: AuthClient, *, project_id: int
 ) -> PrintInterface:
 
     res = await client.delete(
         f"{settings.BASE_URL}/project/{project_id}",
     )
     check_response(res, expected_status_code=204)
     return PrintInterface(retcode=0, data="")
 
 
 async def patch_project(
     client: AuthClient,
+    *,
     project_id: int,
     new_name: Optional[str] = None,
     make_read_only: bool = False,
     remove_read_only: bool = False,
-    **kwargs,
 ) -> Union[RichJsonInterface, PrintInterface]:
     update = {}
     if new_name:
         update["name"] = new_name
     if make_read_only:
         update["read_only"] = True
     if remove_read_only:
```

### Comparing `fractal_client-1.3.0a0/fractal/cmd/_task.py` & `fractal_client-1.3.0a1/fractal/cmd/_task.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 import json
+import logging
+import sys
 from typing import Optional
 
 from ..authclient import AuthClient
 from ..common.schemas import StateRead
 from ..common.schemas import TaskCollectPip
 from ..common.schemas import TaskCreate
 from ..common.schemas import TaskRead
 from ..common.schemas import TaskUpdate
 from ..config import settings
 from ..interface import BaseInterface
 from ..interface import PrintInterface
 from ..interface import RichJsonInterface
 from ..response import check_response
-from .utils import get_cached_task_by_name
-from .utils import refresh_task_cache
+from ._aux_task_caching import FractalCacheError
+from ._aux_task_caching import get_task_id_from_cache
+from ._aux_task_caching import refresh_task_cache
 
 
-async def get_task_list(client: AuthClient, **kwargs) -> RichJsonInterface:
-    task_list = await refresh_task_cache(client=client, **kwargs)
+async def get_task_list(client: AuthClient) -> RichJsonInterface:
+    task_list = await refresh_task_cache(client=client)
     return RichJsonInterface(retcode=0, data=task_list)
 
 
 async def task_collect_pip(
     client: AuthClient,
     *,
     package: str,
     package_version: Optional[str] = None,
-    python_version: Optional[str],
+    python_version: Optional[str] = None,
     package_extras: Optional[str] = None,
-    private: Optional[bool] = False,
     batch: bool = False,
-    **kwargs,
 ) -> BaseInterface:
-    task_collect = TaskCollectPip(
-        package=package,
-        version=package_version,
-        python_version=python_version,
-        package_extras=package_extras,
-    )
+
+    # Construct TaskCollectPip object
+    attributes = dict(package=package)
+    if package_version:
+        attributes["package_version"] = package_version
+    if python_version:
+        attributes["python_version"] = python_version
+    if package_extras:
+        attributes["package_extras"] = package_extras
+    task_collect = TaskCollectPip(**attributes)
 
     res = await client.post(
-        f"{settings.BASE_URL}/task/collect/pip/?public={not private}",
-        json=task_collect.dict(),
+        f"{settings.BASE_URL}/task/collect/pip/",
+        json=task_collect.dict(exclude_unset=True),
     )
 
     state = check_response(
         res, expected_status_code=[200, 201], coerce=StateRead
     )
     if batch:
         output = f"{state.id} {state.data['venv_path']}"
@@ -87,22 +92,24 @@
 
 async def post_task(
     client: AuthClient,
     *,
     name: str,
     command: str,
     source: str,
-    batch: bool = False,
-    input_type: Optional[str] = "Any",
-    output_type: Optional[str] = "Any",
+    input_type: str = "Any",
+    output_type: str = "Any",
+    version: Optional[str] = None,
     default_args_file: Optional[str] = None,
     meta_file: Optional[str] = None,
-    **kwargs,
+    batch: bool = False,
 ) -> BaseInterface:
     optionals = {}
+    if version:
+        optionals["version"] = version
     if default_args_file:
         with open(default_args_file, "r") as f:
             optionals["default_args"] = json.load(f)
     if meta_file:
         with open(meta_file, "r") as f:
             optionals["meta"] = json.load(f)
     payload = TaskCreate(
@@ -121,62 +128,71 @@
     else:
         return RichJsonInterface(retcode=0, data=new_task.dict())
 
 
 async def patch_task(
     client: AuthClient,
     *,
-    task_id_or_name: str,
+    id: Optional[int] = None,
     name: Optional[str] = None,
-    command: Optional[str] = None,
-    input_type: Optional[str] = None,
-    output_type: Optional[str] = None,
+    version: Optional[str] = None,
+    new_name: Optional[str] = None,
+    new_command: Optional[str] = None,
+    new_input_type: Optional[str] = None,
+    new_output_type: Optional[str] = None,
+    new_version: Optional[str] = None,
     default_args_file: Optional[str] = None,
     meta_file: Optional[str] = None,
-    **kwargs,
 ) -> BaseInterface:
+
+    if id:
+        if version:
+            logging.error(
+                "Too many arguments: cannot provide both `id` and `version`."
+            )
+            sys.exit(1)
+    else:
+        try:
+            id = await get_task_id_from_cache(
+                client=client, task_name=name, version=version
+            )
+        except FractalCacheError as e:
+            print(e)
+            sys.exit(1)
+
     update = {}
-    if name:
-        update["name"] = name
-    if command:
-        update["command"] = command
-    if input_type:
-        update["input_type"] = input_type
-    if output_type:
-        update["output_type"] = output_type
+    if new_name:
+        update["name"] = new_name
+    if new_command:
+        update["command"] = new_command
+    if new_version:
+        update["version"] = new_version
+    if new_input_type:
+        update["input_type"] = new_input_type
+    if new_output_type:
+        update["output_type"] = new_output_type
     if default_args_file:
         with open(default_args_file, "r") as f:
             update["default_args"] = json.load(f)
     if meta_file:
         with open(meta_file, "r") as f:
             update["meta"] = json.load(f)
 
-    task_update = TaskUpdate(**update)  # validation
+    task_update = TaskUpdate(**update)
     payload = task_update.dict(exclude_unset=True)
     if not payload:
         return PrintInterface(retcode=1, data="Nothing to update")
 
-    try:
-        task_id = int(task_id_or_name)
-    except ValueError:
-        task_id = await get_cached_task_by_name(
-            name=task_id_or_name, client=client
-        )
-
-    res = await client.patch(
-        f"{settings.BASE_URL}/task/{task_id}", json=payload
-    )
+    res = await client.patch(f"{settings.BASE_URL}/task/{id}", json=payload)
     new_task = check_response(res, expected_status_code=200, coerce=TaskRead)
     return RichJsonInterface(retcode=0, data=new_task.dict())
 
 
 async def delete_task(
-    client: AuthClient, *, task_id: int = None, **kwargs
+    client: AuthClient,
+    *,
+    id: Optional[int] = None,
+    name: Optional[str] = None,
+    version: Optional[str] = None,
 ) -> PrintInterface:
 
     raise NotImplementedError("task_delete")
-
-    # res = await client.delete(
-    #    f"{settings.BASE_URL}/xxxx"
-    # )
-    # check_response(res, expected_status_code=204)
-    # return PrintInterface(retcode=0, data="")
```

### Comparing `fractal_client-1.3.0a0/fractal/cmd/_user.py` & `fractal_client-1.3.0a1/fractal/cmd/_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,31 +9,34 @@
 from ..interface import PrintInterface
 from ..interface import RichJsonInterface
 from ..response import check_response
 
 
 async def user_register(
     client: AuthClient,
+    *,
     new_email: str,
     new_password: Optional[str] = None,
     slurm_user: Optional[str] = None,
     cache_dir: Optional[str] = None,
+    username: Optional[str] = None,
     superuser: bool = False,
     batch: bool = False,
-    **kwargs,
 ) -> Union[RichJsonInterface, PrintInterface]:
 
     user_dict = dict(
         email=new_email,
         password=new_password,
     )
     if slurm_user:
         user_dict["slurm_user"] = slurm_user
     if cache_dir:
         user_dict["cache_dir"] = cache_dir
+    if username:
+        user_dict["username"] = username
     new_user = UserCreate(**user_dict)
 
     from getpass import getpass
 
     if new_password is None:
         new_password = getpass()
         confirm_new_password = getpass("Confirm password: ")
@@ -58,89 +61,90 @@
 
     if batch:
         return PrintInterface(retcode=0, data=data.id)
     else:
         return RichJsonInterface(retcode=0, data=data.dict())
 
 
-async def user_list(client: AuthClient, **kwargs) -> RichJsonInterface:
+async def user_list(client: AuthClient) -> RichJsonInterface:
     res = await client.get(f"{settings.FRACTAL_SERVER}/auth/userlist")
     users = check_response(res, expected_status_code=200)
     users = [UserRead(**user).dict() for user in users]
     return RichJsonInterface(
         retcode=0,
         data=users,
     )
 
 
-async def user_show(
-    client: AuthClient, user_id: str, **kwargs
-) -> RichJsonInterface:
+async def user_show(client: AuthClient, *, user_id: str) -> RichJsonInterface:
     res = await client.get(f"{settings.FRACTAL_SERVER}/auth/users/{user_id}")
     user = check_response(res, expected_status_code=200, coerce=UserRead)
     return RichJsonInterface(
         retcode=0,
         data=user.dict(),
     )
 
 
 async def user_edit(
     client: AuthClient,
+    *,
     user_id: str,
     new_email: Optional[str] = None,
     new_password: Optional[str] = None,
     new_slurm_user: Optional[str] = None,
     new_cache_dir: Optional[str] = None,
+    new_username: Optional[str] = None,
     make_superuser: bool = False,
     remove_superuser: bool = False,
-    **kwargs,
 ) -> Union[RichJsonInterface, PrintInterface]:
+
     user_dict = dict(
         email=new_email,
         password=new_password,
     )
+
     if new_cache_dir is not None:
         user_dict["cache_dir"] = new_cache_dir
     if new_slurm_user is not None:
         user_dict["slurm_user"] = new_slurm_user
+    if new_username is not None:
+        user_dict["username"] = new_username
+
     user_update = UserUpdate(**user_dict)
 
     if make_superuser:
         user_update.is_superuser = True
     if remove_superuser:
         user_update.is_superuser = False
 
     payload = user_update.dict(exclude_unset=True, exclude_none=True)
     if not payload:
         return PrintInterface(retcode=1, data="Nothing to update")
-
     res = await client.patch(
         f"{settings.FRACTAL_SERVER}/auth/users/{user_id}", json=payload
     )
     new_user = check_response(res, expected_status_code=200, coerce=UserRead)
 
     return RichJsonInterface(
         retcode=0,
         data=new_user.dict(),
     )
 
 
-async def user_delete(
-    client: AuthClient, user_id: str, **kwargs
-) -> PrintInterface:
+async def user_delete(client: AuthClient, *, user_id: str) -> PrintInterface:
 
     res = await client.delete(
         f"{settings.FRACTAL_SERVER}/auth/users/{user_id}"
     )
     check_response(res, expected_status_code=204)
     return PrintInterface(retcode=0, data="")
 
 
 async def user_whoami(
-    client: AuthClient, batch: bool, **kwargs
+    client: AuthClient, *, batch: bool
 ) -> Union[RichJsonInterface, PrintInterface]:
     res = await client.get(f"{settings.FRACTAL_SERVER}/auth/whoami")
     user = check_response(res, expected_status_code=200, coerce=UserRead)
 
     if batch:
         return PrintInterface(retcode=0, data=user.id)
     else:
```

### Comparing `fractal_client-1.3.0a0/fractal/cmd/_workflow.py` & `fractal_client-1.3.0a1/fractal/cmd/_workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+import sys
 from pathlib import Path
 from typing import Optional
 
 from ..authclient import AuthClient
 from ..common.schemas import ApplyWorkflowCreate
 from ..common.schemas import ApplyWorkflowRead
 from ..common.schemas import WorkflowCreate
@@ -15,76 +16,61 @@
 from ..common.schemas import WorkflowTaskUpdate
 from ..common.schemas import WorkflowUpdate
 from ..config import settings
 from ..interface import BaseInterface
 from ..interface import PrintInterface
 from ..interface import RichJsonInterface
 from ..response import check_response
-from .utils import get_cached_task_by_name
+from ._aux_task_caching import FractalCacheError
+from ._aux_task_caching import get_task_id_from_cache
 
 
 async def post_workflow(
-    client: AuthClient,
-    name: str,
-    project_id: int,
-    batch: bool = False,
-    **kwargs,
+    client: AuthClient, *, name: str, project_id: int, batch: bool = False
 ) -> BaseInterface:
     workflow = WorkflowCreate(
         name=name,
         project_id=project_id,
     )
-    logging.info(workflow)
     res = await client.post(
         f"{settings.BASE_URL}/project/{project_id}/workflow/",
         json=workflow.dict(),
     )
     workflow = check_response(
         res, expected_status_code=201, coerce=WorkflowRead
     )
     if batch:
         return PrintInterface(retcode=0, data=workflow.id)
     else:
         return RichJsonInterface(retcode=0, data=workflow.dict())
 
 
 async def get_workflow_list(
-    client: AuthClient,
-    project_id: int,
-    batch: bool = False,
-    **kwargs,
+    client: AuthClient, *, project_id: int, batch: bool = False
 ) -> RichJsonInterface:
 
     res = await client.get(
         f"{settings.BASE_URL}/project/{project_id}/workflow/"
     )
     workflow_list = check_response(res, expected_status_code=200)
     return RichJsonInterface(retcode=0, data=workflow_list)
 
 
 async def delete_workflow(
-    client: AuthClient,
-    *,
-    project_id: int,
-    workflow_id: int,
-    **kwargs,
+    client: AuthClient, *, project_id: int, workflow_id: int
 ) -> BaseInterface:
     res = await client.delete(
         f"{settings.BASE_URL}/project/{project_id}/workflow/{workflow_id}"
     )
     check_response(res, expected_status_code=204)
     return PrintInterface(retcode=0, data="")
 
 
 async def get_workflow(
-    client: AuthClient,
-    *,
-    project_id: int,
-    workflow_id: int,
-    **kwargs,
+    client: AuthClient, *, project_id: int, workflow_id: int
 ) -> RichJsonInterface:
     res = await client.get(
         f"{settings.BASE_URL}/project/{project_id}/workflow/{workflow_id}"
     )
     workflow = check_response(
         res, expected_status_code=200, coerce=WorkflowRead
     )
@@ -92,26 +78,38 @@
 
 
 async def post_workflowtask(
     client: AuthClient,
     *,
     project_id: int,
     workflow_id: int,
+    task_id: Optional[int] = None,
+    task_name: Optional[str] = None,
+    task_version: Optional[str] = None,
     batch: bool = False,
-    task_id_or_name: str,
     order: Optional[int] = None,
     args_file: Optional[str] = None,
     meta_file: Optional[str] = None,
-    **kwargs,
 ) -> RichJsonInterface:
 
-    try:
-        task_id = int(task_id_or_name)
-    except ValueError:
-        task_id = await get_cached_task_by_name(task_id_or_name, client)
+    if task_id:
+        if task_version:
+            logging.error(
+                "Too many arguments: cannot provide both "
+                "`task_id` and `task_version`."
+            )
+            sys.exit(1)
+    else:
+        try:
+            task_id = await get_task_id_from_cache(
+                client=client, task_name=task_name, version=task_version
+            )
+        except FractalCacheError as e:
+            print(e)
+            sys.exit(1)
 
     if order is None:
         workflow_task = WorkflowTaskCreate()
     else:
         workflow_task = WorkflowTaskCreate(order=order)
     if args_file:
         with Path(args_file).open("r") as f:
@@ -144,15 +142,14 @@
     client: AuthClient,
     *,
     project_id: int,
     workflow_id: int,
     workflow_task_id: int,
     args_file: Optional[str] = None,
     meta_file: Optional[str] = None,
-    **kwargs,
 ) -> RichJsonInterface:
 
     # Check that at least one of args_file or meta_file was given (note: it
     # would be reasonable to check it in the parser, but we are not aware of a
     # method within argparse).
     if not (args_file or meta_file):
         raise ValueError(
@@ -187,15 +184,14 @@
 
 async def delete_workflowtask(
     client: AuthClient,
     *,
     project_id: int,
     workflow_id: int,
     workflow_task_id: int,
-    **kwargs,
 ) -> BaseInterface:
 
     res = await client.delete(
         f"{settings.BASE_URL}/project/{project_id}/"
         f"workflow/{workflow_id}/wftask/{workflow_task_id}"
     )
     check_response(res, expected_status_code=204)
@@ -203,20 +199,19 @@
 
 
 async def patch_workflow(
     client: AuthClient,
     *,
     project_id: int,
     workflow_id: int,
-    **workflow_update_dict,
+    new_name: str,
 ) -> BaseInterface:
-    workflow_update = WorkflowUpdate(**workflow_update_dict)
+
+    workflow_update = WorkflowUpdate(name=new_name)
     payload = workflow_update.dict(exclude_unset=True)
-    if not payload:
-        return PrintInterface(retcode=1, data="Nothing to update")
 
     res = await client.patch(
         f"{settings.BASE_URL}/project/{project_id}/workflow/{workflow_id}",
         json=payload,
     )
     new_workflow = check_response(
         res, expected_status_code=200, coerce=WorkflowRead
@@ -228,15 +223,14 @@
     client: AuthClient,
     *,
     project_id: int,
     workflow_id: int,
     input_dataset_id: int,
     output_dataset_id: int,
     worker_init: Optional[str] = None,
-    **kwargs,
 ) -> BaseInterface:
     apply_wf_create_dict = dict(
         workflow_id=workflow_id,
         input_dataset_id=input_dataset_id,
         output_dataset_id=output_dataset_id,
     )
     # Prepare ApplyWorkflowCreate object, without None attributes
@@ -260,20 +254,15 @@
     apply_wf_read = check_response(
         res, expected_status_code=202, coerce=ApplyWorkflowRead
     )
     return RichJsonInterface(retcode=0, data=apply_wf_read.sanitised_dict())
 
 
 async def workflow_import(
-    client: AuthClient,
-    *,
-    project_id: int,
-    json_file: str,
-    batch: bool = False,
-    **kwargs,
+    client: AuthClient, *, project_id: int, json_file: str, batch: bool = False
 ) -> BaseInterface:
     with Path(json_file).open("r") as f:
         workflow = json.load(f)
     workflow = WorkflowImport(**workflow)
     res = await client.post(
         f"{settings.BASE_URL}/project/{project_id}/workflow/import/",
         json=workflow.dict(exclude_unset=True),
@@ -292,15 +281,14 @@
 
 async def workflow_export(
     client: AuthClient,
     *,
     project_id: int,
     workflow_id: int,
     json_file: str,
-    **kwargs,
 ) -> BaseInterface:
     res = await client.get(
         (
             f"{settings.BASE_URL}/project/{project_id}/"
             f"workflow/{workflow_id}/export/"
         ),
     )
```

### Comparing `fractal_client-1.3.0a0/fractal/common/.github/workflows/ci.yml` & `fractal_client-1.3.0a1/fractal/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/.pre-commit-config.yaml` & `fractal_client-1.3.0a1/fractal/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/README.md` & `fractal_client-1.3.0a1/fractal/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/__init__.py` & `fractal_client-1.3.0a1/fractal/common/schemas/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from .applyworkflow import *  # noqa: F403
 from .manifest import *  # noqa: F403
 from .project import *  # noqa: F403
 from .state import *  # noqa: F403
 from .task import *  # noqa: F403
+from .task_collection import *  # noqa: F403
 from .user import *  # noqa: F403
 from .workflow import *  # noqa: F403
 
 
 __all__ = (
     project.__all__  # noqa: F405
     + task.__all__  # noqa: F405
+    + task_collection.__all__  # noqa: F405
     + workflow.__all__  # noqa: F405
     + applyworkflow.__all__  # noqa: F405
     + manifest.__all__  # noqa: F405
     + state.__all__  # noqa: F405
     + user.__all__  # noqa: F405
 )
```

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc` & `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 11 16:07:56 2023 UTC, .py size: 1044 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,73 @@
-00000000: 6f0d 0d0a 0000 0000 dc12 5d64 1404 0000  o.........]d....
+00000000: 6f0d 0d0a 0000 0000 5b56 7064 a102 0000  o.......[Vpd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c01 6d03 5a03  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c06 6d07 5a07 0100 6406 6407 6c08  d.l.m.Z...d.d.l.
-00000070: 6d09 5a09 0100 6408 5a0a 4700 6409 640a  m.Z...d.Z.G.d.d.
-00000080: 8400 640a 6507 8303 5a0b 4700 640b 640c  ..d.e...Z.G.d.d.
-00000090: 8400 640c 650b 8303 5a0c 4700 640d 640e  ..d.e...Z.G.d.d.
-000000a0: 8400 640e 650b 8303 5a0d 640f 5300 2910  ..d.e...Z.d.S.).
-000000b0: e900 0000 0029 01da 0864 6174 6574 696d  .....)...datetim
-000000c0: 6529 01da 044c 6973 7429 01da 084f 7074  e)...List)...Opt
-000000d0: 696f 6e61 6c29 01da 0976 616c 6964 6174  ional)...validat
-000000e0: 6f72 2901 da08 5351 4c4d 6f64 656c e901  or)...SQLModel..
-000000f0: 0000 0029 01da 0676 616c 7374 7229 03da  ...)...valstr)..
-00000100: 1141 7070 6c79 576f 726b 666c 6f77 4261  .ApplyWorkflowBa
-00000110: 7365 da13 4170 706c 7957 6f72 6b66 6c6f  se..ApplyWorkflo
-00000120: 7743 7265 6174 65da 1141 7070 6c79 576f  wCreate..ApplyWo
-00000130: 726b 666c 6f77 5265 6164 6300 0000 0000  rkflowReadc.....
-00000140: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00000150: 0000 0073 1e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000160: 5500 6401 5a03 6504 6505 1900 6506 6402  U.d.Z.e.e...e.d.
-00000170: 3c00 6403 5300 2904 7209 0000 007a 500a  <.d.S.).r....zP.
-00000180: 2020 2020 4261 7365 2063 6c61 7373 2066      Base class f
-00000190: 6f72 2041 7070 6c79 576f 726b 666c 6f77  or ApplyWorkflow
-000001a0: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
-000001b0: 3a0a 2020 2020 2020 2020 776f 726b 6572  :.        worker
-000001c0: 5f69 6e69 743a 2054 4244 0a20 2020 20da  _init: TBD.    .
-000001d0: 0b77 6f72 6b65 725f 696e 6974 4e29 07da  .worker_initN)..
-000001e0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000001f0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000200: 655f 5fda 075f 5f64 6f63 5f5f 7204 0000  e__..__doc__r...
-00000210: 00da 0373 7472 da0f 5f5f 616e 6e6f 7461  ...str..__annota
-00000220: 7469 6f6e 735f 5fa9 0072 1300 0000 7213  tions__..r....r.
-00000230: 0000 00fa 452f 686f 6d65 2f74 6f6d 6d61  ....E/home/tomma
-00000240: 736f 2f46 7261 6374 616c 2f66 7261 6374  so/Fractal/fract
-00000250: 616c 2f66 7261 6374 616c 2f63 6f6d 6d6f  al/fractal/commo
-00000260: 6e2f 7363 6865 6d61 732f 6170 706c 7977  n/schemas/applyw
-00000270: 6f72 6b66 6c6f 772e 7079 7209 0000 0011  orkflow.pyr.....
-00000280: 0000 0073 0600 0000 0a00 0401 1007 7209  ...s..........r.
-00000290: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000002a0: 0000 0000 0400 0000 4000 0000 7320 0000  ........@...s ..
-000002b0: 0065 005a 0164 005a 0265 0364 0164 0264  .e.Z.d.Z.e.d.d.d
-000002c0: 038d 0265 0464 0183 0183 015a 0564 0453  ...e.d.....Z.d.S
-000002d0: 0029 0572 0a00 0000 720c 0000 0054 2901  .).r....r....T).
-000002e0: da0b 616c 6c6f 775f 7265 7573 654e 2906  ..allow_reuseN).
-000002f0: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-00000300: 0500 0000 7208 0000 00da 0c5f 776f 726b  ....r......_work
-00000310: 6572 5f69 6e69 7472 1300 0000 7213 0000  er_initr....r...
-00000320: 0072 1300 0000 7214 0000 0072 0a00 0000  .r....r....r....
-00000330: 1c00 0000 7308 0000 0008 000a 0306 0108  ....s...........
-00000340: ff72 0a00 0000 6300 0000 0000 0000 0000  .r....c.........
-00000350: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-00000360: 8200 0000 6500 5a01 6400 5a02 5500 6503  ....e.Z.d.Z.U.e.
-00000370: 6504 6401 3c00 6503 6504 6402 3c00 6503  e.d.<.e.e.d.<.e.
-00000380: 6504 6403 3c00 6503 6504 6404 3c00 6503  e.d.<.e.e.d.<.e.
-00000390: 6504 6405 3c00 6505 6504 6406 3c00 6506  e.d.<.e.e.d.<.e.
-000003a0: 6504 6407 3c00 6507 6506 1900 6504 6408  e.d.<.e.e...e.d.
-000003b0: 3c00 6507 6508 6506 1900 1900 6504 6409  <.e.e.e.....e.d.
-000003c0: 3c00 6507 6506 1900 6504 640a 3c00 6507  <.e.e...e.d.<.e.
-000003d0: 6506 1900 6504 640b 3c00 640c 640d 8400  e...e.d.<.d.d...
-000003e0: 5a09 640e 5300 290f 720b 0000 00da 0269  Z.d.S.).r......i
-000003f0: 64da 0a70 726f 6a65 6374 5f69 64da 0b77  d..project_id..w
-00000400: 6f72 6b66 6c6f 775f 6964 da10 696e 7075  orkflow_id..inpu
-00000410: 745f 6461 7461 7365 745f 6964 da11 6f75  t_dataset_id..ou
-00000420: 7470 7574 5f64 6174 6173 6574 5f69 64da  tput_dataset_id.
-00000430: 0f73 7461 7274 5f74 696d 6573 7461 6d70  .start_timestamp
-00000440: da06 7374 6174 7573 da03 6c6f 67da 0768  ..status..log..h
-00000450: 6973 746f 7279 da0b 776f 726b 696e 675f  istory..working_
-00000460: 6469 72da 1077 6f72 6b69 6e67 5f64 6972  dir..working_dir
-00000470: 5f75 7365 7263 0100 0000 0000 0000 0000  _userc..........
-00000480: 0000 0200 0000 0300 0000 4300 0000 731a  ..........C...s.
-00000490: 0000 007c 00a0 00a1 007d 0174 017c 006a  ...|.....}.t.|.j
-000004a0: 0283 017c 0164 013c 007c 0153 0029 024e  ...|.d.<.|.S.).N
-000004b0: 721c 0000 0029 03da 0464 6963 7472 1100  r....)...dictr..
-000004c0: 0000 721c 0000 0029 02da 0473 656c 66da  ..r....)...self.
-000004d0: 0164 7213 0000 0072 1300 0000 7214 0000  .dr....r....r...
-000004e0: 00da 0e73 616e 6974 6973 6564 5f64 6963  ...sanitised_dic
-000004f0: 7431 0000 0073 0600 0000 0801 0e01 0401  t1...s..........
-00000500: 7a20 4170 706c 7957 6f72 6b66 6c6f 7752  z ApplyWorkflowR
-00000510: 6561 642e 7361 6e69 7469 7365 645f 6469  ead.sanitised_di
-00000520: 6374 4e29 0a72 0d00 0000 720e 0000 0072  ctN).r....r....r
-00000530: 0f00 0000 da03 696e 7472 1200 0000 7202  ......intr....r.
-00000540: 0000 0072 1100 0000 7204 0000 0072 0300  ...r....r....r..
-00000550: 0000 7225 0000 0072 1300 0000 7213 0000  ..r%...r....r...
-00000560: 0072 1300 0000 7214 0000 0072 0b00 0000  .r....r....r....
-00000570: 2400 0000 731a 0000 000a 0008 0108 0108  $...s...........
-00000580: 0108 0108 0108 0108 010c 0110 010c 010c  ................
-00000590: 010c 0272 0b00 0000 4e29 0e72 0200 0000  ...r....N).r....
-000005a0: da06 7479 7069 6e67 7203 0000 0072 0400  ..typingr....r..
-000005b0: 0000 da08 7079 6461 6e74 6963 7205 0000  ....pydanticr...
-000005c0: 00da 0873 716c 6d6f 6465 6c72 0600 0000  ...sqlmodelr....
-000005d0: da0b 5f76 616c 6964 6174 6f72 7372 0800  .._validatorsr..
-000005e0: 0000 da07 5f5f 616c 6c5f 5f72 0900 0000  ....__all__r....
-000005f0: 720a 0000 0072 0b00 0000 7213 0000 0072  r....r....r....r
-00000600: 1300 0000 7213 0000 0072 1400 0000 da08  ....r....r......
-00000610: 3c6d 6f64 756c 653e 0100 0000 7314 0000  <module>....s...
-00000620: 000c 000c 010c 010c 020c 010c 0204 0210  ................
-00000630: 0710 0b14 08                             .....
+00000050: 0100 6400 6404 6c04 6d05 5a05 0100 6405  ..d.d.l.m.Z...d.
+00000060: 5a06 4700 6406 6407 8400 6407 6505 8303  Z.G.d.d...d.e...
+00000070: 5a07 4700 6408 6409 8400 6409 6507 8303  Z.G.d.d...d.e...
+00000080: 5a08 640a 5300 290b e900 0000 0029 01da  Z.d.S.)......)..
+00000090: 0864 6174 6574 696d 6529 01da 0341 6e79  .datetime)...Any
+000000a0: 2901 da08 4f70 7469 6f6e 616c 2901 da09  )...Optional)...
+000000b0: 4261 7365 4d6f 6465 6c29 02da 0a5f 5374  BaseModel)..._St
+000000c0: 6174 6542 6173 65da 0953 7461 7465 5265  ateBase..StateRe
+000000d0: 6164 6300 0000 0000 0000 0000 0000 0000  adc.............
+000000e0: 0000 0003 0000 0040 0000 0073 3200 0000  .......@...s2...
+000000f0: 6500 5a01 6400 5a02 5500 6401 5a03 6504  e.Z.d.Z.U.d.Z.e.
+00000100: 6505 6506 6602 1900 6507 6402 3c00 6508  e.e.f...e.d.<.e.
+00000110: 6507 6403 3c00 6404 6405 8400 5a09 6406  e.d.<.d.d...Z.d.
+00000120: 5300 2907 7206 0000 007a 970a 2020 2020  S.).r....z..    
+00000130: 4261 7365 2063 6c61 7373 2066 6f72 2060  Base class for `
+00000140: 5374 6174 6560 0a0a 2020 2020 4174 7472  State`..    Attr
+00000150: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
+00000160: 6964 3a20 5072 696d 6172 7920 6b65 790a  id: Primary key.
+00000170: 2020 2020 2020 2020 6461 7461 3a20 436f          data: Co
+00000180: 6e74 656e 7420 6f66 2074 6865 2073 7461  ntent of the sta
+00000190: 7465 0a20 2020 2020 2020 2074 696d 6573  te.        times
+000001a0: 7461 6d70 3a20 5469 6d65 2073 7461 6d70  tamp: Time stamp
+000001b0: 206f 6620 7468 6520 7374 6174 650a 2020   of the state.  
+000001c0: 2020 da04 6461 7461 da09 7469 6d65 7374    ..data..timest
+000001d0: 616d 7063 0100 0000 0000 0000 0000 0000  ampc............
+000001e0: 0200 0000 0300 0000 4300 0000 731a 0000  ........C...s...
+000001f0: 007c 00a0 00a1 007d 0174 017c 006a 0283  .|.....}.t.|.j..
+00000200: 017c 0164 013c 007c 0153 0029 027a 510a  .|.d.<.|.S.).zQ.
+00000210: 2020 2020 2020 2020 5265 7475 726e 2060          Return `
+00000220: 7365 6c66 2e64 6963 7428 2960 2061 6674  self.dict()` aft
+00000230: 6572 2063 6173 7469 6e67 2060 7365 6c66  er casting `self
+00000240: 2e74 696d 6573 7461 6d70 6020 746f 2061  .timestamp` to a
+00000250: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00000260: 7209 0000 0029 03da 0464 6963 74da 0373  r....)...dict..s
+00000270: 7472 7209 0000 0029 02da 0473 656c 66da  trr....)...self.
+00000280: 0164 a900 720e 0000 00fa 3d2f 686f 6d65  .d..r.....=/home
+00000290: 2f74 6f6d 6d61 736f 2f46 7261 6374 616c  /tommaso/Fractal
+000002a0: 2f66 7261 6374 616c 2f66 7261 6374 616c  /fractal/fractal
+000002b0: 2f63 6f6d 6d6f 6e2f 7363 6865 6d61 732f  /common/schemas/
+000002c0: 7374 6174 652e 7079 da0e 7361 6e69 7469  state.py..saniti
+000002d0: 7365 645f 6469 6374 1b00 0000 7306 0000  sed_dict....s...
+000002e0: 0008 040e 0104 017a 195f 5374 6174 6542  .......z._StateB
+000002f0: 6173 652e 7361 6e69 7469 7365 645f 6469  ase.sanitised_di
+00000300: 6374 4e29 0ada 085f 5f6e 616d 655f 5fda  ctN)...__name__.
+00000310: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000320: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+00000330: 5f5f 720a 0000 0072 0b00 0000 7203 0000  __r....r....r...
+00000340: 00da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  ...__annotations
+00000350: 5f5f 7202 0000 0072 1000 0000 720e 0000  __r....r....r...
+00000360: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00000370: 7206 0000 000e 0000 0073 0a00 0000 0a00  r........s......
+00000380: 0401 1009 0801 0c02 7206 0000 0063 0000  ........r....c..
+00000390: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+000003a0: 0000 4000 0000 731a 0000 0065 005a 0164  ..@...s....e.Z.d
+000003b0: 005a 0255 0065 0365 0419 0065 0564 013c  .Z.U.e.e...e.d.<
+000003c0: 0064 0253 0029 0372 0700 0000 da02 6964  .d.S.).r......id
+000003d0: 4e29 0672 1100 0000 7212 0000 0072 1300  N).r....r....r..
+000003e0: 0000 7204 0000 00da 0369 6e74 7215 0000  ..r......intr...
+000003f0: 0072 0e00 0000 720e 0000 0072 0e00 0000  .r....r....r....
+00000400: 720f 0000 0072 0700 0000 2400 0000 7304  r....r....$...s.
+00000410: 0000 000a 0010 0172 0700 0000 4e29 0972  .......r....N).r
+00000420: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
+00000430: 0072 0400 0000 da08 7079 6461 6e74 6963  .r......pydantic
+00000440: 7205 0000 00da 075f 5f61 6c6c 5f5f 7206  r......__all__r.
+00000450: 0000 0072 0700 0000 720e 0000 0072 0e00  ...r....r....r..
+00000460: 0000 720e 0000 0072 0f00 0000 da08 3c6d  ..r....r......<m
+00000470: 6f64 756c 653e 0100 0000 730e 0000 000c  odule>....s.....
+00000480: 000c 010c 010c 0204 0310 0614 16         .............
```

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc` & `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb 21 08:49:27 2023 UTC, .py size: 2817 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9785 f463 010b 0000  o..........c....
+00000000: 610d 0d0a 0000 0000 9785 f463 010b 0000  a..........c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c02 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c02 6d06 5a06 0100 6400 6406 6c02  d.l.m.Z...d.d.l.
 00000070: 6d07 5a07 0100 6400 6407 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
@@ -86,136 +86,135 @@
 00000550: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
 00000560: 2065 7865 6375 7461 626c 652c 2073 7065   executable, spe
 00000570: 6369 6669 6320 7275 6e74 696d 6520 7265  cific runtime re
 00000580: 7175 6972 656d 656e 7473 2028 652e 672e  quirements (e.g.
 00000590: 2c20 6e65 6564 5f67 7075 3d54 7275 6529  , need_gpu=True)
 000005a0: 2c0a 2020 2020 2020 2020 2020 2020 6574  ,.            et
 000005b0: 632e 0a20 2020 20da 046e 616d 65da 0a65  c..    ..name..e
-000005c0: 7865 6375 7461 626c 65da 0a69 6e70 7574  xecutable..input
+000005c0: 7865 6375 7461 626c 655a 0a69 6e70 7574  xecutableZ.input
 000005d0: 5f74 7970 65da 0b6f 7574 7075 745f 7479  _type..output_ty
 000005e0: 7065 2901 da0f 6465 6661 756c 745f 6661  pe)...default_fa
 000005f0: 6374 6f72 79da 0c64 6566 6175 6c74 5f61  ctory..default_a
 00000600: 7267 73da 046d 6574 614e 290e da08 5f5f  rgs..metaN)...__
 00000610: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
 00000620: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
 00000630: da07 5f5f 646f 635f 5fda 0373 7472 da0f  ..__doc__..str..
 00000640: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
 00000650: 0200 0000 720a 0000 00da 0464 6963 7472  ....r......dictr
-00000660: 1300 0000 7206 0000 0072 0400 0000 7203  ....r....r....r.
-00000670: 0000 0072 1400 0000 a900 721c 0000 0072  ...r......r....r
-00000680: 1c00 0000 fa40 2f68 6f6d 652f 746f 6d6d  .....@/home/tomm
+00000660: 1200 0000 7206 0000 0072 0400 0000 7203  ....r....r....r.
+00000670: 0000 0072 1300 0000 a900 721b 0000 0072  ...r......r....r
+00000680: 1b00 0000 fa40 2f68 6f6d 652f 746f 6d6d  .....@/home/tomm
 00000690: 6173 6f2f 4672 6163 7461 6c2f 6672 6163  aso/Fractal/frac
 000006a0: 7461 6c2f 6672 6163 7461 6c2f 636f 6d6d  tal/fractal/comm
 000006b0: 6f6e 2f73 6368 656d 6173 2f6d 616e 6966  on/schemas/manif
 000006c0: 6573 742e 7079 720d 0000 0010 0000 0073  est.pyr........s
-000006d0: 1000 0000 0a00 0401 081c 0801 0801 0801  ................
-000006e0: 1e01 2201 720d 0000 00da 1054 6173 6b4d  ..".r......TaskM
-000006f0: 616e 6966 6573 7454 7970 6529 01da 0562  anifestType)...b
-00000700: 6f75 6e64 6300 0000 0000 0000 0000 0000  oundc...........
-00000710: 0000 0000 0003 0000 0040 0000 0073 2600  .........@...s&.
-00000720: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-00000730: 6504 6505 6402 3c00 6506 6507 1900 6505  e.e.d.<.e.e...e.
-00000740: 6403 3c00 6404 5300 2905 da0d 5f4d 616e  d.<.d.S.)..._Man
-00000750: 6966 6573 7442 6173 6561 2803 0000 0a20  ifestBasea(.... 
-00000760: 2020 204d 616e 6966 6573 7420 6261 7365     Manifest base
-00000770: 2063 6c61 7373 0a0a 2020 2020 5061 636b   class..    Pack
-00000780: 6167 6573 2063 6f6e 7461 696e 696e 6720  ages containing 
-00000790: 7461 736b 7320 6172 6520 7265 7175 6972  tasks are requir
-000007a0: 6564 2074 6f20 696e 636c 7564 6520 6120  ed to include a 
-000007b0: 7370 6563 6961 6c20 6669 6c65 0a20 2020  special file.   
-000007c0: 2060 5f5f 4652 4143 5441 4c5f 4d41 4e49   `__FRACTAL_MANI
-000007d0: 4645 5354 5f5f 2e6a 736f 6e60 2069 6e20  FEST__.json` in 
-000007e0: 6f72 6465 7220 746f 2062 6520 6469 7363  order to be disc
-000007f0: 6f76 6572 6564 2061 6e64 2075 7365 6420  overed and used 
-00000800: 6279 2046 7261 6374 616c 2e0a 0a20 2020  by Fractal...   
-00000810: 2054 6869 7320 6d6f 6465 6c20 636c 6173   This model clas
-00000820: 7320 616e 6420 7468 6520 6d6f 6465 6c20  s and the model 
-00000830: 636c 6173 7365 7320 6974 2064 6570 656e  classes it depen
-00000840: 6473 206f 6e20 7072 6f76 6964 6520 7468  ds on provide th
-00000850: 6520 6261 7365 0a20 2020 2073 6368 656d  e base.    schem
-00000860: 6120 746f 2072 6561 642c 2077 7269 7465  a to read, write
-00000870: 2061 6e64 2076 616c 6964 6174 6520 6d61   and validate ma
-00000880: 6e69 6665 7374 732e 0a0a 2020 2020 4174  nifests...    At
-00000890: 7472 6962 7574 6573 3a0a 2020 2020 2020  tributes:.      
-000008a0: 2020 6d61 6e69 6665 7374 5f76 6572 7369    manifest_versi
-000008b0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-000008c0: 4120 7665 7273 696f 6e20 7374 7269 6e67  A version string
-000008d0: 2074 6861 7420 7072 6f76 6964 6573 2069   that provides i
-000008e0: 6e64 6963 6174 696f 6e20 666f 7220 636f  ndication for co
-000008f0: 6d70 6174 6962 696c 6974 7920 6265 7477  mpatibility betw
-00000900: 6565 6e0a 2020 2020 2020 2020 2020 2020  een.            
-00000910: 6d61 6e69 6665 7374 7320 6173 2074 6865  manifests as the
-00000920: 2073 6368 656d 6120 6576 6f6c 7665 732e   schema evolves.
-00000930: 2054 6869 7320 6973 2066 6f72 2069 6e73   This is for ins
-00000940: 7461 6e63 6520 7573 6564 2062 790a 2020  tance used by.  
-00000950: 2020 2020 2020 2020 2020 4672 6163 7461            Fracta
-00000960: 6c20 746f 2064 6574 6572 6d69 6e65 2077  l to determine w
-00000970: 6869 6368 2073 7562 636c 6173 7320 6f66  hich subclass of
-00000980: 2074 6865 2070 7265 7365 6e74 2062 6173   the present bas
-00000990: 6520 636c 6173 7320 6e65 6564 730a 2020  e class needs.  
-000009a0: 2020 2020 2020 2020 2020 6265 2075 7365            be use
-000009b0: 6420 746f 2072 6561 6420 616e 6420 7661  d to read and va
-000009c0: 6c69 6461 7465 2074 6865 2069 6e70 7574  lidate the input
-000009d0: 2e0a 2020 2020 2020 2020 7461 736b 5f6c  ..        task_l
-000009e0: 6973 7420 3a20 4c69 7374 5b54 6173 6b4d  ist : List[TaskM
-000009f0: 616e 6966 6573 7454 7970 655d 0a20 2020  anifestType].   
-00000a00: 2020 2020 2020 2020 2054 6865 206c 6973           The lis
-00000a10: 7420 6f66 2074 6173 6b73 2c20 7265 7072  t of tasks, repr
-00000a20: 6573 656e 7465 6420 6173 2073 7065 6369  esented as speci
-00000a30: 6669 6564 2062 7920 7375 6263 6c61 7373  fied by subclass
-00000a40: 6573 206f 6620 7468 650a 2020 2020 2020  es of the.      
-00000a50: 2020 2020 2020 5f54 6173 6b4d 616e 6966        _TaskManif
-00000a60: 6573 7442 6173 6520 2861 2e6b 2e61 2e20  estBase (a.k.a. 
-00000a70: 5461 736b 4d61 6e69 6665 7374 5479 7065  TaskManifestType
-00000a80: 290a 2020 2020 da10 6d61 6e69 6665 7374  ).    ..manifest
-00000a90: 5f76 6572 7369 6f6e da09 7461 736b 5f6c  _version..task_l
-00000aa0: 6973 744e 2908 7215 0000 0072 1600 0000  istN).r....r....
-00000ab0: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-00000ac0: 1a00 0000 7205 0000 0072 1e00 0000 721c  ....r....r....r.
-00000ad0: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
-00000ae0: 0000 7220 0000 0038 0000 0073 0800 0000  ..r ...8...s....
-00000af0: 0a00 0401 0814 1001 7220 0000 0063 0000  ........r ...c..
-00000b00: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-00000b10: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
-00000b20: 005a 0264 0153 0029 0272 0b00 0000 4e29  .Z.d.S.).r....N)
-00000b30: 0372 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000b40: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
-00000b50: 1d00 0000 720b 0000 0051 0000 0073 0400  ....r....Q...s..
-00000b60: 0000 0800 0401 720b 0000 0063 0000 0000  ......r....c....
-00000b70: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000b80: 4000 0000 732e 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00000b90: 0255 0064 015a 0365 0465 0519 0065 0664  .U.d.Z.e.e...e.d
-00000ba0: 023c 0065 0764 0383 0164 0464 0584 0083  .<.e.d...d.d....
-00000bb0: 015a 0864 0653 0029 0772 0c00 0000 7a23  .Z.d.S.).r....z#
-00000bc0: 0a20 2020 204d 616e 6966 6573 7420 7363  .    Manifest sc
-00000bd0: 6865 6d61 2076 6572 7369 6f6e 2031 0a20  hema version 1. 
-00000be0: 2020 2072 2200 0000 7221 0000 0063 0200     r"...r!...c..
-00000bf0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00000c00: 0000 4300 0000 7314 0000 007c 0164 016b  ..C...s....|.d.k
-00000c10: 0372 0874 0064 0283 0182 0164 0053 0029  .r.t.d.....d.S.)
-00000c20: 034e da01 317a 1657 726f 6e67 206d 616e  .N..1z.Wrong man
-00000c30: 6966 6573 7420 7665 7273 696f 6e29 01da  ifest version)..
-00000c40: 0a56 616c 7565 4572 726f 7229 02da 0363  .ValueError)...c
-00000c50: 6c73 da05 7661 6c75 6572 1c00 0000 721c  ls..valuer....r.
-00000c60: 0000 0072 1d00 0000 da12 6d61 6e69 6665  ...r......manife
-00000c70: 7374 5f76 6572 7369 6f6e 5f31 5c00 0000  st_version_1\...
-00000c80: 7306 0000 0008 0208 0104 ff7a 1d4d 616e  s..........z.Man
-00000c90: 6966 6573 7456 312e 6d61 6e69 6665 7374  ifestV1.manifest
-00000ca0: 5f76 6572 7369 6f6e 5f31 4e29 0972 1500  _version_1N).r..
-00000cb0: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00000cc0: 0072 0500 0000 720b 0000 0072 1a00 0000  .r....r....r....
-00000cd0: 7209 0000 0072 2700 0000 721c 0000 0072  r....r'...r....r
-00000ce0: 1c00 0000 721c 0000 0072 1d00 0000 720c  ....r....r....r.
-00000cf0: 0000 0055 0000 0073 0a00 0000 0a00 0401  ...U...s........
-00000d00: 0c04 0602 0e01 720c 0000 004e 2913 da07  ......r....N)...
-00000d10: 7061 7468 6c69 6272 0200 0000 da06 7479  pathlibr......ty
-00000d20: 7069 6e67 7203 0000 0072 0400 0000 7205  pingr....r....r.
-00000d30: 0000 0072 0600 0000 7207 0000 00da 0870  ...r....r......p
-00000d40: 7964 616e 7469 6372 0800 0000 7209 0000  ydanticr....r...
-00000d50: 00da 0873 716c 6d6f 6465 6c72 0a00 0000  ...sqlmodelr....
-00000d60: da07 5f5f 616c 6c5f 5f72 0d00 0000 721e  ..__all__r....r.
-00000d70: 0000 0072 2000 0000 720b 0000 0072 0c00  ...r ...r....r..
-00000d80: 0000 721c 0000 0072 1c00 0000 721c 0000  ..r....r....r...
-00000d90: 0072 1d00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000da0: 0100 0000 731e 0000 000c 000c 010c 010c  ....s...........
-00000db0: 010c 010c 010c 020c 010c 0104 0310 030c  ................
-00000dc0: 2510 0310 1914 04                        %......
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

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc` & `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Feb 21 08:49:27 2023 UTC, .py size: 2817 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,220 +1,217 @@
-00000000: 610d 0d0a 0000 0000 9785 f463 010b 0000  a..........c....
+00000000: 6f0d 0d0a 0000 0000 3d55 6f64 d10a 0000  o.......=Uod....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c02 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
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
+00000060: 6405 6c06 6d07 5a07 0100 6400 6406 6c06  d.l.m.Z...d.d.l.
+00000070: 6d08 5a08 0100 6400 6407 6c06 6d09 5a09  m.Z...d.d.l.m.Z.
+00000080: 0100 6408 5a0a 4700 6409 640a 8400 640a  ..d.Z.G.d.d...d.
+00000090: 6507 8303 5a0b 6505 640b 650b 640c 8d02  e...Z.e.d.e.d...
+000000a0: 5a0c 4700 640d 640e 8400 640e 6507 8303  Z.G.d.d...d.e...
+000000b0: 5a0d 4700 640f 6410 8400 6410 650b 8303  Z.G.d.d...d.e...
+000000c0: 5a0e 4700 6411 6412 8400 6412 650d 8303  Z.G.d.d...d.e...
+000000d0: 5a0f 6413 5300 2914 e900 0000 0029 01da  Z.d.S.)......)..
+000000e0: 0450 6174 6829 01da 0341 6e79 2901 da08  .Path)...Any)...
+000000f0: 4f70 7469 6f6e 616c 2901 da07 5479 7065  Optional)...Type
+00000100: 5661 7229 01da 0942 6173 654d 6f64 656c  Var)...BaseModel
+00000110: 2901 da05 4669 656c 6429 01da 0976 616c  )...Field)...val
+00000120: 6964 6174 6f72 2902 da0e 5461 736b 4d61  idator)...TaskMa
+00000130: 6e69 6665 7374 5631 da0a 4d61 6e69 6665  nifestV1..Manife
+00000140: 7374 5631 6300 0000 0000 0000 0000 0000  stV1c...........
+00000150: 0000 0000 0004 0000 0040 0000 0073 6e00  .........@...sn.
+00000160: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
+00000170: 6504 6505 6402 3c00 6506 6505 6403 3c00  e.e.d.<.e.e.d.<.
+00000180: 6504 6505 6404 3c00 6504 6505 6405 3c00  e.e.d.<.e.e.d.<.
+00000190: 6507 6508 6406 8d01 5a09 650a 6508 6504  e.e.d...Z.e.e.e.
+000001a0: 650b 6602 1900 1900 6505 6407 3c00 6507  e.f.....e.d.<.e.
+000001b0: 6508 6406 8d01 5a0c 650a 6508 6504 650b  e.d...Z.e.e.e.e.
+000001c0: 6602 1900 1900 6505 6408 3c00 6409 5300  f.....e.d.<.d.S.
+000001d0: 290a da11 5f54 6173 6b4d 616e 6966 6573  )..._TaskManifes
+000001e0: 7442 6173 6561 a503 0000 0a20 2020 2042  tBasea.....    B
+000001f0: 6173 6520 636c 6173 7320 666f 7220 5461  ase class for Ta
+00000200: 736b 4d61 6e69 6665 7374 0a0a 2020 2020  skManifest..    
+00000210: 5265 7072 6573 656e 7473 2061 2074 6173  Represents a tas
+00000220: 6b20 7769 7468 696e 2061 206d 616e 6665  k within a manfe
+00000230: 7374 0a0a 2020 2020 4174 7472 6962 7574  st..    Attribut
+00000240: 6573 3a0a 2020 2020 2020 2020 6e61 6d65  es:.        name
+00000250: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00000260: 6520 7461 736b 206e 616d 650a 2020 2020  e task name.    
+00000270: 2020 2020 6578 6563 7574 6162 6c65 3a0a      executable:.
+00000280: 2020 2020 2020 2020 2020 2020 5061 7468              Path
+00000290: 2074 6f20 7468 6520 6578 6563 7574 6162   to the executab
+000002a0: 6c65 2072 656c 6174 6976 6520 746f 2074  le relative to t
+000002b0: 6865 2070 6163 6b61 6765 2072 6f6f 740a  he package root.
+000002c0: 0a20 2020 2020 2020 2020 2020 204e 6f74  .            Not
+000002d0: 653a 2062 7920 7061 636b 6167 6520 726f  e: by package ro
+000002e0: 6f74 2077 6520 6d65 616e 2022 6173 2069  ot we mean "as i
+000002f0: 7420 7769 6c6c 2062 6520 696e 7374 616c  t will be instal
+00000300: 6c65 6422 2e20 4966 2061 0a20 2020 2020  led". If a.     
+00000310: 2020 2020 2020 2070 6163 6b61 6765 2060         package `
+00000320: 506b 6760 2069 6e73 7461 6c6c 7320 696e  Pkg` installs in
+00000330: 2074 6865 2066 6f6c 6465 7220 6070 6b67   the folder `pkg
+00000340: 6020 7468 6520 6578 6563 7574 6162 6c65  ` the executable
+00000350: 0a20 2020 2020 2020 2020 2020 2060 706b  .            `pk
+00000360: 672f 6578 6563 7574 6162 6c65 2e70 7960  g/executable.py`
+00000370: 2c20 7468 6973 2061 7474 7269 6275 7465  , this attribute
+00000380: 206d 7573 7420 636f 6e74 6169 6e20 6f6e   must contain on
+00000390: 6c79 0a20 2020 2020 2020 2020 2020 2060  ly.            `
+000003a0: 6578 6563 7574 6162 6c65 2e70 7960 2e0a  executable.py`..
+000003b0: 2020 2020 2020 2020 696e 7075 745f 7479          input_ty
+000003c0: 7065 3a0a 2020 2020 2020 2020 2020 2020  pe:.            
+000003d0: 5468 6520 696e 7075 7420 7479 7065 2061  The input type a
+000003e0: 6363 6570 7465 6420 6279 2074 6865 2074  ccepted by the t
+000003f0: 6173 6b0a 2020 2020 2020 2020 6f75 7470  ask.        outp
+00000400: 7574 5f74 7970 653a 0a20 2020 2020 2020  ut_type:.       
+00000410: 2020 2020 2054 6865 206f 7574 7075 7420       The output 
+00000420: 7479 7065 2072 6574 7572 6e65 6420 6279  type returned by
+00000430: 2074 6865 2074 6173 6b0a 2020 2020 2020   the task.      
+00000440: 2020 6465 6661 756c 745f 6172 6773 3a0a    default_args:.
+00000450: 2020 2020 2020 2020 2020 2020 416e 2061              An a
+00000460: 7262 6974 7261 7279 2c20 4a53 4f4e 2d73  rbitrary, JSON-s
+00000470: 6572 6961 6c69 7a61 626c 6520 6469 6374  erializable dict
+00000480: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
+00000490: 6720 7468 6520 6465 6661 756c 740a 2020  g the default.  
+000004a0: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
+000004b0: 7465 7273 2074 6861 7420 7769 6c6c 2062  ters that will b
+000004c0: 6520 7061 7373 6564 2074 6f20 7468 6520  e passed to the 
+000004d0: 7461 736b 0a20 2020 2020 2020 206d 6574  task.        met
+000004e0: 613a 0a20 2020 2020 2020 2020 2020 2041  a:.            A
+000004f0: 6464 6974 696f 6e61 6c20 696e 666f 726d  dditional inform
+00000500: 6174 696f 6e20 6162 6f75 7420 7468 6520  ation about the 
+00000510: 7061 636b 6167 652c 2073 7563 6820 6173  package, such as
+00000520: 2068 6173 6820 6f66 2074 6865 0a20 2020   hash of the.   
+00000530: 2020 2020 2020 2020 2065 7865 6375 7461           executa
+00000540: 626c 652c 2073 7065 6369 6669 6320 7275  ble, specific ru
+00000550: 6e74 696d 6520 7265 7175 6972 656d 656e  ntime requiremen
+00000560: 7473 2028 652e 672e 2c20 6e65 6564 5f67  ts (e.g., need_g
+00000570: 7075 3d54 7275 6529 2c0a 2020 2020 2020  pu=True),.      
+00000580: 2020 2020 2020 6574 632e 0a20 2020 20da        etc..    .
+00000590: 046e 616d 65da 0a65 7865 6375 7461 626c  .name..executabl
+000005a0: 65da 0a69 6e70 7574 5f74 7970 65da 0b6f  e..input_type..o
+000005b0: 7574 7075 745f 7479 7065 2901 da0f 6465  utput_type)...de
+000005c0: 6661 756c 745f 6661 6374 6f72 79da 0c64  fault_factory..d
+000005d0: 6566 6175 6c74 5f61 7267 73da 046d 6574  efault_args..met
+000005e0: 614e 290d da08 5f5f 6e61 6d65 5f5f da0a  aN)...__name__..
+000005f0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000600: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+00000610: 5fda 0373 7472 da0f 5f5f 616e 6e6f 7461  _..str..__annota
+00000620: 7469 6f6e 735f 5f72 0200 0000 7207 0000  tions__r....r...
+00000630: 00da 0464 6963 7472 1100 0000 7204 0000  ...dictr....r...
+00000640: 0072 0300 0000 7212 0000 00a9 0072 1a00  .r....r......r..
+00000650: 0000 721a 0000 00fa 402f 686f 6d65 2f74  ..r.....@/home/t
+00000660: 6f6d 6d61 736f 2f46 7261 6374 616c 2f66  ommaso/Fractal/f
+00000670: 7261 6374 616c 2f66 7261 6374 616c 2f63  ractal/fractal/c
+00000680: 6f6d 6d6f 6e2f 7363 6865 6d61 732f 6d61  ommon/schemas/ma
+00000690: 6e69 6665 7374 2e70 7972 0b00 0000 0e00  nifest.pyr......
+000006a0: 0000 7310 0000 000a 0004 0108 1c08 0108  ..s.............
+000006b0: 0108 011e 0122 0172 0b00 0000 da10 5461  .....".r......Ta
+000006c0: 736b 4d61 6e69 6665 7374 5479 7065 2901  skManifestType).
+000006d0: da05 626f 756e 6463 0000 0000 0000 0000  ..boundc........
+000006e0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+000006f0: 7326 0000 0065 005a 0164 005a 0255 0064  s&...e.Z.d.Z.U.d
+00000700: 015a 0365 0465 0564 023c 0065 0665 0719  .Z.e.e.d.<.e.e..
+00000710: 0065 0564 033c 0064 0453 0029 05da 0d5f  .e.d.<.d.S.)..._
+00000720: 4d61 6e69 6665 7374 4261 7365 6128 0300  ManifestBasea(..
+00000730: 000a 2020 2020 4d61 6e69 6665 7374 2062  ..    Manifest b
+00000740: 6173 6520 636c 6173 730a 0a20 2020 2050  ase class..    P
+00000750: 6163 6b61 6765 7320 636f 6e74 6169 6e69  ackages containi
+00000760: 6e67 2074 6173 6b73 2061 7265 2072 6571  ng tasks are req
+00000770: 7569 7265 6420 746f 2069 6e63 6c75 6465  uired to include
+00000780: 2061 2073 7065 6369 616c 2066 696c 650a   a special file.
+00000790: 2020 2020 605f 5f46 5241 4354 414c 5f4d      `__FRACTAL_M
+000007a0: 414e 4946 4553 545f 5f2e 6a73 6f6e 6020  ANIFEST__.json` 
+000007b0: 696e 206f 7264 6572 2074 6f20 6265 2064  in order to be d
+000007c0: 6973 636f 7665 7265 6420 616e 6420 7573  iscovered and us
+000007d0: 6564 2062 7920 4672 6163 7461 6c2e 0a0a  ed by Fractal...
+000007e0: 2020 2020 5468 6973 206d 6f64 656c 2063      This model c
+000007f0: 6c61 7373 2061 6e64 2074 6865 206d 6f64  lass and the mod
+00000800: 656c 2063 6c61 7373 6573 2069 7420 6465  el classes it de
+00000810: 7065 6e64 7320 6f6e 2070 726f 7669 6465  pends on provide
+00000820: 2074 6865 2062 6173 650a 2020 2020 7363   the base.    sc
+00000830: 6865 6d61 2074 6f20 7265 6164 2c20 7772  hema to read, wr
+00000840: 6974 6520 616e 6420 7661 6c69 6461 7465  ite and validate
+00000850: 206d 616e 6966 6573 7473 2e0a 0a20 2020   manifests...   
+00000860: 2041 7474 7269 6275 7465 733a 0a20 2020   Attributes:.   
+00000870: 2020 2020 206d 616e 6966 6573 745f 7665       manifest_ve
+00000880: 7273 696f 6e3a 0a20 2020 2020 2020 2020  rsion:.         
+00000890: 2020 2041 2076 6572 7369 6f6e 2073 7472     A version str
+000008a0: 696e 6720 7468 6174 2070 726f 7669 6465  ing that provide
+000008b0: 7320 696e 6469 6361 7469 6f6e 2066 6f72  s indication for
+000008c0: 2063 6f6d 7061 7469 6269 6c69 7479 2062   compatibility b
+000008d0: 6574 7765 656e 0a20 2020 2020 2020 2020  etween.         
+000008e0: 2020 206d 616e 6966 6573 7473 2061 7320     manifests as 
+000008f0: 7468 6520 7363 6865 6d61 2065 766f 6c76  the schema evolv
+00000900: 6573 2e20 5468 6973 2069 7320 666f 7220  es. This is for 
+00000910: 696e 7374 616e 6365 2075 7365 6420 6279  instance used by
+00000920: 0a20 2020 2020 2020 2020 2020 2046 7261  .            Fra
+00000930: 6374 616c 2074 6f20 6465 7465 726d 696e  ctal to determin
+00000940: 6520 7768 6963 6820 7375 6263 6c61 7373  e which subclass
+00000950: 206f 6620 7468 6520 7072 6573 656e 7420   of the present 
+00000960: 6261 7365 2063 6c61 7373 206e 6565 6473  base class needs
+00000970: 0a20 2020 2020 2020 2020 2020 2062 6520  .            be 
+00000980: 7573 6564 2074 6f20 7265 6164 2061 6e64  used to read and
+00000990: 2076 616c 6964 6174 6520 7468 6520 696e   validate the in
+000009a0: 7075 742e 0a20 2020 2020 2020 2074 6173  put..        tas
+000009b0: 6b5f 6c69 7374 203a 206c 6973 745b 5461  k_list : list[Ta
+000009c0: 736b 4d61 6e69 6665 7374 5479 7065 5d0a  skManifestType].
+000009d0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+000009e0: 6c69 7374 206f 6620 7461 736b 732c 2072  list of tasks, r
+000009f0: 6570 7265 7365 6e74 6564 2061 7320 7370  epresented as sp
+00000a00: 6563 6966 6965 6420 6279 2073 7562 636c  ecified by subcl
+00000a10: 6173 7365 7320 6f66 2074 6865 0a20 2020  asses of the.   
+00000a20: 2020 2020 2020 2020 205f 5461 736b 4d61           _TaskMa
+00000a30: 6e69 6665 7374 4261 7365 2028 612e 6b2e  nifestBase (a.k.
+00000a40: 612e 2054 6173 6b4d 616e 6966 6573 7454  a. TaskManifestT
+00000a50: 7970 6529 0a20 2020 20da 106d 616e 6966  ype).    ..manif
+00000a60: 6573 745f 7665 7273 696f 6eda 0974 6173  est_version..tas
+00000a70: 6b5f 6c69 7374 4e29 0872 1300 0000 7214  k_listN).r....r.
+00000a80: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
+00000a90: 0000 7218 0000 00da 046c 6973 7472 1c00  ..r......listr..
+00000aa0: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+00000ab0: 0072 1b00 0000 721e 0000 0036 0000 0073  .r....r....6...s
+00000ac0: 0800 0000 0a00 0401 0814 1001 721e 0000  ............r...
+00000ad0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000ae0: 0000 0100 0000 4000 0000 730c 0000 0065  ......@...s....e
+00000af0: 005a 0164 005a 0264 0153 0029 0272 0900  .Z.d.Z.d.S.).r..
+00000b00: 0000 4e29 0372 1300 0000 7214 0000 0072  ..N).r....r....r
+00000b10: 1500 0000 721a 0000 0072 1a00 0000 721a  ....r....r....r.
+00000b20: 0000 0072 1b00 0000 7209 0000 004f 0000  ...r....r....O..
+00000b30: 0073 0400 0000 0800 0401 7209 0000 0063  .s........r....c
+00000b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b50: 0300 0000 4000 0000 732e 0000 0065 005a  ....@...s....e.Z
+00000b60: 0164 005a 0255 0064 015a 0365 0465 0519  .d.Z.U.d.Z.e.e..
+00000b70: 0065 0664 023c 0065 0764 0383 0164 0464  .e.d.<.e.d...d.d
+00000b80: 0584 0083 015a 0864 0653 0029 0772 0a00  .....Z.d.S.).r..
+00000b90: 0000 7a23 0a20 2020 204d 616e 6966 6573  ..z#.    Manifes
+00000ba0: 7420 7363 6865 6d61 2076 6572 7369 6f6e  t schema version
+00000bb0: 2031 0a20 2020 2072 2000 0000 721f 0000   1.    r ...r...
+00000bc0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+00000bd0: 0000 0200 0000 4300 0000 7314 0000 007c  ......C...s....|
+00000be0: 0164 016b 0372 0874 0064 0283 0182 0164  .d.k.r.t.d.....d
+00000bf0: 0053 0029 034e da01 317a 1657 726f 6e67  .S.).N..1z.Wrong
+00000c00: 206d 616e 6966 6573 7420 7665 7273 696f   manifest versio
+00000c10: 6e29 01da 0a56 616c 7565 4572 726f 7229  n)...ValueError)
+00000c20: 02da 0363 6c73 da05 7661 6c75 6572 1a00  ...cls..valuer..
+00000c30: 0000 721a 0000 0072 1b00 0000 da12 6d61  ..r....r......ma
+00000c40: 6e69 6665 7374 5f76 6572 7369 6f6e 5f31  nifest_version_1
+00000c50: 5a00 0000 7306 0000 0008 0208 0104 ff7a  Z...s..........z
+00000c60: 1d4d 616e 6966 6573 7456 312e 6d61 6e69  .ManifestV1.mani
+00000c70: 6665 7374 5f76 6572 7369 6f6e 5f31 4e29  fest_version_1N)
+00000c80: 0972 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000c90: 7216 0000 0072 2100 0000 7209 0000 0072  r....r!...r....r
+00000ca0: 1800 0000 7208 0000 0072 2600 0000 721a  ....r....r&...r.
+00000cb0: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
+00000cc0: 0000 720a 0000 0053 0000 0073 0a00 0000  ..r....S...s....
+00000cd0: 0a00 0401 0c04 0602 0e01 720a 0000 004e  ..........r....N
+00000ce0: 2910 da07 7061 7468 6c69 6272 0200 0000  )...pathlibr....
+00000cf0: da06 7479 7069 6e67 7203 0000 0072 0400  ..typingr....r..
+00000d00: 0000 7205 0000 00da 0870 7964 616e 7469  ..r......pydanti
+00000d10: 6372 0600 0000 7207 0000 0072 0800 0000  cr....r....r....
+00000d20: da07 5f5f 616c 6c5f 5f72 0b00 0000 721c  ..__all__r....r.
+00000d30: 0000 0072 1e00 0000 7209 0000 0072 0a00  ...r....r....r..
+00000d40: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+00000d50: 0072 1b00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000d60: 0100 0000 731a 0000 000c 000c 010c 010c  ....s...........
+00000d70: 010c 020c 010c 0104 0310 030c 2510 0310  ............%...
+00000d80: 1914 04                                  ...
```

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/project.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr  6 11:30:39 2023 UTC, .py size: 2527 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,225 +1,232 @@
-00000000: 6f0d 0d0a 0000 0000 5fad 2e64 df09 0000  o......._..d....
+00000000: 610d 0d0a 0000 0000 65b3 1164 b10a 0000  a.......e..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3401 0000 6400  .....@...s4...d.
+00000020: 0004 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c05 6d06 5a06 0100 6400 6406 6c05  d.l.m.Z...d.d.l.
 00000070: 6d07 5a07 0100 6400 6407 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000080: 0100 6408 6409 6c0a 6d0b 5a0b 0100 6408  ..d.d.l.m.Z...d.
-00000090: 640a 6c0a 6d0c 5a0c 0100 640b 5a0d 4700  d.l.m.Z...d.Z.G.
-000000a0: 640c 640d 8400 640d 6509 8303 5a0e 4700  d.d...d.e...Z.G.
-000000b0: 640e 640f 8400 640f 650e 8303 5a0f 4700  d.d...d.e...Z.G.
-000000c0: 6410 6411 8400 6411 650e 8303 5a10 4700  d.d...d.e...Z.G.
-000000d0: 6412 6413 8400 6413 650e 8303 5a11 4700  d.d...d.e...Z.G.
-000000e0: 6414 6415 8400 6415 6509 8303 5a12 4700  d.d...d.e...Z.G.
-000000f0: 6416 6417 8400 6417 6512 8303 5a13 4700  d.d...d.e...Z.G.
-00000100: 6418 6419 8400 6419 6512 8303 5a14 4700  d.d...d.e...Z.G.
-00000110: 641a 641b 8400 641b 6512 8303 5a15 4700  d.d...d.e...Z.G.
-00000120: 641c 641d 8400 641d 6509 8303 5a16 4700  d.d...d.e...Z.G.
-00000130: 641e 641f 8400 641f 6516 8303 5a17 4700  d.d...d.e...Z.G.
-00000140: 6420 6421 8400 6421 6516 8303 5a18 4700  d d!..d!e...Z.G.
-00000150: 6422 6423 8400 6423 6516 8303 5a19 6424  d"d#..d#e...Z.d$
-00000160: 5300 2925 e900 0000 0029 01da 0341 6e79  S.)%.....)...Any
-00000170: 2901 da04 4469 6374 2901 da04 4c69 7374  )...Dict)...List
-00000180: 2901 da08 4f70 7469 6f6e 616c 2901 da05  )...Optional)...
-00000190: 4669 656c 6429 01da 0976 616c 6964 6174  Field)...validat
-000001a0: 6f72 2901 da08 5351 4c4d 6f64 656c e901  or)...SQLModel..
-000001b0: 0000 0029 01da 1176 616c 5f61 6273 6f6c  ...)...val_absol
-000001c0: 7574 655f 7061 7468 2901 da06 7661 6c73  ute_path)...vals
-000001d0: 7472 2909 da0d 5072 6f6a 6563 7443 7265  tr)...ProjectCre
-000001e0: 6174 65da 0b50 726f 6a65 6374 5265 6164  ate..ProjectRead
-000001f0: da0d 5072 6f6a 6563 7455 7064 6174 65da  ..ProjectUpdate.
-00000200: 0d44 6174 6173 6574 5570 6461 7465 da0d  .DatasetUpdate..
-00000210: 4461 7461 7365 7443 7265 6174 65da 0b44  DatasetCreate..D
-00000220: 6174 6173 6574 5265 6164 da0e 5265 736f  atasetRead..Reso
-00000230: 7572 6365 4372 6561 7465 da0c 5265 736f  urceCreate..Reso
-00000240: 7572 6365 5265 6164 da0e 5265 736f 7572  urceRead..Resour
-00000250: 6365 5570 6461 7465 6300 0000 0000 0000  ceUpdatec.......
-00000260: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000270: 0073 1a00 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
-00000280: 6401 5a03 6504 6505 6402 3c00 6403 5300  d.Z.e.e.d.<.d.S.
-00000290: 2904 da0d 5f52 6573 6f75 7263 6542 6173  )..._ResourceBas
-000002a0: 657a 210a 2020 2020 4261 7365 2063 6c61  ez!.    Base cla
-000002b0: 7373 2066 6f72 2052 6573 6f75 7263 650a  ss for Resource.
-000002c0: 2020 2020 da04 7061 7468 4e29 06da 085f      ..pathN)..._
-000002d0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-000002e0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000002f0: 5fda 075f 5f64 6f63 5f5f da03 7374 72da  _..__doc__..str.
-00000300: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
-00000310: a900 721d 0000 0072 1d00 0000 fa3f 2f68  ..r....r.....?/h
-00000320: 6f6d 652f 746f 6d6d 6173 6f2f 4672 6163  ome/tommaso/Frac
-00000330: 7461 6c2f 6672 6163 7461 6c2f 6672 6163  tal/fractal/frac
-00000340: 7461 6c2f 636f 6d6d 6f6e 2f73 6368 656d  tal/common/schem
-00000350: 6173 2f70 726f 6a65 6374 2e70 7972 1500  as/project.pyr..
-00000360: 0000 1e00 0000 7306 0000 000a 0004 010c  ......s.........
-00000370: 0472 1500 0000 6300 0000 0000 0000 0000  .r....c.........
-00000380: 0000 0000 0000 0004 0000 0040 0000 00f3  ...........@....
-00000390: 2000 0000 6500 5a01 6400 5a02 6503 6401   ...e.Z.d.Z.e.d.
-000003a0: 6402 6403 8d02 6504 6401 8301 8301 5a05  d.d...e.d.....Z.
-000003b0: 6404 5300 2905 7212 0000 0072 1600 0000  d.S.).r....r....
-000003c0: 54a9 01da 0b61 6c6c 6f77 5f72 6575 7365  T....allow_reuse
-000003d0: 4ea9 0672 1700 0000 7218 0000 0072 1900  N..r....r....r..
-000003e0: 0000 7207 0000 0072 0a00 0000 da05 5f70  ..r....r......_p
-000003f0: 6174 6872 1d00 0000 721d 0000 0072 1d00  athr....r....r..
-00000400: 0000 721e 0000 0072 1200 0000 2600 0000  ..r....r....&...
-00000410: f304 0000 0008 0018 0272 1200 0000 6300  .........r....c.
-00000420: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00000430: 0000 0040 0000 0072 1f00 0000 2905 7214  ...@...r....).r.
-00000440: 0000 0072 1600 0000 5472 2000 0000 4e72  ...r....Tr ...Nr
-00000450: 2200 0000 721d 0000 0072 1d00 0000 721d  "...r....r....r.
-00000460: 0000 0072 1e00 0000 7214 0000 002b 0000  ...r....r....+..
-00000470: 0072 2400 0000 7214 0000 0063 0000 0000  .r$...r....c....
-00000480: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000490: 4000 0000 731e 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-000004a0: 0255 0065 0365 0464 013c 0065 0365 0464  .U.e.e.d.<.e.e.d
-000004b0: 023c 0064 0353 0029 0472 1300 0000 da02  .<.d.S.).r......
-000004c0: 6964 da0a 6461 7461 7365 745f 6964 4e29  id..dataset_idN)
-000004d0: 0572 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
-000004e0: da03 696e 7472 1c00 0000 721d 0000 0072  ..intr....r....r
-000004f0: 1d00 0000 721d 0000 0072 1e00 0000 7213  ....r....r....r.
-00000500: 0000 0030 0000 0073 0600 0000 0a00 0801  ...0...s........
-00000510: 0c01 7213 0000 0063 0000 0000 0000 0000  ..r....c........
-00000520: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000530: 734c 0000 0065 005a 0164 005a 0255 0064  sL...e.Z.d.Z.U.d
-00000540: 015a 0365 0465 0564 023c 0065 0665 0419  .Z.e.e.d.<.e.e..
-00000550: 0065 0564 033c 0065 0769 0064 048d 015a  .e.d.<.e.i.d...Z
-00000560: 0865 0965 0465 0a66 0219 0065 0564 053c  .e.e.e.f...e.d.<
-00000570: 0064 065a 0b65 0c65 0564 073c 0064 0853  .d.Z.e.e.d.<.d.S
-00000580: 0029 09da 0c5f 4461 7461 7365 7442 6173  .)..._DatasetBas
-00000590: 657a 7e0a 2020 2020 4261 7365 2063 6c61  ez~.    Base cla
-000005a0: 7373 2066 6f72 2044 6174 6173 6574 0a0a  ss for Dataset..
-000005b0: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
-000005c0: 2020 2020 2020 2020 6e61 6d65 3a20 5442          name: TB
-000005d0: 440a 2020 2020 2020 2020 7479 7065 3a20  D.        type: 
-000005e0: 5442 440a 2020 2020 2020 2020 6d65 7461  TBD.        meta
-000005f0: 3a20 5442 440a 2020 2020 2020 2020 7265  : TBD.        re
-00000600: 6164 5f6f 6e6c 793a 2054 4244 0a20 2020  ad_only: TBD.   
-00000610: 20da 046e 616d 65da 0474 7970 6529 01da   ..name..type)..
-00000620: 0764 6566 6175 6c74 da04 6d65 7461 46da  .default..metaF.
-00000630: 0972 6561 645f 6f6e 6c79 4e29 0d72 1700  .read_onlyN).r..
+00000080: 0100 6408 6409 6c0a 6d0b 5a0b 0100 640a  ..d.d.l.m.Z...d.
+00000090: 5a0c 4700 640b 640c 8400 640c 6509 8303  Z.G.d.d...d.e...
+000000a0: 5a0d 4700 640d 640e 8400 640e 650d 8303  Z.G.d.d...d.e...
+000000b0: 5a0e 4700 640f 6410 8400 6410 650d 8303  Z.G.d.d...d.e...
+000000c0: 5a0f 4700 6411 6412 8400 6412 650d 8303  Z.G.d.d...d.e...
+000000d0: 5a10 4700 6413 6414 8400 6414 6509 8303  Z.G.d.d...d.e...
+000000e0: 5a11 4700 6415 6416 8400 6416 6511 8303  Z.G.d.d...d.e...
+000000f0: 5a12 4700 6417 6418 8400 6418 6511 8303  Z.G.d.d...d.e...
+00000100: 5a13 4700 6419 641a 8400 641a 6511 8303  Z.G.d.d...d.e...
+00000110: 5a14 4700 641b 641c 8400 641c 6509 8303  Z.G.d.d...d.e...
+00000120: 5a15 4700 641d 641e 8400 641e 6515 8303  Z.G.d.d...d.e...
+00000130: 5a16 4700 641f 6420 8400 6420 6515 8303  Z.G.d.d ..d e...
+00000140: 5a17 4700 6421 6422 8400 6422 6515 8303  Z.G.d!d"..d"e...
+00000150: 5a18 6423 5300 2924 e900 0000 0029 01da  Z.d#S.)$.....)..
+00000160: 0341 6e79 2901 da04 4469 6374 2901 da04  .Any)...Dict)...
+00000170: 4c69 7374 2901 da08 4f70 7469 6f6e 616c  List)...Optional
+00000180: 2901 da05 4669 656c 6429 01da 0976 616c  )...Field)...val
+00000190: 6964 6174 6f72 2901 da08 5351 4c4d 6f64  idator)...SQLMod
+000001a0: 656c e901 0000 0029 01da 0676 616c 7374  el.....)...valst
+000001b0: 7229 09da 0d50 726f 6a65 6374 4372 6561  r)...ProjectCrea
+000001c0: 7465 da0b 5072 6f6a 6563 7452 6561 64da  te..ProjectRead.
+000001d0: 0d50 726f 6a65 6374 5570 6461 7465 da0d  .ProjectUpdate..
+000001e0: 4461 7461 7365 7455 7064 6174 65da 0d44  DatasetUpdate..D
+000001f0: 6174 6173 6574 4372 6561 7465 da0b 4461  atasetCreate..Da
+00000200: 7461 7365 7452 6561 64da 0e52 6573 6f75  tasetRead..Resou
+00000210: 7263 6543 7265 6174 65da 0c52 6573 6f75  rceCreate..Resou
+00000220: 7263 6552 6561 64da 0e52 6573 6f75 7263  rceRead..Resourc
+00000230: 6555 7064 6174 6563 0000 0000 0000 0000  eUpdatec........
+00000240: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000250: 731a 0000 0065 005a 0164 005a 0255 0064  s....e.Z.d.Z.U.d
+00000260: 015a 0365 0465 0564 023c 0064 0353 0029  .Z.e.e.d.<.d.S.)
+00000270: 04da 0d5f 5265 736f 7572 6365 4261 7365  ..._ResourceBase
+00000280: 7a21 0a20 2020 2042 6173 6520 636c 6173  z!.    Base clas
+00000290: 7320 666f 7220 5265 736f 7572 6365 0a20  s for Resource. 
+000002a0: 2020 20da 0470 6174 684e 2906 da08 5f5f     ..pathN)...__
+000002b0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+000002c0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+000002d0: da07 5f5f 646f 635f 5fda 0373 7472 da0f  ..__doc__..str..
+000002e0: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5fa9  __annotations__.
+000002f0: 0072 1c00 0000 721c 0000 00fa 3f2f 686f  .r....r.....?/ho
+00000300: 6d65 2f74 6f6d 6d61 736f 2f46 7261 6374  me/tommaso/Fract
+00000310: 616c 2f66 7261 6374 616c 2f66 7261 6374  al/fractal/fract
+00000320: 616c 2f63 6f6d 6d6f 6e2f 7363 6865 6d61  al/common/schema
+00000330: 732f 7072 6f6a 6563 742e 7079 7214 0000  s/project.pyr...
+00000340: 001d 0000 0073 0400 0000 0a01 0404 7214  .....s........r.
+00000350: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000360: 0000 0000 0400 0000 4000 0000 7320 0000  ........@...s ..
+00000370: 0065 005a 0164 005a 0265 0364 0164 0264  .e.Z.d.Z.e.d.d.d
+00000380: 038d 0265 0464 0183 0183 015a 0564 0453  ...e.d.....Z.d.S
+00000390: 0029 0572 1100 0000 7215 0000 0054 a901  .).r....r....T..
+000003a0: da0b 616c 6c6f 775f 7265 7573 654e a906  ..allow_reuseN..
+000003b0: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+000003c0: 0700 0000 720a 0000 00da 055f 7061 7468  ....r......_path
+000003d0: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
+000003e0: 1d00 0000 7211 0000 0025 0000 0073 0200  ....r....%...s..
+000003f0: 0000 0802 7211 0000 0063 0000 0000 0000  ....r....c......
+00000400: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+00000410: 0000 7320 0000 0065 005a 0164 005a 0265  ..s ...e.Z.d.Z.e
+00000420: 0364 0164 0264 038d 0265 0464 0183 0183  .d.d.d...e.d....
+00000430: 015a 0564 0453 0029 0572 1300 0000 7215  .Z.d.S.).r....r.
+00000440: 0000 0054 721e 0000 004e 7220 0000 0072  ...Tr....Nr ...r
+00000450: 1c00 0000 721c 0000 0072 1c00 0000 721d  ....r....r....r.
+00000460: 0000 0072 1300 0000 2a00 0000 7302 0000  ...r....*...s...
+00000470: 0008 0272 1300 0000 6300 0000 0000 0000  ...r....c.......
+00000480: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000490: 0073 1e00 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+000004a0: 6503 6504 6401 3c00 6503 6504 6402 3c00  e.e.d.<.e.e.d.<.
+000004b0: 6403 5300 2904 7212 0000 00da 0269 64da  d.S.).r......id.
+000004c0: 0a64 6174 6173 6574 5f69 644e 2905 7216  .dataset_idN).r.
+000004d0: 0000 0072 1700 0000 7218 0000 00da 0369  ...r....r......i
+000004e0: 6e74 721b 0000 0072 1c00 0000 721c 0000  ntr....r....r...
+000004f0: 0072 1c00 0000 721d 0000 0072 1200 0000  .r....r....r....
+00000500: 2f00 0000 7304 0000 000a 0108 0172 1200  /...s........r..
+00000510: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000520: 0000 0003 0000 0040 0000 0073 4c00 0000  .......@...sL...
+00000530: 6500 5a01 6400 5a02 5500 6401 5a03 6504  e.Z.d.Z.U.d.Z.e.
+00000540: 6505 6402 3c00 6506 6504 1900 6505 6403  e.d.<.e.e...e.d.
+00000550: 3c00 6507 6900 6404 8d01 5a08 6509 6504  <.e.i.d...Z.e.e.
+00000560: 650a 6602 1900 6505 6405 3c00 6406 5a0b  e.f...e.d.<.d.Z.
+00000570: 650c 6505 6407 3c00 6408 5300 2909 da0c  e.e.d.<.d.S.)...
+00000580: 5f44 6174 6173 6574 4261 7365 7a7e 0a20  _DatasetBasez~. 
+00000590: 2020 2042 6173 6520 636c 6173 7320 666f     Base class fo
+000005a0: 7220 4461 7461 7365 740a 0a20 2020 2041  r Dataset..    A
+000005b0: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
+000005c0: 2020 206e 616d 653a 2054 4244 0a20 2020     name: TBD.   
+000005d0: 2020 2020 2074 7970 653a 2054 4244 0a20       type: TBD. 
+000005e0: 2020 2020 2020 206d 6574 613a 2054 4244         meta: TBD
+000005f0: 0a20 2020 2020 2020 2072 6561 645f 6f6e  .        read_on
+00000600: 6c79 3a20 5442 440a 2020 2020 da04 6e61  ly: TBD.    ..na
+00000610: 6d65 da04 7479 7065 2901 da07 6465 6661  me..type)...defa
+00000620: 756c 74da 046d 6574 6146 da09 7265 6164  ult..metaF..read
+00000630: 5f6f 6e6c 794e 290d 7216 0000 0072 1700  _onlyN).r....r..
 00000640: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000650: 0072 1b00 0000 721c 0000 0072 0500 0000  .r....r....r....
-00000660: 7206 0000 0072 2c00 0000 7203 0000 0072  r....r,...r....r
-00000670: 0200 0000 722d 0000 00da 0462 6f6f 6c72  ....r-.....boolr
-00000680: 1d00 0000 721d 0000 0072 1d00 0000 721e  ....r....r....r.
-00000690: 0000 0072 2800 0000 3800 0000 730c 0000  ...r(...8...s...
-000006a0: 000a 0004 0108 0a0c 011a 0110 0172 2800  .............r(.
-000006b0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000006c0: 0000 0004 0000 0040 0000 0073 6600 0000  .......@...sf...
-000006d0: 6500 5a01 6400 5a02 5500 6503 6504 1900  e.Z.d.Z.U.e.e...
-000006e0: 6505 6401 3c00 6402 5a06 6503 6507 6504  e.d.<.d.Z.e.e.e.
-000006f0: 6508 6602 1900 1900 6505 6403 3c00 6503  e.f.....e.d.<.e.
-00000700: 6509 1900 6505 6404 3c00 650a 6401 6405  e...e.d.<.e.d.d.
-00000710: 6406 8d02 650b 6401 8301 8301 5a0c 650a  d...e.d.....Z.e.
-00000720: 6407 6405 6406 8d02 650b 6407 8301 8301  d.d.d...e.d.....
-00000730: 5a0d 6402 5300 2908 720f 0000 0072 2900  Z.d.S.).r....r).
-00000740: 0000 4e72 2c00 0000 722d 0000 0054 7220  ..Nr,...r-...Tr 
-00000750: 0000 0072 2a00 0000 290e 7217 0000 0072  ...r*...).r....r
-00000760: 1800 0000 7219 0000 0072 0500 0000 721b  ....r....r....r.
-00000770: 0000 0072 1c00 0000 722c 0000 0072 0300  ...r....r,...r..
-00000780: 0000 7202 0000 0072 2e00 0000 7207 0000  ..r....r....r...
-00000790: 0072 0b00 0000 da05 5f6e 616d 65da 055f  .r......_name.._
-000007a0: 7479 7065 721d 0000 0072 1d00 0000 721d  typer....r....r.
-000007b0: 0000 0072 1e00 0000 720f 0000 0049 0000  ...r....r....I..
-000007c0: 0073 0c00 0000 0a00 0c01 1801 0c01 1403  .s..............
-000007d0: 1801 720f 0000 0063 0000 0000 0000 0000  ..r....c........
-000007e0: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-000007f0: 7334 0000 0065 005a 0164 005a 0265 0364  s4...e.Z.d.Z.e.d
-00000800: 0164 0264 038d 0265 0464 0183 0183 015a  .d.d...e.d.....Z
-00000810: 0565 0364 0464 0264 038d 0265 0464 0483  .e.d.d.d...e.d..
-00000820: 0183 015a 0664 0553 0029 0672 1000 0000  ...Z.d.S.).r....
-00000830: 7229 0000 0054 7220 0000 0072 2a00 0000  r)...Tr ...r*...
-00000840: 4e29 0772 1700 0000 7218 0000 0072 1900  N).r....r....r..
-00000850: 0000 7207 0000 0072 0b00 0000 722f 0000  ..r....r....r/..
-00000860: 0072 3000 0000 721d 0000 0072 1d00 0000  .r0...r....r....
-00000870: 721d 0000 0072 1e00 0000 7210 0000 0053  r....r....r....S
-00000880: 0000 0073 0600 0000 0800 1402 1801 7210  ...s..........r.
-00000890: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000008a0: 0000 0000 0300 0000 4000 0000 7332 0000  ........@...s2..
-000008b0: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
-000008c0: 013c 0065 0565 0619 0065 0464 023c 0065  .<.e.e...e.d.<.e
-000008d0: 0365 0464 033c 0065 0765 0464 043c 0064  .e.d.<.e.e.d.<.d
-000008e0: 0553 0029 0672 1100 0000 7225 0000 00da  .S.).r....r%....
-000008f0: 0d72 6573 6f75 7263 655f 6c69 7374 da0a  .resource_list..
-00000900: 7072 6f6a 6563 745f 6964 722d 0000 004e  project_idr-...N
-00000910: 2908 7217 0000 0072 1800 0000 7219 0000  ).r....r....r...
-00000920: 0072 2700 0000 721c 0000 0072 0400 0000  .r'...r....r....
-00000930: 7213 0000 0072 2e00 0000 721d 0000 0072  r....r....r....r
-00000940: 1d00 0000 721d 0000 0072 1e00 0000 7211  ....r....r....r.
-00000950: 0000 0059 0000 0073 0a00 0000 0a00 0801  ...Y...s........
-00000960: 0c01 0801 0c01 7211 0000 0063 0000 0000  ......r....c....
-00000970: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000980: 4000 0000 7326 0000 0065 005a 0164 005a  @...s&...e.Z.d.Z
-00000990: 0255 0064 015a 0365 0465 0564 023c 0064  .U.d.Z.e.e.d.<.d
-000009a0: 035a 0665 0765 0564 043c 0064 0553 0029  .Z.e.e.d.<.d.S.)
-000009b0: 06da 0c5f 5072 6f6a 6563 7442 6173 657a  ..._ProjectBasez
-000009c0: 5a0a 2020 2020 4261 7365 2063 6c61 7373  Z.    Base class
-000009d0: 2066 6f72 2050 726f 6a65 6374 0a0a 2020   for Project..  
-000009e0: 2020 4174 7472 6962 7574 6573 3a0a 2020    Attributes:.  
-000009f0: 2020 2020 2020 6e61 6d65 3a20 5442 440a        name: TBD.
-00000a00: 2020 2020 2020 2020 7265 6164 5f6f 6e6c          read_onl
-00000a10: 793a 2054 4244 0a20 2020 2072 2900 0000  y: TBD.    r)...
-00000a20: 4672 2d00 0000 4e29 0872 1700 0000 7218  Fr-...N).r....r.
-00000a30: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
-00000a40: 0000 721c 0000 0072 2d00 0000 722e 0000  ..r....r-...r...
-00000a50: 0072 1d00 0000 721d 0000 0072 1d00 0000  .r....r....r....
-00000a60: 721e 0000 0072 3300 0000 6300 0000 7308  r....r3...c...s.
-00000a70: 0000 000a 0004 0108 0810 0172 3300 0000  ...........r3...
-00000a80: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000a90: 0004 0000 0040 0000 0073 4600 0000 6500  .....@...sF...e.
-00000aa0: 5a01 6400 5a02 5500 6401 5a03 6504 6505  Z.d.Z.U.d.Z.e.e.
-00000ab0: 1900 6506 6402 3c00 6507 6403 6404 6405  ..e.d.<.e.d.d.d.
-00000ac0: 8d02 6508 6403 8301 8301 5a09 6507 6402  ..e.d.....Z.e.d.
-00000ad0: 6404 6405 8d02 6508 6402 8301 8301 5a0a  d.d...e.d.....Z.
-00000ae0: 6406 5300 2907 720c 0000 0072 2b00 0000  d.S.).r....r+...
-00000af0: da14 6465 6661 756c 745f 6461 7461 7365  ..default_datase
-00000b00: 745f 6e61 6d65 7229 0000 0054 7220 0000  t_namer)...Tr ..
-00000b10: 004e 290b 7217 0000 0072 1800 0000 7219  .N).r....r....r.
-00000b20: 0000 0072 3400 0000 7205 0000 0072 1b00  ...r4...r....r..
-00000b30: 0000 721c 0000 0072 0700 0000 720b 0000  ..r....r....r...
-00000b40: 0072 2f00 0000 da15 5f64 6566 6175 6c74  .r/....._default
-00000b50: 5f64 6174 6173 6574 5f6e 616d 6572 1d00  _dataset_namer..
-00000b60: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00000b70: 0072 0c00 0000 7000 0000 7310 0000 000a  .r....p...s.....
-00000b80: 0010 0114 0302 0104 0104 ff06 0208 fe72  ...............r
-00000b90: 0c00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000ba0: 0000 0000 0003 0000 0040 0000 0073 2600  .........@...s&.
-00000bb0: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-00000bc0: 6401 3c00 6700 5a05 6506 6507 1900 6504  d.<.g.Z.e.e...e.
-00000bd0: 6402 3c00 6403 5300 2904 720d 0000 0072  d.<.d.S.).r....r
-00000be0: 2500 0000 da0c 6461 7461 7365 745f 6c69  %.....dataset_li
-00000bf0: 7374 4e29 0872 1700 0000 7218 0000 0072  stN).r....r....r
-00000c00: 1900 0000 7227 0000 0072 1c00 0000 7236  ....r'...r....r6
-00000c10: 0000 0072 0400 0000 7211 0000 0072 1d00  ...r....r....r..
-00000c20: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00000c30: 0072 0d00 0000 7a00 0000 7306 0000 000a  .r....z...s.....
-00000c40: 0008 0114 0172 0d00 0000 6300 0000 0000  .....r....c.....
-00000c50: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
-00000c60: 0000 0073 3a00 0000 6500 5a01 6400 5a02  ...s:...e.Z.d.Z.
-00000c70: 5500 6503 6504 1900 6505 6401 3c00 6503  U.e.e...e.d.<.e.
-00000c80: 6506 1900 6505 6402 3c00 6507 6401 6403  e...e.d.<.e.d.d.
-00000c90: 6404 8d02 6508 6401 8301 8301 5a09 6405  d...e.d.....Z.d.
-00000ca0: 5300 2906 720e 0000 0072 2900 0000 722d  S.).r....r)...r-
-00000cb0: 0000 0054 7220 0000 004e 290a 7217 0000  ...Tr ...N).r...
-00000cc0: 0072 1800 0000 7219 0000 0072 0500 0000  .r....r....r....
-00000cd0: 721b 0000 0072 1c00 0000 722e 0000 0072  r....r....r....r
-00000ce0: 0700 0000 720b 0000 0072 2f00 0000 721d  ....r....r/...r.
-00000cf0: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
-00000d00: 0000 720e 0000 007f 0000 0073 0800 0000  ..r........s....
-00000d10: 0a00 0c01 0c01 1803 720e 0000 004e 291a  ........r....N).
-00000d20: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
-00000d30: 0000 7204 0000 0072 0500 0000 da08 7079  ..r....r......py
-00000d40: 6461 6e74 6963 7206 0000 0072 0700 0000  danticr....r....
-00000d50: da08 7371 6c6d 6f64 656c 7208 0000 00da  ..sqlmodelr.....
-00000d60: 0b5f 7661 6c69 6461 746f 7273 720a 0000  ._validatorsr...
-00000d70: 0072 0b00 0000 da07 5f5f 616c 6c5f 5f72  .r......__all__r
-00000d80: 1500 0000 7212 0000 0072 1400 0000 7213  ....r....r....r.
-00000d90: 0000 0072 2800 0000 720f 0000 0072 1000  ...r(...r....r..
-00000da0: 0000 7211 0000 0072 3300 0000 720c 0000  ..r....r3...r...
-00000db0: 0072 0d00 0000 720e 0000 0072 1d00 0000  .r....r....r....
-00000dc0: 721d 0000 0072 1d00 0000 721e 0000 00da  r....r....r.....
-00000dd0: 083c 6d6f 6475 6c65 3e01 0000 0073 2c00  .<module>....s,.
-00000de0: 0000 0c00 0c01 0c01 0c01 0c02 0c01 0c01  ................
-00000df0: 0c02 0c01 0403 1010 1008 1005 1005 1008  ................
-00000e00: 1011 100a 1006 100a 100d 100a 1405       ..............
+00000650: 0072 1b00 0000 7205 0000 0072 0600 0000  .r....r....r....
+00000660: 7229 0000 0072 0300 0000 7202 0000 0072  r)...r....r....r
+00000670: 2a00 0000 da04 626f 6f6c 721c 0000 0072  *.....boolr....r
+00000680: 1c00 0000 721c 0000 0072 1d00 0000 7225  ....r....r....r%
+00000690: 0000 0037 0000 0073 0a00 0000 0a01 040a  ...7...s........
+000006a0: 0801 0c01 1a01 7225 0000 0063 0000 0000  ......r%...c....
+000006b0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+000006c0: 4000 0000 7366 0000 0065 005a 0164 005a  @...sf...e.Z.d.Z
+000006d0: 0255 0065 0365 0419 0065 0564 013c 0064  .U.e.e...e.d.<.d
+000006e0: 025a 0665 0365 0765 0465 0866 0219 0019  .Z.e.e.e.e.f....
+000006f0: 0065 0564 033c 0065 0365 0919 0065 0564  .e.d.<.e.e...e.d
+00000700: 043c 0065 0a64 0164 0564 068d 0265 0b64  .<.e.d.d.d...e.d
+00000710: 0183 0183 015a 0c65 0a64 0764 0564 068d  .....Z.e.d.d.d..
+00000720: 0265 0b64 0783 0183 015a 0d64 0253 0029  .e.d.....Z.d.S.)
+00000730: 0872 0e00 0000 7226 0000 004e 7229 0000  .r....r&...Nr)..
+00000740: 0072 2a00 0000 5472 1e00 0000 7227 0000  .r*...Tr....r'..
+00000750: 0029 0e72 1600 0000 7217 0000 0072 1800  .).r....r....r..
+00000760: 0000 7205 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000770: 0072 2900 0000 7203 0000 0072 0200 0000  .r)...r....r....
+00000780: 722b 0000 0072 0700 0000 720a 0000 00da  r+...r....r.....
+00000790: 055f 6e61 6d65 da05 5f74 7970 6572 1c00  ._name.._typer..
+000007a0: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+000007b0: 0072 0e00 0000 4800 0000 730a 0000 000a  .r....H...s.....
+000007c0: 010c 0118 010c 0314 0172 0e00 0000 6300  .........r....c.
+000007d0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+000007e0: 0000 0040 0000 0073 3400 0000 6500 5a01  ...@...s4...e.Z.
+000007f0: 6400 5a02 6503 6401 6402 6403 8d02 6504  d.Z.e.d.d.d...e.
+00000800: 6401 8301 8301 5a05 6503 6404 6402 6403  d.....Z.e.d.d.d.
+00000810: 8d02 6504 6404 8301 8301 5a06 6405 5300  ..e.d.....Z.d.S.
+00000820: 2906 720f 0000 0072 2600 0000 5472 1e00  ).r....r&...Tr..
+00000830: 0000 7227 0000 004e 2907 7216 0000 0072  ..r'...N).r....r
+00000840: 1700 0000 7218 0000 0072 0700 0000 720a  ....r....r....r.
+00000850: 0000 0072 2c00 0000 722d 0000 0072 1c00  ...r,...r-...r..
+00000860: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00000870: 0072 0f00 0000 5200 0000 7304 0000 0008  .r....R...s.....
+00000880: 0214 0172 0f00 0000 6300 0000 0000 0000  ...r....c.......
+00000890: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000008a0: 0073 3200 0000 6500 5a01 6400 5a02 5500  .s2...e.Z.d.Z.U.
+000008b0: 6503 6504 6401 3c00 6505 6506 1900 6504  e.e.d.<.e.e...e.
+000008c0: 6402 3c00 6503 6504 6403 3c00 6507 6504  d.<.e.e.d.<.e.e.
+000008d0: 6404 3c00 6405 5300 2906 7210 0000 0072  d.<.d.S.).r....r
+000008e0: 2200 0000 da0d 7265 736f 7572 6365 5f6c  ".....resource_l
+000008f0: 6973 74da 0a70 726f 6a65 6374 5f69 6472  ist..project_idr
+00000900: 2a00 0000 4e29 0872 1600 0000 7217 0000  *...N).r....r...
+00000910: 0072 1800 0000 7224 0000 0072 1b00 0000  .r....r$...r....
+00000920: 7204 0000 0072 1200 0000 722b 0000 0072  r....r....r+...r
+00000930: 1c00 0000 721c 0000 0072 1c00 0000 721d  ....r....r....r.
+00000940: 0000 0072 1000 0000 5800 0000 7308 0000  ...r....X...s...
+00000950: 000a 0108 010c 0108 0172 1000 0000 6300  .........r....c.
+00000960: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000970: 0000 0040 0000 0073 2e00 0000 6500 5a01  ...@...s....e.Z.
+00000980: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
+00000990: 3c00 6504 6505 6403 3c00 6404 5a06 6507  <.e.e.d.<.d.Z.e.
+000009a0: 6505 6405 3c00 6406 5300 2907 da0c 5f50  e.d.<.d.S.)..._P
+000009b0: 726f 6a65 6374 4261 7365 7a73 0a20 2020  rojectBasezs.   
+000009c0: 2042 6173 6520 636c 6173 7320 666f 7220   Base class for 
+000009d0: 5072 6f6a 6563 740a 0a20 2020 2041 7474  Project..    Att
+000009e0: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
+000009f0: 206e 616d 653a 2054 4244 0a20 2020 2020   name: TBD.     
+00000a00: 2020 2070 726f 6a65 6374 5f64 6972 3a20     project_dir: 
+00000a10: 5442 440a 2020 2020 2020 2020 7265 6164  TBD.        read
+00000a20: 5f6f 6e6c 793a 2054 4244 0a20 2020 2072  _only: TBD.    r
+00000a30: 2600 0000 da0b 7072 6f6a 6563 745f 6469  &.....project_di
+00000a40: 7246 722a 0000 004e 2908 7216 0000 0072  rFr*...N).r....r
+00000a50: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
+00000a60: 0000 0072 1b00 0000 722a 0000 0072 2b00  ...r....r*...r+.
+00000a70: 0000 721c 0000 0072 1c00 0000 721c 0000  ..r....r....r...
+00000a80: 0072 1d00 0000 7230 0000 0062 0000 0073  .r....r0...b...s
+00000a90: 0800 0000 0a01 0409 0801 0801 7230 0000  ............r0..
+00000aa0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000ab0: 0000 0400 0000 4000 0000 735a 0000 0065  ......@...sZ...e
+00000ac0: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
+00000ad0: 0519 0065 0664 023c 0065 0764 0364 0464  ...e.d.<.e.d.d.d
+00000ae0: 058d 0265 0864 0383 0183 015a 0965 0764  ...e.d.....Z.e.d
+00000af0: 0664 0464 058d 0265 0864 0683 0183 015a  .d.d...e.d.....Z
+00000b00: 0a65 0764 0264 0464 058d 0265 0864 0283  .e.d.d.d...e.d..
+00000b10: 0183 015a 0b64 0753 0029 0872 0b00 0000  ...Z.d.S.).r....
+00000b20: 7228 0000 00da 1464 6566 6175 6c74 5f64  r(.....default_d
+00000b30: 6174 6173 6574 5f6e 616d 6572 2600 0000  ataset_namer&...
+00000b40: 5472 1e00 0000 7231 0000 004e 290c 7216  Tr....r1...N).r.
+00000b50: 0000 0072 1700 0000 7218 0000 0072 3200  ...r....r....r2.
+00000b60: 0000 7205 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000b70: 0072 0700 0000 720a 0000 0072 2c00 0000  .r....r....r,...
+00000b80: da0c 5f70 726f 6a65 6374 5f64 6972 5a15  .._project_dirZ.
+00000b90: 5f64 6566 6175 6c74 5f64 6174 6173 6574  _default_dataset
+00000ba0: 5f6e 616d 6572 1c00 0000 721c 0000 0072  _namer....r....r
+00000bb0: 1c00 0000 721d 0000 0072 0b00 0000 7100  ....r....r....q.
+00000bc0: 0000 7314 0000 000a 0110 0314 010a 0106  ..s.............
+00000bd0: ff04 0302 0104 ff04 0206 fe72 0b00 0000  ...........r....
+00000be0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000bf0: 0003 0000 0040 0000 0073 2600 0000 6500  .....@...s&...e.
+00000c00: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
+00000c10: 6700 5a05 6506 6507 1900 6504 6402 3c00  g.Z.e.e...e.d.<.
+00000c20: 6403 5300 2904 720c 0000 0072 2200 0000  d.S.).r....r"...
+00000c30: da0c 6461 7461 7365 745f 6c69 7374 4e29  ..dataset_listN)
+00000c40: 0872 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000c50: 7224 0000 0072 1b00 0000 7234 0000 0072  r$...r....r4...r
+00000c60: 0400 0000 7210 0000 0072 1c00 0000 721c  ....r....r....r.
+00000c70: 0000 0072 1c00 0000 721d 0000 0072 0c00  ...r....r....r..
+00000c80: 0000 7e00 0000 7304 0000 000a 0108 0172  ..~...s........r
+00000c90: 0c00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000ca0: 0000 0000 0004 0000 0040 0000 0073 5a00  .........@...sZ.
+00000cb0: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
+00000cc0: 1900 6505 6401 3c00 6503 6504 1900 6505  ..e.d.<.e.e...e.
+00000cd0: 6402 3c00 6503 6506 1900 6505 6403 3c00  d.<.e.e...e.d.<.
+00000ce0: 6507 6401 6404 6405 8d02 6508 6401 8301  e.d.d.d...e.d...
+00000cf0: 8301 5a09 6507 6402 6404 6405 8d02 6508  ..Z.e.d.d.d...e.
+00000d00: 6402 8301 8301 5a0a 6406 5300 2907 720d  d.....Z.d.S.).r.
+00000d10: 0000 0072 2600 0000 7231 0000 0072 2a00  ...r&...r1...r*.
+00000d20: 0000 5472 1e00 0000 4e29 0b72 1600 0000  ..Tr....N).r....
+00000d30: 7217 0000 0072 1800 0000 7205 0000 0072  r....r....r....r
+00000d40: 1a00 0000 721b 0000 0072 2b00 0000 7207  ....r....r+...r.
+00000d50: 0000 0072 0a00 0000 722c 0000 0072 3300  ...r....r,...r3.
+00000d60: 0000 721c 0000 0072 1c00 0000 721c 0000  ..r....r....r...
+00000d70: 0072 1d00 0000 720d 0000 0083 0000 0073  .r....r........s
+00000d80: 0e00 0000 0a01 0c01 0c01 0c03 1401 0a01  ................
+00000d90: 06ff 720d 0000 004e 2919 da06 7479 7069  ..r....N)...typi
+00000da0: 6e67 7202 0000 0072 0300 0000 7204 0000  ngr....r....r...
+00000db0: 0072 0500 0000 da08 7079 6461 6e74 6963  .r......pydantic
+00000dc0: 7206 0000 0072 0700 0000 da08 7371 6c6d  r....r......sqlm
+00000dd0: 6f64 656c 7208 0000 00da 0b5f 7661 6c69  odelr......_vali
+00000de0: 6461 746f 7273 720a 0000 00da 075f 5f61  datorsr......__a
+00000df0: 6c6c 5f5f 7214 0000 0072 1100 0000 7213  ll__r....r....r.
+00000e00: 0000 0072 1200 0000 7225 0000 0072 0e00  ...r....r%...r..
+00000e10: 0000 720f 0000 0072 1000 0000 7230 0000  ..r....r....r0..
+00000e20: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000e30: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
+00000e40: 1d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000e50: 0000 7328 0000 000c 010c 010c 010c 020c  ..s(............
+00000e60: 010c 010c 020c 0304 1010 0810 0510 0510  ................
+00000e70: 0810 1110 0a10 0610 0a10 0f10 0d10 05    ...............
```

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/project.cpython-39.pyc` & `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Mar 15 12:00:37 2023 UTC, .py size: 2737 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,232 +1,222 @@
-00000000: 610d 0d0a 0000 0000 65b3 1164 b10a 0000  a.......e..d....
+00000000: 6f0d 0d0a 0000 0000 5b56 7064 b309 0000  o.......[Vpd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
+00000020: 0004 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
-00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c05 6d06 5a06 0100 6400 6406 6c05  d.l.m.Z...d.d.l.
-00000070: 6d07 5a07 0100 6400 6407 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000080: 0100 6408 6409 6c0a 6d0b 5a0b 0100 640a  ..d.d.l.m.Z...d.
-00000090: 5a0c 4700 640b 640c 8400 640c 6509 8303  Z.G.d.d...d.e...
-000000a0: 5a0d 4700 640d 640e 8400 640e 650d 8303  Z.G.d.d...d.e...
-000000b0: 5a0e 4700 640f 6410 8400 6410 650d 8303  Z.G.d.d...d.e...
-000000c0: 5a0f 4700 6411 6412 8400 6412 650d 8303  Z.G.d.d...d.e...
-000000d0: 5a10 4700 6413 6414 8400 6414 6509 8303  Z.G.d.d...d.e...
-000000e0: 5a11 4700 6415 6416 8400 6416 6511 8303  Z.G.d.d...d.e...
-000000f0: 5a12 4700 6417 6418 8400 6418 6511 8303  Z.G.d.d...d.e...
-00000100: 5a13 4700 6419 641a 8400 641a 6511 8303  Z.G.d.d...d.e...
-00000110: 5a14 4700 641b 641c 8400 641c 6509 8303  Z.G.d.d...d.e...
-00000120: 5a15 4700 641d 641e 8400 641e 6515 8303  Z.G.d.d...d.e...
-00000130: 5a16 4700 641f 6420 8400 6420 6515 8303  Z.G.d.d ..d e...
-00000140: 5a17 4700 6421 6422 8400 6422 6515 8303  Z.G.d!d"..d"e...
-00000150: 5a18 6423 5300 2924 e900 0000 0029 01da  Z.d#S.)$.....)..
-00000160: 0341 6e79 2901 da04 4469 6374 2901 da04  .Any)...Dict)...
-00000170: 4c69 7374 2901 da08 4f70 7469 6f6e 616c  List)...Optional
-00000180: 2901 da05 4669 656c 6429 01da 0976 616c  )...Field)...val
-00000190: 6964 6174 6f72 2901 da08 5351 4c4d 6f64  idator)...SQLMod
-000001a0: 656c e901 0000 0029 01da 0676 616c 7374  el.....)...valst
-000001b0: 7229 09da 0d50 726f 6a65 6374 4372 6561  r)...ProjectCrea
-000001c0: 7465 da0b 5072 6f6a 6563 7452 6561 64da  te..ProjectRead.
-000001d0: 0d50 726f 6a65 6374 5570 6461 7465 da0d  .ProjectUpdate..
-000001e0: 4461 7461 7365 7455 7064 6174 65da 0d44  DatasetUpdate..D
-000001f0: 6174 6173 6574 4372 6561 7465 da0b 4461  atasetCreate..Da
-00000200: 7461 7365 7452 6561 64da 0e52 6573 6f75  tasetRead..Resou
-00000210: 7263 6543 7265 6174 65da 0c52 6573 6f75  rceCreate..Resou
-00000220: 7263 6552 6561 64da 0e52 6573 6f75 7263  rceRead..Resourc
-00000230: 6555 7064 6174 6563 0000 0000 0000 0000  eUpdatec........
-00000240: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000250: 731a 0000 0065 005a 0164 005a 0255 0064  s....e.Z.d.Z.U.d
-00000260: 015a 0365 0465 0564 023c 0064 0353 0029  .Z.e.e.d.<.d.S.)
-00000270: 04da 0d5f 5265 736f 7572 6365 4261 7365  ..._ResourceBase
-00000280: 7a21 0a20 2020 2042 6173 6520 636c 6173  z!.    Base clas
-00000290: 7320 666f 7220 5265 736f 7572 6365 0a20  s for Resource. 
-000002a0: 2020 20da 0470 6174 684e 2906 da08 5f5f     ..pathN)...__
-000002b0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000002c0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000002d0: da07 5f5f 646f 635f 5fda 0373 7472 da0f  ..__doc__..str..
-000002e0: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5fa9  __annotations__.
-000002f0: 0072 1c00 0000 721c 0000 00fa 3f2f 686f  .r....r.....?/ho
-00000300: 6d65 2f74 6f6d 6d61 736f 2f46 7261 6374  me/tommaso/Fract
-00000310: 616c 2f66 7261 6374 616c 2f66 7261 6374  al/fractal/fract
-00000320: 616c 2f63 6f6d 6d6f 6e2f 7363 6865 6d61  al/common/schema
-00000330: 732f 7072 6f6a 6563 742e 7079 7214 0000  s/project.pyr...
-00000340: 001d 0000 0073 0400 0000 0a01 0404 7214  .....s........r.
-00000350: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000360: 0000 0000 0400 0000 4000 0000 7320 0000  ........@...s ..
-00000370: 0065 005a 0164 005a 0265 0364 0164 0264  .e.Z.d.Z.e.d.d.d
-00000380: 038d 0265 0464 0183 0183 015a 0564 0453  ...e.d.....Z.d.S
-00000390: 0029 0572 1100 0000 7215 0000 0054 a901  .).r....r....T..
-000003a0: da0b 616c 6c6f 775f 7265 7573 654e a906  ..allow_reuseN..
-000003b0: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-000003c0: 0700 0000 720a 0000 00da 055f 7061 7468  ....r......_path
-000003d0: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
-000003e0: 1d00 0000 7211 0000 0025 0000 0073 0200  ....r....%...s..
-000003f0: 0000 0802 7211 0000 0063 0000 0000 0000  ....r....c......
-00000400: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
-00000410: 0000 7320 0000 0065 005a 0164 005a 0265  ..s ...e.Z.d.Z.e
-00000420: 0364 0164 0264 038d 0265 0464 0183 0183  .d.d.d...e.d....
-00000430: 015a 0564 0453 0029 0572 1300 0000 7215  .Z.d.S.).r....r.
-00000440: 0000 0054 721e 0000 004e 7220 0000 0072  ...Tr....Nr ...r
-00000450: 1c00 0000 721c 0000 0072 1c00 0000 721d  ....r....r....r.
-00000460: 0000 0072 1300 0000 2a00 0000 7302 0000  ...r....*...s...
-00000470: 0008 0272 1300 0000 6300 0000 0000 0000  ...r....c.......
-00000480: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000490: 0073 1e00 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
-000004a0: 6503 6504 6401 3c00 6503 6504 6402 3c00  e.e.d.<.e.e.d.<.
-000004b0: 6403 5300 2904 7212 0000 00da 0269 64da  d.S.).r......id.
-000004c0: 0a64 6174 6173 6574 5f69 644e 2905 7216  .dataset_idN).r.
-000004d0: 0000 0072 1700 0000 7218 0000 00da 0369  ...r....r......i
-000004e0: 6e74 721b 0000 0072 1c00 0000 721c 0000  ntr....r....r...
-000004f0: 0072 1c00 0000 721d 0000 0072 1200 0000  .r....r....r....
-00000500: 2f00 0000 7304 0000 000a 0108 0172 1200  /...s........r..
-00000510: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000520: 0000 0003 0000 0040 0000 0073 4c00 0000  .......@...sL...
-00000530: 6500 5a01 6400 5a02 5500 6401 5a03 6504  e.Z.d.Z.U.d.Z.e.
-00000540: 6505 6402 3c00 6506 6504 1900 6505 6403  e.d.<.e.e...e.d.
-00000550: 3c00 6507 6900 6404 8d01 5a08 6509 6504  <.e.i.d...Z.e.e.
-00000560: 650a 6602 1900 6505 6405 3c00 6406 5a0b  e.f...e.d.<.d.Z.
-00000570: 650c 6505 6407 3c00 6408 5300 2909 da0c  e.e.d.<.d.S.)...
-00000580: 5f44 6174 6173 6574 4261 7365 7a7e 0a20  _DatasetBasez~. 
-00000590: 2020 2042 6173 6520 636c 6173 7320 666f     Base class fo
-000005a0: 7220 4461 7461 7365 740a 0a20 2020 2041  r Dataset..    A
-000005b0: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
-000005c0: 2020 206e 616d 653a 2054 4244 0a20 2020     name: TBD.   
-000005d0: 2020 2020 2074 7970 653a 2054 4244 0a20       type: TBD. 
-000005e0: 2020 2020 2020 206d 6574 613a 2054 4244         meta: TBD
-000005f0: 0a20 2020 2020 2020 2072 6561 645f 6f6e  .        read_on
-00000600: 6c79 3a20 5442 440a 2020 2020 da04 6e61  ly: TBD.    ..na
-00000610: 6d65 da04 7479 7065 2901 da07 6465 6661  me..type)...defa
-00000620: 756c 74da 046d 6574 6146 da09 7265 6164  ult..metaF..read
-00000630: 5f6f 6e6c 794e 290d 7216 0000 0072 1700  _onlyN).r....r..
-00000640: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000650: 0072 1b00 0000 7205 0000 0072 0600 0000  .r....r....r....
-00000660: 7229 0000 0072 0300 0000 7202 0000 0072  r)...r....r....r
-00000670: 2a00 0000 da04 626f 6f6c 721c 0000 0072  *.....boolr....r
-00000680: 1c00 0000 721c 0000 0072 1d00 0000 7225  ....r....r....r%
-00000690: 0000 0037 0000 0073 0a00 0000 0a01 040a  ...7...s........
-000006a0: 0801 0c01 1a01 7225 0000 0063 0000 0000  ......r%...c....
-000006b0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-000006c0: 4000 0000 7366 0000 0065 005a 0164 005a  @...sf...e.Z.d.Z
-000006d0: 0255 0065 0365 0419 0065 0564 013c 0064  .U.e.e...e.d.<.d
-000006e0: 025a 0665 0365 0765 0465 0866 0219 0019  .Z.e.e.e.e.f....
-000006f0: 0065 0564 033c 0065 0365 0919 0065 0564  .e.d.<.e.e...e.d
-00000700: 043c 0065 0a64 0164 0564 068d 0265 0b64  .<.e.d.d.d...e.d
-00000710: 0183 0183 015a 0c65 0a64 0764 0564 068d  .....Z.e.d.d.d..
-00000720: 0265 0b64 0783 0183 015a 0d64 0253 0029  .e.d.....Z.d.S.)
-00000730: 0872 0e00 0000 7226 0000 004e 7229 0000  .r....r&...Nr)..
-00000740: 0072 2a00 0000 5472 1e00 0000 7227 0000  .r*...Tr....r'..
-00000750: 0029 0e72 1600 0000 7217 0000 0072 1800  .).r....r....r..
-00000760: 0000 7205 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00000770: 0072 2900 0000 7203 0000 0072 0200 0000  .r)...r....r....
-00000780: 722b 0000 0072 0700 0000 720a 0000 00da  r+...r....r.....
-00000790: 055f 6e61 6d65 da05 5f74 7970 6572 1c00  ._name.._typer..
-000007a0: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-000007b0: 0072 0e00 0000 4800 0000 730a 0000 000a  .r....H...s.....
-000007c0: 010c 0118 010c 0314 0172 0e00 0000 6300  .........r....c.
-000007d0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-000007e0: 0000 0040 0000 0073 3400 0000 6500 5a01  ...@...s4...e.Z.
-000007f0: 6400 5a02 6503 6401 6402 6403 8d02 6504  d.Z.e.d.d.d...e.
-00000800: 6401 8301 8301 5a05 6503 6404 6402 6403  d.....Z.e.d.d.d.
-00000810: 8d02 6504 6404 8301 8301 5a06 6405 5300  ..e.d.....Z.d.S.
-00000820: 2906 720f 0000 0072 2600 0000 5472 1e00  ).r....r&...Tr..
-00000830: 0000 7227 0000 004e 2907 7216 0000 0072  ..r'...N).r....r
-00000840: 1700 0000 7218 0000 0072 0700 0000 720a  ....r....r....r.
-00000850: 0000 0072 2c00 0000 722d 0000 0072 1c00  ...r,...r-...r..
-00000860: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00000870: 0072 0f00 0000 5200 0000 7304 0000 0008  .r....R...s.....
-00000880: 0214 0172 0f00 0000 6300 0000 0000 0000  ...r....c.......
-00000890: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-000008a0: 0073 3200 0000 6500 5a01 6400 5a02 5500  .s2...e.Z.d.Z.U.
-000008b0: 6503 6504 6401 3c00 6505 6506 1900 6504  e.e.d.<.e.e...e.
-000008c0: 6402 3c00 6503 6504 6403 3c00 6507 6504  d.<.e.e.d.<.e.e.
-000008d0: 6404 3c00 6405 5300 2906 7210 0000 0072  d.<.d.S.).r....r
-000008e0: 2200 0000 da0d 7265 736f 7572 6365 5f6c  ".....resource_l
-000008f0: 6973 74da 0a70 726f 6a65 6374 5f69 6472  ist..project_idr
-00000900: 2a00 0000 4e29 0872 1600 0000 7217 0000  *...N).r....r...
-00000910: 0072 1800 0000 7224 0000 0072 1b00 0000  .r....r$...r....
-00000920: 7204 0000 0072 1200 0000 722b 0000 0072  r....r....r+...r
-00000930: 1c00 0000 721c 0000 0072 1c00 0000 721d  ....r....r....r.
-00000940: 0000 0072 1000 0000 5800 0000 7308 0000  ...r....X...s...
-00000950: 000a 0108 010c 0108 0172 1000 0000 6300  .........r....c.
-00000960: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000970: 0000 0040 0000 0073 2e00 0000 6500 5a01  ...@...s....e.Z.
-00000980: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
-00000990: 3c00 6504 6505 6403 3c00 6404 5a06 6507  <.e.e.d.<.d.Z.e.
-000009a0: 6505 6405 3c00 6406 5300 2907 da0c 5f50  e.d.<.d.S.)..._P
-000009b0: 726f 6a65 6374 4261 7365 7a73 0a20 2020  rojectBasezs.   
-000009c0: 2042 6173 6520 636c 6173 7320 666f 7220   Base class for 
-000009d0: 5072 6f6a 6563 740a 0a20 2020 2041 7474  Project..    Att
-000009e0: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
-000009f0: 206e 616d 653a 2054 4244 0a20 2020 2020   name: TBD.     
-00000a00: 2020 2070 726f 6a65 6374 5f64 6972 3a20     project_dir: 
-00000a10: 5442 440a 2020 2020 2020 2020 7265 6164  TBD.        read
-00000a20: 5f6f 6e6c 793a 2054 4244 0a20 2020 2072  _only: TBD.    r
-00000a30: 2600 0000 da0b 7072 6f6a 6563 745f 6469  &.....project_di
-00000a40: 7246 722a 0000 004e 2908 7216 0000 0072  rFr*...N).r....r
-00000a50: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
-00000a60: 0000 0072 1b00 0000 722a 0000 0072 2b00  ...r....r*...r+.
-00000a70: 0000 721c 0000 0072 1c00 0000 721c 0000  ..r....r....r...
-00000a80: 0072 1d00 0000 7230 0000 0062 0000 0073  .r....r0...b...s
-00000a90: 0800 0000 0a01 0409 0801 0801 7230 0000  ............r0..
-00000aa0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000ab0: 0000 0400 0000 4000 0000 735a 0000 0065  ......@...sZ...e
-00000ac0: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
-00000ad0: 0519 0065 0664 023c 0065 0764 0364 0464  ...e.d.<.e.d.d.d
-00000ae0: 058d 0265 0864 0383 0183 015a 0965 0764  ...e.d.....Z.e.d
-00000af0: 0664 0464 058d 0265 0864 0683 0183 015a  .d.d...e.d.....Z
-00000b00: 0a65 0764 0264 0464 058d 0265 0864 0283  .e.d.d.d...e.d..
-00000b10: 0183 015a 0b64 0753 0029 0872 0b00 0000  ...Z.d.S.).r....
-00000b20: 7228 0000 00da 1464 6566 6175 6c74 5f64  r(.....default_d
-00000b30: 6174 6173 6574 5f6e 616d 6572 2600 0000  ataset_namer&...
-00000b40: 5472 1e00 0000 7231 0000 004e 290c 7216  Tr....r1...N).r.
-00000b50: 0000 0072 1700 0000 7218 0000 0072 3200  ...r....r....r2.
-00000b60: 0000 7205 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00000b70: 0072 0700 0000 720a 0000 0072 2c00 0000  .r....r....r,...
-00000b80: da0c 5f70 726f 6a65 6374 5f64 6972 5a15  .._project_dirZ.
-00000b90: 5f64 6566 6175 6c74 5f64 6174 6173 6574  _default_dataset
-00000ba0: 5f6e 616d 6572 1c00 0000 721c 0000 0072  _namer....r....r
-00000bb0: 1c00 0000 721d 0000 0072 0b00 0000 7100  ....r....r....q.
-00000bc0: 0000 7314 0000 000a 0110 0314 010a 0106  ..s.............
-00000bd0: ff04 0302 0104 ff04 0206 fe72 0b00 0000  ...........r....
-00000be0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000bf0: 0003 0000 0040 0000 0073 2600 0000 6500  .....@...s&...e.
-00000c00: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
-00000c10: 6700 5a05 6506 6507 1900 6504 6402 3c00  g.Z.e.e...e.d.<.
-00000c20: 6403 5300 2904 720c 0000 0072 2200 0000  d.S.).r....r"...
-00000c30: da0c 6461 7461 7365 745f 6c69 7374 4e29  ..dataset_listN)
-00000c40: 0872 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000c50: 7224 0000 0072 1b00 0000 7234 0000 0072  r$...r....r4...r
-00000c60: 0400 0000 7210 0000 0072 1c00 0000 721c  ....r....r....r.
-00000c70: 0000 0072 1c00 0000 721d 0000 0072 0c00  ...r....r....r..
-00000c80: 0000 7e00 0000 7304 0000 000a 0108 0172  ..~...s........r
-00000c90: 0c00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000ca0: 0000 0000 0004 0000 0040 0000 0073 5a00  .........@...sZ.
-00000cb0: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-00000cc0: 1900 6505 6401 3c00 6503 6504 1900 6505  ..e.d.<.e.e...e.
-00000cd0: 6402 3c00 6503 6506 1900 6505 6403 3c00  d.<.e.e...e.d.<.
-00000ce0: 6507 6401 6404 6405 8d02 6508 6401 8301  e.d.d.d...e.d...
-00000cf0: 8301 5a09 6507 6402 6404 6405 8d02 6508  ..Z.e.d.d.d...e.
-00000d00: 6402 8301 8301 5a0a 6406 5300 2907 720d  d.....Z.d.S.).r.
-00000d10: 0000 0072 2600 0000 7231 0000 0072 2a00  ...r&...r1...r*.
-00000d20: 0000 5472 1e00 0000 4e29 0b72 1600 0000  ..Tr....N).r....
-00000d30: 7217 0000 0072 1800 0000 7205 0000 0072  r....r....r....r
-00000d40: 1a00 0000 721b 0000 0072 2b00 0000 7207  ....r....r+...r.
-00000d50: 0000 0072 0a00 0000 722c 0000 0072 3300  ...r....r,...r3.
-00000d60: 0000 721c 0000 0072 1c00 0000 721c 0000  ..r....r....r...
-00000d70: 0072 1d00 0000 720d 0000 0083 0000 0073  .r....r........s
-00000d80: 0e00 0000 0a01 0c01 0c01 0c03 1401 0a01  ................
-00000d90: 06ff 720d 0000 004e 2919 da06 7479 7069  ..r....N)...typi
-00000da0: 6e67 7202 0000 0072 0300 0000 7204 0000  ngr....r....r...
-00000db0: 0072 0500 0000 da08 7079 6461 6e74 6963  .r......pydantic
-00000dc0: 7206 0000 0072 0700 0000 da08 7371 6c6d  r....r......sqlm
-00000dd0: 6f64 656c 7208 0000 00da 0b5f 7661 6c69  odelr......_vali
-00000de0: 6461 746f 7273 720a 0000 00da 075f 5f61  datorsr......__a
-00000df0: 6c6c 5f5f 7214 0000 0072 1100 0000 7213  ll__r....r....r.
-00000e00: 0000 0072 1200 0000 7225 0000 0072 0e00  ...r....r%...r..
-00000e10: 0000 720f 0000 0072 1000 0000 7230 0000  ..r....r....r0..
-00000e20: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000e30: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
-00000e40: 1d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000e50: 0000 7328 0000 000c 010c 010c 010c 020c  ..s(............
-00000e60: 010c 010c 020c 0304 1010 0810 0510 0510  ................
-00000e70: 0810 1110 0a10 0610 0a10 0f10 0d10 05    ...............
+00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6405 6c03 6d06 5a06 0100 6406 6407 6c07  d.l.m.Z...d.d.l.
+00000070: 6d08 5a08 0100 6406 6408 6c07 6d09 5a09  m.Z...d.d.l.m.Z.
+00000080: 0100 6409 5a0a 4700 640a 640b 8400 640b  ..d.Z.G.d.d...d.
+00000090: 6504 8303 5a0b 4700 640c 640d 8400 640d  e...Z.G.d.d...d.
+000000a0: 650b 8303 5a0c 4700 640e 640f 8400 640f  e...Z.G.d.d...d.
+000000b0: 650b 8303 5a0d 4700 6410 6411 8400 6411  e...Z.G.d.d...d.
+000000c0: 650b 8303 5a0e 4700 6412 6413 8400 6413  e...Z.G.d.d...d.
+000000d0: 6504 8303 5a0f 4700 6414 6415 8400 6415  e...Z.G.d.d...d.
+000000e0: 650f 8303 5a10 4700 6416 6417 8400 6417  e...Z.G.d.d...d.
+000000f0: 650f 8303 5a11 4700 6418 6419 8400 6419  e...Z.G.d.d...d.
+00000100: 650f 8303 5a12 4700 641a 641b 8400 641b  e...Z.G.d.d...d.
+00000110: 6504 8303 5a13 4700 641c 641d 8400 641d  e...Z.G.d.d...d.
+00000120: 6513 8303 5a14 4700 641e 641f 8400 641f  e...Z.G.d.d...d.
+00000130: 6513 8303 5a15 4700 6420 6421 8400 6421  e...Z.G.d d!..d!
+00000140: 6513 8303 5a16 6422 5300 2923 e900 0000  e...Z.d"S.)#....
+00000150: 0029 01da 0341 6e79 2901 da08 4f70 7469  .)...Any)...Opti
+00000160: 6f6e 616c 2901 da09 4261 7365 4d6f 6465  onal)...BaseMode
+00000170: 6c29 01da 0546 6965 6c64 2901 da09 7661  l)...Field)...va
+00000180: 6c69 6461 746f 72e9 0100 0000 2901 da11  lidator.....)...
+00000190: 7661 6c5f 6162 736f 6c75 7465 5f70 6174  val_absolute_pat
+000001a0: 6829 01da 0676 616c 7374 7229 09da 0d50  h)...valstr)...P
+000001b0: 726f 6a65 6374 4372 6561 7465 da0b 5072  rojectCreate..Pr
+000001c0: 6f6a 6563 7452 6561 64da 0d50 726f 6a65  ojectRead..Proje
+000001d0: 6374 5570 6461 7465 da0d 4461 7461 7365  ctUpdate..Datase
+000001e0: 7455 7064 6174 65da 0d44 6174 6173 6574  tUpdate..Dataset
+000001f0: 4372 6561 7465 da0b 4461 7461 7365 7452  Create..DatasetR
+00000200: 6561 64da 0e52 6573 6f75 7263 6543 7265  ead..ResourceCre
+00000210: 6174 65da 0c52 6573 6f75 7263 6552 6561  ate..ResourceRea
+00000220: 64da 0e52 6573 6f75 7263 6555 7064 6174  d..ResourceUpdat
+00000230: 6563 0000 0000 0000 0000 0000 0000 0000  ec..............
+00000240: 0000 0300 0000 4000 0000 731a 0000 0065  ......@...s....e
+00000250: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
+00000260: 0564 023c 0064 0353 0029 04da 0d5f 5265  .d.<.d.S.)..._Re
+00000270: 736f 7572 6365 4261 7365 7a21 0a20 2020  sourceBasez!.   
+00000280: 2042 6173 6520 636c 6173 7320 666f 7220   Base class for 
+00000290: 5265 736f 7572 6365 0a20 2020 20da 0470  Resource.    ..p
+000002a0: 6174 684e 2906 da08 5f5f 6e61 6d65 5f5f  athN)...__name__
+000002b0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+000002c0: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+000002d0: 635f 5fda 0373 7472 da0f 5f5f 616e 6e6f  c__..str..__anno
+000002e0: 7461 7469 6f6e 735f 5fa9 0072 1b00 0000  tations__..r....
+000002f0: 721b 0000 00fa 3f2f 686f 6d65 2f74 6f6d  r.....?/home/tom
+00000300: 6d61 736f 2f46 7261 6374 616c 2f66 7261  maso/Fractal/fra
+00000310: 6374 616c 2f66 7261 6374 616c 2f63 6f6d  ctal/fractal/com
+00000320: 6d6f 6e2f 7363 6865 6d61 732f 7072 6f6a  mon/schemas/proj
+00000330: 6563 742e 7079 7213 0000 001c 0000 0073  ect.pyr........s
+00000340: 0600 0000 0a00 0401 0c04 7213 0000 0063  ..........r....c
+00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000360: 0400 0000 4000 0000 f320 0000 0065 005a  ....@.... ...e.Z
+00000370: 0164 005a 0265 0364 0164 0264 038d 0265  .d.Z.e.d.d.d...e
+00000380: 0464 0183 0183 015a 0564 0453 0029 0572  .d.....Z.d.S.).r
+00000390: 1000 0000 7214 0000 0054 a901 da0b 616c  ....r....T....al
+000003a0: 6c6f 775f 7265 7573 654e a906 7215 0000  low_reuseN..r...
+000003b0: 0072 1600 0000 7217 0000 0072 0600 0000  .r....r....r....
+000003c0: 7208 0000 00da 055f 7061 7468 721b 0000  r......_pathr...
+000003d0: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+000003e0: 7210 0000 0024 0000 00f3 0400 0000 0800  r....$..........
+000003f0: 1802 7210 0000 0063 0000 0000 0000 0000  ..r....c........
+00000400: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
+00000410: 721d 0000 0029 0572 1200 0000 7214 0000  r....).r....r...
+00000420: 0054 721e 0000 004e 7220 0000 0072 1b00  .Tr....Nr ...r..
+00000430: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00000440: 0072 1200 0000 2900 0000 7222 0000 0072  .r....)...r"...r
+00000450: 1200 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000460: 0000 0000 0003 0000 0040 0000 0073 1e00  .........@...s..
+00000470: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
+00000480: 6401 3c00 6503 6504 6402 3c00 6403 5300  d.<.e.e.d.<.d.S.
+00000490: 2904 7211 0000 00da 0269 64da 0a64 6174  ).r......id..dat
+000004a0: 6173 6574 5f69 644e 2905 7215 0000 0072  aset_idN).r....r
+000004b0: 1600 0000 7217 0000 00da 0369 6e74 721a  ....r......intr.
+000004c0: 0000 0072 1b00 0000 721b 0000 0072 1b00  ...r....r....r..
+000004d0: 0000 721c 0000 0072 1100 0000 2e00 0000  ..r....r........
+000004e0: 7306 0000 000a 0008 010c 0172 1100 0000  s..........r....
+000004f0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000500: 0003 0000 0040 0000 0073 4c00 0000 6500  .....@...sL...e.
+00000510: 5a01 6400 5a02 5500 6401 5a03 6504 6505  Z.d.Z.U.d.Z.e.e.
+00000520: 6402 3c00 6506 6504 1900 6505 6403 3c00  d.<.e.e...e.d.<.
+00000530: 6507 6900 6404 8d01 5a08 6509 6504 650a  e.i.d...Z.e.e.e.
+00000540: 6602 1900 6505 6405 3c00 6406 5a0b 650c  f...e.d.<.d.Z.e.
+00000550: 6505 6407 3c00 6408 5300 2909 da0c 5f44  e.d.<.d.S.)..._D
+00000560: 6174 6173 6574 4261 7365 7a7e 0a20 2020  atasetBasez~.   
+00000570: 2042 6173 6520 636c 6173 7320 666f 7220   Base class for 
+00000580: 4461 7461 7365 740a 0a20 2020 2041 7474  Dataset..    Att
+00000590: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
+000005a0: 206e 616d 653a 2054 4244 0a20 2020 2020   name: TBD.     
+000005b0: 2020 2074 7970 653a 2054 4244 0a20 2020     type: TBD.   
+000005c0: 2020 2020 206d 6574 613a 2054 4244 0a20       meta: TBD. 
+000005d0: 2020 2020 2020 2072 6561 645f 6f6e 6c79         read_only
+000005e0: 3a20 5442 440a 2020 2020 da04 6e61 6d65  : TBD.    ..name
+000005f0: da04 7479 7065 2901 da07 6465 6661 756c  ..type)...defaul
+00000600: 74da 046d 6574 6146 da09 7265 6164 5f6f  t..metaF..read_o
+00000610: 6e6c 794e 290d 7215 0000 0072 1600 0000  nlyN).r....r....
+00000620: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+00000630: 1a00 0000 7203 0000 0072 0500 0000 722a  ....r....r....r*
+00000640: 0000 00da 0464 6963 7472 0200 0000 722b  .....dictr....r+
+00000650: 0000 00da 0462 6f6f 6c72 1b00 0000 721b  .....boolr....r.
+00000660: 0000 0072 1b00 0000 721c 0000 0072 2600  ...r....r....r&.
+00000670: 0000 3600 0000 730c 0000 000a 0004 0108  ..6...s.........
+00000680: 0a0c 011a 0110 0172 2600 0000 6300 0000  .......r&...c...
+00000690: 0000 0000 0000 0000 0000 0000 0004 0000  ................
+000006a0: 0040 0000 0073 6600 0000 6500 5a01 6400  .@...sf...e.Z.d.
+000006b0: 5a02 5500 6503 6504 1900 6505 6401 3c00  Z.U.e.e...e.d.<.
+000006c0: 6402 5a06 6503 6507 6504 6508 6602 1900  d.Z.e.e.e.e.f...
+000006d0: 1900 6505 6403 3c00 6503 6509 1900 6505  ..e.d.<.e.e...e.
+000006e0: 6404 3c00 650a 6401 6405 6406 8d02 650b  d.<.e.d.d.d...e.
+000006f0: 6401 8301 8301 5a0c 650a 6407 6405 6406  d.....Z.e.d.d.d.
+00000700: 8d02 650b 6407 8301 8301 5a0d 6402 5300  ..e.d.....Z.d.S.
+00000710: 2908 720d 0000 0072 2700 0000 4e72 2a00  ).r....r'...Nr*.
+00000720: 0000 722b 0000 0054 721e 0000 0072 2800  ..r+...Tr....r(.
+00000730: 0000 290e 7215 0000 0072 1600 0000 7217  ..).r....r....r.
+00000740: 0000 0072 0300 0000 7219 0000 0072 1a00  ...r....r....r..
+00000750: 0000 722a 0000 0072 2c00 0000 7202 0000  ..r*...r,...r...
+00000760: 0072 2d00 0000 7206 0000 0072 0900 0000  .r-...r....r....
+00000770: da05 5f6e 616d 65da 055f 7479 7065 721b  .._name.._typer.
+00000780: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
+00000790: 0000 720d 0000 0047 0000 0073 0c00 0000  ..r....G...s....
+000007a0: 0a00 0c01 1801 0c01 1403 1801 720d 0000  ............r...
+000007b0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000007c0: 0000 0400 0000 4000 0000 7334 0000 0065  ......@...s4...e
+000007d0: 005a 0164 005a 0265 0364 0164 0264 038d  .Z.d.Z.e.d.d.d..
+000007e0: 0265 0464 0183 0183 015a 0565 0364 0464  .e.d.....Z.e.d.d
+000007f0: 0264 038d 0265 0464 0483 0183 015a 0664  .d...e.d.....Z.d
+00000800: 0553 0029 0672 0e00 0000 7227 0000 0054  .S.).r....r'...T
+00000810: 721e 0000 0072 2800 0000 4e29 0772 1500  r....r(...N).r..
+00000820: 0000 7216 0000 0072 1700 0000 7206 0000  ..r....r....r...
+00000830: 0072 0900 0000 722e 0000 0072 2f00 0000  .r....r....r/...
+00000840: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
+00000850: 1c00 0000 720e 0000 0051 0000 0073 0600  ....r....Q...s..
+00000860: 0000 0800 1402 1801 720e 0000 0063 0000  ........r....c..
+00000870: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00000880: 0000 4000 0000 7332 0000 0065 005a 0164  ..@...s2...e.Z.d
+00000890: 005a 0255 0065 0365 0464 013c 0065 0565  .Z.U.e.e.d.<.e.e
+000008a0: 0619 0065 0464 023c 0065 0365 0464 033c  ...e.d.<.e.e.d.<
+000008b0: 0065 0765 0464 043c 0064 0553 0029 0672  .e.e.d.<.d.S.).r
+000008c0: 0f00 0000 7223 0000 00da 0d72 6573 6f75  ....r#.....resou
+000008d0: 7263 655f 6c69 7374 da0a 7072 6f6a 6563  rce_list..projec
+000008e0: 745f 6964 722b 0000 004e 2908 7215 0000  t_idr+...N).r...
+000008f0: 0072 1600 0000 7217 0000 0072 2500 0000  .r....r....r%...
+00000900: 721a 0000 00da 046c 6973 7472 1100 0000  r......listr....
+00000910: 722d 0000 0072 1b00 0000 721b 0000 0072  r-...r....r....r
+00000920: 1b00 0000 721c 0000 0072 0f00 0000 5700  ....r....r....W.
+00000930: 0000 730a 0000 000a 0008 010c 0108 010c  ..s.............
+00000940: 0172 0f00 0000 6300 0000 0000 0000 0000  .r....c.........
+00000950: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00000960: 2600 0000 6500 5a01 6400 5a02 5500 6401  &...e.Z.d.Z.U.d.
+00000970: 5a03 6504 6505 6402 3c00 6403 5a06 6507  Z.e.e.d.<.d.Z.e.
+00000980: 6505 6404 3c00 6405 5300 2906 da0c 5f50  e.d.<.d.S.)..._P
+00000990: 726f 6a65 6374 4261 7365 7a5a 0a20 2020  rojectBasezZ.   
+000009a0: 2042 6173 6520 636c 6173 7320 666f 7220   Base class for 
+000009b0: 5072 6f6a 6563 740a 0a20 2020 2041 7474  Project..    Att
+000009c0: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
+000009d0: 206e 616d 653a 2054 4244 0a20 2020 2020   name: TBD.     
+000009e0: 2020 2072 6561 645f 6f6e 6c79 3a20 5442     read_only: TB
+000009f0: 440a 2020 2020 7227 0000 0046 722b 0000  D.    r'...Fr+..
+00000a00: 004e 2908 7215 0000 0072 1600 0000 7217  .N).r....r....r.
+00000a10: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
+00000a20: 0000 722b 0000 0072 2d00 0000 721b 0000  ..r+...r-...r...
+00000a30: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00000a40: 7233 0000 0061 0000 0073 0800 0000 0a00  r3...a...s......
+00000a50: 0401 0808 1001 7233 0000 0063 0000 0000  ......r3...c....
+00000a60: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00000a70: 4000 0000 7346 0000 0065 005a 0164 005a  @...sF...e.Z.d.Z
+00000a80: 0255 0064 015a 0365 0465 0519 0065 0664  .U.d.Z.e.e...e.d
+00000a90: 023c 0065 0764 0364 0464 058d 0265 0864  .<.e.d.d.d...e.d
+00000aa0: 0383 0183 015a 0965 0764 0264 0464 058d  .....Z.e.d.d.d..
+00000ab0: 0265 0864 0283 0183 015a 0a64 0653 0029  .e.d.....Z.d.S.)
+00000ac0: 0772 0a00 0000 7229 0000 00da 1464 6566  .r....r).....def
+00000ad0: 6175 6c74 5f64 6174 6173 6574 5f6e 616d  ault_dataset_nam
+00000ae0: 6572 2700 0000 5472 1e00 0000 4e29 0b72  er'...Tr....N).r
+00000af0: 1500 0000 7216 0000 0072 1700 0000 7234  ....r....r....r4
+00000b00: 0000 0072 0300 0000 7219 0000 0072 1a00  ...r....r....r..
+00000b10: 0000 7206 0000 0072 0900 0000 722e 0000  ..r....r....r...
+00000b20: 00da 155f 6465 6661 756c 745f 6461 7461  ..._default_data
+00000b30: 7365 745f 6e61 6d65 721b 0000 0072 1b00  set_namer....r..
+00000b40: 0000 721b 0000 0072 1c00 0000 720a 0000  ..r....r....r...
+00000b50: 006e 0000 0073 1000 0000 0a00 1001 1403  .n...s..........
+00000b60: 0201 0401 04ff 0602 08fe 720a 0000 0063  ..........r....c
+00000b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b80: 0300 0000 4000 0000 7326 0000 0065 005a  ....@...s&...e.Z
+00000b90: 0164 005a 0255 0065 0365 0464 013c 0067  .d.Z.U.e.e.d.<.g
+00000ba0: 005a 0565 0665 0719 0065 0464 023c 0064  .Z.e.e...e.d.<.d
+00000bb0: 0353 0029 0472 0b00 0000 7223 0000 00da  .S.).r....r#....
+00000bc0: 0c64 6174 6173 6574 5f6c 6973 744e 2908  .dataset_listN).
+00000bd0: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000be0: 2500 0000 721a 0000 0072 3600 0000 7232  %...r....r6...r2
+00000bf0: 0000 0072 0f00 0000 721b 0000 0072 1b00  ...r....r....r..
+00000c00: 0000 721b 0000 0072 1c00 0000 720b 0000  ..r....r....r...
+00000c10: 0078 0000 0073 0600 0000 0a00 0801 1401  .x...s..........
+00000c20: 720b 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000c30: 0000 0000 0000 0400 0000 4000 0000 733a  ..........@...s:
+00000c40: 0000 0065 005a 0164 005a 0255 0065 0365  ...e.Z.d.Z.U.e.e
+00000c50: 0419 0065 0564 013c 0065 0365 0619 0065  ...e.d.<.e.e...e
+00000c60: 0564 023c 0065 0764 0164 0364 048d 0265  .d.<.e.d.d.d...e
+00000c70: 0864 0183 0183 015a 0964 0553 0029 0672  .d.....Z.d.S.).r
+00000c80: 0c00 0000 7227 0000 0072 2b00 0000 5472  ....r'...r+...Tr
+00000c90: 1e00 0000 4e29 0a72 1500 0000 7216 0000  ....N).r....r...
+00000ca0: 0072 1700 0000 7203 0000 0072 1900 0000  .r....r....r....
+00000cb0: 721a 0000 0072 2d00 0000 7206 0000 0072  r....r-...r....r
+00000cc0: 0900 0000 722e 0000 0072 1b00 0000 721b  ....r....r....r.
+00000cd0: 0000 0072 1b00 0000 721c 0000 0072 0c00  ...r....r....r..
+00000ce0: 0000 7d00 0000 7308 0000 000a 000c 010c  ..}...s.........
+00000cf0: 0118 0372 0c00 0000 4e29 17da 0674 7970  ...r....N)...typ
+00000d00: 696e 6772 0200 0000 7203 0000 00da 0870  ingr....r......p
+00000d10: 7964 616e 7469 6372 0400 0000 7205 0000  ydanticr....r...
+00000d20: 0072 0600 0000 da0b 5f76 616c 6964 6174  .r......_validat
+00000d30: 6f72 7372 0800 0000 7209 0000 00da 075f  orsr....r......_
+00000d40: 5f61 6c6c 5f5f 7213 0000 0072 1000 0000  _all__r....r....
+00000d50: 7212 0000 0072 1100 0000 7226 0000 0072  r....r....r&...r
+00000d60: 0d00 0000 720e 0000 0072 0f00 0000 7233  ....r....r....r3
+00000d70: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
+00000d80: 0000 721b 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+00000d90: 0072 1c00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000da0: 0100 0000 7328 0000 000c 000c 010c 020c  ....s(..........
+00000db0: 010c 010c 020c 0104 0310 1010 0810 0510  ................
+00000dc0: 0510 0810 1110 0a10 0610 0a10 0d10 0a14  ................
+00000dd0: 05                                       .
```

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/state.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar  6 14:07:44 2023 UTC, .py size: 695 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b0f3 0564 b702 0000  o..........d....
+00000000: 610d 0d0a 0000 0000 b0f3 0564 b702 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c01 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c01 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c05 6d06 5a06 0100 6406 5a07 4700  d.l.m.Z...d.Z.G.
 00000070: 6407 6408 8400 6408 6506 8303 5a08 4700  d.d...d.e...Z.G.
@@ -41,35 +41,35 @@
 00000280: da03 7374 7272 0a00 0000 2902 da04 7365  ..strr....)...se
 00000290: 6c66 da01 64a9 0072 0f00 0000 fa3d 2f68  lf..d..r.....=/h
 000002a0: 6f6d 652f 746f 6d6d 6173 6f2f 4672 6163  ome/tommaso/Frac
 000002b0: 7461 6c2f 6672 6163 7461 6c2f 6672 6163  tal/fractal/frac
 000002c0: 7461 6c2f 636f 6d6d 6f6e 2f73 6368 656d  tal/common/schem
 000002d0: 6173 2f73 7461 7465 2e70 79da 0e73 616e  as/state.py..san
 000002e0: 6974 6973 6564 5f64 6963 741c 0000 0073  itised_dict....s
-000002f0: 0600 0000 0804 0e01 0401 7a19 5f53 7461  ..........z._Sta
+000002f0: 0600 0000 0004 0801 0e01 7a19 5f53 7461  ..........z._Sta
 00000300: 7465 4261 7365 2e73 616e 6974 6973 6564  teBase.sanitised
 00000310: 5f64 6963 744e 290a da08 5f5f 6e61 6d65  _dictN)...__name
 00000320: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
 00000330: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
 00000340: 646f 635f 5f72 0400 0000 720c 0000 0072  doc__r....r....r
 00000350: 0300 0000 da0f 5f5f 616e 6e6f 7461 7469  ......__annotati
 00000360: 6f6e 735f 5f72 0200 0000 7211 0000 0072  ons__r....r....r
 00000370: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-00000380: 0000 0072 0700 0000 0f00 0000 730a 0000  ...r........s...
-00000390: 000a 0004 0110 0908 010c 0272 0700 0000  ...........r....
-000003a0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000003b0: 0003 0000 0040 0000 0073 1a00 0000 6500  .....@...s....e.
-000003c0: 5a01 6400 5a02 5500 6503 6504 1900 6505  Z.d.Z.U.e.e...e.
-000003d0: 6401 3c00 6402 5300 2903 7208 0000 00da  d.<.d.S.).r.....
-000003e0: 0269 644e 2906 7212 0000 0072 1300 0000  .idN).r....r....
-000003f0: 7214 0000 0072 0500 0000 da03 696e 7472  r....r......intr
-00000400: 1600 0000 720f 0000 0072 0f00 0000 720f  ....r....r....r.
-00000410: 0000 0072 1000 0000 7208 0000 0025 0000  ...r....r....%..
-00000420: 0073 0400 0000 0a00 1001 7208 0000 004e  .s........r....N
-00000430: 290a 7202 0000 00da 0674 7970 696e 6772  ).r......typingr
-00000440: 0300 0000 7204 0000 0072 0500 0000 da08  ....r....r......
-00000450: 7371 6c6d 6f64 656c 7206 0000 00da 075f  sqlmodelr......_
-00000460: 5f61 6c6c 5f5f 7207 0000 0072 0800 0000  _all__r....r....
-00000470: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00000480: 1000 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000490: 0000 7310 0000 000c 000c 010c 010c 010c  ..s.............
-000004a0: 0204 0310 0614 16                        .......
+00000380: 0000 0072 0700 0000 0f00 0000 7308 0000  ...r........s...
+00000390: 000a 0104 0910 0108 0272 0700 0000 6300  .........r....c.
+000003a0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+000003b0: 0000 0040 0000 0073 1a00 0000 6500 5a01  ...@...s....e.Z.
+000003c0: 6400 5a02 5500 6503 6504 1900 6505 6401  d.Z.U.e.e...e.d.
+000003d0: 3c00 6402 5300 2903 7208 0000 00da 0269  <.d.S.).r......i
+000003e0: 644e 2906 7212 0000 0072 1300 0000 7214  dN).r....r....r.
+000003f0: 0000 0072 0500 0000 da03 696e 7472 1600  ...r......intr..
+00000400: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+00000410: 0072 1000 0000 7208 0000 0025 0000 0073  .r....r....%...s
+00000420: 0200 0000 0a01 7208 0000 004e 290a 7202  ......r....N).r.
+00000430: 0000 00da 0674 7970 696e 6772 0300 0000  .....typingr....
+00000440: 7204 0000 0072 0500 0000 da08 7371 6c6d  r....r......sqlm
+00000450: 6f64 656c 7206 0000 00da 075f 5f61 6c6c  odelr......__all
+00000460: 5f5f 7207 0000 0072 0800 0000 720f 0000  __r....r....r...
+00000470: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
+00000480: da08 3c6d 6f64 756c 653e 0100 0000 730e  ..<module>....s.
+00000490: 0000 000c 010c 010c 010c 020c 0304 0610  ................
+000004a0: 16                                       .
```

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/task.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 20:00:26 2023 UTC, .py size: 4323 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5aa6 5a64 e310 0000  o.......Z.Zd....
+00000000: 610d 0d0a 0000 0000 15f0 0564 8411 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c02 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c02 6d06 5a06 0100 6400 6406 6c02  d.l.m.Z...d.d.l.
 00000070: 6d07 5a07 0100 6400 6407 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
@@ -89,221 +89,225 @@
 00000580: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
 00000590: 6f63 5f5f da03 7374 72da 0f5f 5f61 6e6e  oc__..str..__ann
 000005a0: 6f74 6174 696f 6e73 5f5f a900 721e 0000  otations__..r...
 000005b0: 0072 1e00 0000 fa3c 2f68 6f6d 652f 746f  .r.....</home/to
 000005c0: 6d6d 6173 6f2f 4672 6163 7461 6c2f 6672  mmaso/Fractal/fr
 000005d0: 6163 7461 6c2f 6672 6163 7461 6c2f 636f  actal/fractal/co
 000005e0: 6d6d 6f6e 2f73 6368 656d 6173 2f74 6173  mmon/schemas/tas
-000005f0: 6b2e 7079 7215 0000 001a 0000 0073 0800  k.pyr........s..
-00000600: 0000 0a00 0401 0817 0c01 7215 0000 0063  ..........r....c
-00000610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000620: 0400 0000 4000 0000 73d6 0000 0065 005a  ....@...s....e.Z
-00000630: 0164 005a 0255 0065 0365 0419 0065 0564  .d.Z.U.e.e...e.d
-00000640: 013c 0065 0365 0419 0065 0564 023c 0065  .<.e.e...e.d.<.e
-00000650: 0365 0419 0065 0564 033c 0065 0365 0419  .e...e.d.<.e.e..
-00000660: 0065 0564 043c 0065 0365 0419 0065 0564  .e.d.<.e.e...e.d
-00000670: 053c 0065 0365 0665 0465 0766 0219 0019  .<.e.e.e.e.f....
-00000680: 0065 0564 063c 0065 0365 0665 0465 0766  .e.d.<.e.e.e.e.f
-00000690: 0219 0019 0065 0564 073c 0065 0864 0164  .....e.d.<.e.d.d
-000006a0: 0864 098d 0265 0964 0183 0183 015a 0a65  .d...e.d.....Z.e
-000006b0: 0864 0264 0864 098d 0265 0964 0283 0183  .d.d.d...e.d....
-000006c0: 015a 0b65 0864 0364 0864 098d 0265 0964  .Z.e.d.d.d...e.d
-000006d0: 0383 0183 015a 0c65 0864 0464 0864 098d  .....Z.e.d.d.d..
-000006e0: 0265 0964 0483 0183 015a 0d65 0864 0564  .e.d.....Z.e.d.d
-000006f0: 0864 098d 0265 0964 0583 0183 015a 0e64  .d...e.d.....Z.d
-00000700: 0a53 0029 0b72 0f00 0000 7216 0000 00da  .S.).r....r.....
-00000710: 0a69 6e70 7574 5f74 7970 65da 0b6f 7574  .input_type..out
-00000720: 7075 745f 7479 7065 da07 636f 6d6d 616e  put_type..comman
-00000730: 6472 1700 0000 da0c 6465 6661 756c 745f  dr......default_
-00000740: 6172 6773 da04 6d65 7461 54a9 01da 0b61  args..metaT....a
-00000750: 6c6c 6f77 5f72 6575 7365 4e29 0f72 1800  llow_reuseN).r..
-00000760: 0000 7219 0000 0072 1a00 0000 7207 0000  ..r....r....r...
-00000770: 0072 1c00 0000 721d 0000 0072 0400 0000  .r....r....r....
-00000780: 7203 0000 0072 0900 0000 720d 0000 00da  r....r....r.....
-00000790: 055f 6e61 6d65 da0b 5f69 6e70 7574 5f74  ._name.._input_t
-000007a0: 7970 65da 0c5f 6f75 7470 7574 5f74 7970  ype.._output_typ
-000007b0: 65da 085f 636f 6d6d 616e 64da 075f 736f  e.._command.._so
-000007c0: 7572 6365 721e 0000 0072 1e00 0000 721e  urcer....r....r.
-000007d0: 0000 0072 1f00 0000 720f 0000 0036 0000  ...r....r....6..
-000007e0: 0073 2200 0000 0a00 0c01 0c01 0c01 0c01  .s".............
-000007f0: 0c01 1401 1401 1403 0a01 0601 04ff 0a03  ................
-00000800: 0601 04ff 1403 1801 720f 0000 0063 0000  ........r....c..
-00000810: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00000820: 0000 4000 0000 7334 0000 0065 005a 0164  ..@...s4...e.Z.d
-00000830: 005a 0265 0364 0164 0264 038d 0265 0464  .Z.e.d.d.d...e.d
-00000840: 0183 0183 015a 0565 0364 0464 0264 038d  .....Z.e.d.d.d..
-00000850: 0265 0464 0483 0183 015a 0664 0553 0029  .e.d.....Z.d.S.)
-00000860: 0672 1100 0000 7216 0000 0054 7225 0000  .r....r....Tr%..
-00000870: 0072 1700 0000 4e29 0772 1800 0000 7219  .r....N).r....r.
-00000880: 0000 0072 1a00 0000 7209 0000 0072 0d00  ...r....r....r..
-00000890: 0000 7227 0000 0072 2b00 0000 721e 0000  ..r'...r+...r...
-000008a0: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-000008b0: 7211 0000 004b 0000 0073 0600 0000 0800  r....K...s......
-000008c0: 1401 1801 7211 0000 0063 0000 0000 0000  ....r....c......
-000008d0: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-000008e0: 0000 f30c 0000 0065 005a 0164 005a 0264  .......e.Z.d.Z.d
-000008f0: 0153 0029 0272 1200 0000 4ea9 0372 1800  .S.).r....N..r..
-00000900: 0000 7219 0000 0072 1a00 0000 721e 0000  ..r....r....r...
-00000910: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00000920: 7212 0000 0050 0000 00f3 0400 0000 0800  r....P..........
-00000930: 0401 7212 0000 0063 0000 0000 0000 0000  ..r....c........
-00000940: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-00000950: 736a 0000 0065 005a 0164 005a 0255 0065  sj...e.Z.d.Z.U.e
-00000960: 0365 0464 013c 0065 0565 0464 023c 0065  .e.d.<.e.e.d.<.e
-00000970: 0565 0464 033c 0065 0565 0464 043c 0065  .e.d.<.e.e.d.<.e
-00000980: 0669 0064 058d 015a 0765 0865 0965 0565  .i.d...Z.e.e.e.e
-00000990: 0a66 0219 0019 0065 0464 063c 0065 0669  .f.....e.d.<.e.i
-000009a0: 0064 058d 015a 0b65 0865 0965 0565 0a66  .d...Z.e.e.e.e.f
-000009b0: 0219 0019 0065 0464 073c 0064 0853 0029  .....e.d.<.d.S.)
-000009c0: 0972 1000 0000 da02 6964 7222 0000 0072  .r......idr"...r
-000009d0: 2000 0000 7221 0000 00a9 01da 0764 6566   ...r!.......def
-000009e0: 6175 6c74 7223 0000 0072 2400 0000 4e29  aultr#...r$...N)
-000009f0: 0c72 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000a00: da03 696e 7472 1d00 0000 721c 0000 0072  ..intr....r....r
-00000a10: 0a00 0000 7223 0000 0072 0700 0000 7204  ....r#...r....r.
-00000a20: 0000 0072 0300 0000 7224 0000 0072 1e00  ...r....r$...r..
-00000a30: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00000a40: 0072 1000 0000 5400 0000 730e 0000 000a  .r....T...s.....
-00000a50: 0008 0108 0108 0108 011e 0122 0172 1000  ...........".r..
-00000a60: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000a70: 0000 0004 0000 0040 0000 0073 c600 0000  .......@...s....
-00000a80: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
-00000a90: 3c00 6503 6504 6402 3c00 6503 6504 6403  <.e.e.d.<.e.e.d.
-00000aa0: 3c00 6505 6900 6404 8d01 5a06 6507 6508  <.e.i.d...Z.e.e.
-00000ab0: 6503 6509 6602 1900 1900 6504 6405 3c00  e.e.f.....e.d.<.
-00000ac0: 6505 6900 6404 8d01 5a0a 6507 6508 6503  e.i.d...Z.e.e.e.
-00000ad0: 6509 6602 1900 1900 6504 6406 3c00 650b  e.f.....e.d.<.e.
-00000ae0: 6407 6408 6409 8d02 650c 6407 8301 8301  d.d.d...e.d.....
-00000af0: 5a0d 650b 6402 6408 6409 8d02 650c 6402  Z.e.d.d.d...e.d.
-00000b00: 8301 8301 5a0e 650b 6403 6408 6409 8d02  ....Z.e.d.d.d...
-00000b10: 650c 6403 8301 8301 5a0f 650b 6401 6408  e.d.....Z.e.d.d.
-00000b20: 6409 8d02 650c 6401 8301 8301 5a10 650b  d...e.d.....Z.e.
-00000b30: 640a 6408 6409 8d02 650c 640a 8301 8301  d.d.d...e.d.....
-00000b40: 5a11 640b 5300 290c 720e 0000 0072 2200  Z.d.S.).r....r".
-00000b50: 0000 7220 0000 0072 2100 0000 7230 0000  ..r ...r!...r0..
-00000b60: 0072 2300 0000 7224 0000 0072 1600 0000  .r#...r$...r....
-00000b70: 5472 2500 0000 7217 0000 004e 2912 7218  Tr%...r....N).r.
-00000b80: 0000 0072 1900 0000 721a 0000 0072 1c00  ...r....r....r..
-00000b90: 0000 721d 0000 0072 0a00 0000 7223 0000  ..r....r....r#..
-00000ba0: 0072 0700 0000 7204 0000 0072 0300 0000  .r....r....r....
-00000bb0: 7224 0000 0072 0900 0000 720d 0000 0072  r$...r....r....r
-00000bc0: 2700 0000 7228 0000 0072 2900 0000 722a  '...r(...r)...r*
-00000bd0: 0000 0072 2b00 0000 721e 0000 0072 1e00  ...r+...r....r..
-00000be0: 0000 721e 0000 0072 1f00 0000 720e 0000  ..r....r....r...
-00000bf0: 005d 0000 0073 1e00 0000 0a00 0801 0801  .]...s..........
-00000c00: 0801 1e01 1e01 1403 0a01 0601 04ff 0a03  ................
-00000c10: 0601 04ff 1403 1801 720e 0000 0063 0000  ........r....c..
-00000c20: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-00000c30: 0000 4000 0000 722c 0000 0029 02da 105f  ..@...r,...)..._
+000005f0: 6b2e 7079 7215 0000 001a 0000 0073 0600  k.pyr........s..
+00000600: 0000 0a01 0417 0801 7215 0000 0063 0000  ........r....c..
+00000610: 0000 0000 0000 0000 0000 0000 0000 0400  ................
+00000620: 0000 4000 0000 73d6 0000 0065 005a 0164  ..@...s....e.Z.d
+00000630: 005a 0255 0065 0365 0419 0065 0564 013c  .Z.U.e.e...e.d.<
+00000640: 0065 0365 0419 0065 0564 023c 0065 0365  .e.e...e.d.<.e.e
+00000650: 0419 0065 0564 033c 0065 0365 0419 0065  ...e.d.<.e.e...e
+00000660: 0564 043c 0065 0365 0419 0065 0564 053c  .d.<.e.e...e.d.<
+00000670: 0065 0365 0665 0465 0766 0219 0019 0065  .e.e.e.e.f.....e
+00000680: 0564 063c 0065 0365 0665 0465 0766 0219  .d.<.e.e.e.e.f..
+00000690: 0019 0065 0564 073c 0065 0864 0164 0864  ...e.d.<.e.d.d.d
+000006a0: 098d 0265 0964 0183 0183 015a 0a65 0864  ...e.d.....Z.e.d
+000006b0: 0264 0864 098d 0265 0964 0283 0183 015a  .d.d...e.d.....Z
+000006c0: 0b65 0864 0364 0864 098d 0265 0964 0383  .e.d.d.d...e.d..
+000006d0: 0183 015a 0c65 0864 0464 0864 098d 0265  ...Z.e.d.d.d...e
+000006e0: 0964 0483 0183 015a 0d65 0864 0564 0864  .d.....Z.e.d.d.d
+000006f0: 098d 0265 0964 0583 0183 015a 0e64 0a53  ...e.d.....Z.d.S
+00000700: 0029 0b72 0f00 0000 7216 0000 00da 0a69  .).r....r......i
+00000710: 6e70 7574 5f74 7970 65da 0b6f 7574 7075  nput_type..outpu
+00000720: 745f 7479 7065 da07 636f 6d6d 616e 6472  t_type..commandr
+00000730: 1700 0000 da0c 6465 6661 756c 745f 6172  ......default_ar
+00000740: 6773 da04 6d65 7461 54a9 01da 0b61 6c6c  gs..metaT....all
+00000750: 6f77 5f72 6575 7365 4e29 0f72 1800 0000  ow_reuseN).r....
+00000760: 7219 0000 0072 1a00 0000 7207 0000 0072  r....r....r....r
+00000770: 1c00 0000 721d 0000 0072 0400 0000 7203  ....r....r....r.
+00000780: 0000 0072 0900 0000 720d 0000 00da 055f  ...r....r......_
+00000790: 6e61 6d65 da0b 5f69 6e70 7574 5f74 7970  name.._input_typ
+000007a0: 65da 0c5f 6f75 7470 7574 5f74 7970 65da  e.._output_type.
+000007b0: 085f 636f 6d6d 616e 64da 075f 736f 7572  ._command.._sour
+000007c0: 6365 721e 0000 0072 1e00 0000 721e 0000  cer....r....r...
+000007d0: 0072 1f00 0000 720f 0000 0036 0000 0073  .r....r....6...s
+000007e0: 2000 0000 0a01 0c01 0c01 0c01 0c01 0c01   ...............
+000007f0: 1401 1403 1401 0a01 06ff 0403 0a01 06ff  ................
+00000800: 0403 1401 720f 0000 0063 0000 0000 0000  ....r....c......
+00000810: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+00000820: 0000 7334 0000 0065 005a 0164 005a 0265  ..s4...e.Z.d.Z.e
+00000830: 0364 0164 0264 038d 0265 0464 0183 0183  .d.d.d...e.d....
+00000840: 015a 0565 0364 0464 0264 038d 0265 0464  .Z.e.d.d.d...e.d
+00000850: 0483 0183 015a 0664 0553 0029 0672 1100  .....Z.d.S.).r..
+00000860: 0000 7216 0000 0054 7225 0000 0072 1700  ..r....Tr%...r..
+00000870: 0000 4e29 0772 1800 0000 7219 0000 0072  ..N).r....r....r
+00000880: 1a00 0000 7209 0000 0072 0d00 0000 7227  ....r....r....r'
+00000890: 0000 0072 2b00 0000 721e 0000 0072 1e00  ...r+...r....r..
+000008a0: 0000 721e 0000 0072 1f00 0000 7211 0000  ..r....r....r...
+000008b0: 004b 0000 0073 0400 0000 0801 1401 7211  .K...s........r.
+000008c0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000008d0: 0000 0000 0100 0000 4000 0000 730c 0000  ........@...s...
+000008e0: 0065 005a 0164 005a 0264 0153 0029 0272  .e.Z.d.Z.d.S.).r
+000008f0: 1200 0000 4ea9 0372 1800 0000 7219 0000  ....N..r....r...
+00000900: 0072 1a00 0000 721e 0000 0072 1e00 0000  .r....r....r....
+00000910: 721e 0000 0072 1f00 0000 7212 0000 0050  r....r....r....P
+00000920: 0000 0073 0200 0000 0801 7212 0000 0063  ...s......r....c
+00000930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000940: 0400 0000 4000 0000 736a 0000 0065 005a  ....@...sj...e.Z
+00000950: 0164 005a 0255 0065 0365 0464 013c 0065  .d.Z.U.e.e.d.<.e
+00000960: 0565 0464 023c 0065 0565 0464 033c 0065  .e.d.<.e.e.d.<.e
+00000970: 0565 0464 043c 0065 0669 0064 058d 015a  .e.d.<.e.i.d...Z
+00000980: 0765 0865 0965 0565 0a66 0219 0019 0065  .e.e.e.e.f.....e
+00000990: 0464 063c 0065 0669 0064 058d 015a 0b65  .d.<.e.i.d...Z.e
+000009a0: 0865 0965 0565 0a66 0219 0019 0065 0464  .e.e.e.f.....e.d
+000009b0: 073c 0064 0853 0029 0972 1000 0000 da02  .<.d.S.).r......
+000009c0: 6964 7222 0000 0072 2000 0000 7221 0000  idr"...r ...r!..
+000009d0: 00a9 01da 0764 6566 6175 6c74 7223 0000  .....defaultr#..
+000009e0: 0072 2400 0000 4e29 0c72 1800 0000 7219  .r$...N).r....r.
+000009f0: 0000 0072 1a00 0000 da03 696e 7472 1d00  ...r......intr..
+00000a00: 0000 721c 0000 0072 0a00 0000 7223 0000  ..r....r....r#..
+00000a10: 0072 0700 0000 7204 0000 0072 0300 0000  .r....r....r....
+00000a20: 7224 0000 0072 1e00 0000 721e 0000 0072  r$...r....r....r
+00000a30: 1e00 0000 721f 0000 0072 1000 0000 5400  ....r....r....T.
+00000a40: 0000 730c 0000 000a 0108 0108 0108 0108  ..s.............
+00000a50: 011e 0172 1000 0000 6300 0000 0000 0000  ...r....c.......
+00000a60: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+00000a70: 0073 c600 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+00000a80: 6503 6504 6401 3c00 6503 6504 6402 3c00  e.e.d.<.e.e.d.<.
+00000a90: 6503 6504 6403 3c00 6505 6900 6404 8d01  e.e.d.<.e.i.d...
+00000aa0: 5a06 6507 6508 6503 6509 6602 1900 1900  Z.e.e.e.e.f.....
+00000ab0: 6504 6405 3c00 6505 6900 6404 8d01 5a0a  e.d.<.e.i.d...Z.
+00000ac0: 6507 6508 6503 6509 6602 1900 1900 6504  e.e.e.e.f.....e.
+00000ad0: 6406 3c00 650b 6407 6408 6409 8d02 650c  d.<.e.d.d.d...e.
+00000ae0: 6407 8301 8301 5a0d 650b 6402 6408 6409  d.....Z.e.d.d.d.
+00000af0: 8d02 650c 6402 8301 8301 5a0e 650b 6403  ..e.d.....Z.e.d.
+00000b00: 6408 6409 8d02 650c 6403 8301 8301 5a0f  d.d...e.d.....Z.
+00000b10: 650b 6401 6408 6409 8d02 650c 6401 8301  e.d.d.d...e.d...
+00000b20: 8301 5a10 650b 640a 6408 6409 8d02 650c  ..Z.e.d.d.d...e.
+00000b30: 640a 8301 8301 5a11 640b 5300 290c 720e  d.....Z.d.S.).r.
+00000b40: 0000 0072 2200 0000 7220 0000 0072 2100  ...r"...r ...r!.
+00000b50: 0000 722e 0000 0072 2300 0000 7224 0000  ..r....r#...r$..
+00000b60: 0072 1600 0000 5472 2500 0000 7217 0000  .r....Tr%...r...
+00000b70: 004e 2912 7218 0000 0072 1900 0000 721a  .N).r....r....r.
+00000b80: 0000 0072 1c00 0000 721d 0000 0072 0a00  ...r....r....r..
+00000b90: 0000 7223 0000 0072 0700 0000 7204 0000  ..r#...r....r...
+00000ba0: 0072 0300 0000 7224 0000 0072 0900 0000  .r....r$...r....
+00000bb0: 720d 0000 0072 2700 0000 7228 0000 0072  r....r'...r(...r
+00000bc0: 2900 0000 722a 0000 0072 2b00 0000 721e  )...r*...r+...r.
+00000bd0: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
+00000be0: 0000 720e 0000 005d 0000 0073 1c00 0000  ..r....]...s....
+00000bf0: 0a01 0801 0801 0801 1e01 1e03 1401 0a01  ................
+00000c00: 06ff 0403 0a01 06ff 0403 1401 720e 0000  ............r...
+00000c10: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000c20: 0000 0100 0000 4000 0000 730c 0000 0065  ......@...s....e
+00000c30: 005a 0164 005a 0264 0153 0029 02da 105f  .Z.d.Z.d.S.)..._
 00000c40: 5461 736b 436f 6c6c 6563 7442 6173 654e  TaskCollectBaseN
-00000c50: 722d 0000 0072 1e00 0000 721e 0000 0072  r-...r....r....r
-00000c60: 1e00 0000 721f 0000 0072 3300 0000 7000  ....r....r3...p.
-00000c70: 0000 722e 0000 0072 3300 0000 6300 0000  ..r....r3...c...
-00000c80: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000c90: 0040 0000 0073 5200 0000 6500 5a01 6400  .@...sR...e.Z.d.
-00000ca0: 5a02 5500 6401 5a03 6504 6505 6402 3c00  Z.U.d.Z.e.e.d.<.
-00000cb0: 6506 6504 1900 6505 6403 3c00 6404 5a07  e.e...e.d.<.d.Z.
-00000cc0: 6506 6504 1900 6505 6405 3c00 6506 6504  e.e...e.d.<.e.e.
-00000cd0: 1900 6505 6406 3c00 6508 6402 8301 6407  ..e.d.<.e.d...d.
-00000ce0: 6408 8400 8301 5a09 6404 5300 2909 7213  d.....Z.d.S.).r.
-00000cf0: 0000 007a 910a 2020 2020 5461 736b 436f  ...z..    TaskCo
-00000d00: 6c6c 6563 7450 6970 2063 6c61 7373 0a0a  llectPip class..
-00000d10: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
-00000d20: 2020 2020 2020 2020 7061 636b 6167 653a          package:
-00000d30: 2054 4244 0a20 2020 2020 2020 2076 6572   TBD.        ver
-00000d40: 7369 6f6e 3a20 5442 440a 2020 2020 2020  sion: TBD.      
-00000d50: 2020 7079 7468 6f6e 5f76 6572 7369 6f6e    python_version
-00000d60: 3a20 5442 440a 2020 2020 2020 2020 7061  : TBD.        pa
-00000d70: 636b 6167 655f 6578 7472 6173 3a20 5442  ckage_extras: TB
-00000d80: 440a 2020 2020 da07 7061 636b 6167 65da  D.    ..package.
-00000d90: 0776 6572 7369 6f6e 4eda 0e70 7974 686f  .versionN..pytho
-00000da0: 6e5f 7665 7273 696f 6eda 0e70 6163 6b61  n_version..packa
-00000db0: 6765 5f65 7874 7261 7363 0200 0000 0000  ge_extrasc......
-00000dc0: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
-00000dd0: 0000 732a 0000 0064 017c 0176 0072 1374  ..s*...d.|.v.r.t
-00000de0: 007c 0183 017d 027c 02a0 01a1 0073 1374  .|...}.|.....s.t
-00000df0: 0264 027c 029b 009d 0283 0182 017c 0153  .d.|.........|.S
-00000e00: 0029 034e fa01 2f7a 1f50 6163 6b61 6765  .).N../z.Package
-00000e10: 2070 6174 6820 6d75 7374 2062 6520 6162   path must be ab
-00000e20: 736f 6c75 7465 3a20 2903 7202 0000 00da  solute: ).r.....
-00000e30: 0b69 735f 6162 736f 6c75 7465 da0a 5661  .is_absolute..Va
-00000e40: 6c75 6545 7272 6f72 2903 da03 636c 73da  lueError)...cls.
-00000e50: 0576 616c 7565 da0c 7061 636b 6167 655f  .value..package_
-00000e60: 7061 7468 721e 0000 0072 1e00 0000 721f  pathr....r....r.
-00000e70: 0000 00da 1570 6163 6b61 6765 5f70 6174  .....package_pat
-00000e80: 685f 6162 736f 6c75 7465 8400 0000 730e  h_absolute....s.
-00000e90: 0000 0008 0208 0108 0102 0108 0104 ff04  ................
-00000ea0: 037a 2454 6173 6b43 6f6c 6c65 6374 5069  .z$TaskCollectPi
-00000eb0: 702e 7061 636b 6167 655f 7061 7468 5f61  p.package_path_a
-00000ec0: 6273 6f6c 7574 6529 0a72 1800 0000 7219  bsolute).r....r.
-00000ed0: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
-00000ee0: 0000 721d 0000 0072 0700 0000 7236 0000  ..r....r....r6..
-00000ef0: 0072 0900 0000 723e 0000 0072 1e00 0000  .r....r>...r....
-00000f00: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00000f10: 1300 0000 7400 0000 7310 0000 000a 0004  ....t...s.......
-00000f20: 0108 0a0c 0110 010c 0106 020e 0172 1300  .............r..
-00000f30: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000f40: 0000 0003 0000 0040 0000 0073 6800 0000  .......@...sh...
-00000f50: 6500 5a01 6400 5a02 5500 6401 5a03 6504  e.Z.d.Z.U.d.Z.e.
-00000f60: 6402 1900 6505 6403 3c00 6506 6505 6404  d...e.d.<.e.e.d.
-00000f70: 3c00 6507 6505 6405 3c00 6508 6700 6406  <.e.e.d.<.e.g.d.
-00000f80: 8d01 5a09 650a 650b 650c 1900 1900 6505  ..Z.e.e.e.....e.
-00000f90: 6407 3c00 650a 6506 1900 6505 6408 3c00  d.<.e.e...e.d.<.
-00000fa0: 650a 6506 1900 6505 6409 3c00 640a 640b  e.e...e.d.<.d.d.
-00000fb0: 8400 5a0d 640c 5300 290d 7214 0000 007a  ..Z.d.S.).r....z
-00000fc0: ac0a 2020 2020 5461 736b 436f 6c6c 6563  ..    TaskCollec
-00000fd0: 7453 7461 7475 7320 636c 6173 730a 0a20  tStatus class.. 
-00000fe0: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
-00000ff0: 2020 2020 2020 2073 7461 7475 733a 2054         status: T
-00001000: 4244 0a20 2020 2020 2020 2070 6163 6b61  BD.        packa
-00001010: 6765 3a20 5442 440a 2020 2020 2020 2020  ge: TBD.        
-00001020: 7665 6e76 5f70 6174 683a 2054 4244 0a20  venv_path: TBD. 
-00001030: 2020 2020 2020 2074 6173 6b5f 6c69 7374         task_list
-00001040: 3a20 5442 440a 2020 2020 2020 2020 6c6f  : TBD.        lo
-00001050: 673a 2054 4244 0a20 2020 2020 2020 2069  g: TBD.        i
-00001060: 6e66 6f3a 2054 4244 0a20 2020 2029 05da  nfo: TBD.    )..
-00001070: 0770 656e 6469 6e67 da0a 696e 7374 616c  .pending..instal
-00001080: 6c69 6e67 da0a 636f 6c6c 6563 7469 6e67  ling..collecting
-00001090: da04 6661 696c da02 4f4b da06 7374 6174  ..fail..OK..stat
-000010a0: 7573 7234 0000 00da 0976 656e 765f 7061  usr4.....venv_pa
-000010b0: 7468 7230 0000 00da 0974 6173 6b5f 6c69  thr0.....task_li
-000010c0: 7374 da03 6c6f 67da 0469 6e66 6f63 0100  st..log..infoc..
-000010d0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000010e0: 0000 4300 0000 731a 0000 007c 00a0 00a1  ..C...s....|....
-000010f0: 007d 0174 017c 006a 0283 017c 0164 013c  .}.t.|.j...|.d.<
-00001100: 007c 0153 0029 027a 510a 2020 2020 2020  .|.S.).zQ.      
-00001110: 2020 5265 7475 726e 2060 7365 6c66 2e64    Return `self.d
-00001120: 6963 7428 2960 2061 6674 6572 2063 6173  ict()` after cas
-00001130: 7469 6e67 2060 7365 6c66 2e76 656e 765f  ting `self.venv_
-00001140: 7061 7468 6020 746f 2061 2073 7472 696e  path` to a strin
-00001150: 670a 2020 2020 2020 2020 7245 0000 0029  g.        rE...)
-00001160: 03da 0464 6963 7472 1c00 0000 7245 0000  ...dictr....rE..
-00001170: 0029 02da 0473 656c 66da 0164 721e 0000  .)...self..dr...
-00001180: 0072 1e00 0000 721f 0000 00da 0e73 616e  .r....r......san
-00001190: 6974 6973 6564 5f64 6963 74a3 0000 0073  itised_dict....s
-000011a0: 0600 0000 0804 0e01 0401 7a20 5461 736b  ..........z Task
-000011b0: 436f 6c6c 6563 7453 7461 7475 732e 7361  CollectStatus.sa
-000011c0: 6e69 7469 7365 645f 6469 6374 4e29 0e72  nitised_dictN).r
-000011d0: 1800 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
-000011e0: 0000 0072 0600 0000 721d 0000 0072 1c00  ...r....r....r..
-000011f0: 0000 7202 0000 0072 0a00 0000 7246 0000  ..r....r....rF..
-00001200: 0072 0700 0000 7205 0000 0072 1000 0000  .r....r....r....
-00001210: 724c 0000 0072 1e00 0000 721e 0000 0072  rL...r....r....r
-00001220: 1e00 0000 721f 0000 0072 1400 0000 8f00  ....r....r......
-00001230: 0000 7312 0000 000a 0004 010c 0c08 0108  ..s.............
-00001240: 011a 010c 010c 010c 0272 1400 0000 4e29  .........r....N)
-00001250: 1ada 0770 6174 686c 6962 7202 0000 00da  ...pathlibr.....
-00001260: 0674 7970 696e 6772 0300 0000 7204 0000  .typingr....r...
-00001270: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
-00001280: da08 7079 6461 6e74 6963 7208 0000 0072  ..pydanticr....r
-00001290: 0900 0000 da08 7371 6c6d 6f64 656c 720a  ......sqlmodelr.
-000012a0: 0000 0072 0b00 0000 da0b 5f76 616c 6964  ...r......_valid
-000012b0: 6174 6f72 7372 0d00 0000 da07 5f5f 616c  atorsr......__al
-000012c0: 6c5f 5f72 1500 0000 720f 0000 0072 1100  l__r....r....r..
-000012d0: 0000 7212 0000 0072 1000 0000 720e 0000  ..r....r....r...
-000012e0: 0072 3300 0000 7213 0000 0072 1400 0000  .r3...r....r....
-000012f0: 721e 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
-00001300: 1f00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00001310: 0000 732a 0000 000c 000c 010c 010c 010c  ..s*............
-00001320: 010c 010c 020c 010c 010c 010c 0204 0210  ................
-00001330: 0b10 1c10 1510 0510 0410 0910 1310 0414  ................
-00001340: 1b                                       .
+00000c50: 722c 0000 0072 1e00 0000 721e 0000 0072  r,...r....r....r
+00000c60: 1e00 0000 721f 0000 0072 3100 0000 7000  ....r....r1...p.
+00000c70: 0000 7302 0000 0008 0172 3100 0000 6300  ..s......r1...c.
+00000c80: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000c90: 0000 0040 0000 0073 5200 0000 6500 5a01  ...@...sR...e.Z.
+00000ca0: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
+00000cb0: 3c00 6506 6504 1900 6505 6403 3c00 6404  <.e.e...e.d.<.d.
+00000cc0: 5a07 6506 6504 1900 6505 6405 3c00 6506  Z.e.e...e.d.<.e.
+00000cd0: 6504 1900 6505 6406 3c00 6508 6402 8301  e...e.d.<.e.d...
+00000ce0: 6407 6408 8400 8301 5a09 6404 5300 2909  d.d.....Z.d.S.).
+00000cf0: 7213 0000 007a 910a 2020 2020 5461 736b  r....z..    Task
+00000d00: 436f 6c6c 6563 7450 6970 2063 6c61 7373  CollectPip class
+00000d10: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
+00000d20: 3a0a 2020 2020 2020 2020 7061 636b 6167  :.        packag
+00000d30: 653a 2054 4244 0a20 2020 2020 2020 2076  e: TBD.        v
+00000d40: 6572 7369 6f6e 3a20 5442 440a 2020 2020  ersion: TBD.    
+00000d50: 2020 2020 7079 7468 6f6e 5f76 6572 7369      python_versi
+00000d60: 6f6e 3a20 5442 440a 2020 2020 2020 2020  on: TBD.        
+00000d70: 7061 636b 6167 655f 6578 7472 6173 3a20  package_extras: 
+00000d80: 5442 440a 2020 2020 da07 7061 636b 6167  TBD.    ..packag
+00000d90: 65da 0776 6572 7369 6f6e 4eda 0e70 7974  e..versionN..pyt
+00000da0: 686f 6e5f 7665 7273 696f 6e5a 0e70 6163  hon_versionZ.pac
+00000db0: 6b61 6765 5f65 7874 7261 7363 0200 0000  kage_extrasc....
+00000dc0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00000dd0: 4300 0000 7340 0000 0064 017c 0176 0072  C...s@...d.|.v.r
+00000de0: 3c74 007c 0183 017d 027c 02a0 01a1 0073  <t.|...}.|.....s
+00000df0: 2674 0264 027c 029b 009d 0283 0182 017c  &t.d.|.........|
+00000e00: 02a0 03a1 0073 3c74 0264 037c 029b 009d  .....s<t.d.|....
+00000e10: 0283 0182 017c 0153 0029 044e fa01 2f7a  .....|.S.).N../z
+00000e20: 1f50 6163 6b61 6765 2070 6174 6820 6d75  .Package path mu
+00000e30: 7374 2062 6520 6162 736f 6c75 7465 3a20  st be absolute: 
+00000e40: 7a1d 5061 636b 6167 6520 6669 6c65 2064  z.Package file d
+00000e50: 6f65 7320 6e6f 7420 6578 6973 743a 2029  oes not exist: )
+00000e60: 0472 0200 0000 da0b 6973 5f61 6273 6f6c  .r......is_absol
+00000e70: 7574 65da 0a56 616c 7565 4572 726f 72da  ute..ValueError.
+00000e80: 0665 7869 7374 7329 03da 0363 6c73 da05  .exists)...cls..
+00000e90: 7661 6c75 65da 0c70 6163 6b61 6765 5f70  value..package_p
+00000ea0: 6174 6872 1e00 0000 721e 0000 0072 1f00  athr....r....r..
+00000eb0: 0000 da15 7061 636b 6167 655f 7061 7468  ....package_path
+00000ec0: 5f61 6273 6f6c 7574 6584 0000 0073 1600  _absolute....s..
+00000ed0: 0000 0002 0801 0801 0801 0201 08ff 0403  ................
+00000ee0: 0801 0201 08ff 0403 7a24 5461 736b 436f  ........z$TaskCo
+00000ef0: 6c6c 6563 7450 6970 2e70 6163 6b61 6765  llectPip.package
+00000f00: 5f70 6174 685f 6162 736f 6c75 7465 290a  _path_absolute).
+00000f10: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00000f20: 1b00 0000 721c 0000 0072 1d00 0000 7207  ....r....r....r.
+00000f30: 0000 0072 3400 0000 7209 0000 0072 3c00  ...r4...r....r<.
+00000f40: 0000 721e 0000 0072 1e00 0000 721e 0000  ..r....r....r...
+00000f50: 0072 1f00 0000 7213 0000 0074 0000 0073  .r....r....t...s
+00000f60: 0e00 0000 0a01 040a 0801 0c01 1001 0c02  ................
+00000f70: 0601 7213 0000 0063 0000 0000 0000 0000  ..r....c........
+00000f80: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000f90: 7368 0000 0065 005a 0164 005a 0255 0064  sh...e.Z.d.Z.U.d
+00000fa0: 015a 0365 0464 0219 0065 0564 033c 0065  .Z.e.d...e.d.<.e
+00000fb0: 0665 0564 043c 0065 0765 0564 053c 0065  .e.d.<.e.e.d.<.e
+00000fc0: 0867 0064 068d 015a 0965 0a65 0b65 0c19  .g.d...Z.e.e.e..
+00000fd0: 0019 0065 0564 073c 0065 0a65 0619 0065  ...e.d.<.e.e...e
+00000fe0: 0564 083c 0065 0a65 0619 0065 0564 093c  .d.<.e.e...e.d.<
+00000ff0: 0064 0a64 0b84 005a 0d64 0c53 0029 0d72  .d.d...Z.d.S.).r
+00001000: 1400 0000 7aac 0a20 2020 2054 6173 6b43  ....z..    TaskC
+00001010: 6f6c 6c65 6374 5374 6174 7573 2063 6c61  ollectStatus cla
+00001020: 7373 0a0a 2020 2020 4174 7472 6962 7574  ss..    Attribut
+00001030: 6573 3a0a 2020 2020 2020 2020 7374 6174  es:.        stat
+00001040: 7573 3a20 5442 440a 2020 2020 2020 2020  us: TBD.        
+00001050: 7061 636b 6167 653a 2054 4244 0a20 2020  package: TBD.   
+00001060: 2020 2020 2076 656e 765f 7061 7468 3a20       venv_path: 
+00001070: 5442 440a 2020 2020 2020 2020 7461 736b  TBD.        task
+00001080: 5f6c 6973 743a 2054 4244 0a20 2020 2020  _list: TBD.     
+00001090: 2020 206c 6f67 3a20 5442 440a 2020 2020     log: TBD.    
+000010a0: 2020 2020 696e 666f 3a20 5442 440a 2020      info: TBD.  
+000010b0: 2020 2905 da07 7065 6e64 696e 675a 0a69    )...pendingZ.i
+000010c0: 6e73 7461 6c6c 696e 675a 0a63 6f6c 6c65  nstallingZ.colle
+000010d0: 6374 696e 675a 0466 6169 6cda 024f 4bda  ctingZ.fail..OK.
+000010e0: 0673 7461 7475 7372 3200 0000 da09 7665  .statusr2.....ve
+000010f0: 6e76 5f70 6174 6872 2e00 0000 da09 7461  nv_pathr......ta
+00001100: 736b 5f6c 6973 74da 036c 6f67 da04 696e  sk_list..log..in
+00001110: 666f 6301 0000 0000 0000 0000 0000 0002  foc.............
+00001120: 0000 0003 0000 0043 0000 0073 1a00 0000  .......C...s....
+00001130: 7c00 a000 a100 7d01 7401 7c00 6a02 8301  |.....}.t.|.j...
+00001140: 7c01 6401 3c00 7c01 5300 2902 7a51 0a20  |.d.<.|.S.).zQ. 
+00001150: 2020 2020 2020 2052 6574 7572 6e20 6073         Return `s
+00001160: 656c 662e 6469 6374 2829 6020 6166 7465  elf.dict()` afte
+00001170: 7220 6361 7374 696e 6720 6073 656c 662e  r casting `self.
+00001180: 7665 6e76 5f70 6174 6860 2074 6f20 6120  venv_path` to a 
+00001190: 7374 7269 6e67 0a20 2020 2020 2020 2072  string.        r
+000011a0: 4000 0000 2903 da04 6469 6374 721c 0000  @...)...dictr...
+000011b0: 0072 4000 0000 2902 da04 7365 6c66 da01  .r@...)...self..
+000011c0: 6472 1e00 0000 721e 0000 0072 1f00 0000  dr....r....r....
+000011d0: da0e 7361 6e69 7469 7365 645f 6469 6374  ..sanitised_dict
+000011e0: a700 0000 7306 0000 0000 0408 010e 017a  ....s..........z
+000011f0: 2054 6173 6b43 6f6c 6c65 6374 5374 6174   TaskCollectStat
+00001200: 7573 2e73 616e 6974 6973 6564 5f64 6963  us.sanitised_dic
+00001210: 744e 290e 7218 0000 0072 1900 0000 721a  tN).r....r....r.
+00001220: 0000 0072 1b00 0000 7206 0000 0072 1d00  ...r....r....r..
+00001230: 0000 721c 0000 0072 0200 0000 720a 0000  ..r....r....r...
+00001240: 0072 4100 0000 7207 0000 0072 0500 0000  .rA...r....r....
+00001250: 7210 0000 0072 4700 0000 721e 0000 0072  r....rG...r....r
+00001260: 1e00 0000 721e 0000 0072 1f00 0000 7214  ....r....r....r.
+00001270: 0000 0093 0000 0073 1000 0000 0a01 040c  .......s........
+00001280: 0c01 0801 0801 1a01 0c01 0c02 7214 0000  ............r...
+00001290: 004e 291a da07 7061 7468 6c69 6272 0200  .N)...pathlibr..
+000012a0: 0000 da06 7479 7069 6e67 7203 0000 0072  ....typingr....r
+000012b0: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
+000012c0: 0000 00da 0870 7964 616e 7469 6372 0800  .....pydanticr..
+000012d0: 0000 7209 0000 00da 0873 716c 6d6f 6465  ..r......sqlmode
+000012e0: 6c72 0a00 0000 720b 0000 00da 0b5f 7661  lr....r......_va
+000012f0: 6c69 6461 746f 7273 720d 0000 00da 075f  lidatorsr......_
+00001300: 5f61 6c6c 5f5f 7215 0000 0072 0f00 0000  _all__r....r....
+00001310: 7211 0000 0072 1200 0000 7210 0000 0072  r....r....r....r
+00001320: 0e00 0000 7231 0000 0072 1300 0000 7214  ....r1...r....r.
+00001330: 0000 0072 1e00 0000 721e 0000 0072 1e00  ...r....r....r..
+00001340: 0000 721f 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00001350: 3e01 0000 0073 2800 0000 0c01 0c01 0c01  >....s(.........
+00001360: 0c01 0c01 0c02 0c01 0c01 0c01 0c02 0c02  ................
+00001370: 040b 101c 1015 1005 1004 1009 1013 1004  ................
+00001380: 101f                                     ..
```

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/user.cpython-39.pyc` & `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/user.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_client-1.3.0a1/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 11 16:07:56 2023 UTC, .py size: 2502 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,247 +1,243 @@
-00000000: 6f0d 0d0a 0000 0000 dc12 5d64 c609 0000  o.........]d....
+00000000: 6f0d 0d0a 0000 0000 5b56 7064 9909 0000  o.......[Vpd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4c01 0000 6400  .....@...sL...d.
+00000020: 0004 0000 0040 0000 0073 3401 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
-00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c05 6d06 5a06 0100 6400 6406 6c07  d.l.m.Z...d.d.l.
-00000070: 6d08 5a08 0100 6407 6408 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000080: 0100 6407 6409 6c09 6d0b 5a0b 0100 6407  ..d.d.l.m.Z...d.
-00000090: 640a 6c0c 6d0d 5a0d 0100 6407 640b 6c0c  d.l.m.Z...d.d.l.
-000000a0: 6d0e 5a0e 0100 6407 640c 6c0c 6d0f 5a0f  m.Z...d.d.l.m.Z.
-000000b0: 0100 640d 5a10 4700 640e 640f 8400 640f  ..d.Z.G.d.d...d.
-000000c0: 6508 8303 5a11 4700 6410 6411 8400 6411  e...Z.G.d.d...d.
-000000d0: 6511 8303 5a12 4700 6412 6413 8400 6413  e...Z.G.d.d...d.
-000000e0: 6511 8303 5a13 4700 6414 6415 8400 6415  e...Z.G.d.d...d.
-000000f0: 6511 8303 5a14 4700 6416 6417 8400 6417  e...Z.G.d.d...d.
-00000100: 6511 8303 5a15 4700 6418 6419 8400 6419  e...Z.G.d.d...d.
-00000110: 6511 8303 5a16 4700 641a 641b 8400 641b  e...Z.G.d.d...d.
-00000120: 6508 8303 5a17 4700 641c 641d 8400 641d  e...Z.G.d.d...d.
-00000130: 6517 8303 5a18 4700 641e 641f 8400 641f  e...Z.G.d.d...d.
-00000140: 6517 8303 5a19 4700 6420 6421 8400 6421  e...Z.G.d d!..d!
-00000150: 6517 8303 5a1a 4700 6422 6423 8400 6423  e...Z.G.d"d#..d#
-00000160: 6517 8303 5a1b 4700 6424 6425 8400 6425  e...Z.G.d$d%..d%
-00000170: 6517 8303 5a1c 6426 5300 2927 e900 0000  e...Z.d&S.)'....
-00000180: 0029 01da 0341 6e79 2901 da04 4469 6374  .)...Any)...Dict
-00000190: 2901 da04 4c69 7374 2901 da08 4f70 7469  )...List)...Opti
-000001a0: 6f6e 616c 2901 da09 7661 6c69 6461 746f  onal)...validato
-000001b0: 7229 01da 0853 514c 4d6f 6465 6ce9 0100  r)...SQLModel...
-000001c0: 0000 2901 da06 7661 6c69 6e74 2901 da06  ..)...valint)...
-000001d0: 7661 6c73 7472 2901 da0a 5461 736b 4578  valstr)...TaskEx
-000001e0: 706f 7274 2901 da0a 5461 736b 496d 706f  port)...TaskImpo
-000001f0: 7274 2901 da08 5461 736b 5265 6164 290a  rt)...TaskRead).
-00000200: da0e 576f 726b 666c 6f77 4372 6561 7465  ..WorkflowCreate
-00000210: da0c 576f 726b 666c 6f77 5265 6164 da0e  ..WorkflowRead..
-00000220: 576f 726b 666c 6f77 5570 6461 7465 da0e  WorkflowUpdate..
-00000230: 576f 726b 666c 6f77 496d 706f 7274 da0e  WorkflowImport..
-00000240: 576f 726b 666c 6f77 4578 706f 7274 da12  WorkflowExport..
-00000250: 576f 726b 666c 6f77 5461 736b 4372 6561  WorkflowTaskCrea
-00000260: 7465 da12 576f 726b 666c 6f77 5461 736b  te..WorkflowTask
-00000270: 496d 706f 7274 da12 576f 726b 666c 6f77  Import..Workflow
-00000280: 5461 736b 4578 706f 7274 da10 576f 726b  TaskExport..Work
-00000290: 666c 6f77 5461 736b 5265 6164 da12 576f  flowTaskRead..Wo
-000002a0: 726b 666c 6f77 5461 736b 5570 6461 7465  rkflowTaskUpdate
-000002b0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000002c0: 0004 0000 0040 0000 0073 3e00 0000 6500  .....@...s>...e.
-000002d0: 5a01 6400 5a02 5500 6401 5a03 6504 6505  Z.d.Z.U.d.Z.e.e.
-000002e0: 6506 6507 6602 1900 1900 6508 6402 3c00  e.e.f.....e.d.<.
-000002f0: 6401 5a09 6504 6505 6506 6507 6602 1900  d.Z.e.e.e.e.f...
-00000300: 1900 6508 6403 3c00 6401 5300 2904 da11  ..e.d.<.d.S.)...
-00000310: 5f57 6f72 6b66 6c6f 7754 6173 6b42 6173  _WorkflowTaskBas
-00000320: 654e da04 6d65 7461 da04 6172 6773 290a  eN..meta..args).
-00000330: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000340: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000350: 6d65 5f5f 7219 0000 0072 0500 0000 7203  me__r....r....r.
-00000360: 0000 00da 0373 7472 7202 0000 00da 0f5f  .....strr......_
-00000370: 5f61 6e6e 6f74 6174 696f 6e73 5f5f 721a  _annotations__r.
-00000380: 0000 00a9 0072 2000 0000 7220 0000 00fa  .....r ...r ....
-00000390: 402f 686f 6d65 2f74 6f6d 6d61 736f 2f46  @/home/tommaso/F
-000003a0: 7261 6374 616c 2f66 7261 6374 616c 2f66  ractal/fractal/f
-000003b0: 7261 6374 616c 2f63 6f6d 6d6f 6e2f 7363  ractal/common/sc
-000003c0: 6865 6d61 732f 776f 726b 666c 6f77 2e70  hemas/workflow.p
-000003d0: 7972 1800 0000 1e00 0000 7306 0000 000a  yr........s.....
-000003e0: 0018 021c 0172 1800 0000 6300 0000 0000  .....r....c.....
-000003f0: 0000 0000 0000 0000 0000 0005 0000 0040  ...............@
-00000400: 0000 0073 3200 0000 6500 5a01 6400 5a02  ...s2...e.Z.d.Z.
-00000410: 5500 6503 6504 1900 6505 6401 3c00 6506  U.e.e...e.d.<.e.
-00000420: 6401 6402 6403 8d02 6507 6401 6404 6405  d.d.d...e.d.d.d.
-00000430: 8d02 8301 5a08 6406 5300 2907 7213 0000  ....Z.d.S.).r...
-00000440: 00da 056f 7264 6572 54a9 01da 0b61 6c6c  ...orderT....all
-00000450: 6f77 5f72 6575 7365 7201 0000 0029 01da  ow_reuser....)..
-00000460: 076d 696e 5f76 616c 4e29 0972 1b00 0000  .min_valN).r....
-00000470: 721c 0000 0072 1d00 0000 7205 0000 00da  r....r....r.....
-00000480: 0369 6e74 721f 0000 0072 0600 0000 7209  .intr....r....r.
-00000490: 0000 00da 065f 6f72 6465 7272 2000 0000  ....._orderr ...
-000004a0: 7220 0000 0072 2000 0000 7221 0000 0072  r ...r ...r!...r
-000004b0: 1300 0000 2400 0000 7306 0000 000a 000c  ....$...s.......
-000004c0: 011c 0272 1300 0000 6300 0000 0000 0000  ...r....c.......
-000004d0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-000004e0: 0073 3a00 0000 6500 5a01 6400 5a02 5500  .s:...e.Z.d.Z.U.
-000004f0: 6503 6504 6401 3c00 6505 6503 1900 6504  e.e.d.<.e.e...e.
-00000500: 6402 3c00 6503 6504 6403 3c00 6503 6504  d.<.e.e.d.<.e.e.
-00000510: 6404 3c00 6506 6504 6405 3c00 6406 5300  d.<.e.e.d.<.d.S.
-00000520: 2907 7216 0000 00da 0269 6472 2200 0000  ).r......idr"...
-00000530: da0b 776f 726b 666c 6f77 5f69 64da 0774  ..workflow_id..t
-00000540: 6173 6b5f 6964 da04 7461 736b 4e29 0772  ask_id..taskN).r
-00000550: 1b00 0000 721c 0000 0072 1d00 0000 7226  ....r....r....r&
-00000560: 0000 0072 1f00 0000 7205 0000 0072 0d00  ...r....r....r..
-00000570: 0000 7220 0000 0072 2000 0000 7220 0000  ..r ...r ...r ..
-00000580: 0072 2100 0000 7216 0000 002a 0000 0073  .r!...r....*...s
-00000590: 0c00 0000 0a00 0801 0c01 0801 0801 0c01  ................
-000005a0: 7216 0000 0063 0000 0000 0000 0000 0000  r....c..........
-000005b0: 0000 0000 0000 0300 0000 4000 0000 f316  ..........@.....
-000005c0: 0000 0065 005a 0164 005a 0255 0065 0365  ...e.Z.d.Z.U.e.e
-000005d0: 0464 013c 0064 0253 0029 0372 1400 0000  .d.<.d.S.).r....
-000005e0: 722b 0000 004e 2905 721b 0000 0072 1c00  r+...N).r....r..
-000005f0: 0000 721d 0000 0072 0c00 0000 721f 0000  ..r....r....r...
-00000600: 0072 2000 0000 7220 0000 0072 2000 0000  .r ...r ...r ...
-00000610: 7221 0000 0072 1400 0000 3200 0000 f304  r!...r....2.....
-00000620: 0000 000a 000c 0172 1400 0000 6300 0000  .......r....c...
-00000630: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000640: 0040 0000 0072 2c00 0000 2903 7215 0000  .@...r,...).r...
-00000650: 0072 2b00 0000 4e29 0572 1b00 0000 721c  .r+...N).r....r.
-00000660: 0000 0072 1d00 0000 720b 0000 0072 1f00  ...r....r....r..
-00000670: 0000 7220 0000 0072 2000 0000 7220 0000  ..r ...r ...r ..
-00000680: 0072 2100 0000 7215 0000 0036 0000 0072  .r!...r....6...r
-00000690: 2d00 0000 7215 0000 0063 0000 0000 0000  -...r....c......
-000006a0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-000006b0: 0000 731c 0000 0065 005a 0164 005a 0265  ..s....e.Z.d.Z.e
-000006c0: 0364 0183 0164 0264 0384 0083 015a 0464  .d...d.d.....Z.d
-000006d0: 0453 0029 0572 1700 0000 7219 0000 0063  .S.).r....r....c
-000006e0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000006f0: 0200 0000 4300 0000 7314 0000 0064 017c  ....C...s....d.|
-00000700: 0176 0072 0874 0064 0283 0182 017c 0153  .v.r.t.d.....|.S
-00000710: 0029 034e da15 7061 7261 6c6c 656c 697a  .).N..paralleliz
-00000720: 6174 696f 6e5f 6c65 7665 6c7a 3b4f 7665  ation_levelz;Ove
-00000730: 7272 6964 696e 6720 7461 736b 2070 6172  rriding task par
-00000740: 616c 6c65 6c69 7a61 7469 6f6e 206c 6576  allelization lev
-00000750: 656c 2063 7572 7265 6e74 6c79 206e 6f74  el currently not
-00000760: 2061 6c6c 6f77 6564 2901 da0a 5661 6c75   allowed)...Valu
-00000770: 6545 7272 6f72 2902 da03 636c 73da 016d  eError)...cls..m
-00000780: 7220 0000 0072 2000 0000 7221 0000 00da  r ...r ...r!....
-00000790: 1e63 6865 636b 5f6e 6f5f 7061 7261 6c6c  .check_no_parall
-000007a0: 656c 6973 6174 696f 6e5f 6c65 7665 6c3c  elisation_level<
-000007b0: 0000 0073 0a00 0000 0802 0201 0201 04ff  ...s............
-000007c0: 0403 7a31 576f 726b 666c 6f77 5461 736b  ..z1WorkflowTask
-000007d0: 5570 6461 7465 2e63 6865 636b 5f6e 6f5f  Update.check_no_
-000007e0: 7061 7261 6c6c 656c 6973 6174 696f 6e5f  parallelisation_
-000007f0: 6c65 7665 6c4e 2905 721b 0000 0072 1c00  levelN).r....r..
-00000800: 0000 721d 0000 0072 0600 0000 7232 0000  ..r....r....r2..
-00000810: 0072 2000 0000 7220 0000 0072 2000 0000  .r ...r ...r ...
-00000820: 7221 0000 0072 1700 0000 3a00 0000 7306  r!...r....:...s.
-00000830: 0000 0008 0006 020e 0172 1700 0000 6300  .........r....c.
-00000840: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000850: 0000 0040 0000 0072 2c00 0000 2903 da0d  ...@...r,...)...
-00000860: 5f57 6f72 6b66 6c6f 7742 6173 65da 046e  _WorkflowBase..n
-00000870: 616d 654e 2905 721b 0000 0072 1c00 0000  ameN).r....r....
-00000880: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00000890: 2000 0000 7220 0000 0072 2000 0000 7221   ...r ...r ...r!
-000008a0: 0000 0072 3300 0000 4500 0000 722d 0000  ...r3...E...r-..
-000008b0: 0072 3300 0000 6300 0000 0000 0000 0000  .r3...c.........
-000008c0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000008d0: 2a00 0000 6500 5a01 6400 5a02 5500 6503  *...e.Z.d.Z.U.e.
-000008e0: 6504 6401 3c00 6503 6504 6402 3c00 6505  e.d.<.e.e.d.<.e.
-000008f0: 6506 1900 6504 6403 3c00 6404 5300 2905  e...e.d.<.d.S.).
-00000900: 720f 0000 0072 2800 0000 da0a 7072 6f6a  r....r(.....proj
-00000910: 6563 745f 6964 da09 7461 736b 5f6c 6973  ect_id..task_lis
-00000920: 744e 2907 721b 0000 0072 1c00 0000 721d  tN).r....r....r.
-00000930: 0000 0072 2600 0000 721f 0000 0072 0400  ...r&...r....r..
-00000940: 0000 7216 0000 0072 2000 0000 7220 0000  ..r....r ...r ..
-00000950: 0072 2000 0000 7221 0000 0072 0f00 0000  .r ...r!...r....
-00000960: 4900 0000 7308 0000 000a 0008 0108 0110  I...s...........
-00000970: 0172 0f00 0000 6300 0000 0000 0000 0000  .r....c.........
-00000980: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
-00000990: 2000 0000 6500 5a01 6400 5a02 6503 6401   ...e.Z.d.Z.e.d.
-000009a0: 6402 6403 8d02 6504 6401 8301 8301 5a05  d.d...e.d.....Z.
-000009b0: 6404 5300 2905 720e 0000 0072 3400 0000  d.S.).r....r4...
-000009c0: 5472 2300 0000 4e29 0672 1b00 0000 721c  Tr#...N).r....r.
-000009d0: 0000 0072 1d00 0000 7206 0000 0072 0a00  ...r....r....r..
-000009e0: 0000 da05 5f6e 616d 6572 2000 0000 7220  ...._namer ...r 
-000009f0: 0000 0072 2000 0000 7221 0000 0072 0e00  ...r ...r!...r..
-00000a00: 0000 4f00 0000 7304 0000 0008 0018 0272  ..O...s........r
-00000a10: 0e00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000a20: 0000 0000 0004 0000 0040 0000 0073 4e00  .........@...sN.
-00000a30: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-00000a40: 1900 6505 6401 3c00 6503 6506 6507 1900  ..e.d.<.e.e.e...
-00000a50: 1900 6505 6402 3c00 6508 6401 6403 6404  ..e.d.<.e.d.d.d.
-00000a60: 8d02 6509 6401 8301 8301 5a0a 6508 6402  ..e.d.....Z.e.d.
-00000a70: 8301 6405 6406 8400 8301 5a0b 6407 5300  ..d.d.....Z.d.S.
-00000a80: 2908 7210 0000 0072 3400 0000 da1a 7265  ).r....r4.....re
-00000a90: 6f72 6465 7265 645f 776f 726b 666c 6f77  ordered_workflow
-00000aa0: 7461 736b 5f69 6473 5472 2300 0000 6302  task_idsTr#...c.
-00000ab0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000ac0: 0000 0043 0000 0073 3a00 0000 7400 6401  ...C...s:...t.d.
-00000ad0: 6402 8400 7c01 4400 8301 8301 720d 7401  d...|.D.....r.t.
-00000ae0: 6403 8301 8201 7402 7c01 8301 7402 7403  d.....t.|...t.t.
-00000af0: 7c01 8301 8301 6b03 721b 7401 6404 8301  |.....k.r.t.d...
-00000b00: 8201 7c01 5300 2905 4e63 0100 0000 0000  ..|.S.).Nc......
-00000b10: 0000 0000 0000 0200 0000 0300 0000 7300  ..............s.
-00000b20: 0000 7318 0000 0081 007c 005d 077d 017c  ..s......|.].}.|
-00000b30: 0164 006b 0056 0001 0071 0264 0153 0029  .d.k.V...q.d.S.)
-00000b40: 0272 0100 0000 4e72 2000 0000 2902 da02  .r....Nr ...)...
-00000b50: 2e30 da01 6972 2000 0000 7220 0000 0072  .0..ir ...r ...r
-00000b60: 2100 0000 da09 3c67 656e 6578 7072 3e5d  !.....<genexpr>]
-00000b70: 0000 0073 0400 0000 0280 1600 7a3b 576f  ...s........z;Wo
-00000b80: 726b 666c 6f77 5570 6461 7465 2e63 6865  rkflowUpdate.che
-00000b90: 636b 5f70 6f73 6974 6976 655f 616e 645f  ck_positive_and_
-00000ba0: 756e 6971 7565 2e3c 6c6f 6361 6c73 3e2e  unique.<locals>.
-00000bb0: 3c67 656e 6578 7072 3e7a 2d4e 6567 6174  <genexpr>z-Negat
-00000bc0: 6976 6520 6069 6460 2069 6e20 6072 656f  ive `id` in `reo
-00000bd0: 7264 6572 6564 5f77 6f72 6b66 6c6f 7774  rdered_workflowt
-00000be0: 6173 6b5f 6964 7360 7a2c 6072 656f 7264  ask_ids`z,`reord
-00000bf0: 6572 6564 5f77 6f72 6b66 6c6f 7774 6173  ered_workflowtas
-00000c00: 6b5f 6964 7360 2068 6173 2072 6570 6574  k_ids` has repet
-00000c10: 6974 696f 6e73 2904 da03 616e 7972 2f00  itions)...anyr/.
-00000c20: 0000 da03 6c65 6eda 0373 6574 2902 7230  ....len..set).r0
-00000c30: 0000 00da 0576 616c 7565 7220 0000 0072  .....valuer ...r
-00000c40: 2000 0000 7221 0000 00da 1963 6865 636b   ...r!.....check
-00000c50: 5f70 6f73 6974 6976 655f 616e 645f 756e  _positive_and_un
-00000c60: 6971 7565 5b00 0000 730a 0000 0012 0208  ique[...s.......
-00000c70: 0114 0108 0104 017a 2857 6f72 6b66 6c6f  .......z(Workflo
-00000c80: 7755 7064 6174 652e 6368 6563 6b5f 706f  wUpdate.check_po
-00000c90: 7369 7469 7665 5f61 6e64 5f75 6e69 7175  sitive_and_uniqu
-00000ca0: 654e 290c 721b 0000 0072 1c00 0000 721d  eN).r....r....r.
-00000cb0: 0000 0072 0500 0000 721e 0000 0072 1f00  ...r....r....r..
-00000cc0: 0000 7204 0000 0072 2600 0000 7206 0000  ..r....r&...r...
-00000cd0: 0072 0a00 0000 7237 0000 0072 4000 0000  .r....r7...r@...
-00000ce0: 7220 0000 0072 2000 0000 7220 0000 0072  r ...r ...r ...r
-00000cf0: 2100 0000 7210 0000 0054 0000 0073 0c00  !...r....T...s..
-00000d00: 0000 0a00 0c01 1001 1403 0602 0e01 7210  ..............r.
-00000d10: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000d20: 0000 0000 0400 0000 4000 0000 732e 0000  ........@...s...
-00000d30: 0065 005a 0164 005a 0255 0065 0365 0419  .e.Z.d.Z.U.e.e..
-00000d40: 0065 0564 013c 0065 0664 0264 0364 048d  .e.d.<.e.d.d.d..
-00000d50: 0265 0764 0283 0183 015a 0864 0553 0029  .e.d.....Z.d.S.)
-00000d60: 0672 1100 0000 7236 0000 0072 3400 0000  .r....r6...r4...
-00000d70: 5472 2300 0000 4e29 0972 1b00 0000 721c  Tr#...N).r....r.
-00000d80: 0000 0072 1d00 0000 7204 0000 0072 1400  ...r....r....r..
-00000d90: 0000 721f 0000 0072 0600 0000 720a 0000  ..r....r....r...
-00000da0: 0072 3700 0000 7220 0000 0072 2000 0000  .r7...r ...r ...
-00000db0: 7220 0000 0072 2100 0000 7211 0000 0064  r ...r!...r....d
-00000dc0: 0000 0073 0600 0000 0a00 0c01 1803 7211  ...s..........r.
-00000dd0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000de0: 0000 0000 0300 0000 4000 0000 731a 0000  ........@...s...
-00000df0: 0065 005a 0164 005a 0255 0065 0365 0419  .e.Z.d.Z.U.e.e..
-00000e00: 0065 0564 013c 0064 0253 0029 0372 1200  .e.d.<.d.S.).r..
-00000e10: 0000 7236 0000 004e 2906 721b 0000 0072  ..r6...N).r....r
-00000e20: 1c00 0000 721d 0000 0072 0400 0000 7215  ....r....r....r.
-00000e30: 0000 0072 1f00 0000 7220 0000 0072 2000  ...r....r ...r .
-00000e40: 0000 7220 0000 0072 2100 0000 7212 0000  ..r ...r!...r...
-00000e50: 006b 0000 0073 0400 0000 0a00 1001 7212  .k...s........r.
-00000e60: 0000 004e 291d da06 7479 7069 6e67 7202  ...N)...typingr.
-00000e70: 0000 0072 0300 0000 7204 0000 0072 0500  ...r....r....r..
-00000e80: 0000 da08 7079 6461 6e74 6963 7206 0000  ....pydanticr...
-00000e90: 00da 0873 716c 6d6f 6465 6c72 0700 0000  ...sqlmodelr....
-00000ea0: da0b 5f76 616c 6964 6174 6f72 7372 0900  .._validatorsr..
-00000eb0: 0000 720a 0000 0072 2b00 0000 720b 0000  ..r....r+...r...
-00000ec0: 0072 0c00 0000 720d 0000 00da 075f 5f61  .r....r......__a
-00000ed0: 6c6c 5f5f 7218 0000 0072 1300 0000 7216  ll__r....r....r.
-00000ee0: 0000 0072 1400 0000 7215 0000 0072 1700  ...r....r....r..
-00000ef0: 0000 7233 0000 0072 0f00 0000 720e 0000  ..r3...r....r...
-00000f00: 0072 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
-00000f10: 7220 0000 0072 2000 0000 7220 0000 0072  r ...r ...r ...r
-00000f20: 2100 0000 da08 3c6d 6f64 756c 653e 0100  !.....<module>..
-00000f30: 0000 7330 0000 000c 000c 010c 010c 010c  ..s0............
-00000f40: 020c 010c 020c 010c 010c 010c 0104 0310  ................
-00000f50: 0e10 0610 0610 0810 0410 0410 0b10 0410  ................
-00000f60: 0610 0510 1014 07                        .......
+00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6405  ..d.d.l.m.Z...d.
+00000060: 6406 6c06 6d07 5a07 0100 6405 6407 6c06  d.l.m.Z...d.d.l.
+00000070: 6d08 5a08 0100 6405 6408 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
+00000080: 0100 6405 6409 6c09 6d0b 5a0b 0100 6405  ..d.d.l.m.Z...d.
+00000090: 640a 6c09 6d0c 5a0c 0100 640b 5a0d 4700  d.l.m.Z...d.Z.G.
+000000a0: 640c 640d 8400 640d 6504 8303 5a0e 4700  d.d...d.e...Z.G.
+000000b0: 640e 640f 8400 640f 650e 8303 5a0f 4700  d.d...d.e...Z.G.
+000000c0: 6410 6411 8400 6411 650e 8303 5a10 4700  d.d...d.e...Z.G.
+000000d0: 6412 6413 8400 6413 650e 8303 5a11 4700  d.d...d.e...Z.G.
+000000e0: 6414 6415 8400 6415 650e 8303 5a12 4700  d.d...d.e...Z.G.
+000000f0: 6416 6417 8400 6417 650e 8303 5a13 4700  d.d...d.e...Z.G.
+00000100: 6418 6419 8400 6419 6504 8303 5a14 4700  d.d...d.e...Z.G.
+00000110: 641a 641b 8400 641b 6514 8303 5a15 4700  d.d...d.e...Z.G.
+00000120: 641c 641d 8400 641d 6514 8303 5a16 4700  d.d...d.e...Z.G.
+00000130: 641e 641f 8400 641f 6514 8303 5a17 4700  d.d...d.e...Z.G.
+00000140: 6420 6421 8400 6421 6514 8303 5a18 4700  d d!..d!e...Z.G.
+00000150: 6422 6423 8400 6423 6514 8303 5a19 6424  d"d#..d#e...Z.d$
+00000160: 5300 2925 e900 0000 0029 01da 0341 6e79  S.)%.....)...Any
+00000170: 2901 da08 4f70 7469 6f6e 616c 2901 da09  )...Optional)...
+00000180: 4261 7365 4d6f 6465 6c29 01da 0976 616c  BaseModel)...val
+00000190: 6964 6174 6f72 e901 0000 0029 01da 0676  idator.....)...v
+000001a0: 616c 696e 7429 01da 0676 616c 7374 7229  alint)...valstr)
+000001b0: 01da 0a54 6173 6b45 7870 6f72 7429 01da  ...TaskExport)..
+000001c0: 0a54 6173 6b49 6d70 6f72 7429 01da 0854  .TaskImport)...T
+000001d0: 6173 6b52 6561 6429 0ada 0e57 6f72 6b66  askRead)...Workf
+000001e0: 6c6f 7743 7265 6174 65da 0c57 6f72 6b66  lowCreate..Workf
+000001f0: 6c6f 7752 6561 64da 0e57 6f72 6b66 6c6f  lowRead..Workflo
+00000200: 7755 7064 6174 65da 0e57 6f72 6b66 6c6f  wUpdate..Workflo
+00000210: 7749 6d70 6f72 74da 0e57 6f72 6b66 6c6f  wImport..Workflo
+00000220: 7745 7870 6f72 74da 1257 6f72 6b66 6c6f  wExport..Workflo
+00000230: 7754 6173 6b43 7265 6174 65da 1257 6f72  wTaskCreate..Wor
+00000240: 6b66 6c6f 7754 6173 6b49 6d70 6f72 74da  kflowTaskImport.
+00000250: 1257 6f72 6b66 6c6f 7754 6173 6b45 7870  .WorkflowTaskExp
+00000260: 6f72 74da 1057 6f72 6b66 6c6f 7754 6173  ort..WorkflowTas
+00000270: 6b52 6561 64da 1257 6f72 6b66 6c6f 7754  kRead..WorkflowT
+00000280: 6173 6b55 7064 6174 6563 0000 0000 0000  askUpdatec......
+00000290: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+000002a0: 0000 733e 0000 0065 005a 0164 005a 0255  ..s>...e.Z.d.Z.U
+000002b0: 0064 015a 0365 0465 0565 0665 0766 0219  .d.Z.e.e.e.e.f..
+000002c0: 0019 0065 0864 023c 0064 015a 0965 0465  ...e.d.<.d.Z.e.e
+000002d0: 0565 0665 0766 0219 0019 0065 0864 033c  .e.e.f.....e.d.<
+000002e0: 0064 0153 0029 04da 115f 576f 726b 666c  .d.S.)..._Workfl
+000002f0: 6f77 5461 736b 4261 7365 4eda 046d 6574  owTaskBaseN..met
+00000300: 61da 0461 7267 7329 0ada 085f 5f6e 616d  a..args)...__nam
+00000310: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000320: 0c5f 5f71 7561 6c6e 616d 655f 5f72 1700  .__qualname__r..
+00000330: 0000 7203 0000 00da 0464 6963 74da 0373  ..r......dict..s
+00000340: 7472 7202 0000 00da 0f5f 5f61 6e6e 6f74  trr......__annot
+00000350: 6174 696f 6e73 5f5f 7218 0000 00a9 0072  ations__r......r
+00000360: 1f00 0000 721f 0000 00fa 402f 686f 6d65  ....r.....@/home
+00000370: 2f74 6f6d 6d61 736f 2f46 7261 6374 616c  /tommaso/Fractal
+00000380: 2f66 7261 6374 616c 2f66 7261 6374 616c  /fractal/fractal
+00000390: 2f63 6f6d 6d6f 6e2f 7363 6865 6d61 732f  /common/schemas/
+000003a0: 776f 726b 666c 6f77 2e70 7972 1600 0000  workflow.pyr....
+000003b0: 1c00 0000 7306 0000 000a 0018 021c 0172  ....s..........r
+000003c0: 1600 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000003d0: 0000 0000 0005 0000 0040 0000 0073 3200  .........@...s2.
+000003e0: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
+000003f0: 1900 6505 6401 3c00 6506 6401 6402 6403  ..e.d.<.e.d.d.d.
+00000400: 8d02 6507 6401 6404 6405 8d02 8301 5a08  ..e.d.d.d.....Z.
+00000410: 6406 5300 2907 7211 0000 00da 056f 7264  d.S.).r......ord
+00000420: 6572 54a9 01da 0b61 6c6c 6f77 5f72 6575  erT....allow_reu
+00000430: 7365 7201 0000 0029 01da 076d 696e 5f76  ser....)...min_v
+00000440: 616c 4e29 0972 1900 0000 721a 0000 0072  alN).r....r....r
+00000450: 1b00 0000 7203 0000 00da 0369 6e74 721e  ....r......intr.
+00000460: 0000 0072 0500 0000 7207 0000 00da 065f  ...r....r......_
+00000470: 6f72 6465 7272 1f00 0000 721f 0000 0072  orderr....r....r
+00000480: 1f00 0000 7220 0000 0072 1100 0000 2200  ....r ...r....".
+00000490: 0000 7306 0000 000a 000c 011c 0272 1100  ..s..........r..
+000004a0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000004b0: 0000 0003 0000 0040 0000 0073 3a00 0000  .......@...s:...
+000004c0: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
+000004d0: 3c00 6505 6503 1900 6504 6402 3c00 6503  <.e.e...e.d.<.e.
+000004e0: 6504 6403 3c00 6503 6504 6404 3c00 6506  e.d.<.e.e.d.<.e.
+000004f0: 6504 6405 3c00 6406 5300 2907 7214 0000  e.d.<.d.S.).r...
+00000500: 00da 0269 6472 2100 0000 da0b 776f 726b  ...idr!.....work
+00000510: 666c 6f77 5f69 64da 0774 6173 6b5f 6964  flow_id..task_id
+00000520: da04 7461 736b 4e29 0772 1900 0000 721a  ..taskN).r....r.
+00000530: 0000 0072 1b00 0000 7225 0000 0072 1e00  ...r....r%...r..
+00000540: 0000 7203 0000 0072 0b00 0000 721f 0000  ..r....r....r...
+00000550: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00000560: 7214 0000 0028 0000 0073 0c00 0000 0a00  r....(...s......
+00000570: 0801 0c01 0801 0801 0c01 7214 0000 0063  ..........r....c
+00000580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000590: 0300 0000 4000 0000 f316 0000 0065 005a  ....@........e.Z
+000005a0: 0164 005a 0255 0065 0365 0464 013c 0064  .d.Z.U.e.e.d.<.d
+000005b0: 0253 0029 0372 1200 0000 722a 0000 004e  .S.).r....r*...N
+000005c0: 2905 7219 0000 0072 1a00 0000 721b 0000  ).r....r....r...
+000005d0: 0072 0a00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+000005e0: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+000005f0: 1200 0000 3000 0000 f304 0000 000a 000c  ....0...........
+00000600: 0172 1200 0000 6300 0000 0000 0000 0000  .r....c.........
+00000610: 0000 0000 0000 0003 0000 0040 0000 0072  ...........@...r
+00000620: 2b00 0000 2903 7213 0000 0072 2a00 0000  +...).r....r*...
+00000630: 4e29 0572 1900 0000 721a 0000 0072 1b00  N).r....r....r..
+00000640: 0000 7209 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00000650: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00000660: 7213 0000 0034 0000 0072 2c00 0000 7213  r....4...r,...r.
+00000670: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000680: 0000 0000 0300 0000 4000 0000 731c 0000  ........@...s...
+00000690: 0065 005a 0164 005a 0265 0364 0183 0164  .e.Z.d.Z.e.d...d
+000006a0: 0264 0384 0083 015a 0464 0453 0029 0572  .d.....Z.d.S.).r
+000006b0: 1500 0000 7217 0000 0063 0200 0000 0000  ....r....c......
+000006c0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+000006d0: 0000 7314 0000 0064 017c 0176 0072 0874  ..s....d.|.v.r.t
+000006e0: 0064 0283 0182 017c 0153 0029 034e da15  .d.....|.S.).N..
+000006f0: 7061 7261 6c6c 656c 697a 6174 696f 6e5f  parallelization_
+00000700: 6c65 7665 6c7a 3b4f 7665 7272 6964 696e  levelz;Overridin
+00000710: 6720 7461 736b 2070 6172 616c 6c65 6c69  g task paralleli
+00000720: 7a61 7469 6f6e 206c 6576 656c 2063 7572  zation level cur
+00000730: 7265 6e74 6c79 206e 6f74 2061 6c6c 6f77  rently not allow
+00000740: 6564 2901 da0a 5661 6c75 6545 7272 6f72  ed)...ValueError
+00000750: 2902 da03 636c 73da 016d 721f 0000 0072  )...cls..mr....r
+00000760: 1f00 0000 7220 0000 00da 1e63 6865 636b  ....r .....check
+00000770: 5f6e 6f5f 7061 7261 6c6c 656c 6973 6174  _no_parallelisat
+00000780: 696f 6e5f 6c65 7665 6c3a 0000 0073 0a00  ion_level:...s..
+00000790: 0000 0802 0201 0201 04ff 0403 7a31 576f  ............z1Wo
+000007a0: 726b 666c 6f77 5461 736b 5570 6461 7465  rkflowTaskUpdate
+000007b0: 2e63 6865 636b 5f6e 6f5f 7061 7261 6c6c  .check_no_parall
+000007c0: 656c 6973 6174 696f 6e5f 6c65 7665 6c4e  elisation_levelN
+000007d0: 2905 7219 0000 0072 1a00 0000 721b 0000  ).r....r....r...
+000007e0: 0072 0500 0000 7231 0000 0072 1f00 0000  .r....r1...r....
+000007f0: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+00000800: 1500 0000 3800 0000 7306 0000 0008 0006  ....8...s.......
+00000810: 020e 0172 1500 0000 6300 0000 0000 0000  ...r....c.......
+00000820: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000830: 0072 2b00 0000 2903 da0d 5f57 6f72 6b66  .r+...)..._Workf
+00000840: 6c6f 7742 6173 65da 046e 616d 654e 2905  lowBase..nameN).
+00000850: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+00000860: 1d00 0000 721e 0000 0072 1f00 0000 721f  ....r....r....r.
+00000870: 0000 0072 1f00 0000 7220 0000 0072 3200  ...r....r ...r2.
+00000880: 0000 4300 0000 722c 0000 0072 3200 0000  ..C...r,...r2...
+00000890: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000008a0: 0003 0000 0040 0000 0073 2a00 0000 6500  .....@...s*...e.
+000008b0: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
+000008c0: 6503 6504 6402 3c00 6505 6506 1900 6504  e.e.d.<.e.e...e.
+000008d0: 6403 3c00 6404 5300 2905 720d 0000 0072  d.<.d.S.).r....r
+000008e0: 2700 0000 da0a 7072 6f6a 6563 745f 6964  '.....project_id
+000008f0: da09 7461 736b 5f6c 6973 744e 2907 7219  ..task_listN).r.
+00000900: 0000 0072 1a00 0000 721b 0000 0072 2500  ...r....r....r%.
+00000910: 0000 721e 0000 00da 046c 6973 7472 1400  ..r......listr..
+00000920: 0000 721f 0000 0072 1f00 0000 721f 0000  ..r....r....r...
+00000930: 0072 2000 0000 720d 0000 0047 0000 0073  .r ...r....G...s
+00000940: 0800 0000 0a00 0801 0801 1001 720d 0000  ............r...
+00000950: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000960: 0000 0400 0000 4000 0000 7320 0000 0065  ......@...s ...e
+00000970: 005a 0164 005a 0265 0364 0164 0264 038d  .Z.d.Z.e.d.d.d..
+00000980: 0265 0464 0183 0183 015a 0564 0453 0029  .e.d.....Z.d.S.)
+00000990: 0572 0c00 0000 7233 0000 0054 7222 0000  .r....r3...Tr"..
+000009a0: 004e 2906 7219 0000 0072 1a00 0000 721b  .N).r....r....r.
+000009b0: 0000 0072 0500 0000 7208 0000 00da 055f  ...r....r......_
+000009c0: 6e61 6d65 721f 0000 0072 1f00 0000 721f  namer....r....r.
+000009d0: 0000 0072 2000 0000 720c 0000 004d 0000  ...r ...r....M..
+000009e0: 0073 0400 0000 0800 1802 720c 0000 0063  .s........r....c
+000009f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000a00: 0400 0000 4000 0000 734e 0000 0065 005a  ....@...sN...e.Z
+00000a10: 0164 005a 0255 0065 0365 0419 0065 0564  .d.Z.U.e.e...e.d
+00000a20: 013c 0065 0365 0665 0719 0019 0065 0564  .<.e.e.e.....e.d
+00000a30: 023c 0065 0864 0164 0364 048d 0265 0964  .<.e.d.d.d...e.d
+00000a40: 0183 0183 015a 0a65 0864 0283 0164 0564  .....Z.e.d...d.d
+00000a50: 0684 0083 015a 0b64 0753 0029 0872 0e00  .....Z.d.S.).r..
+00000a60: 0000 7233 0000 00da 1a72 656f 7264 6572  ..r3.....reorder
+00000a70: 6564 5f77 6f72 6b66 6c6f 7774 6173 6b5f  ed_workflowtask_
+00000a80: 6964 7354 7222 0000 0063 0200 0000 0000  idsTr"...c......
+00000a90: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+00000aa0: 0000 733a 0000 0074 0064 0164 0284 007c  ..s:...t.d.d...|
+00000ab0: 0144 0083 0183 0172 0d74 0164 0383 0182  .D.....r.t.d....
+00000ac0: 0174 027c 0183 0174 0274 037c 0183 0183  .t.|...t.t.|....
+00000ad0: 016b 0372 1b74 0164 0483 0182 017c 0153  .k.r.t.d.....|.S
+00000ae0: 0029 054e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00000af0: 0002 0000 0003 0000 0073 0000 0073 1800  .........s...s..
+00000b00: 0000 8100 7c00 5d07 7d01 7c01 6400 6b00  ....|.].}.|.d.k.
+00000b10: 5600 0100 7102 6401 5300 2902 7201 0000  V...q.d.S.).r...
+00000b20: 004e 721f 0000 0029 02da 022e 30da 0169  .Nr....)....0..i
+00000b30: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
+00000b40: 093c 6765 6e65 7870 723e 5b00 0000 7304  .<genexpr>[...s.
+00000b50: 0000 0002 8016 007a 3b57 6f72 6b66 6c6f  .......z;Workflo
+00000b60: 7755 7064 6174 652e 6368 6563 6b5f 706f  wUpdate.check_po
+00000b70: 7369 7469 7665 5f61 6e64 5f75 6e69 7175  sitive_and_uniqu
+00000b80: 652e 3c6c 6f63 616c 733e 2e3c 6765 6e65  e.<locals>.<gene
+00000b90: 7870 723e 7a2d 4e65 6761 7469 7665 2060  xpr>z-Negative `
+00000ba0: 6964 6020 696e 2060 7265 6f72 6465 7265  id` in `reordere
+00000bb0: 645f 776f 726b 666c 6f77 7461 736b 5f69  d_workflowtask_i
+00000bc0: 6473 607a 2c60 7265 6f72 6465 7265 645f  ds`z,`reordered_
+00000bd0: 776f 726b 666c 6f77 7461 736b 5f69 6473  workflowtask_ids
+00000be0: 6020 6861 7320 7265 7065 7469 7469 6f6e  ` has repetition
+00000bf0: 7329 04da 0361 6e79 722e 0000 00da 036c  s)...anyr......l
+00000c00: 656e da03 7365 7429 0272 2f00 0000 da05  en..set).r/.....
+00000c10: 7661 6c75 6572 1f00 0000 721f 0000 0072  valuer....r....r
+00000c20: 2000 0000 da19 6368 6563 6b5f 706f 7369   .....check_posi
+00000c30: 7469 7665 5f61 6e64 5f75 6e69 7175 6559  tive_and_uniqueY
+00000c40: 0000 0073 0a00 0000 1202 0801 1401 0801  ...s............
+00000c50: 0401 7a28 576f 726b 666c 6f77 5570 6461  ..z(WorkflowUpda
+00000c60: 7465 2e63 6865 636b 5f70 6f73 6974 6976  te.check_positiv
+00000c70: 655f 616e 645f 756e 6971 7565 4e29 0c72  e_and_uniqueN).r
+00000c80: 1900 0000 721a 0000 0072 1b00 0000 7203  ....r....r....r.
+00000c90: 0000 0072 1d00 0000 721e 0000 0072 3600  ...r....r....r6.
+00000ca0: 0000 7225 0000 0072 0500 0000 7208 0000  ..r%...r....r...
+00000cb0: 0072 3700 0000 7240 0000 0072 1f00 0000  .r7...r@...r....
+00000cc0: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+00000cd0: 0e00 0000 5200 0000 730c 0000 000a 000c  ....R...s.......
+00000ce0: 0110 0114 0306 020e 0172 0e00 0000 6300  .........r....c.
+00000cf0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+00000d00: 0000 0040 0000 0073 2e00 0000 6500 5a01  ...@...s....e.Z.
+00000d10: 6400 5a02 5500 6503 6504 1900 6505 6401  d.Z.U.e.e...e.d.
+00000d20: 3c00 6506 6402 6403 6404 8d02 6507 6402  <.e.d.d.d...e.d.
+00000d30: 8301 8301 5a08 6405 5300 2906 720f 0000  ....Z.d.S.).r...
+00000d40: 0072 3500 0000 7233 0000 0054 7222 0000  .r5...r3...Tr"..
+00000d50: 004e 2909 7219 0000 0072 1a00 0000 721b  .N).r....r....r.
+00000d60: 0000 0072 3600 0000 7212 0000 0072 1e00  ...r6...r....r..
+00000d70: 0000 7205 0000 0072 0800 0000 7237 0000  ..r....r....r7..
+00000d80: 0072 1f00 0000 721f 0000 0072 1f00 0000  .r....r....r....
+00000d90: 7220 0000 0072 0f00 0000 6200 0000 7306  r ...r....b...s.
+00000da0: 0000 000a 000c 0118 0372 0f00 0000 6300  .........r....c.
+00000db0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000dc0: 0000 0040 0000 0073 1a00 0000 6500 5a01  ...@...s....e.Z.
+00000dd0: 6400 5a02 5500 6503 6504 1900 6505 6401  d.Z.U.e.e...e.d.
+00000de0: 3c00 6402 5300 2903 7210 0000 0072 3500  <.d.S.).r....r5.
+00000df0: 0000 4e29 0672 1900 0000 721a 0000 0072  ..N).r....r....r
+00000e00: 1b00 0000 7236 0000 0072 1300 0000 721e  ....r6...r....r.
+00000e10: 0000 0072 1f00 0000 721f 0000 0072 1f00  ...r....r....r..
+00000e20: 0000 7220 0000 0072 1000 0000 6900 0000  ..r ...r....i...
+00000e30: 7304 0000 000a 0010 0172 1000 0000 4e29  s........r....N)
+00000e40: 1ada 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
+00000e50: 0000 00da 0870 7964 616e 7469 6372 0400  .....pydanticr..
+00000e60: 0000 7205 0000 00da 0b5f 7661 6c69 6461  ..r......_valida
+00000e70: 746f 7273 7207 0000 0072 0800 0000 722a  torsr....r....r*
+00000e80: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
+00000e90: 0000 da07 5f5f 616c 6c5f 5f72 1600 0000  ....__all__r....
+00000ea0: 7211 0000 0072 1400 0000 7212 0000 0072  r....r....r....r
+00000eb0: 1300 0000 7215 0000 0072 3200 0000 720d  ....r....r2...r.
+00000ec0: 0000 0072 0c00 0000 720e 0000 0072 0f00  ...r....r....r..
+00000ed0: 0000 7210 0000 0072 1f00 0000 721f 0000  ..r....r....r...
+00000ee0: 0072 1f00 0000 7220 0000 00da 083c 6d6f  .r....r .....<mo
+00000ef0: 6475 6c65 3e01 0000 0073 2c00 0000 0c00  dule>....s,.....
+00000f00: 0c01 0c02 0c01 0c02 0c01 0c01 0c01 0c01  ................
+00000f10: 0403 100e 1006 1006 1008 1004 1004 100b  ................
+00000f20: 1004 1006 1005 1010 1407                 ..........
```

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/_validators.py` & `fractal_client-1.3.0a1/fractal/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/applyworkflow.py` & `fractal_client-1.3.0a1/fractal/common/schemas/applyworkflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 from datetime import datetime
-from typing import List
 from typing import Optional
 
+from pydantic import BaseModel
 from pydantic import validator
-from sqlmodel import SQLModel
 
 from ._validators import valstr
 
 __all__ = (
-    "ApplyWorkflowBase",
+    "_ApplyWorkflowBase",
     "ApplyWorkflowCreate",
     "ApplyWorkflowRead",
 )
 
 
-class ApplyWorkflowBase(SQLModel):
+class _ApplyWorkflowBase(BaseModel):
     """
     Base class for ApplyWorkflow
 
     Attributes:
         worker_init: TBD
     """
 
     worker_init: Optional[str]
 
 
-class ApplyWorkflowCreate(ApplyWorkflowBase):
+class ApplyWorkflowCreate(_ApplyWorkflowBase):
 
     # Validators
     _worker_init = validator("worker_init", allow_reuse=True)(
         valstr("worker_init")
     )
 
 
-class ApplyWorkflowRead(ApplyWorkflowBase):
+class ApplyWorkflowRead(_ApplyWorkflowBase):
     id: int
     project_id: int
     workflow_id: int
     input_dataset_id: int
     output_dataset_id: int
     start_timestamp: datetime
+    end_timestamp: Optional[datetime]
     status: str
     log: Optional[str]
-    history: Optional[List[str]]
+    history: Optional[list[str]]
     working_dir: Optional[str]
     working_dir_user: Optional[str]
 
     def sanitised_dict(self):
         d = self.dict()
         d["start_timestamp"] = str(self.start_timestamp)
+        d["end_timestamp"] = str(self.end_timestamp)
         return d
```

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/manifest.py` & `fractal_client-1.3.0a1/fractal/common/schemas/manifest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from pathlib import Path
 from typing import Any
-from typing import Dict
-from typing import List
 from typing import Optional
 from typing import TypeVar
 
 from pydantic import BaseModel
+from pydantic import Field
 from pydantic import validator
-from sqlmodel import Field
 
 
 __all__ = ("TaskManifestV1", "ManifestV1")
 
 
 class _TaskManifestBase(BaseModel):
     """
@@ -42,16 +40,16 @@
             etc.
     """
 
     name: str
     executable: Path
     input_type: str
     output_type: str
-    default_args: Optional[Dict[str, Any]] = Field(default_factory=dict)
-    meta: Optional[Dict[str, Any]] = Field(default_factory=dict)
+    default_args: Optional[dict[str, Any]] = Field(default_factory=dict)
+    meta: Optional[dict[str, Any]] = Field(default_factory=dict)
 
 
 TaskManifestType = TypeVar("TaskManifestType", bound=_TaskManifestBase)
 
 
 class _ManifestBase(BaseModel):
     """
@@ -65,31 +63,31 @@
 
     Attributes:
         manifest_version:
             A version string that provides indication for compatibility between
             manifests as the schema evolves. This is for instance used by
             Fractal to determine which subclass of the present base class needs
             be used to read and validate the input.
-        task_list : List[TaskManifestType]
+        task_list : list[TaskManifestType]
             The list of tasks, represented as specified by subclasses of the
             _TaskManifestBase (a.k.a. TaskManifestType)
     """
 
     manifest_version: str
-    task_list: List[TaskManifestType]  # type: ignore
+    task_list: list[TaskManifestType]  # type: ignore
 
 
 class TaskManifestV1(_TaskManifestBase):
     pass
 
 
 class ManifestV1(_ManifestBase):
     """
     Manifest schema version 1
     """
 
-    task_list: List[TaskManifestV1]
+    task_list: list[TaskManifestV1]
 
     @validator("manifest_version")
     def manifest_version_1(cls, value):
         if value != "1":
             raise ValueError("Wrong manifest version")
```

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/project.py` & `fractal_client-1.3.0a1/fractal/common/schemas/project.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from typing import Any
-from typing import Dict
-from typing import List
 from typing import Optional
 
+from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
-from sqlmodel import SQLModel
 
 from ._validators import val_absolute_path
 from ._validators import valstr
 
 
 __all__ = (
     "ProjectCreate",
@@ -23,15 +21,15 @@
     "ResourceUpdate",
 )
 
 
 # RESOURCE
 
 
-class _ResourceBase(SQLModel):
+class _ResourceBase(BaseModel):
     """
     Base class for Resource
     """
 
     path: str
 
 
@@ -49,34 +47,34 @@
     id: int
     dataset_id: int
 
 
 # DATASET
 
 
-class _DatasetBase(SQLModel):
+class _DatasetBase(BaseModel):
     """
     Base class for Dataset
 
     Attributes:
         name: TBD
         type: TBD
         meta: TBD
         read_only: TBD
     """
 
     name: str
     type: Optional[str]
-    meta: Dict[str, Any] = Field(default={})
+    meta: dict[str, Any] = Field(default={})
     read_only: bool = False
 
 
 class DatasetUpdate(_DatasetBase):
     name: Optional[str]
-    meta: Optional[Dict[str, Any]] = None
+    meta: Optional[dict[str, Any]] = None
     read_only: Optional[bool]
 
     # Validators
     _name = validator("name", allow_reuse=True)(valstr("name"))
     _type = validator("type", allow_reuse=True)(valstr("type"))
 
 
@@ -84,23 +82,23 @@
     # Validators
     _name = validator("name", allow_reuse=True)(valstr("name"))
     _type = validator("type", allow_reuse=True)(valstr("type"))
 
 
 class DatasetRead(_DatasetBase):
     id: int
-    resource_list: List[ResourceRead]
+    resource_list: list[ResourceRead]
     project_id: int
     read_only: bool
 
 
 # PROJECT
 
 
-class _ProjectBase(SQLModel):
+class _ProjectBase(BaseModel):
     """
     Base class for Project
 
     Attributes:
         name: TBD
         read_only: TBD
     """
@@ -117,15 +115,15 @@
     _default_dataset_name = validator(
         "default_dataset_name", allow_reuse=True
     )(valstr("default_dataset_name"))
 
 
 class ProjectRead(_ProjectBase):
     id: int
-    dataset_list: List[DatasetRead] = []
+    dataset_list: list[DatasetRead] = []
 
 
 class ProjectUpdate(_ProjectBase):
     name: Optional[str]
     read_only: Optional[bool]
 
     # Validators
```

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/state.py` & `fractal_client-1.3.0a1/fractal/common/schemas/state.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from datetime import datetime
 from typing import Any
-from typing import Dict
 from typing import Optional
 
-from sqlmodel import SQLModel
+from pydantic import BaseModel
 
 
 __all__ = (
     "_StateBase",
     "StateRead",
 )
 
 
-class _StateBase(SQLModel):
+class _StateBase(BaseModel):
     """
     Base class for `State`
 
     Attributes:
         id: Primary key
         data: Content of the state
         timestamp: Time stamp of the state
     """
 
-    data: Dict[str, Any]
+    data: dict[str, Any]
     timestamp: datetime
 
     def sanitised_dict(self):
         """
         Return `self.dict()` after casting `self.timestamp` to a string
         """
         d = self.dict()
```

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/user.py` & `fractal_client-1.3.0a1/fractal/common/schemas/user.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,33 +13,38 @@
     "UserCreate",
 )
 
 
 class UserRead(schemas.BaseUser[int]):
     slurm_user: Optional[str]
     cache_dir: Optional[str]
+    username: Optional[str]
 
 
 class UserUpdate(schemas.BaseUserUpdate):
     slurm_user: Optional[str]
     cache_dir: Optional[str]
+    username: Optional[str]
 
     # Validators
     _slurm_user = validator("slurm_user", allow_reuse=True)(
         valstr("slurm_user")
     )
+    _username = validator("username", allow_reuse=True)(valstr("username"))
     _cache_dir = validator("cache_dir", allow_reuse=True)(
         val_absolute_path("cache_dir")
     )
 
 
 class UserCreate(schemas.BaseUserCreate):
     slurm_user: Optional[str]
     cache_dir: Optional[str]
+    username: Optional[str]
 
     # Validators
     _slurm_user = validator("slurm_user", allow_reuse=True)(
         valstr("slurm_user")
     )
+    _username = validator("username", allow_reuse=True)(valstr("username"))
     _cache_dir = validator("cache_dir", allow_reuse=True)(
         val_absolute_path("cache_dir")
     )
```

### Comparing `fractal_client-1.3.0a0/fractal/common/schemas/workflow.py` & `fractal_client-1.3.0a1/fractal/common/schemas/workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Any
-from typing import Dict
-from typing import List
 from typing import Optional
 
+from pydantic import BaseModel
 from pydantic import validator
-from sqlmodel import SQLModel
 
 from ._validators import valint
 from ._validators import valstr
 from .task import TaskExport
 from .task import TaskImport
 from .task import TaskRead
 
@@ -23,18 +21,18 @@
     "WorkflowTaskImport",
     "WorkflowTaskExport",
     "WorkflowTaskRead",
     "WorkflowTaskUpdate",
 )
 
 
-class _WorkflowTaskBase(SQLModel):
+class _WorkflowTaskBase(BaseModel):
 
-    meta: Optional[Dict[str, Any]] = None
-    args: Optional[Dict[str, Any]] = None
+    meta: Optional[dict[str, Any]] = None
+    args: Optional[dict[str, Any]] = None
 
 
 class WorkflowTaskCreate(_WorkflowTaskBase):
     order: Optional[int]
     # Validators
     _order = validator("order", allow_reuse=True)(valint("order", min_val=0))
 
@@ -62,47 +60,47 @@
         if "parallelization_level" in m:
             raise ValueError(
                 "Overriding task parallelization level currently not allowed"
             )
         return m
 
 
-class _WorkflowBase(SQLModel):
+class _WorkflowBase(BaseModel):
     name: str
 
 
 class WorkflowRead(_WorkflowBase):
     id: int
     project_id: int
-    task_list: List[WorkflowTaskRead]
+    task_list: list[WorkflowTaskRead]
 
 
 class WorkflowCreate(_WorkflowBase):
     # Validators
     _name = validator("name", allow_reuse=True)(valstr("name"))
 
 
 class WorkflowUpdate(_WorkflowBase):
     name: Optional[str]
-    reordered_workflowtask_ids: Optional[List[int]]
+    reordered_workflowtask_ids: Optional[list[int]]
 
     # Validators
     _name = validator("name", allow_reuse=True)(valstr("name"))
 
     @validator("reordered_workflowtask_ids")
     def check_positive_and_unique(cls, value):
         if any(i < 0 for i in value):
             raise ValueError("Negative `id` in `reordered_workflowtask_ids`")
         if len(value) != len(set(value)):
             raise ValueError("`reordered_workflowtask_ids` has repetitions")
         return value
 
 
 class WorkflowImport(_WorkflowBase):
-    task_list: List[WorkflowTaskImport]
+    task_list: list[WorkflowTaskImport]
 
     # Validators
     _name = validator("name", allow_reuse=True)(valstr("name"))
 
 
 class WorkflowExport(_WorkflowBase):
-    task_list: List[WorkflowTaskExport]
+    task_list: list[WorkflowTaskExport]
```

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar  6 13:52:21 2023 UTC, .py size: 748 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-00000000: 6f0d 0d0a 0000 0000 15f0 0564 ec02 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 3d55 6f64 a604 0000  o.......=Uod....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6400 6405 6c0b 6d0d 5a0d 0100  Z...d.d.l.m.Z...
 00000080: 6406 6407 8400 5a0e 6408 6409 8400 5a0f  d.d...Z.d.d...Z.
 00000090: 6401 5300 290a e900 0000 004e 2901 da05  d.S.)......N)...
 000000a0: 6465 6275 6729 01da 0f56 616c 6964 6174  debug)...Validat
 000000b0: 696f 6e45 7272 6f72 2901 da0a 5461 736b  ionError)...Task
 000000c0: 4372 6561 7465 2901 da0a 5461 736b 5570  Create)...TaskUp
 000000d0: 6461 7465 6300 0000 0000 0000 0000 0000  datec...........
-000000e0: 000b 0000 000c 0000 0043 0000 0073 3002  .........C...s0.
+000000e0: 000d 0000 000c 0000 0043 0000 0073 6203  .........C...sb.
 000000f0: 0000 7400 6401 6402 8d01 7d00 7401 7c00  ..t.d.d...}.t.|.
 00000100: 8301 0100 7c00 6a02 7d01 6403 7d02 7c01  ....|.j.}.d.}.|.
 00000110: 7c02 6404 8d01 7d03 7c03 6a03 7d04 7c04  |.d...}.|.j.}.|.
 00000120: 8300 7d05 7404 7c05 8301 7d06 6401 6701  ..}.t.|...}.d.g.
 00000130: 7d07 7c06 7c07 6b02 7d08 7c08 737f 7405  }.|.|.k.}.|.s.t.
 00000140: a006 6405 7c08 6601 6406 7c06 7c07 6602  ..d.|.f.d.|.|.f.
 00000150: a104 6407 7407 a008 a100 7600 733b 7405  ..d.t.....v.s;t.
@@ -43,97 +43,133 @@
 000002a0: 6e01 6408 7405 a00a 7c01 a101 7405 a00a  n.d.t...|...t...
 000002b0: 7c02 a101 7405 a00a 7c03 a101 7405 a00a  |...t...|...t...
 000002c0: 7c04 a101 7405 a00a 7c05 a101 7405 a00a  |...t...|...t...
 000002d0: 7c06 a101 7405 a00a 7c07 a101 6409 9c09  |...t...|...d...
 000002e0: 1600 7d09 640a 640b 7c09 6901 1600 7d0a  ..}.d.d.|.i...}.
 000002f0: 740b 7405 a00c 7c0a a101 8301 8201 6400  t.t...|.......d.
 00000300: 0400 7d01 0400 7d02 0400 7d03 0400 7d04  ..}...}...}...}.
-00000310: 0400 7d05 0400 7d06 0400 7d08 7d07 6400  ..}...}...}.}.d.
-00000320: 5300 290e 4eda 046e 616d 6529 0172 0600  S.).N..name).r..
-00000330: 0000 5429 01da 0c65 7863 6c75 6465 5f6e  ..T)...exclude_n
-00000340: 6f6e 6529 01fa 023d 3d29 017a ab25 2870  one)...==).z.%(p
-00000350: 7931 3329 730a 7b25 2870 7931 3329 7320  y13)s.{%(py13)s 
-00000360: 3d20 2528 7079 3029 7328 2528 7079 3131  = %(py0)s(%(py11
-00000370: 2973 0a7b 2528 7079 3131 2973 203d 2025  )s.{%(py11)s = %
-00000380: 2870 7939 2973 0a7b 2528 7079 3929 7320  (py9)s.{%(py9)s 
-00000390: 3d20 2528 7079 3729 730a 7b25 2870 7937  = %(py7)s.{%(py7
-000003a0: 2973 203d 2025 2870 7933 2973 0a7b 2528  )s = %(py3)s.{%(
-000003b0: 7079 3329 7320 3d20 2528 7079 3129 732e  py3)s = %(py1)s.
-000003c0: 6469 6374 0a7d 2865 7863 6c75 6465 5f6e  dict.}(exclude_n
-000003d0: 6f6e 653d 2528 7079 3529 7329 0a7d 2e6b  one=%(py5)s).}.k
-000003e0: 6579 730a 7d28 290a 7d29 0a7d 203d 3d20  eys.}().}).} == 
-000003f0: 2528 7079 3136 2973 da04 6c69 7374 da01  %(py16)s..list..
-00000400: 7429 09da 0370 7930 da03 7079 31da 0370  t)...py0..py1..p
-00000410: 7933 da03 7079 35da 0370 7937 da03 7079  y3..py5..py7..py
-00000420: 39da 0470 7931 31da 0470 7931 33da 0470  9..py11..py13..p
-00000430: 7931 367a 0f61 7373 6572 7420 2528 7079  y16z.assert %(py
-00000440: 3138 2973 da04 7079 3138 2901 da0d 6578  18)s..py18)...ex
-00000450: 636c 7564 655f 756e 7365 7429 017a ac25  clude_unset).z.%
-00000460: 2870 7931 3329 730a 7b25 2870 7931 3329  (py13)s.{%(py13)
-00000470: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
-00000480: 3131 2973 0a7b 2528 7079 3131 2973 203d  11)s.{%(py11)s =
-00000490: 2025 2870 7939 2973 0a7b 2528 7079 3929   %(py9)s.{%(py9)
-000004a0: 7320 3d20 2528 7079 3729 730a 7b25 2870  s = %(py7)s.{%(p
-000004b0: 7937 2973 203d 2025 2870 7933 2973 0a7b  y7)s = %(py3)s.{
-000004c0: 2528 7079 3329 7320 3d20 2528 7079 3129  %(py3)s = %(py1)
-000004d0: 732e 6469 6374 0a7d 2865 7863 6c75 6465  s.dict.}(exclude
-000004e0: 5f75 6e73 6574 3d25 2870 7935 2973 290a  _unset=%(py5)s).
-000004f0: 7d2e 6b65 7973 0a7d 2829 0a7d 290a 7d20  }.keys.}().}).} 
-00000500: 3d3d 2025 2870 7931 3629 7329 0d72 0500  == %(py16)s).r..
-00000510: 0000 7202 0000 00da 0464 6963 74da 046b  ..r......dict..k
-00000520: 6579 7372 0900 0000 da0a 4070 7974 6573  eysr......@pytes
-00000530: 745f 6172 da11 5f63 616c 6c5f 7265 7072  t_ar.._call_repr
-00000540: 636f 6d70 6172 65da 0c40 7079 5f62 7569  compare..@py_bui
-00000550: 6c74 696e 73da 066c 6f63 616c 73da 185f  ltins..locals.._
-00000560: 7368 6f75 6c64 5f72 6570 725f 676c 6f62  should_repr_glob
-00000570: 616c 5f6e 616d 65da 095f 7361 6665 7265  al_name.._safere
-00000580: 7072 da0e 4173 7365 7274 696f 6e45 7272  pr..AssertionErr
-00000590: 6f72 da13 5f66 6f72 6d61 745f 6578 706c  or.._format_expl
-000005a0: 616e 6174 696f 6e29 0b72 0a00 0000 da0b  anation).r......
-000005b0: 4070 795f 6173 7365 7274 32da 0b40 7079  @py_assert2..@py
-000005c0: 5f61 7373 6572 7434 da0b 4070 795f 6173  _assert4..@py_as
-000005d0: 7365 7274 36da 0b40 7079 5f61 7373 6572  sert6..@py_asser
-000005e0: 7438 da0c 4070 795f 6173 7365 7274 3130  t8..@py_assert10
-000005f0: da0c 4070 795f 6173 7365 7274 3132 da0c  ..@py_assert12..
-00000600: 4070 795f 6173 7365 7274 3135 da0c 4070  @py_assert15..@p
-00000610: 795f 6173 7365 7274 3134 da0c 4070 795f  y_assert14..@py_
-00000620: 666f 726d 6174 3137 da0c 4070 795f 666f  format17..@py_fo
-00000630: 726d 6174 3139 a900 722a 0000 00fa 3f2f  rmat19..r*....?/
-00000640: 686f 6d65 2f74 6f6d 6d61 736f 2f46 7261  home/tommaso/Fra
-00000650: 6374 616c 2f66 7261 6374 616c 2f66 7261  ctal/fractal/fra
-00000660: 6374 616c 2f63 6f6d 6d6f 6e2f 7465 7374  ctal/common/test
-00000670: 732f 7465 7374 5f74 6173 6b2e 7079 da10  s/test_task.py..
-00000680: 7465 7374 5f74 6173 6b5f 7570 6461 7465  test_task_update
-00000690: 0900 0000 730c 0000 000a 0208 01fe 010e  ....s...........
-000006a0: 00fe 0114 0072 2c00 0000 6300 0000 0000  .....r,...c.....
-000006b0: 0000 0000 0000 0001 0000 0008 0000 0043  ...............C
-000006c0: 0000 0073 5600 0000 7400 6401 6402 6403  ...sV...t.d.d.d.
-000006d0: 6404 6405 6406 8d05 7d00 7401 7c00 8301  d.d.d...}.t.|...
-000006e0: 0100 7402 a003 7404 a101 8f0f 0100 7400  ..t...t.......t.
-000006f0: 6401 6402 6407 8d02 0100 5700 6400 0400  d.d.d.....W.d...
-00000700: 0400 8303 0100 6400 5300 3100 7324 7701  ......d.S.1.s$w.
-00000710: 0100 0100 0100 5900 0100 6400 5300 2908  ......Y...d.S.).
-00000720: 4eda 0474 6173 6bda 0673 6f75 7263 65da  N..task..source.
-00000730: 0763 6f6d 6d61 6e64 da0a 696e 7075 745f  .command..input_
-00000740: 7479 7065 da0b 6f75 7470 7574 5f74 7970  type..output_typ
-00000750: 6529 0572 0600 0000 722e 0000 0072 2f00  e).r....r....r/.
-00000760: 0000 7230 0000 0072 3100 0000 2902 7206  ..r0...r1...).r.
-00000770: 0000 0072 2e00 0000 2905 7204 0000 0072  ...r....).r....r
-00000780: 0200 0000 da06 7079 7465 7374 da06 7261  ......pytest..ra
-00000790: 6973 6573 7203 0000 0029 0172 0a00 0000  isesr....).r....
-000007a0: 722a 0000 0072 2a00 0000 722b 0000 00da  r*...r*...r+....
-000007b0: 1074 6573 745f 7461 736b 5f63 7265 6174  .test_task_creat
-000007c0: 6511 0000 0073 1600 0000 0202 0201 0201  e....s..........
-000007d0: 0201 0201 0201 06fb 0807 0c02 0e01 22ff  ..............".
-000007e0: 7234 0000 0029 10da 0862 7569 6c74 696e  r4...)...builtin
-000007f0: 7372 1a00 0000 da19 5f70 7974 6573 742e  sr......_pytest.
-00000800: 6173 7365 7274 696f 6e2e 7265 7772 6974  assertion.rewrit
-00000810: 65da 0961 7373 6572 7469 6f6e da07 7265  e..assertion..re
-00000820: 7772 6974 6572 1800 0000 7232 0000 00da  writer....r2....
-00000830: 0864 6576 746f 6f6c 7372 0200 0000 da17  .devtoolsr......
-00000840: 7079 6461 6e74 6963 2e65 7272 6f72 5f77  pydantic.error_w
-00000850: 7261 7070 6572 7372 0300 0000 da07 7363  rappersr......sc
-00000860: 6865 6d61 7372 0400 0000 7205 0000 0072  hemasr....r....r
-00000870: 2c00 0000 7234 0000 0072 2a00 0000 722a  ,...r4...r*...r*
-00000880: 0000 0072 2a00 0000 722b 0000 00da 083c  ...r*...r+.....<
-00000890: 6d6f 6475 6c65 3e01 0000 0073 0e00 0000  module>....s....
-000008a0: 2200 0c01 0c01 0c02 0c01 0803 0c08       ".............
+00000310: 0400 7d05 0400 7d06 0400 7d08 7d07 740d  ..}...}...}.}.t.
+00000320: a00e 740f a101 8f0e 0100 7400 640e 640f  ..t.......t.d.d.
+00000330: 6410 8d02 0100 5700 6400 0400 0400 8303  d.....W.d.......
+00000340: 0100 6e09 3100 9001 732d 7701 0100 0100  ..n.1...s-w.....
+00000350: 0100 5900 0100 740d a00e 740f a101 8f0e  ..Y...t...t.....
+00000360: 0100 7400 640e 6400 6410 8d02 0100 5700  ..t.d.d.d.....W.
+00000370: 6400 0400 0400 8303 0100 6e09 3100 9001  d.........n.1...
+00000380: 7349 7701 0100 0100 0100 5900 0100 7400  sIw.......Y...t.
+00000390: 640e 6411 6412 6413 8d03 7d00 7401 7c00  d.d.d.d...}.t.|.
+000003a0: 8301 0100 7c00 6a10 7d0b 7c0b 9001 7382  ....|.j.}.|...s.
+000003b0: 6414 6408 7407 a008 a100 7600 9001 736d  d.d.t.....v...sm
+000003c0: 7405 a009 7c00 a101 9001 7272 7405 a00a  t...|.....rrt...
+000003d0: 7c00 a101 6e01 6408 7405 a00a 7c0b a101  |...n.d.t...|...
+000003e0: 6415 9c02 1600 7d0c 740b 7405 a00c 7c0c  d.....}.t.t...|.
+000003f0: a101 8301 8201 6400 7d0b 7c00 6a11 7d0b  ......d.}.|.j.}.
+00000400: 7c0b 9001 73ad 6416 6408 7407 a008 a100  |...s.d.d.t.....
+00000410: 7600 9001 7398 7405 a009 7c00 a101 9001  v...s.t...|.....
+00000420: 729d 7405 a00a 7c00 a101 6e01 6408 7405  r.t...|...n.d.t.
+00000430: a00a 7c0b a101 6415 9c02 1600 7d0c 740b  ..|...d.....}.t.
+00000440: 7405 a00c 7c0c a101 8301 8201 6400 7d0b  t...|.......d.}.
+00000450: 6400 5300 2917 4eda 046e 616d 6529 0172  d.S.).N..name).r
+00000460: 0600 0000 5429 01da 0c65 7863 6c75 6465  ....T)...exclude
+00000470: 5f6e 6f6e 6529 01fa 023d 3d29 017a ab25  _none)...==).z.%
+00000480: 2870 7931 3329 730a 7b25 2870 7931 3329  (py13)s.{%(py13)
+00000490: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
+000004a0: 3131 2973 0a7b 2528 7079 3131 2973 203d  11)s.{%(py11)s =
+000004b0: 2025 2870 7939 2973 0a7b 2528 7079 3929   %(py9)s.{%(py9)
+000004c0: 7320 3d20 2528 7079 3729 730a 7b25 2870  s = %(py7)s.{%(p
+000004d0: 7937 2973 203d 2025 2870 7933 2973 0a7b  y7)s = %(py3)s.{
+000004e0: 2528 7079 3329 7320 3d20 2528 7079 3129  %(py3)s = %(py1)
+000004f0: 732e 6469 6374 0a7d 2865 7863 6c75 6465  s.dict.}(exclude
+00000500: 5f6e 6f6e 653d 2528 7079 3529 7329 0a7d  _none=%(py5)s).}
+00000510: 2e6b 6579 730a 7d28 290a 7d29 0a7d 203d  .keys.}().}).} =
+00000520: 3d20 2528 7079 3136 2973 da04 6c69 7374  = %(py16)s..list
+00000530: da01 7429 09da 0370 7930 da03 7079 31da  ..t)...py0..py1.
+00000540: 0370 7933 da03 7079 35da 0370 7937 da03  .py3..py5..py7..
+00000550: 7079 39da 0470 7931 31da 0470 7931 33da  py9..py11..py13.
+00000560: 0470 7931 367a 0f61 7373 6572 7420 2528  .py16z.assert %(
+00000570: 7079 3138 2973 da04 7079 3138 2901 da0d  py18)s..py18)...
+00000580: 6578 636c 7564 655f 756e 7365 7429 017a  exclude_unset).z
+00000590: ac25 2870 7931 3329 730a 7b25 2870 7931  .%(py13)s.{%(py1
+000005a0: 3329 7320 3d20 2528 7079 3029 7328 2528  3)s = %(py0)s(%(
+000005b0: 7079 3131 2973 0a7b 2528 7079 3131 2973  py11)s.{%(py11)s
+000005c0: 203d 2025 2870 7939 2973 0a7b 2528 7079   = %(py9)s.{%(py
+000005d0: 3929 7320 3d20 2528 7079 3729 730a 7b25  9)s = %(py7)s.{%
+000005e0: 2870 7937 2973 203d 2025 2870 7933 2973  (py7)s = %(py3)s
+000005f0: 0a7b 2528 7079 3329 7320 3d20 2528 7079  .{%(py3)s = %(py
+00000600: 3129 732e 6469 6374 0a7d 2865 7863 6c75  1)s.dict.}(exclu
+00000610: 6465 5f75 6e73 6574 3d25 2870 7935 2973  de_unset=%(py5)s
+00000620: 290a 7d2e 6b65 7973 0a7d 2829 0a7d 290a  ).}.keys.}().}).
+00000630: 7d20 3d3d 2025 2870 7931 3629 73da 0474  } == %(py16)s..t
+00000640: 6173 6bda 0029 0272 0600 0000 da07 7665  ask..).r......ve
+00000650: 7273 696f 6efa 0531 2e32 2e33 da07 736f  rsion..1.2.3..so
+00000660: 6d65 6f6e 6529 0372 0600 0000 7218 0000  meone).r....r...
+00000670: 00da 056f 776e 6572 7a28 6173 7365 7274  ...ownerz(assert
+00000680: 2025 2870 7932 2973 0a7b 2528 7079 3229   %(py2)s.{%(py2)
+00000690: 7320 3d20 2528 7079 3029 732e 6e61 6d65  s = %(py0)s.name
+000006a0: 0a7d 2902 720b 0000 00da 0370 7932 7a2b  .}).r......py2z+
+000006b0: 6173 7365 7274 2025 2870 7932 2973 0a7b  assert %(py2)s.{
+000006c0: 2528 7079 3229 7320 3d20 2528 7079 3029  %(py2)s = %(py0)
+000006d0: 732e 7665 7273 696f 6e0a 7d29 1272 0500  s.version.}).r..
+000006e0: 0000 7202 0000 00da 0464 6963 74da 046b  ..r......dict..k
+000006f0: 6579 7372 0900 0000 da0a 4070 7974 6573  eysr......@pytes
+00000700: 745f 6172 da11 5f63 616c 6c5f 7265 7072  t_ar.._call_repr
+00000710: 636f 6d70 6172 65da 0c40 7079 5f62 7569  compare..@py_bui
+00000720: 6c74 696e 73da 066c 6f63 616c 73da 185f  ltins..locals.._
+00000730: 7368 6f75 6c64 5f72 6570 725f 676c 6f62  should_repr_glob
+00000740: 616c 5f6e 616d 65da 095f 7361 6665 7265  al_name.._safere
+00000750: 7072 da0e 4173 7365 7274 696f 6e45 7272  pr..AssertionErr
+00000760: 6f72 da13 5f66 6f72 6d61 745f 6578 706c  or.._format_expl
+00000770: 616e 6174 696f 6eda 0670 7974 6573 74da  anation..pytest.
+00000780: 0672 6169 7365 7372 0300 0000 7206 0000  .raisesr....r...
+00000790: 0072 1800 0000 290d 720a 0000 00da 0b40  .r....).r......@
+000007a0: 7079 5f61 7373 6572 7432 da0b 4070 795f  py_assert2..@py_
+000007b0: 6173 7365 7274 34da 0b40 7079 5f61 7373  assert4..@py_ass
+000007c0: 6572 7436 da0b 4070 795f 6173 7365 7274  ert6..@py_assert
+000007d0: 38da 0c40 7079 5f61 7373 6572 7431 30da  8..@py_assert10.
+000007e0: 0c40 7079 5f61 7373 6572 7431 32da 0c40  .@py_assert12..@
+000007f0: 7079 5f61 7373 6572 7431 35da 0c40 7079  py_assert15..@py
+00000800: 5f61 7373 6572 7431 34da 0c40 7079 5f66  _assert14..@py_f
+00000810: 6f72 6d61 7431 37da 0c40 7079 5f66 6f72  ormat17..@py_for
+00000820: 6d61 7431 39da 0b40 7079 5f61 7373 6572  mat19..@py_asser
+00000830: 7431 da0b 4070 795f 666f 726d 6174 33a9  t1..@py_format3.
+00000840: 0072 3500 0000 fa3f 2f68 6f6d 652f 746f  .r5....?/home/to
+00000850: 6d6d 6173 6f2f 4672 6163 7461 6c2f 6672  mmaso/Fractal/fr
+00000860: 6163 7461 6c2f 6672 6163 7461 6c2f 636f  actal/fractal/co
+00000870: 6d6d 6f6e 2f74 6573 7473 2f74 6573 745f  mmon/tests/test_
+00000880: 7461 736b 2e70 79da 1074 6573 745f 7461  task.py..test_ta
+00000890: 736b 5f75 7064 6174 6509 0000 0073 2800  sk_update....s(.
+000008a0: 0000 0a02 0801 fe01 0e00 fe01 1000 0c02  ................
+000008b0: 0e01 1eff 0c02 0e01 1eff 0203 0201 0201  ................
+000008c0: 0201 06fd 0805 5601 5a01 7237 0000 0063  ......V.Z.r7...c
+000008d0: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+000008e0: 0900 0000 4300 0000 735a 0000 0074 0064  ....C...sZ...t.d
+000008f0: 0164 0264 0364 0464 0564 0664 0764 088d  .d.d.d.d.d.d.d..
+00000900: 077d 0074 017c 0083 0101 0074 02a0 0374  .}.t.|.....t...t
+00000910: 04a1 018f 0f01 0074 0064 0164 0264 098d  .......t.d.d.d..
+00000920: 0201 0057 0064 0004 0004 0083 0301 0064  ...W.d.........d
+00000930: 0053 0031 0073 2677 0101 0001 0001 0059  .S.1.s&w.......Y
+00000940: 0001 0064 0053 0029 0a4e 7216 0000 00da  ...d.S.).Nr.....
+00000950: 0673 6f75 7263 65da 0763 6f6d 6d61 6e64  .source..command
+00000960: da0a 696e 7075 745f 7479 7065 da0b 6f75  ..input_type..ou
+00000970: 7470 7574 5f74 7970 6572 1900 0000 721a  tput_typer....r.
+00000980: 0000 0029 0772 0600 0000 7238 0000 0072  ...).r....r8...r
+00000990: 3900 0000 723a 0000 0072 3b00 0000 7218  9...r:...r;...r.
+000009a0: 0000 0072 1b00 0000 2902 7206 0000 0072  ...r....).r....r
+000009b0: 3800 0000 2905 7204 0000 0072 0200 0000  8...).r....r....
+000009c0: 7227 0000 0072 2800 0000 7203 0000 0029  r'...r(...r....)
+000009d0: 0172 0a00 0000 7235 0000 0072 3500 0000  .r....r5...r5...
+000009e0: 7236 0000 00da 1074 6573 745f 7461 736b  r6.....test_task
+000009f0: 5f63 7265 6174 651f 0000 0073 1a00 0000  _create....s....
+00000a00: 0202 0201 0201 0201 0201 0201 0201 0201  ................
+00000a10: 06f9 0809 0c02 0e01 22ff 723c 0000 0029  ........".r<...)
+00000a20: 10da 0862 7569 6c74 696e 7372 2100 0000  ...builtinsr!...
+00000a30: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
+00000a40: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
+00000a50: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
+00000a60: 1f00 0000 7227 0000 00da 0864 6576 746f  ....r'.....devto
+00000a70: 6f6c 7372 0200 0000 da17 7079 6461 6e74  olsr......pydant
+00000a80: 6963 2e65 7272 6f72 5f77 7261 7070 6572  ic.error_wrapper
+00000a90: 7372 0300 0000 da07 7363 6865 6d61 7372  sr......schemasr
+00000aa0: 0400 0000 7205 0000 0072 3700 0000 723c  ....r....r7...r<
+00000ab0: 0000 0072 3500 0000 7235 0000 0072 3500  ...r5...r5...r5.
+00000ac0: 0000 7236 0000 00da 083c 6d6f 6475 6c65  ..r6.....<module
+00000ad0: 3e01 0000 0073 0e00 0000 2200 0c01 0c01  >....s....".....
+00000ae0: 0c02 0c01 0803 0c16                      ........
```

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr  6 11:30:39 2023 UTC, .py size: 1224 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-00000000: 6f0d 0d0a 0000 0000 5fad 2e64 c804 0000  o......._..d....
+00000000: 6f0d 0d0a 0000 0000 3d55 6f64 db05 0000  o.......=Uod....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6405 6406 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
 00000080: 2907 e900 0000 004e 2901 da05 6465 6275  )......N)...debu
 00000090: 6729 01da 0f56 616c 6964 6174 696f 6e45  g)...ValidationE
 000000a0: 7272 6f72 2901 da0a 5573 6572 4372 6561  rror)...UserCrea
 000000b0: 7465 6300 0000 0000 0000 0000 0000 000d  tec.............
-000000c0: 0000 0008 0000 0043 0000 0073 6803 0000  .......C...sh...
+000000c0: 0000 0008 0000 0043 0000 0073 8404 0000  .......C...s....
 000000d0: 7400 6401 6402 6403 8d02 7d00 7401 7c00  t.d.d.d...}.t.|.
 000000e0: 8301 0100 7c00 6a02 7d01 6400 7d02 7c01  ....|.j.}.d.}.|.
 000000f0: 7c02 7500 7d03 7c03 7349 7403 a004 6404  |.u.}.|.sIt...d.
 00000100: 7c03 6601 6405 7c01 7c02 6602 a104 6406  |.f.d.|.|.f...d.
 00000110: 7405 a006 a100 7600 732a 7403 a007 7c00  t.....v.s*t...|.
 00000120: a101 722f 7403 a008 7c00 a101 6e01 6406  ..r/t...|...n.d.
 00000130: 7403 a008 7c01 a101 7403 a008 7c02 a101  t...|...t...|...
@@ -61,79 +61,107 @@
 000003c0: 7d0b 7c0a 6a0f a010 a100 6419 1900 641a  }.|.j.....d...d.
 000003d0: 1900 7d03 7c0b 7c03 7600 7d0c 7c0c 9001  ..}.|.|.v.}.|...
 000003e0: 73ac 7403 a004 641b 7c0c 6601 641c 7c0b  s.t...d.|.f.d.|.
 000003f0: 7c03 6602 a104 7403 a008 7c0b a101 7403  |.f...t...|...t.
 00000400: a008 7c03 a101 641d 9c02 1600 7d08 6416  ..|...d.....}.d.
 00000410: 6417 7c08 6901 1600 7d09 7409 7403 a00a  d.|.i...}.t.t...
 00000420: 7c09 a101 8301 8201 6400 0400 7d0b 0400  |.......d...}...
-00000430: 7d0c 7d03 6400 5300 2920 4e7a 0561 4062  }.}.d.S.) Nz.a@b
-00000440: 2e63 da03 6173 6429 02da 0565 6d61 696c  .c..asd)...email
-00000450: da08 7061 7373 776f 7264 2901 da02 6973  ..password)...is
-00000460: 2901 7a32 2528 7079 3229 730a 7b25 2870  ).z2%(py2)s.{%(p
-00000470: 7932 2973 203d 2025 2870 7930 2973 2e73  y2)s = %(py0)s.s
-00000480: 6c75 726d 5f75 7365 720a 7d20 6973 2025  lurm_user.} is %
-00000490: 2870 7935 2973 da01 7529 03da 0370 7930  (py5)s..u)...py0
-000004a0: da03 7079 32da 0370 7935 7a0e 6173 7365  ..py2..py5z.asse
-000004b0: 7274 2025 2870 7937 2973 da03 7079 37da  rt %(py7)s..py7.
-000004c0: 0a73 6c75 726d 5f75 7365 7229 0372 0600  .slurm_user).r..
-000004d0: 0000 7207 0000 0072 0e00 0000 7a2e 6173  ..r....r....z.as
-000004e0: 7365 7274 2025 2870 7932 2973 0a7b 2528  sert %(py2)s.{%(
-000004f0: 7079 3229 7320 3d20 2528 7079 3029 732e  py2)s = %(py0)s.
-00000500: 736c 7572 6d5f 7573 6572 0a7d 2902 720a  slurm_user.}).r.
-00000510: 0000 0072 0b00 0000 7a02 2020 7a04 2f78  ...r....z.  z./x
-00000520: 7878 7a03 2020 2029 0372 0600 0000 7207  xxz.   ).r....r.
-00000530: 0000 00da 0963 6163 6865 5f64 6972 2901  .....cache_dir).
-00000540: fa02 3d3d 2901 7a31 2528 7079 3229 730a  ..==).z1%(py2)s.
-00000550: 7b25 2870 7932 2973 203d 2025 2870 7930  {%(py2)s = %(py0
-00000560: 2973 2e63 6163 6865 5f64 6972 0a7d 203d  )s.cache_dir.} =
-00000570: 3d20 2528 7079 3429 73da 0943 4143 4845  = %(py4)s..CACHE
-00000580: 5f44 4952 2903 720a 0000 0072 0b00 0000  _DIR).r....r....
-00000590: da03 7079 347a 0e61 7373 6572 7420 2528  ..py4z.assert %(
-000005a0: 7079 3629 73da 0370 7936 7a0f 6361 6e6e  py6)s..py6z.cann
-000005b0: 6f74 2062 6520 656d 7074 7972 0100 0000  ot be emptyr....
-000005c0: da03 6d73 6729 01da 0269 6e29 017a 1225  ..msg)...in).z.%
-000005d0: 2870 7931 2973 2069 6e20 2528 7079 3429  (py1)s in %(py4)
-000005e0: 7329 02da 0370 7931 7212 0000 00da 0378  s)...py1r......x
-000005f0: 7878 7a18 6d75 7374 2062 6520 616e 2061  xxz.must be an a
-00000600: 6273 6f6c 7574 6520 7061 7468 2911 7204  bsolute path).r.
-00000610: 0000 0072 0200 0000 720e 0000 00da 0a40  ...r....r......@
-00000620: 7079 7465 7374 5f61 72da 115f 6361 6c6c  pytest_ar.._call
-00000630: 5f72 6570 7263 6f6d 7061 7265 da0c 4070  _reprcompare..@p
-00000640: 795f 6275 696c 7469 6e73 da06 6c6f 6361  y_builtins..loca
-00000650: 6c73 da18 5f73 686f 756c 645f 7265 7072  ls.._should_repr
-00000660: 5f67 6c6f 6261 6c5f 6e61 6d65 da09 5f73  _global_name.._s
-00000670: 6166 6572 6570 72da 0e41 7373 6572 7469  aferepr..Asserti
-00000680: 6f6e 4572 726f 72da 135f 666f 726d 6174  onError.._format
-00000690: 5f65 7870 6c61 6e61 7469 6f6e da06 7079  _explanation..py
-000006a0: 7465 7374 da06 7261 6973 6573 7203 0000  test..raisesr...
-000006b0: 0072 0f00 0000 da05 7661 6c75 65da 0665  .r......value..e
-000006c0: 7272 6f72 7329 0d72 0900 0000 da0b 4070  rrors).r......@p
-000006d0: 795f 6173 7365 7274 31da 0b40 7079 5f61  y_assert1..@py_a
-000006e0: 7373 6572 7434 da0b 4070 795f 6173 7365  ssert4..@py_asse
-000006f0: 7274 33da 0b40 7079 5f66 6f72 6d61 7436  rt3..@py_format6
-00000700: da0b 4070 795f 666f 726d 6174 38da 0b40  ..@py_format8..@
-00000710: 7079 5f66 6f72 6d61 7433 7211 0000 00da  py_format3r.....
-00000720: 0b40 7079 5f66 6f72 6d61 7435 da0b 4070  .@py_format5..@p
-00000730: 795f 666f 726d 6174 37da 0165 da0b 4070  y_format7..e..@p
-00000740: 795f 6173 7365 7274 30da 0b40 7079 5f61  y_assert0..@py_a
-00000750: 7373 6572 7432 a900 722f 0000 00fa 3f2f  ssert2..r/....?/
-00000760: 686f 6d65 2f74 6f6d 6d61 736f 2f46 7261  home/tommaso/Fra
-00000770: 6374 616c 2f66 7261 6374 616c 2f66 7261  ctal/fractal/fra
-00000780: 6374 616c 2f63 6f6d 6d6f 6e2f 7465 7374  ctal/common/test
-00000790: 732f 7465 7374 5f75 7365 722e 7079 da10  s/test_user.py..
-000007a0: 7465 7374 5f75 7365 725f 6372 6561 7465  test_user_create
-000007b0: 0800 0000 732c 0000 000c 0208 018a 010e  ....s,..........
-000007c0: 0208 0150 010c 0210 011c ff04 0314 019c  ...P............
-000007d0: 010c 0210 011e ff0a 0276 010c 0210 011e  .........v......
-000007e0: ff0a 027a 0172 3100 0000 290e da08 6275  ...z.r1...)...bu
-000007f0: 696c 7469 6e73 721a 0000 00da 195f 7079  iltinsr......_py
-00000800: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
-00000810: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
-00000820: 6eda 0772 6577 7269 7465 7218 0000 0072  n..rewriter....r
-00000830: 2000 0000 da08 6465 7674 6f6f 6c73 7202   .....devtoolsr.
-00000840: 0000 00da 1770 7964 616e 7469 632e 6572  .....pydantic.er
-00000850: 726f 725f 7772 6170 7065 7273 7203 0000  ror_wrappersr...
-00000860: 00da 0773 6368 656d 6173 7204 0000 0072  ...schemasr....r
-00000870: 3100 0000 722f 0000 0072 2f00 0000 722f  1...r/...r/...r/
-00000880: 0000 0072 3000 0000 da08 3c6d 6f64 756c  ...r0.....<modul
-00000890: 653e 0100 0000 730a 0000 0022 000c 010c  e>....s...."....
-000008a0: 010c 020c 03                             .....
+00000430: 7d0c 7d03 7400 6401 6420 640a 6421 6422  }.}.t.d.d d.d!d"
+00000440: 6423 8d05 7d00 7401 7c00 8301 0100 7c00  d#..}.t.|.....|.
+00000450: 6a02 7d01 7c01 9001 73e8 640c 6406 7405  j.}.|...s.d.d.t.
+00000460: a006 a100 7600 9001 73d3 7403 a007 7c00  ....v...s.t...|.
+00000470: a101 9001 72d8 7403 a008 7c00 a101 6e01  ....r.t...|...n.
+00000480: 6406 7403 a008 7c01 a101 640d 9c02 1600  d.t...|...d.....
+00000490: 7d06 7409 7403 a00a 7c06 a101 8301 8201  }.t.t...|.......
+000004a0: 6400 7d01 7c00 6a0e 7d01 7c01 9002 7313  d.}.|.j.}.|...s.
+000004b0: 6424 6406 7405 a006 a100 7600 9001 73fe  d$d.t.....v...s.
+000004c0: 7403 a007 7c00 a101 9002 7203 7403 a008  t...|.....r.t...
+000004d0: 7c00 a101 6e01 6406 7403 a008 7c01 a101  |...n.d.t...|...
+000004e0: 640d 9c02 1600 7d06 7409 7403 a00a 7c06  d.....}.t.t...|.
+000004f0: a101 8301 8201 6400 7d01 7c00 6a11 7d01  ......d.}.|.j.}.
+00000500: 7c01 9002 733e 6425 6406 7405 a006 a100  |...s>d%d.t.....
+00000510: 7600 9002 7329 7403 a007 7c00 a101 9002  v...s)t...|.....
+00000520: 722e 7403 a008 7c00 a101 6e01 6406 7403  r.t...|...n.d.t.
+00000530: a008 7c01 a101 640d 9c02 1600 7d06 7409  ..|...d.....}.t.
+00000540: 7403 a00a 7c06 a101 8301 8201 6400 7d01  t...|.......d.}.
+00000550: 6400 5300 2926 4e7a 0561 4062 2e63 da03  d.S.)&Nz.a@b.c..
+00000560: 6173 6429 02da 0565 6d61 696c da08 7061  asd)...email..pa
+00000570: 7373 776f 7264 2901 da02 6973 2901 7a32  ssword)...is).z2
+00000580: 2528 7079 3229 730a 7b25 2870 7932 2973  %(py2)s.{%(py2)s
+00000590: 203d 2025 2870 7930 2973 2e73 6c75 726d   = %(py0)s.slurm
+000005a0: 5f75 7365 720a 7d20 6973 2025 2870 7935  _user.} is %(py5
+000005b0: 2973 da01 7529 03da 0370 7930 da03 7079  )s..u)...py0..py
+000005c0: 32da 0370 7935 7a0e 6173 7365 7274 2025  2..py5z.assert %
+000005d0: 2870 7937 2973 da03 7079 37da 0a73 6c75  (py7)s..py7..slu
+000005e0: 726d 5f75 7365 7229 0372 0600 0000 7207  rm_user).r....r.
+000005f0: 0000 0072 0e00 0000 7a2e 6173 7365 7274  ...r....z.assert
+00000600: 2025 2870 7932 2973 0a7b 2528 7079 3229   %(py2)s.{%(py2)
+00000610: 7320 3d20 2528 7079 3029 732e 736c 7572  s = %(py0)s.slur
+00000620: 6d5f 7573 6572 0a7d 2902 720a 0000 0072  m_user.}).r....r
+00000630: 0b00 0000 7a02 2020 7a04 2f78 7878 7a03  ....z.  z./xxxz.
+00000640: 2020 2029 0372 0600 0000 7207 0000 00da     ).r....r.....
+00000650: 0963 6163 6865 5f64 6972 2901 fa02 3d3d  .cache_dir)...==
+00000660: 2901 7a31 2528 7079 3229 730a 7b25 2870  ).z1%(py2)s.{%(p
+00000670: 7932 2973 203d 2025 2870 7930 2973 2e63  y2)s = %(py0)s.c
+00000680: 6163 6865 5f64 6972 0a7d 203d 3d20 2528  ache_dir.} == %(
+00000690: 7079 3429 73da 0943 4143 4845 5f44 4952  py4)s..CACHE_DIR
+000006a0: 2903 720a 0000 0072 0b00 0000 da03 7079  ).r....r......py
+000006b0: 347a 0e61 7373 6572 7420 2528 7079 3629  4z.assert %(py6)
+000006c0: 73da 0370 7936 7a0f 6361 6e6e 6f74 2062  s..py6z.cannot b
+000006d0: 6520 656d 7074 7972 0100 0000 da03 6d73  e emptyr......ms
+000006e0: 6729 01da 0269 6e29 017a 1225 2870 7931  g)...in).z.%(py1
+000006f0: 2973 2069 6e20 2528 7079 3429 7329 02da  )s in %(py4)s)..
+00000700: 0370 7931 7212 0000 00da 0378 7878 7a18  .py1r......xxxz.
+00000710: 6d75 7374 2062 6520 616e 2061 6273 6f6c  must be an absol
+00000720: 7574 6520 7061 7468 da03 7077 64da 0875  ute path..pwd..u
+00000730: 7365 726e 616d 657a 0a2f 736f 6d65 2f70  sernamez./some/p
+00000740: 6174 6829 0572 0600 0000 7207 0000 0072  ath).r....r....r
+00000750: 0e00 0000 7219 0000 0072 0f00 0000 7a2d  ....r....r....z-
+00000760: 6173 7365 7274 2025 2870 7932 2973 0a7b  assert %(py2)s.{
+00000770: 2528 7079 3229 7320 3d20 2528 7079 3029  %(py2)s = %(py0)
+00000780: 732e 6361 6368 655f 6469 720a 7d7a 2c61  s.cache_dir.}z,a
+00000790: 7373 6572 7420 2528 7079 3229 730a 7b25  ssert %(py2)s.{%
+000007a0: 2870 7932 2973 203d 2025 2870 7930 2973  (py2)s = %(py0)s
+000007b0: 2e75 7365 726e 616d 650a 7d29 1272 0400  .username.}).r..
+000007c0: 0000 7202 0000 0072 0e00 0000 da0a 4070  ..r....r......@p
+000007d0: 7974 6573 745f 6172 da11 5f63 616c 6c5f  ytest_ar.._call_
+000007e0: 7265 7072 636f 6d70 6172 65da 0c40 7079  reprcompare..@py
+000007f0: 5f62 7569 6c74 696e 73da 066c 6f63 616c  _builtins..local
+00000800: 73da 185f 7368 6f75 6c64 5f72 6570 725f  s.._should_repr_
+00000810: 676c 6f62 616c 5f6e 616d 65da 095f 7361  global_name.._sa
+00000820: 6665 7265 7072 da0e 4173 7365 7274 696f  ferepr..Assertio
+00000830: 6e45 7272 6f72 da13 5f66 6f72 6d61 745f  nError.._format_
+00000840: 6578 706c 616e 6174 696f 6eda 0670 7974  explanation..pyt
+00000850: 6573 74da 0672 6169 7365 7372 0300 0000  est..raisesr....
+00000860: 720f 0000 00da 0576 616c 7565 da06 6572  r......value..er
+00000870: 726f 7273 7219 0000 0029 0d72 0900 0000  rorsr....).r....
+00000880: da0b 4070 795f 6173 7365 7274 31da 0b40  ..@py_assert1..@
+00000890: 7079 5f61 7373 6572 7434 da0b 4070 795f  py_assert4..@py_
+000008a0: 6173 7365 7274 33da 0b40 7079 5f66 6f72  assert3..@py_for
+000008b0: 6d61 7436 da0b 4070 795f 666f 726d 6174  mat6..@py_format
+000008c0: 38da 0b40 7079 5f66 6f72 6d61 7433 7211  8..@py_format3r.
+000008d0: 0000 00da 0b40 7079 5f66 6f72 6d61 7435  .....@py_format5
+000008e0: da0b 4070 795f 666f 726d 6174 37da 0165  ..@py_format7..e
+000008f0: da0b 4070 795f 6173 7365 7274 30da 0b40  ..@py_assert0..@
+00000900: 7079 5f61 7373 6572 7432 a900 7231 0000  py_assert2..r1..
+00000910: 00fa 3f2f 686f 6d65 2f74 6f6d 6d61 736f  ..?/home/tommaso
+00000920: 2f46 7261 6374 616c 2f66 7261 6374 616c  /Fractal/fractal
+00000930: 2f66 7261 6374 616c 2f63 6f6d 6d6f 6e2f  /fractal/common/
+00000940: 7465 7374 732f 7465 7374 5f75 7365 722e  tests/test_user.
+00000950: 7079 da10 7465 7374 5f75 7365 725f 6372  py..test_user_cr
+00000960: 6561 7465 0800 0000 7342 0000 000c 0208  eate....sB......
+00000970: 018a 010e 0208 0150 010c 0210 011c ff04  .......P........
+00000980: 0314 019c 010c 0210 011e ff0a 0276 010c  .............v..
+00000990: 0210 011e ff0a 0276 0102 0202 0102 0102  .......v........
+000009a0: 0102 0102 0106 fb08 0756 0156 015a 0172  .........V.V.Z.r
+000009b0: 3300 0000 290e da08 6275 696c 7469 6e73  3...)...builtins
+000009c0: 721c 0000 00da 195f 7079 7465 7374 2e61  r......_pytest.a
+000009d0: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
+000009e0: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
+000009f0: 7269 7465 721a 0000 0072 2200 0000 da08  riter....r".....
+00000a00: 6465 7674 6f6f 6c73 7202 0000 00da 1770  devtoolsr......p
+00000a10: 7964 616e 7469 632e 6572 726f 725f 7772  ydantic.error_wr
+00000a20: 6170 7065 7273 7203 0000 00da 0773 6368  appersr......sch
+00000a30: 656d 6173 7204 0000 0072 3300 0000 7231  emasr....r3...r1
+00000a40: 0000 0072 3100 0000 7231 0000 0072 3200  ...r1...r1...r2.
+00000a50: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000a60: 730a 0000 0022 000c 010c 010c 020c 03    s....".........
```

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a1/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/test_dataset.py` & `fractal_client-1.3.0a1/fractal/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/test_manifest.py` & `fractal_client-1.3.0a1/fractal/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/test_project.py` & `fractal_client-1.3.0a1/fractal/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/test_state.py` & `fractal_client-1.3.0a1/fractal/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/test_user.py` & `fractal_client-1.3.0a1/fractal/common/tests/test_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,7 +27,19 @@
     debug(e.value)
     assert "cannot be empty" in e.value.errors()[0]["msg"]
     # With invalid cache_dir attribute
     with pytest.raises(ValidationError) as e:
         u = UserCreate(email="a@b.c", password="asd", cache_dir="xxx")
     debug(e.value)
     assert "must be an absolute path" in e.value.errors()[0]["msg"]
+    # With all attributes
+    u = UserCreate(
+        email="a@b.c",
+        password="pwd",
+        slurm_user="slurm_user",
+        username="username",
+        cache_dir="/some/path",
+    )
+    debug(u)
+    assert u.slurm_user
+    assert u.cache_dir
+    assert u.username
```

### Comparing `fractal_client-1.3.0a0/fractal/common/tests/test_workflow.py` & `fractal_client-1.3.0a1/fractal/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/config.py` & `fractal_client-1.3.0a1/fractal/config.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/interface.py` & `fractal_client-1.3.0a1/fractal/interface.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/fractal/parser.py` & `fractal_client-1.3.0a1/fractal/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -291,20 +291,14 @@
     help=(
         "Comma separated list of extra components for the package to be "
         "installed, e.g., `collect fractal-tasks-core "
         "--package-extras=torch,tensorflow` will trigger the installation of "
         "`fractal-tasks-core[torch,tensorflow]`"
     ),
 )
-task_collect_parser.add_argument(
-    "--private",
-    default=False,
-    action="store_true",
-    help="Intall tasks as private to the user (as opposed to global)",
-)
 
 # task check-collection
 task_check_collection_parser = task_subparsers.add_parser(
     "check-collection",
     description="Check status of background task collection processes",
     allow_abbrev=False,
 )
@@ -353,14 +347,19 @@
 task_new_parser.add_argument(
     "--output-type",
     help="The type of data the task expects as output",
     type=str,
     default="Any",
 )
 task_new_parser.add_argument(
+    "--version",
+    type=str,
+    help="Task version",
+)
+task_new_parser.add_argument(
     "--default-args-file",
     help="Path to JSON file with default task arguments",
     type=str,
 )
 task_new_parser.add_argument(
     "--meta-file",
     help="Path to JSON file with additional parameters useful for execution",
@@ -370,48 +369,93 @@
 # task edit
 task_edit_parser = task_subparsers.add_parser(
     "edit",
     description="Edit task",
     argument_default=ap.SUPPRESS,
     allow_abbrev=False,
 )
+
+task_edit_id_or_name_group = task_edit_parser.add_mutually_exclusive_group(
+    required=True
+)
+task_edit_id_or_name_group.add_argument(
+    "--id", help="ID of the task to edit", type=int
+)
+task_edit_id_or_name_group.add_argument(
+    "--name", help="Name of the task to edit", type=str
+)
+
+task_edit_parser.add_argument(
+    "--version",
+    type=str,
+    help=(
+        "Version of the task to edit "
+        "(only accepted in combination with --name)"
+    ),
+)
+task_edit_parser.add_argument("--new-name", help="New task name", type=str)
 task_edit_parser.add_argument(
-    "task_id_or_name", help="ID or name of task to edit", type=str
+    "--new-command", help="New task command", type=str
 )
-task_edit_parser.add_argument("--name", help="New task name")
-task_edit_parser.add_argument("--command", help="New task command")
 task_edit_parser.add_argument(
-    "--input-type",
+    "--new-input-type",
+    type=str,
     help="New input type",
 )
 task_edit_parser.add_argument(
-    "--output-type",
+    "--new-output-type",
+    type=str,
     help="New output type",
 )
 task_edit_parser.add_argument(
     "--default-args-file",
+    type=str,
     help=(
-        "Path to JSON serialised file containing "
-        "the task default arguments dictionary"
+        "Path to JSON serialised file containing updates to the current"
+        "`default_args` dictionary"
     ),
 )
 task_edit_parser.add_argument(
     "--meta-file",
-    help="Path to JSON serialised file containing the task meta dictionary",
+    type=str,
+    help=(
+        "Path to JSON serialised file containing updates to the current "
+        "`meta` dictionary"
+    ),
 )
+task_edit_parser.add_argument(
+    "--new-version",
+    type=str,
+    help="New version",
+)
+
 
 # task delete
 task_delete_parser = task_subparsers.add_parser(
     "delete",
     description="Delete task",
     argument_default=ap.SUPPRESS,
     allow_abbrev=False,
 )
+task_delete_id_or_name_group = task_delete_parser.add_mutually_exclusive_group(
+    required=True
+)
+task_delete_id_or_name_group.add_argument(
+    "--id", help="ID of the task to delete", type=int
+)
+task_delete_id_or_name_group.add_argument(
+    "--name", help="Name of the task to delete", type=str
+)
 task_delete_parser.add_argument(
-    "task_id_or_name", help="ID or name of task to delete", type=str
+    "--version",
+    type=str,
+    help=(
+        "Version of the task to delete "
+        "(only accepted in combination with --name)"
+    ),
 )
 
 
 # WORKFLOW GROUP
 
 workflow_parser = subparsers_main.add_parser(
     "workflow",
@@ -457,15 +501,20 @@
     "edit",
     description="Edit workflow",
     argument_default=ap.SUPPRESS,
     allow_abbrev=False,
 )
 workflow_edit_parser.add_argument("project_id", type=int, help="Project ID")
 workflow_edit_parser.add_argument("workflow_id", type=int, help="Workflow ID")
-workflow_edit_parser.add_argument("--name", type=str, help="New workflow name")
+workflow_edit_parser.add_argument(
+    "--new-name",
+    type=str,
+    help="New workflow name",
+    required=True,
+)
 
 # workflow delete
 workflow_delete_parser = workflow_subparsers.add_parser(
     "delete",
     description="Delete workflow",
     allow_abbrev=False,
 )
@@ -485,16 +534,32 @@
     "project_id", type=int, help="Project ID"
 )
 workflow_add_task_parser.add_argument(
     "workflow_id",
     type=int,
     help="Workflow ID",
 )
+
+workflow_add_task_id_or_name_group = (
+    workflow_add_task_parser.add_mutually_exclusive_group(required=True)
+)
+workflow_add_task_id_or_name_group.add_argument(
+    "--task-id", help="ID of the task to add", type=int
+)
+workflow_add_task_id_or_name_group.add_argument(
+    "--task-name", help="Name of the task to add", type=str
+)
+
 workflow_add_task_parser.add_argument(
-    "task_id_or_name", help="ID or name of the new task", type=str
+    "--task-version",
+    type=str,
+    help=(
+        "Version of task to add "
+        "(only accepted in combination with --task-name)"
+    ),
 )
 workflow_add_task_parser.add_argument(
     "--order", help="Order of this task within the workflow's task list"
 )
 workflow_add_task_parser.add_argument(
     "--args-file",
     help=(
@@ -733,14 +798,19 @@
 )
 user_register_parser.add_argument(
     "--slurm-user",
     help="Username to login into SLURM cluster",
     required=False,
 )
 user_register_parser.add_argument(
+    "--username",
+    help="Username associated to the user",
+    required=False,
+)
+user_register_parser.add_argument(
     "--superuser",
     help="Give superuser privileges to the new user",
     action="store_true",
     required=False,
 )
 
 # user list
@@ -779,15 +849,17 @@
     ),
     type=str,
     required=False,
 )
 user_edit_parser.add_argument(
     "--new-slurm-user", help="New SLURM username", type=str, required=False
 )
-
+user_edit_parser.add_argument(
+    "--new-username", help="New user username", type=str, required=False
+)
 user_edit_parser_superuser = user_edit_parser.add_mutually_exclusive_group()
 user_edit_parser_superuser.add_argument(
     "--make-superuser",
     help="Give superuser privileges to user",
     action="store_true",
     required=False,
 )
```

### Comparing `fractal_client-1.3.0a0/fractal/response.py` & `fractal_client-1.3.0a1/fractal/response.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a0/pyproject.toml` & `fractal_client-1.3.0a1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-client"
-version = "1.3.0a0"
+version = "1.3.0a1"
 description = "Client component of the Fractal analytics platform"
 authors = [
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
 readme = "README.md"
@@ -16,19 +16,19 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^0.20.0"
 rich = "^12.5.1"
 httpx = "^0.23.0"
 PyJWT = "^2.4.0"
-pydantic = "^1.10.1"
-sqlmodel = "^0.0.8"
+pydantic = ">=1.10.8"
 fastapi-users = "^10.4.1"
 
 [tool.poetry.group.dev.dependencies]
+sqlmodel = "^0.0.8"
 devtools = "^0.9.0"
 pytest = "^7.1.2"
 bumpver = "^2022.1118"
 pytest-asyncio = "^0.19.0"
 fractal-server = { git = "https://github.com/fractal-analytics-platform/fractal-server.git", branch = "main" }
 coverage = {extras = ["toml"], version = "^6.5.0"}
 pytest-pretty = "^1.0.1"
@@ -43,15 +43,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.bumpver]
-current_version = "1.3.0a0"
+current_version = "1.3.0a1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_client-1.3.0a0/setup.py` & `fractal_client-1.3.0a1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fractal-client
+Version: 1.3.0a1
+Summary: Client component of the Fractal analytics platform
+Home-page: https://github.com/fractal-analytics-platform/fractal
+License: BSD-3-Clause
+Author: Tommaso Comparin
+Author-email: tommaso.comparin@exact-lab.it
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
+Requires-Dist: fastapi-users (>=10.4.1,<11.0.0)
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: pydantic (>=1.10.8)
+Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Description-Content-Type: text/markdown
+
+# Fractal Client
+
+[![PyPI version](https://img.shields.io/pypi/v/fractal-client?color=gree)](https://pypi.org/project/fractal-client/)
+[![CI Status](https://github.com/fractal-analytics-platform/fractal/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal/actions/workflows/ci.yml)
+[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal/blob/python-coverage-comment-action-data/htmlcov/index.html)
+[![Documentation Status](https://github.com/fractal-analytics-platform/fractal/actions/workflows/documentation.yaml/badge.svg)](https://fractal-analytics-platform.github.io/fractal)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+
+Fractal is a framework to process high-content imaging data at scale and prepare it for interactive visualization.
+
+![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)
+
+Fractal provides distributed workflows that convert TBs of image data into OME-Zarr files. The platform then processes the 3D image data by applying tasks like illumination correction, maximum intensity projection, 3D segmentation using [cellpose](https://cellpose.readthedocs.io/en/latest/) and measurements using [napari workflows](https://github.com/haesleinhuepf/napari-workflows). The pyramidal OME-Zarr files enable interactive visualization in the napari viewer.
+
+This is the repository that contains the **Fractal client**. Find more information about Fractal in general and the other repositories at the [Fractal home page](https://fractal-analytics-platform.github.io).
+
+## Documentation
 
-packages = \
-['fractal',
- 'fractal.cmd',
- 'fractal.common',
- 'fractal.common.schemas',
- 'fractal.common.tests']
-
-package_data = \
-{'': ['*'], 'fractal.common': ['.github/workflows/*']}
-
-install_requires = \
-['PyJWT>=2.4.0,<3.0.0',
- 'fastapi-users>=10.4.1,<11.0.0',
- 'httpx>=0.23.0,<0.24.0',
- 'pydantic>=1.10.1,<2.0.0',
- 'python-dotenv>=0.20.0,<0.21.0',
- 'rich>=12.5.1,<13.0.0',
- 'sqlmodel>=0.0.8,<0.0.9']
-
-entry_points = \
-{'console_scripts': ['fractal = fractal.__main__:run',
-                     'fractal_new = fractal.new:run',
-                     'fractal_old = fractal.old:run']}
-
-setup_kwargs = {
-    'name': 'fractal-client',
-    'version': '1.3.0a0',
-    'description': 'Client component of the Fractal analytics platform',
-    'long_description': '# Fractal Client\n\n[![PyPI version](https://img.shields.io/pypi/v/fractal-client?color=gree)](https://pypi.org/project/fractal-client/)\n[![CI Status](https://github.com/fractal-analytics-platform/fractal/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal/actions/workflows/ci.yml)\n[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal/blob/python-coverage-comment-action-data/htmlcov/index.html)\n[![Documentation Status](https://github.com/fractal-analytics-platform/fractal/actions/workflows/documentation.yaml/badge.svg)](https://fractal-analytics-platform.github.io/fractal)\n[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\nFractal is a framework to process high-content imaging data at scale and prepare it for interactive visualization.\n\n![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)\n\nFractal provides distributed workflows that convert TBs of image data into OME-Zarr files. The platform then processes the 3D image data by applying tasks like illumination correction, maximum intensity projection, 3D segmentation using [cellpose](https://cellpose.readthedocs.io/en/latest/) and measurements using [napari workflows](https://github.com/haesleinhuepf/napari-workflows). The pyramidal OME-Zarr files enable interactive visualization in the napari viewer.\n\nThis is the repository that contains the **Fractal client**. Find more information about Fractal in general and the other repositories at the [Fractal home page](https://fractal-analytics-platform.github.io).\n\n## Documentation\n\nSee https://fractal-analytics-platform.github.io/fractal.\n\n# Contributors and license\n\nUnless otherwise stated in each individual module, all Fractal components are released according to a BSD 3-Clause License, and Copyright is with Friedrich Miescher Institute for Biomedical Research and University of Zurich.\n\nFractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa) & [@jacopo-exact](https://github.com/jacopo-exact) from [eXact lab S.r.l.](exact-lab.it).\n',
-    'author': 'Tommaso Comparin',
-    'author_email': 'tommaso.comparin@exact-lab.it',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/fractal-analytics-platform/fractal',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+See https://fractal-analytics-platform.github.io/fractal.
 
+# Contributors and license
+
+Unless otherwise stated in each individual module, all Fractal components are released according to a BSD 3-Clause License, and Copyright is with Friedrich Miescher Institute for Biomedical Research and University of Zurich.
+
+Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa) & [@jacopo-exact](https://github.com/jacopo-exact) from [eXact lab S.r.l.](exact-lab.it).
 
-setup(**setup_kwargs)
```

