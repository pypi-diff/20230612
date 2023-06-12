# Comparing `tmp/pytest-tui-1.9.2.tar.gz` & `tmp/pytest-tui-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-tui-1.9.2.tar", last modified: Thu Apr  6 20:34:34 2023, max compression
+gzip compressed data, was "pytest-tui-2.0.0.tar", last modified: Mon Jun 12 04:05:25 2023, max compression
```

## Comparing `pytest-tui-1.9.2.tar` & `pytest-tui-2.0.0.tar`

### file list

```diff
@@ -1,80 +1,98 @@
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.910988 pytest-tui-1.9.2/
--rw-r--r--   0 jwr003   (623385768) 542971493     1138 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/.gitignore
--rw-r--r--   0 jwr003   (623385768) 542971493       25 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/.isort.cfg
--rw-r--r--   0 jwr003   (623385768) 542971493      202 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/.pre-commit-config.yaml
--rw-r--r--   0 jwr003   (623385768) 542971493     7852 2023-04-06 20:07:16.000000 pytest-tui-1.9.2/CHANGELOG.md
--rw-r--r--   0 jwr003   (623385768) 542971493     1079 2022-04-12 03:00:30.000000 pytest-tui-1.9.2/LICENSE
--rw-r--r--   0 jwr003   (623385768) 542971493    11442 2023-04-06 20:34:34.911276 pytest-tui-1.9.2/PKG-INFO
--rw-r--r--   0 jwr003   (623385768) 542971493    10678 2023-04-06 17:30:25.000000 pytest-tui-1.9.2/README.md
--rw-r--r--   0 jwr003   (623385768) 542971493       30 2022-09-15 05:14:38.000000 pytest-tui-1.9.2/conftest.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.812182 pytest-tui-1.9.2/demo-tests/
--rw-r--r--   0 jwr003   (623385768) 542971493     6240 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/demo-tests/conftest.py
--rw-r--r--   0 jwr003   (623385768) 542971493     1421 2023-02-12 14:23:47.000000 pytest-tui-1.9.2/demo-tests/test_0.py
--rw-r--r--   0 jwr003   (623385768) 542971493    14208 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/demo-tests/test_1.py
--rw-r--r--   0 jwr003   (623385768) 542971493     2824 2023-01-12 06:08:17.000000 pytest-tui-1.9.2/demo-tests/test_2.py
--rw-r--r--   0 jwr003   (623385768) 542971493     2685 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/demo-tests/test_basic.py
--rw-r--r--   0 jwr003   (623385768) 542971493      352 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/demo-tests/test_class.py
--rw-r--r--   0 jwr003   (623385768) 542971493     2227 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/demo-tests/test_hoefling.py
--rw-r--r--   0 jwr003   (623385768) 542971493      276 2022-09-15 05:14:38.000000 pytest-tui-1.9.2/demo-tests/test_issue_1004.py
--rw-r--r--   0 jwr003   (623385768) 542971493    13004 2023-01-12 06:08:17.000000 pytest-tui-1.9.2/demo-tests/test_random_results.py
--rw-r--r--   0 jwr003   (623385768) 542971493      398 2023-01-17 12:50:37.000000 pytest-tui-1.9.2/demo-tests/test_rerun_fixed.py
--rw-r--r--   0 jwr003   (623385768) 542971493      824 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/demo-tests/test_rerun_random.py
--rw-r--r--   0 jwr003   (623385768) 542971493      623 2023-01-12 06:08:17.000000 pytest-tui-1.9.2/demo-tests/test_single_xpass_xfail.py
--rw-r--r--   0 jwr003   (623385768) 542971493     1687 2023-01-12 06:08:17.000000 pytest-tui-1.9.2/demo-tests/test_warnings.py
--rw-r--r--   0 jwr003   (623385768) 542971493     1017 2023-01-12 06:08:17.000000 pytest-tui-1.9.2/demo-tests/test_xpass_xfail.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.822466 pytest-tui-1.9.2/misc/
--rw-r--r--   0 jwr003   (623385768) 542971493     1441 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/misc/RELEASE_INSTRUCTIONS
--rw-r--r--   0 jwr003   (623385768) 542971493     1453 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/misc/outcome_questions.txt
--rw-r--r--   0 jwr003   (623385768) 542971493      194 2023-04-06 16:55:39.000000 pytest-tui-1.9.2/pytest.ini
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.851798 pytest-tui-1.9.2/pytest_tui/
--rw-r--r--   0 jwr003   (623385768) 542971493      144 2023-01-30 05:13:19.000000 pytest-tui-1.9.2/pytest_tui/__init__.py
--rw-r--r--   0 jwr003   (623385768) 542971493     5805 2023-04-01 13:46:31.000000 pytest-tui-1.9.2/pytest_tui/__main__.py
--rw-r--r--   0 jwr003   (623385768) 542971493     9983 2023-04-01 13:46:31.000000 pytest-tui-1.9.2/pytest_tui/_tree_control.py
--rw-r--r--   0 jwr003   (623385768) 542971493    19487 2023-04-06 20:04:47.000000 pytest-tui-1.9.2/pytest_tui/html_gen.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.862823 pytest-tui-1.9.2/pytest_tui/log_experiments/
--rw-r--r--   0 jwr003   (623385768) 542971493     1817 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/pytest_tui/log_experiments/debug_context.py
--rw-r--r--   0 jwr003   (623385768) 542971493     2911 2023-04-01 13:46:31.000000 pytest-tui-1.9.2/pytest_tui/log_experiments/debug_html_logger.py
--rw-r--r--   0 jwr003   (623385768) 542971493     2888 2023-04-01 13:46:31.000000 pytest-tui-1.9.2/pytest_tui/log_experiments/foldable_loggers.py
--rw-r--r--   0 jwr003   (623385768) 542971493     1777 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/pytest_tui/log_experiments/test_debug_logger_html.py
--rw-r--r--   0 jwr003   (623385768) 542971493     2830 2023-04-01 13:46:31.000000 pytest-tui-1.9.2/pytest_tui/log_experiments/test_me.py
--rw-r--r--   0 jwr003   (623385768) 542971493     4526 2023-04-06 17:35:00.000000 pytest-tui-1.9.2/pytest_tui/log_experiments/tui_logger.py
--rw-r--r--   0 jwr003   (623385768) 542971493    17493 2023-04-06 16:42:20.000000 pytest-tui-1.9.2/pytest_tui/plugin.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.865170 pytest-tui-1.9.2/pytest_tui/resources/
--rw-r--r--   0 jwr003   (623385768) 542971493     2323 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/pytest_tui/resources/scripts.js
--rw-r--r--   0 jwr003   (623385768) 542971493    26897 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/pytest_tui/resources/styles.css
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.869717 pytest-tui-1.9.2/pytest_tui/stuff/
--rw-r--r--   0 jwr003   (623385768) 542971493     1379 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/pytest_tui/stuff/devnotes.md
--rw-r--r--   0 jwr003   (623385768) 542971493      718 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/pytest_tui/stuff/nonprintable_​​characters.md
--rw-r--r--   0 jwr003   (623385768) 542971493      455 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/pytest_tui/stuff/nonprintable_​​characters.txt
--rw-r--r--   0 jwr003   (623385768) 542971493     8855 2023-04-01 13:46:31.000000 pytest-tui-1.9.2/pytest_tui/tui_gen.py
--rw-r--r--   0 jwr003   (623385768) 542971493     9046 2023-04-06 17:35:00.000000 pytest-tui-1.9.2/pytest_tui/utils.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.857082 pytest-tui-1.9.2/pytest_tui.egg-info/
--rw-r--r--   0 jwr003   (623385768) 542971493    11442 2023-04-06 20:34:34.000000 pytest-tui-1.9.2/pytest_tui.egg-info/PKG-INFO
--rw-r--r--   0 jwr003   (623385768) 542971493     1827 2023-04-06 20:34:34.000000 pytest-tui-1.9.2/pytest_tui.egg-info/SOURCES.txt
--rw-r--r--   0 jwr003   (623385768) 542971493        1 2023-04-06 20:34:34.000000 pytest-tui-1.9.2/pytest_tui.egg-info/dependency_links.txt
--rw-r--r--   0 jwr003   (623385768) 542971493      123 2023-04-06 20:34:34.000000 pytest-tui-1.9.2/pytest_tui.egg-info/entry_points.txt
--rw-r--r--   0 jwr003   (623385768) 542971493      113 2023-04-06 20:34:34.000000 pytest-tui-1.9.2/pytest_tui.egg-info/requires.txt
--rw-r--r--   0 jwr003   (623385768) 542971493       11 2023-04-06 20:34:34.000000 pytest-tui-1.9.2/pytest_tui.egg-info/top_level.txt
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.876465 pytest-tui-1.9.2/requirements/
--rw-r--r--   0 jwr003   (623385768) 542971493      111 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/requirements/requirements-dev.in
--rw-r--r--   0 jwr003   (623385768) 542971493     1491 2023-04-06 17:32:59.000000 pytest-tui-1.9.2/requirements/requirements-dev.txt
--rw-r--r--   0 jwr003   (623385768) 542971493      113 2023-03-30 17:44:17.000000 pytest-tui-1.9.2/requirements/requirements.in
--rw-r--r--   0 jwr003   (623385768) 542971493      992 2023-04-06 17:32:40.000000 pytest-tui-1.9.2/requirements/requirements.txt
--rw-r--r--   0 jwr003   (623385768) 542971493       67 2023-04-06 20:34:34.919768 pytest-tui-1.9.2/setup.cfg
--rw-r--r--   0 jwr003   (623385768) 542971493     1661 2023-04-06 17:17:01.000000 pytest-tui-1.9.2/setup.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.719815 pytest-tui-1.9.2/testing/
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.896938 pytest-tui-1.9.2/testing/bash/
--rwxr-xr-x   0 jwr003   (623385768) 542971493     2231 2023-04-06 20:33:56.000000 pytest-tui-1.9.2/testing/bash/test.sh
--rw-r--r--   0 jwr003   (623385768) 542971493      195 2023-02-01 13:08:57.000000 pytest-tui-1.9.2/testing/bash/tui_expect.tcl
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.900777 pytest-tui-1.9.2/testing/python/
--rw-r--r--   0 jwr003   (623385768) 542971493        0 2023-01-30 05:37:43.000000 pytest-tui-1.9.2/testing/python/conftest.ini
--rw-r--r--   0 jwr003   (623385768) 542971493      431 2023-01-17 01:43:11.000000 pytest-tui-1.9.2/testing/python/test_pytest_tui.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.720635 pytest-tui-1.9.2/testing/robot/
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.904837 pytest-tui-1.9.2/testing/robot/Resources/
--rw-r--r--   0 jwr003   (623385768) 542971493      129 2023-02-01 13:08:57.000000 pytest-tui-1.9.2/testing/robot/Resources/common.resource
--rw-r--r--   0 jwr003   (623385768) 542971493      420 2023-01-17 12:50:37.000000 pytest-tui-1.9.2/testing/robot/Resources/vars.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-04-06 20:34:34.910166 pytest-tui-1.9.2/testing/robot/Tests/
--rw-r--r--   0 jwr003   (623385768) 542971493     1253 2023-02-01 13:08:57.000000 pytest-tui-1.9.2/testing/robot/Tests/001_test_basic.robot
--rw-r--r--   0 jwr003   (623385768) 542971493      738 2023-02-01 13:08:57.000000 pytest-tui-1.9.2/testing/robot/Tests/002_test_tui.robot
--rw-r--r--   0 jwr003   (623385768) 542971493      345 2023-02-01 13:08:57.000000 pytest-tui-1.9.2/testing/robot/Tests/003_test_tuih.robot
--rw-r--r--   0 jwr003   (623385768) 542971493     1964 2023-02-01 13:08:57.000000 pytest-tui-1.9.2/tox.ini
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.654799 pytest-tui-2.0.0/
+-rw-r--r--   0 jwr003   (623385768) 542971493     1141 2023-06-12 04:04:49.000000 pytest-tui-2.0.0/.gitignore
+-rw-r--r--   0 jwr003   (623385768) 542971493       25 2023-03-30 17:44:17.000000 pytest-tui-2.0.0/.isort.cfg
+-rw-r--r--   0 jwr003   (623385768) 542971493      202 2023-03-30 17:44:17.000000 pytest-tui-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 jwr003   (623385768) 542971493     8779 2023-06-12 02:30:29.000000 pytest-tui-2.0.0/CHANGELOG.md
+-rw-r--r--   0 jwr003   (623385768) 542971493     1079 2022-04-12 03:00:30.000000 pytest-tui-2.0.0/LICENSE
+-rw-r--r--   0 jwr003   (623385768) 542971493    14249 2023-06-12 04:05:25.655217 pytest-tui-2.0.0/PKG-INFO
+-rw-r--r--   0 jwr003   (623385768) 542971493    13485 2023-06-11 22:23:06.000000 pytest-tui-2.0.0/README.md
+-rw-r--r--   0 jwr003   (623385768) 542971493       30 2023-06-10 12:11:18.000000 pytest-tui-2.0.0/conftest.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.276678 pytest-tui-2.0.0/demo-tests/
+-rw-r--r--   0 jwr003   (623385768) 542971493     6241 2023-04-12 05:23:43.000000 pytest-tui-2.0.0/demo-tests/conftest.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     1759 2023-06-11 23:53:32.000000 pytest-tui-2.0.0/demo-tests/test_0.py
+-rw-r--r--   0 jwr003   (623385768) 542971493    14208 2023-03-30 17:44:17.000000 pytest-tui-2.0.0/demo-tests/test_1.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     2824 2023-01-12 06:08:17.000000 pytest-tui-2.0.0/demo-tests/test_2.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     2685 2023-03-30 17:44:17.000000 pytest-tui-2.0.0/demo-tests/test_basic.py
+-rw-r--r--   0 jwr003   (623385768) 542971493      352 2023-03-30 17:44:17.000000 pytest-tui-2.0.0/demo-tests/test_class.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     6170 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/demo-tests/test_fold_regex.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     2227 2023-03-30 17:44:17.000000 pytest-tui-2.0.0/demo-tests/test_hoefling.py
+-rw-r--r--   0 jwr003   (623385768) 542971493      276 2022-09-15 05:14:38.000000 pytest-tui-2.0.0/demo-tests/test_issue_1004.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     3061 2023-04-12 05:23:23.000000 pytest-tui-2.0.0/demo-tests/test_logging.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     2443 2023-06-12 03:09:08.000000 pytest-tui-2.0.0/demo-tests/test_random_results.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     1346 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/demo-tests/test_regex.py
+-rw-r--r--   0 jwr003   (623385768) 542971493      398 2023-01-17 12:50:37.000000 pytest-tui-2.0.0/demo-tests/test_rerun_fixed.py
+-rw-r--r--   0 jwr003   (623385768) 542971493      824 2023-03-30 17:44:17.000000 pytest-tui-2.0.0/demo-tests/test_rerun_random.py
+-rw-r--r--   0 jwr003   (623385768) 542971493      623 2023-01-12 06:08:17.000000 pytest-tui-2.0.0/demo-tests/test_single_xpass_xfail.py
+-rw-r--r--   0 jwr003   (623385768) 542971493      464 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/demo-tests/test_sleep.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     1687 2023-01-12 06:08:17.000000 pytest-tui-2.0.0/demo-tests/test_warnings.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     1017 2023-01-12 06:08:17.000000 pytest-tui-2.0.0/demo-tests/test_xpass_xfail.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.285580 pytest-tui-2.0.0/misc/
+-rw-r--r--   0 jwr003   (623385768) 542971493     2184 2023-06-12 00:22:07.000000 pytest-tui-2.0.0/misc/RELEASE_INSTRUCTIONS
+-rw-r--r--   0 jwr003   (623385768) 542971493     1453 2023-03-30 17:44:17.000000 pytest-tui-2.0.0/misc/outcome_questions.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493     2751 2023-04-12 05:23:43.000000 pytest-tui-2.0.0/noxfile.py
+-rw-r--r--   0 jwr003   (623385768) 542971493      558 2023-06-11 05:24:10.000000 pytest-tui-2.0.0/pytest.ini
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.344290 pytest-tui-2.0.0/pytest_tui/
+-rw-r--r--   0 jwr003   (623385768) 542971493      144 2023-01-30 05:13:19.000000 pytest-tui-2.0.0/pytest_tui/__init__.py
+-rw-r--r--   0 jwr003   (623385768) 542971493    23039 2023-06-12 03:44:05.000000 pytest-tui-2.0.0/pytest_tui/html_gen.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.439535 pytest-tui-2.0.0/pytest_tui/log_experiments/
+-rw-r--r--   0 jwr003   (623385768) 542971493     1817 2023-03-30 17:44:17.000000 pytest-tui-2.0.0/pytest_tui/log_experiments/debug_context.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     2911 2023-04-01 13:46:31.000000 pytest-tui-2.0.0/pytest_tui/log_experiments/debug_html_logger.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     2888 2023-04-01 13:46:31.000000 pytest-tui-2.0.0/pytest_tui/log_experiments/foldable_loggers.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     1777 2023-03-30 17:44:17.000000 pytest-tui-2.0.0/pytest_tui/log_experiments/test_debug_logger_html.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     2830 2023-04-01 13:46:31.000000 pytest-tui-2.0.0/pytest_tui/log_experiments/test_me.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     4526 2023-04-06 17:35:00.000000 pytest-tui-2.0.0/pytest_tui/log_experiments/tui_logger.py
+-rw-r--r--   0 jwr003   (623385768) 542971493    18991 2023-06-12 03:44:05.000000 pytest-tui-2.0.0/pytest_tui/plugin.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.452821 pytest-tui-2.0.0/pytest_tui/resources/
+-rw-r--r--   0 jwr003   (623385768) 542971493     6624 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/pytest_tui/resources/scripts.js
+-rw-r--r--   0 jwr003   (623385768) 542971493    27486 2023-06-12 04:03:04.000000 pytest-tui-2.0.0/pytest_tui/resources/styles.css
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.484858 pytest-tui-2.0.0/pytest_tui/stuff/
+-rw-r--r--   0 jwr003   (623385768) 542971493     5805 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/pytest_tui/stuff/__main__.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     1379 2023-03-30 17:44:17.000000 pytest-tui-2.0.0/pytest_tui/stuff/devnotes.md
+-rw-r--r--   0 jwr003   (623385768) 542971493      718 2023-03-30 17:44:17.000000 pytest-tui-2.0.0/pytest_tui/stuff/nonprintable_​​characters.md
+-rw-r--r--   0 jwr003   (623385768) 542971493      401 2023-06-11 23:51:24.000000 pytest-tui-2.0.0/pytest_tui/stuff/nonprintable_​​characters.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493       34 2023-06-11 23:55:11.000000 pytest-tui-2.0.0/pytest_tui/stuff/tui_regexes_npc.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493     9983 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/pytest_tui/tree_control.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     8854 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/pytest_tui/tui_gen.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     8928 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/pytest_tui/utils.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.352652 pytest-tui-2.0.0/pytest_tui.egg-info/
+-rw-r--r--   0 jwr003   (623385768) 542971493    14249 2023-06-12 04:05:24.000000 pytest-tui-2.0.0/pytest_tui.egg-info/PKG-INFO
+-rw-r--r--   0 jwr003   (623385768) 542971493     2292 2023-06-12 04:05:24.000000 pytest-tui-2.0.0/pytest_tui.egg-info/SOURCES.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493        1 2023-06-12 04:05:24.000000 pytest-tui-2.0.0/pytest_tui.egg-info/dependency_links.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493      123 2023-06-12 04:05:24.000000 pytest-tui-2.0.0/pytest_tui.egg-info/entry_points.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493      127 2023-06-12 04:05:24.000000 pytest-tui-2.0.0/pytest_tui.egg-info/requires.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493       22 2023-06-12 04:05:24.000000 pytest-tui-2.0.0/pytest_tui.egg-info/top_level.txt
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.490537 pytest-tui-2.0.0/recordings/
+-rw-r--r--   0 jwr003   (623385768) 542971493        0 2023-04-07 00:07:15.000000 pytest-tui-2.0.0/recordings/__init__.py
+-rw-r--r--   0 jwr003   (623385768) 542971493      214 2023-04-07 00:10:40.000000 pytest-tui-2.0.0/recordings/new_recording_rec.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.495872 pytest-tui-2.0.0/requirements/
+-rw-r--r--   0 jwr003   (623385768) 542971493      160 2023-06-11 23:22:15.000000 pytest-tui-2.0.0/requirements/requirements-dev.in
+-rw-r--r--   0 jwr003   (623385768) 542971493      127 2023-06-11 22:59:52.000000 pytest-tui-2.0.0/requirements/requirements.in
+-rw-r--r--   0 jwr003   (623385768) 542971493       67 2023-06-12 04:05:25.673902 pytest-tui-2.0.0/setup.cfg
+-rw-r--r--   0 jwr003   (623385768) 542971493     1686 2023-06-12 02:32:40.000000 pytest-tui-2.0.0/setup.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.079171 pytest-tui-2.0.0/testing/
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.524807 pytest-tui-2.0.0/testing/bash/
+-rwxr-xr-x   0 jwr003   (623385768) 542971493     2231 2023-06-11 05:17:13.000000 pytest-tui-2.0.0/testing/bash/test.sh
+-rw-r--r--   0 jwr003   (623385768) 542971493      195 2023-02-01 13:08:57.000000 pytest-tui-2.0.0/testing/bash/tui_expect.tcl
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.540172 pytest-tui-2.0.0/testing/pytester/
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.579070 pytest-tui-2.0.0/testing/pytester/examples/
+-rw-r--r--   0 jwr003   (623385768) 542971493       20 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/testing/pytester/examples/example_regex.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493     1421 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/testing/pytester/examples/test_0.py
+-rw-r--r--   0 jwr003   (623385768) 542971493       14 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/testing/pytester/examples/test_empty.py
+-rw-r--r--   0 jwr003   (623385768) 542971493       49 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/testing/pytester/examples/test_pass.py
+-rw-r--r--   0 jwr003   (623385768) 542971493      750 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/testing/pytester/ideas.md
+-rw-r--r--   0 jwr003   (623385768) 542971493     1673 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/testing/pytester/test_plugin_options.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     8364 2023-06-12 03:45:20.000000 pytest-tui-2.0.0/testing/pytester/test_tui_with_pytester.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.585301 pytest-tui-2.0.0/testing/python/
+-rw-r--r--   0 jwr003   (623385768) 542971493        0 2023-06-10 21:45:58.000000 pytest-tui-2.0.0/testing/python/conftest.ini
+-rw-r--r--   0 jwr003   (623385768) 542971493      431 2023-06-10 21:45:58.000000 pytest-tui-2.0.0/testing/python/test_pytest_tui.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.078629 pytest-tui-2.0.0/testing/robot/
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.593232 pytest-tui-2.0.0/testing/robot/Resources/
+-rw-r--r--   0 jwr003   (623385768) 542971493      129 2023-02-01 13:08:57.000000 pytest-tui-2.0.0/testing/robot/Resources/common.resource
+-rw-r--r--   0 jwr003   (623385768) 542971493      420 2023-01-17 12:50:37.000000 pytest-tui-2.0.0/testing/robot/Resources/vars.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.628191 pytest-tui-2.0.0/testing/robot/Tests/
+-rw-r--r--   0 jwr003   (623385768) 542971493     1253 2023-02-01 13:08:57.000000 pytest-tui-2.0.0/testing/robot/Tests/001_test_basic.robot
+-rw-r--r--   0 jwr003   (623385768) 542971493      738 2023-02-01 13:08:57.000000 pytest-tui-2.0.0/testing/robot/Tests/002_test_tui.robot
+-rw-r--r--   0 jwr003   (623385768) 542971493      345 2023-02-01 13:08:57.000000 pytest-tui-2.0.0/testing/robot/Tests/003_test_tuih.robot
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-06-12 04:05:25.653783 pytest-tui-2.0.0/testing/sb/
+-rw-r--r--   0 jwr003   (623385768) 542971493     4788 2023-04-09 03:04:56.000000 pytest-tui-2.0.0/testing/sb/conftest.py
+-rw-r--r--   0 jwr003   (623385768) 542971493    12122 2023-06-11 04:44:54.000000 pytest-tui-2.0.0/testing/sb/test_html_report.py
```

### Comparing `pytest-tui-1.9.2/.gitignore` & `pytest-tui-2.0.0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 env/
-venv/
-.venv/
+venv*/
+.venvi*/
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
 lib/
@@ -57,15 +57,15 @@
 log.html
 report.html
 output.xml
 
 # Pytest and plugins
 .pytest_cache
 report.html
-ptt_files/
+tui_files/
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `pytest-tui-1.9.2/CHANGELOG.md` & `pytest-tui-2.0.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project tries to adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [1.9.2] 2023-04-36
-- Fixed issue 100 - an unfortunate bug where if the user does not specify the `--tui-fold-level` option, the HTML report will not render individual test cases correctly (they won't open/close when clicked). `--tui-fold-level ` is still supported but now if user does not specify it, the level defaults to WARNING, and displays the new Foldedd Output section anyway.
+## [2.0.0] 2023-06-12
+- Removed `--tui-fold-level` option, now replaced by modified ``--tui-regexfile` implementation (previous bullet point); allows for regex(es) to be specified in a file, rather than on the command line.
+- Fixed Issue 100 (obviated by previous change in fold behavior).
+- Changed output files folder to ./tui_files.
+- Added new buttons to About tab to remove/restore/invert colors.
+- Introduced tests to test the plugin itself, using pytest's 'pytester' fixture.
+- New buttons in HTML report to invert/remove/restore colors.
+- Added Faker library to standard dependencies.
+
+## [1.10.0] 2023-04-12
+- Added new folding mode `--tui-fold-regex`. This mode allows specifying reg-ex's marking the beginning and end of a section that the user wants to fold. See README for details.
+- Bumped `rich` library version to 12.6.0 to allow for use of SeleniumBase library during testing.
+- Fixed issue 100, where if the user does not specify the `--tui-fold-level` option, the HTML report will not render individual test cases correctly (they won't open/close when clicked). `--tui-fold-level ` is still supported but now if user does not specify it, the level defaults to WARNING, and displays the new Folded Output section anyway.
+- Added comprehensive HTML page testing using SelniumBase.
 - Fixed minor issue with bash test script not installing faker lib.
 - Fixed exception issue when specifying non-default output filename for HTML report.
 
 ## [1.9.1] 2023-03-30
-- Re-implemented the folding feature for HTML report. This version doesn't rely on the user having to do anything with their tests other than smartly partition their log statements into the proper debug levels for their application (i.e. no clunky logfile shananigans). The folding feature automatically folds all log output that is less than a configurable level. This is controlled with new command line option '--tui-fold-level'. Also, there is a new 'Actions' button in the HTML which folds/unfolds all fold sections.
+- Re-implemented the folding feature for HTML report. This version doesn't rely on the user having to do anything with their tests other than smartly partition their log statements into the proper debug levels for their application (i.e. no clunky logfile shananigans). The folding feature automatically folds all consecutive log statements that are less than a configurable level. This is controlled with new command line option '--tui-fold-level'. Also, there is a new 'Actions' button in the HTML which folds/unfolds all fold sections.
 - Fix sticky issue with topbar.
 - Pin requirements with pip-tools.
 
 ## [1.9.0] 2023-03-20
 - Added initial implementation for foldable HTML lines (see docstring on class TuiLogger in tui_logger.py for details). This feature is experimental.
 - Minor improvements to HTML report "About" page.
 
 ## [1.8.0] 2023-01-30
-- New command-line option `tui-reportfile', which allows user to specify the name of the HTML file produced when the console script `tuih` is run.
+- New command-line option `tui-reportfile`, which allows user to specify the name of the HTML file produced when the console script `tuih` is run.
 
 ## [1.7.2] 2023-01-29
 - Fixed Issue 94 (KeyError when user env has no JAVA_HOME).
 
 ## [1.7.1] 2023-01-28
 - Fixed Issue 84 (dataclass exception with Python 3.11).
 
@@ -35,15 +47,15 @@
 - Added duration to existing start and stop times for test session.
 - Changed look 'n' feel of About page in the HTML report (uses accordian buttons now).
 - Moved initalization of pytest-tui-specific Config object attributes from pytest-sessionstart to pytest_cmdline_main, as that method seems to be visited by the code earlier. This is to prevent AttributeError seen while testing latest build: "AttributeError: 'Config' object has no attribute '_tui_test_results'."
 - Internal implementation of pickling now uses a single file for TestReport and Section data. The pickled data is in the form of a dict, and also has some timedate info in it.
 - Tweaked and formatted a bunch of the tests in /demo-tests.
 ## [1.6.1] 2022-09-23
 
-- Added '*' .gitignore to ptt_files/ so that when people run pytest --tui in other directories they don't see the ptt_files/ dir.
+- Added '*' .gitignore to tui_files/ so that when people run pytest --tui in other directories they don't see the tui_files/ dir.
 
 ## [1.6.0] - 2022-09-20
 
 - Addressed issue 63:
   - Fixed tuih and tui console scripts not running
   - Removed autolaunch feature (TUI and HTML pages must now be launched by the user using 'tui' or 'tuih')
   - Removed config script 'tuiconf'
@@ -106,15 +118,15 @@
 
 ## [1.2.0] - 2022-08-19
 
 - Working/revamped HTML file output, with more modern look/feel.
 - Fixed tui1 (Textual) so that it works with new internal implementation.
 - Retiring tui2 (PyTermTk) for now.
 - Reordered/removed some menu items in tuiconf to fit new content/choices.
-- Changed output files folder to ./ptt_files.
+- Changed output files folder to ./tui_files.
 
 ## [1.1.3] - 2022-08-13
 
 - Fixed bug where if config file existed but was empty, an exception would occur on launching HTML file.
 
 ## [1.1.2] - 2022-08-10
```

### Comparing `pytest-tui-1.9.2/LICENSE` & `pytest-tui-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/PKG-INFO` & `pytest-tui-2.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,24 @@
-Metadata-Version: 2.1
-Name: pytest-tui
-Version: 1.9.2
-Summary: Text User Interface (TUI) and HTML report for Pytest test runs
-Home-page: https://github.com/jeffwright13/pytest-tui
-Author: Jeff Wright
-Author-email: jeff.washcloth@gmail.com
-License: MIT
-Keywords: pytest pytest-plugin testing tui textual html
-Classifier: Framework :: Pytest
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Testing
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Build Status](https://app.travis-ci.com/jsh/trendlist.svg?branch=master)](https://app.travis-ci.com/jsh/trendlist)
 [![Documentation Status](https://readthedocs.org/projects/trendlist/badge/?version=latest)](https://trendlist.readthedocs.io/en/latest/?badge=latest)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jsh/trendlist-notebooks/master)
 [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/jsh/trendlist)
 
 # pytest-tui
 ## A Pytest plugin for viewing test run results, with console scripts to launch a Text User Interface (TUI) or an HTML page
 
 ### TUI:
 ![2022-05-01 19 25 19](https://user-images.githubusercontent.com/4308435/166174159-b442a5b5-416d-42a0-badd-7401e9980e47.gif)
 
 ### HTML:
 ![2022-08-27 08 07 11](https://user-images.githubusercontent.com/4308435/187034046-312b1ee8-0f7b-49a1-994f-9c38a9d3941c.gif)
 
+### Log Folding:
+![2023-04-11 23 56 57](https://user-images.githubusercontent.com/4308435/231364763-132e8c35-cb61-4172-9686-176d84c038ca.gif)
+
 ## Introduction
 When you run Pytest campaigns that produce a lot of terminal output (e.g. with many tests, very detailed output, or with multiple failures), the standard Pytest output can make it difficult to examine the results. You end up scrolling way back in the terminal, looking for that one test you want to examine more closely. Pytest-tui provides a Text User Interface (TUI) and an HTML page that aim to make it easier to find the information you're looking for.
 
 Test results are categorized in the same way Pytest does it:
 
 - By outcome: `[Pass|Fail|Error|Skipped|Xpass|Xfail]`
 - By output section: `[Summary|Full|Errors|Passes|Failures|Warnings]`
@@ -44,15 +26,16 @@
 The intent it to make it easier for you to find the specific results you want so you can examine it without all the other results getting in your way.
 
 How does it work in practice? Easy. You just run your Pytest campaigns like you normally would, adding the command line option `--tui` (`pytest --tui`). Your test session will proceed as it always does (always in verbose mode), showing you the familiar terminal output while running. Then, at the end of the session, a TUI or an HTML page can be launched via the included console scripts (`tui` and/or `tuih`). The results are displayed on-screen or in-browser for you to examine. When you're done, just exit the TUI to go back to the terminal, or close the HTML page. Don't worry about losing your test session data. Results are stored to local disk and you can always relaunch the TUI or HTML page using those same console scripts.
 
 Output sections and individual test results are expandable/collapsible, and test summary statistics are displayed for convenience. Both the TUI and the HTML page retain the original pytest ANSI-encoded color output, lending a familiar look and feel.
 
 ## Features
-- **New** Log message folding on the HTML page, configurable by log level! See "Python Log Message Folding" section below.
+- **New** in 1.10.0 Regex-based folding on the HTML page, configurable by user-provided regex! See "Python Regex Folding" section below.
+- **New** in 1.9.1 Log message folding on the HTML page, configurable by log level. See "Python Log Message Folding" section below.
 - Launch either or both of the [Textual](https://github.com/Textualize/textual) TUI or the HTML page using built in console scripts
 - ANSI text markup support - whatever the output on your console looks like is how things are going to show up in the TUI
 - Mouse and keyboard support (including scrolling)
 - Support for all output formats/modes:
   - `-v`, `-vv`, `-no-header`, `--showlocals`, `--color=<yes|no|auto>`
   - all variants of `--tb` except "native"
   - "live-log" (aka log_cli)
@@ -84,15 +67,15 @@
 
 ### Running Your Tests
 
 Pretty much just run pytest like you always do, adding the `--tui` option to the list of command line options:
 
 `pytest --tui <whatever-else-you-normally-do>`
 
-In some environments, where the working directory for pytest has been changed from the default, it may be necessary to cd into the working directory in order to successfully launch the TUI or HTML. Basically, you need to be in the parent directory of wherever the `/ptt_files` folder has been placed by the plugin after a test run. This is a known issue and will be fixed at some point.
+In some environments, where the working directory for pytest has been changed from the default, it may be necessary to cd into the working directory in order to successfully launch the TUI or HTML. Basically, you need to be in the parent directory of wherever the `/tui_files` folder has been placed by the plugin after a test run. This is a known issue and will be fixed at some point.
 
 ### Sample / Demo Tests
 
 If you would like some dummy tests that will allow you to take pytest-tui for a testdrive, copy all the files at https://github.com/jeffwright13/pytest-tui/tree/main/demo-tests into a folder called `demo-tests/` where your test environment resides. You will need the additional libraries listed in /requirements/requirements-dev.txt, so install them (`pip install -r requirements-dev.txt`). Then:
 
 `pytest demo-tests/`
 
@@ -104,33 +87,42 @@
 
 On Linux terminals, you can typically press and hold the SHIFT key on your keyboard to temporarily bypass the TUI and access the terminal's native mouse copy/paste functionality (commonly, click-drag-release or double-click to select text, middle-click to paste). This copy/paste works with the terminal's selection buffer, as opposed to the TUI's buffer.
 
 On Windows, use the ALT key while click-dragging the mouse. Mac users can get the same effect with the Option key.
 
 ### Generating and viewing the HTML File
 
-The HTML output file is located at `<cwd>/ptt_files/html_report.html`. The HTML file is generated and launched via browser when the `tuih` script is invoked on the command line.
+The HTML output file is located at `<cwd>/tui_files/html_report.html`. The HTML file is automatically generated when a test run is completed with the "--tui" option. It can also be generated manually with the `tuih` script by invoking it on the command line.
+
+### Visibility
+
+Sometimes it can be difficult to read the terminal output when rendered on the HTML report. Pytest embeds ANSI color codes in its output, which are interpreted by a terminal program to display various colors for text. Pytest-tui takes these ANSI color codes and translates them to HTML (using the [ansi2html](https://pypi.org/project/ansi2html/) librray). Because the dhe default color scheme for the HTML report is a light background with dark text, it can be difficult to see some of the colors. To address this, there are three buttons that can help. The first ("Toggle Background") allow you to toggle the bakcground color of all console output. This should result in a page that closely resembles the output you would get in a standard terminal environment (assuming you have white text on a black background). The other two buttons, Invert Colors and Remove/Restore Colors, are a bit more drastic in that they affect all text in the report. Experiment and see what works for you. Also note that if you have your browser set to dark mode, or have a theme that changes the default color scheme, this can also affect the visibility of the text.
+### "Folding" output in the HTML report
 
-### Python Log Message Folding (HTML file)
+New in 1.11.0 is the integrated "folding" feature, which will automatically roll up any output lines from your test's output which match a regex (or regexes) specified in the file given on the command line. This option allows you to match on specific lines of console output from pytest, and 'fold' them (hide them).
 
-New in 1.9.1 is the "folding" feature, which will automatically roll up any output lines from the test run which are from the Python logger and which are at or below a configurable level. This lets you view verbose debug-level output when you need it, and fold it away, out of sight when you don't. There is no special configuration that has to be done to use this feature, other than enabling at run time with the `--tui-fold-level` option (see `pytest --help`). By default, this value is set to WARNING, in keeping with the default level of Python's logging module when creating a new logger.
+The folding feature is activated by passing the `--tui-regexfile` option (see `pytest --help`), and setting the path of a file containing the desired regex or regexes.
 
-This new feature produces a section in the HTML report file called "Folded Output", which displays the test run's console output with all lines of the configured log level folded up. Each folded section can be individually toggled opened/closed by clicking the "Folded WARNING" line (or whatever level you have configured). You can toggle all folded sections by clicking the "Fold/Unfold Logs" button inside the "Fold Actions" menu at the top right of the HTML page, and they can be hidden entirely by double-clicking the "Show/Hide Fold Markers" button.
+The file itself must contain plain text (UTF-8 encoded) with either a single regex, specified on a single line of the file; or two 'marker' patterns, specified in two consecutive lines of the file. If there is a single line in the file, that line is assumed to contain a regular expressoin that will cause the folding action to be used on any line in the console output of pytest if that line matches the regex. Consecutive lines that match will be folded into the same section. If there are two lines in the regex file, the first line is assumed to be a start marker, and the second line is assumed to be a stop marker. The folding action will be applied to all lines between the start and stop markers
 
+Ideas and tips for folding:
+- Run all tests with DEBUG level logging, but only view those DEBUG messages when necessary. I find this option particularly helpful when trying to debug a test that is only failing intermittently.
+- Mark certain sections of a test's output with a pair of start/end markers. If you have test output that is very chatty, but you only want to see it when you need to, this is a good option. For example, if you have a test that is making a bunch of API calls, and you want to see the output of those calls, but only when the test fails, you can mark the start and stop of the API calls with a pair of markers, and then fold them away when you don't need to see them.
+- Use the non-printable characters 'ZWS' and 'ZWJ' ((Zero Width Space)[https://en.wikipedia.org/wiki/Zero-width_space] / (Zero Width Joiner)[https://en.wikipedia.org/wiki/Zero-width_joiner]) as start and stop markers. The visual impact on the output is minimal (only inserts one visible space), and the regex pattern is very unlikely to match anything else in the output. The repo contains a file called `nonprintable_​​characters.txt` that contains cobinations of these characters, which can be used as a starting point for your own regexes.
 
 ## Known Limitations / Issues
 
 - Python support for 3.10+ is not guaranteed. Changes were made to the `importlib.metadata` library that are not backwards-compatible, and may result in exceptions when attempting to run. I have not had the chance to chase this down definitively, so until such a time that I fully understand the issue, I recommend using Python 3.8 or 3.9. Of course, YMMV...give it a try, and let me know how things go. :-)
 - User interfaces need work:
   - Overall layouts need optimization (I am definitely not a UX guy)
   - Textual interface may be sluggish, esp. if run within an IDE
   - All code here is like a sausage factory: pleasant enough, until you look inside - do so at your own peril!
 - Not fully tested with all combinations of output formats. Probably some use-cases where things won't work 100% right.
 - `pytest-tui` is currently incompatible with pytest command line option `--tb=native`, and will cause an INTERNALERROR if the two are used together.
-- HTML page cannot offer clickable links to local filesystem. This is one of the workflows I depend on when using iTerm2...traceback lines with a `file://` link to a locally-hosted resource are clickable, and open up my VSCode to that line in that file. Unfortunately, web browsers are much more security-minded than terminal apps, and actions like this are strictly disallowed.
+- HTML page cannot offer clickable links to local filesystem. This is one of the workflows I depend on when using iTerm2...traceback lines with a `file://` URL to a locally-hosted resource are clickable, and open up my IDE to that line in that file. Unfortunately, web browsers are much more security-minded than terminal apps, and actions like this are strictly disallowed.
 
 ## History
 
 This project was originally envisioned to only show test failures, and allow the user to 'fold' the details of the failed tests by clicking a line so that the details would alternately show/hide. In fact, the original repo was called `pytest-fold`. As development progressed, it became clear that what was really needed was a real TUI, one that organized the output in such a way that all of pytest's output was available in a more streamlined way.
 
 Several TUIs (using different TUI libraries) have been cycled through this project. The Textual interface is the only one currently supported, since some internal optimization has been done to make the results simpler to consume. However, other TUIs should be able to be integrated without too much work (e.g. Asciimatics, PyTermTk, pyermgui, etc.). Same would be true of a GUI. Contact the author if you have a desire to implement one of these. The results of any given testrun are collected and sorted in such a way that it should relatively simple to take them and put them into the presentation mode of choice.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest-tui-1.9.2/demo-tests/conftest.py` & `pytest-tui-2.0.0/demo-tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 import random
 
+
 data = [
     "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
     "Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
     (
         "Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut"
         " aliquip ex ea commodo consequat."
     ),
```

### Comparing `pytest-tui-1.9.2/demo-tests/test_0.py` & `pytest-tui-2.0.0/testing/pytester/examples/test_0.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/demo-tests/test_1.py` & `pytest-tui-2.0.0/demo-tests/test_1.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/demo-tests/test_2.py` & `pytest-tui-2.0.0/demo-tests/test_2.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/demo-tests/test_basic.py` & `pytest-tui-2.0.0/demo-tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/demo-tests/test_hoefling.py` & `pytest-tui-2.0.0/demo-tests/test_hoefling.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/demo-tests/test_rerun_random.py` & `pytest-tui-2.0.0/demo-tests/test_rerun_random.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/demo-tests/test_single_xpass_xfail.py` & `pytest-tui-2.0.0/demo-tests/test_single_xpass_xfail.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/demo-tests/test_warnings.py` & `pytest-tui-2.0.0/demo-tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/demo-tests/test_xpass_xfail.py` & `pytest-tui-2.0.0/demo-tests/test_xpass_xfail.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/misc/outcome_questions.txt` & `pytest-tui-2.0.0/misc/outcome_questions.txt`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/pytest_tui/__main__.py` & `pytest-tui-2.0.0/pytest_tui/stuff/__main__.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/pytest_tui/_tree_control.py` & `pytest-tui-2.0.0/pytest_tui/tree_control.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/pytest_tui/html_gen.py` & `pytest-tui-2.0.0/pytest_tui/html_gen.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,33 @@
+import argparse
+
 # import configparser
 import json
+import logging
 import re
 import webbrowser
 from datetime import datetime, timezone
 from pathlib import Path
+from typing import Dict, List, Tuple, Union
 
 import json2table
 from ansi2html import Ansi2HTMLConverter
+from strip_ansi import strip_ansi
 
 from pytest_tui import __version__
 from pytest_tui.utils import (
-    HTML_OUTPUT_FILE,
-    LOG_LEVEL_MAP,
+    DEFAULT_HTML_FILE,
     PYTEST_TUI_FILES_DIR,
     TERMINAL_OUTPUT_FILE,
-    TUI_FOLD_CONTENT_BEGIN,
-    TUI_FOLD_CONTENT_END,
-    TUI_FOLD_TITLE_BEGIN,
-    TUI_FOLD_TITLE_END,
     Results,
     test_session_starts_results_grabber,
 )
 
-# Next 3 lines are saved from earlier CLI-Config work
-# CLI CONFIG SAVED WORK
-# from pytest_tui.__main__ import Cli
-# from pytest_tui.utils import CONFIGFILE, HTML_OUTPUT_FILE, TERMINAL_OUTPUT_FILE, Results
-
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
 
 CSS_FILE = Path(__file__).parent / "resources" / "styles.css"
 JS_FILE = Path(__file__).parent / "resources" / "scripts.js"
 
 TAB_ABOUT = ["About"]
 TAB_ABOUT_COLOR = {"About": "hsl(199, 100%, 50%)"}
 TABS_RESULTS = [
@@ -120,19 +117,14 @@
             key: self.converter.convert(value, full=False)
             for key, value in self.fetch_raw_sections().items()
         }
 
 
 class HtmlPage:
     def __init__(self, results: Results):
-        # Read existing config from file, or apply default if not exist
-        # self.config_parser = configparser.ConfigParser()
-        # self.cli = Cli()
-        # self.cli.read_config_file()
-
         self.results = results
         self.tab_content = TabContent(results)
         self.fetched_sections_html = self.tab_content.fetch_sections_html()
         self.converter = Ansi2HTMLConverter()
 
     def remove_tabs_without_content(self):
         # Remove tabs for sections that do not contain any data.
@@ -169,15 +161,15 @@
                 self.results.tui_sections.lastline.content.replace("=", ""), full=False
             )
             + """</b></pre>"""
         )
 
     def create_final_test_summary(self) -> str:
         return (
-            """<button class="accordion">Final Test Summary  (click to expand)</button><div class="panel-closed"><p><pre>"""
+            """<button class="accordion-open">Final Test Summary  (click to expand)</button><div class="panel-open"><p><pre>"""
             + self.converter.convert(
                 self.results.tui_sections.short_test_summary.content, full=False
             )
             + "\n"
             + self.converter.convert(
                 self.results.tui_sections.lastline.content, full=False
             )
@@ -189,15 +181,15 @@
             test_session_starts_results_grabber,
             self.results.tui_sections.test_session_starts.content.encode(
                 "unicode_escape"
             ).decode(),
         )
         ripped = search.groups()[0].encode().decode("unicode-escape") if search else ""
         return (
-            """<button class="accordion">Live Test Session Summary  (click to expand)</button><div class="panel-closed"><p><pre>"""
+            """<button class="accordion-open">Live Test Session Summary  (click to expand)</button><div class="panel-open"><p><pre>"""
             + self.converter.convert(
                 self.results.tui_sections.lastline.content, full=False
             )
             + self.converter.convert(ripped, full=False)
             + self.converter.convert(
                 self.results.tui_sections.lastline.content, full=False
             )
@@ -227,22 +219,22 @@
             "This report generated": f"{now} UTC",
             "pytest-tui version": f"{__version__}",
         }
         dj = json2table.convert(
             d, build_direction="LEFT_TO_RIGHT", table_attributes=table_attributes
         )
         return (
-            """<button class="accordion">Test Execution Info</button><div class="panel-open"><p><pre>"""
+            """<button class="accordion-closed">Test Execution Info (click to expand)</button><div class="panel-closed"><p><pre>"""
             + dj
             + """</pre></p></div>"""
         )
 
     def create_environment_info(self, m, table_attributes) -> str:
         return (
-            """<button class="accordion">Environment</button><div class="panel-open"><p><pre>"""
+            """<button class="accordion-closed">Environment (click to expand)</button><div class="panel-closed"><p><pre>"""
             + json2table.convert(
                 m, build_direction="LEFT_TO_RIGHT", table_attributes=table_attributes
             )
             + """</pre></p></div>"""
         )
 
     def get_js(self) -> str:
@@ -280,54 +272,62 @@
             [
                 f"""<span><button class="dropdown-item tablinks" style="background-color: {TABS_SECTIONS_COLORS[section]}" onclick="openTab(event, '{section}')" >{section}</button></span>"""
                 for section in TABS_SECTIONS
             ]
         )
         tabs_links.extend(["""</span> </span>"""])
 
-        # Dropdown for fold-section actions
-        if self.results.tui_fold_level:
+        # Full Output tab
+        tabs_links.extend(
+            [
+                f"""<span><button class="tablinks" style="background-color: {TAB_FULL_OUTPUT_COLOR[section]}" onclick="openTab(event, '{section}')" >{section}</button></span>"""
+                for section in TAB_FULL_OUTPUT
+            ]
+        )
+
+        # This variable determines if the "Folded Output" tab and "Fold Actions" tabs are displayed or not
+        fold_visibility = "" if self.results.tui_regexfile else "display: none;"
+        if self.results.tui_regexfile:
             tabs_links.extend(
                 [
                     """<span class="dropdown"> <button class="dropbtn" style="color: brown; background-color: #d9ead3">Fold Actions</button> <span class="dropdown-content">"""
                 ]
             )
-
             tabs_links.extend(
                 [
-                    """<span><button class="dropdown-item tablinks" style="background-color: #a8b3dc" onclick="toggleAllDetails()">Fold/Unfold Logs</button> </span>"""
+                    """<span><button class="dropdown-item tablinks" style="background-color: #a8b3dc" onclick="toggleAllDetails()">Fold / Unfold</button> </span>"""
                 ]
             )
+            # tabs_links.extend(
+            #     [
+            #         """<span><button class="dropdown-item tablinks btn-rt" style="background-color: #b3dca8" id="toggle-details" onclick="toggleDetailsElements()">Hide / Show Fold Markers</button></span>"""
+            #     ]
+            # )
             tabs_links.extend(
                 [
-                    """<span><button class="dropdown-item tablinks btn-rt" style="background-color: #b3dca8" id="toggle-details" onclick="toggleDetailsElements()">Show/Hide Fold Markers</button></span>"""
+                    """<span><button class="dropdown-item tablinks btn-rt" style="background-color: #b3dca8" id="toggle-summary" onclick="toggleSummaryElements()">Hide / Show Fold Markers</button></span>"""
                 ]
             )
             tabs_links.extend(["""</span> </span>"""])
 
-        # Full Output tab
+        # The actual folded output content, tab "Folded Output" is just a container for this content
         tabs_links.extend(
             [
-                f"""<span><button class="tablinks" style="background-color: {TAB_FULL_OUTPUT_COLOR[section]}" onclick="openTab(event, '{section}')" >{section}</button></span>"""
-                for section in TAB_FULL_OUTPUT
+                f"""<span><button class="tablinks" style="{fold_visibility} background-color: {TAB_FOLDED_OUTPUT_COLOR[section]}" onclick="openTab(event, '{section}')" >{section}</button></span> </div>"""
+                for section in TAB_FOLDED_OUTPUT
             ]
         )
 
-        if self.results.tui_fold_level:
-            tabs_links.extend(
-                [
-                    f"""<span><button class="tablinks" style="background-color: {TAB_FOLDED_OUTPUT_COLOR[section]}" onclick="openTab(event, '{section}')" >{section}</button></span> </div>"""
-                    for section in TAB_FOLDED_OUTPUT
-                ]
-            )
-
+        # Stitch all the tabs together to be displayed at top of page
         tab_links_section = (
             """<span class="tab">""" + "".join(tabs_links) + """</span>"""
         )
 
+        # Build up content for each tab that shows a results category (Pass, Fail, etc.)
+        # Each results tab is populated with individual result content, each of which is collapsible
         tab_result_content = []
         for tab in TABS_RESULTS:
             if tab == "All Tests":
                 tab_result_content.append(
                     f"""<div id="{tab}" class="tabcontent"> {self.get_collapsible_results("tests")} </div>"""
                 )
             elif tab == "Reruns":
@@ -335,38 +335,42 @@
                     f"""<div id="{tab}" class="tabcontent"> {self.get_collapsible_results("reruns")} </div>"""
                 )
             else:
                 tab_result_content.append(
                     f"""<div id="{tab}" class="tabcontent"> {self.get_collapsible_results(tab.lower())} </div>"""
                 )
 
+        # Stitch all the results together to be displayed withint their individual category tabs
         tab_results = "".join(tab_result_content)
 
+        # Construct a single tab which drops down and displays individual Pytest output sections (e.g. "Summary", "Errors", etc.)
+        # This content comes ANSI-encoded, so it needs to be converted to HTML for proper display
         tab_section_content = [
             f"""<div id="{section}" class="tabcontent"> <pre>{self.converter.convert(self.tab_content.tabs[section], full=False) or ""}</pre> </div>"""
             for section in TABS_SECTIONS
             if self.tab_content.tabs[section]
         ]
         tab_sections = "".join(tab_section_content)
 
+        # The "About" tab (metadata, etc for this test run)
         tab_about = f"""<div id="{TAB_ABOUT[0]}" class="tabcontent"> <p>{self.get_metadata()}</p> </div>"""
 
+        # The "Full Output" tab (all output from the test run), as it occured chronologically on the console
         tab_full_output = f"""<div id="{TAB_FULL_OUTPUT[0]}" class="tabcontent"> <pre>{self.get_terminal_output()}</pre> </div>"""
 
-        if self.results.tui_fold_level:
-            tab_folded_output = f"""<span id="{TAB_FOLDED_OUTPUT[0]}" class="tabcontent"> <pre>{self.fold_terminal_output(self.results.tui_fold_level)}</pre> </span>"""
-        else:
-            tab_folded_output = ""
+        # Folded Output tab; always generated but only displayed if self.results.tui_regexfile is True
+        # (i.e. if the user provided a regex file)
+        tab_folded_output = f"""<span id="{TAB_FOLDED_OUTPUT[0]}" class="tabcontent"> <pre>{self.fold_terminal_output_by_regex()}</pre> </span>"""
 
         return (
             tab_links_section
             + tab_about
             + tab_results
-            + tab_sections
             + tab_full_output
+            + tab_sections
             + tab_folded_output
         )
 
     def get_collapsible_results(self, outcome) -> str:
         collapsible_results = ""
         if outcome == "reruns":
             results = []
@@ -403,97 +407,145 @@
             "border": "ridge",
             "style": "width:auto%; table-layout: auto;",
             "border-collapse": "collapse",
             "text-align": "left",
             "tr": "nth-child(even) {background-color: #f2f2f2;}",
         }
 
+        # tab_color_button =  """<rainbow-button onclick="removeColor()">Remove color</rainbow-button>"""
+        # tab_color_button =  """<button class=button-43 onclick="removeColor(); this.style.display = 'none'">Remove Color</button>"""
+        tab_color_button = """<button class="button-43" onclick="removeOrRestoreColor()">Remove / Restore Colors</button>"""
+        tab_invert_button = """<button class=button-43 onclick="invertColors()">Invert Colors</button>"""
+        # tab_toggle_background_button = """<button class=button-43 onclick="togglePreBackground()">Toggle Background</button>"""
+        tab_toggle_background_button = """<button class="button-43" onclick="togglePreBackground()">Toggle Background</button>"""
+
         return (
             "<hr>"
             + f"{self.create_final_test_summary()}<hr>"
             + f"{self.create_live_test_session_summary()}<hr>"
             + f"{self.create_test_execution_info()}<hr>"
-            + f"{self.create_environment_info(m, table_attributes)}"
+            + f"{self.create_environment_info(m, table_attributes)}<hr>"
+            + tab_color_button
+            + "<hr>"
+            + tab_invert_button
+            + "<hr>"
+            + tab_toggle_background_button
         )
 
     def get_terminal_output(self) -> str:
         with open(TERMINAL_OUTPUT_FILE, "rb") as f:
             tout = str(f.read(), "utf-8")
         return self.converter.convert(tout, full=False)
 
     def get_terminal_output_ansi(self) -> str:
         with open(TERMINAL_OUTPUT_FILE, "rb") as f:
             tout = str(f.read(), "utf-8")
         return tout
 
-    def get_line_level(self, line: str) -> str:
-        """Is this line a log entry (DEBUG, INFO, WARNING, ERROR, CRITICAL)?"""
-        for level, value in LOG_LEVEL_MAP.items():
-            if level in line:
-                return value
+    def get_regex(self, tui_regexfile: Path) -> List[str]:
+        """Read regex file and return list of regexes"""
+        try:
+            with open(tui_regexfile, "r") as file:
+                # lines = [ast.literal_eval(line) for line in file.readlines() if line]
+                lines = [eval(line) for line in file.readlines() if line]
+                return [line.rstrip() for line in lines if line]
+        except FileNotFoundError as e:
+            logger.error(
+                f"Regex file not found: {tui_regexfile}. Proceeding with folding"
+                " feature disabled."
+            )
+            return []
 
-    def fold_log_lines(self, lines: list, level: str) -> str:
+    def fold_regex_lines(self, lines: List[str]) -> str:
         """
-        Search each line of console output and look for a log level indicator (DEBUG, INFO, WARNING, ERROR, CRITICAL).
-        If a line contains a log level indicator, check if log level is <= the level passed to the function.
-        If the log level is <= the level passed to the function, then the line is folded.
-        If the log level is > than the level passed to the function, then the line is not folded.
+        Refactored code
+        Search each line of console output and look for a regex match,
+        using the regex patterns defined in file TODO.
+        If a line contains a match for the regex patterrn, the line
+        will be folded. Consecutive lines that match regex are grouped
+        together wihin the same fold.
         """
-        html_lines = []
+        converter = Ansi2HTMLConverter()
         html_str = ""
         fold_started = False
-        for l in lines:
-            line = self.converter.convert(l, full=False)
-            this_line_log_level = self.get_line_level(l)
-            if this_line_log_level:
-                if this_line_log_level <= LOG_LEVEL_MAP[level]:
+        regexes = self.get_regex(self.results.tui_regexfile)
+
+        if len(regexes) == 1:
+            # If there is only one regex pattern, use it to fold any line that matches
+            regex = regexes[0]
+            for line in lines:
+                line_stripped = strip_ansi(line)
+                line_converted = converter.convert(line, full=False)
+                match = re.search(regex, line_stripped)
+
+                if match:
                     if not fold_started:
+                        fold_started = True
                         html_str += (
-                            f"<details><summary style='nobr'>Folded {level}</summary>"
+                            "<details><summary style='nobr'>Folded RegEx:"
+                            f" '{regex}'</summary>"
                         )
-                        fold_started = True
-                else:
-                    if fold_started:
-                        html_str += "</details>"
-                        fold_started = False
-                html_str += line + "\n"
-            else:
-                if fold_started:
+                    html_str += line_converted + "\n"
+                elif fold_started:
+                    fold_started = False
                     html_str += "</details>"
+                    html_str += line_converted + "\n"
+                else:
+                    html_str += line_converted + "\n"
+
+        if len(regexes) >= 2:
+            # With 2 regexes, the first is the 'starter' regex and the second is the 'ender' regex
+            regex_starter = regexes[0]
+            regex_ender = regexes[1]
+            for line in lines:
+                line_stripped = strip_ansi(line)
+                line_converted = converter.convert(line, full=False)
+                match_starter = re.search(regex_starter, line_stripped)
+                match_ender = re.search(regex_ender, line_stripped)
+
+                if match_starter:
+                    if not fold_started:
+                        fold_started = True
+                        html_str += (
+                            "<details><summary style='nobr'>Folded RegEx:"
+                            f" '{regex_starter}'</summary>"
+                        )
+                    html_str += line_converted + "\n"
+                elif match_ender:
                     fold_started = False
-                    html_str += line + "\n"
+                    html_str += "</details>"
+                    html_str += line_converted + "\n"
+                elif fold_started:
+                    html_str += line_converted + "\n"
                 else:
-                    html_str += line + "\n"
+                    html_str += line_converted + "\n"
+
         return html_str
 
-    def fold_terminal_output(self, level: str) -> str:
+    def fold_terminal_output_by_regex(self) -> Union[str, None]:
         terminal_output_ansi = self.get_terminal_output_ansi()
         lines = terminal_output_ansi.splitlines()
-        return self.fold_log_lines(lines, level)
+        return self.fold_regex_lines(lines) if self.results.tui_regexfile else None
+
+    def create_output_file(self, html_outfile: Path, html_out: str) -> None:
+        assert isinstance(html_outfile, Path), "html_outfile must be a Path object"
+        html_outfile.parent.mkdir(parents=True, exist_ok=True)
+        with html_outfile.open("w") as f:
+            f.write(html_out)
+        logger.info(f"HTML report generated: {html_outfile}")
 
 
 def main():
     results = Results()
     page = HtmlPage(results)
     page.remove_tabs_without_content()
     html_header = page.create_header()
     html_tabs = page.create_tabs()
     html_trailer = page.create_trailer()
     html_out = html_header + html_tabs + html_trailer
 
-    global HTML_OUTPUT_FILE
-    if results.tui_test_info.get("tui_htmlfile"):
-        HTML_OUTPUT_FILE = Path(
-            PYTEST_TUI_FILES_DIR / results.tui_test_info["tui_htmlfile"]
-        )
-    with open(HTML_OUTPUT_FILE, "w+") as f:
-        f.write(html_out)
-    webbrowser.open(f"file://{HTML_OUTPUT_FILE._str}")
-
-    # Open in browser if autolaunch_html config is set
-    # page.cli.read_config_file()
-    # if page.cli.html_autolaunch:
-    #     webbrowser.open(f"file://{HTML_OUTPUT_FILE._str}")
+    html_outfile = Path(results.tui_test_info.get("tui_htmlfile", DEFAULT_HTML_FILE))
+    page.create_output_file(html_outfile, html_out)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pytest-tui-1.9.2/pytest_tui/log_experiments/debug_context.py` & `pytest-tui-2.0.0/pytest_tui/log_experiments/debug_context.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/pytest_tui/log_experiments/debug_html_logger.py` & `pytest-tui-2.0.0/pytest_tui/log_experiments/debug_html_logger.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/pytest_tui/log_experiments/foldable_loggers.py` & `pytest-tui-2.0.0/pytest_tui/log_experiments/foldable_loggers.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/pytest_tui/log_experiments/test_debug_logger_html.py` & `pytest-tui-2.0.0/pytest_tui/log_experiments/test_debug_logger_html.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/pytest_tui/log_experiments/test_me.py` & `pytest-tui-2.0.0/pytest_tui/log_experiments/test_me.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/pytest_tui/log_experiments/tui_logger.py` & `pytest-tui-2.0.0/pytest_tui/log_experiments/tui_logger.py`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/pytest_tui/plugin.py` & `pytest-tui-2.0.0/pytest_tui/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import itertools
-import logging
 import pickle
 import re
 import tempfile
+import traceback
 from concurrent.futures.thread import ThreadPoolExecutor
 from datetime import datetime, timezone
 from io import StringIO
+from pathlib import Path
 from types import SimpleNamespace
 from typing import List
 
 import pytest
 from _pytest._io.terminalwriter import TerminalWriter
 from _pytest.config import Config, create_terminal_writer
+from _pytest.config.argparsing import Parser
 from _pytest.nodes import Item
 from _pytest.reports import TestReport
 from strip_ansi import strip_ansi
 
-# from pytest_tui.__main__ import tui_launch
-from pytest_tui.html_gen import main as tuihtml
-from pytest_tui.utils import (
-    HTML_OUTPUT_FILE,
+from pytest_tui.html_gen import main as tuih
+from pytest_tui.utils import (  # HTML_OUTPUT_FILE,
     TERMINAL_OUTPUT_FILE,
     TUI_RESULTS_FILE,
     TuiRerunTestGroup,
     TuiSection,
     TuiSections,
     TuiTestResult,
     TuiTestResults,
@@ -42,40 +42,88 @@
 # Don't collect tests from any of these files
 collect_ignore = [
     "setup.py",
     "plugin.py",
 ]
 
 
-def pytest_addoption(parser) -> None:
+def pytest_addoption(parser: Parser) -> None:
+    # Add options to the Pytest command line parser.
     group = parser.getgroup("tui")
     group.addoption(
         "--tui",
         action="store_true",
+        dest="_tui",
+        default=None,
         help=(
             "Enable the pytest-tui plugin. Both text user interface (TUI) and HTML"
-            " output are supported.\nRun TUI with console command 'tui'; run HTML"
-            " report with 'tuih'."
+            " output are supported. Run TUI with console command 'tui' ('q' to quit)."
+            " Create HTML report with 'tuih'. Also see option '--tui-html'."
         ),
     )
     group.addoption(
         "--tui-htmlfile",
+        action="store",
+        dest="_tui_htmlfile",
+        nargs="?",
+        # type=argparse.FileType("w"),
+        default=Path(f"{Path.cwd()}/tui_files/html_report.html"),
+        const=Path(f"{Path.cwd()}/tui_files/html_report.html"),
         help=(
-            "Specify a non-default name for the HTML report file. Default is"
-            " 'html-report.html,' and will be placed in the ptt_files/ folder."
+            "Specify a non-default name for the HTML report file. Can be a relative or"
+            " absolute pathname, using your operating system's standard format. Default"
+            " is 'html-report.html' in the 'tui_files/' directory under the cwd."
+            " If you specify a relative pathname, it will be relative to the cwd."
         ),
     )
+    # TODO
+    # parser.addini("tui_html", help="Specify a non-default name for the HTML report file", type=argparse.FileType('w'), default=Path(f"{Path.cwd()}/tui_files/html_report.html"))
+
+    # TODO: clean up HELP strings
     group.addoption(
-        "--tui-fold-level",
+        "--tui-regexfile",
+        action="store",
+        dest="_tui_regexfile",
+        nargs="?",
+        default=None,
+        const=Path(f"{Path.cwd()}/tui_regexfile.txt"),
         help=(
-            "Enable auto-folding of log messages in the HTML report, and specify the"
-            " level at which folding occurs. When enabled, log messages at or below the"
-            " specified level will be folded."
+            "Enable folding in the HTML report for console output lines that match the"
+            " regex given by the specified TUI_REGEXFILE file (default:"
+            " cwd()/tui_regexfile.txt). TUI_REGEXFILE specifies one or more Python"
+            " regular expressions, including quotes. It can be either a file or a"
+            " string literal. If it is a file, it has one or more Python regular"
+            " expressions, one per line (quoted). If it is a string literal, it has one"
+            " or more Python regular expressions, separated by semicolons (each"
+            " quoted). See README for more information:"
+            " https://github.com/jeffwright13/pytest-tui/blob/main/README.md."
         ),
     )
+    # TODO
+    # parse.FileType('w'), default=None, const=Path(f"{Path.cwd()}/tui_regexfile.txt"))
+
+    # Add options for pytest.ini
+    parser.addini(
+        "tui",
+        type="bool",
+        help="Enable the TUI plugin",
+        default=False,
+    )
+    parser.addini(
+        "tui_htmlfile",
+        type="string",
+        help="Path to the HTML report file generated by the TUI plugin",
+        default=str(Path(f"{Path.cwd()}/tui_files/html_report.html")),
+    )
+    parser.addini(
+        "tui_regexfile",
+        type="string",
+        help="Path to a regex file for the TUI plugin's 'folding' feature",
+        default=None,
+    )
 
 
 def add_ansi_to_report(config: Config, report: TestReport) -> None:
     """
     If the report has longreprtext (traceback info), mark it up with ANSI codes
     From https://stackoverflow.com/questions/71846269/algorithm-for-extracting-first-and-last-lines-from-sectionalized-output-file
     """
@@ -99,25 +147,26 @@
 
 
 def pytest_sessionstart(session: pytest.Session) -> None:
     pass
 
 
 def pytest_cmdline_main(config: Config) -> None:
-    # Set up the TUI-specific attributes on the config object:
-    # Verbose (easier parsing of final test results)
-    # Reportchars =RA (all test results, plus Reruns)
-    if hasattr(config.option, "tui"):
-        if config.option.tui:
-            config.option.verbose = 1
-            config.option.reportchars = "A"
+    # If the tiui option is enabled, put the TUI plugin in verbose mode,
+    # and force all test results to be reported, including reruns.
+    # Verbose (makes final outcome classification possible)
+    # Reportchars =RA (forces All test results, plus Reruns)
+    if hasattr(config.option, "_tui") and config.option._tui:
+        config.option.verbose = 1
+        config.option.reportchars = "A"
         if hasattr(config.option, "reruns"):
-            config.option.reportchars = "AR"
+            config.option.reportchars += "R"
 
-    # Initialize TUI-specific attributes on the config object:
+    # Using global Config object to store TUI-specific attributes.
+    # TODO: port to Stash.
     config._tui_session_start_time = (
         datetime.now(timezone.utc).replace(microsecond=0).strftime("%Y-%m-%d %H:%M:%S")
     )
     if not hasattr(config, "_tui_sessionstart"):
         config._tui_sessionstart = True
     if not hasattr(config, "_tui_sessionstart_test_outcome_next"):
         config._tui_sessionstart_test_outcome_next = False
@@ -144,45 +193,19 @@
             passes=TuiSection(name="passes", content=""),
             warnings_summary=TuiSection(name="warnings_summary", content=""),
             rerun_test_summary=TuiSection(name="rerun_test_summary", content=""),
             short_test_summary=TuiSection(name="short_test_summary", content=""),
             lastline=TuiSection(name="lastline", content=""),
         )
 
-    # Override default HTML report file name, if specified on the command line
-    if (
-        hasattr(config.option, "tui_htmlfile")
-        and not config.option.tui_htmlfile
-        or not hasattr(config.option, "tui_htmlfile")
-    ):
-        config._tui_htmlfile = HTML_OUTPUT_FILE
-    else:
-        config._tui_htmlfile = config.option.tui_htmlfile
-
-    # Set default fold level, if specified on the command line
-    if (
-        hasattr(config.option, "tui_fold_level")
-        and not config.option.tui_fold_level
-        or not hasattr(config.option, "tui_fold_level")
-    ):
-        config._tui_fold_level = "WARNING"
-    else:
-        config._tui_fold_level = (
-            config.option.tui_fold_level
-            if config.option.tui_fold_level.lower()
-            in ["debug", "info", "warning", "error", "critical"]
-            else "WARNING"
-        )
-
 
 def pytest_report_teststatus(report: TestReport, config: Config) -> None:
-    # Don't process any TUI-specific code if the plugin is not enabled
-    if not hasattr(config.option, "tui"):
+    if not hasattr(config.option, "_tui"):
         return
-    if not config.option.tui:
+    if not config.option._tui:
         return
 
     if hasattr(report, "caplog") and report.caplog:
         for tui_test_result in config._tui_test_results.test_results:
             if tui_test_result.fqtn == report.nodeid:
                 tui_test_result.caplog = report.caplog
 
@@ -204,15 +227,15 @@
 
     config._tui_reports.append(report)
 
 
 def timestamp_result(config: Config, item: Item) -> None:
     if not hasattr(item.config.option, "tui"):
         return
-    if not item.config.option.tui:
+    if not item.config.option._tui:
         return
 
     now = datetime.now()
     now_str = now.strftime("%Y-%m-%d %H:%M:%S.%f")
     for tui_test_result in item.config._tui_test_results.test_results:
         if tui_test_result.fqtn == item.nodeid and not tui_test_result.start_time:
             tui_test_result.start_time = now_str
@@ -231,22 +254,21 @@
 @pytest.hookimpl()
 def pytest_runtest_teardown(item):
     timestamp_result(item.config, item)
 
 
 @pytest.hookimpl(trylast=True)
 def pytest_configure(config: Config) -> None:
-    # Don't process any TUI-specific code if the plugin is not enabled
-    if not hasattr(config.option, "tui"):
+    if not hasattr(config.option, "_tui"):
         return
-    if not config.option.tui:
+    if not config.option._tui:
         return
 
     # Examine Pytest terminal output to mark different sections of the output.
-    # This code is based on code in pytest's 'pastebin.py'.
+    # This code is based on pytest's 'pastebin.py'.
     tr = config.pluginmanager.getplugin("terminalreporter")
     if tr is not None:
         # Save the old terminal writer instance so we can restore it later
         oldwrite = tr._tw.write
 
         # identify and mark each results section
         def tee_write(s, **kwargs):
@@ -355,22 +377,20 @@
                     group.final_test = test_result
     for group in rerun_test_groups:
         group.full_test_list = group.forerunners + [group.final_test]
     return rerun_test_groups
 
 
 def pytest_unconfigure(config: Config) -> None:
-    # Don't process any TUI-specific code if the plugin is not enabled
-    if not hasattr(config.option, "tui"):
+    if not hasattr(config.option, "_tui"):
         return
-    if not config.option.tui:
+    if not config.option._tui:
         return
 
     config._tui_rerun_test_groups = populate_rerun_groups(config)
-
     config._tui_session_end_time = (
         datetime.now(timezone.utc).replace(microsecond=0).strftime("%Y-%m-%d %H:%M:%S")
     )
     config._tui_session_duration = datetime.strptime(
         config._tui_session_end_time, "%Y-%m-%d %H:%M:%S"
     ) - datetime.strptime(config._tui_session_start_time, "%Y-%m-%d %H:%M:%S")
 
@@ -380,23 +400,25 @@
     ):
         if test_report.nodeid == tui_test_result.fqtn:
             tui_test_result.duration += test_report.duration
 
     # Assume any test that was not categorized earlier with an outcome is a Skipped test.
     # JUSTIFICATION:
     # Pytest displays Skipped tests in a different format than all other test categories in the
-    # "=== short test summary info ===" section, truncating their fqtns and appending a line number
+    # "== short test summary info ==" section, truncating their fqtns and appending a line number
     # instead of specifying their test names. This plugin identifies all other test categories
     # (passed, failed, errors, etc.) and populates their fqtns and outcomes with the appropriate
     # values, leaving open one other possibility (Skipped).
     for tui_test_result in config._tui_test_results.test_results:
         if tui_test_result.outcome == "":
             tui_test_result.outcome = "SKIPPED"
 
-    config.pluginmanager.getplugin("terminalreporter")  # <= ???
+    config.pluginmanager.getplugin(
+        "terminalreporter"
+    )  # <= ???  does not appear to be used
 
     # Rewind the temp file containing all the raw ANSI lines sent to the terminal;
     # read its contents;  then close it. Then, write info to file.
     config._tui_terminal_out.seek(0)
     terminal_out = config._tui_terminal_out.read()
     config._tui_terminal_out.close()
     with open(TERMINAL_OUTPUT_FILE, "wb") as file:
@@ -407,30 +429,36 @@
             {
                 "session_start_time": config._tui_session_start_time,
                 "session_end_time": config._tui_session_end_time,
                 "session_duration": config._tui_session_duration,
                 "tui_test_results": config._tui_test_results,
                 "tui_rerun_test_groups": config._tui_rerun_test_groups,
                 "tui_sections": config._tui_sections,
-                "tui_htmlfile": config._tui_htmlfile,
-                "tui_fold_level": config._tui_fold_level,
+                "tui_htmlfile": config.option._tui_htmlfile,
+                "tui_regexfile": config.option._tui_regexfile,
             },
             file,
         )
     pytui_launch(config)
 
 
 def pytui_launch(config: Config) -> None:
     """
-    Final code invocation after Pytest run has completed.
+    Final code invocation after Pytest run has completed; creates HTML report
+    and optionall launches TUI.
     """
     try:
         # disable capturing while TUI runs to avoid error `redirected stdin is pseudofile, has
         # no fileno()`; adapted from https://githubmemory.com/repo/jsbueno/terminedia/issues/25
         capmanager = config.pluginmanager.getplugin("capturemanager")
         capmanager.suspend_global_capture(in_=True)
     finally:
         # re-enable capturing
-        with ThreadPoolExecutor() as executor:
-            executor.submit(tuihtml)
-        # tui_launch()
+        try:
+            with ThreadPoolExecutor() as executor:
+                future = executor.submit(tuih)
+                result = future.result()
+        except Exception as e:
+            traceback_str = traceback.format_exc()
+            print(f"Exception in worker thread while running tuih() function: {e}")
+            print(f"Traceback: {traceback_str}")
         capmanager.resume_global_capture()
```

### Comparing `pytest-tui-1.9.2/pytest_tui/resources/styles.css` & `pytest-tui-2.0.0/pytest_tui/resources/styles.css`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,19 @@
 }
 
 div.sticky {
      position: -webkit-sticky;
      position: sticky;
      top: 0;
 }
- pre, .pre {
+.pre-bg-black {
+    background-color: black;
+    color: white;
+  }
+pre, .pre {
      display: block;
      font-family: monospace;
      white-space: pre-wrap;
      margin: 4px 0;
      overflow: auto overflow-wrap: break-word;
      word-break: break-all;
      word-wrap: break-word;
@@ -98,78 +102,82 @@
      border-radius: 4px;
      outline: none;
      cursor: pointer;
      padding: 14px 16px;
      transition: 0.3s;
      font-size: 15px
 }
- .tab button:hover {
-     background-color: #ddd;
-     opacity: 1.0;
-     transition: 0.3s;
-}
- .tab button.focus {
-     background-color: #ccc;
-     opacity: 1.0;
-     transition: 0.3s;
-}
  .tab button.active {
      opacity: 1.0;
      transition: 0.3s;
 }
  .tablinks {
      font-family: "Arial", sans-serif;
      font-size: 15px opacity: 1.0;
 }
- .tabcontent {
+.tablinks.hidden {
+    display: none;
+}
+.tabcontent {
      background-color: #ddd;
      display: none;
      border: 1px solid #ccc;
      border-top: none;
      -webkit-animation: fadeEffect 1s;
      animation: fadeEffect .25s;
 }
 /* Style the buttons that are used to open and close the accordion panel */
- .accordion {
+ .accordion-open, .accordion-closed {
      background-color: #ddd;
      font-weight: bold;
+     font-size: 14px;
      color: #222;
      cursor: pointer;
      padding: 16px;
      width: 100%;
      text-align: left;
      border: none;
      outline: none;
-     transition: 0.4s;
+     transition: 0.3s;
 }
 .button-43 {
-    background-image: linear-gradient(-180deg, #37AEE2 0%, #1E96C8 100%);
     border-radius: .5rem;
     box-sizing: border-box;
-    color: #FFFFFF;
+    font-weight: bold;
+    color: #222;
+    background-color: #ddd;
     display: flex;
-    font-size: 16px;
+    font-size: 14px;
     justify-content: center;
-    padding: 1rem 1.75rem;
+    padding: 16px;
     text-decoration: none;
-    width: 100%;
     border: 0;
     cursor: pointer;
     user-select: none;
     -webkit-user-select: none;
     touch-action: manipulation;
-}
-.button-43:hover {
-    background-image: linear-gradient(-180deg, #1D95C9 0%, #17759C 100%);
-}
-@media (min-width: 768px) {
-  .button-43 {
-    padding: 1rem 2rem;
   }
-}
+
+  .button-43:hover {
+    background-color: #ccc;
+    opacity: 1.0;
+    transition: 0.3s;
+  }
+
+  .button-43:focus {
+    background-color: #ccc;
+    opacity: 1.0;
+    transition: 0.3s;
+  }
+
+  @media (min-width: 768px) {
+    .button-43 {
+      padding: 16px;
+    }
+  }
 summary {
     font-size: 12px;
     font-weight: bold;
     color: #000;
     animation: pulsate 1.6s ease-out infinite;
 }
 @keyframes pulsate {
@@ -184,25 +192,26 @@
     100% {
       color: #0000;
       text: 8px 8px 12px #000;
     }
 }
 /* Add background color to the button if it is clicked (add the .active class */
 /* with JS), and when you move the mouse over it (hover) */
- .active, .accordion:hover {
+ .active, .accordion-open:hover, .accordion-closed:hover {
      background-color: #ccc;
 }
 /* Style the accordion panel. Note: hidden by default */
- .panel-open {
-     max-height: 100%;
+ .panel-closed {
+     /* max-height: 100%; */
+     max-height: 0;
      padding: 0 16px;
      background-color: #ddd;
-     /* display: none; */
+     /* /* display: none; */
      overflow: hidden;
-     transition: max-height 0.2s ease-out;
+     transition: max-height 0.3s ease-out;
 }
  @-webkit-keyframes fadeEffect {
      from {
         opacity: 0;
     }
      to {
         opacity: .5;
@@ -212,21 +221,21 @@
      from {
         opacity: 0;
     }
      to {
         opacity: 1.5;
     }
 }
-.panel-closed {
+.panel-open {
     max-height: 100%;
     padding: 0 16px;
     background-color: #ccc;
     display: none;
     overflow: hidden;
-    transition: max-height 0.2s ease-out;
+    transition: max-height 0.3s ease-out;
 }
 @-webkit-keyframes fadeEffect {
     from {
        opacity: 0;
    }
     to {
        opacity: .5;
@@ -272,15 +281,40 @@
      display: inline-block;
 }
  .line{
      background-color:black;
      height:auto;
      width:5px;
 }
- p {
+
+@keyframes rainbow {
+    0% {background: red;}
+    14% {background: orange;}
+    28% {background: yellow;}
+    42% {background: green;}
+    57% {background: blue;}
+    71% {background: indigo;}
+    85% {background: violet;}
+    100% {background: red;}
+}
+
+rainbow-button {
+    color: white;
+    border: none;
+    padding: 10px 20px;
+    animation: rainbow 4s linear infinite;
+    cursor: pointer;
+}
+
+body.invert-colors {
+    filter: invert(100%);
+    background: #000; /* Add this if you want a black background */
+}
+
+p {
      font-size: 14px;
      font-family: "Arial", sans-serif;
 }
  h1, h2, h3, h4, h5, h6 {
      font-family: "Arial", sans-serif;
 }
  table, th, td {
```

### Comparing `pytest-tui-1.9.2/pytest_tui/stuff/devnotes.md` & `pytest-tui-2.0.0/pytest_tui/stuff/devnotes.md`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/pytest_tui/stuff/nonprintable_​​characters.md` & `pytest-tui-2.0.0/pytest_tui/stuff/nonprintable_​​characters.md`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/pytest_tui/tui_gen.py` & `pytest-tui-2.0.0/pytest_tui/tui_gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from rich.panel import Panel
 from rich.text import Text
 from textual import events
 from textual.app import App
 from textual.widget import Widget
 from textual.widgets import ScrollView, TreeClick
 
-from pytest_tui._tree_control import TreeControl
+from pytest_tui.tree_control import TreeControl
 from pytest_tui.utils import Results
 
 TREE_WIDTH = 120
 SECTIONS = {
     "PASSES": "bold green underline",
     "FAILURES": "bold red underline",
     "ERRORS": "bold magenta underline",
```

### Comparing `pytest-tui-1.9.2/pytest_tui/utils.py` & `pytest-tui-2.0.0/pytest_tui/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,27 @@
+import ast
 import pickle
 import re
 from dataclasses import dataclass, field
 from datetime import datetime
 from pathlib import Path
 from typing import List
 
 # Files generated by plugin.py
-PYTEST_TUI_FILES_DIR = Path.cwd().resolve() / "ptt_files"
+PYTEST_TUI_FILES_DIR = Path.cwd().resolve() / "tui_files"
 PYTEST_TUI_FILES_DIR.mkdir(exist_ok=True)
-HTML_OUTPUT_FILE = PYTEST_TUI_FILES_DIR / "html_report.html"
+# HTML_OUTPUT_FILE = PYTEST_TUI_FILES_DIR / "html_report.html"
 # Path(HTML_OUTPUT_FILE).touch(exist_ok=True)
 # CONFIGFILE = PYTEST_TUI_FILES_DIR / "config.ini"
 # Path(CONFIGFILE).touch(exist_ok=True)
 TUI_RESULTS_FILE = PYTEST_TUI_FILES_DIR / "tui_results.pickle"
 TUI_RESULT_OBJECTS_FILE = PYTEST_TUI_FILES_DIR / "tui_result_objects.pickle"
 TUI_SECTIONS_FILE = PYTEST_TUI_FILES_DIR / "tui_sections.pickle"
 TERMINAL_OUTPUT_FILE = PYTEST_TUI_FILES_DIR / "terminal_output.ansi"
-
-LOG_LEVEL_MAP = {
-    "DEBUG": 10,
-    "INFO": 20,
-    "WARNING": 30,
-    "ERROR": 40,
-    "CRITICAL": 50,
-}
-
-
-# ZWNJ = "\u200C"
-# ZWS = "\u200B"
-# BOM = "\uFEFF"
-# ZWJ = "\u200D"
-
-
-TUI_FOLD_CONTENT_BEGIN = r"​​​"
-TUI_FOLD_TITLE_BEGIN = r"‌‌‌"
-TUI_FOLD_CONTENT_END = r"‍‍‍"
-TUI_FOLD_TITLE_END = r"   "
-
-# TUI_FOLD_TITLE_BEGIN = "~~tui_fold_title_begin~~"
-# TUI_FOLD_TITLE_END = "~~tui_fold_title_end~~"
-# TUI_FOLD_CONTENT_BEGIN = "~~tui_fold_content_begin~~"
-# TUI_FOLD_CONTENT_END = "~~tui_fold_content_end~~"
-
-# tui_fold_matcher = re.compile(r"^~~tui_")
-# TUI_FOLD_TITLE_BEGIN = "~~tui_fold_title_begin~~"
-# TUI_FOLD_TITLE_END = "~~tui_fold_title_end~~"
-# TUI_FOLD_CONTENT_BEGIN = "~~tui_fold_content_begin~~"
-# TUI_FOLD_CONTENT_END = "~~tui_fold_content_end~~"
+DEFAULT_HTML_FILE = PYTEST_TUI_FILES_DIR / "html_report.html"
 
 # regex matching patterns for Pytest sections
 # live_log_sessionstart_matcher = re.compile(r"^==.*\s live log sessionstart\s==+")
 test_session_starts_matcher = re.compile(r"^==.*\stest session starts\s==+")
 test_session_starts_results_grabber = re.compile(r"(collected\s\d+\sitems[\s\S]+)")
 test_session_starts_test_matcher = r"^(.*::.*)"
 errors_section_matcher = re.compile(r"^==.*\sERRORS\s==+")
@@ -260,16 +231,15 @@
         self.tui_session_start_time = self.tui_test_info["session_start_time"]
         self.tui_session_end_time = self.tui_test_info["session_end_time"]
         self.tui_session_duration = self.tui_test_info["session_duration"]
         self.tui_test_results = self.tui_test_info["tui_test_results"]
         self.tui_rerun_test_groups = self.tui_test_info["tui_rerun_test_groups"]
         self.tui_sections = self.tui_test_info["tui_sections"]
         self.tui_htmlfile = self.tui_test_info["tui_htmlfile"]
-        self.tui_fold_level = self.tui_test_info["tui_fold_level"]
-
+        self.tui_regexfile = self.tui_test_info["tui_regexfile"]
         self.terminal_output = self._get_terminal_output()
 
     def _unpickle_tui_test_info(self):
         """Unpack pickled results file"""
         try:
             with open(TUI_RESULTS_FILE, "rb") as rfile:
                 return pickle.load(rfile)
@@ -285,8 +255,23 @@
             with open(file_path, "r") as file:
                 return file.read()
         except FileNotFoundError as e:
             raise FileNotFoundError(
                 f"Cannot find {file_path}. Have you run pytest with the '--tui' option"
                 " yet?"
             ) from e
-            pass
+
+
+# def get_regex(tui_regexfile: Path) -> List[str]:
+#     """Read regex file and return list of regexes"""
+#     try:
+#         with open(tui_regexfile, "r") as file:
+#             # lines = [ast.literal_eval(line) for line in file.readlines() if line]
+#             lines = [eval(line) for line in file.readlines() if line]
+#             return [line.rstrip() for line in lines if line]
+#     except FileNotFoundError as e:
+#         print(e)
+#         return []
+
+
+# TUI_REGEXES = get_regex(Path.cwd().resolve() / "tui_regexes.txt")
+# # ^^^ really bad idea, since it can fail even if --tui option is not specified
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytest-tui-1.9.2/pytest_tui.egg-info/PKG-INFO` & `pytest-tui-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-tui
-Version: 1.9.2
+Version: 2.0.0
 Summary: Text User Interface (TUI) and HTML report for Pytest test runs
 Home-page: https://github.com/jeffwright13/pytest-tui
 Author: Jeff Wright
 Author-email: jeff.washcloth@gmail.com
 License: MIT
 Keywords: pytest pytest-plugin testing tui textual html
 Classifier: Framework :: Pytest
@@ -29,14 +29,17 @@
 
 ### TUI:
 ![2022-05-01 19 25 19](https://user-images.githubusercontent.com/4308435/166174159-b442a5b5-416d-42a0-badd-7401e9980e47.gif)
 
 ### HTML:
 ![2022-08-27 08 07 11](https://user-images.githubusercontent.com/4308435/187034046-312b1ee8-0f7b-49a1-994f-9c38a9d3941c.gif)
 
+### Log Folding:
+![2023-04-11 23 56 57](https://user-images.githubusercontent.com/4308435/231364763-132e8c35-cb61-4172-9686-176d84c038ca.gif)
+
 ## Introduction
 When you run Pytest campaigns that produce a lot of terminal output (e.g. with many tests, very detailed output, or with multiple failures), the standard Pytest output can make it difficult to examine the results. You end up scrolling way back in the terminal, looking for that one test you want to examine more closely. Pytest-tui provides a Text User Interface (TUI) and an HTML page that aim to make it easier to find the information you're looking for.
 
 Test results are categorized in the same way Pytest does it:
 
 - By outcome: `[Pass|Fail|Error|Skipped|Xpass|Xfail]`
 - By output section: `[Summary|Full|Errors|Passes|Failures|Warnings]`
@@ -44,15 +47,16 @@
 The intent it to make it easier for you to find the specific results you want so you can examine it without all the other results getting in your way.
 
 How does it work in practice? Easy. You just run your Pytest campaigns like you normally would, adding the command line option `--tui` (`pytest --tui`). Your test session will proceed as it always does (always in verbose mode), showing you the familiar terminal output while running. Then, at the end of the session, a TUI or an HTML page can be launched via the included console scripts (`tui` and/or `tuih`). The results are displayed on-screen or in-browser for you to examine. When you're done, just exit the TUI to go back to the terminal, or close the HTML page. Don't worry about losing your test session data. Results are stored to local disk and you can always relaunch the TUI or HTML page using those same console scripts.
 
 Output sections and individual test results are expandable/collapsible, and test summary statistics are displayed for convenience. Both the TUI and the HTML page retain the original pytest ANSI-encoded color output, lending a familiar look and feel.
 
 ## Features
-- **New** Log message folding on the HTML page, configurable by log level! See "Python Log Message Folding" section below.
+- **New** in 1.10.0 Regex-based folding on the HTML page, configurable by user-provided regex! See "Python Regex Folding" section below.
+- **New** in 1.9.1 Log message folding on the HTML page, configurable by log level. See "Python Log Message Folding" section below.
 - Launch either or both of the [Textual](https://github.com/Textualize/textual) TUI or the HTML page using built in console scripts
 - ANSI text markup support - whatever the output on your console looks like is how things are going to show up in the TUI
 - Mouse and keyboard support (including scrolling)
 - Support for all output formats/modes:
   - `-v`, `-vv`, `-no-header`, `--showlocals`, `--color=<yes|no|auto>`
   - all variants of `--tb` except "native"
   - "live-log" (aka log_cli)
@@ -84,15 +88,15 @@
 
 ### Running Your Tests
 
 Pretty much just run pytest like you always do, adding the `--tui` option to the list of command line options:
 
 `pytest --tui <whatever-else-you-normally-do>`
 
-In some environments, where the working directory for pytest has been changed from the default, it may be necessary to cd into the working directory in order to successfully launch the TUI or HTML. Basically, you need to be in the parent directory of wherever the `/ptt_files` folder has been placed by the plugin after a test run. This is a known issue and will be fixed at some point.
+In some environments, where the working directory for pytest has been changed from the default, it may be necessary to cd into the working directory in order to successfully launch the TUI or HTML. Basically, you need to be in the parent directory of wherever the `/tui_files` folder has been placed by the plugin after a test run. This is a known issue and will be fixed at some point.
 
 ### Sample / Demo Tests
 
 If you would like some dummy tests that will allow you to take pytest-tui for a testdrive, copy all the files at https://github.com/jeffwright13/pytest-tui/tree/main/demo-tests into a folder called `demo-tests/` where your test environment resides. You will need the additional libraries listed in /requirements/requirements-dev.txt, so install them (`pip install -r requirements-dev.txt`). Then:
 
 `pytest demo-tests/`
 
@@ -104,33 +108,42 @@
 
 On Linux terminals, you can typically press and hold the SHIFT key on your keyboard to temporarily bypass the TUI and access the terminal's native mouse copy/paste functionality (commonly, click-drag-release or double-click to select text, middle-click to paste). This copy/paste works with the terminal's selection buffer, as opposed to the TUI's buffer.
 
 On Windows, use the ALT key while click-dragging the mouse. Mac users can get the same effect with the Option key.
 
 ### Generating and viewing the HTML File
 
-The HTML output file is located at `<cwd>/ptt_files/html_report.html`. The HTML file is generated and launched via browser when the `tuih` script is invoked on the command line.
+The HTML output file is located at `<cwd>/tui_files/html_report.html`. The HTML file is automatically generated when a test run is completed with the "--tui" option. It can also be generated manually with the `tuih` script by invoking it on the command line.
+
+### Visibility
+
+Sometimes it can be difficult to read the terminal output when rendered on the HTML report. Pytest embeds ANSI color codes in its output, which are interpreted by a terminal program to display various colors for text. Pytest-tui takes these ANSI color codes and translates them to HTML (using the [ansi2html](https://pypi.org/project/ansi2html/) librray). Because the dhe default color scheme for the HTML report is a light background with dark text, it can be difficult to see some of the colors. To address this, there are three buttons that can help. The first ("Toggle Background") allow you to toggle the bakcground color of all console output. This should result in a page that closely resembles the output you would get in a standard terminal environment (assuming you have white text on a black background). The other two buttons, Invert Colors and Remove/Restore Colors, are a bit more drastic in that they affect all text in the report. Experiment and see what works for you. Also note that if you have your browser set to dark mode, or have a theme that changes the default color scheme, this can also affect the visibility of the text.
+### "Folding" output in the HTML report
 
-### Python Log Message Folding (HTML file)
+New in 1.11.0 is the integrated "folding" feature, which will automatically roll up any output lines from your test's output which match a regex (or regexes) specified in the file given on the command line. This option allows you to match on specific lines of console output from pytest, and 'fold' them (hide them).
 
-New in 1.9.1 is the "folding" feature, which will automatically roll up any output lines from the test run which are from the Python logger and which are at or below a configurable level. This lets you view verbose debug-level output when you need it, and fold it away, out of sight when you don't. There is no special configuration that has to be done to use this feature, other than enabling at run time with the `--tui-fold-level` option (see `pytest --help`). By default, this value is set to WARNING, in keeping with the default level of Python's logging module when creating a new logger.
+The folding feature is activated by passing the `--tui-regexfile` option (see `pytest --help`), and setting the path of a file containing the desired regex or regexes.
 
-This new feature produces a section in the HTML report file called "Folded Output", which displays the test run's console output with all lines of the configured log level folded up. Each folded section can be individually toggled opened/closed by clicking the "Folded WARNING" line (or whatever level you have configured). You can toggle all folded sections by clicking the "Fold/Unfold Logs" button inside the "Fold Actions" menu at the top right of the HTML page, and they can be hidden entirely by double-clicking the "Show/Hide Fold Markers" button.
+The file itself must contain plain text (UTF-8 encoded) with either a single regex, specified on a single line of the file; or two 'marker' patterns, specified in two consecutive lines of the file. If there is a single line in the file, that line is assumed to contain a regular expressoin that will cause the folding action to be used on any line in the console output of pytest if that line matches the regex. Consecutive lines that match will be folded into the same section. If there are two lines in the regex file, the first line is assumed to be a start marker, and the second line is assumed to be a stop marker. The folding action will be applied to all lines between the start and stop markers
 
+Ideas and tips for folding:
+- Run all tests with DEBUG level logging, but only view those DEBUG messages when necessary. I find this option particularly helpful when trying to debug a test that is only failing intermittently.
+- Mark certain sections of a test's output with a pair of start/end markers. If you have test output that is very chatty, but you only want to see it when you need to, this is a good option. For example, if you have a test that is making a bunch of API calls, and you want to see the output of those calls, but only when the test fails, you can mark the start and stop of the API calls with a pair of markers, and then fold them away when you don't need to see them.
+- Use the non-printable characters 'ZWS' and 'ZWJ' ((Zero Width Space)[https://en.wikipedia.org/wiki/Zero-width_space] / (Zero Width Joiner)[https://en.wikipedia.org/wiki/Zero-width_joiner]) as start and stop markers. The visual impact on the output is minimal (only inserts one visible space), and the regex pattern is very unlikely to match anything else in the output. The repo contains a file called `nonprintable_​​characters.txt` that contains cobinations of these characters, which can be used as a starting point for your own regexes.
 
 ## Known Limitations / Issues
 
 - Python support for 3.10+ is not guaranteed. Changes were made to the `importlib.metadata` library that are not backwards-compatible, and may result in exceptions when attempting to run. I have not had the chance to chase this down definitively, so until such a time that I fully understand the issue, I recommend using Python 3.8 or 3.9. Of course, YMMV...give it a try, and let me know how things go. :-)
 - User interfaces need work:
   - Overall layouts need optimization (I am definitely not a UX guy)
   - Textual interface may be sluggish, esp. if run within an IDE
   - All code here is like a sausage factory: pleasant enough, until you look inside - do so at your own peril!
 - Not fully tested with all combinations of output formats. Probably some use-cases where things won't work 100% right.
 - `pytest-tui` is currently incompatible with pytest command line option `--tb=native`, and will cause an INTERNALERROR if the two are used together.
-- HTML page cannot offer clickable links to local filesystem. This is one of the workflows I depend on when using iTerm2...traceback lines with a `file://` link to a locally-hosted resource are clickable, and open up my VSCode to that line in that file. Unfortunately, web browsers are much more security-minded than terminal apps, and actions like this are strictly disallowed.
+- HTML page cannot offer clickable links to local filesystem. This is one of the workflows I depend on when using iTerm2...traceback lines with a `file://` URL to a locally-hosted resource are clickable, and open up my IDE to that line in that file. Unfortunately, web browsers are much more security-minded than terminal apps, and actions like this are strictly disallowed.
 
 ## History
 
 This project was originally envisioned to only show test failures, and allow the user to 'fold' the details of the failed tests by clicking a line so that the details would alternately show/hide. In fact, the original repo was called `pytest-fold`. As development progressed, it became clear that what was really needed was a real TUI, one that organized the output in such a way that all of pytest's output was available in a more streamlined way.
 
 Several TUIs (using different TUI libraries) have been cycled through this project. The Textual interface is the only one currently supported, since some internal optimization has been done to make the results simpler to consume. However, other TUIs should be able to be integrated without too much work (e.g. Asciimatics, PyTermTk, pyermgui, etc.). Same would be true of a GUI. Contact the author if you have a desire to implement one of these. The results of any given testrun are collected and sorted in such a way that it should relatively simple to take them and put them into the presentation mode of choice.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest-tui-1.9.2/setup.py` & `pytest-tui-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 setup(
     name="pytest-tui",
-    version="1.9.2",
+    version="2.0.0",
     author="Jeff Wright",
     author_email="jeff.washcloth@gmail.com",
     license="MIT",
     url="https://github.com/jeffwright13/pytest-tui",
     description="Text User Interface (TUI) and HTML report for Pytest test runs",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     py_modules=["pytest_tui"],
     python_requires=">=3.8",
     install_requires=[
         "ansi2html==1.8.0",
+        "faker==18.3.1",
         "json2table==1.1.5",
         "pytest-metadata==2.0.4",
         "single-source==0.3.0",
         "strip-ansi==0.1.1",
         "textual==0.1.18",
     ],
     setup_requires=["setuptools_scm"],
```

### Comparing `pytest-tui-1.9.2/testing/bash/test.sh` & `pytest-tui-2.0.0/testing/bash/test.sh`

 * *Files 1% similar despite different names*

```diff
@@ -75,16 +75,16 @@
 EOD
 )
 # Recover from any ANSI corruption that may have occured as a result of running pytest-tui
 reset
 
 printf "Launching HTML\n"
 tuih
-printf "Check for exisence of output file '.ptt_files/hacked.html..."
-FILE=ptt_files/hacked.html
+printf "Check for exisence of output file '.tui_files/hacked.html..."
+FILE=tui_files/hacked.html
 if [ -f "$FILE" ]; then
     echo "$FILE exists."
 else
     echo "$FILE does not exist!"
 fi
```

### Comparing `pytest-tui-1.9.2/testing/robot/Tests/001_test_basic.robot` & `pytest-tui-2.0.0/testing/robot/Tests/001_test_basic.robot`

 * *Files identical despite different names*

### Comparing `pytest-tui-1.9.2/testing/robot/Tests/002_test_tui.robot` & `pytest-tui-2.0.0/testing/robot/Tests/002_test_tui.robot`

 * *Files identical despite different names*

