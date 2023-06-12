# Comparing `tmp/ambition-utils-3.0.3.tar.gz` & `tmp/ambition-utils-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ambition-utils-3.0.3.tar", last modified: Mon Jun 12 18:59:51 2023, max compression
+gzip compressed data, was "dist/ambition-utils-3.1.0.tar", last modified: Wed Mar 15 19:41:35 2023, max compression
```

## Comparing `ambition-utils-3.0.3.tar` & `ambition-utils-3.1.0.tar`

### file list

```diff
@@ -1,102 +1,101 @@
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils.egg-info/
--rw-r--r--   0 jared     (1000) jared     (1000)     3085 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jared     (1000) jared     (1000)        1 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jared     (1000) jared     (1000)       15 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils.egg-info/top_level.txt
--rw-r--r--   0 jared     (1000) jared     (1000)     2390 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils.egg-info/PKG-INFO
--rw-r--r--   0 jared     (1000) jared     (1000)      299 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils.egg-info/requires.txt
--rw-r--r--   0 jared     (1000) jared     (1000)     1075 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/LICENSE
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/tests/
--rw-rw-r--   0 jared     (1000) jared     (1000)     3144 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/tests/sql_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)    16240 2020-05-08 15:58:44.000000 ambition-utils-3.0.3/ambition_utils/tests/form_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     3435 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/tests/time_helper_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      190 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/tests/apps.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      364 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/tests/models.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/tests/migrations/
--rw-rw-r--   0 jared     (1000) jared     (1000)      685 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/tests/migrations/0002_auto_20230124_1754.py
--rw-rw-r--   0 jared     (1000) jared     (1000)        0 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/tests/migrations/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      489 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/tests/migrations/0001_initial.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       74 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/tests/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2666 2023-03-15 19:46:16.000000 ambition-utils-3.0.3/ambition_utils/tests/field_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)    13636 2021-03-10 18:52:40.000000 ambition-utils-3.0.3/ambition_utils/forms.py
--rw-r--r--   0 jared     (1000) jared     (1000)     7349 2020-05-08 15:58:44.000000 ambition-utils-3.0.3/ambition_utils/sql.py
--rw-r--r--   0 jared     (1000) jared     (1000)      138 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/apps.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/postgres_lock/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/postgres_lock/tests/
--rw-r--r--   0 jared     (1000) jared     (1000)     4399 2022-05-25 19:46:46.000000 ambition-utils-3.0.3/ambition_utils/postgres_lock/tests/lock_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/postgres_lock/tests/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     3782 2022-05-25 18:18:33.000000 ambition-utils-3.0.3/ambition_utils/postgres_lock/lock.py
--rw-r--r--   0 jared     (1000) jared     (1000)      875 2022-05-25 17:51:38.000000 ambition-utils-3.0.3/ambition_utils/postgres_lock/models.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/postgres_lock/migrations/
--rw-r--r--   0 jared     (1000) jared     (1000)      581 2022-05-25 17:54:45.000000 ambition-utils-3.0.3/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py
--rw-r--r--   0 jared     (1000) jared     (1000)      434 2020-05-08 15:58:44.000000 ambition-utils-3.0.3/ambition_utils/postgres_lock/migrations/0002_auto_20191030_1417.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/postgres_lock/migrations/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)      487 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/postgres_lock/migrations/0001_initial.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/postgres_lock/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2059 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/fields.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/transaction/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/transaction/tests/
--rw-r--r--   0 jared     (1000) jared     (1000)     2023 2021-03-11 16:47:27.000000 ambition-utils-3.0.3/ambition_utils/transaction/tests/durable_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2021-03-10 18:52:40.000000 ambition-utils-3.0.3/ambition_utils/transaction/tests/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     2261 2021-03-10 18:52:40.000000 ambition-utils-3.0.3/ambition_utils/transaction/decorators.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2666 2021-03-11 15:49:49.000000 ambition-utils-3.0.3/ambition_utils/transaction/utils.py
--rw-r--r--   0 jared     (1000) jared     (1000)       46 2021-03-10 18:52:40.000000 ambition-utils-3.0.3/ambition_utils/transaction/__init__.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/anomaly/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/anomaly/tests/
--rw-rw-r--   0 jared     (1000) jared     (1000)      202 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/anomaly/tests/apps.py
--rw-r--r--   0 jared     (1000) jared     (1000)      928 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/anomaly/tests/models.py
--rw-r--r--   0 jared     (1000) jared     (1000)     6036 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/anomaly/tests/anomaly_tests.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/anomaly/tests/migrations/
--rw-rw-r--   0 jared     (1000) jared     (1000)        0 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/anomaly/tests/migrations/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2748 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/anomaly/tests/migrations/0001_initial.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       76 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/anomaly/tests/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     9808 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/anomaly/models.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/anomaly/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)       38 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/urls.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       22 2023-06-12 18:48:33.000000 ambition-utils-3.0.3/ambition_utils/version.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/rrule/
--rw-r--r--   0 jared     (1000) jared     (1000)      389 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/rrule/handler.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/rrule/tests/
--rw-rw-r--   0 jared     (1000) jared     (1000)    17567 2023-06-12 18:05:35.000000 ambition-utils-3.0.3/ambition_utils/rrule/tests/form_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      200 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/rrule/tests/apps.py
--rw-rw-r--   0 jared     (1000) jared     (1000)    56586 2023-06-12 18:45:27.000000 ambition-utils-3.0.3/ambition_utils/rrule/tests/model_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      713 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/rrule/tests/models.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/rrule/tests/migrations/
--rw-rw-r--   0 jared     (1000) jared     (1000)        0 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/rrule/tests/migrations/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     1005 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/rrule/tests/migrations/0001_initial.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       72 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/rrule/tests/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     9796 2023-06-12 18:53:04.000000 ambition-utils-3.0.3/ambition_utils/rrule/forms.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      162 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/rrule/apps.py
--rw-r--r--   0 jared     (1000) jared     (1000)      127 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/rrule/constants.py
--rw-rw-r--   0 jared     (1000) jared     (1000)    18850 2023-06-05 21:16:36.000000 ambition-utils-3.0.3/ambition_utils/rrule/models.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/rrule/migrations/
--rw-r--r--   0 jared     (1000) jared     (1000)      486 2023-06-05 19:55:19.000000 ambition-utils-3.0.3/ambition_utils/rrule/migrations/0004_rrule_rrule_exclusion_params.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      936 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
--rw-r--r--   0 jared     (1000) jared     (1000)      415 2020-05-08 15:58:44.000000 ambition-utils-3.0.3/ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/rrule/migrations/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     1071 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/rrule/migrations/0001_initial.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       61 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/rrule/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)      112 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/__init__.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/activity/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/activity/tests/
--rw-r--r--   0 jared     (1000) jared     (1000)     2785 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/activity/tests/task_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)      229 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/activity/tests/model_tests.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/activity/tests/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     4446 2023-03-15 18:34:46.000000 ambition-utils-3.0.3/ambition_utils/activity/models.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/ambition_utils/activity/migrations/
--rw-r--r--   0 jared     (1000) jared     (1000)     1696 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/activity/migrations/0002_auto_20180427_1819.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/activity/migrations/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     2271 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/activity/migrations/0001_initial.py
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/activity/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     2799 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/ambition_utils/activity/tasks.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     4765 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/ambition_utils/time_helpers.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/requirements/
--rw-rw-r--   0 jared     (1000) jared     (1000)      113 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/requirements/requirements-testing.txt
--rw-rw-r--   0 jared     (1000) jared     (1000)      208 2023-03-15 19:46:16.000000 ambition-utils-3.0.3/requirements/requirements.txt
--rw-r--r--   0 jared     (1000) jared     (1000)       31 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/requirements/docs.txt
--rw-rw-r--   0 jared     (1000) jared     (1000)     1990 2023-03-15 18:33:18.000000 ambition-utils-3.0.3/setup.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      252 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/setup.cfg
--rw-r--r--   0 jared     (1000) jared     (1000)     1114 2018-12-06 16:28:22.000000 ambition-utils-3.0.3/README.rst
--rw-r--r--   0 jared     (1000) jared     (1000)       68 2018-12-06 16:50:17.000000 ambition-utils-3.0.3/MANIFEST.in
--rw-rw-r--   0 jared     (1000) jared     (1000)     2390 2023-06-12 18:59:51.000000 ambition-utils-3.0.3/PKG-INFO
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils.egg-info/
+-rw-r--r--   0 jared     (1000) jared     (1000)     3016 2023-03-15 19:41:34.000000 ambition-utils-3.1.0/ambition_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)        1 2023-03-15 19:41:34.000000 ambition-utils-3.1.0/ambition_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)       15 2023-03-15 19:41:34.000000 ambition-utils-3.1.0/ambition_utils.egg-info/top_level.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)     2390 2023-03-15 19:41:34.000000 ambition-utils-3.1.0/ambition_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jared     (1000) jared     (1000)      287 2023-03-15 19:41:34.000000 ambition-utils-3.1.0/ambition_utils.egg-info/requires.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)     1075 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/LICENSE
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/tests/
+-rw-rw-r--   0 jared     (1000) jared     (1000)     3144 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/sql_tests.py
+-rw-r--r--   0 jared     (1000) jared     (1000)    16240 2020-05-08 15:58:44.000000 ambition-utils-3.1.0/ambition_utils/tests/form_tests.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)     3435 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/time_helper_tests.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)      190 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/apps.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)      364 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/models.py
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/tests/migrations/
+-rw-rw-r--   0 jared     (1000) jared     (1000)      685 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/migrations/0002_auto_20230124_1754.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)        0 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/migrations/__init__.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)      489 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/migrations/0001_initial.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)       74 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/tests/__init__.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)     2556 2023-03-15 19:41:28.000000 ambition-utils-3.1.0/ambition_utils/tests/field_tests.py
+-rw-r--r--   0 jared     (1000) jared     (1000)    13636 2021-03-10 18:52:40.000000 ambition-utils-3.1.0/ambition_utils/forms.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     7349 2020-05-08 15:58:44.000000 ambition-utils-3.1.0/ambition_utils/sql.py
+-rw-r--r--   0 jared     (1000) jared     (1000)      138 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/apps.py
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/tests/
+-rw-r--r--   0 jared     (1000) jared     (1000)     4399 2022-05-25 19:46:46.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/tests/lock_tests.py
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/tests/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     3782 2022-05-25 18:18:33.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/lock.py
+-rw-r--r--   0 jared     (1000) jared     (1000)      875 2022-05-25 17:51:38.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/models.py
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/migrations/
+-rw-r--r--   0 jared     (1000) jared     (1000)      581 2022-05-25 17:54:45.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py
+-rw-r--r--   0 jared     (1000) jared     (1000)      434 2020-05-08 15:58:44.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/migrations/0002_auto_20191030_1417.py
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/migrations/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)      487 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/migrations/0001_initial.py
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/postgres_lock/__init__.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)     2059 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/fields.py
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/transaction/
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/transaction/tests/
+-rw-r--r--   0 jared     (1000) jared     (1000)     2023 2021-03-11 16:47:27.000000 ambition-utils-3.1.0/ambition_utils/transaction/tests/durable_tests.py
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2021-03-10 18:52:40.000000 ambition-utils-3.1.0/ambition_utils/transaction/tests/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     2261 2021-03-10 18:52:40.000000 ambition-utils-3.1.0/ambition_utils/transaction/decorators.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)     2666 2021-03-11 15:49:49.000000 ambition-utils-3.1.0/ambition_utils/transaction/utils.py
+-rw-r--r--   0 jared     (1000) jared     (1000)       46 2021-03-10 18:52:40.000000 ambition-utils-3.1.0/ambition_utils/transaction/__init__.py
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/anomaly/
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/
+-rw-rw-r--   0 jared     (1000) jared     (1000)      202 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/apps.py
+-rw-r--r--   0 jared     (1000) jared     (1000)      928 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/models.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     6036 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/anomaly_tests.py
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/migrations/
+-rw-rw-r--   0 jared     (1000) jared     (1000)        0 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/migrations/__init__.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)     2748 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/migrations/0001_initial.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)       76 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/anomaly/tests/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     9808 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/anomaly/models.py
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/anomaly/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)       38 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/urls.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)       22 2023-03-15 19:41:28.000000 ambition-utils-3.1.0/ambition_utils/version.py
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/rrule/
+-rw-r--r--   0 jared     (1000) jared     (1000)      389 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/rrule/handler.py
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/
+-rw-rw-r--   0 jared     (1000) jared     (1000)    16189 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/form_tests.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)      200 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/apps.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)    54228 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/model_tests.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)      713 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/models.py
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/migrations/
+-rw-rw-r--   0 jared     (1000) jared     (1000)        0 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/migrations/__init__.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)     1005 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/migrations/0001_initial.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)       72 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/tests/__init__.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)     8681 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/forms.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)      162 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/apps.py
+-rw-r--r--   0 jared     (1000) jared     (1000)      127 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/rrule/constants.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)    16920 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/models.py
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/rrule/migrations/
+-rw-rw-r--   0 jared     (1000) jared     (1000)      936 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
+-rw-r--r--   0 jared     (1000) jared     (1000)      415 2020-05-08 15:58:44.000000 ambition-utils-3.1.0/ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/rrule/migrations/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     1071 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/rrule/migrations/0001_initial.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)       61 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/rrule/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)      112 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/__init__.py
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/activity/
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/activity/tests/
+-rw-r--r--   0 jared     (1000) jared     (1000)     2785 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/tests/task_tests.py
+-rw-r--r--   0 jared     (1000) jared     (1000)      229 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/tests/model_tests.py
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/tests/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     4446 2023-03-15 18:34:46.000000 ambition-utils-3.1.0/ambition_utils/activity/models.py
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/ambition_utils/activity/migrations/
+-rw-r--r--   0 jared     (1000) jared     (1000)     1696 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/migrations/0002_auto_20180427_1819.py
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/migrations/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     2271 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/migrations/0001_initial.py
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     2799 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/ambition_utils/activity/tasks.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)     4765 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/ambition_utils/time_helpers.py
+drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/requirements/
+-rw-rw-r--   0 jared     (1000) jared     (1000)      113 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/requirements/requirements-testing.txt
+-rw-rw-r--   0 jared     (1000) jared     (1000)      168 2023-03-15 19:41:28.000000 ambition-utils-3.1.0/requirements/requirements.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)       31 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/requirements/docs.txt
+-rw-rw-r--   0 jared     (1000) jared     (1000)     1990 2023-03-15 18:33:18.000000 ambition-utils-3.1.0/setup.py
+-rw-rw-r--   0 jared     (1000) jared     (1000)      252 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/setup.cfg
+-rw-r--r--   0 jared     (1000) jared     (1000)     1114 2018-12-06 16:28:22.000000 ambition-utils-3.1.0/README.rst
+-rw-r--r--   0 jared     (1000) jared     (1000)       68 2018-12-06 16:50:17.000000 ambition-utils-3.1.0/MANIFEST.in
+-rw-rw-r--   0 jared     (1000) jared     (1000)     2390 2023-03-15 19:41:35.000000 ambition-utils-3.1.0/PKG-INFO
```

### Comparing `ambition-utils-3.0.3/ambition_utils.egg-info/SOURCES.txt` & `ambition-utils-3.1.0/ambition_utils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 ambition_utils/rrule/constants.py
 ambition_utils/rrule/forms.py
 ambition_utils/rrule/handler.py
 ambition_utils/rrule/models.py
 ambition_utils/rrule/migrations/0001_initial.py
 ambition_utils/rrule/migrations/0002_auto_20190422_2037.py
 ambition_utils/rrule/migrations/0003_auto_20220623_1649.py
-ambition_utils/rrule/migrations/0004_rrule_rrule_exclusion_params.py
 ambition_utils/rrule/migrations/__init__.py
 ambition_utils/rrule/tests/__init__.py
 ambition_utils/rrule/tests/apps.py
 ambition_utils/rrule/tests/form_tests.py
 ambition_utils/rrule/tests/model_tests.py
 ambition_utils/rrule/tests/models.py
 ambition_utils/rrule/tests/migrations/0001_initial.py
```

### Comparing `ambition-utils-3.0.3/ambition_utils.egg-info/PKG-INFO` & `ambition-utils-3.1.0/ambition_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambition-utils
-Version: 3.0.3
+Version: 3.1.0
 Summary: Various utility packages used across Ambition projects.
 Home-page: https://github.com/ambitioninc/ambition-utils
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
 Description: .. image:: https://travis-ci.org/ambitioninc/ambition-utils.png
            :target: https://travis-ci.org/ambitioninc/ambition-utils
```

### Comparing `ambition-utils-3.0.3/LICENSE` & `ambition-utils-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/tests/sql_tests.py` & `ambition-utils-3.1.0/ambition_utils/tests/sql_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/tests/form_tests.py` & `ambition-utils-3.1.0/ambition_utils/tests/form_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/tests/time_helper_tests.py` & `ambition-utils-3.1.0/ambition_utils/tests/time_helper_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/tests/migrations/0002_auto_20230124_1754.py` & `ambition-utils-3.1.0/ambition_utils/tests/migrations/0002_auto_20230124_1754.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/tests/field_tests.py` & `ambition-utils-3.1.0/ambition_utils/tests/field_tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,32 +24,31 @@
         instance.save()
         self.assertEqual(instance.cast_time_zone_field, pytz.timezone('US/Eastern'))
 
         # Load from db and verify again
         instance.refresh_from_db()
         self.assertEqual(instance.cast_time_zone_field, pytz.timezone('US/Eastern'))
 
-    # TODO: uncomment when we are off of the forked timezone field
-    # def test_no_cast_on_assign(self):
-    #     """
-    #     Verifies the base time zone field is not cast when being assigned
-    #     """
-    #     instance = FakeModel()
-    #     instance.no_cast_time_zone_field = 'US/Eastern'
-    #
-    #     # Verify the timezone is a string
-    #     self.assertEqual(instance.no_cast_time_zone_field, 'US/Eastern')
-    #
-    #     # Save and verify it is still a string
-    #     instance.save()
-    #     self.assertEqual(instance.no_cast_time_zone_field, 'US/Eastern')
-    #
-    #     # Load from db and verify it is now cast as a time zone
-    #     instance.refresh_from_db()
-    #     self.assertEqual(instance.no_cast_time_zone_field, pytz.timezone('US/Eastern'))
+    def test_no_cast_on_assign(self):
+        """
+        Verifies the base time zone field is not cast when being assigned
+        """
+        instance = FakeModel()
+        instance.no_cast_time_zone_field = 'US/Eastern'
+
+        # Verify the timezone is a string
+        self.assertEqual(instance.no_cast_time_zone_field, 'US/Eastern')
+
+        # Save and verify it is still a string
+        instance.save()
+        self.assertEqual(instance.no_cast_time_zone_field, 'US/Eastern')
+
+        # Load from db and verify it is now cast as a time zone
+        instance.refresh_from_db()
+        self.assertEqual(instance.no_cast_time_zone_field, pytz.timezone('US/Eastern'))
 
     def test_all_time_zones_choices(self):
         """
         Verifies that all time zones are available in a method for usage in form choices
         """
         # Obtain a timezone that is in pytz.all_timezones, but not in pytz.common_timezones
         timezones = set(pytz.all_timezones) - set(pytz.common_timezones)
```

### Comparing `ambition-utils-3.0.3/ambition_utils/forms.py` & `ambition-utils-3.1.0/ambition_utils/forms.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/sql.py` & `ambition-utils-3.1.0/ambition_utils/sql.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/postgres_lock/tests/lock_tests.py` & `ambition-utils-3.1.0/ambition_utils/postgres_lock/tests/lock_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/postgres_lock/lock.py` & `ambition-utils-3.1.0/ambition_utils/postgres_lock/lock.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/postgres_lock/models.py` & `ambition-utils-3.1.0/ambition_utils/postgres_lock/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py` & `ambition-utils-3.1.0/ambition_utils/postgres_lock/migrations/0003_auto_20220525_1754.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/fields.py` & `ambition-utils-3.1.0/ambition_utils/fields.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/transaction/tests/durable_tests.py` & `ambition-utils-3.1.0/ambition_utils/transaction/tests/durable_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/transaction/decorators.py` & `ambition-utils-3.1.0/ambition_utils/transaction/decorators.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/transaction/utils.py` & `ambition-utils-3.1.0/ambition_utils/transaction/utils.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/anomaly/tests/models.py` & `ambition-utils-3.1.0/ambition_utils/anomaly/tests/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/anomaly/tests/anomaly_tests.py` & `ambition-utils-3.1.0/ambition_utils/anomaly/tests/anomaly_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/anomaly/tests/migrations/0001_initial.py` & `ambition-utils-3.1.0/ambition_utils/anomaly/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/anomaly/models.py` & `ambition-utils-3.1.0/ambition_utils/anomaly/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/rrule/tests/form_tests.py` & `ambition-utils-3.1.0/ambition_utils/rrule/tests/form_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime
-import json
 
 from dateutil import rrule
 from django.test import TestCase
 from freezegun import freeze_time
 
 from ambition_utils.rrule.constants import RecurrenceEnds
 from ambition_utils.rrule.forms import RecurrenceForm
@@ -114,15 +113,14 @@
             'byminute': 0,
             'bynweekday': [],
             'byweekday': [],
             'count': None,
             'repeat_by': '',
             'until': None,
             'rrule': None,
-            'rrule_exclusion': None
         })
 
     def test_missing_after_occurrences_count(self):
         data = {
             'freq': rrule.DAILY,
             'interval': 4,
             'dtstart': '6/1/2017',
@@ -486,40 +484,7 @@
         form = RecurrenceForm(data=data)
         self.assertTrue(form.is_valid())
         rrule_model = form.save(
             occurrence_handler_path='ambition_utils.rrule.handler.OccurrenceHandler',
         )
         self.assertEqual(RRule.objects.count(), 1)
         self.assertEqual(rrule_model.next_occurrence, datetime.datetime(2017, 6, 7))
-
-    def test_exclusion_rule(self):
-        exclusion_data = {
-            'freq': rrule.MONTHLY,
-            'interval': 1,
-            'dtstart': '6/1/2023',
-            'byhour': '0',
-            'bysetpos': 2,
-            'bynweekday': json.dumps([[0, 2]]),
-            'ends': RecurrenceEnds.NEVER,
-            'repeat_by': 'DAY_OF_THE_WEEK_START'
-        }
-        data = {
-            'freq': rrule.WEEKLY,
-            'interval': 1,
-            'dtstart': '6/1/2023',
-            'byhour': '0',
-            'byweekday': json.dumps([0]),
-            'time_zone': 'UTC',
-            'ends': RecurrenceEnds.NEVER,
-            'rrule_exclusion': json.dumps(exclusion_data)
-        }
-        form = RecurrenceForm(data=data)
-        self.assertTrue(form.is_valid())
-        rrule_model = form.save()
-        self.assertEqual(
-            rrule_model.get_dates(num_dates=10),
-            [datetime.datetime(2023, 6, 5, 0, 0), datetime.datetime(2023, 6, 19, 0, 0),
-             datetime.datetime(2023, 6, 26, 0, 0), datetime.datetime(2023, 7, 3, 0, 0),
-             datetime.datetime(2023, 7, 17, 0, 0), datetime.datetime(2023, 7, 24, 0, 0),
-             datetime.datetime(2023, 7, 31, 0, 0), datetime.datetime(2023, 8, 7, 0, 0),
-             datetime.datetime(2023, 8, 21, 0, 0), datetime.datetime(2023, 8, 28, 0, 0)]
-        )
```

### Comparing `ambition-utils-3.0.3/ambition_utils/rrule/tests/model_tests.py` & `ambition-utils-3.1.0/ambition_utils/rrule/tests/model_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1418,60 +1418,7 @@
             [
                 datetime.datetime(2022, 10, 28, 7),
                 datetime.datetime(2022, 10, 29, 7),
                 datetime.datetime(2022, 10, 30, 8),
                 datetime.datetime(2022, 10, 31, 8),
             ]
         )
-
-
-class RRuleWithExclusionTest(TestCase):
-    def test_exclusion(self):
-        weekly_program = Program.objects.create(name='Weekly Program')
-        weekly_rrule = RRule.objects.create(
-            rrule_params={
-                'freq': rrule.DAILY,
-                'interval': 1,
-                'dtstart': datetime.datetime(2023, 6, 1),
-                'byweekday': 0,
-            },
-            rrule_exclusion_params={
-                'freq': rrule.MONTHLY,
-                'interval': 1,
-                'dtstart': datetime.datetime(2023, 6, 1),
-                'bysetpos': 2,
-                'byweekday': 0
-            },
-            related_object=weekly_program,
-            related_object_handler_name='handle_start_recurrence',
-        )
-        monthly_program = Program.objects.create(name='Monthly Program')
-        monthly_rrule = RRule.objects.create(
-            rrule_params={
-                'freq': rrule.MONTHLY,
-                'interval': 1,
-                'dtstart': datetime.datetime(2023, 6, 1),
-                'bysetpos': 2,
-                'byweekday': 0
-            },
-            related_object=monthly_program,
-            related_object_handler_name='handle_start_recurrence',
-        )
-
-        weekly_dates = weekly_rrule.get_dates(num_dates=10)
-        monthly_dates = monthly_rrule.get_dates(num_dates=10)
-        self.assertEqual(
-            weekly_dates,
-            [datetime.datetime(2023, 6, 5, 0, 0), datetime.datetime(2023, 6, 19, 0, 0),
-             datetime.datetime(2023, 6, 26, 0, 0), datetime.datetime(2023, 7, 3, 0, 0),
-             datetime.datetime(2023, 7, 17, 0, 0), datetime.datetime(2023, 7, 24, 0, 0),
-             datetime.datetime(2023, 7, 31, 0, 0), datetime.datetime(2023, 8, 7, 0, 0),
-             datetime.datetime(2023, 8, 21, 0, 0), datetime.datetime(2023, 8, 28, 0, 0)]
-        )
-        self.assertEqual(
-            monthly_dates,
-            [datetime.datetime(2023, 6, 12, 0, 0), datetime.datetime(2023, 7, 10, 0, 0),
-             datetime.datetime(2023, 8, 14, 0, 0), datetime.datetime(2023, 9, 11, 0, 0),
-             datetime.datetime(2023, 10, 9, 0, 0), datetime.datetime(2023, 11, 13, 0, 0),
-             datetime.datetime(2023, 12, 11, 0, 0), datetime.datetime(2024, 1, 8, 0, 0),
-             datetime.datetime(2024, 2, 12, 0, 0), datetime.datetime(2024, 3, 11, 0, 0)]
-        )
```

### Comparing `ambition-utils-3.0.3/ambition_utils/rrule/tests/models.py` & `ambition-utils-3.1.0/ambition_utils/rrule/tests/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/rrule/tests/migrations/0001_initial.py` & `ambition-utils-3.1.0/ambition_utils/rrule/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/rrule/forms.py` & `ambition-utils-3.1.0/ambition_utils/rrule/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,19 +30,20 @@
     ('DAY_OF_THE_WEEK_START', 'Day of the week counting from the beginning of the month'),
     ('DAY_OF_THE_WEEK_END', 'Day of the week counting backwards from the end of the month'),
     # ('FIRST_DAY_OF_MONTH', 'First day of Month'),
     ('DAY_OF_THE_MONTH_END', 'Last day of Month'),
 )
 
 
-class RRuleForm(forms.Form):
+class RecurrenceForm(forms.Form):
     """
     Handles submission of data for populating rrule objects. The field names are based on the rrule
     params defined here http://dateutil.readthedocs.io/en/stable/rrule.html
     """
+    rrule = forms.ModelChoiceField(queryset=RRule.objects.all(), required=False)
 
     # Date from which the recurrence will be started from. This might not always be the first recurrence in the series
     dtstart = forms.DateField(
         error_messages={'required': 'Starts on is required'},
     )
 
     # The hour for each recurrence (0-23)
@@ -83,25 +84,32 @@
     # Number of times the recurrence will occur. Only required if ends is set to AFTER
     count = forms.IntegerField(required=False)
 
     # Date when the recurrence will end. Only required if ends is set to ON. The 'until' date might not be the last
     # recurrence date
     until = forms.DateField(required=False)
 
+    def __init__(self, *args, **kwargs):
+        # Remove the instance param if it exists. Model forms will try to pass this, but it isn't used here and will
+        # cause the base form init to fail
+        kwargs.pop('instance', None)
+
+        super(RecurrenceForm, self).__init__(*args, **kwargs)
+
     def clean_freq(self):
         """
         Make sure the frequency is an integer
         """
         return int(self.data.get('freq', -1))
 
     def clean(self):
         """
         Perform additional form validation based on submitted params
         """
-        cleaned_data = super().clean()
+        cleaned_data = super(RecurrenceForm, self).clean()
 
         if self.errors:
             return cleaned_data
 
         # Check if count is required
         if self.cleaned_data['ends'] == RecurrenceEnds.AFTER and not self.cleaned_data['count']:
             raise ValidationError('Number of occurrences is required')
@@ -160,15 +168,18 @@
         try:
             value = json.loads(self.data.get('bynweekday', '[]'))
         except ValueError:
             pass
 
         return value
 
-    def get_rrule_params_from_cleaned_data(self):
+    def save(self, **kwargs):
+        """
+        Saves the RRule model and returns it
+        """
         rrule_freq = self.cleaned_data['freq']
         start_date = self.cleaned_data['dtstart']
 
         # Convert date to datetime
         start_datetime = datetime.combine(start_date, datetime.min.time())
 
         # Build params for rrule object
@@ -201,72 +212,27 @@
                 params['bymonthday'] = start_datetime.day
             elif self.cleaned_data.get('repeat_by') == 'DAY_OF_THE_MONTH_END':
                 params['bymonthday'] = -1
             else:
                 params['byweekday'] = self.cleaned_data['bynweekday'][0][0]
                 params['bysetpos'] = self.cleaned_data['bynweekday'][0][1]
 
-        # Return the params
-        return params
-
-
-class RecurrenceForm(RRuleForm):
-    """
-    Converts rrule options into an rrule model
-    """
-
-    # Optional rrule object that we are modifying
-    rrule = forms.ModelChoiceField(queryset=RRule.objects.all(), required=False)
-
-    # Optional rrule exclusion params
-    rrule_exclusion = forms.CharField(required=False)
-
-    def __init__(self, *args, **kwargs):
-        # Remove the instance param if it exists. Model forms will try to pass this, but it isn't used here and will
-        # cause the base form init to fail
-        kwargs.pop('instance', None)
-
-        super(RecurrenceForm, self).__init__(*args, **kwargs)
-
-    def clean_rrule_exclusion(self):
-        # Get the value from data
-        rrule_exclusion = self.cleaned_data.get('rrule_exclusion')
-        if not rrule_exclusion:
-            return None
-
-        # Parse the exclusion options
-        rrule_exclusion = json.loads(rrule_exclusion)
-        rrule_exclusion['time_zone'] = self.cleaned_data['time_zone']
-
-        # Validate the options
-        rrule_exclusion_form = RRuleForm(data=rrule_exclusion)
-        if not rrule_exclusion_form.is_valid():
-            raise ValidationError('Exclusion options invalid')
-
-        # Return the exclusion params
-        return rrule_exclusion_form.get_rrule_params_from_cleaned_data()
-
-    def save(self, **kwargs):
-        """
-        Saves the RRule model and returns it
-        """
         # Keep track if this is an existing rrule that needs occurrence updated
         need_to_refresh_next_recurrence = False
 
         # Get the rrule model from the cleaned data
         rrule_model = self.cleaned_data.get('rrule')
         if rrule_model:
             need_to_refresh_next_recurrence = True
         else:
             # Use the recurrence passed into save kwargs
             rrule_model = kwargs.get('recurrence') or RRule()
 
         # Create or update the rule
-        rrule_model.rrule_params = self.get_rrule_params_from_cleaned_data()
-        rrule_model.rrule_exclusion_params = self.cleaned_data.get('rrule_exclusion')
+        rrule_model.rrule_params = params
         rrule_model.time_zone = self.cleaned_data.get('time_zone')
         for key, value in kwargs.items():
             if hasattr(rrule_model, key):
                 # This try except is because some field names might be reverse foreign key relationships
                 try:
                     setattr(rrule_model, key, value)
                 except TypeError:  # pragma: no cover
```

### Comparing `ambition-utils-3.0.3/ambition_utils/rrule/models.py` & `ambition-utils-3.1.0/ambition_utils/rrule/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from datetime import datetime, timedelta
 from dateutil import parser
-from dateutil.rrule import rrule, rruleset
+from dateutil.rrule import rrule
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.contrib.postgres.fields import JSONField
 from django.db import models, transaction
 from django.utils.module_loading import import_string
 from fleming import fleming
 from manager_utils import bulk_update
@@ -105,17 +105,14 @@
     """
     Model that will hold rrule details and generate recurrences to be handled by the supplied handler
     """
 
     # Params used to generate the rrule
     rrule_params = JSONField()
 
-    # Optional params used to generate the rrule exclusion
-    rrule_exclusion_params = JSONField(default=None, blank=True, null=True)
-
     # Any meta data associated with the object that created this rule
     meta_data = JSONField(default=dict)
 
     # The timezone all dates should be converted to
     time_zone = TimeZoneField(default='UTC')
 
     # The last occurrence date that was handled
@@ -136,17 +133,14 @@
     # The name of the method to call on the related_object when the recurrence has expired
     related_object_handler_name = models.TextField(default=None, null=True, blank=True)
 
     # Custom object manager
     objects = RRuleManager()
 
     def get_time_zone_object(self):
-        """
-        Returns the time zone object from pytz
-        """
         if self.time_zone is None:
             return pytz.utc
 
         # There is a test for this but it still doesn't hit this block
         if isinstance(self.time_zone, str):  # pragma: no cover
             return pytz.timezone(self.time_zone)
 
@@ -160,50 +154,21 @@
         """
         try:
             handler_class = import_string(self.occurrence_handler_path)()
             return handler_class
         except:
             return None
 
-    def get_rrule_set(self):
-        """
-        Returns the rrule set that will combine the rrule and optional exclusion rrule
-        """
-        rrule_set = rruleset()
-        rrule_set.rrule(self.get_rrule())
-        rrule_exclusion = self.get_rrule_exclusion()
-        if rrule_exclusion:
-            rrule_set.exrule(rrule_exclusion)
-        return rrule_set
-
     def get_rrule(self):
         """
         Builds the rrule object by restoring all the params.
-        """
-        return self.get_rrule_from_params(self.rrule_params)
-
-    def get_rrule_exclusion(self):
-        """
-        Builds the rrule exclusion object by restoring all the params.
-        :rtype: rrule
-        """
-        return self.get_rrule_from_params(self.rrule_exclusion_params)
-
-    def get_rrule_from_params(self, params):
-        """
-        Creates an rrule object from a dict of rrule params. Returns None if no params exists.
         The dtstart param will be converted to local time if it is set.
         :rtype: rrule
         """
-        # Check for none or empty
-        if not params:
-            return None
-
-        # Create a deep copy because we will manipulate
-        params = copy.deepcopy(params)
+        params = copy.deepcopy(self.rrule_params)
 
         # Convert next scheduled from utc back to time zone
         if params.get('dtstart') and not hasattr(params.get('dtstart'), 'date'):
             params['dtstart'] = parser.parse(params['dtstart'])
 
         # Convert until date from utc back to time zone
         if params.get('until') and not hasattr(params.get('until'), 'date'):
@@ -221,38 +186,38 @@
         :param last_occurrence: The last occurrence that was generated
         :param force: If the next occurrence is none, force the rrule to generate another
         :rtype: rrule or None
         """
         # Get the last occurrence
         last_occurrence = last_occurrence or self.last_occurrence or datetime.utcnow()
 
-        # Get the rule set
-        rule_set = self.get_rrule_set()
+        # Get the rule
+        rule = self.get_rrule()
 
         # Convert to local time zone for getting next occurrence, otherwise time zones ahead of utc will return the same
         last_occurrence = fleming.convert_to_tz(last_occurrence, self.get_time_zone_object(), return_naive=True)
 
         # Generate the next occurrence
-        next_occurrence = rule_set.after(last_occurrence)
+        next_occurrence = rule.after(last_occurrence)
 
         # If next occurrence is none and force is true, force the rrule to generate another date
         if next_occurrence is None and force:
             # Keep a reference to the original rrule_params
             original_rrule_params = {}
             original_rrule_params.update(self.rrule_params)
 
             # Remove any limiting params
             self.rrule_params.pop('count', None)
             self.rrule_params.pop('until', None)
 
-            # Refetch the rule set
-            rule_set = self.get_rrule_set()
+            # Refetch the rule
+            rule = self.get_rrule()
 
             # Generate the next occurrence
-            next_occurrence = rule_set.after(last_occurrence)
+            next_occurrence = rule.after(last_occurrence)
 
             # Restore the rrule params
             self.rrule_params = original_rrule_params
 
         # If there is a next occurrence, convert to utc
         if next_occurrence:
             next_occurrence = self.convert_to_utc(next_occurrence)
@@ -315,107 +280,83 @@
         else:
             self.next_occurrence = next_occurrence
 
     def pre_save_hooks(self):
         self.set_date_objects()
 
     def set_date_objects(self):
-        """
-        Ensure that all the date keys are properly set on all rrule params
-        """
+        # Check if this is a new rrule object
+        if self.pk is None:
+            # Convert next scheduled from utc back to time zone
+            if self.rrule_params.get('dtstart') and not hasattr(self.rrule_params.get('dtstart'), 'date'):
+                self.rrule_params['dtstart'] = parser.parse(self.rrule_params['dtstart'])
 
-        # Convert the rrule and exclusion rrule params to properly set date keys
-        is_new = self.pk is None
-        self.set_date_objects_for_params(self.rrule_params, is_new=is_new)
-        self.set_date_objects_for_params(self.rrule_exclusion_params, is_new=is_new)
+            # Convert until date from utc back to time zone
+            if self.rrule_params.get('until') and not hasattr(self.rrule_params.get('until'), 'date'):
+                self.rrule_params['until'] = parser.parse(self.rrule_params['until'])
 
-        # Check if this is a new rrule object
-        if is_new:
             # Get the first scheduled time according to the rrule (this converts from utc back to local time)
-            self.next_occurrence = self.get_rrule_set()[0]
+            self.next_occurrence = self.get_rrule()[0]
 
             # Convert back to utc before saving
             self.next_occurrence = self.convert_to_utc(self.next_occurrence)
 
-    def set_date_objects_for_params(self, params, is_new=False):
-        """
-        Give an rrule params object, ensure that the date keys are properly set and properly converted to strings
-        """
-        # Check for no params
-        if not params:
-            return params
-
-        # Check if this is a new rrule object
-        if is_new:
-            # Convert next scheduled from utc back to time zone
-            if params.get('dtstart') and not hasattr(params.get('dtstart'), 'date'):
-                params['dtstart'] = parser.parse(params['dtstart'])
-
-            # Convert until date from utc back to time zone
-            if params.get('until') and not hasattr(params.get('until'), 'date'):
-                params['until'] = parser.parse(params['until'])
-
         # Serialize the datetime objects if they exist
-        if params.get('dtstart') and hasattr(params.get('dtstart'), 'date'):
-            params['dtstart'] = params['dtstart'].strftime('%Y-%m-%d %H:%M:%S')
+        if self.rrule_params.get('dtstart') and hasattr(self.rrule_params.get('dtstart'), 'date'):
+            self.rrule_params['dtstart'] = self.rrule_params['dtstart'].strftime('%Y-%m-%d %H:%M:%S')
 
-        if params.get('until') and hasattr(params.get('until'), 'date'):
-            params['until'] = params['until'].strftime('%Y-%m-%d %H:%M:%S')
+        if self.rrule_params.get('until') and hasattr(self.rrule_params.get('until'), 'date'):
+            self.rrule_params['until'] = self.rrule_params['until'].strftime('%Y-%m-%d %H:%M:%S')
 
     def save(self, *args, **kwargs):
         """
         Saves the rrule model to the database. If this is a new object, the first next_scheduled time is
         determined and set. The `dtstart` and `until` objects will be safely encoded as strings if they are
         datetime objects.
         """
-
-        # Run any pre save hooks
         self.pre_save_hooks()
 
         # Call the parent save method
         super().save(*args, **kwargs)
 
     def get_dates(self, num_dates=20, start_date=None) -> List[datetime]:
         """
         Return a list of datetime objects the recurrence will generate, after the start date (if defined).
         :param num_dates: The maximum number of dates to calculate. Will stop at passed start_date
         :param start_date: The optional start date to begin generating dates after
         :return: A list of datetime objects
         """
-
-        # Assert that we have dates
         assert num_dates > 0
 
-        # Ensure that pre save hooks have been run
         self.pre_save_hooks()
 
-        # Generate the dates
         dates = []
+
         try:
             # Capture the rule's first date for use in RRule.after() in the loop.
-            rule_set = self.get_rrule_set()
+            rule = self.get_rrule()
 
             # Evaluate if the first date should be retained.
-            d = self.convert_to_utc(rule_set[0])
+            d = self.convert_to_utc(rule[0])
             if not start_date or d > start_date:
                 dates.append(d)
 
             # Continue evaluating and appending dates to satisfy desired number,
             # retaining date for evaluation in the next iteration.
             while len(dates) < num_dates:
                 d = self.get_next_occurrence(last_occurrence=d)
                 if d:
                     if not start_date or d > start_date:
                         dates.append(d)
                 else:
                     break
+
         except Exception:  # pragma: no cover
             pass
 
-        # Return the generated dates
         return dates
 
     def generate_dates(self, num_dates=20):
         """
         DEPRECATED. Replaced by get_dates.
         Return a list of the next num_dates datetimes of the recurrence.
         """
@@ -426,15 +367,17 @@
         """
         Creates a clone of itself.
         """
 
         # Clear id to force a new object.
         clone = copy.deepcopy(self)
         clone.id = None
+
         clone.save()
+
         return clone
 
     def clone_with_day_offset(self, day_offset: int) -> RRule:
         """
         Creates a clone of a passed RRule object offset by a specified number of days
         :param day_offset: The number of days to offset the clone's start date. Can be negative.
         """
```

### Comparing `ambition-utils-3.0.3/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py` & `ambition-utils-3.1.0/ambition_utils/rrule/migrations/0003_auto_20220623_1649.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/rrule/migrations/0001_initial.py` & `ambition-utils-3.1.0/ambition_utils/rrule/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/activity/tests/task_tests.py` & `ambition-utils-3.1.0/ambition_utils/activity/tests/task_tests.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/activity/models.py` & `ambition-utils-3.1.0/ambition_utils/activity/models.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/activity/migrations/0002_auto_20180427_1819.py` & `ambition-utils-3.1.0/ambition_utils/activity/migrations/0002_auto_20180427_1819.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/activity/migrations/0001_initial.py` & `ambition-utils-3.1.0/ambition_utils/activity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/activity/tasks.py` & `ambition-utils-3.1.0/ambition_utils/activity/tasks.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/ambition_utils/time_helpers.py` & `ambition-utils-3.1.0/ambition_utils/time_helpers.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/setup.py` & `ambition-utils-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/README.rst` & `ambition-utils-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `ambition-utils-3.0.3/PKG-INFO` & `ambition-utils-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambition-utils
-Version: 3.0.3
+Version: 3.1.0
 Summary: Various utility packages used across Ambition projects.
 Home-page: https://github.com/ambitioninc/ambition-utils
 Author: Wes Okes
 Author-email: wes.okes@gmail.com
 License: MIT
 Description: .. image:: https://travis-ci.org/ambitioninc/ambition-utils.png
            :target: https://travis-ci.org/ambitioninc/ambition-utils
```

