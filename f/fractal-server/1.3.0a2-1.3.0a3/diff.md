# Comparing `tmp/fractal_server-1.3.0a2.tar.gz` & `tmp/fractal_server-1.3.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.3.0a2.tar", max compression
+gzip compressed data, was "fractal_server-1.3.0a3.tar", max compression
```

## Comparing `fractal_server-1.3.0a2.tar` & `fractal_server-1.3.0a3.tar`

### file list

```diff
@@ -1,132 +1,135 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.3.0a2/LICENSE
--rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.3.0a2/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.3.0a2/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-05-15 12:56:24.711398 fractal_server-1.3.0a2/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-04-19 11:52:26.187278 fractal_server-1.3.0a2/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.3.0a2/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.3.0a2/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      952 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.3.0a2/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     6314 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/app/api/v1/_aux_functions.py
--rw-r--r--   0        0        0     6974 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/app/api/v1/dataset.py
--rw-r--r--   0        0        0     4817 2023-05-15 12:45:48.614516 fractal_server-1.3.0a2/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0     8880 2023-05-15 09:02:05.627121 fractal_server-1.3.0a2/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    12661 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    12202 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     3081 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.3.0a2/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3370 2023-05-12 09:56:36.874307 fractal_server-1.3.0a2/fractal_server/app/models/job.py
--rw-r--r--   0        0        0      309 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     2295 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     2534 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.3.0a2/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.3.0a2/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5464 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a2/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0     8969 2023-05-15 10:36:57.758906 fractal_server-1.3.0a2/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    19458 2023-05-12 12:34:32.122055 fractal_server-1.3.0a2/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     5464 2023-05-12 12:34:32.122055 fractal_server-1.3.0a2/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.3.0a2/fractal_server/app/runner/_local/_local_config.py
--rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.3.0a2/fractal_server/app/runner/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.3.0a2/fractal_server/app/runner/_local/executor.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3839 2023-05-12 12:34:32.122055 fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     4331 2023-05-15 10:36:57.758906 fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    19861 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    42127 2023-05-15 10:36:57.758906 fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     7900 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0    11324 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.3.0a2/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.3.0a2/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.3.0a2/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.3.0a2/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.3.0a2/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.3.0a2/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       48 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.3.0a2/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1658 2023-05-12 09:55:08.603302 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3612 2023-05-08 12:02:12.597892 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1205 2023-05-08 12:02:12.605892 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     4943 2023-05-09 12:55:27.450288 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     1135 2023-05-12 09:55:08.619302 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     3957 2023-05-09 12:55:27.454288 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1135 2023-05-12 09:54:53.927466 fractal_server-1.3.0a2/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.3.0a2/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2527 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      695 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     4323 2023-05-09 11:24:30.681084 fractal_server-1.3.0a2/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0      980 2023-05-12 09:54:53.927466 fractal_server-1.3.0a2/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2502 2023-05-09 11:24:30.681084 fractal_server-1.3.0a2/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      620 2023-05-09 18:15:54.737187 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      873 2023-05-08 12:02:13.009887 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2236 2023-05-08 12:02:13.013887 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2227 2023-05-08 12:02:13.017887 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2925 2023-05-09 18:15:54.765188 fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-05-09 11:24:30.681084 fractal_server-1.3.0a2/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0      541 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0      748 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0     1224 2023-05-08 12:01:46.018194 fractal_server-1.3.0a2/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-05-09 11:24:30.681084 fractal_server-1.3.0a2/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    12164 2023-05-12 12:34:32.122055 fractal_server-1.3.0a2/fractal_server/config.py
--rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.3.0a2/fractal_server/logger.py
--rw-r--r--   0        0        0     5726 2023-05-12 12:34:32.122055 fractal_server-1.3.0a2/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.3.0a2/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.3.0a2/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.3.0a2/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      751 2023-05-12 09:56:36.874307 fractal_server-1.3.0a2/fractal_server/migrations/versions/bb1cca2acc40_add_applyworkflow_end_timestamp.py
--rw-r--r--   0        0        0     8438 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/migrations/versions/e8f4051440be_new_initial_schema.py
--rw-r--r--   0        0        0      745 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/migrations/versions/fda995215ae9_drop_applyworkflow_overwrite_input.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.3.0a2/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.3.0a2/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.3.0a2/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    12869 2023-05-12 06:48:40.382595 fractal_server-1.3.0a2/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.3.0a2/fractal_server/utils.py
--rw-r--r--   0        0        0     2667 2023-05-15 12:56:24.711398 fractal_server-1.3.0a2/pyproject.toml
--rw-r--r--   0        0        0     4078 1970-01-01 00:00:00.000000 fractal_server-1.3.0a2/setup.py
--rw-r--r--   0        0        0     3596 1970-01-01 00:00:00.000000 fractal_server-1.3.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.3.0a3/LICENSE
+-rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.3.0a3/README.md
+-rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.3.0a3/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-06-12 06:37:28.730485 fractal_server-1.3.0a3/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-05-25 12:06:55.503794 fractal_server-1.3.0a3/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.3.0a3/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.3.0a3/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      952 2023-05-12 06:48:40.382595 fractal_server-1.3.0a3/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.3.0a3/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     6314 2023-05-12 06:48:40.382595 fractal_server-1.3.0a3/fractal_server/app/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0     7624 2023-05-23 13:25:45.067972 fractal_server-1.3.0a3/fractal_server/app/api/v1/dataset.py
+-rw-r--r--   0        0        0     4817 2023-05-15 12:45:48.614516 fractal_server-1.3.0a3/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0     8880 2023-05-15 09:02:05.627121 fractal_server-1.3.0a3/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    15343 2023-06-07 12:54:11.623397 fractal_server-1.3.0a3/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    12501 2023-05-29 15:02:27.725371 fractal_server-1.3.0a3/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     3081 2023-05-12 06:48:40.382595 fractal_server-1.3.0a3/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.3.0a3/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3412 2023-05-29 08:51:11.986940 fractal_server-1.3.0a3/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0      309 2023-05-12 06:48:40.382595 fractal_server-1.3.0a3/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     2355 2023-05-29 08:51:11.986940 fractal_server-1.3.0a3/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     2563 2023-05-29 09:51:02.494983 fractal_server-1.3.0a3/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1119 2023-05-29 08:51:11.986940 fractal_server-1.3.0a3/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     1591 2023-06-08 09:21:57.166713 fractal_server-1.3.0a3/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5948 2023-06-08 09:22:21.105956 fractal_server-1.3.0a3/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a3/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0     8969 2023-05-15 10:36:57.758906 fractal_server-1.3.0a3/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    19523 2023-06-08 09:22:21.105956 fractal_server-1.3.0a3/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     5464 2023-05-12 12:34:32.122055 fractal_server-1.3.0a3/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.3.0a3/fractal_server/app/runner/_local/_local_config.py
+-rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.3.0a3/fractal_server/app/runner/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.3.0a3/fractal_server/app/runner/_local/executor.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3839 2023-05-12 12:34:32.122055 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     4331 2023-05-15 10:36:57.758906 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    19861 2023-05-12 06:48:40.382595 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    42200 2023-05-18 09:57:35.703959 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     7900 2023-06-08 08:33:26.930560 fractal_server-1.3.0a3/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0    11324 2023-05-12 06:48:40.382595 fractal_server-1.3.0a3/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.3.0a3/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.3.0a3/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.3.0a3/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.3.0a3/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.3.0a3/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.3.0a3/fractal_server/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       57 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      614 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      425 2023-05-26 06:49:50.432129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1624 2023-05-26 06:49:50.432129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
+-rw-r--r--   0        0        0     4082 2023-06-06 13:10:35.738263 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
+-rw-r--r--   0        0        0     3551 2023-05-26 06:49:50.436129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
+-rw-r--r--   0        0        0     1179 2023-05-26 06:49:50.444129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     2719 2023-06-06 13:10:35.746263 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     3112 2023-05-26 06:49:50.448129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1216 2023-05-26 06:49:50.448129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     3896 2023-05-26 06:49:50.452129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1117 2023-05-26 06:47:44.353797 fractal_server-1.3.0a3/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     3479 2023-06-06 13:04:16.393219 fractal_server-1.3.0a3/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2483 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      673 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     2578 2023-06-06 13:04:16.393219 fractal_server-1.3.0a3/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0     2741 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/schemas/task_collection.py
+-rw-r--r--   0        0        0     1216 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2457 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      620 2023-05-09 18:15:54.737187 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1255 2023-06-06 07:10:27.608505 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2806 2023-05-26 06:49:50.864124 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1238 2023-05-26 06:49:50.868124 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2685 2023-05-26 06:49:50.868124 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2925 2023-05-09 18:15:54.765188 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-05-09 11:24:30.681084 fractal_server-1.3.0a3/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0     1420 2023-06-06 07:08:01.329849 fractal_server-1.3.0a3/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0     1190 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0      773 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/tests/test_task_collection.py
+-rw-r--r--   0        0        0     1499 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-05-09 11:24:30.681084 fractal_server-1.3.0a3/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    12164 2023-05-12 12:34:32.122055 fractal_server-1.3.0a3/fractal_server/config.py
+-rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.3.0a3/fractal_server/logger.py
+-rw-r--r--   0        0        0     5849 2023-05-26 06:42:41.017595 fractal_server-1.3.0a3/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.3.0a3/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.3.0a3/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.3.0a3/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2023-06-08 09:21:57.166713 fractal_server-1.3.0a3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     8770 2023-05-29 15:02:27.725371 fractal_server-1.3.0a3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0      746 2023-06-08 09:21:57.166713 fractal_server-1.3.0a3/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.3.0a3/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.3.0a3/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.3.0a3/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    15725 2023-06-12 06:36:49.598978 fractal_server-1.3.0a3/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.3.0a3/fractal_server/utils.py
+-rw-r--r--   0        0        0     2689 2023-06-12 06:37:28.726485 fractal_server-1.3.0a3/pyproject.toml
+-rw-r--r--   0        0        0     3631 1970-01-01 00:00:00.000000 fractal_server-1.3.0a3/PKG-INFO
```

### Comparing `fractal_server-1.3.0a2/LICENSE` & `fractal_server-1.3.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/README.md` & `fractal_server-1.3.0a3/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/__main__.py` & `fractal_server-1.3.0a3/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/alembic.ini` & `fractal_server-1.3.0a3/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/api/__init__.py` & `fractal_server-1.3.0a3/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/api/v1/_aux_functions.py` & `fractal_server-1.3.0a3/fractal_server/app/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/api/v1/dataset.py` & `fractal_server-1.3.0a3/fractal_server/app/api/v1/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import Optional
 
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import Response
 from fastapi import status
+from sqlmodel import or_
 from sqlmodel import select
 
 from ...db import AsyncSession
 from ...db import get_db
+from ...models import ApplyWorkflow
 from ...models import Dataset
 from ...models import DatasetCreate
 from ...models import DatasetRead
 from ...models import DatasetUpdate
 from ...models import Resource
 from ...models import ResourceCreate
 from ...models import ResourceRead
@@ -120,14 +122,33 @@
     output = await _get_dataset_check_owner(
         project_id=project_id,
         dataset_id=dataset_id,
         user_id=user.id,
         db=db,
     )
     dataset = output["dataset"]
+
+    # Check that no ApplyWorkflow is in relationship with the current Dataset
+    stm = select(ApplyWorkflow).filter(
+        or_(
+            ApplyWorkflow.input_dataset_id == dataset_id,
+            ApplyWorkflow.output_dataset_id == dataset_id,
+        )
+    )
+    res = await db.execute(stm)
+    job = res.scalars().first()
+    if job:
+        raise HTTPException(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=(
+                f"Cannot remove dataset {dataset_id}: "
+                f"it's still linked to job {job.id}."
+            ),
+        )
+
     await db.delete(dataset)
     await db.commit()
     await db.close()
     return Response(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.post(
```

### Comparing `fractal_server-1.3.0a2/fractal_server/app/api/v1/job.py` & `fractal_server-1.3.0a3/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/api/v1/project.py` & `fractal_server-1.3.0a3/fractal_server/app/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/api/v1/task.py` & `fractal_server-1.3.0a3/fractal_server/app/api/v1/task.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,20 +37,21 @@
 from ....tasks.collection import inspect_package
 from ...db import AsyncSession
 from ...db import DBSyncSession
 from ...db import get_db
 from ...db import get_sync_db
 from ...models import State
 from ...models import Task
-from ...security import current_active_superuser
 from ...security import current_active_user
 from ...security import User
 
 router = APIRouter()
 
+logger = set_logger(__name__)
+
 
 async def _background_collect_pip(
     state_id: int,
     venv_path: Path,
     task_pkg: _TaskCollectPip,
 ) -> None:
     """
@@ -174,64 +175,80 @@
 )
 async def collect_tasks_pip(
     task_collect: TaskCollectPip,
     background_tasks: BackgroundTasks,
     response: Response,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
-    public: bool = True,
 ) -> StateRead:  # State[TaskCollectStatus]
     """
     Task collection endpoint
 
     Trigger the creation of a dedicated virtual environment, the installation
     of a package and the collection of tasks as advertised in the manifest.
     """
 
     logger = set_logger(logger_name="collect_tasks_pip")
 
     # Validate payload as _TaskCollectPip, which has more strict checks than
     # TaskCollectPip
     try:
-        task_pkg = _TaskCollectPip(**task_collect.dict())
+        task_pkg = _TaskCollectPip(**task_collect.dict(exclude_unset=True))
     except ValidationError as e:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=f"Invalid task-collection object. Original error: {e}",
         )
 
     with TemporaryDirectory() as tmpdir:
         try:
+            # Copy or download the package wheel file to tmpdir
             if task_pkg.is_local_package:
                 shell_copy(task_pkg.package_path.as_posix(), tmpdir)
                 pkg_path = Path(tmpdir) / task_pkg.package_path.name
             else:
                 pkg_path = await download_package(
                     task_pkg=task_pkg, dest=tmpdir
                 )
-
-            version_manifest = inspect_package(pkg_path)
-
-            task_pkg.version = version_manifest["version"]
+            # Read package info from wheel file, and override the ones coming
+            # from the request body
+            pkg_info = inspect_package(pkg_path)
+            task_pkg.package_name = pkg_info["pkg_name"]
+            task_pkg.package_version = pkg_info["pkg_version"]
+            task_pkg.package_manifest = pkg_info["pkg_manifest"]
             task_pkg.check()
         except Exception as e:
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
                 detail=f"Invalid package or manifest. Original error: {e}",
             )
 
     try:
-        pkg_user = None if public else user.slurm_user
-        venv_path = create_package_dir_pip(task_pkg=task_pkg, user=pkg_user)
+        venv_path = create_package_dir_pip(task_pkg=task_pkg)
     except FileExistsError:
-        venv_path = create_package_dir_pip(
-            task_pkg=task_pkg, user=pkg_user, create=False
-        )
+        venv_path = create_package_dir_pip(task_pkg=task_pkg, create=False)
         try:
             task_collect_status = get_collection_data(venv_path)
+            for task in task_collect_status.task_list:
+                db_task = await db.get(Task, task.id)
+                if (
+                    (not db_task)
+                    or db_task.source != task.source
+                    or db_task.name != task.name
+                ):
+                    await db.close()
+                    raise HTTPException(
+                        status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+                        detail=(
+                            "Cannot collect package. Folder already exists, "
+                            f"but task {task.id} does not exists or it does "
+                            f"not have the expected source ({task.source}) or "
+                            f"name ({task.name})."
+                        ),
+                    )
         except FileNotFoundError as e:
             await db.close()
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
                 detail=(
                     "Cannot collect package. Possible reason: another "
                     "collection of the same package is in progress. "
@@ -340,27 +357,50 @@
     return task
 
 
 @router.patch("/{task_id}", response_model=TaskRead)
 async def patch_task(
     task_id: int,
     task_update: TaskUpdate,
-    user: User = Depends(current_active_superuser),
+    user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
 ) -> Optional[TaskRead]:
     """
-    Edit a specific task
+    Edit a specific task (restricted to superusers and task owner)
     """
+
     if task_update.source:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail="patch_task endpoint cannot set `source`",
         )
 
+    # Retrieve task from database
     db_task = await db.get(Task, task_id)
+
+    # This check constitutes a preliminary version of access control:
+    # if the current user is not a superuser and differs from the task owner
+    # (including when `owner is None`), we raise an 403 HTTP Exception.
+    if not user.is_superuser:
+        if db_task.owner is None:
+            raise HTTPException(
+                status_code=status.HTTP_403_FORBIDDEN,
+                detail=("Only a superuser can edit a task with `owner=None`."),
+            )
+        else:
+            owner = user.username or user.slurm_user
+            if owner != db_task.owner:
+                raise HTTPException(
+                    status_code=status.HTTP_403_FORBIDDEN,
+                    detail=(
+                        f"Current user ({owner}) cannot modify task "
+                        f"({task_id}) with different owner ({db_task.owner})."
+                    ),
+                )
+
     update = task_update.dict(exclude_unset=True)
     for key, value in update.items():
         if isinstance(value, str):
             setattr(db_task, key, value)
         elif isinstance(value, dict):
             current_dict = deepcopy(getattr(db_task, key))
             current_dict.update(value)
@@ -382,20 +422,42 @@
     task: TaskCreate,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
 ) -> Optional[TaskRead]:
     """
     Create a new task
     """
+    # Set task.owner attribute
+    if user.username:
+        owner = user.username
+    elif user.slurm_user:
+        owner = user.slurm_user
+    else:
+        raise HTTPException(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=(
+                "Cannot add a new task because current user does not "
+                "have `username` or `slurm_user` attributes."
+            ),
+        )
+
+    # Prepend owner to task.source
+    task.source = f"{owner}:{task.source}"
+
+    # Verify that source is not already in use (note: this check is only useful
+    # to provide a user-friendly error message, but `task.source` uniqueness is
+    # already guaranteed by a constraint in the table definition).
     stm = select(Task).where(Task.source == task.source)
     res = await db.execute(stm)
     if res.scalars().all():
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-            detail=f"Task with source={task.source} already in use",
+            detail=f'Task source "{task.source}" already in use',
         )
-    db_task = Task.from_orm(task)
+
+    # Add task
+    db_task = Task(**task.dict(), owner=owner)
     db.add(db_task)
     await db.commit()
     await db.refresh(db_task)
     await db.close()
     return db_task
```

### Comparing `fractal_server-1.3.0a2/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.3.0a3/fractal_server/app/api/v1/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import Response
 from fastapi import status
 from sqlmodel import select
 
+from ....logger import close_logger
+from ....logger import set_logger
 from ...db import AsyncSession
 from ...db import get_db
+from ...models import ApplyWorkflow
 from ...models import Task
 from ...models import Workflow
 from ...models import WorkflowCreate
 from ...models import WorkflowExport
 from ...models import WorkflowImport
 from ...models import WorkflowRead
 from ...models import WorkflowTaskCreate
@@ -177,14 +180,27 @@
     Delte a workflow
     """
 
     workflow = await _get_workflow_check_owner(
         project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
     )
 
+    # Check that no ApplyWorkflow is in relationship with the current Workflow
+    stm = select(ApplyWorkflow).where(ApplyWorkflow.workflow_id == workflow_id)
+    res = await db.execute(stm)
+    job = res.scalars().first()
+    if job:
+        raise HTTPException(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=(
+                f"Cannot remove workflow {workflow_id}: "
+                f"it's still linked to job {job.id}."
+            ),
+        )
+
     await db.delete(workflow)
     await db.commit()
 
     return Response(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.get(
@@ -199,14 +215,26 @@
 ) -> Optional[WorkflowExport]:
     """
     Export an existing workflow, after stripping all IDs
     """
     workflow = await _get_workflow_check_owner(
         project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
     )
+    # Emit a warning when exporting a workflow with custom tasks
+    logger = set_logger(None)
+    for wftask in workflow.task_list:
+        if wftask.task.owner is not None:
+            logger.warning(
+                f"Custom tasks (like the one with id={wftask.task.id} and "
+                f'source="{wftask.task.source}") are not meant to be '
+                "portable; re-importing this workflow may not work as "
+                "expected."
+            )
+    close_logger(logger)
+
     await db.close()
     return workflow
 
 
 @router.post(
     "/project/{project_id}/workflow/import/",
     response_model=WorkflowRead,
@@ -233,45 +261,29 @@
     )
 
     await _check_workflow_exists(
         name=workflow.name, project_id=project_id, db=db
     )
 
     # Check that all required tasks are available
-    # NOTE: by now we go through the pair (source, name), but later on we may
-    # combine them into source -- see issue #293.
     tasks = [wf_task.task for wf_task in workflow.task_list]
-    sourcename_to_id = {}
+    source_to_id = {}
     for task in tasks:
         source = task.source
-        name = task.name
-        if not (source, name) in sourcename_to_id.keys():
+        if source not in source_to_id.keys():
             stm = select(Task).where(Task.source == source)
             tasks_by_source = (await db.execute(stm)).scalars().all()
-            if not tasks_by_source:
+            if len(tasks_by_source) != 1:
                 raise HTTPException(
                     status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-                    detail=(f"Found 0 tasks with {source=}."),
-                )
-            else:
-                stm = (
-                    select(Task)
-                    .where(Task.source == source)
-                    .where(Task.name == name)
+                    detail=(
+                        f"Found {len(tasks_by_source)} tasks with {source=}."
+                    ),
                 )
-                current_task = (await db.execute(stm)).scalars().all()
-                if len(current_task) != 1:
-                    raise HTTPException(
-                        status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-                        detail=(
-                            f"Found {len(current_task)} tasks with "
-                            f"{name =} and {source=}."
-                        ),
-                    )
-                sourcename_to_id[(source, name)] = current_task[0].id
+            source_to_id[source] = tasks_by_source[0].id
 
     # Create new Workflow (with empty task_list)
     db_workflow = Workflow(
         project_id=project_id,
         **workflow.dict(exclude_none=True, exclude={"task_list"}),
     )
     db.add(db_workflow)
@@ -279,16 +291,15 @@
     await db.refresh(db_workflow)
 
     # Insert tasks
     async with db:
         for _, wf_task in enumerate(workflow.task_list):
             # Identify task_id
             source = wf_task.task.source
-            name = wf_task.task.name
-            task_id = sourcename_to_id[(source, name)]
+            task_id = source_to_id[source]
             # Prepare new_wf_task
             new_wf_task = WorkflowTaskCreate(
                 **wf_task.dict(exclude_none=True),
             )
             # Insert task
             await db_workflow.insert_task(
                 **new_wf_task.dict(),
```

### Comparing `fractal_server-1.3.0a2/fractal_server/app/db/__init__.py` & `fractal_server-1.3.0a3/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/models/job.py` & `fractal_server-1.3.0a3/fractal_server/app/models/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 from enum import Enum
 from typing import Optional
 
 from sqlalchemy import Column
 from sqlalchemy.types import DateTime
 from sqlmodel import Field
 from sqlmodel import Relationship
+from sqlmodel import SQLModel
 
-from ...common.schemas import ApplyWorkflowBase
+from ...common.schemas import _ApplyWorkflowBase
 from ...utils import get_timestamp
 from .project import Dataset
 from .workflow import Workflow
 
 
 class JobStatusType(str, Enum):
     """
@@ -34,15 +35,15 @@
 
     SUBMITTED = "submitted"
     RUNNING = "running"
     DONE = "done"
     FAILED = "failed"
 
 
-class ApplyWorkflow(ApplyWorkflowBase, table=True):
+class ApplyWorkflow(_ApplyWorkflowBase, SQLModel, table=True):
     """
     Represent a workflow run
 
     This table is responsible for storing the state of a workflow execution in
     the database.
 
     Attributes:
```

### Comparing `fractal_server-1.3.0a2/fractal_server/app/models/project.py` & `fractal_server-1.3.0a3/fractal_server/app/models/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import Any
 from typing import Optional
 
 from sqlalchemy import Column
 from sqlalchemy.types import JSON
 from sqlmodel import Field
 from sqlmodel import Relationship
+from sqlmodel import SQLModel
 
 from ...common.schemas.project import _DatasetBase
 from ...common.schemas.project import _ProjectBase
 from ...common.schemas.project import _ResourceBase
 from .linkuserproject import LinkUserProject
 from .security import UserOAuth as User
 from .workflow import Workflow
 
 
-class Dataset(_DatasetBase, table=True):
+class Dataset(_DatasetBase, SQLModel, table=True):
     """
     Represent a dataset
 
     Attributes:
         id:
             Primary key
         project_id:
@@ -45,15 +46,15 @@
         arbitrary_types_allowed = True
 
     @property
     def paths(self) -> list[str]:
         return [r.path for r in self.resource_list]
 
 
-class Project(_ProjectBase, table=True):
+class Project(_ProjectBase, SQLModel, table=True):
     id: Optional[int] = Field(default=None, primary_key=True)
 
     user_list: list[User] = Relationship(
         link_model=LinkUserProject,
         back_populates="project_list",
         sa_relationship_kwargs={
             "lazy": "selectin",
@@ -78,10 +79,10 @@
         sa_relationship_kwargs={
             "lazy": "selectin",
             "cascade": "all, delete-orphan",
         },
     )
 
 
-class Resource(_ResourceBase, table=True):
+class Resource(_ResourceBase, SQLModel, table=True):
     id: Optional[int] = Field(default=None, primary_key=True)
     dataset_id: int = Field(foreign_key="dataset.id")
```

### Comparing `fractal_server-1.3.0a2/fractal_server/app/models/security.py` & `fractal_server-1.3.0a3/fractal_server/app/models/security.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     hashed_password: str
     is_active: bool = Field(True, nullable=False)
     is_superuser: bool = Field(False, nullable=False)
     is_verified: bool = Field(False, nullable=False)
 
     slurm_user: Optional[str]
     cache_dir: Optional[str]
+    username: Optional[str]
+
     oauth_accounts: list["OAuthAccount"] = Relationship(
         back_populates="user",
         sa_relationship_kwargs={"lazy": "selectin", "cascade": "all, delete"},
     )
     project_list: list["Project"] = Relationship(  # noqa
         back_populates="user_list",
         link_model=LinkUserProject,
```

### Comparing `fractal_server-1.3.0a2/fractal_server/app/models/state.py` & `fractal_server-1.3.0a3/fractal_server/app/models/state.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from typing import Any
 from typing import Optional
 
 from sqlalchemy import Column
 from sqlalchemy.types import DateTime
 from sqlalchemy.types import JSON
 from sqlmodel import Field
+from sqlmodel import SQLModel
 
 from ...common.schemas import _StateBase
 from ...utils import get_timestamp
 
 
-class State(_StateBase, table=True):
+class State(_StateBase, SQLModel, table=True):
     """
     Store arbitrary data in the database
 
     This table is just a state interchange that allows the system to store
     arbitrary data for later retrieval. This is particuarly important for long
     background tasks, in which it is not possible to return a meaningful
     response to the client within a single request lifespan.
```

### Comparing `fractal_server-1.3.0a2/fractal_server/app/models/task.py` & `fractal_server-1.3.0a3/fractal_server/app/models/task.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 from typing import Any
 from typing import Optional
 
 from sqlalchemy import Column
 from sqlalchemy.types import JSON
 from sqlmodel import Field
+from sqlmodel import SQLModel
 
 from ...common.schemas.task import _TaskBase
 
 
-class Task(_TaskBase, table=True):
+class Task(_TaskBase, SQLModel, table=True):
     """
     Task model
 
     Attributes:
         id: Primary key
-        command: TBD
-        input_type: TBD
-        output_type: TBD
-        default_args: TBD
-        meta: TBD
+        command: Executable command
+        input_type: Expected type of input `Dataset`
+        output_type: Expected type of output `Dataset`
+        meta:
+            Additional metadata related to execution (e.g. computational
+            resources)
         source: inherited from `_TaskBase`
         name: inherited from `_TaskBase`
+        args_schema: JSON schema of task arguments
+        args_schema_version:
+            label pointing at how the JSON schema of task arguments was
+            generated
     """
 
     id: Optional[int] = Field(default=None, primary_key=True)
+    name: str
     command: str
+    source: str = Field(unique=True)
     input_type: str
     output_type: str
-    default_args: Optional[dict[str, Any]] = Field(
-        sa_column=Column(JSON), default={}
-    )
     meta: Optional[dict[str, Any]] = Field(sa_column=Column(JSON), default={})
+    owner: Optional[str] = None
+    version: Optional[str] = None
+    args_schema: Optional[dict[str, Any]] = Field(
+        sa_column=Column(JSON), default=None
+    )
+    args_schema_version: Optional[str]
 
     @property
     def parallelization_level(self) -> Optional[str]:
         try:
             return self.meta["parallelization_level"]
         except KeyError:
             return None
```

### Comparing `fractal_server-1.3.0a2/fractal_server/app/models/workflow.py` & `fractal_server-1.3.0a3/fractal_server/app/models/workflow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+import json
+import logging
 from typing import Any
 from typing import Optional
 from typing import Union
 
 from pydantic import validator
 from sqlalchemy import Column
 from sqlalchemy.ext.orderinglist import ordering_list
 from sqlalchemy.types import JSON
 from sqlmodel import Field
 from sqlmodel import Relationship
+from sqlmodel import SQLModel
 
 from ...common.schemas.workflow import _WorkflowBase
 from ...common.schemas.workflow import _WorkflowTaskBase
 from ..db import AsyncSession
 from .task import Task
 
 
-class WorkflowTask(_WorkflowTaskBase, table=True):
+class WorkflowTask(_WorkflowTaskBase, SQLModel, table=True):
     """
     A Task as part of a Workflow
 
     This is a crossing table between Task and Workflow. In addition to the
     foreign keys, it allows for parameter overriding and keeps the order
     within the list of tasks of the workflow.
 
@@ -32,16 +35,15 @@
         task_id:
             ID of the task corresponding to the `WorkflowTask`
         order:
             Positional order of the `WorkflowTask` in `Workflow.task_list`
         meta:
             Additional parameters useful for execution
         args:
-            Additional task arguments, overriding the ones in
-            `WorkflowTask.task.args`
+            Task arguments
         task:
             `Task` object associated with the current `WorkflowTask`
 
     """
 
     class Config:
         arbitrary_types_allowed = True
@@ -78,23 +80,14 @@
             raise ValueError(
                 "`args` contains the following forbidden keys: "
                 f"{intersect_keys}"
             )
         return value
 
     @property
-    def arguments(self):
-        """
-        Override default arguments
-        """
-        out = self.task.default_args.copy()
-        out.update(self.args or {})
-        return out
-
-    @property
     def is_parallel(self) -> bool:
         return self.task.is_parallel
 
     @property
     def parallelization_level(self) -> Union[str, None]:
         return self.task.parallelization_level
 
@@ -104,31 +97,16 @@
         Return a combination of self.meta (higher priority) and self.task.meta
         (lower priority) key-value pairs.
         """
         res = self.task.meta.copy() or {}
         res.update(self.meta or {})
         return res
 
-    def assemble_args(self, extra: dict[str, Any] = None) -> dict:
-        """
-        Merge of `extra` arguments and `self.arguments`.
-
-        Returns
-            full_args:
-                A dictionary consisting of the merge of `extra` and
-                `self.arguments`.
-        """
-        full_args = {}
-        if extra:
-            full_args.update(extra)
-        full_args.update(self.arguments)
-        return full_args
-
 
-class Workflow(_WorkflowBase, table=True):
+class Workflow(_WorkflowBase, SQLModel, table=True):
     """
     Workflow
 
     Attributes:
         id:
             Primary key
         project_id:
@@ -168,15 +146,42 @@
             meta: TBD
             order: TBD
             db: TBD
             commit: TBD
         """
         if order is None:
             order = len(self.task_list)
-        wf_task = WorkflowTask(task_id=task_id, args=args, meta=meta)
+
+        # Get task from db, extract the JSON Schema for its arguments (if any),
+        # read default values and set them in default_args
+        db_task = await db.get(Task, task_id)
+        default_args = {}
+        if db_task.args_schema is not None:
+            try:
+                properties = db_task.args_schema["properties"]
+                for prop_name, prop_schema in properties.items():
+                    default_value = prop_schema.get("default", None)
+                    if default_value:
+                        default_args[prop_name] = default_value
+            except KeyError as e:
+                logging.warning(
+                    "Cannot set default_args from args_schema="
+                    f"{json.dumps(db_task.args_schema)}\n"
+                    f"Original KeyError: {str(e)}"
+                )
+        # Override default_args with args
+        actual_args = default_args.copy()
+        if args is not None:
+            for k, v in args.items():
+                actual_args[k] = v
+        if not actual_args:
+            actual_args = None
+
+        # Create DB entry
+        wf_task = WorkflowTask(task_id=task_id, args=actual_args, meta=meta)
         db.add(wf_task)
         self.task_list.insert(order, wf_task)
         self.task_list.reorder()  # type: ignore
         if commit:
             await db.commit()
             await db.refresh(wf_task)
         return wf_task
```

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/__init__.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/_common.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,33 +183,33 @@
     workflow_dir: Path,
     workflow_dir_user: Optional[Path] = None,
 ) -> TaskParameters:
     """
     Call a single task
 
     This assembles the runner arguments (input_paths, output_path, ...) and
-    task arguments (i.e., arguments that are specific to the task, such as
-    message or index in the dummy task), writes them to file, call the task
-    executable command passing the arguments file as an input and assembles
-    the output.
+    wftask arguments (i.e., arguments that are specific to the WorkflowTask,
+    such as message or index in the dummy task), writes them to file, call the
+    task executable command passing the arguments file as an input and
+    assembles the output.
 
     **Note**: This function is directly submitted to a
     `concurrent.futures`-compatible executor, as in
 
         some_future = executor.submit(call_single_task, ...)
 
     If the executor then impersonates another user (as in the
     `FractalSlurmExecutor`), this function is run by that user.  For this
     reason, it should not write any file to workflow_dir, or it may yield
     permission errors.
 
     Args:
         wftask:
             The workflow task to be called. This includes task specific
-            arguments via the task.task.arguments attribute.
+            arguments via the wftask.args attribute.
         task_pars:
             The parameters required to run the task which are not specific to
             the task, e.g., I/O paths.
         workflow_dir:
             The server-side working directory for workflow execution.
         workflow_dir_user:
             The user-side working directory for workflow execution (only
@@ -234,19 +234,20 @@
 
     task_files = get_task_file_paths(
         workflow_dir=workflow_dir,
         workflow_dir_user=workflow_dir_user,
         task_order=wftask.order,
     )
 
-    # assemble full args
-    args_dict = wftask.assemble_args(extra=task_pars.dict())
-
-    # write args file
-    write_args_file(args_dict, path=task_files.args)
+    # write args file (by assembling task_pars and wftask.args)
+    write_args_file(
+        task_pars.dict(),
+        wftask.args or {},
+        path=task_files.args,
+    )
 
     # assemble full command
     cmd = (
         f"{wftask.task.command} -j {task_files.args} "
         f"--metadata-out {task_files.metadiff}"
     )
 
@@ -337,18 +338,18 @@
     task_files = get_task_file_paths(
         workflow_dir=workflow_dir,
         workflow_dir_user=workflow_dir_user,
         task_order=wftask.order,
         component=component,
     )
 
-    # assemble full args
+    # write args file (by assembling task_pars, wftask.args and component)
     write_args_file(
         task_pars.dict(),
-        wftask.arguments,
+        wftask.args or {},
         dict(component=component),
         path=task_files.args,
     )
 
     # assemble full command
     cmd = (
         f"{wftask.task.command} -j {task_files.args} "
```

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/_local/_local_config.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/_local/_submit_setup.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/_local/executor.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -739,15 +739,16 @@
                         "Here are some possible reasons:\n"
                         "1. The SLURM job was scancel-ed, either by the user "
                         "or due to an error (e.g. an out-of-memory or timeout "
                         "error). Note that if the scancel took place before "
                         "the job started running, the SLURM out/err files "
                         "will be empty.\n"
                         "2. Some error occurred upon writing the file to disk "
-                        "(e.g. due to an overloaded NFS filesystem). "
+                        "(e.g. because there is not enough space on disk, or "
+                        "due to an overloaded NFS filesystem). "
                         "Note that the server configuration has "
                         "FRACTAL_SLURM_OUTPUT_FILE_GRACE_TIME="
                         f"{settings.FRACTAL_SLURM_OUTPUT_FILE_GRACE_TIME} "
                         "seconds.\n"
                     )
                     job_exc = self._prepare_JobExecutionError(jobid, info=info)
                     try:
```

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/runner/common.py` & `fractal_server-1.3.0a3/fractal_server/app/runner/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/app/security/__init__.py` & `fractal_server-1.3.0a3/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.3.0a3/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.3.0a3/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/README.md` & `fractal_server-1.3.0a3/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__init__.py` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__init__.py`

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

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 12 09:54:53 2023 UTC, .py size: 1135 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,102 @@
-00000000: 6f0d 0d0a 0000 0000 ed0c 5e64 6f04 0000  o.........^do...
+00000000: 6f0d 0d0a 0000 0000 1056 7064 5d04 0000  o........Vpd]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
-00000040: 6d02 5a02 0100 6400 6403 6c01 6d03 5a03  m.Z...d.d.l.m.Z.
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
-00000230: 0000 00fa 532f 686f 6d65 2f74 6f6d 6d61  ....S/home/tomma
-00000240: 736f 2f46 7261 6374 616c 2f66 7261 6374  so/Fractal/fract
-00000250: 616c 2d73 6572 7665 722f 6672 6163 7461  al-server/fracta
-00000260: 6c5f 7365 7276 6572 2f63 6f6d 6d6f 6e2f  l_server/common/
-00000270: 7363 6865 6d61 732f 6170 706c 7977 6f72  schemas/applywor
-00000280: 6b66 6c6f 772e 7079 7209 0000 0011 0000  kflow.pyr.......
-00000290: 0073 0600 0000 0a00 0401 1007 7209 0000  .s..........r...
-000002a0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000002b0: 0000 0400 0000 4000 0000 7320 0000 0065  ......@...s ...e
-000002c0: 005a 0164 005a 0265 0364 0164 0264 038d  .Z.d.Z.e.d.d.d..
-000002d0: 0265 0464 0183 0183 015a 0564 0453 0029  .e.d.....Z.d.S.)
-000002e0: 0572 0a00 0000 720c 0000 0054 2901 da0b  .r....r....T)...
-000002f0: 616c 6c6f 775f 7265 7573 654e 2906 720d  allow_reuseN).r.
-00000300: 0000 0072 0e00 0000 720f 0000 0072 0500  ...r....r....r..
-00000310: 0000 7208 0000 00da 0c5f 776f 726b 6572  ..r......_worker
-00000320: 5f69 6e69 7472 1300 0000 7213 0000 0072  _initr....r....r
-00000330: 1300 0000 7214 0000 0072 0a00 0000 1c00  ....r....r......
-00000340: 0000 7308 0000 0008 000a 0306 0108 ff72  ..s............r
-00000350: 0a00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000360: 0000 0000 0003 0000 0040 0000 0073 8e00  .........@...s..
-00000370: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-00000380: 6401 3c00 6503 6504 6402 3c00 6503 6504  d.<.e.e.d.<.e.e.
-00000390: 6403 3c00 6503 6504 6404 3c00 6503 6504  d.<.e.e.d.<.e.e.
-000003a0: 6405 3c00 6505 6504 6406 3c00 6506 6505  d.<.e.e.d.<.e.e.
-000003b0: 1900 6504 6407 3c00 6507 6504 6408 3c00  ..e.d.<.e.e.d.<.
-000003c0: 6506 6507 1900 6504 6409 3c00 6506 6508  e.e...e.d.<.e.e.
-000003d0: 6507 1900 1900 6504 640a 3c00 6506 6507  e.....e.d.<.e.e.
-000003e0: 1900 6504 640b 3c00 6506 6507 1900 6504  ..e.d.<.e.e...e.
-000003f0: 640c 3c00 640d 640e 8400 5a09 640f 5300  d.<.d.d...Z.d.S.
-00000400: 2910 720b 0000 00da 0269 64da 0a70 726f  ).r......id..pro
-00000410: 6a65 6374 5f69 64da 0b77 6f72 6b66 6c6f  ject_id..workflo
-00000420: 775f 6964 da10 696e 7075 745f 6461 7461  w_id..input_data
-00000430: 7365 745f 6964 da11 6f75 7470 7574 5f64  set_id..output_d
-00000440: 6174 6173 6574 5f69 64da 0f73 7461 7274  ataset_id..start
-00000450: 5f74 696d 6573 7461 6d70 da0d 656e 645f  _timestamp..end_
-00000460: 7469 6d65 7374 616d 70da 0673 7461 7475  timestamp..statu
-00000470: 73da 036c 6f67 da07 6869 7374 6f72 79da  s..log..history.
-00000480: 0b77 6f72 6b69 6e67 5f64 6972 da10 776f  .working_dir..wo
-00000490: 726b 696e 675f 6469 725f 7573 6572 6301  rking_dir_userc.
-000004a0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000004b0: 0000 0043 0000 0073 2800 0000 7c00 a000  ...C...s(...|...
-000004c0: a100 7d01 7401 7c00 6a02 8301 7c01 6401  ..}.t.|.j...|.d.
-000004d0: 3c00 7401 7c00 6a03 8301 7c01 6402 3c00  <.t.|.j...|.d.<.
-000004e0: 7c01 5300 2903 4e72 1c00 0000 721d 0000  |.S.).Nr....r...
-000004f0: 0029 04da 0464 6963 7472 1100 0000 721c  .)...dictr....r.
-00000500: 0000 0072 1d00 0000 2902 da04 7365 6c66  ...r....)...self
-00000510: da01 6472 1300 0000 7213 0000 0072 1400  ..dr....r....r..
-00000520: 0000 da0e 7361 6e69 7469 7365 645f 6469  ....sanitised_di
-00000530: 6374 3200 0000 7308 0000 0008 010e 010e  ct2...s.........
-00000540: 0104 017a 2041 7070 6c79 576f 726b 666c  ...z ApplyWorkfl
-00000550: 6f77 5265 6164 2e73 616e 6974 6973 6564  owRead.sanitised
-00000560: 5f64 6963 744e 290a 720d 0000 0072 0e00  _dictN).r....r..
-00000570: 0000 720f 0000 00da 0369 6e74 7212 0000  ..r......intr...
-00000580: 0072 0200 0000 7204 0000 0072 1100 0000  .r....r....r....
-00000590: 7203 0000 0072 2600 0000 7213 0000 0072  r....r&...r....r
-000005a0: 1300 0000 7213 0000 0072 1400 0000 720b  ....r....r....r.
-000005b0: 0000 0024 0000 0073 1c00 0000 0a00 0801  ...$...s........
-000005c0: 0801 0801 0801 0801 0801 0c01 0801 0c01  ................
-000005d0: 1001 0c01 0c01 0c02 720b 0000 004e 290e  ........r....N).
-000005e0: 7202 0000 00da 0674 7970 696e 6772 0300  r......typingr..
-000005f0: 0000 7204 0000 00da 0870 7964 616e 7469  ..r......pydanti
-00000600: 6372 0500 0000 da08 7371 6c6d 6f64 656c  cr......sqlmodel
-00000610: 7206 0000 00da 0b5f 7661 6c69 6461 746f  r......_validato
-00000620: 7273 7208 0000 00da 075f 5f61 6c6c 5f5f  rsr......__all__
-00000630: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00000640: 1300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
-00000650: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000660: 0073 1400 0000 0c00 0c01 0c01 0c02 0c01  .s..............
-00000670: 0c02 0402 1007 100b 1408                 ..........
+00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6405  ..d.d.l.m.Z...d.
+00000060: 6406 6c06 6d07 5a07 0100 6407 5a08 4700  d.l.m.Z...d.Z.G.
+00000070: 6408 6409 8400 6409 6504 8303 5a09 4700  d.d...d.e...Z.G.
+00000080: 640a 640b 8400 640b 6509 8303 5a0a 4700  d.d...d.e...Z.G.
+00000090: 640c 640d 8400 640d 6509 8303 5a0b 640e  d.d...d.e...Z.d.
+000000a0: 5300 290f e900 0000 0029 01da 0864 6174  S.)......)...dat
+000000b0: 6574 696d 6529 01da 084f 7074 696f 6e61  etime)...Optiona
+000000c0: 6c29 01da 0942 6173 654d 6f64 656c 2901  l)...BaseModel).
+000000d0: da09 7661 6c69 6461 746f 72e9 0100 0000  ..validator.....
+000000e0: 2901 da06 7661 6c73 7472 2903 da12 5f41  )...valstr)..._A
+000000f0: 7070 6c79 576f 726b 666c 6f77 4261 7365  pplyWorkflowBase
+00000100: da13 4170 706c 7957 6f72 6b66 6c6f 7743  ..ApplyWorkflowC
+00000110: 7265 6174 65da 1141 7070 6c79 576f 726b  reate..ApplyWork
+00000120: 666c 6f77 5265 6164 6300 0000 0000 0000  flowReadc.......
+00000130: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000140: 0073 1e00 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+00000150: 6401 5a03 6504 6505 1900 6506 6402 3c00  d.Z.e.e...e.d.<.
+00000160: 6403 5300 2904 7208 0000 007a 500a 2020  d.S.).r....zP.  
+00000170: 2020 4261 7365 2063 6c61 7373 2066 6f72    Base class for
+00000180: 2041 7070 6c79 576f 726b 666c 6f77 0a0a   ApplyWorkflow..
+00000190: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
+000001a0: 2020 2020 2020 2020 776f 726b 6572 5f69          worker_i
+000001b0: 6e69 743a 2054 4244 0a20 2020 20da 0b77  nit: TBD.    ..w
+000001c0: 6f72 6b65 725f 696e 6974 4e29 07da 085f  orker_initN)..._
+000001d0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+000001e0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000001f0: 5fda 075f 5f64 6f63 5f5f 7203 0000 00da  _..__doc__r.....
+00000200: 0373 7472 da0f 5f5f 616e 6e6f 7461 7469  .str..__annotati
+00000210: 6f6e 735f 5fa9 0072 1200 0000 7212 0000  ons__..r....r...
+00000220: 00fa 532f 686f 6d65 2f74 6f6d 6d61 736f  ..S/home/tommaso
+00000230: 2f46 7261 6374 616c 2f66 7261 6374 616c  /Fractal/fractal
+00000240: 2d73 6572 7665 722f 6672 6163 7461 6c5f  -server/fractal_
+00000250: 7365 7276 6572 2f63 6f6d 6d6f 6e2f 7363  server/common/sc
+00000260: 6865 6d61 732f 6170 706c 7977 6f72 6b66  hemas/applyworkf
+00000270: 6c6f 772e 7079 7208 0000 0010 0000 0073  low.pyr........s
+00000280: 0600 0000 0a00 0401 1007 7208 0000 0063  ..........r....c
+00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002a0: 0400 0000 4000 0000 7320 0000 0065 005a  ....@...s ...e.Z
+000002b0: 0164 005a 0265 0364 0164 0264 038d 0265  .d.Z.e.d.d.d...e
+000002c0: 0464 0183 0183 015a 0564 0453 0029 0572  .d.....Z.d.S.).r
+000002d0: 0900 0000 720b 0000 0054 2901 da0b 616c  ....r....T)...al
+000002e0: 6c6f 775f 7265 7573 654e 2906 720c 0000  low_reuseN).r...
+000002f0: 0072 0d00 0000 720e 0000 0072 0500 0000  .r....r....r....
+00000300: 7207 0000 00da 0c5f 776f 726b 6572 5f69  r......_worker_i
+00000310: 6e69 7472 1200 0000 7212 0000 0072 1200  nitr....r....r..
+00000320: 0000 7213 0000 0072 0900 0000 1b00 0000  ..r....r........
+00000330: 7308 0000 0008 000a 0306 0108 ff72 0900  s............r..
+00000340: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000350: 0000 0003 0000 0040 0000 0073 8e00 0000  .......@...s....
+00000360: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
+00000370: 3c00 6503 6504 6402 3c00 6503 6504 6403  <.e.e.d.<.e.e.d.
+00000380: 3c00 6503 6504 6404 3c00 6503 6504 6405  <.e.e.d.<.e.e.d.
+00000390: 3c00 6505 6504 6406 3c00 6506 6505 1900  <.e.e.d.<.e.e...
+000003a0: 6504 6407 3c00 6507 6504 6408 3c00 6506  e.d.<.e.e.d.<.e.
+000003b0: 6507 1900 6504 6409 3c00 6506 6508 6507  e...e.d.<.e.e.e.
+000003c0: 1900 1900 6504 640a 3c00 6506 6507 1900  ....e.d.<.e.e...
+000003d0: 6504 640b 3c00 6506 6507 1900 6504 640c  e.d.<.e.e...e.d.
+000003e0: 3c00 640d 640e 8400 5a09 640f 5300 2910  <.d.d...Z.d.S.).
+000003f0: 720a 0000 00da 0269 64da 0a70 726f 6a65  r......id..proje
+00000400: 6374 5f69 64da 0b77 6f72 6b66 6c6f 775f  ct_id..workflow_
+00000410: 6964 da10 696e 7075 745f 6461 7461 7365  id..input_datase
+00000420: 745f 6964 da11 6f75 7470 7574 5f64 6174  t_id..output_dat
+00000430: 6173 6574 5f69 64da 0f73 7461 7274 5f74  aset_id..start_t
+00000440: 696d 6573 7461 6d70 da0d 656e 645f 7469  imestamp..end_ti
+00000450: 6d65 7374 616d 70da 0673 7461 7475 73da  mestamp..status.
+00000460: 036c 6f67 da07 6869 7374 6f72 79da 0b77  .log..history..w
+00000470: 6f72 6b69 6e67 5f64 6972 da10 776f 726b  orking_dir..work
+00000480: 696e 675f 6469 725f 7573 6572 6301 0000  ing_dir_userc...
+00000490: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+000004a0: 0043 0000 0073 2800 0000 7c00 a000 a100  .C...s(...|.....
+000004b0: 7d01 7401 7c00 6a02 8301 7c01 6401 3c00  }.t.|.j...|.d.<.
+000004c0: 7401 7c00 6a03 8301 7c01 6402 3c00 7c01  t.|.j...|.d.<.|.
+000004d0: 5300 2903 4e72 1b00 0000 721c 0000 0029  S.).Nr....r....)
+000004e0: 04da 0464 6963 7472 1000 0000 721b 0000  ...dictr....r...
+000004f0: 0072 1c00 0000 2902 da04 7365 6c66 da01  .r....)...self..
+00000500: 6472 1200 0000 7212 0000 0072 1300 0000  dr....r....r....
+00000510: da0e 7361 6e69 7469 7365 645f 6469 6374  ..sanitised_dict
+00000520: 3100 0000 7308 0000 0008 010e 010e 0104  1...s...........
+00000530: 017a 2041 7070 6c79 576f 726b 666c 6f77  .z ApplyWorkflow
+00000540: 5265 6164 2e73 616e 6974 6973 6564 5f64  Read.sanitised_d
+00000550: 6963 744e 290a 720c 0000 0072 0d00 0000  ictN).r....r....
+00000560: 720e 0000 00da 0369 6e74 7211 0000 0072  r......intr....r
+00000570: 0200 0000 7203 0000 0072 1000 0000 da04  ....r....r......
+00000580: 6c69 7374 7225 0000 0072 1200 0000 7212  listr%...r....r.
+00000590: 0000 0072 1200 0000 7213 0000 0072 0a00  ...r....r....r..
+000005a0: 0000 2300 0000 731c 0000 000a 0008 0108  ..#...s.........
+000005b0: 0108 0108 0108 0108 010c 0108 010c 0110  ................
+000005c0: 010c 010c 010c 0272 0a00 0000 4e29 0c72  .......r....N).r
+000005d0: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
+000005e0: 00da 0870 7964 616e 7469 6372 0400 0000  ...pydanticr....
+000005f0: 7205 0000 00da 0b5f 7661 6c69 6461 746f  r......_validato
+00000600: 7273 7207 0000 00da 075f 5f61 6c6c 5f5f  rsr......__all__
+00000610: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000620: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00000630: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000640: 0073 1200 0000 0c00 0c01 0c02 0c01 0c02  .s..............
+00000650: 0402 1007 100b 1408                      ........
```

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Feb 22 11:04:15 2023 UTC, .py size: 2817 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,222 +1,256 @@
-00000000: 6f0d 0d0a 0000 0000 aff6 f563 010b 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 d02e 7f64 970d 0000  o..........d....
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
-000005c0: 7865 6375 7461 626c 65da 0a69 6e70 7574  xecutable..input
-000005d0: 5f74 7970 65da 0b6f 7574 7075 745f 7479  _type..output_ty
-000005e0: 7065 2901 da0f 6465 6661 756c 745f 6661  pe)...default_fa
-000005f0: 6374 6f72 79da 0c64 6566 6175 6c74 5f61  ctory..default_a
-00000600: 7267 73da 046d 6574 614e 290e da08 5f5f  rgs..metaN)...__
-00000610: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000620: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000630: da07 5f5f 646f 635f 5fda 0373 7472 da0f  ..__doc__..str..
-00000640: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
-00000650: 0200 0000 720a 0000 00da 0464 6963 7472  ....r......dictr
-00000660: 1300 0000 7206 0000 0072 0400 0000 7203  ....r....r....r.
-00000670: 0000 0072 1400 0000 a900 721c 0000 0072  ...r......r....r
-00000680: 1c00 0000 fa4e 2f68 6f6d 652f 746f 6d6d  .....N/home/tomm
-00000690: 6173 6f2f 4672 6163 7461 6c2f 6672 6163  aso/Fractal/frac
-000006a0: 7461 6c2d 7365 7276 6572 2f66 7261 6374  tal-server/fract
-000006b0: 616c 5f73 6572 7665 722f 636f 6d6d 6f6e  al_server/common
-000006c0: 2f73 6368 656d 6173 2f6d 616e 6966 6573  /schemas/manifes
-000006d0: 742e 7079 720d 0000 0010 0000 0073 1000  t.pyr........s..
-000006e0: 0000 0a00 0401 081c 0801 0801 0801 1e01  ................
-000006f0: 2201 720d 0000 00da 1054 6173 6b4d 616e  ".r......TaskMan
-00000700: 6966 6573 7454 7970 6529 01da 0562 6f75  ifestType)...bou
-00000710: 6e64 6300 0000 0000 0000 0000 0000 0000  ndc.............
-00000720: 0000 0003 0000 0040 0000 0073 2600 0000  .......@...s&...
-00000730: 6500 5a01 6400 5a02 5500 6401 5a03 6504  e.Z.d.Z.U.d.Z.e.
-00000740: 6505 6402 3c00 6506 6507 1900 6505 6403  e.d.<.e.e...e.d.
-00000750: 3c00 6404 5300 2905 da0d 5f4d 616e 6966  <.d.S.)..._Manif
-00000760: 6573 7442 6173 6561 2803 0000 0a20 2020  estBasea(....   
-00000770: 204d 616e 6966 6573 7420 6261 7365 2063   Manifest base c
-00000780: 6c61 7373 0a0a 2020 2020 5061 636b 6167  lass..    Packag
-00000790: 6573 2063 6f6e 7461 696e 696e 6720 7461  es containing ta
-000007a0: 736b 7320 6172 6520 7265 7175 6972 6564  sks are required
-000007b0: 2074 6f20 696e 636c 7564 6520 6120 7370   to include a sp
-000007c0: 6563 6961 6c20 6669 6c65 0a20 2020 2060  ecial file.    `
-000007d0: 5f5f 4652 4143 5441 4c5f 4d41 4e49 4645  __FRACTAL_MANIFE
-000007e0: 5354 5f5f 2e6a 736f 6e60 2069 6e20 6f72  ST__.json` in or
-000007f0: 6465 7220 746f 2062 6520 6469 7363 6f76  der to be discov
-00000800: 6572 6564 2061 6e64 2075 7365 6420 6279  ered and used by
-00000810: 2046 7261 6374 616c 2e0a 0a20 2020 2054   Fractal...    T
-00000820: 6869 7320 6d6f 6465 6c20 636c 6173 7320  his model class 
-00000830: 616e 6420 7468 6520 6d6f 6465 6c20 636c  and the model cl
-00000840: 6173 7365 7320 6974 2064 6570 656e 6473  asses it depends
-00000850: 206f 6e20 7072 6f76 6964 6520 7468 6520   on provide the 
-00000860: 6261 7365 0a20 2020 2073 6368 656d 6120  base.    schema 
-00000870: 746f 2072 6561 642c 2077 7269 7465 2061  to read, write a
-00000880: 6e64 2076 616c 6964 6174 6520 6d61 6e69  nd validate mani
-00000890: 6665 7374 732e 0a0a 2020 2020 4174 7472  fests...    Attr
-000008a0: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
-000008b0: 6d61 6e69 6665 7374 5f76 6572 7369 6f6e  manifest_version
-000008c0: 3a0a 2020 2020 2020 2020 2020 2020 4120  :.            A 
-000008d0: 7665 7273 696f 6e20 7374 7269 6e67 2074  version string t
-000008e0: 6861 7420 7072 6f76 6964 6573 2069 6e64  hat provides ind
-000008f0: 6963 6174 696f 6e20 666f 7220 636f 6d70  ication for comp
-00000900: 6174 6962 696c 6974 7920 6265 7477 6565  atibility betwee
-00000910: 6e0a 2020 2020 2020 2020 2020 2020 6d61  n.            ma
-00000920: 6e69 6665 7374 7320 6173 2074 6865 2073  nifests as the s
-00000930: 6368 656d 6120 6576 6f6c 7665 732e 2054  chema evolves. T
-00000940: 6869 7320 6973 2066 6f72 2069 6e73 7461  his is for insta
-00000950: 6e63 6520 7573 6564 2062 790a 2020 2020  nce used by.    
-00000960: 2020 2020 2020 2020 4672 6163 7461 6c20          Fractal 
-00000970: 746f 2064 6574 6572 6d69 6e65 2077 6869  to determine whi
-00000980: 6368 2073 7562 636c 6173 7320 6f66 2074  ch subclass of t
-00000990: 6865 2070 7265 7365 6e74 2062 6173 6520  he present base 
-000009a0: 636c 6173 7320 6e65 6564 730a 2020 2020  class needs.    
-000009b0: 2020 2020 2020 2020 6265 2075 7365 6420          be used 
-000009c0: 746f 2072 6561 6420 616e 6420 7661 6c69  to read and vali
-000009d0: 6461 7465 2074 6865 2069 6e70 7574 2e0a  date the input..
-000009e0: 2020 2020 2020 2020 7461 736b 5f6c 6973          task_lis
-000009f0: 7420 3a20 4c69 7374 5b54 6173 6b4d 616e  t : List[TaskMan
-00000a00: 6966 6573 7454 7970 655d 0a20 2020 2020  ifestType].     
-00000a10: 2020 2020 2020 2054 6865 206c 6973 7420         The list 
-00000a20: 6f66 2074 6173 6b73 2c20 7265 7072 6573  of tasks, repres
-00000a30: 656e 7465 6420 6173 2073 7065 6369 6669  ented as specifi
-00000a40: 6564 2062 7920 7375 6263 6c61 7373 6573  ed by subclasses
-00000a50: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
-00000a60: 2020 2020 5f54 6173 6b4d 616e 6966 6573      _TaskManifes
-00000a70: 7442 6173 6520 2861 2e6b 2e61 2e20 5461  tBase (a.k.a. Ta
-00000a80: 736b 4d61 6e69 6665 7374 5479 7065 290a  skManifestType).
-00000a90: 2020 2020 da10 6d61 6e69 6665 7374 5f76      ..manifest_v
-00000aa0: 6572 7369 6f6e da09 7461 736b 5f6c 6973  ersion..task_lis
-00000ab0: 744e 2908 7215 0000 0072 1600 0000 7217  tN).r....r....r.
-00000ac0: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
-00000ad0: 0000 7205 0000 0072 1e00 0000 721c 0000  ..r....r....r...
-00000ae0: 0072 1c00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00000af0: 7220 0000 0038 0000 0073 0800 0000 0a00  r ...8...s......
-00000b00: 0401 0814 1001 7220 0000 0063 0000 0000  ......r ...c....
-00000b10: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-00000b20: 4000 0000 730c 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00000b30: 0264 0153 0029 0272 0b00 0000 4e29 0372  .d.S.).r....N).r
-00000b40: 1500 0000 7216 0000 0072 1700 0000 721c  ....r....r....r.
-00000b50: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
-00000b60: 0000 720b 0000 0051 0000 0073 0400 0000  ..r....Q...s....
-00000b70: 0800 0401 720b 0000 0063 0000 0000 0000  ....r....c......
-00000b80: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000b90: 0000 732e 0000 0065 005a 0164 005a 0255  ..s....e.Z.d.Z.U
-00000ba0: 0064 015a 0365 0465 0519 0065 0664 023c  .d.Z.e.e...e.d.<
-00000bb0: 0065 0764 0383 0164 0464 0584 0083 015a  .e.d...d.d.....Z
-00000bc0: 0864 0653 0029 0772 0c00 0000 7a23 0a20  .d.S.).r....z#. 
-00000bd0: 2020 204d 616e 6966 6573 7420 7363 6865     Manifest sche
-00000be0: 6d61 2076 6572 7369 6f6e 2031 0a20 2020  ma version 1.   
-00000bf0: 2072 2200 0000 7221 0000 0063 0200 0000   r"...r!...c....
-00000c00: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00000c10: 4300 0000 7314 0000 007c 0164 016b 0372  C...s....|.d.k.r
-00000c20: 0874 0064 0283 0182 0164 0053 0029 034e  .t.d.....d.S.).N
-00000c30: da01 317a 1657 726f 6e67 206d 616e 6966  ..1z.Wrong manif
-00000c40: 6573 7420 7665 7273 696f 6e29 01da 0a56  est version)...V
-00000c50: 616c 7565 4572 726f 7229 02da 0363 6c73  alueError)...cls
-00000c60: da05 7661 6c75 6572 1c00 0000 721c 0000  ..valuer....r...
-00000c70: 0072 1d00 0000 da12 6d61 6e69 6665 7374  .r......manifest
-00000c80: 5f76 6572 7369 6f6e 5f31 5c00 0000 7306  _version_1\...s.
-00000c90: 0000 0008 0208 0104 ff7a 1d4d 616e 6966  .........z.Manif
-00000ca0: 6573 7456 312e 6d61 6e69 6665 7374 5f76  estV1.manifest_v
-00000cb0: 6572 7369 6f6e 5f31 4e29 0972 1500 0000  ersion_1N).r....
-00000cc0: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-00000cd0: 0500 0000 720b 0000 0072 1a00 0000 7209  ....r....r....r.
-00000ce0: 0000 0072 2700 0000 721c 0000 0072 1c00  ...r'...r....r..
-00000cf0: 0000 721c 0000 0072 1d00 0000 720c 0000  ..r....r....r...
-00000d00: 0055 0000 0073 0a00 0000 0a00 0401 0c04  .U...s..........
-00000d10: 0602 0e01 720c 0000 004e 2913 da07 7061  ....r....N)...pa
-00000d20: 7468 6c69 6272 0200 0000 da06 7479 7069  thlibr......typi
-00000d30: 6e67 7203 0000 0072 0400 0000 7205 0000  ngr....r....r...
-00000d40: 0072 0600 0000 7207 0000 00da 0870 7964  .r....r......pyd
-00000d50: 616e 7469 6372 0800 0000 7209 0000 00da  anticr....r.....
-00000d60: 0873 716c 6d6f 6465 6c72 0a00 0000 da07  .sqlmodelr......
-00000d70: 5f5f 616c 6c5f 5f72 0d00 0000 721e 0000  __all__r....r...
-00000d80: 0072 2000 0000 720b 0000 0072 0c00 0000  .r ...r....r....
-00000d90: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
-00000da0: 1d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000db0: 0000 731e 0000 000c 000c 010c 010c 010c  ..s.............
-00000dc0: 010c 010c 020c 010c 0104 0310 030c 2510  ..............%.
-00000dd0: 0310 1914 04                             .....
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
+000005f0: 0000 00fa 4e2f 686f 6d65 2f74 6f6d 6d61  ....N/home/tomma
+00000600: 736f 2f46 7261 6374 616c 2f66 7261 6374  so/Fractal/fract
+00000610: 616c 2d73 6572 7665 722f 6672 6163 7461  al-server/fracta
+00000620: 6c5f 7365 7276 6572 2f63 6f6d 6d6f 6e2f  l_server/common/
+00000630: 7363 6865 6d61 732f 6d61 6e69 6665 7374  schemas/manifest
+00000640: 2e70 7972 0b00 0000 0e00 0000 7310 0000  .pyr........s...
+00000650: 000a 0004 0108 1b08 0108 0108 011e 0118  ................
+00000660: 0172 0b00 0000 da10 5461 736b 4d61 6e69  .r......TaskMani
+00000670: 6665 7374 5479 7065 2901 da05 626f 756e  festType)...boun
+00000680: 6463 0000 0000 0000 0000 0000 0000 0000  dc..............
+00000690: 0000 0300 0000 4000 0000 734c 0000 0065  ......@...sL...e
+000006a0: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
+000006b0: 0564 023c 0065 0665 0719 0065 0564 033c  .d.<.e.e...e.d.<
+000006c0: 0064 045a 0865 0965 0564 053c 0065 0a65  .d.Z.e.e.d.<.e.e
+000006d0: 0419 0065 0564 063c 0065 0b83 0064 0764  ...e.d.<.e...d.d
+000006e0: 0884 0083 015a 0c64 0953 0029 0ada 0d5f  .....Z.d.S.)..._
+000006f0: 4d61 6e69 6665 7374 4261 7365 6111 0400  ManifestBasea...
+00000700: 000a 2020 2020 4d61 6e69 6665 7374 2062  ..    Manifest b
+00000710: 6173 6520 636c 6173 730a 0a20 2020 2050  ase class..    P
+00000720: 6163 6b61 6765 7320 636f 6e74 6169 6e69  ackages containi
+00000730: 6e67 2074 6173 6b73 2061 7265 2072 6571  ng tasks are req
+00000740: 7569 7265 6420 746f 2069 6e63 6c75 6465  uired to include
+00000750: 2061 2073 7065 6369 616c 2066 696c 650a   a special file.
+00000760: 2020 2020 605f 5f46 5241 4354 414c 5f4d      `__FRACTAL_M
+00000770: 414e 4946 4553 545f 5f2e 6a73 6f6e 6020  ANIFEST__.json` 
+00000780: 696e 206f 7264 6572 2074 6f20 6265 2064  in order to be d
+00000790: 6973 636f 7665 7265 6420 616e 6420 7573  iscovered and us
+000007a0: 6564 2062 7920 4672 6163 7461 6c2e 0a0a  ed by Fractal...
+000007b0: 2020 2020 5468 6973 206d 6f64 656c 2063      This model c
+000007c0: 6c61 7373 2061 6e64 2074 6865 206d 6f64  lass and the mod
+000007d0: 656c 2063 6c61 7373 6573 2069 7420 6465  el classes it de
+000007e0: 7065 6e64 7320 6f6e 2070 726f 7669 6465  pends on provide
+000007f0: 2074 6865 2062 6173 650a 2020 2020 7363   the base.    sc
+00000800: 6865 6d61 2074 6f20 7265 6164 2c20 7772  hema to read, wr
+00000810: 6974 6520 616e 6420 7661 6c69 6461 7465  ite and validate
+00000820: 206d 616e 6966 6573 7473 2e0a 0a20 2020   manifests...   
+00000830: 2041 7474 7269 6275 7465 733a 0a20 2020   Attributes:.   
+00000840: 2020 2020 206d 616e 6966 6573 745f 7665       manifest_ve
+00000850: 7273 696f 6e3a 0a20 2020 2020 2020 2020  rsion:.         
+00000860: 2020 2041 2076 6572 7369 6f6e 2073 7472     A version str
+00000870: 696e 6720 7468 6174 2070 726f 7669 6465  ing that provide
+00000880: 7320 696e 6469 6361 7469 6f6e 2066 6f72  s indication for
+00000890: 2063 6f6d 7061 7469 6269 6c69 7479 2062   compatibility b
+000008a0: 6574 7765 656e 0a20 2020 2020 2020 2020  etween.         
+000008b0: 2020 206d 616e 6966 6573 7473 2061 7320     manifests as 
+000008c0: 7468 6520 7363 6865 6d61 2065 766f 6c76  the schema evolv
+000008d0: 6573 2e20 5468 6973 2069 7320 666f 7220  es. This is for 
+000008e0: 696e 7374 616e 6365 2075 7365 6420 6279  instance used by
+000008f0: 0a20 2020 2020 2020 2020 2020 2046 7261  .            Fra
+00000900: 6374 616c 2074 6f20 6465 7465 726d 696e  ctal to determin
+00000910: 6520 7768 6963 6820 7375 6263 6c61 7373  e which subclass
+00000920: 206f 6620 7468 6520 7072 6573 656e 7420   of the present 
+00000930: 6261 7365 2063 6c61 7373 206e 6565 6473  base class needs
+00000940: 0a20 2020 2020 2020 2020 2020 2062 6520  .            be 
+00000950: 7573 6564 2074 6f20 7265 6164 2061 6e64  used to read and
+00000960: 2076 616c 6964 6174 6520 7468 6520 696e   validate the in
+00000970: 7075 742e 0a20 2020 2020 2020 2074 6173  put..        tas
+00000980: 6b5f 6c69 7374 203a 206c 6973 745b 5461  k_list : list[Ta
+00000990: 736b 4d61 6e69 6665 7374 5479 7065 5d0a  skManifestType].
+000009a0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+000009b0: 6c69 7374 206f 6620 7461 736b 732c 2072  list of tasks, r
+000009c0: 6570 7265 7365 6e74 6564 2061 7320 7370  epresented as sp
+000009d0: 6563 6966 6965 6420 6279 2073 7562 636c  ecified by subcl
+000009e0: 6173 7365 7320 6f66 2074 6865 0a20 2020  asses of the.   
+000009f0: 2020 2020 2020 2020 205f 5461 736b 4d61           _TaskMa
+00000a00: 6e69 6665 7374 4261 7365 2028 612e 6b2e  nifestBase (a.k.
+00000a10: 612e 2054 6173 6b4d 616e 6966 6573 7454  a. TaskManifestT
+00000a20: 7970 6529 0a20 2020 2020 2020 2068 6173  ype).        has
+00000a30: 5f61 7267 735f 7363 6865 6d61 733a 0a20  _args_schemas:. 
+00000a40: 2020 2020 2020 2020 2020 2060 5472 7565             `True
+00000a50: 6020 6966 2074 6865 206d 616e 6966 6573  ` if the manifes
+00000a60: 7420 696e 636c 6475 6573 204a 534f 4e20  t incldues JSON 
+00000a70: 5363 6865 6d61 7320 666f 7220 7468 6520  Schemas for the 
+00000a80: 6172 6775 6d65 6e74 7320 6f66 0a20 2020  arguments of.   
+00000a90: 2020 2020 2020 2020 2065 6163 6820 7461           each ta
+00000aa0: 736b 2e0a 2020 2020 2020 2020 6172 6773  sk..        args
+00000ab0: 5f73 6368 656d 615f 7665 7273 696f 6e3a  _schema_version:
+00000ac0: 0a20 2020 2020 2020 2020 2020 204c 6162  .            Lab
+00000ad0: 656c 206f 6620 686f 7720 6061 7267 735f  el of how `args_
+00000ae0: 7363 6865 6d61 6073 2077 6572 6520 6765  schema`s were ge
+00000af0: 6e65 7261 7465 6420 2865 2e67 2e20 6070  nerated (e.g. `p
+00000b00: 7964 616e 7469 635f 7631 6029 2e0a 2020  ydantic_v1`)..  
+00000b10: 2020 da10 6d61 6e69 6665 7374 5f76 6572    ..manifest_ver
+00000b20: 7369 6f6e da09 7461 736b 5f6c 6973 7446  sion..task_listF
+00000b30: da10 6861 735f 6172 6773 5f73 6368 656d  ..has_args_schem
+00000b40: 6173 da13 6172 6773 5f73 6368 656d 615f  as..args_schema_
+00000b50: 7665 7273 696f 6e63 0200 0000 0000 0000  versionc........
+00000b60: 0000 0000 0500 0000 0900 0000 4300 0000  ............C...
+00000b70: 734c 0000 007c 0164 0119 007d 027c 0164  sL...|.d...}.|.d
+00000b80: 0219 007d 037c 0272 247c 0344 005d 177d  ...}.|.r$|.D.].}
+00000b90: 047c 046a 0064 0075 0072 2374 0164 037c  .|.j.d.u.r#t.d.|
+00000ba0: 029b 0064 047c 046a 029b 0064 057c 046a  ...d.|.j...d.|.j
+00000bb0: 009b 0064 069d 0783 0182 0171 0c7c 0153  ...d.......q.|.S
+00000bc0: 0029 074e 7221 0000 0072 2000 0000 7a11  .).Nr!...r ...z.
+00000bd0: 6861 735f 6172 6773 5f73 6368 656d 6173  has_args_schemas
+00000be0: 3d7a 0b20 6275 7420 7461 736b 2022 7a12  =z. but task "z.
+00000bf0: 2220 6861 7320 6172 6773 5f73 6368 656d  " has args_schem
+00000c00: 613d da01 2e29 0372 1200 0000 da0a 5661  a=...).r......Va
+00000c10: 6c75 6545 7272 6f72 720c 0000 0029 05da  lueErrorr....)..
+00000c20: 0363 6c73 da06 7661 6c75 6573 7221 0000  .cls..valuesr!..
+00000c30: 0072 2000 0000 da04 7461 736b 721a 0000  .r .....taskr...
+00000c40: 0072 1a00 0000 721b 0000 00da 1f5f 6368  .r....r......_ch
+00000c50: 6563 6b5f 6172 6773 5f73 6368 656d 6173  eck_args_schemas
+00000c60: 5f61 7265 5f70 7265 7365 6e74 5400 0000  _are_presentT...
+00000c70: 731c 0000 0008 0208 0104 0108 010a 0102  s...............
+00000c80: 0108 0104 0104 ff04 0106 ff04 ff02 ff04  ................
+00000c90: 057a 2d5f 4d61 6e69 6665 7374 4261 7365  .z-_ManifestBase
+00000ca0: 2e5f 6368 6563 6b5f 6172 6773 5f73 6368  ._check_args_sch
+00000cb0: 656d 6173 5f61 7265 5f70 7265 7365 6e74  emas_are_present
+00000cc0: 4e29 0d72 1300 0000 7214 0000 0072 1500  N).r....r....r..
+00000cd0: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00000ce0: 00da 046c 6973 7472 1c00 0000 7221 0000  ...listr....r!..
+00000cf0: 00da 0462 6f6f 6c72 0300 0000 7207 0000  ...boolr....r...
+00000d00: 0072 2800 0000 721a 0000 0072 1a00 0000  .r(...r....r....
+00000d10: 721a 0000 0072 1b00 0000 721e 0000 0035  r....r....r....5
+00000d20: 0000 0073 1000 0000 0a00 0401 0819 0c01  ...s............
+00000d30: 0c01 0c01 0402 0e01 721e 0000 0063 0000  ........r....c..
+00000d40: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00000d50: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
+00000d60: 005a 0264 0153 0029 0272 0900 0000 4e29  .Z.d.S.).r....N)
+00000d70: 0372 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000d80: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00000d90: 1b00 0000 7209 0000 0062 0000 0073 0400  ....r....b...s..
+00000da0: 0000 0800 0401 7209 0000 0063 0000 0000  ......r....c....
+00000db0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000dc0: 4000 0000 732e 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00000dd0: 0255 0064 015a 0365 0465 0519 0065 0664  .U.d.Z.e.e...e.d
+00000de0: 023c 0065 0764 0383 0164 0464 0584 0083  .<.e.d...d.d....
+00000df0: 015a 0864 0653 0029 0772 0a00 0000 7a23  .Z.d.S.).r....z#
+00000e00: 0a20 2020 204d 616e 6966 6573 7420 7363  .    Manifest sc
+00000e10: 6865 6d61 2076 6572 7369 6f6e 2031 0a20  hema version 1. 
+00000e20: 2020 2072 2000 0000 721f 0000 0063 0200     r ...r....c..
+00000e30: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000e40: 0000 4300 0000 731c 0000 007c 0164 016b  ..C...s....|.d.k
+00000e50: 0372 0c74 0064 027c 019b 0064 039d 0383  .r.t.d.|...d....
+00000e60: 0182 0164 0053 0029 044e da01 317a 1e57  ...d.S.).N..1z.W
+00000e70: 726f 6e67 206d 616e 6966 6573 7420 7665  rong manifest ve
+00000e80: 7273 696f 6e20 2867 6976 656e 20fa 0129  rsion (given ..)
+00000e90: 2901 7224 0000 0029 0272 2500 0000 da05  ).r$...).r%.....
+00000ea0: 7661 6c75 6572 1a00 0000 721a 0000 0072  valuer....r....r
+00000eb0: 1b00 0000 da12 6d61 6e69 6665 7374 5f76  ......manifest_v
+00000ec0: 6572 7369 6f6e 5f31 6d00 0000 7306 0000  ersion_1m...s...
+00000ed0: 0008 0210 0104 ff7a 1d4d 616e 6966 6573  .......z.Manifes
+00000ee0: 7456 312e 6d61 6e69 6665 7374 5f76 6572  tV1.manifest_ver
+00000ef0: 7369 6f6e 5f31 4e29 0972 1300 0000 7214  sion_1N).r....r.
+00000f00: 0000 0072 1500 0000 7216 0000 0072 2900  ...r....r....r).
+00000f10: 0000 7209 0000 0072 1800 0000 7208 0000  ..r....r....r...
+00000f20: 0072 2e00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+00000f30: 721a 0000 0072 1b00 0000 720a 0000 0066  r....r....r....f
+00000f40: 0000 0073 0a00 0000 0a00 0401 0c04 0602  ...s............
+00000f50: 0e01 720a 0000 004e 290f da06 7479 7069  ..r....N)...typi
+00000f60: 6e67 7202 0000 0072 0300 0000 7204 0000  ngr....r....r...
+00000f70: 00da 0870 7964 616e 7469 6372 0500 0000  ...pydanticr....
+00000f80: 7206 0000 0072 0700 0000 7208 0000 00da  r....r....r.....
+00000f90: 075f 5f61 6c6c 5f5f 720b 0000 0072 1c00  .__all__r....r..
+00000fa0: 0000 721e 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00000fb0: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+00000fc0: 721b 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000fd0: 0000 0073 1a00 0000 0c00 0c01 0c01 0c02  ...s............
+00000fe0: 0c01 0c01 0c01 0403 1003 0c24 1003 102d  ...........$...-
+00000ff0: 1404                                     ..
```

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  8 12:01:46 2023 UTC, .py size: 2527 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,226 +1,222 @@
-00000000: 6f0d 0d0a 0000 0000 aae4 5864 df09 0000  o.........Xd....
+00000000: 6f0d 0d0a 0000 0000 b554 7064 b309 0000  o........Tpd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3401 0000 6400  .....@...s4...d.
+00000020: 0004 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
-00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c05 6d06 5a06 0100 6400 6406 6c05  d.l.m.Z...d.d.l.
-00000070: 6d07 5a07 0100 6400 6407 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
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
-00000310: a900 721d 0000 0072 1d00 0000 fa4d 2f68  ..r....r.....M/h
-00000320: 6f6d 652f 746f 6d6d 6173 6f2f 4672 6163  ome/tommaso/Frac
-00000330: 7461 6c2f 6672 6163 7461 6c2d 7365 7276  tal/fractal-serv
-00000340: 6572 2f66 7261 6374 616c 5f73 6572 7665  er/fractal_serve
-00000350: 722f 636f 6d6d 6f6e 2f73 6368 656d 6173  r/common/schemas
-00000360: 2f70 726f 6a65 6374 2e70 7972 1500 0000  /project.pyr....
-00000370: 1e00 0000 7306 0000 000a 0004 010c 0472  ....s..........r
-00000380: 1500 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000390: 0000 0000 0004 0000 0040 0000 00f3 2000  .........@.... .
-000003a0: 0000 6500 5a01 6400 5a02 6503 6401 6402  ..e.Z.d.Z.e.d.d.
-000003b0: 6403 8d02 6504 6401 8301 8301 5a05 6404  d...e.d.....Z.d.
-000003c0: 5300 2905 7212 0000 0072 1600 0000 54a9  S.).r....r....T.
-000003d0: 01da 0b61 6c6c 6f77 5f72 6575 7365 4ea9  ...allow_reuseN.
-000003e0: 0672 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
-000003f0: 7207 0000 0072 0a00 0000 da05 5f70 6174  r....r......_pat
-00000400: 6872 1d00 0000 721d 0000 0072 1d00 0000  hr....r....r....
-00000410: 721e 0000 0072 1200 0000 2600 0000 f304  r....r....&.....
-00000420: 0000 0008 0018 0272 1200 0000 6300 0000  .......r....c...
-00000430: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-00000440: 0040 0000 0072 1f00 0000 2905 7214 0000  .@...r....).r...
-00000450: 0072 1600 0000 5472 2000 0000 4e72 2200  .r....Tr ...Nr".
-00000460: 0000 721d 0000 0072 1d00 0000 721d 0000  ..r....r....r...
-00000470: 0072 1e00 0000 7214 0000 002b 0000 0072  .r....r....+...r
-00000480: 2400 0000 7214 0000 0063 0000 0000 0000  $...r....c......
-00000490: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-000004a0: 0000 731e 0000 0065 005a 0164 005a 0255  ..s....e.Z.d.Z.U
-000004b0: 0065 0365 0464 013c 0065 0365 0464 023c  .e.e.d.<.e.e.d.<
-000004c0: 0064 0353 0029 0472 1300 0000 da02 6964  .d.S.).r......id
-000004d0: da0a 6461 7461 7365 745f 6964 4e29 0572  ..dataset_idN).r
-000004e0: 1700 0000 7218 0000 0072 1900 0000 da03  ....r....r......
-000004f0: 696e 7472 1c00 0000 721d 0000 0072 1d00  intr....r....r..
-00000500: 0000 721d 0000 0072 1e00 0000 7213 0000  ..r....r....r...
-00000510: 0030 0000 0073 0600 0000 0a00 0801 0c01  .0...s..........
-00000520: 7213 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000530: 0000 0000 0000 0300 0000 4000 0000 734c  ..........@...sL
-00000540: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
-00000550: 0365 0465 0564 023c 0065 0665 0419 0065  .e.e.d.<.e.e...e
-00000560: 0564 033c 0065 0769 0064 048d 015a 0865  .d.<.e.i.d...Z.e
-00000570: 0965 0465 0a66 0219 0065 0564 053c 0064  .e.e.f...e.d.<.d
-00000580: 065a 0b65 0c65 0564 073c 0064 0853 0029  .Z.e.e.d.<.d.S.)
-00000590: 09da 0c5f 4461 7461 7365 7442 6173 657a  ..._DatasetBasez
-000005a0: 7e0a 2020 2020 4261 7365 2063 6c61 7373  ~.    Base class
-000005b0: 2066 6f72 2044 6174 6173 6574 0a0a 2020   for Dataset..  
-000005c0: 2020 4174 7472 6962 7574 6573 3a0a 2020    Attributes:.  
-000005d0: 2020 2020 2020 6e61 6d65 3a20 5442 440a        name: TBD.
-000005e0: 2020 2020 2020 2020 7479 7065 3a20 5442          type: TB
-000005f0: 440a 2020 2020 2020 2020 6d65 7461 3a20  D.        meta: 
-00000600: 5442 440a 2020 2020 2020 2020 7265 6164  TBD.        read
-00000610: 5f6f 6e6c 793a 2054 4244 0a20 2020 20da  _only: TBD.    .
-00000620: 046e 616d 65da 0474 7970 6529 01da 0764  .name..type)...d
-00000630: 6566 6175 6c74 da04 6d65 7461 46da 0972  efault..metaF..r
-00000640: 6561 645f 6f6e 6c79 4e29 0d72 1700 0000  ead_onlyN).r....
-00000650: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00000660: 1b00 0000 721c 0000 0072 0500 0000 7206  ....r....r....r.
-00000670: 0000 0072 2c00 0000 7203 0000 0072 0200  ...r,...r....r..
-00000680: 0000 722d 0000 00da 0462 6f6f 6c72 1d00  ..r-.....boolr..
-00000690: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-000006a0: 0072 2800 0000 3800 0000 730c 0000 000a  .r(...8...s.....
-000006b0: 0004 0108 0a0c 011a 0110 0172 2800 0000  ...........r(...
-000006c0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000006d0: 0004 0000 0040 0000 0073 6600 0000 6500  .....@...sf...e.
-000006e0: 5a01 6400 5a02 5500 6503 6504 1900 6505  Z.d.Z.U.e.e...e.
-000006f0: 6401 3c00 6402 5a06 6503 6507 6504 6508  d.<.d.Z.e.e.e.e.
-00000700: 6602 1900 1900 6505 6403 3c00 6503 6509  f.....e.d.<.e.e.
-00000710: 1900 6505 6404 3c00 650a 6401 6405 6406  ..e.d.<.e.d.d.d.
-00000720: 8d02 650b 6401 8301 8301 5a0c 650a 6407  ..e.d.....Z.e.d.
-00000730: 6405 6406 8d02 650b 6407 8301 8301 5a0d  d.d...e.d.....Z.
-00000740: 6402 5300 2908 720f 0000 0072 2900 0000  d.S.).r....r)...
-00000750: 4e72 2c00 0000 722d 0000 0054 7220 0000  Nr,...r-...Tr ..
-00000760: 0072 2a00 0000 290e 7217 0000 0072 1800  .r*...).r....r..
-00000770: 0000 7219 0000 0072 0500 0000 721b 0000  ..r....r....r...
-00000780: 0072 1c00 0000 722c 0000 0072 0300 0000  .r....r,...r....
-00000790: 7202 0000 0072 2e00 0000 7207 0000 0072  r....r....r....r
-000007a0: 0b00 0000 da05 5f6e 616d 65da 055f 7479  ......_name.._ty
-000007b0: 7065 721d 0000 0072 1d00 0000 721d 0000  per....r....r...
-000007c0: 0072 1e00 0000 720f 0000 0049 0000 0073  .r....r....I...s
-000007d0: 0c00 0000 0a00 0c01 1801 0c01 1403 1801  ................
-000007e0: 720f 0000 0063 0000 0000 0000 0000 0000  r....c..........
-000007f0: 0000 0000 0000 0400 0000 4000 0000 7334  ..........@...s4
-00000800: 0000 0065 005a 0164 005a 0265 0364 0164  ...e.Z.d.Z.e.d.d
-00000810: 0264 038d 0265 0464 0183 0183 015a 0565  .d...e.d.....Z.e
-00000820: 0364 0464 0264 038d 0265 0464 0483 0183  .d.d.d...e.d....
-00000830: 015a 0664 0553 0029 0672 1000 0000 7229  .Z.d.S.).r....r)
-00000840: 0000 0054 7220 0000 0072 2a00 0000 4e29  ...Tr ...r*...N)
-00000850: 0772 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000860: 7207 0000 0072 0b00 0000 722f 0000 0072  r....r....r/...r
-00000870: 3000 0000 721d 0000 0072 1d00 0000 721d  0...r....r....r.
-00000880: 0000 0072 1e00 0000 7210 0000 0053 0000  ...r....r....S..
-00000890: 0073 0600 0000 0800 1402 1801 7210 0000  .s..........r...
-000008a0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000008b0: 0000 0300 0000 4000 0000 7332 0000 0065  ......@...s2...e
-000008c0: 005a 0164 005a 0255 0065 0365 0464 013c  .Z.d.Z.U.e.e.d.<
-000008d0: 0065 0565 0619 0065 0464 023c 0065 0365  .e.e...e.d.<.e.e
-000008e0: 0464 033c 0065 0765 0464 043c 0064 0553  .d.<.e.e.d.<.d.S
-000008f0: 0029 0672 1100 0000 7225 0000 00da 0d72  .).r....r%.....r
-00000900: 6573 6f75 7263 655f 6c69 7374 da0a 7072  esource_list..pr
-00000910: 6f6a 6563 745f 6964 722d 0000 004e 2908  oject_idr-...N).
-00000920: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-00000930: 2700 0000 721c 0000 0072 0400 0000 7213  '...r....r....r.
-00000940: 0000 0072 2e00 0000 721d 0000 0072 1d00  ...r....r....r..
-00000950: 0000 721d 0000 0072 1e00 0000 7211 0000  ..r....r....r...
-00000960: 0059 0000 0073 0a00 0000 0a00 0801 0c01  .Y...s..........
-00000970: 0801 0c01 7211 0000 0063 0000 0000 0000  ....r....c......
-00000980: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000990: 0000 7326 0000 0065 005a 0164 005a 0255  ..s&...e.Z.d.Z.U
-000009a0: 0064 015a 0365 0465 0564 023c 0064 035a  .d.Z.e.e.d.<.d.Z
-000009b0: 0665 0765 0564 043c 0064 0553 0029 06da  .e.e.d.<.d.S.)..
-000009c0: 0c5f 5072 6f6a 6563 7442 6173 657a 5a0a  ._ProjectBasezZ.
-000009d0: 2020 2020 4261 7365 2063 6c61 7373 2066      Base class f
-000009e0: 6f72 2050 726f 6a65 6374 0a0a 2020 2020  or Project..    
-000009f0: 4174 7472 6962 7574 6573 3a0a 2020 2020  Attributes:.    
-00000a00: 2020 2020 6e61 6d65 3a20 5442 440a 2020      name: TBD.  
-00000a10: 2020 2020 2020 7265 6164 5f6f 6e6c 793a        read_only:
-00000a20: 2054 4244 0a20 2020 2072 2900 0000 4672   TBD.    r)...Fr
-00000a30: 2d00 0000 4e29 0872 1700 0000 7218 0000  -...N).r....r...
-00000a40: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000a50: 721c 0000 0072 2d00 0000 722e 0000 0072  r....r-...r....r
-00000a60: 1d00 0000 721d 0000 0072 1d00 0000 721e  ....r....r....r.
-00000a70: 0000 0072 3300 0000 6300 0000 7308 0000  ...r3...c...s...
-00000a80: 000a 0004 0108 0810 0172 3300 0000 6300  .........r3...c.
-00000a90: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00000aa0: 0000 0040 0000 0073 4600 0000 6500 5a01  ...@...sF...e.Z.
-00000ab0: 6400 5a02 5500 6401 5a03 6504 6505 1900  d.Z.U.d.Z.e.e...
-00000ac0: 6506 6402 3c00 6507 6403 6404 6405 8d02  e.d.<.e.d.d.d...
-00000ad0: 6508 6403 8301 8301 5a09 6507 6402 6404  e.d.....Z.e.d.d.
-00000ae0: 6405 8d02 6508 6402 8301 8301 5a0a 6406  d...e.d.....Z.d.
-00000af0: 5300 2907 720c 0000 0072 2b00 0000 da14  S.).r....r+.....
-00000b00: 6465 6661 756c 745f 6461 7461 7365 745f  default_dataset_
-00000b10: 6e61 6d65 7229 0000 0054 7220 0000 004e  namer)...Tr ...N
-00000b20: 290b 7217 0000 0072 1800 0000 7219 0000  ).r....r....r...
-00000b30: 0072 3400 0000 7205 0000 0072 1b00 0000  .r4...r....r....
-00000b40: 721c 0000 0072 0700 0000 720b 0000 0072  r....r....r....r
-00000b50: 2f00 0000 da15 5f64 6566 6175 6c74 5f64  /....._default_d
-00000b60: 6174 6173 6574 5f6e 616d 6572 1d00 0000  ataset_namer....
-00000b70: 721d 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00000b80: 0c00 0000 7000 0000 7310 0000 000a 0010  ....p...s.......
-00000b90: 0114 0302 0104 0104 ff06 0208 fe72 0c00  .............r..
-00000ba0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000bb0: 0000 0003 0000 0040 0000 0073 2600 0000  .......@...s&...
-00000bc0: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
-00000bd0: 3c00 6700 5a05 6506 6507 1900 6504 6402  <.g.Z.e.e...e.d.
-00000be0: 3c00 6403 5300 2904 720d 0000 0072 2500  <.d.S.).r....r%.
-00000bf0: 0000 da0c 6461 7461 7365 745f 6c69 7374  ....dataset_list
-00000c00: 4e29 0872 1700 0000 7218 0000 0072 1900  N).r....r....r..
-00000c10: 0000 7227 0000 0072 1c00 0000 7236 0000  ..r'...r....r6..
-00000c20: 0072 0400 0000 7211 0000 0072 1d00 0000  .r....r....r....
-00000c30: 721d 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00000c40: 0d00 0000 7a00 0000 7306 0000 000a 0008  ....z...s.......
-00000c50: 0114 0172 0d00 0000 6300 0000 0000 0000  ...r....c.......
-00000c60: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000c70: 0073 3a00 0000 6500 5a01 6400 5a02 5500  .s:...e.Z.d.Z.U.
-00000c80: 6503 6504 1900 6505 6401 3c00 6503 6506  e.e...e.d.<.e.e.
-00000c90: 1900 6505 6402 3c00 6507 6401 6403 6404  ..e.d.<.e.d.d.d.
-00000ca0: 8d02 6508 6401 8301 8301 5a09 6405 5300  ..e.d.....Z.d.S.
-00000cb0: 2906 720e 0000 0072 2900 0000 722d 0000  ).r....r)...r-..
-00000cc0: 0054 7220 0000 004e 290a 7217 0000 0072  .Tr ...N).r....r
-00000cd0: 1800 0000 7219 0000 0072 0500 0000 721b  ....r....r....r.
-00000ce0: 0000 0072 1c00 0000 722e 0000 0072 0700  ...r....r....r..
-00000cf0: 0000 720b 0000 0072 2f00 0000 721d 0000  ..r....r/...r...
-00000d00: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00000d10: 720e 0000 007f 0000 0073 0800 0000 0a00  r........s......
-00000d20: 0c01 0c01 1803 720e 0000 004e 291a da06  ......r....N)...
-00000d30: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
-00000d40: 7204 0000 0072 0500 0000 da08 7079 6461  r....r......pyda
-00000d50: 6e74 6963 7206 0000 0072 0700 0000 da08  nticr....r......
-00000d60: 7371 6c6d 6f64 656c 7208 0000 00da 0b5f  sqlmodelr......_
-00000d70: 7661 6c69 6461 746f 7273 720a 0000 0072  validatorsr....r
-00000d80: 0b00 0000 da07 5f5f 616c 6c5f 5f72 1500  ......__all__r..
-00000d90: 0000 7212 0000 0072 1400 0000 7213 0000  ..r....r....r...
-00000da0: 0072 2800 0000 720f 0000 0072 1000 0000  .r(...r....r....
-00000db0: 7211 0000 0072 3300 0000 720c 0000 0072  r....r3...r....r
-00000dc0: 0d00 0000 720e 0000 0072 1d00 0000 721d  ....r....r....r.
-00000dd0: 0000 0072 1d00 0000 721e 0000 00da 083c  ...r....r......<
-00000de0: 6d6f 6475 6c65 3e01 0000 0073 2c00 0000  module>....s,...
-00000df0: 0c00 0c01 0c01 0c01 0c02 0c01 0c01 0c02  ................
-00000e00: 0c01 0403 1010 1008 1005 1005 1008 1011  ................
-00000e10: 100a 1006 100a 100d 100a 1405            ............
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
+000002f0: 721b 0000 00fa 4d2f 686f 6d65 2f74 6f6d  r.....M/home/tom
+00000300: 6d61 736f 2f46 7261 6374 616c 2f66 7261  maso/Fractal/fra
+00000310: 6374 616c 2d73 6572 7665 722f 6672 6163  ctal-server/frac
+00000320: 7461 6c5f 7365 7276 6572 2f63 6f6d 6d6f  tal_server/commo
+00000330: 6e2f 7363 6865 6d61 732f 7072 6f6a 6563  n/schemas/projec
+00000340: 742e 7079 7213 0000 001c 0000 0073 0600  t.pyr........s..
+00000350: 0000 0a00 0401 0c04 7213 0000 0063 0000  ........r....c..
+00000360: 0000 0000 0000 0000 0000 0000 0000 0400  ................
+00000370: 0000 4000 0000 f320 0000 0065 005a 0164  ..@.... ...e.Z.d
+00000380: 005a 0265 0364 0164 0264 038d 0265 0464  .Z.e.d.d.d...e.d
+00000390: 0183 0183 015a 0564 0453 0029 0572 1000  .....Z.d.S.).r..
+000003a0: 0000 7214 0000 0054 a901 da0b 616c 6c6f  ..r....T....allo
+000003b0: 775f 7265 7573 654e a906 7215 0000 0072  w_reuseN..r....r
+000003c0: 1600 0000 7217 0000 0072 0600 0000 7208  ....r....r....r.
+000003d0: 0000 00da 055f 7061 7468 721b 0000 0072  ....._pathr....r
+000003e0: 1b00 0000 721b 0000 0072 1c00 0000 7210  ....r....r....r.
+000003f0: 0000 0024 0000 00f3 0400 0000 0800 1802  ...$............
+00000400: 7210 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000410: 0000 0000 0000 0400 0000 4000 0000 721d  ..........@...r.
+00000420: 0000 0029 0572 1200 0000 7214 0000 0054  ...).r....r....T
+00000430: 721e 0000 004e 7220 0000 0072 1b00 0000  r....Nr ...r....
+00000440: 721b 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+00000450: 1200 0000 2900 0000 7222 0000 0072 1200  ....)...r"...r..
+00000460: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000470: 0000 0003 0000 0040 0000 0073 1e00 0000  .......@...s....
+00000480: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
+00000490: 3c00 6503 6504 6402 3c00 6403 5300 2904  <.e.e.d.<.d.S.).
+000004a0: 7211 0000 00da 0269 64da 0a64 6174 6173  r......id..datas
+000004b0: 6574 5f69 644e 2905 7215 0000 0072 1600  et_idN).r....r..
+000004c0: 0000 7217 0000 00da 0369 6e74 721a 0000  ..r......intr...
+000004d0: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
+000004e0: 721c 0000 0072 1100 0000 2e00 0000 7306  r....r........s.
+000004f0: 0000 000a 0008 010c 0172 1100 0000 6300  .........r....c.
+00000500: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000510: 0000 0040 0000 0073 4c00 0000 6500 5a01  ...@...sL...e.Z.
+00000520: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
+00000530: 3c00 6506 6504 1900 6505 6403 3c00 6507  <.e.e...e.d.<.e.
+00000540: 6900 6404 8d01 5a08 6509 6504 650a 6602  i.d...Z.e.e.e.f.
+00000550: 1900 6505 6405 3c00 6406 5a0b 650c 6505  ..e.d.<.d.Z.e.e.
+00000560: 6407 3c00 6408 5300 2909 da0c 5f44 6174  d.<.d.S.)..._Dat
+00000570: 6173 6574 4261 7365 7a7e 0a20 2020 2042  asetBasez~.    B
+00000580: 6173 6520 636c 6173 7320 666f 7220 4461  ase class for Da
+00000590: 7461 7365 740a 0a20 2020 2041 7474 7269  taset..    Attri
+000005a0: 6275 7465 733a 0a20 2020 2020 2020 206e  butes:.        n
+000005b0: 616d 653a 2054 4244 0a20 2020 2020 2020  ame: TBD.       
+000005c0: 2074 7970 653a 2054 4244 0a20 2020 2020   type: TBD.     
+000005d0: 2020 206d 6574 613a 2054 4244 0a20 2020     meta: TBD.   
+000005e0: 2020 2020 2072 6561 645f 6f6e 6c79 3a20       read_only: 
+000005f0: 5442 440a 2020 2020 da04 6e61 6d65 da04  TBD.    ..name..
+00000600: 7479 7065 2901 da07 6465 6661 756c 74da  type)...default.
+00000610: 046d 6574 6146 da09 7265 6164 5f6f 6e6c  .metaF..read_onl
+00000620: 794e 290d 7215 0000 0072 1600 0000 7217  yN).r....r....r.
+00000630: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
+00000640: 0000 7203 0000 0072 0500 0000 722a 0000  ..r....r....r*..
+00000650: 00da 0464 6963 7472 0200 0000 722b 0000  ...dictr....r+..
+00000660: 00da 0462 6f6f 6c72 1b00 0000 721b 0000  ...boolr....r...
+00000670: 0072 1b00 0000 721c 0000 0072 2600 0000  .r....r....r&...
+00000680: 3600 0000 730c 0000 000a 0004 0108 0a0c  6...s...........
+00000690: 011a 0110 0172 2600 0000 6300 0000 0000  .....r&...c.....
+000006a0: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
+000006b0: 0000 0073 6600 0000 6500 5a01 6400 5a02  ...sf...e.Z.d.Z.
+000006c0: 5500 6503 6504 1900 6505 6401 3c00 6402  U.e.e...e.d.<.d.
+000006d0: 5a06 6503 6507 6504 6508 6602 1900 1900  Z.e.e.e.e.f.....
+000006e0: 6505 6403 3c00 6503 6509 1900 6505 6404  e.d.<.e.e...e.d.
+000006f0: 3c00 650a 6401 6405 6406 8d02 650b 6401  <.e.d.d.d...e.d.
+00000700: 8301 8301 5a0c 650a 6407 6405 6406 8d02  ....Z.e.d.d.d...
+00000710: 650b 6407 8301 8301 5a0d 6402 5300 2908  e.d.....Z.d.S.).
+00000720: 720d 0000 0072 2700 0000 4e72 2a00 0000  r....r'...Nr*...
+00000730: 722b 0000 0054 721e 0000 0072 2800 0000  r+...Tr....r(...
+00000740: 290e 7215 0000 0072 1600 0000 7217 0000  ).r....r....r...
+00000750: 0072 0300 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00000760: 722a 0000 0072 2c00 0000 7202 0000 0072  r*...r,...r....r
+00000770: 2d00 0000 7206 0000 0072 0900 0000 da05  -...r....r......
+00000780: 5f6e 616d 65da 055f 7479 7065 721b 0000  _name.._typer...
+00000790: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+000007a0: 720d 0000 0047 0000 0073 0c00 0000 0a00  r....G...s......
+000007b0: 0c01 1801 0c01 1403 1801 720d 0000 0063  ..........r....c
+000007c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007d0: 0400 0000 4000 0000 7334 0000 0065 005a  ....@...s4...e.Z
+000007e0: 0164 005a 0265 0364 0164 0264 038d 0265  .d.Z.e.d.d.d...e
+000007f0: 0464 0183 0183 015a 0565 0364 0464 0264  .d.....Z.e.d.d.d
+00000800: 038d 0265 0464 0483 0183 015a 0664 0553  ...e.d.....Z.d.S
+00000810: 0029 0672 0e00 0000 7227 0000 0054 721e  .).r....r'...Tr.
+00000820: 0000 0072 2800 0000 4e29 0772 1500 0000  ...r(...N).r....
+00000830: 7216 0000 0072 1700 0000 7206 0000 0072  r....r....r....r
+00000840: 0900 0000 722e 0000 0072 2f00 0000 721b  ....r....r/...r.
+00000850: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
+00000860: 0000 720e 0000 0051 0000 0073 0600 0000  ..r....Q...s....
+00000870: 0800 1402 1801 720e 0000 0063 0000 0000  ......r....c....
+00000880: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000890: 4000 0000 7332 0000 0065 005a 0164 005a  @...s2...e.Z.d.Z
+000008a0: 0255 0065 0365 0464 013c 0065 0565 0619  .U.e.e.d.<.e.e..
+000008b0: 0065 0464 023c 0065 0365 0464 033c 0065  .e.d.<.e.e.d.<.e
+000008c0: 0765 0464 043c 0064 0553 0029 0672 0f00  .e.d.<.d.S.).r..
+000008d0: 0000 7223 0000 00da 0d72 6573 6f75 7263  ..r#.....resourc
+000008e0: 655f 6c69 7374 da0a 7072 6f6a 6563 745f  e_list..project_
+000008f0: 6964 722b 0000 004e 2908 7215 0000 0072  idr+...N).r....r
+00000900: 1600 0000 7217 0000 0072 2500 0000 721a  ....r....r%...r.
+00000910: 0000 00da 046c 6973 7472 1100 0000 722d  .....listr....r-
+00000920: 0000 0072 1b00 0000 721b 0000 0072 1b00  ...r....r....r..
+00000930: 0000 721c 0000 0072 0f00 0000 5700 0000  ..r....r....W...
+00000940: 730a 0000 000a 0008 010c 0108 010c 0172  s..............r
+00000950: 0f00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000960: 0000 0000 0003 0000 0040 0000 0073 2600  .........@...s&.
+00000970: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
+00000980: 6504 6505 6402 3c00 6403 5a06 6507 6505  e.e.d.<.d.Z.e.e.
+00000990: 6404 3c00 6405 5300 2906 da0c 5f50 726f  d.<.d.S.)..._Pro
+000009a0: 6a65 6374 4261 7365 7a5a 0a20 2020 2042  jectBasezZ.    B
+000009b0: 6173 6520 636c 6173 7320 666f 7220 5072  ase class for Pr
+000009c0: 6f6a 6563 740a 0a20 2020 2041 7474 7269  oject..    Attri
+000009d0: 6275 7465 733a 0a20 2020 2020 2020 206e  butes:.        n
+000009e0: 616d 653a 2054 4244 0a20 2020 2020 2020  ame: TBD.       
+000009f0: 2072 6561 645f 6f6e 6c79 3a20 5442 440a   read_only: TBD.
+00000a00: 2020 2020 7227 0000 0046 722b 0000 004e      r'...Fr+...N
+00000a10: 2908 7215 0000 0072 1600 0000 7217 0000  ).r....r....r...
+00000a20: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00000a30: 722b 0000 0072 2d00 0000 721b 0000 0072  r+...r-...r....r
+00000a40: 1b00 0000 721b 0000 0072 1c00 0000 7233  ....r....r....r3
+00000a50: 0000 0061 0000 0073 0800 0000 0a00 0401  ...a...s........
+00000a60: 0808 1001 7233 0000 0063 0000 0000 0000  ....r3...c......
+00000a70: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+00000a80: 0000 7346 0000 0065 005a 0164 005a 0255  ..sF...e.Z.d.Z.U
+00000a90: 0064 015a 0365 0465 0519 0065 0664 023c  .d.Z.e.e...e.d.<
+00000aa0: 0065 0764 0364 0464 058d 0265 0864 0383  .e.d.d.d...e.d..
+00000ab0: 0183 015a 0965 0764 0264 0464 058d 0265  ...Z.e.d.d.d...e
+00000ac0: 0864 0283 0183 015a 0a64 0653 0029 0772  .d.....Z.d.S.).r
+00000ad0: 0a00 0000 7229 0000 00da 1464 6566 6175  ....r).....defau
+00000ae0: 6c74 5f64 6174 6173 6574 5f6e 616d 6572  lt_dataset_namer
+00000af0: 2700 0000 5472 1e00 0000 4e29 0b72 1500  '...Tr....N).r..
+00000b00: 0000 7216 0000 0072 1700 0000 7234 0000  ..r....r....r4..
+00000b10: 0072 0300 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00000b20: 7206 0000 0072 0900 0000 722e 0000 00da  r....r....r.....
+00000b30: 155f 6465 6661 756c 745f 6461 7461 7365  ._default_datase
+00000b40: 745f 6e61 6d65 721b 0000 0072 1b00 0000  t_namer....r....
+00000b50: 721b 0000 0072 1c00 0000 720a 0000 006e  r....r....r....n
+00000b60: 0000 0073 1000 0000 0a00 1001 1403 0201  ...s............
+00000b70: 0401 04ff 0602 08fe 720a 0000 0063 0000  ........r....c..
+00000b80: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00000b90: 0000 4000 0000 7326 0000 0065 005a 0164  ..@...s&...e.Z.d
+00000ba0: 005a 0255 0065 0365 0464 013c 0067 005a  .Z.U.e.e.d.<.g.Z
+00000bb0: 0565 0665 0719 0065 0464 023c 0064 0353  .e.e...e.d.<.d.S
+00000bc0: 0029 0472 0b00 0000 7223 0000 00da 0c64  .).r....r#.....d
+00000bd0: 6174 6173 6574 5f6c 6973 744e 2908 7215  ataset_listN).r.
+00000be0: 0000 0072 1600 0000 7217 0000 0072 2500  ...r....r....r%.
+00000bf0: 0000 721a 0000 0072 3600 0000 7232 0000  ..r....r6...r2..
+00000c00: 0072 0f00 0000 721b 0000 0072 1b00 0000  .r....r....r....
+00000c10: 721b 0000 0072 1c00 0000 720b 0000 0078  r....r....r....x
+00000c20: 0000 0073 0600 0000 0a00 0801 1401 720b  ...s..........r.
+00000c30: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000c40: 0000 0000 0400 0000 4000 0000 733a 0000  ........@...s:..
+00000c50: 0065 005a 0164 005a 0255 0065 0365 0419  .e.Z.d.Z.U.e.e..
+00000c60: 0065 0564 013c 0065 0365 0619 0065 0564  .e.d.<.e.e...e.d
+00000c70: 023c 0065 0764 0164 0364 048d 0265 0864  .<.e.d.d.d...e.d
+00000c80: 0183 0183 015a 0964 0553 0029 0672 0c00  .....Z.d.S.).r..
+00000c90: 0000 7227 0000 0072 2b00 0000 5472 1e00  ..r'...r+...Tr..
+00000ca0: 0000 4e29 0a72 1500 0000 7216 0000 0072  ..N).r....r....r
+00000cb0: 1700 0000 7203 0000 0072 1900 0000 721a  ....r....r....r.
+00000cc0: 0000 0072 2d00 0000 7206 0000 0072 0900  ...r-...r....r..
+00000cd0: 0000 722e 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+00000ce0: 0072 1b00 0000 721c 0000 0072 0c00 0000  .r....r....r....
+00000cf0: 7d00 0000 7308 0000 000a 000c 010c 0118  }...s...........
+00000d00: 0372 0c00 0000 4e29 17da 0674 7970 696e  .r....N)...typin
+00000d10: 6772 0200 0000 7203 0000 00da 0870 7964  gr....r......pyd
+00000d20: 616e 7469 6372 0400 0000 7205 0000 0072  anticr....r....r
+00000d30: 0600 0000 da0b 5f76 616c 6964 6174 6f72  ......_validator
+00000d40: 7372 0800 0000 7209 0000 00da 075f 5f61  sr....r......__a
+00000d50: 6c6c 5f5f 7213 0000 0072 1000 0000 7212  ll__r....r....r.
+00000d60: 0000 0072 1100 0000 7226 0000 0072 0d00  ...r....r&...r..
+00000d70: 0000 720e 0000 0072 0f00 0000 7233 0000  ..r....r....r3..
+00000d80: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+00000d90: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
+00000da0: 1c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000db0: 0000 7328 0000 000c 000c 010c 020c 010c  ..s(............
+00000dc0: 010c 020c 0104 0310 1010 0810 0510 0510  ................
+00000dd0: 0810 1110 0a10 0610 0a10 0d10 0a14 05    ...............
```

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  8 12:01:46 2023 UTC, .py size: 695 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,74 @@
-00000000: 6f0d 0d0a 0000 0000 aae4 5864 b702 0000  o.........Xd....
+00000000: 6f0d 0d0a 0000 0000 b554 7064 a102 0000  o........Tpd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
+00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c01 6d03 5a03  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c01 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c05 6d06 5a06 0100 6406 5a07 4700  d.l.m.Z...d.Z.G.
-00000070: 6407 6408 8400 6408 6506 8303 5a08 4700  d.d...d.e...Z.G.
-00000080: 6409 640a 8400 640a 6508 8303 5a09 640b  d.d...d.e...Z.d.
-00000090: 5300 290c e900 0000 0029 01da 0864 6174  S.)......)...dat
-000000a0: 6574 696d 6529 01da 0341 6e79 2901 da04  etime)...Any)...
-000000b0: 4469 6374 2901 da08 4f70 7469 6f6e 616c  Dict)...Optional
-000000c0: 2901 da08 5351 4c4d 6f64 656c 2902 da0a  )...SQLModel)...
-000000d0: 5f53 7461 7465 4261 7365 da09 5374 6174  _StateBase..Stat
-000000e0: 6552 6561 6463 0000 0000 0000 0000 0000  eReadc..........
-000000f0: 0000 0000 0000 0300 0000 4000 0000 7332  ..........@...s2
-00000100: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
-00000110: 0365 0465 0565 0666 0219 0065 0764 023c  .e.e.e.f...e.d.<
-00000120: 0065 0865 0764 033c 0064 0464 0584 005a  .e.e.d.<.d.d...Z
-00000130: 0964 0653 0029 0772 0700 0000 7a97 0a20  .d.S.).r....z.. 
-00000140: 2020 2042 6173 6520 636c 6173 7320 666f     Base class fo
-00000150: 7220 6053 7461 7465 600a 0a20 2020 2041  r `State`..    A
-00000160: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
-00000170: 2020 2069 643a 2050 7269 6d61 7279 206b     id: Primary k
-00000180: 6579 0a20 2020 2020 2020 2064 6174 613a  ey.        data:
-00000190: 2043 6f6e 7465 6e74 206f 6620 7468 6520   Content of the 
-000001a0: 7374 6174 650a 2020 2020 2020 2020 7469  state.        ti
-000001b0: 6d65 7374 616d 703a 2054 696d 6520 7374  mestamp: Time st
-000001c0: 616d 7020 6f66 2074 6865 2073 7461 7465  amp of the state
-000001d0: 0a20 2020 20da 0464 6174 61da 0974 696d  .    ..data..tim
-000001e0: 6573 7461 6d70 6301 0000 0000 0000 0000  estampc.........
-000001f0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00000200: 1a00 0000 7c00 a000 a100 7d01 7401 7c00  ....|.....}.t.|.
-00000210: 6a02 8301 7c01 6401 3c00 7c01 5300 2902  j...|.d.<.|.S.).
-00000220: 7a51 0a20 2020 2020 2020 2052 6574 7572  zQ.        Retur
-00000230: 6e20 6073 656c 662e 6469 6374 2829 6020  n `self.dict()` 
-00000240: 6166 7465 7220 6361 7374 696e 6720 6073  after casting `s
-00000250: 656c 662e 7469 6d65 7374 616d 7060 2074  elf.timestamp` t
-00000260: 6f20 6120 7374 7269 6e67 0a20 2020 2020  o a string.     
-00000270: 2020 2072 0a00 0000 2903 da04 6469 6374     r....)...dict
-00000280: da03 7374 7272 0a00 0000 2902 da04 7365  ..strr....)...se
-00000290: 6c66 da01 64a9 0072 0f00 0000 fa4b 2f68  lf..d..r.....K/h
-000002a0: 6f6d 652f 746f 6d6d 6173 6f2f 4672 6163  ome/tommaso/Frac
-000002b0: 7461 6c2f 6672 6163 7461 6c2d 7365 7276  tal/fractal-serv
-000002c0: 6572 2f66 7261 6374 616c 5f73 6572 7665  er/fractal_serve
-000002d0: 722f 636f 6d6d 6f6e 2f73 6368 656d 6173  r/common/schemas
-000002e0: 2f73 7461 7465 2e70 79da 0e73 616e 6974  /state.py..sanit
-000002f0: 6973 6564 5f64 6963 741c 0000 0073 0600  ised_dict....s..
-00000300: 0000 0804 0e01 0401 7a19 5f53 7461 7465  ........z._State
-00000310: 4261 7365 2e73 616e 6974 6973 6564 5f64  Base.sanitised_d
-00000320: 6963 744e 290a da08 5f5f 6e61 6d65 5f5f  ictN)...__name__
-00000330: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000340: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00000350: 635f 5f72 0400 0000 720c 0000 0072 0300  c__r....r....r..
-00000360: 0000 da0f 5f5f 616e 6e6f 7461 7469 6f6e  ....__annotation
-00000370: 735f 5f72 0200 0000 7211 0000 0072 0f00  s__r....r....r..
-00000380: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00000390: 0072 0700 0000 0f00 0000 730a 0000 000a  .r........s.....
-000003a0: 0004 0110 0908 010c 0272 0700 0000 6300  .........r....c.
-000003b0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-000003c0: 0000 0040 0000 0073 1a00 0000 6500 5a01  ...@...s....e.Z.
-000003d0: 6400 5a02 5500 6503 6504 1900 6505 6401  d.Z.U.e.e...e.d.
-000003e0: 3c00 6402 5300 2903 7208 0000 00da 0269  <.d.S.).r......i
-000003f0: 644e 2906 7212 0000 0072 1300 0000 7214  dN).r....r....r.
-00000400: 0000 0072 0500 0000 da03 696e 7472 1600  ...r......intr..
-00000410: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-00000420: 0072 1000 0000 7208 0000 0025 0000 0073  .r....r....%...s
-00000430: 0400 0000 0a00 1001 7208 0000 004e 290a  ........r....N).
-00000440: 7202 0000 00da 0674 7970 696e 6772 0300  r......typingr..
-00000450: 0000 7204 0000 0072 0500 0000 da08 7371  ..r....r......sq
-00000460: 6c6d 6f64 656c 7206 0000 00da 075f 5f61  lmodelr......__a
-00000470: 6c6c 5f5f 7207 0000 0072 0800 0000 720f  ll__r....r....r.
-00000480: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00000490: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000004a0: 7310 0000 000c 000c 010c 010c 010c 0204  s...............
-000004b0: 0310 0614 16                             .....
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
+00000280: 0164 a900 720e 0000 00fa 4b2f 686f 6d65  .d..r.....K/home
+00000290: 2f74 6f6d 6d61 736f 2f46 7261 6374 616c  /tommaso/Fractal
+000002a0: 2f66 7261 6374 616c 2d73 6572 7665 722f  /fractal-server/
+000002b0: 6672 6163 7461 6c5f 7365 7276 6572 2f63  fractal_server/c
+000002c0: 6f6d 6d6f 6e2f 7363 6865 6d61 732f 7374  ommon/schemas/st
+000002d0: 6174 652e 7079 da0e 7361 6e69 7469 7365  ate.py..sanitise
+000002e0: 645f 6469 6374 1b00 0000 7306 0000 0008  d_dict....s.....
+000002f0: 040e 0104 017a 195f 5374 6174 6542 6173  .....z._StateBas
+00000300: 652e 7361 6e69 7469 7365 645f 6469 6374  e.sanitised_dict
+00000310: 4e29 0ada 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000320: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000330: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00000340: 720a 0000 0072 0b00 0000 7203 0000 00da  r....r....r.....
+00000350: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
+00000360: 7202 0000 0072 1000 0000 720e 0000 0072  r....r....r....r
+00000370: 0e00 0000 720e 0000 0072 0f00 0000 7206  ....r....r....r.
+00000380: 0000 000e 0000 0073 0a00 0000 0a00 0401  .......s........
+00000390: 1009 0801 0c02 7206 0000 0063 0000 0000  ......r....c....
+000003a0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+000003b0: 4000 0000 731a 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+000003c0: 0255 0065 0365 0419 0065 0564 013c 0064  .U.e.e...e.d.<.d
+000003d0: 0253 0029 0372 0700 0000 da02 6964 4e29  .S.).r......idN)
+000003e0: 0672 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+000003f0: 7204 0000 00da 0369 6e74 7215 0000 0072  r......intr....r
+00000400: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
+00000410: 0000 0072 0700 0000 2400 0000 7304 0000  ...r....$...s...
+00000420: 000a 0010 0172 0700 0000 4e29 0972 0200  .....r....N).r..
+00000430: 0000 da06 7479 7069 6e67 7203 0000 0072  ....typingr....r
+00000440: 0400 0000 da08 7079 6461 6e74 6963 7205  ......pydanticr.
+00000450: 0000 00da 075f 5f61 6c6c 5f5f 7206 0000  .....__all__r...
+00000460: 0072 0700 0000 720e 0000 0072 0e00 0000  .r....r....r....
+00000470: 720e 0000 0072 0f00 0000 da08 3c6d 6f64  r....r......<mod
+00000480: 756c 653e 0100 0000 730e 0000 000c 000c  ule>....s.......
+00000490: 010c 010c 0204 0310 0614 16              ...........
```

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 11:24:30 2023 UTC, .py size: 2502 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,248 +1,244 @@
-00000000: 6f0d 0d0a 0000 0000 6e2d 5a64 c609 0000  o.......n-Zd....
+00000000: 6f0d 0d0a 0000 0000 b554 7064 9909 0000  o........Tpd....
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
-00000390: 4e2f 686f 6d65 2f74 6f6d 6d61 736f 2f46  N/home/tommaso/F
-000003a0: 7261 6374 616c 2f66 7261 6374 616c 2d73  ractal/fractal-s
-000003b0: 6572 7665 722f 6672 6163 7461 6c5f 7365  erver/fractal_se
-000003c0: 7276 6572 2f63 6f6d 6d6f 6e2f 7363 6865  rver/common/sche
-000003d0: 6d61 732f 776f 726b 666c 6f77 2e70 7972  mas/workflow.pyr
-000003e0: 1800 0000 1e00 0000 7306 0000 000a 0018  ........s.......
-000003f0: 021c 0172 1800 0000 6300 0000 0000 0000  ...r....c.......
-00000400: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
-00000410: 0073 3200 0000 6500 5a01 6400 5a02 5500  .s2...e.Z.d.Z.U.
-00000420: 6503 6504 1900 6505 6401 3c00 6506 6401  e.e...e.d.<.e.d.
-00000430: 6402 6403 8d02 6507 6401 6404 6405 8d02  d.d...e.d.d.d...
-00000440: 8301 5a08 6406 5300 2907 7213 0000 00da  ..Z.d.S.).r.....
-00000450: 056f 7264 6572 54a9 01da 0b61 6c6c 6f77  .orderT....allow
-00000460: 5f72 6575 7365 7201 0000 0029 01da 076d  _reuser....)...m
-00000470: 696e 5f76 616c 4e29 0972 1b00 0000 721c  in_valN).r....r.
-00000480: 0000 0072 1d00 0000 7205 0000 00da 0369  ...r....r......i
-00000490: 6e74 721f 0000 0072 0600 0000 7209 0000  ntr....r....r...
-000004a0: 00da 065f 6f72 6465 7272 2000 0000 7220  ..._orderr ...r 
-000004b0: 0000 0072 2000 0000 7221 0000 0072 1300  ...r ...r!...r..
-000004c0: 0000 2400 0000 7306 0000 000a 000c 011c  ..$...s.........
-000004d0: 0272 1300 0000 6300 0000 0000 0000 0000  .r....c.........
-000004e0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000004f0: 3a00 0000 6500 5a01 6400 5a02 5500 6503  :...e.Z.d.Z.U.e.
-00000500: 6504 6401 3c00 6505 6503 1900 6504 6402  e.d.<.e.e...e.d.
-00000510: 3c00 6503 6504 6403 3c00 6503 6504 6404  <.e.e.d.<.e.e.d.
-00000520: 3c00 6506 6504 6405 3c00 6406 5300 2907  <.e.e.d.<.d.S.).
-00000530: 7216 0000 00da 0269 6472 2200 0000 da0b  r......idr".....
-00000540: 776f 726b 666c 6f77 5f69 64da 0774 6173  workflow_id..tas
-00000550: 6b5f 6964 da04 7461 736b 4e29 0772 1b00  k_id..taskN).r..
-00000560: 0000 721c 0000 0072 1d00 0000 7226 0000  ..r....r....r&..
-00000570: 0072 1f00 0000 7205 0000 0072 0d00 0000  .r....r....r....
-00000580: 7220 0000 0072 2000 0000 7220 0000 0072  r ...r ...r ...r
-00000590: 2100 0000 7216 0000 002a 0000 0073 0c00  !...r....*...s..
-000005a0: 0000 0a00 0801 0c01 0801 0801 0c01 7216  ..............r.
-000005b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000005c0: 0000 0000 0300 0000 4000 0000 f316 0000  ........@.......
-000005d0: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
-000005e0: 013c 0064 0253 0029 0372 1400 0000 722b  .<.d.S.).r....r+
-000005f0: 0000 004e 2905 721b 0000 0072 1c00 0000  ...N).r....r....
-00000600: 721d 0000 0072 0c00 0000 721f 0000 0072  r....r....r....r
-00000610: 2000 0000 7220 0000 0072 2000 0000 7221   ...r ...r ...r!
-00000620: 0000 0072 1400 0000 3200 0000 f304 0000  ...r....2.......
-00000630: 000a 000c 0172 1400 0000 6300 0000 0000  .....r....c.....
-00000640: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00000650: 0000 0072 2c00 0000 2903 7215 0000 0072  ...r,...).r....r
-00000660: 2b00 0000 4e29 0572 1b00 0000 721c 0000  +...N).r....r...
-00000670: 0072 1d00 0000 720b 0000 0072 1f00 0000  .r....r....r....
-00000680: 7220 0000 0072 2000 0000 7220 0000 0072  r ...r ...r ...r
-00000690: 2100 0000 7215 0000 0036 0000 0072 2d00  !...r....6...r-.
-000006a0: 0000 7215 0000 0063 0000 0000 0000 0000  ..r....c........
-000006b0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-000006c0: 731c 0000 0065 005a 0164 005a 0265 0364  s....e.Z.d.Z.e.d
-000006d0: 0183 0164 0264 0384 0083 015a 0464 0453  ...d.d.....Z.d.S
-000006e0: 0029 0572 1700 0000 7219 0000 0063 0200  .).r....r....c..
-000006f0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00000700: 0000 4300 0000 7314 0000 0064 017c 0176  ..C...s....d.|.v
-00000710: 0072 0874 0064 0283 0182 017c 0153 0029  .r.t.d.....|.S.)
-00000720: 034e da15 7061 7261 6c6c 656c 697a 6174  .N..parallelizat
-00000730: 696f 6e5f 6c65 7665 6c7a 3b4f 7665 7272  ion_levelz;Overr
-00000740: 6964 696e 6720 7461 736b 2070 6172 616c  iding task paral
-00000750: 6c65 6c69 7a61 7469 6f6e 206c 6576 656c  lelization level
-00000760: 2063 7572 7265 6e74 6c79 206e 6f74 2061   currently not a
-00000770: 6c6c 6f77 6564 2901 da0a 5661 6c75 6545  llowed)...ValueE
-00000780: 7272 6f72 2902 da03 636c 73da 016d 7220  rror)...cls..mr 
-00000790: 0000 0072 2000 0000 7221 0000 00da 1e63  ...r ...r!.....c
-000007a0: 6865 636b 5f6e 6f5f 7061 7261 6c6c 656c  heck_no_parallel
-000007b0: 6973 6174 696f 6e5f 6c65 7665 6c3c 0000  isation_level<..
-000007c0: 0073 0a00 0000 0802 0201 0201 04ff 0403  .s..............
-000007d0: 7a31 576f 726b 666c 6f77 5461 736b 5570  z1WorkflowTaskUp
-000007e0: 6461 7465 2e63 6865 636b 5f6e 6f5f 7061  date.check_no_pa
-000007f0: 7261 6c6c 656c 6973 6174 696f 6e5f 6c65  rallelisation_le
-00000800: 7665 6c4e 2905 721b 0000 0072 1c00 0000  velN).r....r....
-00000810: 721d 0000 0072 0600 0000 7232 0000 0072  r....r....r2...r
-00000820: 2000 0000 7220 0000 0072 2000 0000 7221   ...r ...r ...r!
-00000830: 0000 0072 1700 0000 3a00 0000 7306 0000  ...r....:...s...
-00000840: 0008 0006 020e 0172 1700 0000 6300 0000  .......r....c...
-00000850: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000860: 0040 0000 0072 2c00 0000 2903 da0d 5f57  .@...r,...)..._W
-00000870: 6f72 6b66 6c6f 7742 6173 65da 046e 616d  orkflowBase..nam
-00000880: 654e 2905 721b 0000 0072 1c00 0000 721d  eN).r....r....r.
-00000890: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
-000008a0: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
-000008b0: 0072 3300 0000 4500 0000 722d 0000 0072  .r3...E...r-...r
-000008c0: 3300 0000 6300 0000 0000 0000 0000 0000  3...c...........
-000008d0: 0000 0000 0003 0000 0040 0000 0073 2a00  .........@...s*.
-000008e0: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-000008f0: 6401 3c00 6503 6504 6402 3c00 6505 6506  d.<.e.e.d.<.e.e.
-00000900: 1900 6504 6403 3c00 6404 5300 2905 720f  ..e.d.<.d.S.).r.
-00000910: 0000 0072 2800 0000 da0a 7072 6f6a 6563  ...r(.....projec
-00000920: 745f 6964 da09 7461 736b 5f6c 6973 744e  t_id..task_listN
-00000930: 2907 721b 0000 0072 1c00 0000 721d 0000  ).r....r....r...
-00000940: 0072 2600 0000 721f 0000 0072 0400 0000  .r&...r....r....
-00000950: 7216 0000 0072 2000 0000 7220 0000 0072  r....r ...r ...r
-00000960: 2000 0000 7221 0000 0072 0f00 0000 4900   ...r!...r....I.
-00000970: 0000 7308 0000 000a 0008 0108 0110 0172  ..s............r
-00000980: 0f00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000990: 0000 0000 0004 0000 0040 0000 0073 2000  .........@...s .
-000009a0: 0000 6500 5a01 6400 5a02 6503 6401 6402  ..e.Z.d.Z.e.d.d.
-000009b0: 6403 8d02 6504 6401 8301 8301 5a05 6404  d...e.d.....Z.d.
-000009c0: 5300 2905 720e 0000 0072 3400 0000 5472  S.).r....r4...Tr
-000009d0: 2300 0000 4e29 0672 1b00 0000 721c 0000  #...N).r....r...
-000009e0: 0072 1d00 0000 7206 0000 0072 0a00 0000  .r....r....r....
-000009f0: da05 5f6e 616d 6572 2000 0000 7220 0000  .._namer ...r ..
-00000a00: 0072 2000 0000 7221 0000 0072 0e00 0000  .r ...r!...r....
-00000a10: 4f00 0000 7304 0000 0008 0018 0272 0e00  O...s........r..
-00000a20: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000a30: 0000 0004 0000 0040 0000 0073 4e00 0000  .......@...sN...
-00000a40: 6500 5a01 6400 5a02 5500 6503 6504 1900  e.Z.d.Z.U.e.e...
-00000a50: 6505 6401 3c00 6503 6506 6507 1900 1900  e.d.<.e.e.e.....
-00000a60: 6505 6402 3c00 6508 6401 6403 6404 8d02  e.d.<.e.d.d.d...
-00000a70: 6509 6401 8301 8301 5a0a 6508 6402 8301  e.d.....Z.e.d...
-00000a80: 6405 6406 8400 8301 5a0b 6407 5300 2908  d.d.....Z.d.S.).
-00000a90: 7210 0000 0072 3400 0000 da1a 7265 6f72  r....r4.....reor
-00000aa0: 6465 7265 645f 776f 726b 666c 6f77 7461  dered_workflowta
-00000ab0: 736b 5f69 6473 5472 2300 0000 6302 0000  sk_idsTr#...c...
-00000ac0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000ad0: 0043 0000 0073 3a00 0000 7400 6401 6402  .C...s:...t.d.d.
-00000ae0: 8400 7c01 4400 8301 8301 720d 7401 6403  ..|.D.....r.t.d.
-00000af0: 8301 8201 7402 7c01 8301 7402 7403 7c01  ....t.|...t.t.|.
-00000b00: 8301 8301 6b03 721b 7401 6404 8301 8201  ....k.r.t.d.....
-00000b10: 7c01 5300 2905 4e63 0100 0000 0000 0000  |.S.).Nc........
-00000b20: 0000 0000 0200 0000 0300 0000 7300 0000  ............s...
-00000b30: 7318 0000 0081 007c 005d 077d 017c 0164  s......|.].}.|.d
-00000b40: 006b 0056 0001 0071 0264 0153 0029 0272  .k.V...q.d.S.).r
-00000b50: 0100 0000 4e72 2000 0000 2902 da02 2e30  ....Nr ...)....0
-00000b60: da01 6972 2000 0000 7220 0000 0072 2100  ..ir ...r ...r!.
-00000b70: 0000 da09 3c67 656e 6578 7072 3e5d 0000  ....<genexpr>]..
-00000b80: 0073 0400 0000 0280 1600 7a3b 576f 726b  .s........z;Work
-00000b90: 666c 6f77 5570 6461 7465 2e63 6865 636b  flowUpdate.check
-00000ba0: 5f70 6f73 6974 6976 655f 616e 645f 756e  _positive_and_un
-00000bb0: 6971 7565 2e3c 6c6f 6361 6c73 3e2e 3c67  ique.<locals>.<g
-00000bc0: 656e 6578 7072 3e7a 2d4e 6567 6174 6976  enexpr>z-Negativ
-00000bd0: 6520 6069 6460 2069 6e20 6072 656f 7264  e `id` in `reord
-00000be0: 6572 6564 5f77 6f72 6b66 6c6f 7774 6173  ered_workflowtas
-00000bf0: 6b5f 6964 7360 7a2c 6072 656f 7264 6572  k_ids`z,`reorder
-00000c00: 6564 5f77 6f72 6b66 6c6f 7774 6173 6b5f  ed_workflowtask_
-00000c10: 6964 7360 2068 6173 2072 6570 6574 6974  ids` has repetit
-00000c20: 696f 6e73 2904 da03 616e 7972 2f00 0000  ions)...anyr/...
-00000c30: da03 6c65 6eda 0373 6574 2902 7230 0000  ..len..set).r0..
-00000c40: 00da 0576 616c 7565 7220 0000 0072 2000  ...valuer ...r .
-00000c50: 0000 7221 0000 00da 1963 6865 636b 5f70  ..r!.....check_p
-00000c60: 6f73 6974 6976 655f 616e 645f 756e 6971  ositive_and_uniq
-00000c70: 7565 5b00 0000 730a 0000 0012 0208 0114  ue[...s.........
-00000c80: 0108 0104 017a 2857 6f72 6b66 6c6f 7755  .....z(WorkflowU
-00000c90: 7064 6174 652e 6368 6563 6b5f 706f 7369  pdate.check_posi
-00000ca0: 7469 7665 5f61 6e64 5f75 6e69 7175 654e  tive_and_uniqueN
-00000cb0: 290c 721b 0000 0072 1c00 0000 721d 0000  ).r....r....r...
-00000cc0: 0072 0500 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00000cd0: 7204 0000 0072 2600 0000 7206 0000 0072  r....r&...r....r
-00000ce0: 0a00 0000 7237 0000 0072 4000 0000 7220  ....r7...r@...r 
-00000cf0: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-00000d00: 0000 7210 0000 0054 0000 0073 0c00 0000  ..r....T...s....
-00000d10: 0a00 0c01 1001 1403 0602 0e01 7210 0000  ............r...
-00000d20: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000d30: 0000 0400 0000 4000 0000 732e 0000 0065  ......@...s....e
-00000d40: 005a 0164 005a 0255 0065 0365 0419 0065  .Z.d.Z.U.e.e...e
-00000d50: 0564 013c 0065 0664 0264 0364 048d 0265  .d.<.e.d.d.d...e
-00000d60: 0764 0283 0183 015a 0864 0553 0029 0672  .d.....Z.d.S.).r
-00000d70: 1100 0000 7236 0000 0072 3400 0000 5472  ....r6...r4...Tr
-00000d80: 2300 0000 4e29 0972 1b00 0000 721c 0000  #...N).r....r...
-00000d90: 0072 1d00 0000 7204 0000 0072 1400 0000  .r....r....r....
-00000da0: 721f 0000 0072 0600 0000 720a 0000 0072  r....r....r....r
-00000db0: 3700 0000 7220 0000 0072 2000 0000 7220  7...r ...r ...r 
-00000dc0: 0000 0072 2100 0000 7211 0000 0064 0000  ...r!...r....d..
-00000dd0: 0073 0600 0000 0a00 0c01 1803 7211 0000  .s..........r...
-00000de0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000df0: 0000 0300 0000 4000 0000 731a 0000 0065  ......@...s....e
-00000e00: 005a 0164 005a 0255 0065 0365 0419 0065  .Z.d.Z.U.e.e...e
-00000e10: 0564 013c 0064 0253 0029 0372 1200 0000  .d.<.d.S.).r....
-00000e20: 7236 0000 004e 2906 721b 0000 0072 1c00  r6...N).r....r..
-00000e30: 0000 721d 0000 0072 0400 0000 7215 0000  ..r....r....r...
-00000e40: 0072 1f00 0000 7220 0000 0072 2000 0000  .r....r ...r ...
-00000e50: 7220 0000 0072 2100 0000 7212 0000 006b  r ...r!...r....k
-00000e60: 0000 0073 0400 0000 0a00 1001 7212 0000  ...s........r...
-00000e70: 004e 291d da06 7479 7069 6e67 7202 0000  .N)...typingr...
-00000e80: 0072 0300 0000 7204 0000 0072 0500 0000  .r....r....r....
-00000e90: da08 7079 6461 6e74 6963 7206 0000 00da  ..pydanticr.....
-00000ea0: 0873 716c 6d6f 6465 6c72 0700 0000 da0b  .sqlmodelr......
-00000eb0: 5f76 616c 6964 6174 6f72 7372 0900 0000  _validatorsr....
-00000ec0: 720a 0000 0072 2b00 0000 720b 0000 0072  r....r+...r....r
-00000ed0: 0c00 0000 720d 0000 00da 075f 5f61 6c6c  ....r......__all
-00000ee0: 5f5f 7218 0000 0072 1300 0000 7216 0000  __r....r....r...
-00000ef0: 0072 1400 0000 7215 0000 0072 1700 0000  .r....r....r....
-00000f00: 7233 0000 0072 0f00 0000 720e 0000 0072  r3...r....r....r
-00000f10: 1000 0000 7211 0000 0072 1200 0000 7220  ....r....r....r 
-00000f20: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-00000f30: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000f40: 7330 0000 000c 000c 010c 010c 010c 020c  s0..............
-00000f50: 010c 020c 010c 010c 010c 0104 0310 0e10  ................
-00000f60: 0610 0610 0810 0410 0410 0b10 0410 0610  ................
-00000f70: 0510 1014 07                             .....
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
+00000360: 1f00 0000 721f 0000 00fa 4e2f 686f 6d65  ....r.....N/home
+00000370: 2f74 6f6d 6d61 736f 2f46 7261 6374 616c  /tommaso/Fractal
+00000380: 2f66 7261 6374 616c 2d73 6572 7665 722f  /fractal-server/
+00000390: 6672 6163 7461 6c5f 7365 7276 6572 2f63  fractal_server/c
+000003a0: 6f6d 6d6f 6e2f 7363 6865 6d61 732f 776f  ommon/schemas/wo
+000003b0: 726b 666c 6f77 2e70 7972 1600 0000 1c00  rkflow.pyr......
+000003c0: 0000 7306 0000 000a 0018 021c 0172 1600  ..s..........r..
+000003d0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000003e0: 0000 0005 0000 0040 0000 0073 3200 0000  .......@...s2...
+000003f0: 6500 5a01 6400 5a02 5500 6503 6504 1900  e.Z.d.Z.U.e.e...
+00000400: 6505 6401 3c00 6506 6401 6402 6403 8d02  e.d.<.e.d.d.d...
+00000410: 6507 6401 6404 6405 8d02 8301 5a08 6406  e.d.d.d.....Z.d.
+00000420: 5300 2907 7211 0000 00da 056f 7264 6572  S.).r......order
+00000430: 54a9 01da 0b61 6c6c 6f77 5f72 6575 7365  T....allow_reuse
+00000440: 7201 0000 0029 01da 076d 696e 5f76 616c  r....)...min_val
+00000450: 4e29 0972 1900 0000 721a 0000 0072 1b00  N).r....r....r..
+00000460: 0000 7203 0000 00da 0369 6e74 721e 0000  ..r......intr...
+00000470: 0072 0500 0000 7207 0000 00da 065f 6f72  .r....r......_or
+00000480: 6465 7272 1f00 0000 721f 0000 0072 1f00  derr....r....r..
+00000490: 0000 7220 0000 0072 1100 0000 2200 0000  ..r ...r...."...
+000004a0: 7306 0000 000a 000c 011c 0272 1100 0000  s..........r....
+000004b0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000004c0: 0003 0000 0040 0000 0073 3a00 0000 6500  .....@...s:...e.
+000004d0: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
+000004e0: 6505 6503 1900 6504 6402 3c00 6503 6504  e.e...e.d.<.e.e.
+000004f0: 6403 3c00 6503 6504 6404 3c00 6506 6504  d.<.e.e.d.<.e.e.
+00000500: 6405 3c00 6406 5300 2907 7214 0000 00da  d.<.d.S.).r.....
+00000510: 0269 6472 2100 0000 da0b 776f 726b 666c  .idr!.....workfl
+00000520: 6f77 5f69 64da 0774 6173 6b5f 6964 da04  ow_id..task_id..
+00000530: 7461 736b 4e29 0772 1900 0000 721a 0000  taskN).r....r...
+00000540: 0072 1b00 0000 7225 0000 0072 1e00 0000  .r....r%...r....
+00000550: 7203 0000 0072 0b00 0000 721f 0000 0072  r....r....r....r
+00000560: 1f00 0000 721f 0000 0072 2000 0000 7214  ....r....r ...r.
+00000570: 0000 0028 0000 0073 0c00 0000 0a00 0801  ...(...s........
+00000580: 0c01 0801 0801 0c01 7214 0000 0063 0000  ........r....c..
+00000590: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+000005a0: 0000 4000 0000 f316 0000 0065 005a 0164  ..@........e.Z.d
+000005b0: 005a 0255 0065 0365 0464 013c 0064 0253  .Z.U.e.e.d.<.d.S
+000005c0: 0029 0372 1200 0000 722a 0000 004e 2905  .).r....r*...N).
+000005d0: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+000005e0: 0a00 0000 721e 0000 0072 1f00 0000 721f  ....r....r....r.
+000005f0: 0000 0072 1f00 0000 7220 0000 0072 1200  ...r....r ...r..
+00000600: 0000 3000 0000 f304 0000 000a 000c 0172  ..0............r
+00000610: 1200 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000620: 0000 0000 0003 0000 0040 0000 0072 2b00  .........@...r+.
+00000630: 0000 2903 7213 0000 0072 2a00 0000 4e29  ..).r....r*...N)
+00000640: 0572 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00000650: 7209 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00000660: 1f00 0000 721f 0000 0072 2000 0000 7213  ....r....r ...r.
+00000670: 0000 0034 0000 0072 2c00 0000 7213 0000  ...4...r,...r...
+00000680: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000690: 0000 0300 0000 4000 0000 731c 0000 0065  ......@...s....e
+000006a0: 005a 0164 005a 0265 0364 0183 0164 0264  .Z.d.Z.e.d...d.d
+000006b0: 0384 0083 015a 0464 0453 0029 0572 1500  .....Z.d.S.).r..
+000006c0: 0000 7217 0000 0063 0200 0000 0000 0000  ..r....c........
+000006d0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+000006e0: 7314 0000 0064 017c 0176 0072 0874 0064  s....d.|.v.r.t.d
+000006f0: 0283 0182 017c 0153 0029 034e da15 7061  .....|.S.).N..pa
+00000700: 7261 6c6c 656c 697a 6174 696f 6e5f 6c65  rallelization_le
+00000710: 7665 6c7a 3b4f 7665 7272 6964 696e 6720  velz;Overriding 
+00000720: 7461 736b 2070 6172 616c 6c65 6c69 7a61  task paralleliza
+00000730: 7469 6f6e 206c 6576 656c 2063 7572 7265  tion level curre
+00000740: 6e74 6c79 206e 6f74 2061 6c6c 6f77 6564  ntly not allowed
+00000750: 2901 da0a 5661 6c75 6545 7272 6f72 2902  )...ValueError).
+00000760: da03 636c 73da 016d 721f 0000 0072 1f00  ..cls..mr....r..
+00000770: 0000 7220 0000 00da 1e63 6865 636b 5f6e  ..r .....check_n
+00000780: 6f5f 7061 7261 6c6c 656c 6973 6174 696f  o_parallelisatio
+00000790: 6e5f 6c65 7665 6c3a 0000 0073 0a00 0000  n_level:...s....
+000007a0: 0802 0201 0201 04ff 0403 7a31 576f 726b  ..........z1Work
+000007b0: 666c 6f77 5461 736b 5570 6461 7465 2e63  flowTaskUpdate.c
+000007c0: 6865 636b 5f6e 6f5f 7061 7261 6c6c 656c  heck_no_parallel
+000007d0: 6973 6174 696f 6e5f 6c65 7665 6c4e 2905  isation_levelN).
+000007e0: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+000007f0: 0500 0000 7231 0000 0072 1f00 0000 721f  ....r1...r....r.
+00000800: 0000 0072 1f00 0000 7220 0000 0072 1500  ...r....r ...r..
+00000810: 0000 3800 0000 7306 0000 0008 0006 020e  ..8...s.........
+00000820: 0172 1500 0000 6300 0000 0000 0000 0000  .r....c.........
+00000830: 0000 0000 0000 0003 0000 0040 0000 0072  ...........@...r
+00000840: 2b00 0000 2903 da0d 5f57 6f72 6b66 6c6f  +...)..._Workflo
+00000850: 7742 6173 65da 046e 616d 654e 2905 7219  wBase..nameN).r.
+00000860: 0000 0072 1a00 0000 721b 0000 0072 1d00  ...r....r....r..
+00000870: 0000 721e 0000 0072 1f00 0000 721f 0000  ..r....r....r...
+00000880: 0072 1f00 0000 7220 0000 0072 3200 0000  .r....r ...r2...
+00000890: 4300 0000 722c 0000 0072 3200 0000 6300  C...r,...r2...c.
+000008a0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+000008b0: 0000 0040 0000 0073 2a00 0000 6500 5a01  ...@...s*...e.Z.
+000008c0: 6400 5a02 5500 6503 6504 6401 3c00 6503  d.Z.U.e.e.d.<.e.
+000008d0: 6504 6402 3c00 6505 6506 1900 6504 6403  e.d.<.e.e...e.d.
+000008e0: 3c00 6404 5300 2905 720d 0000 0072 2700  <.d.S.).r....r'.
+000008f0: 0000 da0a 7072 6f6a 6563 745f 6964 da09  ....project_id..
+00000900: 7461 736b 5f6c 6973 744e 2907 7219 0000  task_listN).r...
+00000910: 0072 1a00 0000 721b 0000 0072 2500 0000  .r....r....r%...
+00000920: 721e 0000 00da 046c 6973 7472 1400 0000  r......listr....
+00000930: 721f 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00000940: 2000 0000 720d 0000 0047 0000 0073 0800   ...r....G...s..
+00000950: 0000 0a00 0801 0801 1001 720d 0000 0063  ..........r....c
+00000960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000970: 0400 0000 4000 0000 7320 0000 0065 005a  ....@...s ...e.Z
+00000980: 0164 005a 0265 0364 0164 0264 038d 0265  .d.Z.e.d.d.d...e
+00000990: 0464 0183 0183 015a 0564 0453 0029 0572  .d.....Z.d.S.).r
+000009a0: 0c00 0000 7233 0000 0054 7222 0000 004e  ....r3...Tr"...N
+000009b0: 2906 7219 0000 0072 1a00 0000 721b 0000  ).r....r....r...
+000009c0: 0072 0500 0000 7208 0000 00da 055f 6e61  .r....r......_na
+000009d0: 6d65 721f 0000 0072 1f00 0000 721f 0000  mer....r....r...
+000009e0: 0072 2000 0000 720c 0000 004d 0000 0073  .r ...r....M...s
+000009f0: 0400 0000 0800 1802 720c 0000 0063 0000  ........r....c..
+00000a00: 0000 0000 0000 0000 0000 0000 0000 0400  ................
+00000a10: 0000 4000 0000 734e 0000 0065 005a 0164  ..@...sN...e.Z.d
+00000a20: 005a 0255 0065 0365 0419 0065 0564 013c  .Z.U.e.e...e.d.<
+00000a30: 0065 0365 0665 0719 0019 0065 0564 023c  .e.e.e.....e.d.<
+00000a40: 0065 0864 0164 0364 048d 0265 0964 0183  .e.d.d.d...e.d..
+00000a50: 0183 015a 0a65 0864 0283 0164 0564 0684  ...Z.e.d...d.d..
+00000a60: 0083 015a 0b64 0753 0029 0872 0e00 0000  ...Z.d.S.).r....
+00000a70: 7233 0000 00da 1a72 656f 7264 6572 6564  r3.....reordered
+00000a80: 5f77 6f72 6b66 6c6f 7774 6173 6b5f 6964  _workflowtask_id
+00000a90: 7354 7222 0000 0063 0200 0000 0000 0000  sTr"...c........
+00000aa0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00000ab0: 733a 0000 0074 0064 0164 0284 007c 0144  s:...t.d.d...|.D
+00000ac0: 0083 0183 0172 0d74 0164 0383 0182 0174  .....r.t.d.....t
+00000ad0: 027c 0183 0174 0274 037c 0183 0183 016b  .|...t.t.|.....k
+00000ae0: 0372 1b74 0164 0483 0182 017c 0153 0029  .r.t.d.....|.S.)
+00000af0: 054e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
+00000b00: 0000 0003 0000 0073 0000 0073 1800 0000  .......s...s....
+00000b10: 8100 7c00 5d07 7d01 7c01 6400 6b00 5600  ..|.].}.|.d.k.V.
+00000b20: 0100 7102 6401 5300 2902 7201 0000 004e  ..q.d.S.).r....N
+00000b30: 721f 0000 0029 02da 022e 30da 0169 721f  r....)....0..ir.
+00000b40: 0000 0072 1f00 0000 7220 0000 00da 093c  ...r....r .....<
+00000b50: 6765 6e65 7870 723e 5b00 0000 7304 0000  genexpr>[...s...
+00000b60: 0002 8016 007a 3b57 6f72 6b66 6c6f 7755  .....z;WorkflowU
+00000b70: 7064 6174 652e 6368 6563 6b5f 706f 7369  pdate.check_posi
+00000b80: 7469 7665 5f61 6e64 5f75 6e69 7175 652e  tive_and_unique.
+00000b90: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00000ba0: 723e 7a2d 4e65 6761 7469 7665 2060 6964  r>z-Negative `id
+00000bb0: 6020 696e 2060 7265 6f72 6465 7265 645f  ` in `reordered_
+00000bc0: 776f 726b 666c 6f77 7461 736b 5f69 6473  workflowtask_ids
+00000bd0: 607a 2c60 7265 6f72 6465 7265 645f 776f  `z,`reordered_wo
+00000be0: 726b 666c 6f77 7461 736b 5f69 6473 6020  rkflowtask_ids` 
+00000bf0: 6861 7320 7265 7065 7469 7469 6f6e 7329  has repetitions)
+00000c00: 04da 0361 6e79 722e 0000 00da 036c 656e  ...anyr......len
+00000c10: da03 7365 7429 0272 2f00 0000 da05 7661  ..set).r/.....va
+00000c20: 6c75 6572 1f00 0000 721f 0000 0072 2000  luer....r....r .
+00000c30: 0000 da19 6368 6563 6b5f 706f 7369 7469  ....check_positi
+00000c40: 7665 5f61 6e64 5f75 6e69 7175 6559 0000  ve_and_uniqueY..
+00000c50: 0073 0a00 0000 1202 0801 1401 0801 0401  .s..............
+00000c60: 7a28 576f 726b 666c 6f77 5570 6461 7465  z(WorkflowUpdate
+00000c70: 2e63 6865 636b 5f70 6f73 6974 6976 655f  .check_positive_
+00000c80: 616e 645f 756e 6971 7565 4e29 0c72 1900  and_uniqueN).r..
+00000c90: 0000 721a 0000 0072 1b00 0000 7203 0000  ..r....r....r...
+00000ca0: 0072 1d00 0000 721e 0000 0072 3600 0000  .r....r....r6...
+00000cb0: 7225 0000 0072 0500 0000 7208 0000 0072  r%...r....r....r
+00000cc0: 3700 0000 7240 0000 0072 1f00 0000 721f  7...r@...r....r.
+00000cd0: 0000 0072 1f00 0000 7220 0000 0072 0e00  ...r....r ...r..
+00000ce0: 0000 5200 0000 730c 0000 000a 000c 0110  ..R...s.........
+00000cf0: 0114 0306 020e 0172 0e00 0000 6300 0000  .......r....c...
+00000d00: 0000 0000 0000 0000 0000 0000 0004 0000  ................
+00000d10: 0040 0000 0073 2e00 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000d20: 5a02 5500 6503 6504 1900 6505 6401 3c00  Z.U.e.e...e.d.<.
+00000d30: 6506 6402 6403 6404 8d02 6507 6402 8301  e.d.d.d...e.d...
+00000d40: 8301 5a08 6405 5300 2906 720f 0000 0072  ..Z.d.S.).r....r
+00000d50: 3500 0000 7233 0000 0054 7222 0000 004e  5...r3...Tr"...N
+00000d60: 2909 7219 0000 0072 1a00 0000 721b 0000  ).r....r....r...
+00000d70: 0072 3600 0000 7212 0000 0072 1e00 0000  .r6...r....r....
+00000d80: 7205 0000 0072 0800 0000 7237 0000 0072  r....r....r7...r
+00000d90: 1f00 0000 721f 0000 0072 1f00 0000 7220  ....r....r....r 
+00000da0: 0000 0072 0f00 0000 6200 0000 7306 0000  ...r....b...s...
+00000db0: 000a 000c 0118 0372 0f00 0000 6300 0000  .......r....c...
+00000dc0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000dd0: 0040 0000 0073 1a00 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000de0: 5a02 5500 6503 6504 1900 6505 6401 3c00  Z.U.e.e...e.d.<.
+00000df0: 6402 5300 2903 7210 0000 0072 3500 0000  d.S.).r....r5...
+00000e00: 4e29 0672 1900 0000 721a 0000 0072 1b00  N).r....r....r..
+00000e10: 0000 7236 0000 0072 1300 0000 721e 0000  ..r6...r....r...
+00000e20: 0072 1f00 0000 721f 0000 0072 1f00 0000  .r....r....r....
+00000e30: 7220 0000 0072 1000 0000 6900 0000 7304  r ...r....i...s.
+00000e40: 0000 000a 0010 0172 1000 0000 4e29 1ada  .......r....N)..
+00000e50: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
+00000e60: 00da 0870 7964 616e 7469 6372 0400 0000  ...pydanticr....
+00000e70: 7205 0000 00da 0b5f 7661 6c69 6461 746f  r......_validato
+00000e80: 7273 7207 0000 0072 0800 0000 722a 0000  rsr....r....r*..
+00000e90: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000ea0: da07 5f5f 616c 6c5f 5f72 1600 0000 7211  ..__all__r....r.
+00000eb0: 0000 0072 1400 0000 7212 0000 0072 1300  ...r....r....r..
+00000ec0: 0000 7215 0000 0072 3200 0000 720d 0000  ..r....r2...r...
+00000ed0: 0072 0c00 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00000ee0: 7210 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00000ef0: 1f00 0000 7220 0000 00da 083c 6d6f 6475  ....r .....<modu
+00000f00: 6c65 3e01 0000 0073 2c00 0000 0c00 0c01  le>....s,.......
+00000f10: 0c02 0c01 0c02 0c01 0c01 0c01 0c01 0403  ................
+00000f20: 100e 1006 1006 1008 1004 1004 100b 1004  ................
+00000f30: 1006 1005 1010 1407                      ........
```

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc` & `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/_validators.py` & `fractal_server-1.3.0a3/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.3.0a3/fractal_server/common/schemas/applyworkflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,52 @@
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
     end_timestamp: Optional[datetime]
     status: str
     log: Optional[str]
-    history: Optional[List[str]]
+    history: Optional[list[str]]
     working_dir: Optional[str]
     working_dir_user: Optional[str]
 
     def sanitised_dict(self):
         d = self.dict()
         d["start_timestamp"] = str(self.start_timestamp)
         d["end_timestamp"] = str(self.end_timestamp)
```

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/project.py` & `fractal_server-1.3.0a3/fractal_server/common/schemas/project.py`

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

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/state.py` & `fractal_server-1.3.0a3/fractal_server/common/schemas/state.py`

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

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/user.py` & `fractal_server-1.3.0a3/fractal_server/common/schemas/user.py`

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

### Comparing `fractal_server-1.3.0a2/fractal_server/common/schemas/workflow.py` & `fractal_server-1.3.0a3/fractal_server/common/schemas/workflow.py`

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

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  8 12:01:46 2023 UTC, .py size: 748 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-00000000: 6f0d 0d0a 0000 0000 aae4 5864 ec02 0000  o.........Xd....
+00000000: 6f0d 0d0a 0000 0000 b554 7064 a604 0000  o........Tpd....
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
@@ -43,98 +43,134 @@
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
-00000630: 726d 6174 3139 a900 722a 0000 00fa 4d2f  rmat19..r*....M/
-00000640: 686f 6d65 2f74 6f6d 6d61 736f 2f46 7261  home/tommaso/Fra
-00000650: 6374 616c 2f66 7261 6374 616c 2d73 6572  ctal/fractal-ser
-00000660: 7665 722f 6672 6163 7461 6c5f 7365 7276  ver/fractal_serv
-00000670: 6572 2f63 6f6d 6d6f 6e2f 7465 7374 732f  er/common/tests/
-00000680: 7465 7374 5f74 6173 6b2e 7079 da10 7465  test_task.py..te
-00000690: 7374 5f74 6173 6b5f 7570 6461 7465 0900  st_task_update..
-000006a0: 0000 730c 0000 000a 0208 01fe 010e 00fe  ..s.............
-000006b0: 0114 0072 2c00 0000 6300 0000 0000 0000  ...r,...c.......
-000006c0: 0000 0000 0001 0000 0008 0000 0043 0000  .............C..
-000006d0: 0073 5600 0000 7400 6401 6402 6403 6404  .sV...t.d.d.d.d.
-000006e0: 6405 6406 8d05 7d00 7401 7c00 8301 0100  d.d...}.t.|.....
-000006f0: 7402 a003 7404 a101 8f0f 0100 7400 6401  t...t.......t.d.
-00000700: 6402 6407 8d02 0100 5700 6400 0400 0400  d.d.....W.d.....
-00000710: 8303 0100 6400 5300 3100 7324 7701 0100  ....d.S.1.s$w...
-00000720: 0100 0100 5900 0100 6400 5300 2908 4eda  ....Y...d.S.).N.
-00000730: 0474 6173 6bda 0673 6f75 7263 65da 0763  .task..source..c
-00000740: 6f6d 6d61 6e64 da0a 696e 7075 745f 7479  ommand..input_ty
-00000750: 7065 da0b 6f75 7470 7574 5f74 7970 6529  pe..output_type)
-00000760: 0572 0600 0000 722e 0000 0072 2f00 0000  .r....r....r/...
-00000770: 7230 0000 0072 3100 0000 2902 7206 0000  r0...r1...).r...
-00000780: 0072 2e00 0000 2905 7204 0000 0072 0200  .r....).r....r..
-00000790: 0000 da06 7079 7465 7374 da06 7261 6973  ....pytest..rais
-000007a0: 6573 7203 0000 0029 0172 0a00 0000 722a  esr....).r....r*
-000007b0: 0000 0072 2a00 0000 722b 0000 00da 1074  ...r*...r+.....t
-000007c0: 6573 745f 7461 736b 5f63 7265 6174 6511  est_task_create.
-000007d0: 0000 0073 1600 0000 0202 0201 0201 0201  ...s............
-000007e0: 0201 0201 06fb 0807 0c02 0e01 22ff 7234  ............".r4
-000007f0: 0000 0029 10da 0862 7569 6c74 696e 7372  ...)...builtinsr
-00000800: 1a00 0000 da19 5f70 7974 6573 742e 6173  ......_pytest.as
-00000810: 7365 7274 696f 6e2e 7265 7772 6974 65da  sertion.rewrite.
-00000820: 0961 7373 6572 7469 6f6e da07 7265 7772  .assertion..rewr
-00000830: 6974 6572 1800 0000 7232 0000 00da 0864  iter....r2.....d
-00000840: 6576 746f 6f6c 7372 0200 0000 da17 7079  evtoolsr......py
-00000850: 6461 6e74 6963 2e65 7272 6f72 5f77 7261  dantic.error_wra
-00000860: 7070 6572 7372 0300 0000 da07 7363 6865  ppersr......sche
-00000870: 6d61 7372 0400 0000 7205 0000 0072 2c00  masr....r....r,.
-00000880: 0000 7234 0000 0072 2a00 0000 722a 0000  ..r4...r*...r*..
-00000890: 0072 2a00 0000 722b 0000 00da 083c 6d6f  .r*...r+.....<mo
-000008a0: 6475 6c65 3e01 0000 0073 0e00 0000 2200  dule>....s....".
-000008b0: 0c01 0c01 0c02 0c01 0803 0c08            ............
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
+00000840: 0072 3500 0000 fa4d 2f68 6f6d 652f 746f  .r5....M/home/to
+00000850: 6d6d 6173 6f2f 4672 6163 7461 6c2f 6672  mmaso/Fractal/fr
+00000860: 6163 7461 6c2d 7365 7276 6572 2f66 7261  actal-server/fra
+00000870: 6374 616c 5f73 6572 7665 722f 636f 6d6d  ctal_server/comm
+00000880: 6f6e 2f74 6573 7473 2f74 6573 745f 7461  on/tests/test_ta
+00000890: 736b 2e70 79da 1074 6573 745f 7461 736b  sk.py..test_task
+000008a0: 5f75 7064 6174 6509 0000 0073 2800 0000  _update....s(...
+000008b0: 0a02 0801 fe01 0e00 fe01 1000 0c02 0e01  ................
+000008c0: 1eff 0c02 0e01 1eff 0203 0201 0201 0201  ................
+000008d0: 06fd 0805 5601 5a01 7237 0000 0063 0000  ....V.Z.r7...c..
+000008e0: 0000 0000 0000 0000 0000 0100 0000 0900  ................
+000008f0: 0000 4300 0000 735a 0000 0074 0064 0164  ..C...sZ...t.d.d
+00000900: 0264 0364 0464 0564 0664 0764 088d 077d  .d.d.d.d.d.d...}
+00000910: 0074 017c 0083 0101 0074 02a0 0374 04a1  .t.|.....t...t..
+00000920: 018f 0f01 0074 0064 0164 0264 098d 0201  .....t.d.d.d....
+00000930: 0057 0064 0004 0004 0083 0301 0064 0053  .W.d.........d.S
+00000940: 0031 0073 2677 0101 0001 0001 0059 0001  .1.s&w.......Y..
+00000950: 0064 0053 0029 0a4e 7216 0000 00da 0673  .d.S.).Nr......s
+00000960: 6f75 7263 65da 0763 6f6d 6d61 6e64 da0a  ource..command..
+00000970: 696e 7075 745f 7479 7065 da0b 6f75 7470  input_type..outp
+00000980: 7574 5f74 7970 6572 1900 0000 721a 0000  ut_typer....r...
+00000990: 0029 0772 0600 0000 7238 0000 0072 3900  .).r....r8...r9.
+000009a0: 0000 723a 0000 0072 3b00 0000 7218 0000  ..r:...r;...r...
+000009b0: 0072 1b00 0000 2902 7206 0000 0072 3800  .r....).r....r8.
+000009c0: 0000 2905 7204 0000 0072 0200 0000 7227  ..).r....r....r'
+000009d0: 0000 0072 2800 0000 7203 0000 0029 0172  ...r(...r....).r
+000009e0: 0a00 0000 7235 0000 0072 3500 0000 7236  ....r5...r5...r6
+000009f0: 0000 00da 1074 6573 745f 7461 736b 5f63  .....test_task_c
+00000a00: 7265 6174 651f 0000 0073 1a00 0000 0202  reate....s......
+00000a10: 0201 0201 0201 0201 0201 0201 0201 06f9  ................
+00000a20: 0809 0c02 0e01 22ff 723c 0000 0029 10da  ......".r<...)..
+00000a30: 0862 7569 6c74 696e 7372 2100 0000 da19  .builtinsr!.....
+00000a40: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
+00000a50: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
+00000a60: 7469 6f6e da07 7265 7772 6974 6572 1f00  tion..rewriter..
+00000a70: 0000 7227 0000 00da 0864 6576 746f 6f6c  ..r'.....devtool
+00000a80: 7372 0200 0000 da17 7079 6461 6e74 6963  sr......pydantic
+00000a90: 2e65 7272 6f72 5f77 7261 7070 6572 7372  .error_wrappersr
+00000aa0: 0300 0000 da07 7363 6865 6d61 7372 0400  ......schemasr..
+00000ab0: 0000 7205 0000 0072 3700 0000 723c 0000  ..r....r7...r<..
+00000ac0: 0072 3500 0000 7235 0000 0072 3500 0000  .r5...r5...r5...
+00000ad0: 7236 0000 00da 083c 6d6f 6475 6c65 3e01  r6.....<module>.
+00000ae0: 0000 0073 0e00 0000 2200 0c01 0c01 0c02  ...s....".......
+00000af0: 0c01 0803 0c16                           ......
```

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  8 12:01:46 2023 UTC, .py size: 1224 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-00000000: 6f0d 0d0a 0000 0000 aae4 5864 c804 0000  o.........Xd....
+00000000: 6f0d 0d0a 0000 0000 b554 7064 db05 0000  o........Tpd....
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
@@ -61,80 +61,108 @@
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
-00000750: 7373 6572 7432 a900 722f 0000 00fa 4d2f  ssert2..r/....M/
-00000760: 686f 6d65 2f74 6f6d 6d61 736f 2f46 7261  home/tommaso/Fra
-00000770: 6374 616c 2f66 7261 6374 616c 2d73 6572  ctal/fractal-ser
-00000780: 7665 722f 6672 6163 7461 6c5f 7365 7276  ver/fractal_serv
-00000790: 6572 2f63 6f6d 6d6f 6e2f 7465 7374 732f  er/common/tests/
-000007a0: 7465 7374 5f75 7365 722e 7079 da10 7465  test_user.py..te
-000007b0: 7374 5f75 7365 725f 6372 6561 7465 0800  st_user_create..
-000007c0: 0000 732c 0000 000c 0208 018a 010e 0208  ..s,............
-000007d0: 0150 010c 0210 011c ff04 0314 019c 010c  .P..............
-000007e0: 0210 011e ff0a 0276 010c 0210 011e ff0a  .......v........
-000007f0: 027a 0172 3100 0000 290e da08 6275 696c  .z.r1...)...buil
-00000800: 7469 6e73 721a 0000 00da 195f 7079 7465  tinsr......_pyte
-00000810: 7374 2e61 7373 6572 7469 6f6e 2e72 6577  st.assertion.rew
-00000820: 7269 7465 da09 6173 7365 7274 696f 6eda  rite..assertion.
-00000830: 0772 6577 7269 7465 7218 0000 0072 2000  .rewriter....r .
-00000840: 0000 da08 6465 7674 6f6f 6c73 7202 0000  ....devtoolsr...
-00000850: 00da 1770 7964 616e 7469 632e 6572 726f  ...pydantic.erro
-00000860: 725f 7772 6170 7065 7273 7203 0000 00da  r_wrappersr.....
-00000870: 0773 6368 656d 6173 7204 0000 0072 3100  .schemasr....r1.
-00000880: 0000 722f 0000 0072 2f00 0000 722f 0000  ..r/...r/...r/..
-00000890: 0072 3000 0000 da08 3c6d 6f64 756c 653e  .r0.....<module>
-000008a0: 0100 0000 730a 0000 0022 000c 010c 010c  ....s...."......
-000008b0: 020c 03                                  ...
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
+00000910: 00fa 4d2f 686f 6d65 2f74 6f6d 6d61 736f  ..M/home/tommaso
+00000920: 2f46 7261 6374 616c 2f66 7261 6374 616c  /Fractal/fractal
+00000930: 2d73 6572 7665 722f 6672 6163 7461 6c5f  -server/fractal_
+00000940: 7365 7276 6572 2f63 6f6d 6d6f 6e2f 7465  server/common/te
+00000950: 7374 732f 7465 7374 5f75 7365 722e 7079  sts/test_user.py
+00000960: da10 7465 7374 5f75 7365 725f 6372 6561  ..test_user_crea
+00000970: 7465 0800 0000 7342 0000 000c 0208 018a  te....sB........
+00000980: 010e 0208 0150 010c 0210 011c ff04 0314  .....P..........
+00000990: 019c 010c 0210 011e ff0a 0276 010c 0210  ...........v....
+000009a0: 011e ff0a 0276 0102 0202 0102 0102 0102  .....v..........
+000009b0: 0102 0106 fb08 0756 0156 015a 0172 3300  .......V.V.Z.r3.
+000009c0: 0000 290e da08 6275 696c 7469 6e73 721c  ..)...builtinsr.
+000009d0: 0000 00da 195f 7079 7465 7374 2e61 7373  ....._pytest.ass
+000009e0: 6572 7469 6f6e 2e72 6577 7269 7465 da09  ertion.rewrite..
+000009f0: 6173 7365 7274 696f 6eda 0772 6577 7269  assertion..rewri
+00000a00: 7465 721a 0000 0072 2200 0000 da08 6465  ter....r".....de
+00000a10: 7674 6f6f 6c73 7202 0000 00da 1770 7964  vtoolsr......pyd
+00000a20: 616e 7469 632e 6572 726f 725f 7772 6170  antic.error_wrap
+00000a30: 7065 7273 7203 0000 00da 0773 6368 656d  persr......schem
+00000a40: 6173 7204 0000 0072 3300 0000 7231 0000  asr....r3...r1..
+00000a50: 0072 3100 0000 7231 0000 0072 3200 0000  .r1...r1...r2...
+00000a60: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+00000a70: 0000 0022 000c 010c 010c 020c 03         ...".........
```

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.3.0a3/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/test_project.py` & `fractal_server-1.3.0a3/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/test_state.py` & `fractal_server-1.3.0a3/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/test_user.py` & `fractal_server-1.3.0a3/fractal_server/common/tests/test_user.py`

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

### Comparing `fractal_server-1.3.0a2/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.3.0a3/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/config.py` & `fractal_server-1.3.0a3/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/logger.py` & `fractal_server-1.3.0a3/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/main.py` & `fractal_server-1.3.0a3/fractal_server/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 
 async def _create_first_user(
     email: str,
     password: str,
     is_superuser: bool = False,
     slurm_user: Optional[str] = None,
     cache_dir: Optional[str] = None,
+    username: Optional[str] = None,
 ) -> None:
     """
     Private method to create the first fractal-server user
 
     Create a user with the given default arguments and return a message with
     the relevant informations. If the user alredy exists, for example after a
     restart, it returns a message to inform that user already exists.
@@ -117,14 +118,16 @@
                         password=password,
                         is_superuser=is_superuser,
                     )
                     if slurm_user:
                         kwargs["slurm_user"] = slurm_user
                     if cache_dir:
                         kwargs["cache_dir"] = cache_dir
+                    if username:
+                        kwargs["username"] = username
                     user = await user_manager.create(UserCreate(**kwargs))
                     logger.info(f"User {user.email} created")
 
     except IntegrityError:
         logger.warning(
             f"Creation of user {email} failed with IntegrityError "
             "(likely due to concurrent attempts from different workers)."
```

### Comparing `fractal_server-1.3.0a2/fractal_server/migrations/env.py` & `fractal_server-1.3.0a3/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/migrations/script.py.mako` & `fractal_server-1.3.0a3/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/migrations/versions/e8f4051440be_new_initial_schema.py` & `fractal_server-1.3.0a3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""New initial schema
+"""Initial schema
 
-Revision ID: e8f4051440be
+Revision ID: 50a13d6138fd
 Revises:
-Create Date: 2023-05-08 09:23:14.013706
+Create Date: 2023-05-29 12:14:56.670243
 
 """
 import sqlalchemy as sa
 import sqlmodel
 from alembic import op
 
 
 # revision identifiers, used by Alembic.
-revision = "e8f4051440be"
+revision = "50a13d6138fd"
 down_revision = None
 branch_labels = None
 depends_on = None
 
 
 def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
@@ -33,29 +33,34 @@
         sa.Column("id", sa.Integer(), nullable=False),
         sa.PrimaryKeyConstraint("id"),
     )
     op.create_table(
         "task",
         sa.Column("default_args", sa.JSON(), nullable=True),
         sa.Column("meta", sa.JSON(), nullable=True),
-        sa.Column("name", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
         sa.Column(
             "source", sqlmodel.sql.sqltypes.AutoString(), nullable=False
         ),
         sa.Column("id", sa.Integer(), nullable=False),
+        sa.Column("name", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
         sa.Column(
             "command", sqlmodel.sql.sqltypes.AutoString(), nullable=False
         ),
         sa.Column(
             "input_type", sqlmodel.sql.sqltypes.AutoString(), nullable=False
         ),
         sa.Column(
             "output_type", sqlmodel.sql.sqltypes.AutoString(), nullable=False
         ),
+        sa.Column("owner", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
+        sa.Column(
+            "version", sqlmodel.sql.sqltypes.AutoString(), nullable=True
+        ),
         sa.PrimaryKeyConstraint("id"),
+        sa.UniqueConstraint("source"),
     )
     op.create_table(
         "user_oauth",
         sa.Column("id", sa.Integer(), nullable=False),
         sa.Column("email", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
         sa.Column(
             "hashed_password",
@@ -67,14 +72,17 @@
         sa.Column("is_verified", sa.Boolean(), nullable=False),
         sa.Column(
             "slurm_user", sqlmodel.sql.sqltypes.AutoString(), nullable=True
         ),
         sa.Column(
             "cache_dir", sqlmodel.sql.sqltypes.AutoString(), nullable=True
         ),
+        sa.Column(
+            "username", sqlmodel.sql.sqltypes.AutoString(), nullable=True
+        ),
         sa.PrimaryKeyConstraint("id"),
     )
     op.create_index(
         op.f("ix_user_oauth_email"), "user_oauth", ["email"], unique=True
     )
     op.create_table(
         "dataset",
@@ -154,23 +162,23 @@
         sa.PrimaryKeyConstraint("id"),
     )
     op.create_table(
         "applyworkflow",
         sa.Column(
             "start_timestamp", sa.DateTime(timezone=True), nullable=True
         ),
-        sa.Column("project_id", sa.Integer(), nullable=False),
-        sa.Column("input_dataset_id", sa.Integer(), nullable=False),
-        sa.Column("output_dataset_id", sa.Integer(), nullable=False),
-        sa.Column("workflow_id", sa.Integer(), nullable=False),
-        sa.Column("overwrite_input", sa.Boolean(), nullable=False),
+        sa.Column("end_timestamp", sa.DateTime(timezone=True), nullable=True),
         sa.Column(
             "worker_init", sqlmodel.sql.sqltypes.AutoString(), nullable=True
         ),
         sa.Column("id", sa.Integer(), nullable=False),
+        sa.Column("project_id", sa.Integer(), nullable=False),
+        sa.Column("input_dataset_id", sa.Integer(), nullable=False),
+        sa.Column("output_dataset_id", sa.Integer(), nullable=False),
+        sa.Column("workflow_id", sa.Integer(), nullable=False),
         sa.Column(
             "working_dir", sqlmodel.sql.sqltypes.AutoString(), nullable=True
         ),
         sa.Column(
             "working_dir_user",
             sqlmodel.sql.sqltypes.AutoString(),
             nullable=True,
```

### Comparing `fractal_server-1.3.0a2/fractal_server/migrations/versions/fda995215ae9_drop_applyworkflow_overwrite_input.py` & `fractal_server-1.3.0a3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,38 @@
-"""Drop ApplyWorkflow.overwrite_input
+"""Add task.args_schema and task.args_schema_version
 
-Revision ID: fda995215ae9
-Revises: e8f4051440be
-Create Date: 2023-05-11 17:02:46.208476
+Revision ID: 4c308bcaea2b
+Revises: 50a13d6138fd
+Create Date: 2023-05-29 17:09:02.492639
 
 """
 import sqlalchemy as sa
+import sqlmodel
 from alembic import op
 
 
 # revision identifiers, used by Alembic.
-revision = "fda995215ae9"
-down_revision = "e8f4051440be"
+revision = "4c308bcaea2b"
+down_revision = "50a13d6138fd"
 branch_labels = None
 depends_on = None
 
 
 def upgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
-    op.drop_column("applyworkflow", "overwrite_input")
+    op.add_column("task", sa.Column("args_schema", sa.JSON(), nullable=True))
+    op.add_column(
+        "task",
+        sa.Column(
+            "args_schema_version",
+            sqlmodel.sql.sqltypes.AutoString(),
+            nullable=True,
+        ),
+    )
     # ### end Alembic commands ###
 
 
 def downgrade() -> None:
     # ### commands auto generated by Alembic - please adjust! ###
-    op.add_column(
-        "applyworkflow",
-        sa.Column("overwrite_input", sa.BOOLEAN(), nullable=False),
-    )
+    op.drop_column("task", "args_schema_version")
+    op.drop_column("task", "args_schema")
     # ### end Alembic commands ###
```

### Comparing `fractal_server-1.3.0a2/fractal_server/syringe.py` & `fractal_server-1.3.0a3/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/fractal_server/tasks/collection.py` & `fractal_server-1.3.0a3/fractal_server/tasks/collection.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,22 +7,20 @@
 # This file is part of Fractal and was originally developed by eXact lab S.r.l.
 # <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
 # Institute for Biomedical Research and Pelkmans Lab from the University of
 # Zurich.
 """
 This module takes care of installing tasks so that fractal can execute them
 
-Tasks can be private or public. Private tasks are installed under
-`Settings.FRACTAL_TASKS_DIR/{username}`. For public tasks, `username =
-.fractal`.
+Tasks are installed under `Settings.FRACTAL_TASKS_DIR/{username}`, with
+`username = ".fractal"`.
 """
 import json
 import shutil
 import sys
-from io import IOBase
 from pathlib import Path
 from typing import Optional
 from typing import Union
 from zipfile import ZipFile
 
 from pydantic import root_validator
 
@@ -106,19 +104,27 @@
     return TaskCollectStatus(**data)
 
 
 class _TaskCollectPip(TaskCollectPip):
     """
     Internal TaskCollectPip schema
 
-    The difference with its parent class is that we check if the package
-    corresponds to a path in the filesystem, and whether it exists.
+    Differences with its parent class (`TaskCollectPip`):
+
+        1. We check if the package corresponds to a path in the filesystem, and
+           whether it exists (via new validator `check_local_package`, new
+           method `is_local_package` and new attribute `package_path`).
+        2. We include an additional `package_manifest` attribute.
+        3. We expose an additional attribute `package_name`, which is filled
+           during task collection.
     """
 
+    package_name: Optional[str] = None
     package_path: Optional[Path] = None
+    package_manifest: Optional[ManifestV1] = None
 
     @property
     def is_local_package(self) -> bool:
         return bool(self.package_path)
 
     @root_validator(pre=True)
     def check_local_package(cls, values):
@@ -141,55 +147,72 @@
                     *_,
                 ) = package_path.name.split("-")
             else:
                 raise ValueError(f"Package {package_path} does not exist.")
         return values
 
     @property
-    def pip_package_version(self):
-        """
-        Return pip compatible specification of package and version
-        """
-        version = f"=={self.version}" if self.version else ""
-        return f"{self.package}{version}"
-
-    @property
-    def source(self):
+    def package_source(self):
+        if not self.package_name or not self.package_version:
+            raise ValueError(
+                "Cannot construct `package_source` property with "
+                f"{self.package_name=} and {self.package_version=}."
+            )
         if self.is_local_package:
-            return f"pip-local:{self.package_path.name}"
+            collection_type = "pip_local"
         else:
-            return f"pip:{self.pip_package_version}"
+            collection_type = "pip_remote"
 
-    def check(self):
-        if not self.version:
-            raise ValueError("Version is not set or cannot be determined")
+        package_extras = self.package_extras or ""
+        if self.python_version:
+            python_version = f"py{self.python_version}"
+        else:
+            python_version = ""  # FIXME: can we allow this?
 
+        source = ":".join(
+            (
+                collection_type,
+                self.package_name,
+                self.package_version,
+                package_extras,
+                python_version,
+            )
+        )
+        return source
 
-def _package_from_path(wheel_path: Path) -> tuple[str, str]:
-    """
-    Extract package name and version from package files such as wheel files.
-    """
-    wheel_filename = wheel_path.name
-    package, version, *_rest = wheel_filename.split("-")
-    return package, version
+    def check(self):
+        """
+        Verify that the package has all attributes that are needed to continue
+        with task collection
+        """
+        if not self.package_name:
+            raise ValueError("`package_name` attribute is not set")
+        if not self.package_version:
+            raise ValueError("`package_version` attribute is not set")
+        if not self.package_manifest:
+            raise ValueError("`package_manifest` attribute is not set")
 
 
 def create_package_dir_pip(
     *,
     task_pkg: _TaskCollectPip,
-    user: Optional[str] = None,
     create: bool = True,
-    **_,  # FIXME remove this catch-all argument
 ) -> Path:
+    """
+    Create venv folder for a task package and return corresponding Path object
+    """
     settings = Inject(get_settings)
-    user = user or FRACTAL_PUBLIC_TASK_SUBDIR
-
-    package_dir = f"{task_pkg.package}{task_pkg.version or ''}"
+    user = FRACTAL_PUBLIC_TASK_SUBDIR
+    if task_pkg.package_version is None:
+        raise ValueError(
+            f"Cannot create venv folder for package `{task_pkg.package}` "
+            "with `version=None`."
+        )
+    package_dir = f"{task_pkg.package}{task_pkg.package_version}"
     venv_path = settings.FRACTAL_TASKS_DIR / user / package_dir  # type: ignore
-    # TODO check the access right of the venv_path and subdirs
     if create:
         venv_path.mkdir(exist_ok=False, parents=True)
     return venv_path
 
 
 async def download_package(
     *,
@@ -197,141 +220,181 @@
     dest: Union[str, Path],
 ):
     """
     Download package to destination
     """
     interpreter = get_python_interpreter(version=task_pkg.python_version)
     pip = f"{interpreter} -m pip"
-    cmd = (
-        f"{pip} download --no-deps {task_pkg.pip_package_version} "
-        f"-d {dest}"
+    version = (
+        f"=={task_pkg.package_version}" if task_pkg.package_version else ""
     )
+    package_and_version = f"{task_pkg.package}{version}"
+    cmd = f"{pip} download --no-deps {package_and_version} -d {dest}"
     stdout = await execute_command(command=cmd, cwd=Path("."))
     pkg_file = next(
         line.split()[-1] for line in stdout.split("\n") if "Saved" in line
     )
     return Path(pkg_file)
 
 
-def inspect_package(path: Path) -> dict:
+def _load_manifest_from_wheel(
+    path: Path, wheel: ZipFile, logger_name: Optional[str] = None
+) -> ManifestV1:
+    logger = get_logger(logger_name)
+    namelist = wheel.namelist()
+    try:
+        manifest = next(
+            name for name in namelist if "__FRACTAL_MANIFEST__.json" in name
+        )
+    except StopIteration:
+        msg = f"{path.as_posix()} does not include __FRACTAL_MANIFEST__.json"
+        logger.error(msg)
+        raise ValueError(msg)
+    with wheel.open(manifest) as manifest_fd:
+        manifest_dict = json.load(manifest_fd)
+    manifest_version = str(manifest_dict["manifest_version"])
+    if manifest_version == "1":
+        pkg_manifest = ManifestV1(**manifest_dict)
+        return pkg_manifest
+    else:
+        msg = f"Manifest version {manifest_version=} not supported"
+        logger.error(msg)
+        raise ValueError(msg)
+
+
+def inspect_package(path: Path, logger_name: Optional[str] = None) -> dict:
     """
-    Inspect task package for version and manifest
+    Inspect task package to extract version, name and manifest
+
+    Note that this only works with wheel files, which have a well-defined
+    dist-info section. If we need to generalize to to tar.gz archives, we would
+    need to go and look for `PKG-INFO`.
+
+    Note: package name is normalized by replacing `{-,.}` with `_`.
 
     Args:
         path: Path
             the path in which the package is saved
 
     Returns:
         version_manifest: A dictionary containing `version`, the version of the
         pacakge, and `manifest`, the Fractal manifest object relative to the
         tasks.
     """
-    if "whl" in path.as_posix():
-        # it is simply a zip file
-        # we can extract the version number from *.dist-info/METADATA
-        # and read the fractal manifest from the package content
-        with ZipFile(path) as wheel:
-            namelist = wheel.namelist()
-            metadata = next(
-                name for name in namelist if "dist-info/METADATA" in name
+
+    logger = get_logger(logger_name)
+
+    if not path.as_posix().endswith(".whl"):
+        raise ValueError(
+            f"Only wheel packages are supported, given {path.as_posix()}."
+        )
+
+    with ZipFile(path) as wheel:
+        namelist = wheel.namelist()
+
+        # Read and validate task manifest
+        logger.debug(f"Now reading manifest for {path.as_posix()}")
+        pkg_manifest = _load_manifest_from_wheel(
+            path, wheel, logger_name=logger_name
+        )
+        logger.debug("Manifest read correctly.")
+
+        # Read package name and version from *.dist-info/METADATA
+        logger.debug(
+            f"Now reading package name and version for {path.as_posix()}"
+        )
+        metadata = next(
+            name for name in namelist if "dist-info/METADATA" in name
+        )
+        with wheel.open(metadata) as metadata_fd:
+            meta = metadata_fd.read().decode("utf-8")
+            pkg_name = next(
+                line.split()[-1]
+                for line in meta.splitlines()
+                if line.startswith("Name")
             )
-            manifest = next(
-                name for name in namelist if "__FRACTAL_MANIFEST__" in name
+            pkg_version = next(
+                line.split()[-1]
+                for line in meta.splitlines()
+                if line.startswith("Version")
             )
+        logger.debug("Package name and version read correctly.")
 
-            with wheel.open(metadata) as metadata_fd:
-                meta = metadata_fd.read().decode("utf-8")
-                version = next(
-                    line.split()[-1]
-                    for line in meta.splitlines()
-                    if line.startswith("Version")
-                )
+    # Normalize package name:
+    pkg_name = pkg_name.replace("-", "_").replace(".", "_")
 
-            with wheel.open(manifest) as manifest_fd:
-                manifest_obj = read_manifest(manifest_fd)  # type: ignore
-
-    version_manifest = dict(version=version, manifest=manifest_obj)
-    return version_manifest
+    info = dict(
+        pkg_name=pkg_name,
+        pkg_version=pkg_version,
+        pkg_manifest=pkg_manifest,
+    )
+    return info
 
 
 async def create_package_environment_pip(
     *,
     task_pkg: _TaskCollectPip,
     venv_path: Path,
     logger_name: str,
 ) -> list[TaskCreate]:
     """
-    Create environment and install package
+    Create environment, install package, and prepare task list
     """
+
     logger = get_logger(logger_name)
+
+    # Only proceed if package, version and manifest attributes are set
+    task_pkg.check()
+
     try:
-        logger.debug("Creating venv and installing package")
 
+        logger.debug("Creating venv and installing package")
         python_bin, package_root = await _create_venv_install_package(
             path=venv_path,
             task_pkg=task_pkg,
             logger_name=logger_name,
         )
+        logger.debug("Venv creation and package installation ended correctly.")
 
-        logger.debug("Loading task manifest")
-
-        task_list = load_manifest(
-            package_root=package_root,
-            python_bin=python_bin,
-            source=task_pkg.source,
-        )
-        logger.debug("Loaded task manifest")
+        # Prepare task_list with appropriate metadata
+        logger.debug("Creating task list from manifest")
+        task_list = []
+        for t in task_pkg.package_manifest.task_list:
+            # Fill in attributes for TaskCreate
+            task_executable = package_root / t.executable
+            cmd = f"{python_bin.as_posix()} {task_executable.as_posix()}"
+            task_name_slug = t.name.replace(" ", "_").lower()
+            task_source = f"{task_pkg.package_source}:{task_name_slug}"
+            if not task_executable.exists():
+                raise FileNotFoundError(
+                    f"Cannot find executable `{task_executable}` "
+                    f"for task `{t.name}`"
+                )
+            manifest = task_pkg.package_manifest
+            if manifest.has_args_schemas:
+                additional_attrs = dict(
+                    args_schema_version=manifest.args_schema_version
+                )
+            else:
+                additional_attrs = {}
+            this_task = TaskCreate(
+                **t.dict(),
+                command=cmd,
+                version=task_pkg.package_version,
+                **additional_attrs,
+                source=task_source,
+            )
+            task_list.append(this_task)
+        logger.debug("Task list created correctly")
     except Exception as e:
         logger.error("Task manifest loading failed")
         raise e
     return task_list
 
 
-def read_manifest(file: Union[Path, IOBase]) -> ManifestV1:
-    """
-    Read and parse manifest file
-    """
-    if isinstance(file, IOBase):
-        manifest_dict = json.load(file)
-    else:
-        with file.open("r") as f:
-            manifest_dict = json.load(f)
-
-    manifest_version = str(manifest_dict["manifest_version"])
-    if manifest_version == "1":
-        manifest = ManifestV1(**manifest_dict)
-    else:
-        raise ValueError("Manifest version {manifest_version=} not supported")
-
-    return manifest
-
-
-def load_manifest(
-    package_root: Path,
-    python_bin: Path,
-    source: str,
-) -> list[TaskCreate]:
-
-    manifest_file = package_root / "__FRACTAL_MANIFEST__.json"
-    manifest = read_manifest(manifest_file)
-
-    task_list = []
-    for t in manifest.task_list:
-        task_executable = package_root / t.executable
-        if not task_executable.exists():
-            raise FileNotFoundError(
-                f"Cannot find executable `{task_executable}` "
-                f"for task `{t.name}`"
-            )
-        cmd = f"{python_bin.as_posix()} {task_executable.as_posix()}"
-        this_task = TaskCreate(**t.dict(), command=cmd, source=source)
-        task_list.append(this_task)
-    return task_list
-
-
 async def _create_venv_install_package(
     *,
     task_pkg: _TaskCollectPip,
     path: Path,
     logger_name: str,
 ) -> tuple[Path, Path]:
     """Create venv and install package
@@ -399,15 +462,17 @@
     pip = venv_path / "venv/bin/pip"
 
     extras = f"[{task_pkg.package_extras}]" if task_pkg.package_extras else ""
 
     if task_pkg.is_local_package:
         pip_install_str = f"{task_pkg.package_path.as_posix()}{extras}"
     else:
-        version_string = f"=={task_pkg.version}" if task_pkg.version else ""
+        version_string = (
+            f"=={task_pkg.package_version}" if task_pkg.package_version else ""
+        )
         pip_install_str = f"{task_pkg.package}{extras}{version_string}"
 
     cmd_install = f"{pip} install {pip_install_str}"
     cmd_inspect = f"{pip} show {task_pkg.package}"
 
     await execute_command(
         cwd=venv_path,
```

### Comparing `fractal_server-1.3.0a2/fractal_server/utils.py` & `fractal_server-1.3.0a3/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a2/pyproject.toml` & `fractal_server-1.3.0a3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.3.0a2"
+version = "1.3.0a3"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -19,14 +19,15 @@
 sqlmodel = "^0.0.8"
 aiosqlite = "^0.17.0"
 fastapi-users = {extras = ["oauth"], version = "^10.1"}
 alembic = "^1.9.1"
 uvicorn = "^0.20.0"
 sqlalchemy = "^1.4"
 SQLAlchemy-Utils = "^0.38.3"
+pydantic = ">=1.10.8"
 
 clusterfutures = { version = "^0.5", optional = true}
 cloudpickle = {version = ">=2.2.1 <2.3.0", optional = true}
 
 asyncpg = { version = "^0.27.0", optional = true }
 psycopg2 = { version = "^2.9.5", optional = true }
 gunicorn = { version = "^20.1.0", optional = true }
@@ -71,15 +72,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.3.0a2"
+current_version = "1.3.0a3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.3.0a2/PKG-INFO` & `fractal_server-1.3.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.3.0a2
+Version: 1.3.0a3
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -21,14 +21,15 @@
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0) ; extra == "postgres"
 Requires-Dist: cloudpickle (>=2.2.1,<2.3.0) ; extra == "slurm"
 Requires-Dist: clusterfutures (>=0.5,<0.6) ; extra == "slurm"
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: fastapi-users[oauth] (>=10.1,<11.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0) ; extra == "gunicorn"
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0) ; extra == "postgres"
+Requires-Dist: pydantic (>=1.10.8)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: sqlalchemy (>=1.4,<2.0)
 Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
 # Fractal Server
```

