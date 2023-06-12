# Comparing `tmp/inet-nm-0.0.4.tar.gz` & `tmp/inet-nm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inet-nm-0.0.4.tar", last modified: Thu Jun  8 11:47:24 2023, max compression
+gzip compressed data, was "inet-nm-0.0.5.tar", last modified: Mon Jun 12 15:27:18 2023, max compression
```

## Comparing `inet-nm-0.0.4.tar` & `inet-nm-0.0.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.088981 inet-nm-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-08 11:46:43.000000 inet-nm-0.0.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.080981 inet-nm-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.084981 inet-nm-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-08 11:46:43.000000 inet-nm-0.0.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 11:46:43.000000 inet-nm-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 11:46:43.000000 inet-nm-0.0.4/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-08 11:46:43.000000 inet-nm-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-08 11:46:43.000000 inet-nm-0.0.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 11:46:43.000000 inet-nm-0.0.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-08 11:46:43.000000 inet-nm-0.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-06-08 11:46:43.000000 inet-nm-0.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-08 11:46:43.000000 inet-nm-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-06-08 11:47:24.088981 inet-nm-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-08 11:46:43.000000 inet-nm-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.084981 inet-nm-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.084981 inet-nm-0.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-08 11:46:43.000000 inet-nm-0.0.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-08 11:46:43.000000 inet-nm-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 11:46:43.000000 inet-nm-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-08 11:47:24.088981 inet-nm-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-08 11:46:43.000000 inet-nm-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.080981 inet-nm-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.084981 inet-nm-0.0.4/src/inet_nm/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/commissioner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/locking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/runner_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/runner_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-08 11:46:43.000000 inet-nm-0.0.4/src/inet_nm/update_os_board_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.084981 inet-nm-0.0.4/src/inet_nm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-06-08 11:47:24.000000 inet-nm-0.0.4/src/inet_nm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-08 11:47:24.000000 inet-nm-0.0.4/src/inet_nm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:47:24.000000 inet-nm-0.0.4/src/inet_nm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-08 11:47:24.000000 inet-nm-0.0.4/src/inet_nm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:47:23.000000 inet-nm-0.0.4/src/inet_nm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 11:47:24.000000 inet-nm-0.0.4/src/inet_nm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 11:47:24.000000 inet-nm-0.0.4/src/inet_nm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:24.088981 inet-nm-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_comissioner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_locking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_runner_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tests/test_runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-08 11:46:43.000000 inet-nm-0.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.473480 inet-nm-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-12 15:26:36.000000 inet-nm-0.0.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.453480 inet-nm-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.461480 inet-nm-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-12 15:26:36.000000 inet-nm-0.0.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-12 15:26:36.000000 inet-nm-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-12 15:26:36.000000 inet-nm-0.0.5/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-12 15:26:36.000000 inet-nm-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 15:26:36.000000 inet-nm-0.0.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 15:26:36.000000 inet-nm-0.0.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-12 15:26:36.000000 inet-nm-0.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-06-12 15:26:36.000000 inet-nm-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-12 15:26:36.000000 inet-nm-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-12 15:27:18.473480 inet-nm-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-06-12 15:26:36.000000 inet-nm-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.465480 inet-nm-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.465480 inet-nm-0.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 15:26:36.000000 inet-nm-0.0.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-12 15:26:36.000000 inet-nm-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 15:26:36.000000 inet-nm-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-12 15:27:18.473480 inet-nm-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-12 15:26:36.000000 inet-nm-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.453480 inet-nm-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.469480 inet-nm-0.0.5/src/inet_nm/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/commissioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/locking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/runner_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/runner_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-12 15:26:36.000000 inet-nm-0.0.5/src/inet_nm/update_os_board_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.469480 inet-nm-0.0.5/src/inet_nm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 15:27:18.000000 inet-nm-0.0.5/src/inet_nm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:27:18.473480 inet-nm-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_comissioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_locking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_runner_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tests/test_runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-12 15:26:36.000000 inet-nm-0.0.5/tox.ini
```

### Comparing `inet-nm-0.0.4/.coveragerc` & `inet-nm-0.0.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/.github/workflows/ci.yml` & `inet-nm-0.0.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/.gitignore` & `inet-nm-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/.pre-commit-config.yaml` & `inet-nm-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/.readthedocs.yml` & `inet-nm-0.0.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/CHANGELOG.md` & `inet-nm-0.0.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/CONTRIBUTING.md` & `inet-nm-0.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/LICENSE.txt` & `inet-nm-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/PKG-INFO` & `inet-nm-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inet-nm
-Version: 0.0.4
+Version: 0.0.5
 Summary: cli application for managing nodes
 Home-page: https://github.com/inetrg/inet-nm
 Author: Kevin Weiss
 Author-email: weiss.kevin604@gmail.com
 License: MIT
 Project-URL: Documentation, https://inet-nm.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/inetrg/inet-nm
@@ -282,28 +282,53 @@
 This project is licensed under the terms of the MIT license. See the LICENSE file.
 
 ---
 For any questions or contributions, please refer to the issues tab or the contributing guide.
 
 ## Roadmap
 
-- Check to see if config file is writeable first
-- Prompt to write config board info files if failures occur
 - Add optional power control
     - Check if power control available for which boards
     - Turn all ports on by default whenever checking connection
     - Turn all unused off commissioned nodes by default once the action is complete
     - flags to prevent power options
     - Generic command to turn on all ports or specific nodes
     - Caching usb locations
-- check if tmux is installed
 - cleanup exception handling
+  - Removing lock if they have been removed before...
+```
+$ inet-nm-tmux -a
+duplicate session: default
+[exited]
+Traceback (most recent call last):
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_cli.py", line 91, in nm_tmux
+    runner.run()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 123, in run
+    self.release()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 85, in release
+    lock.release()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/filelock.py", line 89, in release
+    os.unlink(self.file_name)
+FileNotFoundError: [Errno 2] No such file or directory: '/tmp/inet_nm/locks/e8d68aaf8b4119ca21db0849a8339568.lock'
+
+During handling of the above exception, another exception occurred:
+
+Traceback (most recent call last):
+  File "/home/weiss/wd/inet-nm/.venv/bin/inet-nm-tmux", line 33, in <module>
+    sys.exit(load_entry_point('inet-nm', 'console_scripts', 'inet-nm-tmux')())
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_cli.py", line 91, in nm_tmux
+    runner.run()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 130, in __exit__
+    self.release()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 85, in release
+    lock.release()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/filelock.py", line 88, in release
+    os.close(self.fd)
+OSError: [Errno 9] Bad file descriptor
+```
 - remove all or one board
-- commission ignored devices
-- shell script prepend a string to stdio
-- test paned windows with many many boards
 - allow user boards that will not get overwritten
 - Nice readme with some gifs of usage
 - Add a CLI way and example get the port live based off UID to handle reconnecting within tmux session
 - Improve getting started
-- exec command should exit all threads safely on keyboard interrupt
 - Add a session or exec timeout that will abort if the call takes too long
+- Add tests that go through the cli
```

### Comparing `inet-nm-0.0.4/README.md` & `inet-nm-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -260,28 +260,53 @@
 This project is licensed under the terms of the MIT license. See the LICENSE file.
 
 ---
 For any questions or contributions, please refer to the issues tab or the contributing guide.
 
 ## Roadmap
 
-- Check to see if config file is writeable first
-- Prompt to write config board info files if failures occur
 - Add optional power control
     - Check if power control available for which boards
     - Turn all ports on by default whenever checking connection
     - Turn all unused off commissioned nodes by default once the action is complete
     - flags to prevent power options
     - Generic command to turn on all ports or specific nodes
     - Caching usb locations
-- check if tmux is installed
 - cleanup exception handling
+  - Removing lock if they have been removed before...
+```
+$ inet-nm-tmux -a
+duplicate session: default
+[exited]
+Traceback (most recent call last):
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_cli.py", line 91, in nm_tmux
+    runner.run()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 123, in run
+    self.release()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 85, in release
+    lock.release()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/filelock.py", line 89, in release
+    os.unlink(self.file_name)
+FileNotFoundError: [Errno 2] No such file or directory: '/tmp/inet_nm/locks/e8d68aaf8b4119ca21db0849a8339568.lock'
+
+During handling of the above exception, another exception occurred:
+
+Traceback (most recent call last):
+  File "/home/weiss/wd/inet-nm/.venv/bin/inet-nm-tmux", line 33, in <module>
+    sys.exit(load_entry_point('inet-nm', 'console_scripts', 'inet-nm-tmux')())
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_cli.py", line 91, in nm_tmux
+    runner.run()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 130, in __exit__
+    self.release()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 85, in release
+    lock.release()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/filelock.py", line 88, in release
+    os.close(self.fd)
+OSError: [Errno 9] Bad file descriptor
+```
 - remove all or one board
-- commission ignored devices
-- shell script prepend a string to stdio
-- test paned windows with many many boards
 - allow user boards that will not get overwritten
 - Nice readme with some gifs of usage
 - Add a CLI way and example get the port live based off UID to handle reconnecting within tmux session
 - Improve getting started
-- exec command should exit all threads safely on keyboard interrupt
 - Add a session or exec timeout that will abort if the call takes too long
+- Add tests that go through the cli
```

### Comparing `inet-nm-0.0.4/docs/Makefile` & `inet-nm-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/docs/conf.py` & `inet-nm-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/docs/index.md` & `inet-nm-0.0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/setup.cfg` & `inet-nm-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/setup.py` & `inet-nm-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/src/inet_nm/_helpers.py` & `inet-nm-0.0.5/src/inet_nm/_helpers.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/src/inet_nm/check.py` & `inet-nm-0.0.5/src/inet_nm/check.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,30 +53,35 @@
             if connected:
                 selected_nodes.append(node)
         elif not connected:
             selected_nodes.append(node)
     return selected_nodes
 
 
-def remove_used_nodes(nodes: List[NmNode], used_uids: List[str]) -> List[NmNode]:
+def filter_used_nodes(
+    nodes: List[NmNode], used_uids: List[str], remove=True
+) -> List[NmNode]:
     """
-    Remove the nodes that are already used from the list of nodes.
+    Filter the nodes based on the provided used UIDs.
 
     Args:
         nodes: A list of nodes to filter.
         used_uids: A list of UIDs of nodes that are already used.
+        remove: If True, remove the used nodes. If False, remove the unused nodes.
 
     Returns:
         List[NmNode]: A list of nodes that are not already used.
     """
     if used_uids is None:
         used_uids = []
     selected_nodes = []
     for node in nodes:
-        if node.uid not in used_uids:
+        if node.uid not in used_uids and remove:
+            selected_nodes.append(node)
+        elif node.uid in used_uids and not remove:
             selected_nodes.append(node)
     return selected_nodes
 
 
 def filter_nodes(nodes: List[NmNode], must_contain: List[str]) -> List[NmNode]:
     """
     Filter the nodes based on the provided features.
@@ -184,44 +189,53 @@
     nodes: List[NmNode],
     all_nodes: bool = False,
     missing: bool = False,
     feat_filter: List[str] = None,
     feat_eval: str = None,
     used: bool = False,
     skip_dups: bool = False,
+    only_used: bool = False,
+    boards: List[str] = None,
     locked_nodes: List[str] = None,
 ) -> List[NmNode]:
     """
     Get a filtered list of nodes based on the provided parameters.
 
     Args:
         nodes: A list of nodes to check.
         all_nodes: If True, all nodes will be returned.
         missing: If True, only the nodes that are missing will be returned.
         feat_filter: A list of features. Only the nodes that contain all of
             these features will be returned.
         feat_eval: The function to use to evaluate the features.
         used: If True, used nodes will also be returned.
         skip_dups: If True, duplicate nodes will be removed.
+        only_used: If True, only the used nodes will be returned.
         locked_nodes: A list of UIDs of nodes that are locked.
 
     Returns:
         A list of filtered nodes.
     """
     features = get_all_features(nodes)
     if not all_nodes:
         nodes = get_nodes_with_state(nodes, connected=not missing)
-    if not used:
-        nodes = remove_used_nodes(nodes, locked_nodes)
+    if only_used:
+        nodes = filter_used_nodes(nodes, locked_nodes, remove=False)
+    elif not used:
+        nodes = filter_used_nodes(nodes, locked_nodes, remove=True)
     if feat_filter:
         nodes = filter_nodes(nodes, feat_filter)
     if feat_eval:
         nodes = eval_features(nodes, features, feat_eval)
     if skip_dups:
         nodes = skip_duplicate_boards(nodes)
+    if boards:
+        nodes = [node for node in nodes if node.board in boards]
+    # filter out ignored nodes
+    nodes = [node for node in nodes if not node.ignore]
     return nodes
 
 
 def check_args(parser: argparse.ArgumentParser):
     """
     Define the arguments for the argparse parser.
 
@@ -246,47 +260,68 @@
     parser.add_argument(
         "-e", "--feat-eval", type=str, help="Evaluate features with this function"
     )
     parser.add_argument(
         "-u", "--used", action="store_true", help="Show used boards as well"
     )
     parser.add_argument(
+        "-o", "--only-used", action="store_true", help="Show only the used boards"
+    )
+    parser.add_argument(
         "-s", "--skip-dups", action="store_true", help="Skip duplicate boards"
     )
+    parser.add_argument(
+        "-b",
+        "--boards",
+        nargs="+",
+        help="Use only the list of boards that match these names",
+    )
 
 
 def get_filtered_nodes(
     config: str,
     all_nodes: bool = False,
     missing: bool = False,
     feat_filter: List[str] = None,
     feat_eval: str = None,
     used: bool = False,
     skip_dups: bool = False,
+    only_used: bool = False,
+    boards: List[str] = None,
 ) -> List[NmNode]:
     """
     Get a list of nodes based on the provided parameters.
 
     Args:
         config: The configuration path for the nodes.
         all_nodes: If True, all nodes will be returned.
         missing: If True, only the nodes that are missing will be returned.
         feat_filter: A list of features. Only the nodes that contain all of
             these features will be returned.
         feat_eval: The function to use to evaluate the features.
         used: If True, used nodes will also be returned.
         skip_dups: If True, duplicate nodes will be removed.
+        only_used: If True, only the used nodes will be returned.
 
     Returns:
         A list of filtered nodes.
     """
     nodes = cfg.NodesConfig(config).load()
     locked_nodes = get_locked_uids()
     nodes = check_nodes(
-        nodes, all_nodes, missing, feat_filter, feat_eval, used, skip_dups, locked_nodes
+        nodes,
+        all_nodes,
+        missing,
+        feat_filter,
+        feat_eval,
+        used,
+        skip_dups,
+        only_used,
+        boards,
+        locked_nodes,
     )
     return nodes
 
 
 def all_features_from_nodes(nodes: List[NmNode]) -> List[str]:
     """
     Get a list of all features provided by the nodes.
```

### Comparing `inet-nm-0.0.4/src/inet_nm/commissioner.py` & `inet-nm-0.0.5/src/inet_nm/commissioner.py`

 * *Files 5% similar despite different names*

```diff
@@ -173,14 +173,21 @@
     )
     parser.add_argument(
         "-m",
         "--mock-dev",
         help="Mock a device, useful for boards that do not have USB interfaces",
         action="store_true",
     )
+    parser.add_argument(
+        "-i",
+        "--ignore",
+        help="Device will always be ignore, used for ttys that are connected "
+        "but not part of the inet-nm ecosystem.",
+        action="store_true",
+    )
 
     args = parser.parse_args()
     nodes_cfg = cfg.NodesConfig(args.config)
     bi_cfg = cfg.BoardInfoConfig(args.config)
     # Check early since we will need to write eventually
     nodes_cfg.check_file(writable=True)
     bi_cfg.check_file(writable=False)
@@ -193,19 +200,24 @@
         nm_nodes.append(mock_device())
     print(f"Found {len(saved_nodes)} saved nodes in {args.config}")
 
     try:
         selected_node = select_available_node(nm_nodes)
     except ValueError:
         print("No available nodes found")
-        return
-    binfo = bi_cfg.load()
-    selected_node.board = select_board(list(binfo.keys()), selected_node)
-    if selected_node.board in binfo:
-        selected_node.features_provided = binfo[selected_node.board]
+        sys.exit(1)
+    if args.ignore:
+        selected_node.ignore = True
+    else:
+        binfo = bi_cfg.load()
+        selected_node.board = args.board or select_board(
+            list(binfo.keys()), selected_node
+        )
+        if selected_node.board in binfo:
+            selected_node.features_provided = binfo[selected_node.board]
 
     nodes = add_node_to_nodes(saved_nodes, selected_node)
     nodes_cfg.save(nodes)
     print(f"Updated {nodes_cfg.file_path}")
 
 
 def update_commissioned():
```

### Comparing `inet-nm-0.0.4/src/inet_nm/config.py` & `inet-nm-0.0.5/src/inet_nm/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -128,37 +128,31 @@
         Returns:
             The loaded nodes data.
         """
         data = super().load()
         return [NmNode.from_dict(item) for item in data]
 
 
-def get_lock_path(config_dir: Union[Path, str]) -> Path:
+def get_default_path() -> Path:
     """
-    Return the lock file path constructed from config_dir.
-
-    Args:
-        config_dir (Union[Path, str]): Directory for the configuration files.
+    Return the default path for the configuration files.
 
     Returns:
-        Path: The full path to the lock file.
+        Path: The default path for the configuration files.
     """
-    config_dir = Path(config_dir).expanduser() / "locks"
-    config_dir.mkdir(parents=True, exist_ok=True)
-    return config_dir
+    return Path(os.environ.get("NM_CONFIG_DIR", "~/.config/inet_nm")).expanduser()
 
 
 def config_arg(parser: argparse.ArgumentParser):
     """
     Add a configuration argument to the provided parser.
 
     Args:
         parser (argparse.ArgumentParser): ArgumentParser object.
     """
-    nm_config_dir = os.environ.get("NM_CONFIG_DIR", "~/.config/inet_nm")
     parser.add_argument(
         "-c",
         "--config",
-        default=nm_config_dir,
+        default=get_default_path(),
         help="Path to the config dir, defaults to NM_CONFIG_DIR or "
         "~/.config/inet_nm if NM_CONFIG_DIR is not set",
     )
```

### Comparing `inet-nm-0.0.4/src/inet_nm/data_types.py` & `inet-nm-0.0.5/src/inet_nm/data_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,26 +42,28 @@
         vendor: Name of the vendor.
         driver: Name of the driver.
         model: Model name of the device.
         uid: Unique ID of the device
         board: Name of the board.
         features_provided: List of features provided by the device.
         mock: Whether the node is a mock node.
+        ignore: Whether the node should be ignored.
     """
 
     serial: str
     vendor_id: str
     product_id: str
     vendor: str
     driver: str
     model: Optional[str] = None
     uid: Optional[str] = None
     board: Optional[str] = None
     features_provided: Optional[List[str]] = None
     mock: bool = False
+    ignore: bool = False
 
     def __post_init__(self):
         """Initialize additional attributes after instantiation."""
         self.features_provided = self.features_provided or []
         self.uid = self.uid or NmNode.calculate_uid(
             self.product_id, self.vendor_id, self.serial
         )
```

### Comparing `inet-nm-0.0.4/src/inet_nm/filelock.py` & `inet-nm-0.0.5/src/inet_nm/filelock.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,18 @@
             FileLockTimeout: If the timeout has passed and the lock
                 has not been released.
         """
         timeout = timeout or self.timeout
         start_time = time.time()
         while True:
             try:
-                self.fd = os.open(self.file_name, os.O_CREAT | os.O_EXCL | os.O_RDWR)
+                os.umask(0)
+                self.fd = os.open(
+                    self.file_name, flags=os.O_CREAT | os.O_EXCL | os.O_RDWR, mode=0o777
+                )
                 self._lock_held = True
                 break
             except FileExistsError:
                 if time.time() - start_time >= timeout:
                     msg = f"Timeout trying to lock {self.file_name}"
                     raise FileLockTimeout(msg)
                 else:
```

### Comparing `inet-nm-0.0.4/src/inet_nm/locking.py` & `inet-nm-0.0.5/src/inet_nm/locking.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module contains functions for locking nodes."""
+import os
 import tempfile
 from pathlib import Path
 from typing import List
 
 from inet_nm._helpers import nm_print
 from inet_nm.data_types import NmNode
 
@@ -13,15 +14,16 @@
 
     If the directory does not exist, create it.
 
     Returns:
         The path to the lock files directory.
     """
     path = Path(tempfile.gettempdir(), "inet_nm", "locks")
-    path.mkdir(parents=True, exist_ok=True)
+    os.umask(0)
+    path.mkdir(parents=True, exist_ok=True, mode=0o777)
     return path
 
 
 def get_locked_uids() -> List[str]:
     """
     Get the list of UIDs of currently locked nodes.
```

### Comparing `inet-nm-0.0.4/src/inet_nm/runner_apps.py` & `inet-nm-0.0.5/src/inet_nm/runner_apps.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/src/inet_nm/runner_base.py` & `inet-nm-0.0.5/src/inet_nm/runner_base.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/src/inet_nm/update_os_board_list.py` & `inet-nm-0.0.5/src/inet_nm/update_os_board_list.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/src/inet_nm.egg-info/PKG-INFO` & `inet-nm-0.0.5/src/inet_nm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inet-nm
-Version: 0.0.4
+Version: 0.0.5
 Summary: cli application for managing nodes
 Home-page: https://github.com/inetrg/inet-nm
 Author: Kevin Weiss
 Author-email: weiss.kevin604@gmail.com
 License: MIT
 Project-URL: Documentation, https://inet-nm.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/inetrg/inet-nm
@@ -282,28 +282,53 @@
 This project is licensed under the terms of the MIT license. See the LICENSE file.
 
 ---
 For any questions or contributions, please refer to the issues tab or the contributing guide.
 
 ## Roadmap
 
-- Check to see if config file is writeable first
-- Prompt to write config board info files if failures occur
 - Add optional power control
     - Check if power control available for which boards
     - Turn all ports on by default whenever checking connection
     - Turn all unused off commissioned nodes by default once the action is complete
     - flags to prevent power options
     - Generic command to turn on all ports or specific nodes
     - Caching usb locations
-- check if tmux is installed
 - cleanup exception handling
+  - Removing lock if they have been removed before...
+```
+$ inet-nm-tmux -a
+duplicate session: default
+[exited]
+Traceback (most recent call last):
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_cli.py", line 91, in nm_tmux
+    runner.run()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 123, in run
+    self.release()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 85, in release
+    lock.release()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/filelock.py", line 89, in release
+    os.unlink(self.file_name)
+FileNotFoundError: [Errno 2] No such file or directory: '/tmp/inet_nm/locks/e8d68aaf8b4119ca21db0849a8339568.lock'
+
+During handling of the above exception, another exception occurred:
+
+Traceback (most recent call last):
+  File "/home/weiss/wd/inet-nm/.venv/bin/inet-nm-tmux", line 33, in <module>
+    sys.exit(load_entry_point('inet-nm', 'console_scripts', 'inet-nm-tmux')())
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_cli.py", line 91, in nm_tmux
+    runner.run()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 130, in __exit__
+    self.release()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/runner_base.py", line 85, in release
+    lock.release()
+  File "/home/weiss/wd/inet-nm/src/inet_nm/filelock.py", line 88, in release
+    os.close(self.fd)
+OSError: [Errno 9] Bad file descriptor
+```
 - remove all or one board
-- commission ignored devices
-- shell script prepend a string to stdio
-- test paned windows with many many boards
 - allow user boards that will not get overwritten
 - Nice readme with some gifs of usage
 - Add a CLI way and example get the port live based off UID to handle reconnecting within tmux session
 - Improve getting started
-- exec command should exit all threads safely on keyboard interrupt
 - Add a session or exec timeout that will abort if the call takes too long
+- Add tests that go through the cli
```

### Comparing `inet-nm-0.0.4/src/inet_nm.egg-info/SOURCES.txt` & `inet-nm-0.0.5/src/inet_nm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/tests/test_check.py` & `inet-nm-0.0.5/tests/test_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import pytest
 
 from inet_nm.check import (
     check_nodes,
     eval_features,
     filter_nodes,
+    filter_used_nodes,
     get_all_features,
-    remove_used_nodes,
     skip_duplicate_boards,
 )
 from inet_nm.data_types import NmNode
 
 
 @pytest.fixture
 def dummy_nodes():
@@ -96,21 +96,26 @@
         dummy_nodes[1].uid,
         dummy_nodes[2].uid,
     ]
     nodes = check_nodes(dummy_nodes)
     assert len(nodes) == 3
 
 
-def test_remove_used_nodes(dummy_nodes, locked_nodes):
+def test_filter_used_nodes(dummy_nodes, locked_nodes):
     """Ensure locked nodes are removed from the list of nodes."""
-    nodes = remove_used_nodes(dummy_nodes, locked_nodes)
+    nodes = filter_used_nodes(dummy_nodes, locked_nodes, remove=True)
     assert len(nodes) == 2
     assert nodes[0].serial == "3"
     assert nodes[1].serial == "4"
 
+    nodes = filter_used_nodes(dummy_nodes, locked_nodes, remove=False)
+    assert len(nodes) == 2
+    assert nodes[0].serial == "1"
+    assert nodes[1].serial == "2"
+
 
 def test_eval_features(dummy_nodes):
     """Ensure nodes are filtered correctly using eval feature."""
     features = get_all_features(dummy_nodes)
     nodes = eval_features(
         dummy_nodes, features, "(feature3 and feature2) or (feature1 and not feature2)"
     )
```

### Comparing `inet-nm-0.0.4/tests/test_comissioner.py` & `inet-nm-0.0.5/tests/test_comissioner.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/tests/test_config.py` & `inet-nm-0.0.5/tests/test_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,13 +33,7 @@
     cfg_inst.save(data)
     loaded_data = cfg_inst.load()
     assert loaded_data == data
 
     res = cfg_type("does_not_exist").load()
     assert len(res) == 0
     assert isinstance(res, cfg_type._LOAD_TYPE)
-
-
-def test_get_lock_path(tmp_path):
-    """Test getting the lock path."""
-    lock_path = cfg.get_lock_path(tmp_path)
-    assert lock_path == tmp_path / "locks"
```

### Comparing `inet-nm-0.0.4/tests/test_data_types.py` & `inet-nm-0.0.5/tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/tests/test_filelock.py` & `inet-nm-0.0.5/tests/test_filelock.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/tests/test_helpers.py` & `inet-nm-0.0.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/tests/test_locking.py` & `inet-nm-0.0.5/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/tests/test_runner_apps.py` & `inet-nm-0.0.5/tests/test_runner_apps.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/tests/test_runner_base.py` & `inet-nm-0.0.5/tests/test_runner_base.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.4/tox.ini` & `inet-nm-0.0.5/tox.ini`

 * *Files identical despite different names*

