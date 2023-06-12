# Comparing `tmp/shroomdk-2.0.7.tar.gz` & `tmp/shroomdk-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shroomdk-2.0.7.tar", last modified: Fri May 26 02:51:58 2023, max compression
+gzip compressed data, was "shroomdk-2.0.8.tar", last modified: Mon Jun 12 15:52:10 2023, max compression
```

## Comparing `shroomdk-2.0.7.tar` & `shroomdk-2.0.8.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.945809 shroomdk-2.0.7/
--rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 shroomdk-2.0.7/LICENSE.txt
--rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 shroomdk-2.0.7/MANIFEST.in
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-26 02:51:58.945891 shroomdk-2.0.7/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 shroomdk-2.0.7/README.md
--rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-26 02:49:25.000000 shroomdk-2.0.7/VERSION
--rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 shroomdk-2.0.7/requirements-dev.txt
--rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 shroomdk-2.0.7/requirements.txt
--rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-26 02:51:58.946148 shroomdk-2.0.7/setup.cfg
--rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 shroomdk-2.0.7/setup.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.933581 shroomdk-2.0.7/shroomdk/
--rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.934874 shroomdk-2.0.7/shroomdk/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/errors/server_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2982 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/flipside.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.934986 shroomdk-2.0.7/shroomdk/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.935460 shroomdk-2.0.7/shroomdk/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9851 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3636 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.936247 shroomdk-2.0.7/shroomdk/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.937063 shroomdk-2.0.7/shroomdk/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.938636 shroomdk-2.0.7/shroomdk/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2231 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1202 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/models/sleep_config.py
--rw-r--r--   0 jim        (501) staff       (20)     5898 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/rpc.py
--rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/shroomdk.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.938931 shroomdk-2.0.7/shroomdk/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.939093 shroomdk-2.0.7/shroomdk/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.939463 shroomdk-2.0.7/shroomdk/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.939680 shroomdk-2.0.7/shroomdk/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.939927 shroomdk-2.0.7/shroomdk/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.940131 shroomdk-2.0.7/shroomdk/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk/utils/sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.934181 shroomdk-2.0.7/shroomdk.egg-info/
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk.egg-info/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk.egg-info/SOURCES.txt
--rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk.egg-info/dependency_links.txt
--rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk.egg-info/requires.txt
--rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-26 02:51:58.000000 shroomdk-2.0.7/shroomdk.egg-info/top_level.txt
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.931999 shroomdk-2.0.7/src/
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.940826 shroomdk-2.0.7/src/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-09 02:05:09.000000 shroomdk-2.0.7/src/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/errors/server_error.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.940950 shroomdk-2.0.7/src/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.941493 shroomdk-2.0.7/src/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9851 2023-05-26 02:49:25.000000 shroomdk-2.0.7/src/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3636 2023-05-25 23:47:03.000000 shroomdk-2.0.7/src/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.942352 shroomdk-2.0.7/src/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.943154 shroomdk-2.0.7/src/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.944464 shroomdk-2.0.7/src/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2231 2023-05-26 02:49:25.000000 shroomdk-2.0.7/src/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1202 2023-05-25 23:47:03.000000 shroomdk-2.0.7/src/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/models/sleep_config.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.944687 shroomdk-2.0.7/src/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.944789 shroomdk-2.0.7/src/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.945073 shroomdk-2.0.7/src/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.945284 shroomdk-2.0.7/src/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.945468 shroomdk-2.0.7/src/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:58.945681 shroomdk-2.0.7/src/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 shroomdk-2.0.7/src/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.997783 shroomdk-2.0.8/
+-rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 shroomdk-2.0.8/LICENSE.txt
+-rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 shroomdk-2.0.8/MANIFEST.in
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-06-12 15:52:10.997865 shroomdk-2.0.8/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 shroomdk-2.0.8/README.md
+-rw-r--r--   0 jim        (501) staff       (20)        5 2023-06-12 15:44:06.000000 shroomdk-2.0.8/VERSION
+-rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 shroomdk-2.0.8/requirements-dev.txt
+-rw-r--r--   0 jim        (501) staff       (20)       33 2023-06-12 15:43:53.000000 shroomdk-2.0.8/requirements.txt
+-rw-r--r--   0 jim        (501) staff       (20)       79 2023-06-12 15:52:10.998157 shroomdk-2.0.8/setup.cfg
+-rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 shroomdk-2.0.8/setup.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.980856 shroomdk-2.0.8/shroomdk/
+-rw-r--r--   0 jim        (501) staff       (20)      147 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.985453 shroomdk-2.0.8/shroomdk/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/errors/server_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2982 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/flipside.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.985665 shroomdk-2.0.8/shroomdk/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.986162 shroomdk-2.0.8/shroomdk/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9851 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3636 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.988262 shroomdk-2.0.8/shroomdk/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.989438 shroomdk-2.0.8/shroomdk/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.990761 shroomdk-2.0.8/shroomdk/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2231 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1202 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/models/sleep_config.py
+-rw-r--r--   0 jim        (501) staff       (20)     5898 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/rpc.py
+-rw-r--r--   0 jim        (501) staff       (20)       68 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/shroomdk.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.990948 shroomdk-2.0.8/shroomdk/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.991053 shroomdk-2.0.8/shroomdk/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.991347 shroomdk-2.0.8/shroomdk/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.991541 shroomdk-2.0.8/shroomdk/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.991724 shroomdk-2.0.8/shroomdk/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.991902 shroomdk-2.0.8/shroomdk/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.982270 shroomdk-2.0.8/shroomdk.egg-info/
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk.egg-info/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)     4101 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jim        (501) staff       (20)        1 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jim        (501) staff       (20)       34 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk.egg-info/requires.txt
+-rw-r--r--   0 jim        (501) staff       (20)       13 2023-06-12 15:52:10.000000 shroomdk-2.0.8/shroomdk.egg-info/top_level.txt
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.978519 shroomdk-2.0.8/src/
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.992544 shroomdk-2.0.8/src/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-09 02:05:09.000000 shroomdk-2.0.8/src/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-06-12 15:43:53.000000 shroomdk-2.0.8/src/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/errors/server_error.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.992649 shroomdk-2.0.8/src/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.993085 shroomdk-2.0.8/src/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9851 2023-05-26 02:49:25.000000 shroomdk-2.0.8/src/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3636 2023-05-25 23:47:03.000000 shroomdk-2.0.8/src/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.993895 shroomdk-2.0.8/src/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.994723 shroomdk-2.0.8/src/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.996064 shroomdk-2.0.8/src/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2231 2023-05-26 02:49:25.000000 shroomdk-2.0.8/src/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1202 2023-05-25 23:47:03.000000 shroomdk-2.0.8/src/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/models/sleep_config.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.996264 shroomdk-2.0.8/src/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.996398 shroomdk-2.0.8/src/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.996907 shroomdk-2.0.8/src/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.997184 shroomdk-2.0.8/src/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.997397 shroomdk-2.0.8/src/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-06-12 15:52:10.997631 shroomdk-2.0.8/src/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 shroomdk-2.0.8/src/utils/sleep.py
```

### Comparing `shroomdk-2.0.7/LICENSE.txt` & `shroomdk-2.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/PKG-INFO` & `shroomdk-2.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shroomdk
-Version: 2.0.7
+Version: 2.0.8
 Summary: SDK by Flipside Crypto: Query the most reliable & comprehensive blockchain data in crypto
 Home-page: https://github.com/FlipsideCrypto/sdk/python
 Author: dev@flipsidecrypto.com
 Author-email: dev@flipsidecrypto.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `shroomdk-2.0.7/README.md` & `shroomdk-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/setup.py` & `shroomdk-2.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/errors/api_error.py` & `shroomdk-2.0.8/shroomdk/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/errors/query_run_errors.py` & `shroomdk-2.0.8/shroomdk/errors/query_run_errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 
 class QueryRunTimeoutError(BaseError):
     """
     Base class for all QueryRunTimeoutError errors.
     """
 
-    def __init__(self, timeoutMinutes: Union[int, float, None] = None):
-        if timeoutMinutes is None:
+    def __init__(self, timeoutSeconds: Union[int, float, None] = None):
+        if timeoutSeconds is None:
             self.message = f"QUERY_RUN_TIMEOUT_ERROR: your query has timed out."
         else:
-            self.message = f"QUERY_RUN_TIMEOUT_ERROR: your query has timed out after {timeoutMinutes} minutes."
+            self.message = f"QUERY_RUN_TIMEOUT_ERROR: your query has timed out after {timeoutSeconds} seconds."
         super().__init__(self.message)
 
 
 class QueryRunExecutionError(BaseError):
     """
     Base class for all QueryRunExecutionError errors.
     """
```

### Comparing `shroomdk-2.0.7/shroomdk/flipside.py` & `shroomdk-2.0.8/shroomdk/flipside.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/integrations/query_integration/compass_query_integration.py` & `shroomdk-2.0.8/shroomdk/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/integrations/query_integration/query_result_set_builder.py` & `shroomdk-2.0.8/shroomdk/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/models/compass/cancel_query_run.py` & `shroomdk-2.0.8/shroomdk/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/models/compass/core/query_run.py` & `shroomdk-2.0.8/shroomdk/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/models/compass/create_query_run.py` & `shroomdk-2.0.8/shroomdk/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/models/compass/get_query_run.py` & `shroomdk-2.0.8/shroomdk/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/models/compass/get_query_run_results.py` & `shroomdk-2.0.8/shroomdk/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/models/compass/get_sql_statement.py` & `shroomdk-2.0.8/shroomdk/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/models/compass/query_results.py` & `shroomdk-2.0.8/shroomdk/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/models/query.py` & `shroomdk-2.0.8/shroomdk/models/query.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/models/query_defaults.py` & `shroomdk-2.0.8/shroomdk/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/models/query_result_set.py` & `shroomdk-2.0.8/shroomdk/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/models/query_run_stats.py` & `shroomdk-2.0.8/shroomdk/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/models/query_status.py` & `shroomdk-2.0.8/shroomdk/models/query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/rpc.py` & `shroomdk-2.0.8/shroomdk/rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py` & `shroomdk-2.0.8/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py` & `shroomdk-2.0.8/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/tests/models/test_query_status.py` & `shroomdk-2.0.8/shroomdk/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/tests/test_rpc.py` & `shroomdk-2.0.8/shroomdk/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/tests/utils/test_sleep.py` & `shroomdk-2.0.8/shroomdk/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk/utils/sleep.py` & `shroomdk-2.0.8/shroomdk/utils/sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/shroomdk.egg-info/PKG-INFO` & `shroomdk-2.0.8/shroomdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shroomdk
-Version: 2.0.7
+Version: 2.0.8
 Summary: SDK by Flipside Crypto: Query the most reliable & comprehensive blockchain data in crypto
 Home-page: https://github.com/FlipsideCrypto/sdk/python
 Author: dev@flipsidecrypto.com
 Author-email: dev@flipsidecrypto.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `shroomdk-2.0.7/shroomdk.egg-info/SOURCES.txt` & `shroomdk-2.0.8/shroomdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/errors/api_error.py` & `shroomdk-2.0.8/src/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/errors/query_run_errors.py` & `shroomdk-2.0.8/src/errors/query_run_errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 
 class QueryRunTimeoutError(BaseError):
     """
     Base class for all QueryRunTimeoutError errors.
     """
 
-    def __init__(self, timeoutMinutes: Union[int, float, None] = None):
-        if timeoutMinutes is None:
+    def __init__(self, timeoutSeconds: Union[int, float, None] = None):
+        if timeoutSeconds is None:
             self.message = f"QUERY_RUN_TIMEOUT_ERROR: your query has timed out."
         else:
-            self.message = f"QUERY_RUN_TIMEOUT_ERROR: your query has timed out after {timeoutMinutes} minutes."
+            self.message = f"QUERY_RUN_TIMEOUT_ERROR: your query has timed out after {timeoutSeconds} seconds."
         super().__init__(self.message)
 
 
 class QueryRunExecutionError(BaseError):
     """
     Base class for all QueryRunExecutionError errors.
     """
```

### Comparing `shroomdk-2.0.7/src/integrations/query_integration/compass_query_integration.py` & `shroomdk-2.0.8/src/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/integrations/query_integration/query_result_set_builder.py` & `shroomdk-2.0.8/src/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/models/compass/cancel_query_run.py` & `shroomdk-2.0.8/src/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/models/compass/core/query_run.py` & `shroomdk-2.0.8/src/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/models/compass/create_query_run.py` & `shroomdk-2.0.8/src/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/models/compass/get_query_run.py` & `shroomdk-2.0.8/src/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/models/compass/get_query_run_results.py` & `shroomdk-2.0.8/src/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/models/compass/get_sql_statement.py` & `shroomdk-2.0.8/src/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/models/compass/query_results.py` & `shroomdk-2.0.8/src/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/models/query.py` & `shroomdk-2.0.8/src/models/query.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/models/query_defaults.py` & `shroomdk-2.0.8/src/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/models/query_result_set.py` & `shroomdk-2.0.8/src/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/models/query_run_stats.py` & `shroomdk-2.0.8/src/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/models/query_status.py` & `shroomdk-2.0.8/src/models/query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/tests/integrations/query_integration/test_query_compass_integration.py` & `shroomdk-2.0.8/src/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/tests/integrations/query_integration/test_query_result_set_builder.py` & `shroomdk-2.0.8/src/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/tests/models/test_query_status.py` & `shroomdk-2.0.8/src/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/tests/test_rpc.py` & `shroomdk-2.0.8/src/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/tests/utils/test_sleep.py` & `shroomdk-2.0.8/src/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.7/src/utils/sleep.py` & `shroomdk-2.0.8/src/utils/sleep.py`

 * *Files identical despite different names*

