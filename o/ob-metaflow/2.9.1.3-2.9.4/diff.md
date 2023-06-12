# Comparing `tmp/ob-metaflow-2.9.1.3.tar.gz` & `tmp/ob-metaflow-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-metaflow-2.9.1.3.tar", last modified: Tue May 16 04:30:48 2023, max compression
+gzip compressed data, was "ob-metaflow-2.9.4.tar", last modified: Mon Jun 12 20:58:32 2023, max compression
```

## Comparing `ob-metaflow-2.9.1.3.tar` & `ob-metaflow-2.9.4.tar`

### file list

```diff
@@ -1,338 +1,338 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.915501 ob-metaflow-2.9.1.3/metaflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/R.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.915501 ob-metaflow-2.9.1.3/metaflow/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.919501 ob-metaflow-2.9.1.3/metaflow/_vendor/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/_bashcomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/_termui_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/_textwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/_unicodefun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/_winconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.919501 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.919501 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/zipp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.919501 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.919501 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/zipp.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)    35131 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.919501 ob-metaflow-2.9.1.3/metaflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69157 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/client/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/client/filecache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.923501 ob-metaflow-2.9.1.3/metaflow/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32883 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cmd/configure_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cmd/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cmd/tutorials_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cmd/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cmd_with_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.923501 ob-metaflow-2.9.1.3/metaflow/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/content_addressed_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/datastore_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/datastore_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/flow_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/task_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/event_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.923501 ob-metaflow-2.9.1.3/metaflow/extension_support/
--rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/extension_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/extension_support/_empty_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/extension_support/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/extension_support/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/extension_support/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/flowspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/includefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.923501 ob-metaflow-2.9.1.3/metaflow/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metadata/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metadata/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18546 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metaflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metaflow_config_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metaflow_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metaflow_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metaflow_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.923501 ob-metaflow-2.9.1.3/metaflow/mflog/
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/mflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/mflog/mflog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/mflog/save_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/mflog/save_logs_periodically.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/mflog/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/multicore_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.927501 ob-metaflow-2.9.1.3/metaflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.927501 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.927501 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/plumbing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/plumbing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/plumbing/set_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.927501 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/base_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/external_task_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/s3_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.927501 ob-metaflow-2.9.1.3/metaflow/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_events.py
--rw-r--r--   0 runner    (1001) docker     (123)   103729 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    20011 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_workflows_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_workflows_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/process_input_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.927501 ob-metaflow-2.9.1.3/metaflow/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/aws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.931501 ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.931501 ob-metaflow-2.9.1.3/metaflow/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/secrets_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.931501 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/dynamo_db_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/event_bridge_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/production_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/schedule_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/set_batch_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42423 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.931501 ob-metaflow-2.9.1.3/metaflow/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/azure/azure_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/azure/azure_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/azure/azure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/azure/blob_service_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/azure/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.931501 ob-metaflow-2.9.1.3/metaflow/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/convert_to_native_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/renderer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/component_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/catch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/conda/batch_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda_step_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/datastores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datastores/azure_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datastores/gs_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datastores/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datastores/s3_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63477 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    42658 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3util.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/debug_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/debug_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/client_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/socket_bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/test_lib_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/data_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/exception_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/override_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/environment_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/events_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/frameworks/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_storage_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28079 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/metadata/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    20202 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/metadata/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/package_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/parallel_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/project_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/resources_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/retry_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/secrets/inline_secrets_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/secrets/secrets_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/storage_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/tag_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/test_unbounded_foreach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/timeout_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/procpoll.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/pylint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55864 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tagging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25393 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tracing_noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tracing_otel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tracing_propagator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.911501 ob-metaflow-2.9.1.3/metaflow/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/tutorials/00-helloworld/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/00-helloworld/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/00-helloworld/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/playlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/stats.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/tutorials/03-playlist-redux/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/03-playlist-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/03-playlist-redux/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/tutorials/04-playlist-plus/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/04-playlist-plus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/04-playlist-plus/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/hello-cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/metaflow/tutorials/06-statistics-redux/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/06-statistics-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/06-statistics-redux/stats.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/metaflow/tutorials/07-worldview/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/07-worldview/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/07-worldview/worldview.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/metaflow/tutorials/08-autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/08-autopilot/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/08-autopilot/autopilot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/unbounded_foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-16 04:30:48.000000 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-05-16 04:30:48.000000 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:30:48.000000 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 04:30:48.000000 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 04:30:48.000000 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 04:30:48.000000 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.158336 ob-metaflow-2.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-12 20:58:32.158336 ob-metaflow-2.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.106337 ob-metaflow-2.9.4/metaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/R.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.106337 ob-metaflow-2.9.4/metaflow/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.110337 ob-metaflow-2.9.4/metaflow/_vendor/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/_bashcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/_unicodefun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.110337 ob-metaflow-2.9.4/metaflow/_vendor/v3_5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.110337 ob-metaflow-2.9.4/metaflow/_vendor/v3_5/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_5/zipp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.110337 ob-metaflow-2.9.4/metaflow/_vendor/v3_6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.114337 ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_6/typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/_vendor/v3_6/zipp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35131 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.114337 ob-metaflow-2.9.4/metaflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69283 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/client/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/client/filecache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.114337 ob-metaflow-2.9.4/metaflow/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33431 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/cmd/configure_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/cmd/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/cmd/tutorials_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/cmd/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/cmd_with_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.114337 ob-metaflow-2.9.4/metaflow/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/datastore/content_addressed_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/datastore/datastore_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/datastore/datastore_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/datastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/datastore/flow_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/datastore/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/datastore/task_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/event_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.118337 ob-metaflow-2.9.4/metaflow/extension_support/
+-rw-r--r--   0 runner    (1001) docker     (123)    49461 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/extension_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/extension_support/_empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/extension_support/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/extension_support/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/extension_support/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/flowspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19721 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/includefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.118337 ob-metaflow-2.9.4/metaflow/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/metadata/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/metadata/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18934 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/metaflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/metaflow_config_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/metaflow_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/metaflow_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/metaflow_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.118337 ob-metaflow-2.9.4/metaflow/mflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/mflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/mflog/mflog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/mflog/save_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/mflog/save_logs_periodically.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/mflog/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/multicore_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.122337 ob-metaflow-2.9.4/metaflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.122337 ob-metaflow-2.9.4/metaflow/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31438 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/airflow/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/airflow/airflow_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/airflow/airflow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/airflow/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/airflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/airflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.122337 ob-metaflow-2.9.4/metaflow/plugins/airflow/plumbing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/airflow/plumbing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/airflow/plumbing/set_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.122337 ob-metaflow-2.9.4/metaflow/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/airflow/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/airflow/sensors/base_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/airflow/sensors/external_task_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/airflow/sensors/s3_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.126337 ob-metaflow-2.9.4/metaflow/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/argo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/argo/argo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/argo/argo_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104779 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/argo/argo_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/argo/argo_workflows_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/argo/argo_workflows_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/argo/process_input_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.126337 ob-metaflow-2.9.4/metaflow/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/aws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.130337 ob-metaflow-2.9.4/metaflow/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/batch/batch_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/batch/batch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/batch/batch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.130337 ob-metaflow-2.9.4/metaflow/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.130337 ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/dynamo_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/event_bridge_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/production_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/schedule_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/set_batch_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42423 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.134337 ob-metaflow-2.9.4/metaflow/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/azure/azure_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/azure/azure_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/azure/azure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/azure/blob_service_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/azure/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.134337 ob-metaflow-2.9.4/metaflow/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.138337 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.138337 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/convert_to_native_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/renderer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/test_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/card_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/component_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/cards/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/catch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.138337 ob-metaflow-2.9.4/metaflow/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/conda/batch_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/conda/conda_step_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.142336 ob-metaflow-2.9.4/metaflow/plugins/datastores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/datastores/azure_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/datastores/gs_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/datastores/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/datastores/s3_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.142336 ob-metaflow-2.9.4/metaflow/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/datatools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/datatools/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.142336 ob-metaflow-2.9.4/metaflow/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/datatools/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63477 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/datatools/s3/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42658 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/datatools/s3/s3op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/datatools/s3/s3tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/datatools/s3/s3util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/debug_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/debug_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.146337 ob-metaflow-2.9.4/metaflow/plugins/env_escape/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/client_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.146337 ob-metaflow-2.9.4/metaflow/plugins/env_escape/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/communication/bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/communication/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/communication/socket_bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/communication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.146337 ob-metaflow-2.9.4/metaflow/plugins/env_escape/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.146337 ob-metaflow-2.9.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.146337 ob-metaflow-2.9.4/metaflow/plugins/env_escape/configurations/test_lib_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/data_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/exception_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/override_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/env_escape/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/environment_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17724 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/events_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.146337 ob-metaflow-2.9.4/metaflow/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/frameworks/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.146337 ob-metaflow-2.9.4/metaflow/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/gcp/gs_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/gcp/gs_storage_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/gcp/gs_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/gcp/gs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/gcp/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.150337 ob-metaflow-2.9.4/metaflow/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16683 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20776 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28164 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.150337 ob-metaflow-2.9.4/metaflow/plugins/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/metadata/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20202 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/metadata/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/package_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/parallel_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/project_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/resources_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/retry_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.150337 ob-metaflow-2.9.4/metaflow/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/secrets/inline_secrets_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/secrets/secrets_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/storage_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/tag_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/test_unbounded_foreach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/plugins/timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/procpoll.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/pylint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55864 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.150337 ob-metaflow-2.9.4/metaflow/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/sidecar/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/sidecar/sidecar_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/sidecar/sidecar_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/sidecar/sidecar_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tagging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25393 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tracing_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tracing_otel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tracing_propagator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.098337 ob-metaflow-2.9.4/metaflow/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.150337 ob-metaflow-2.9.4/metaflow/tutorials/00-helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/00-helloworld/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/00-helloworld/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.154337 ob-metaflow-2.9.4/metaflow/tutorials/01-playlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/01-playlist/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/01-playlist/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/01-playlist/playlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/01-playlist/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.154337 ob-metaflow-2.9.4/metaflow/tutorials/02-statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/02-statistics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/02-statistics/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/02-statistics/stats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/02-statistics/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.154337 ob-metaflow-2.9.4/metaflow/tutorials/03-playlist-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/03-playlist-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/03-playlist-redux/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.154337 ob-metaflow-2.9.4/metaflow/tutorials/04-playlist-plus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/04-playlist-plus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/04-playlist-plus/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.154337 ob-metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/hello-cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.154337 ob-metaflow-2.9.4/metaflow/tutorials/06-statistics-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/06-statistics-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/06-statistics-redux/stats.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.154337 ob-metaflow-2.9.4/metaflow/tutorials/07-worldview/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/07-worldview/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/07-worldview/worldview.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.158336 ob-metaflow-2.9.4/metaflow/tutorials/08-autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/08-autopilot/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/tutorials/08-autopilot/autopilot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/unbounded_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/metaflow/vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:58:32.158336 ob-metaflow-2.9.4/ob_metaflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-12 20:58:32.000000 ob-metaflow-2.9.4/ob_metaflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-12 20:58:32.000000 ob-metaflow-2.9.4/ob_metaflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:58:32.000000 ob-metaflow-2.9.4/ob_metaflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-12 20:58:32.000000 ob-metaflow-2.9.4/ob_metaflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 20:58:32.000000 ob-metaflow-2.9.4/ob_metaflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 20:58:32.000000 ob-metaflow-2.9.4/ob_metaflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-12 20:58:32.158336 ob-metaflow-2.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-12 20:58:18.000000 ob-metaflow-2.9.4/setup.py
```

### Comparing `ob-metaflow-2.9.1.3/LICENSE` & `ob-metaflow-2.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/R.py` & `ob-metaflow-2.9.4/metaflow/R.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/__init__.py` & `ob-metaflow-2.9.4/metaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/__init__.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/_bashcomplete.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/_compat.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/_compat.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/_termui_impl.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/_textwrap.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/_unicodefun.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/_winconsole.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/core.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/core.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/decorators.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/decorators.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/exceptions.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/formatting.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/formatting.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/globals.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/globals.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/parser.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/parser.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/termui.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/termui.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/testing.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/testing.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/types.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/types.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/click/utils.py` & `ob-metaflow-2.9.4/metaflow/_vendor/click/utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/importlib_metadata/__init__.py` & `ob-metaflow-2.9.4/metaflow/_vendor/v3_5/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/importlib_metadata/_compat.py` & `ob-metaflow-2.9.4/metaflow/_vendor/v3_5/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/zipp.py` & `ob-metaflow-2.9.4/metaflow/_vendor/v3_5/zipp.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/__init__.py` & `ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py` & `ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_collections.py` & `ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_compat.py` & `ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_functools.py` & `ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py` & `ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_meta.py` & `ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_text.py` & `ob-metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/typing_extensions.py` & `ob-metaflow-2.9.4/metaflow/_vendor/v3_6/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/zipp.py` & `ob-metaflow-2.9.4/metaflow/_vendor/v3_6/zipp.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/cli.py` & `ob-metaflow-2.9.4/metaflow/cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/cli_args.py` & `ob-metaflow-2.9.4/metaflow/cli_args.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/client/core.py` & `ob-metaflow-2.9.4/metaflow/client/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1705,14 +1705,16 @@
         True if the run completed successfully.
     finished : bool
         True if the run completed.
     finished_at : datetime
         Time this run finished.
     code : MetaflowCode
         Code package for this run (if present). See `MetaflowCode`.
+    trigger : MetaflowTrigger
+        Information about event(s) that triggered this run (if present). See `MetaflowTrigger`.
     end_task : Task
         `Task` for the end step (if it is present already).
     """
 
     _NAME = "run"
     _PARENT_CLASS = "flow"
     _CHILD_CLASS = "step"
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/client/filecache.py` & `ob-metaflow-2.9.4/metaflow/client/filecache.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/cmd/configure_cmd.py` & `ob-metaflow-2.9.4/metaflow/cmd/configure_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -585,48 +585,61 @@
 
 def configure_argo_events(existing_env):
     env = {}
 
     # Argo events service account
     env["METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT"] = click.prompt(
         cyan("[METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT]")
-        + " Argo events service account ",
+        + " Service Account for Argo Events. ",
         default=existing_env.get("METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT", ""),
         show_default=True,
     )
 
     # Argo events event bus
     env["METAFLOW_ARGO_EVENTS_EVENT_BUS"] = click.prompt(
         cyan("[METAFLOW_ARGO_EVENTS_EVENT_BUS]")
         + yellow(" (optional)")
-        + " Argo events event bus ",
+        + " Event Bus for Argo Events.",
         default=existing_env.get("METAFLOW_ARGO_EVENTS_EVENT_BUS", "default"),
         show_default=True,
     )
 
     # Argo events event source
     env["METAFLOW_ARGO_EVENTS_EVENT_SOURCE"] = click.prompt(
-        cyan("[METAFLOW_ARGO_EVENTS_EVENT_SOURCE]") + " Argo events event source ",
+        cyan("[METAFLOW_ARGO_EVENTS_EVENT_SOURCE]") + " Event Source for Argo Events.",
         default=existing_env.get("METAFLOW_ARGO_EVENTS_EVENT_SOURCE", ""),
         show_default=True,
     )
 
     # Argo events event name
     env["METAFLOW_ARGO_EVENTS_EVENT"] = click.prompt(
-        cyan("[METAFLOW_ARGO_EVENTS_EVENT]") + " Argo events event ",
+        cyan("[METAFLOW_ARGO_EVENTS_EVENT]") + " Event name for Argo Events.",
         default=existing_env.get("METAFLOW_ARGO_EVENTS_EVENT", ""),
         show_default=True,
     )
 
     # Argo events webhook url
     env["METAFLOW_ARGO_EVENTS_WEBHOOK_URL"] = click.prompt(
-        cyan("[METAFLOW_ARGO_EVENTS_WEBHOOK_URL]") + " Argo events webhook url ",
+        cyan("[METAFLOW_ARGO_EVENTS_WEBHOOK_URL]")
+        + " Publicly accessible URL for Argo Events Webhook.",
         default=existing_env.get("METAFLOW_ARGO_EVENTS_WEBHOOK_URL", ""),
         show_default=True,
     )
+    # Set internal URL for Argo events webhook
+    env["METAFLOW_ARGO_EVENTS_INTERNAL_WEBHOOK_URL"] = click.prompt(
+        cyan("[METAFLOW_ARGO_EVENTS_INTERNAL_WEBHOOK_URL]")
+        + yellow(" (optional)")
+        + " URL for Argo Events Webhook "
+        + "(Accessible only within a Kubernetes cluster).",
+        default=existing_env.get(
+            "METAFLOW_ARGO_EVENTS_INTERNAL_WEBHOOK_URL",
+            env["METAFLOW_ARGO_EVENTS_WEBHOOK_URL"],
+        ),
+        show_default=True,
+    )
 
     return env
 
 
 def configure_kubernetes(existing_env):
     empty_profile = False
     if not existing_env:
@@ -769,15 +782,14 @@
     "-p",
     default="",
     help="Configure a named profile. Activate the profile by setting "
     "`METAFLOW_PROFILE` environment variable.",
 )
 @click.pass_context
 def azure(ctx, profile):
-
     # Greet the user!
     echo(
         "Welcome to Metaflow! Follow the prompts to configure your installation.\n",
         bold=True,
     )
 
     # Check for existing configuration.
@@ -811,15 +823,14 @@
     "-p",
     default="",
     help="Configure a named profile. Activate the profile by setting "
     "`METAFLOW_PROFILE` environment variable.",
 )
 @click.pass_context
 def gcp(ctx, profile):
-
     # Greet the user!
     echo(
         "Welcome to Metaflow! Follow the prompts to configure your installation.\n",
         bold=True,
     )
 
     # Check for existing configuration.
@@ -853,15 +864,14 @@
     "-p",
     default="",
     help="Configure a named profile. Activate the profile by setting "
     "`METAFLOW_PROFILE` environment variable.",
 )
 @click.pass_context
 def aws(ctx, profile):
-
     # Greet the user!
     echo(
         "Welcome to Metaflow! Follow the prompts to configure your " "installation.\n",
         bold=True,
     )
 
     # Check for existing configuration.
@@ -901,15 +911,14 @@
     "-p",
     default="",
     help="Configure a named profile. Activate the profile by setting "
     "`METAFLOW_PROFILE` environment variable.",
 )
 @click.pass_context
 def kubernetes(ctx, profile):
-
     check_kubernetes_client(ctx)
 
     # Greet the user!
     echo(
         "Welcome to Metaflow! Follow the prompts to configure your " "installation.\n",
         bold=True,
     )
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/cmd/main_cli.py` & `ob-metaflow-2.9.4/metaflow/cmd/main_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/cmd/tutorials_cmd.py` & `ob-metaflow-2.9.4/metaflow/cmd/tutorials_cmd.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/cmd_with_io.py` & `ob-metaflow-2.9.4/metaflow/cmd_with_io.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/current.py` & `ob-metaflow-2.9.4/metaflow/current.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/datastore/content_addressed_store.py` & `ob-metaflow-2.9.4/metaflow/datastore/content_addressed_store.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/datastore/datastore_set.py` & `ob-metaflow-2.9.4/metaflow/datastore/datastore_set.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/datastore/datastore_storage.py` & `ob-metaflow-2.9.4/metaflow/datastore/datastore_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/datastore/flow_datastore.py` & `ob-metaflow-2.9.4/metaflow/datastore/flow_datastore.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/datastore/task_datastore.py` & `ob-metaflow-2.9.4/metaflow/datastore/task_datastore.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/debug.py` & `ob-metaflow-2.9.4/metaflow/debug.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/decorators.py` & `ob-metaflow-2.9.4/metaflow/decorators.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/event_logger.py` & `ob-metaflow-2.9.4/metaflow/event_logger.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/events.py` & `ob-metaflow-2.9.4/metaflow/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -134,15 +134,21 @@
                 if obj.type == "run"
             ]
 
         return list(self._runs) or None
 
     def __getitem__(self, key):
         """
-        If triggering events are runs, `key` corresponds to the flow name of the triggering run. Returns a triggering `Run` object corresponding to the key. If triggering events are not runs, `key` corresponds to the event name and a `MetaflowEvent` object is returned.
+        If triggering events are runs, `key` corresponds to the flow name of the triggering run.
+        Otherwise, `key` corresponds to the event name and a `MetaflowEvent` object is returned.
+
+        Returns
+        -------
+        Run or MetaflowEvent
+            `Run` object if triggered by a run. Otherwise returns a `MetaflowEvent`.
         """
         if self.runs:
             for run in self.runs:
                 if run.path_components[0] == key:
                     return run
         elif self.events:
             for event in self.events:
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/exception.py` & `ob-metaflow-2.9.4/metaflow/exception.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/extension_support/__init__.py` & `ob-metaflow-2.9.4/metaflow/extension_support/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,27 +380,32 @@
     meta_to_pkg = defaultdict(list)
 
     # 1st step: look for distributions (the common case)
     for dist in metadata.distributions():
         if any(
             [pkg == EXT_PKG for pkg in (dist.read_text("top_level.txt") or "").split()]
         ):
+            # In all cases (whether duplicate package or not), we remove the package
+            # from the list of locations to look in.
+            # This is not 100% accurate because it is possible that at the same
+            # location there is a package and a non-package, but this is extremely
+            # unlikely so we are going to ignore this case.
+            dist_root = dist.locate_file(EXT_PKG).as_posix()
+            all_paths.discard(dist_root)
+
             if dist.metadata["Name"] in mf_ext_packages:
                 _ext_debug(
                     "Ignoring duplicate package '%s' (duplicate paths in sys.path? (%s))"
                     % (dist.metadata["Name"], str(sys.path))
                 )
                 continue
-            _ext_debug("Found extension package '%s'..." % dist.metadata["Name"])
-
-            # Remove the path from the paths to search. This is not 100% accurate because
-            # it is possible that at that same location there is a package and a non-package,
-            # but it is exceedingly unlikely, so we are going to ignore this.
-            dist_root = dist.locate_file(EXT_PKG).as_posix()
-            all_paths.discard(dist_root)
+            _ext_debug(
+                "Found extension package '%s' at '%s'..."
+                % (dist.metadata["Name"], dist_root)
+            )
 
             files_to_include = []
             meta_module = None
 
             # At this point, we check to see what extension points this package
             # contributes to. This is to enable multiple namespace packages to contribute
             # to the same extension point (for example, you may have multiple packages
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/extension_support/cmd.py` & `ob-metaflow-2.9.4/metaflow/extension_support/cmd.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/extension_support/integrations.py` & `ob-metaflow-2.9.4/metaflow/extension_support/integrations.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/extension_support/plugins.py` & `ob-metaflow-2.9.4/metaflow/extension_support/plugins.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/flowspec.py` & `ob-metaflow-2.9.4/metaflow/flowspec.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/graph.py` & `ob-metaflow-2.9.4/metaflow/graph.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/includefile.py` & `ob-metaflow-2.9.4/metaflow/includefile.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,18 +140,21 @@
                 flow_name=ctx.obj.flow.name,
                 user_name=get_username(),
                 parameter_name=param.name,
                 logger=ctx.obj.echo,
                 ds_type=ctx.obj.datastore_impl.TYPE,
             )
 
-        if len(value) > 0 and value[0] == "{":
+        if len(value) > 0 and (value.startswith("{") or value.startswith('"{')):
             # This is a blob; no URL starts with `{`. We are thus in scenario A
             try:
                 value = json.loads(value)
+                # to handle quoted json strings
+                if not isinstance(value, dict):
+                    value = json.loads(value)
             except json.JSONDecodeError as e:
                 raise MetaflowException(
                     "IncludeFile '%s' (value: %s) is malformed" % (param.name, value)
                 )
             # All processing has already been done, so we just convert to an `IncludedFile`
             return IncludedFile(value)
 
@@ -425,15 +428,14 @@
         handler = DATACLIENTS.get(prefix)
         if handler is None:
             raise MetaflowException("Could not find data client for '%s'" % prefix)
         return handler
 
 
 class UploaderV2:
-
     file_type = "uploader-v2"
 
     @classmethod
     def encode_url(cls, url_type, url, **kwargs):
         return_value = {
             "note": "Internal representation of IncludeFile(%s)" % url,
             "type": cls.file_type,
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/integrations.py` & `ob-metaflow-2.9.4/metaflow/integrations.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/lint.py` & `ob-metaflow-2.9.4/metaflow/lint.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/metadata/heartbeat.py` & `ob-metaflow-2.9.4/metaflow/metadata/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/metadata/metadata.py` & `ob-metaflow-2.9.4/metaflow/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/metadata/util.py` & `ob-metaflow-2.9.4/metaflow/metadata/util.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/metaflow_config.py` & `ob-metaflow-2.9.4/metaflow/metaflow_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 DEFAULT_ENVIRONMENT = from_conf("DEFAULT_ENVIRONMENT", "local")
 DEFAULT_EVENT_LOGGER = from_conf("DEFAULT_EVENT_LOGGER", "nullSidecarLogger")
 DEFAULT_METADATA = from_conf("DEFAULT_METADATA", "local")
 DEFAULT_MONITOR = from_conf("DEFAULT_MONITOR", "nullSidecarMonitor")
 DEFAULT_PACKAGE_SUFFIXES = from_conf("DEFAULT_PACKAGE_SUFFIXES", ".py,.R,.RDS")
 DEFAULT_AWS_CLIENT_PROVIDER = from_conf("DEFAULT_AWS_CLIENT_PROVIDER", "boto3")
 DEFAULT_SECRETS_BACKEND_TYPE = from_conf("DEFAULT_SECRETS_BACKEND_TYPE")
+DEFAULT_SECRETS_ROLE = from_conf("DEFAULT_SECRETS_ROLE")
 
 ###
 # User configuration
 ###
 USER = from_conf("USER")
 
 
@@ -273,20 +274,24 @@
 # Default node selectors to use by K8S jobs created by Metaflow - foo=bar,baz=bab
 KUBERNETES_NODE_SELECTOR = from_conf("KUBERNETES_NODE_SELECTOR", "")
 KUBERNETES_TOLERATIONS = from_conf("KUBERNETES_TOLERATIONS", "")
 KUBERNETES_PERSISTENT_VOLUME_CLAIMS = from_conf(
     "KUBERNETES_PERSISTENT_VOLUME_CLAIMS", ""
 )
 KUBERNETES_SECRETS = from_conf("KUBERNETES_SECRETS", "")
+# Default labels for kubernetes pods
+KUBERNETES_LABELS = from_conf("KUBERNETES_LABELS", "")
 # Default GPU vendor to use by K8S jobs created by Metaflow (supports nvidia, amd)
 KUBERNETES_GPU_VENDOR = from_conf("KUBERNETES_GPU_VENDOR", "nvidia")
 # Default container image for K8S
 KUBERNETES_CONTAINER_IMAGE = from_conf(
     "KUBERNETES_CONTAINER_IMAGE", DEFAULT_CONTAINER_IMAGE
 )
+# Image pull policy for container images
+KUBERNETES_IMAGE_PULL_POLICY = from_conf("KUBERNETES_IMAGE_PULL_POLICY", None)
 # Default container registry for K8S
 KUBERNETES_CONTAINER_REGISTRY = from_conf(
     "KUBERNETES_CONTAINER_REGISTRY", DEFAULT_CONTAINER_REGISTRY
 )
 # Toggle for trying to fetch EC2 instance metadata
 KUBERNETES_FETCH_EC2_METADATA = from_conf("KUBERNETES_FETCH_EC2_METADATA", False)
 
@@ -297,14 +302,17 @@
 # Argo Events Configuration
 ##
 ARGO_EVENTS_SERVICE_ACCOUNT = from_conf("ARGO_EVENTS_SERVICE_ACCOUNT")
 ARGO_EVENTS_EVENT_BUS = from_conf("ARGO_EVENTS_EVENT_BUS", "default")
 ARGO_EVENTS_EVENT_SOURCE = from_conf("ARGO_EVENTS_EVENT_SOURCE")
 ARGO_EVENTS_EVENT = from_conf("ARGO_EVENTS_EVENT")
 ARGO_EVENTS_WEBHOOK_URL = from_conf("ARGO_EVENTS_WEBHOOK_URL")
+ARGO_EVENTS_INTERNAL_WEBHOOK_URL = from_conf(
+    "ARGO_EVENTS_INTERNAL_WEBHOOK_URL", ARGO_EVENTS_WEBHOOK_URL
+)
 
 ARGO_WORKFLOWS_UI_URL = from_conf("ARGO_WORKFLOWS_UI_URL")
 
 ##
 # Airflow Configuration
 ##
 # This configuration sets `startup_timeout_seconds` in airflow's KubernetesPodOperator.
@@ -336,15 +344,15 @@
 
 ###
 # Debug configuration
 ###
 DEBUG_OPTIONS = ["subcommand", "sidecar", "s3client"]
 
 for typ in DEBUG_OPTIONS:
-    vars()["DEBUG_%s" % typ.upper()] = from_conf("DEBUG_%s" % typ.upper())
+    vars()["DEBUG_%s" % typ.upper()] = from_conf("DEBUG_%s" % typ.upper(), False)
 
 ###
 # Plugin configuration
 ###
 
 # Plugin configuration variables exist in plugins/__init__.py.
 # Specifically, there is an ENABLED_<category> configuration value to determine
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/metaflow_config_funcs.py` & `ob-metaflow-2.9.4/metaflow/metaflow_config_funcs.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,33 +75,45 @@
             else:
                 try:
                     value = json.loads(value)
                 except json.JSONDecodeError:
                     raise ValueError(
                         "Expected a valid JSON for %s, got: %s" % (env_name, value)
                     )
+                if type(value) != type(default):
+                    raise ValueError(
+                        "Expected value of type '%s' for %s, got: %s"
+                        % (type(default), env_name, value)
+                    )
+                is_default = value == default
             _all_configs[env_name] = ConfigValue(
                 value=value,
                 serializer=json.dumps,
                 is_default=is_default,
             )
             return value
         elif isinstance(default, (bool, int, float)) or is_stringish(default):
             try:
-                value = type(default)(value)
-                # Here we can compare values
+                if type(value) != type(default):
+                    if isinstance(default, bool):
+                        # Env vars are strings so try to evaluate logically
+                        value = value.lower() not in ("0", "false", "")
+                    else:
+                        value = type(default)(value)
                 is_default = value == default
             except ValueError:
                 raise ValueError(
                     "Expected a %s for %s, got: %s" % (type(default), env_name, value)
                 )
         else:
             raise RuntimeError(
                 "Default of type %s for %s is not supported" % (type(default), env_name)
             )
+    else:
+        is_default = value is None
     _all_configs[env_name] = ConfigValue(
         value=value,
         serializer=str,
         is_default=is_default,
     )
     return value
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/metaflow_environment.py` & `ob-metaflow-2.9.4/metaflow/metaflow_environment.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/metaflow_version.py` & `ob-metaflow-2.9.4/metaflow/metaflow_version.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/mflog/__init__.py` & `ob-metaflow-2.9.4/metaflow/mflog/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/mflog/mflog.py` & `ob-metaflow-2.9.4/metaflow/mflog/mflog.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/mflog/save_logs.py` & `ob-metaflow-2.9.4/metaflow/mflog/save_logs.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/mflog/save_logs_periodically.py` & `ob-metaflow-2.9.4/metaflow/mflog/save_logs_periodically.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/mflog/tee.py` & `ob-metaflow-2.9.4/metaflow/mflog/tee.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/monitor.py` & `ob-metaflow-2.9.4/metaflow/monitor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/multicore_utils.py` & `ob-metaflow-2.9.4/metaflow/multicore_utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/package.py` & `ob-metaflow-2.9.4/metaflow/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,21 +152,24 @@
     def _add_info(self, tar):
         info = tarfile.TarInfo(os.path.basename(INFO_FILE))
         env = self.environment.get_environment_info(include_ext_info=True)
         buf = BytesIO()
         buf.write(json.dumps(env).encode("utf-8"))
         buf.seek(0)
         info.size = len(buf.getvalue())
+        # Setting this default to Dec 3, 2019
+        info.mtime = 1575360000
         tar.addfile(info, buf)
 
     def _make(self):
         def no_mtime(tarinfo):
             # a modification time change should not change the hash of
             # the package. Only content modifications will.
-            tarinfo.mtime = 0
+            # Setting this default to Dec 3, 2019
+            tarinfo.mtime = 1575360000
             return tarinfo
 
         buf = BytesIO()
         with tarfile.open(
             fileobj=buf, mode="w:gz", compresslevel=3, dereference=True
         ) as tar:
             self._add_info(tar)
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/parameters.py` & `ob-metaflow-2.9.4/metaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/__init__.py` & `ob-metaflow-2.9.4/metaflow/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow.py` & `ob-metaflow-2.9.4/metaflow/plugins/airflow/airflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,18 +638,23 @@
             kube_deco = dict(
                 [deco for deco in node.decorators if deco.name == "kubernetes"][
                     0
                 ].attributes
             )
             if kube_deco:
                 # Only guard against use_tmpfs and tmpfs_size as these determine if tmpfs is enabled.
-                for attr in ["use_tmpfs", "tmpfs_size", "persistent_volume_claims"]:
+                for attr in [
+                    "use_tmpfs",
+                    "tmpfs_size",
+                    "persistent_volume_claims",
+                    "image_pull_policy",
+                ]:
                     if kube_deco[attr]:
                         raise AirflowException(
-                            "tmpfs attribute *%s* is currently not supported on Airflow "
+                            "The decorator attribute *%s* is currently not supported on Airflow "
                             "for the @kubernetes decorator on step *%s*"
                             % (attr, node.name)
                         )
 
             parent_is_foreach = any(  # Any immediate parent is a foreach node.
                 self.graph[n].type == "foreach" for n in node.in_funcs
             )
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow_cli.py` & `ob-metaflow-2.9.4/metaflow/plugins/airflow/airflow_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/airflow/airflow_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow_utils.py` & `ob-metaflow-2.9.4/metaflow/plugins/airflow/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/plumbing/set_parameters.py` & `ob-metaflow-2.9.4/metaflow/plugins/airflow/plumbing/set_parameters.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/base_sensor.py` & `ob-metaflow-2.9.4/metaflow/plugins/airflow/sensors/base_sensor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/external_task_sensor.py` & `ob-metaflow-2.9.4/metaflow/plugins/airflow/sensors/external_task_sensor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/s3_sensor.py` & `ob-metaflow-2.9.4/metaflow/plugins/airflow/sensors/s3_sensor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_client.py` & `ob-metaflow-2.9.4/metaflow/plugins/argo/argo_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_workflows.py` & `ob-metaflow-2.9.4/metaflow/plugins/argo/argo_workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,39 +11,44 @@
 from metaflow.decorators import flow_decorators
 from metaflow.exception import MetaflowException
 from metaflow.metaflow_config import (
     ARGO_EVENTS_EVENT,
     ARGO_EVENTS_EVENT_BUS,
     ARGO_EVENTS_EVENT_SOURCE,
     ARGO_EVENTS_SERVICE_ACCOUNT,
-    ARGO_EVENTS_WEBHOOK_URL,
+    ARGO_EVENTS_INTERNAL_WEBHOOK_URL,
     ARGO_WORKFLOWS_ENV_VARS_TO_SKIP,
     ARGO_WORKFLOWS_KUBERNETES_SECRETS,
     AWS_SECRETS_MANAGER_DEFAULT_REGION,
     AZURE_STORAGE_BLOB_SERVICE_ENDPOINT,
     CARD_AZUREROOT,
     CARD_GSROOT,
     CARD_S3ROOT,
     DATASTORE_SYSROOT_AZURE,
     DATASTORE_SYSROOT_GS,
     DATASTORE_SYSROOT_S3,
     DATATOOLS_S3ROOT,
     DEFAULT_METADATA,
     DEFAULT_SECRETS_BACKEND_TYPE,
     KUBERNETES_FETCH_EC2_METADATA,
+    KUBERNETES_LABELS,
     KUBERNETES_NAMESPACE,
     KUBERNETES_NODE_SELECTOR,
     KUBERNETES_SANDBOX_INIT_SCRIPT,
     KUBERNETES_SECRETS,
     S3_ENDPOINT_URL,
     SERVICE_HEADERS,
     SERVICE_INTERNAL_URL,
 )
 from metaflow.mflog import BASH_SAVE_LOGS, bash_capture_logs, export_mflog_env_vars
 from metaflow.parameters import deploy_time_eval
+from metaflow.plugins.kubernetes.kubernetes import (
+    parse_kube_keyvalue_list,
+    validate_kube_labels,
+)
 from metaflow.util import (
     compress_list,
     dict_to_cli_options,
     to_bytes,
     to_camelcase,
     to_unicode,
 )
@@ -142,14 +147,15 @@
         self.notify_on_success = notify_on_success
         self.notify_slack_webhook_url = notify_slack_webhook_url
 
         self.parameters = self._process_parameters()
         self.triggers, self.trigger_options = self._process_triggers()
         self._schedule, self._timezone = self._get_schedule()
 
+        self.kubernetes_labels = self._get_kubernetes_labels()
         self._workflow_template = self._compile_workflow_template()
         self._sensor = self._compile_sensor()
 
     def __str__(self):
         return str(self._workflow_template)
 
     def deploy(self):
@@ -197,14 +203,27 @@
         try:
             return ArgoClient(namespace=KUBERNETES_NAMESPACE).trigger_workflow_template(
                 name, parameters
             )
         except Exception as e:
             raise ArgoWorkflowsException(str(e))
 
+    @staticmethod
+    def _get_kubernetes_labels():
+        """
+        Get Kubernetes labels from environment variable.
+        Parses the string into a dict and validates that values adhere to Kubernetes restrictions.
+        """
+        if not KUBERNETES_LABELS:
+            return {}
+        env_labels = KUBERNETES_LABELS.split(",")
+        env_labels = parse_kube_keyvalue_list(env_labels, False)
+        validate_kube_labels(env_labels)
+        return env_labels
+
     def _get_schedule(self):
         schedule = self.flow._flow_decorators.get("schedule")
         if schedule:
             # Remove the field "Year" if it exists
             schedule = schedule[0]
             return " ".join(schedule.schedule.split()[:5]), schedule.timezone
         return None, None
@@ -421,17 +440,21 @@
             options = self.flow._flow_decorators.get("trigger_on_finish")[0].options
 
         for event in triggers:
             # Assign a sanitized name since we need this at many places to please
             # Argo Events sensors. There is a slight possibility of name collision
             # but quite unlikely for us to worry about at this point.
             event["sanitized_name"] = event["name"]
-            if any([x in event["name"] for x in [".", "-"]]):
+            if any([x in event["name"] for x in [".", "-", "@", "+"]]):
                 event["sanitized_name"] = "%s_%s" % (
-                    event["name"].replace(".", "").replace("-", ""),
+                    event["name"]
+                    .replace(".", "")
+                    .replace("-", "")
+                    .replace("@", "")
+                    .replace("+", ""),
                     to_unicode(
                         base64.b32encode(sha1(to_bytes(event["name"])).digest())
                     )[:4].lower(),
                 )
         return triggers, options
 
     def _compile_workflow_template(self):
@@ -553,14 +576,15 @@
                 )
                 # Set common pod metadata.
                 .pod_metadata(
                     Metadata()
                     .label("app.kubernetes.io/name", "metaflow-task")
                     .label("app.kubernetes.io/part-of", "metaflow")
                     .annotations(annotations)
+                    .labels(self.kubernetes_labels)
                 )
                 # Set the entrypoint to flow name
                 .entrypoint(self.flow.name)
                 # Set exit hook handlers if notifications are enabled
                 .hooks(
                     {
                         **(
@@ -1029,15 +1053,15 @@
                     **{
                         # Configuration for Argo Events. Keep these in sync with the
                         # environment variables for @kubernetes decorator.
                         "METAFLOW_ARGO_EVENTS_EVENT": ARGO_EVENTS_EVENT,
                         "METAFLOW_ARGO_EVENTS_EVENT_BUS": ARGO_EVENTS_EVENT_BUS,
                         "METAFLOW_ARGO_EVENTS_EVENT_SOURCE": ARGO_EVENTS_EVENT_SOURCE,
                         "METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT": ARGO_EVENTS_SERVICE_ACCOUNT,
-                        "METAFLOW_ARGO_EVENTS_WEBHOOK_URL": ARGO_EVENTS_WEBHOOK_URL,
+                        "METAFLOW_ARGO_EVENTS_WEBHOOK_URL": ARGO_EVENTS_INTERNAL_WEBHOOK_URL,
                     },
                     **{
                         # Some optional values for bookkeeping
                         "METAFLOW_FLOW_NAME": self.flow.name,
                         "METAFLOW_STEP_NAME": node.name,
                         "METAFLOW_RUN_ID": run_id,
                         # "METAFLOW_TASK_ID": task_id,
@@ -1168,14 +1192,15 @@
                     "tmpfs-ephemeral-volume",
                     medium="Memory",
                     size_limit=tmpfs_size if tmpfs_enabled else 0,
                 )
                 .pvc_volumes(resources.get("persistent_volume_claims"))
                 # Set node selectors
                 .node_selectors(resources.get("node_selector"))
+                # Set tolerations
                 .tolerations(resources.get("tolerations"))
                 # Set container
                 .container(
                     # TODO: Unify the logic with kubernetes.py
                     # Important note - Unfortunately, V1Container uses snakecase while
                     # Argo Workflows uses camel. For most of the attributes, both cases
                     # are indistinguishable, but unfortunately, not for all - (
@@ -1207,14 +1232,15 @@
                                     "METAFLOW_KUBERNETES_POD_NAME": "metadata.name",
                                     "METAFLOW_KUBERNETES_POD_ID": "metadata.uid",
                                     "METAFLOW_KUBERNETES_SERVICE_ACCOUNT_NAME": "spec.serviceAccountName",
                                     "METAFLOW_KUBERNETES_NODE_IP": "status.hostIP",
                                 }.items()
                             ],
                             image=resources["image"],
+                            image_pull_policy=resources["image_pull_policy"],
                             resources=kubernetes_sdk.V1ResourceRequirements(
                                 requests={
                                     "cpu": str(resources["cpu"]),
                                     "memory": "%sM" % str(resources["memory"]),
                                     "ephemeral-storage": "%sM" % str(resources["disk"]),
                                 },
                                 limits={
@@ -1380,38 +1406,38 @@
         if ARGO_EVENTS_EVENT is None:
             raise ArgoWorkflowsException(
                 "An Argo Event name hasn't been configured for your deployment yet. "
                 "Please see this article for more details on event names - "
                 "https://argoproj.github.io/argo-events/eventsources/naming/. "
                 "It is very likely that all events for your deployment share the "
                 "same name. You can configure it by executing "
-                "`metaflow configure events` or setting METAFLOW_ARGO_EVENTS_EVENT "
+                "`metaflow configure kubernetes` or setting METAFLOW_ARGO_EVENTS_EVENT "
                 "in your configuration. If in doubt, reach out for support at "
                 "http://chat.metaflow.org"
             )
         # Unfortunately argo events requires knowledge of event source today.
         # Hopefully, some day this requirement can be removed and events can be truly
         # impervious to their source and destination.
         if ARGO_EVENTS_EVENT_SOURCE is None:
             raise ArgoWorkflowsException(
                 "An Argo Event Source name hasn't been configured for your deployment "
                 "yet. Please see this article for more details on event names - "
                 "https://argoproj.github.io/argo-events/eventsources/naming/. "
-                "You can configure it by executing `metaflow configure events` or "
+                "You can configure it by executing `metaflow configure kubernetes` or "
                 "setting METAFLOW_ARGO_EVENTS_EVENT_SOURCE in your configuration. If "
                 "in doubt, reach out for support at http://chat.metaflow.org"
             )
         # Service accounts are a hard requirement since we utilize the
         # argoWorkflow trigger for resource sensors today.
         if ARGO_EVENTS_SERVICE_ACCOUNT is None:
             raise ArgoWorkflowsException(
                 "An Argo Event service account hasn't been configured for your "
                 "deployment yet. Please see this article for more details on event "
                 "names - https://argoproj.github.io/argo-events/service-accounts/. "
-                "You can configure it by executing `metaflow configure events` or "
+                "You can configure it by executing `metaflow configure kubernetes` or "
                 "setting METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT in your configuration. "
                 "If in doubt, reach out for support at http://chat.metaflow.org"
             )
 
         try:
             # Kubernetes is a soft dependency for generating Argo objects.
             # We can very well remove this dependency for Argo with the downside of
@@ -1445,14 +1471,15 @@
             .metadata(
                 # Sensor metadata.
                 ObjectMeta()
                 .name(self.name.replace(".", "-"))
                 .namespace(KUBERNETES_NAMESPACE)
                 .label("app.kubernetes.io/name", "metaflow-sensor")
                 .label("app.kubernetes.io/part-of", "metaflow")
+                .labels(self.kubernetes_labels)
                 .annotations(annotations)
             )
             .spec(
                 SensorSpec().template(
                     # Sensor template.
                     SensorTemplate()
                     .metadata(
@@ -1730,15 +1757,15 @@
     def label(self, key, value):
         self.payload["labels"][key] = str(value)
         return self
 
     def labels(self, labels):
         if "labels" not in self.payload:
             self.payload["labels"] = {}
-        self.payload["labels"].update(labels)
+        self.payload["labels"].update(labels or {})
         return self
 
     def name(self, name):
         self.payload["name"] = name
         return self
 
     def namespace(self, namespace):
@@ -1847,15 +1874,15 @@
     def label(self, key, value):
         self.payload["labels"][key] = str(value)
         return self
 
     def labels(self, labels):
         if "labels" not in self.payload:
             self.payload["labels"] = {}
-        self.payload["labels"].update(labels)
+        self.payload["labels"].update(labels or {})
         return self
 
     def labels_from(self, labels_from):
         # Only available in workflow_metadata
         # https://github.com/argoproj/argo-workflows/blob/master/examples/label-value-from-workflow.yaml
         if "labelsFrom" not in self.payload:
             self.payload["labelsFrom"] = {}
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_workflows_cli.py` & `ob-metaflow-2.9.4/metaflow/plugins/argo/argo_workflows_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,25 +322,29 @@
             % to_unicode(base64.b32encode(sha1(project_branch).digest()))[:16]
         )
         is_project = True
         # Argo Workflow names can't be longer than 253 characters, so we truncate
         # by default. Also, while project and branch allow for underscores, Argo
         # Workflows doesn't (DNS Subdomain names as defined in RFC 1123) - so we will
         # remove any underscores as well as convert the name to lower case.
+        # Also remove + and @ as not allowed characters, which can be part of the
+        # project branch due to using email addresses as user names.
         if len(workflow_name) > 253:
             name_hash = to_unicode(
                 base64.b32encode(sha1(to_bytes(workflow_name)).digest())
             )[:8].lower()
             workflow_name = "%s-%s" % (workflow_name[:242], name_hash)
             obj._is_workflow_name_modified = True
         if not VALID_NAME.search(workflow_name):
             workflow_name = (
                 re.compile(r"^[^A-Za-z0-9]+")
                 .sub("", workflow_name)
                 .replace("_", "")
+                .replace("@", "")
+                .replace("+", "")
                 .lower()
             )
             obj._is_workflow_name_modified = True
     else:
         if name and not VALID_NAME.search(name):
             raise MetaflowException(
                 "Name '%s' contains invalid characters. The "
@@ -363,14 +367,16 @@
             raise ArgoWorkflowsNameTooLong(msg)
 
         if not VALID_NAME.search(workflow_name):
             workflow_name = (
                 re.compile(r"^[^A-Za-z0-9]+")
                 .sub("", workflow_name)
                 .replace("_", "")
+                .replace("@", "")
+                .replace("+", "")
                 .lower()
             )
             obj._is_workflow_name_modified = True
 
     return workflow_name, token_prefix.lower(), is_project
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_workflows_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/argo/argo_workflows_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/argo/process_input_paths.py` & `ob-metaflow-2.9.4/metaflow/plugins/argo/process_input_paths.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/aws_client.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/aws_utils.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/aws_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             raise MetaflowException(
                 "Step %s requires %s CPU units, but you cannot use more than %s per step in this environment"
                 % (step_name, result["cpu"], MAX_CPU_PER_TASK)
             )
     if "memory" in result and MAX_MEMORY_PER_TASK:
         if float(result["memory"]) > float(MAX_MEMORY_PER_TASK):
             raise MetaflowException(
-                "Step %s requires %s CPU units, but you cannot use more than %s per step in this environment"
+                "Step %s requires %s memory, but you cannot use more than %s per step in this environment"
                 % (step_name, result["memory"], MAX_MEMORY_PER_TASK)
             )
 
     return result
 
 
 def sanitize_batch_tag(key, value):
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/batch/batch.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch_cli.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/batch/batch_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch_client.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/batch/batch_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/batch/batch_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     """
     return key.replace("-", "_").replace(".", "_")
 
 
 class AwsSecretsManagerSecretsProvider(SecretsProvider):
     TYPE = "aws-secrets-manager"
 
-    def get_secret_as_dict(self, secret_id, options={}):
+    def get_secret_as_dict(self, secret_id, options={}, role=None):
         """
         Reads a secret from AWS Secrets Manager and returns it as a dictionary of environment variables.
 
         The secret payload from AWS is EITHER a string OR a binary blob.
 
         If the secret contains a string payload ("SecretString"):
         - if the `parse_secret_string_as_json` option is True (default):
@@ -61,34 +61,38 @@
         - The result dic contains '{SecretName}': '{SecretBinary}', where {SecretBinary} is a base64-encoded string
 
         All keys in the result are sanitized to be more valid environment variable names. This is done on a best effort
         basis. Further validation is expected to be done by the invoking @secrets decorator itself.
 
         :param secret_id: ARN or friendly name of the secret
         :param options: unused
+        :param role: AWS IAM Role ARN to assume before reading the secret
         :return: dict of environment variables. All keys and values are strings.
         """
         import botocore
         from metaflow.plugins.aws.aws_client import get_aws_client
 
         effective_aws_region = None
         # arn:aws:secretsmanager:<Region>:<AccountId>:secret:SecretName-6RandomCharacters
         m = re.match("arn:aws:secretsmanager:([^:]+):", secret_id)
         if m:
             effective_aws_region = m.group(1)
         elif "region" in options:
             effective_aws_region = options["region"]
         else:
             effective_aws_region = AWS_SECRETS_MANAGER_DEFAULT_REGION
+
         # At the end of all that, `effective_aws_region` may still be None.
         # This might still be OK, if there is fallback AWS region info in environment like:
         # .aws/config or AWS_REGION env var or AWS_DEFAULT_REGION env var, etc.
         try:
             secrets_manager_client = get_aws_client(
-                "secretsmanager", client_params={"region_name": effective_aws_region}
+                "secretsmanager",
+                client_params={"region_name": effective_aws_region},
+                role_arn=role,
             )
         except botocore.exceptions.NoRegionError:
             # We try our best with a nice error message.
             # When run in Kubernetes or Argo Workflows, the traceback is still monstrous.
             # TODO: Find a way to show a concise error in logs
             raise MetaflowException(
                 "Default region is not specified for AWS Secrets Manager. Please set METAFLOW_AWS_SECRETS_MANAGER_DEFAULT_REGION"
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/dynamo_db_client.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/dynamo_db_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/event_bridge_client.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/event_bridge_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/production_token.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/production_token.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/schedule_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/set_batch_environment.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/set_batch_environment.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions_cli.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions_client.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/azure/azure_tail.py` & `ob-metaflow-2.9.4/metaflow/plugins/azure/azure_tail.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/azure/azure_utils.py` & `ob-metaflow-2.9.4/metaflow/plugins/azure/azure_utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/azure/blob_service_client_factory.py` & `ob-metaflow-2.9.4/metaflow/plugins/azure/blob_service_client_factory.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/azure/includefile_support.py` & `ob-metaflow-2.9.4/metaflow/plugins/azure/includefile_support.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_cli.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_client.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_datastore.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_datastore.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/__init__.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/base.html` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/base.html`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/basic.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/basic.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/bundle.css` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/bundle.css`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/card.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/card.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         try:
             from . import chevron as pt
 
             return pt
         except ImportError:
             return None
 
-    def render(self, task: "Task") -> str:
+    def render(self, task) -> str:
         """
         Produce custom card contents in HTML.
 
         Subclasses override this method to customize the card contents.
 
         Parameters
         ----------
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/main.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/main.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/renderer.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/renderer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/tokenizer.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/components.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/components.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/convert_to_native_type.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/convert_to_native_type.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/main.js` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/main.js`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/renderer_tools.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/renderer_tools.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/test_cards.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_modules/test_cards.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_resolver.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/card_resolver.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/component_serializer.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/component_serializer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/cards/exception.py` & `ob-metaflow-2.9.4/metaflow/plugins/cards/exception.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/catch_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/catch_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/conda/__init__.py` & `ob-metaflow-2.9.4/metaflow/plugins/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/conda/batch_bootstrap.py` & `ob-metaflow-2.9.4/metaflow/plugins/conda/batch_bootstrap.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda.py` & `ob-metaflow-2.9.4/metaflow/plugins/conda/conda.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda_environment.py` & `ob-metaflow-2.9.4/metaflow/plugins/conda/conda_environment.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda_flow_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda_step_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/conda/conda_step_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/datastores/azure_storage.py` & `ob-metaflow-2.9.4/metaflow/plugins/datastores/azure_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/datastores/gs_storage.py` & `ob-metaflow-2.9.4/metaflow/plugins/datastores/gs_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/datastores/local_storage.py` & `ob-metaflow-2.9.4/metaflow/plugins/datastores/local_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/datastores/s3_storage.py` & `ob-metaflow-2.9.4/metaflow/plugins/datastores/s3_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/datatools/__init__.py` & `ob-metaflow-2.9.4/metaflow/plugins/datatools/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/datatools/local.py` & `ob-metaflow-2.9.4/metaflow/plugins/datatools/local.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3.py` & `ob-metaflow-2.9.4/metaflow/plugins/datatools/s3/s3.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3op.py` & `ob-metaflow-2.9.4/metaflow/plugins/datatools/s3/s3op.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3tail.py` & `ob-metaflow-2.9.4/metaflow/plugins/datatools/s3/s3tail.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3util.py` & `ob-metaflow-2.9.4/metaflow/plugins/datatools/s3/s3util.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/debug_logger.py` & `ob-metaflow-2.9.4/metaflow/plugins/debug_logger.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/debug_monitor.py` & `ob-metaflow-2.9.4/metaflow/plugins/debug_monitor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/__init__.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/client.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,28 @@
 from .stub import create_class
 
 BIND_TIMEOUT = 0.1
 BIND_RETRY = 0
 
 
 class Client(object):
-    def __init__(self, python_executable, pythonpath, max_pickle_version, config_dir):
+    def __init__(
+        self, modules, python_executable, pythonpath, max_pickle_version, config_dir
+    ):
+        # Wrap with ImportError so that if users are just using the escaped module
+        # as optional, the typical logic of catching ImportError works properly
+        try:
+            self.inner_init(
+                python_executable, pythonpath, max_pickle_version, config_dir
+            )
+        except Exception as e:
+            # Typically it's one override per config so we just use the first one.
+            raise ImportError("Error loading module: %s" % str(e), name=modules[0])
+
+    def inner_init(self, python_executable, pythonpath, max_pickle_version, config_dir):
         # Make sure to init these variables (used in __del__) early on in case we
         # have an exception
         self._poller = None
         self._poller_lock = threading.Lock()
         self._server_process = None
         self._socket_path = None
 
@@ -81,20 +94,25 @@
         )
 
         # Read override configuration
         # We can't just import the "overrides" module because that does not
         # distinguish it from other modules named "overrides" (either a third party
         # lib -- there is one -- or just other escaped modules). We therefore load
         # a fuller path to distinguish them from one another.
+        # We insert in sys.path a prefix that doesn't go up past metaflow/metaflow_extensions
+        # because overrides may import other modules and we want to make sure we
+        # don't "leak" things from the outside environment.
         pkg_components = []
         prefix, last_basename = os.path.split(config_dir)
-        while last_basename not in ("metaflow", "metaflow_extensions"):
+        while True:
             pkg_components.append(last_basename)
-            prefix, last_basename = os.path.split(prefix)
-        pkg_components.append(last_basename)
+            possible_prefix, last_basename = os.path.split(prefix)
+            if last_basename in ("metaflow", "metaflow_extensions"):
+                break
+            prefix = possible_prefix
 
         try:
             sys.path.insert(0, prefix)
             override_module = importlib.import_module(
                 ".overrides", package=".".join(reversed(pkg_components))
             )
             override_values = override_module.__dict__.values()
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/client_modules.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/client_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,15 @@
             # The max_pickle_version is the pickle version that the server (so
             # the underlying interpreter we call into) supports; we determine
             # what version the current environment support and take the minimum
             # of those two
             max_pickle_version = min(self._max_pickle_version, pickle.HIGHEST_PROTOCOL)
 
             self._client = Client(
+                self._module_prefixes,
                 self._python_executable,
                 self._pythonpath,
                 max_pickle_version,
                 self._config_dir,
             )
             atexit.register(_clean_client, self._client)
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/bytestream.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/communication/bytestream.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/channel.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/communication/channel.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/socket_bytestream.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/communication/socket_bytestream.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/utils.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/communication/utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/consts.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/consts.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/data_transferer.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/data_transferer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/exception_transferer.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/exception_transferer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import sys
 import traceback
 
 try:
     # Import from client
     from .data_transferer import DataTransferer
+    from .stub import Stub
 except ImportError:
     # Import from server
     from data_transferer import DataTransferer
+    from stub import Stub
 
 
 # This file is heavily inspired from the RPYC project
 # The license for this project is reproduced here
 # (from https://rpyc.readthedocs.io/en/latest/license.html):
 # Copyright (c) 2005-2013
 #   Tomer Filiba (tomerfiliba@gmail.com)
@@ -110,16 +112,19 @@
             # Use __import__ so that the user can access this exception
             __import__(exception_module, None, None, "*")
         except Exception:
             pass
     # Try again (will succeed if the __import__ worked)
     if exception_module in sys.modules:
         exception_class = getattr(sys.modules[exception_module], exception_name, None)
-    if exception_class is None:
-        # Best effort to "recreate" an exception
+    if exception_class is None or issubclass(exception_class, Stub):
+        # Best effort to "recreate" an exception. Note that in some cases, exceptions
+        # may actually be both exceptions we can transfer as well as classes we
+        # can transfer (stubs) but for exceptions, we don't want to use the stub
+        # otherwise it will just ping pong.
         name = "%s.%s" % (exception_module, exception_name)
         exception_class = _remote_exceptions_class.setdefault(
             name,
             type(
                 name,
                 (RemoteInterpreterException,),
                 {"__module__": "%s/%s" % (__name__, exception_module)},
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/override_decorators.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/override_decorators.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/server.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/server.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/stub.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/stub.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/utils.py` & `ob-metaflow-2.9.4/metaflow/plugins/env_escape/utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/environment_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/environment_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/events_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/events_decorator.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,20 +22,29 @@
     ```
     @trigger(events=['foo', 'bar'])
     ```
 
     Additionally, you can specify the parameter mappings
     to map event payload to Metaflow parameters for the flow.
     ```
-    @trigger(event={'name':'foo', 'parameters':{'my_param': 'event_field'})
+    @trigger(event={'name':'foo', 'parameters':{'flow_param': 'event_field'}})
     ```
     or
     ```
-    @trigger(events=[{'name':'foo', 'parameters':{'my_param_1': 'event_field_1'},
-                     {'name':'bar', 'parameters':{'my_param_2': 'event_field_2'}])
+    @trigger(events=[{'name':'foo', 'parameters':{'flow_param_1': 'event_field_1'},
+                     {'name':'bar', 'parameters':{'flow_param_2': 'event_field_2'}])
+    ```
+
+    'parameters' can also be a list of strings and tuples like so:
+    ```
+    @trigger(event={'name':'foo', 'parameters':['common_name', ('flow_param', 'event_field')]})
+    ```
+    This is equivalent to:
+    ```
+    @trigger(event={'name':'foo', 'parameters':{'common_name': 'common_name', 'flow_param': 'event_field'}})
     ```
 
     Parameters
     ----------
     event : Union[str, dict], optional
         Event dependency for this flow.
     events : List[Union[str, dict]], optional
@@ -72,19 +81,34 @@
             # event attribute supports the following formats -
             #     1. event='table.prod_db.members'
             #     2. event={'name': 'table.prod_db.members',
             #               'parameters': {'alpha': 'member_weight'}}
             if is_stringish(self.attributes["event"]):
                 self.triggers.append({"name": str(self.attributes["event"])})
             elif isinstance(self.attributes["event"], dict):
-                if "name" not in dict(self.attributes["event"]):
+                if "name" not in self.attributes["event"]:
                     raise MetaflowException(
                         "The *event* attribute for *@trigger* is missing the "
                         "*name* key."
                     )
+                param_value = self.attributes["event"].get("parameters", {})
+                if isinstance(param_value, (list, tuple)):
+                    new_param_value = {}
+                    for mapping in param_value:
+                        if is_stringish(mapping):
+                            new_param_value[mapping] = mapping
+                        elif isinstance(mapping, (list, tuple)) and len(mapping) == 2:
+                            new_param_value[mapping[0]] = mapping[1]
+                        else:
+                            raise MetaflowException(
+                                "The *parameters* attribute for event '%s' is invalid. "
+                                "It should be a list/tuple of strings and lists/tuples "
+                                "of size 2" % self.attributes["event"]["name"]
+                            )
+                    self.attributes["event"]["parameters"] = new_param_value
                 self.triggers.append(self.attributes["event"])
             else:
                 raise MetaflowException(
                     "Incorrect format for *event* attribute in *@trigger* decorator. "
                     "Supported formats are string and dictionary - \n"
                     "@trigger(event='foo') or @trigger(event={'name': 'foo', "
                     "'parameters': {'alpha': 'beta'}})"
@@ -96,19 +120,37 @@
             #                {'name': 'table.prod_db.metadata',
             #               'parameters': {'beta': 'grade'}}]
             if isinstance(self.attributes["events"], list):
                 for event in self.attributes["events"]:
                     if is_stringish(event):
                         self.triggers.append({"name": str(event)})
                     elif isinstance(event, dict):
-                        if "name" not in dict(event):
+                        if "name" not in event:
                             raise MetaflowException(
                                 "One or more events in *events* attribute for "
                                 "*@trigger* are missing the *name* key."
                             )
+                        param_value = event.get("parameters", {})
+                        if isinstance(param_value, (list, tuple)):
+                            new_param_value = {}
+                            for mapping in param_value:
+                                if is_stringish(mapping):
+                                    new_param_value[mapping] = mapping
+                                elif (
+                                    isinstance(mapping, (list, tuple))
+                                    and len(mapping) == 2
+                                ):
+                                    new_param_value[mapping[0]] = mapping[1]
+                                else:
+                                    raise MetaflowException(
+                                        "The *parameters* attribute for event '%s' is "
+                                        "invalid. It should be a list/tuple of strings "
+                                        "and lists/tuples of size 2" % event["name"]
+                                    )
+                            event["parameters"] = new_param_value
                         self.triggers.append(event)
                     else:
                         raise MetaflowException(
                             "One or more events in *events* attribute in *@trigger* "
                             "decorator have an incorrect format. Supported format "
                             "is dictionary - \n"
                             "@trigger(events=[{'name': 'foo', 'parameters': {'alpha': "
@@ -159,19 +201,31 @@
     @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
     ```
     or
     ```
     @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
     ```
 
+    You can also specify just the project or project branch (other values will be
+    inferred from the current project or project branch):
+    ```
+    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
+    ```
+
+    Note that `branch` is typically one of:
+      - `prod`
+      - `user.bob`
+      - `test.my_experiment`
+      - `prod.staging`
+
     Parameters
     ----------
-    flow : str, optional
+    flow : Union[str, Dict[str, str]], optional
         Upstream flow dependency for this flow.
-    flows : List[str], optional
+    flows : List[Union[str, Dict[str, str]], optional
         Upstream flow dependencies for this flow.
     options : dict, optional
         Backend-specific configuration for tuning eventing behavior.
     """
 
     name = "trigger_on_finish"
     defaults = {
@@ -208,36 +262,97 @@
             # flow supports the format @trigger_on_finish(flow='FooFlow')
             if is_stringish(self.attributes["flow"]):
                 self.triggers.append(
                     {
                         "fq_name": self.attributes["flow"],
                     }
                 )
+            elif isinstance(self.attributes["flow"], dict):
+                if "name" not in self.attributes["flow"]:
+                    raise MetaflowException(
+                        "The *flow* attribute for *@trigger_on_finish* is missing the "
+                        "*name* key."
+                    )
+                flow_name = self.attributes["flow"]["name"]
+
+                if not is_stringish(flow_name) or "." in flow_name:
+                    raise MetaflowException(
+                        "The *name* attribute of the *flow* is not a valid string"
+                    )
+                result = {"fq_name": flow_name}
+                if "project" in self.attributes["flow"]:
+                    if is_stringish(self.attributes["flow"]["project"]):
+                        result["project"] = self.attributes["flow"]["project"]
+                    else:
+                        raise MetaflowException(
+                            "The *project* attribute of the *flow* is not a string"
+                        )
+                if "project_branch" in self.attributes["flow"]:
+                    if is_stringish(self.attributes["flow"]["project_branch"]):
+                        result["branch"] = self.attributes["flow"]["project_branch"]
+                    else:
+                        raise MetaflowException(
+                            "The *project_branch* attribute of the *flow* is not a string"
+                        )
+                self.triggers.append(result)
             else:
                 raise MetaflowException(
                     "Incorrect type for *flow* attribute in *@trigger_on_finish* "
-                    " decorator. Supported type is string - \n"
-                    "@trigger_on_finish(flow='FooFlow')"
+                    " decorator. Supported type is string or Dict[str, str] - \n"
+                    "@trigger_on_finish(flow='FooFlow') or "
+                    "@trigger_on_finish(flow={'name':'FooFlow', 'project_branch': 'branch'})"
                 )
         elif self.attributes["flows"]:
             # flows attribute supports the following formats -
             #     1. flows=['FooFlow', 'BarFlow']
             if isinstance(self.attributes["flows"], list):
                 for flow in self.attributes["flows"]:
                     if is_stringish(flow):
                         self.triggers.append(
                             {
                                 "fq_name": flow,
                             }
                         )
+                    elif isinstance(flow, dict):
+                        if "name" not in flow:
+                            raise MetaflowException(
+                                "One or more flows in the *flows* attribute for "
+                                "*@trigger_on_finish* is missing the "
+                                "*name* key."
+                            )
+                        flow_name = flow["name"]
+
+                        if not is_stringish(flow_name) or "." in flow_name:
+                            raise MetaflowException(
+                                "The *name* attribute '%s' is not a valid string"
+                                % str(flow_name)
+                            )
+                        result = {"fq_name": flow_name}
+                        if "project" in flow:
+                            if is_stringish(flow["project"]):
+                                result["project"] = flow["project"]
+                            else:
+                                raise MetaflowException(
+                                    "The *project* attribute of the *flow* '%s' is not "
+                                    "a string" % flow_name
+                                )
+                        if "project_branch" in flow:
+                            if is_stringish(flow["project_branch"]):
+                                result["branch"] = flow["project_branch"]
+                            else:
+                                raise MetaflowException(
+                                    "The *project_branch* attribute of the *flow* %s "
+                                    "is not a string" % flow_name
+                                )
+                        self.triggers.append(result)
                     else:
                         raise MetaflowException(
                             "One or more flows in *flows* attribute in "
                             "*@trigger_on_finish* decorator have an incorrect type. "
-                            "Supported type is string - \n"
+                            "Supported type is string or Dict[str, str]- \n"
                             "@trigger_on_finish(flows=['FooFlow', 'BarFlow']"
                         )
             else:
                 raise MetaflowException(
                     "Incorrect type for *flows* attribute in *@trigger_on_finish* "
                     "decorator. Supported type is list - \n"
                     "@trigger_on_finish(flows=['FooFlow', 'BarFlow']"
@@ -249,15 +364,15 @@
             )
 
         # Make triggers @project aware
         for trigger in self.triggers:
             if trigger["fq_name"].count(".") == 0:
                 # fully qualified name is just the flow name
                 trigger["flow"] = trigger["fq_name"]
-            elif trigger["fq_name"].count(".") in (2, 3):
+            elif trigger["fq_name"].count(".") >= 2:
                 # fully qualified name is of the format - project.branch.flow_name
                 trigger["project"], tail = trigger["fq_name"].split(".", maxsplit=1)
                 trigger["branch"], trigger["flow"] = tail.rsplit(".", maxsplit=1)
             else:
                 raise MetaflowException(
                     "Incorrect format for *flow* in *@trigger_on_finish* "
                     "decorator. Specify either just the *flow_name* or a fully "
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/frameworks/pytorch.py` & `ob-metaflow-2.9.4/metaflow/plugins/frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_storage_client_factory.py` & `ob-metaflow-2.9.4/metaflow/plugins/gcp/gs_storage_client_factory.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_tail.py` & `ob-metaflow-2.9.4/metaflow/plugins/gcp/gs_tail.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_utils.py` & `ob-metaflow-2.9.4/metaflow/plugins/gcp/gs_utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/gcp/includefile_support.py` & `ob-metaflow-2.9.4/metaflow/plugins/gcp/includefile_support.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes.py` & `ob-metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import json
 import math
 import os
+import re
 import shlex
 import time
+from typing import Dict, List, Optional
 
 from metaflow import current, util
 from metaflow.exception import MetaflowException
 from metaflow.metaflow_config import (
     ARGO_EVENTS_EVENT,
     ARGO_EVENTS_EVENT_BUS,
     ARGO_EVENTS_EVENT_SOURCE,
     ARGO_EVENTS_SERVICE_ACCOUNT,
-    ARGO_EVENTS_WEBHOOK_URL,
+    ARGO_EVENTS_INTERNAL_WEBHOOK_URL,
     AWS_SECRETS_MANAGER_DEFAULT_REGION,
     AZURE_STORAGE_BLOB_SERVICE_ENDPOINT,
     CARD_AZUREROOT,
     CARD_GSROOT,
     CARD_S3ROOT,
     DATASTORE_SYSROOT_AZURE,
     DATASTORE_SYSROOT_GS,
     DATASTORE_SYSROOT_S3,
     DATATOOLS_S3ROOT,
     DEFAULT_AWS_CLIENT_PROVIDER,
     DEFAULT_METADATA,
     DEFAULT_SECRETS_BACKEND_TYPE,
     KUBERNETES_FETCH_EC2_METADATA,
+    KUBERNETES_LABELS,
     KUBERNETES_SANDBOX_INIT_SCRIPT,
     S3_ENDPOINT_URL,
     SERVICE_HEADERS,
     SERVICE_INTERNAL_URL,
     OTEL_ENDPOINT,
 )
 from metaflow.mflog import (
@@ -142,14 +145,15 @@
         attempt,
         user,
         code_package_sha,
         code_package_url,
         code_package_ds,
         step_cli,
         docker_image,
+        docker_image_pull_policy,
         service_account=None,
         secrets=None,
         node_selector=None,
         namespace=None,
         cpu=None,
         gpu=None,
         gpu_vendor=None,
@@ -159,14 +163,15 @@
         tmpfs_tempdir=None,
         tmpfs_size=None,
         tmpfs_path=None,
         run_time_limit=None,
         env=None,
         persistent_volume_claims=None,
         tolerations=None,
+        labels=None,
     ):
         if env is None:
             env = {}
 
         job = (
             KubernetesClient()
             .job(
@@ -181,24 +186,26 @@
                     step_name=step_name,
                     task_id=task_id,
                     attempt=attempt,
                     code_package_url=code_package_url,
                     step_cmds=[step_cli],
                 ),
                 image=docker_image,
+                image_pull_policy=docker_image_pull_policy,
                 cpu=cpu,
                 memory=memory,
                 disk=disk,
                 gpu=gpu,
                 gpu_vendor=gpu_vendor,
                 timeout_in_seconds=run_time_limit,
                 # Retries are handled by Metaflow runtime
                 retries=0,
                 step_name=step_name,
                 tolerations=tolerations,
+                labels=self._get_labels(labels),
                 use_tmpfs=use_tmpfs,
                 tmpfs_tempdir=tmpfs_tempdir,
                 tmpfs_size=tmpfs_size,
                 tmpfs_path=tmpfs_path,
                 persistent_volume_claims=persistent_volume_claims,
             )
             .environment_variable("METAFLOW_CODE_SHA", code_package_sha)
@@ -254,15 +261,15 @@
             # assumes metadata is stored in DATASTORE_LOCAL_DIR on the Kubernetes
             # pod; this happens when METAFLOW_DATASTORE_SYSROOT_LOCAL is NOT set (
             # see get_datastore_root_from_config in datastore/local.py).
         )
 
         # Set environment variables to support metaflow.integrations.ArgoEvent
         job.environment_variable(
-            "METAFLOW_ARGO_EVENTS_WEBHOOK_URL", ARGO_EVENTS_WEBHOOK_URL
+            "METAFLOW_ARGO_EVENTS_WEBHOOK_URL", ARGO_EVENTS_INTERNAL_WEBHOOK_URL
         )
         job.environment_variable("METAFLOW_ARGO_EVENTS_EVENT", ARGO_EVENTS_EVENT)
         job.environment_variable(
             "METAFLOW_ARGO_EVENTS_EVENT_BUS", ARGO_EVENTS_EVENT_BUS
         )
         job.environment_variable(
             "METAFLOW_ARGO_EVENTS_EVENT_SOURCE", ARGO_EVENTS_EVENT_SOURCE
@@ -393,7 +400,64 @@
 
         exit_code, _ = self._job.reason
         echo(
             "Task finished with exit code %s." % exit_code,
             "stderr",
             job_id=self._job.id,
         )
+
+    @staticmethod
+    def _get_labels(extra_labels=None):
+        if extra_labels is None:
+            extra_labels = {}
+        env_labels = KUBERNETES_LABELS.split(",") if KUBERNETES_LABELS else []
+        env_labels = parse_kube_keyvalue_list(env_labels, False)
+        labels = {**env_labels, **extra_labels}
+        validate_kube_labels(labels)
+        return labels
+
+
+def validate_kube_labels(
+    labels: Optional[Dict[str, Optional[str]]],
+) -> bool:
+    """Validate label values.
+
+    This validates the kubernetes label values.  It does not validate the keys.
+    Ideally, keys should be static and also the validation rules for keys are
+    more complex than those for values.  For full validation rules, see:
+
+    https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#syntax-and-character-set
+    """
+
+    def validate_label(s: Optional[str]):
+        regex_match = r"^(([A-Za-z0-9][-A-Za-z0-9_.]{0,61})?[A-Za-z0-9])?$"
+        if not s:
+            # allow empty label
+            return True
+        if not re.search(regex_match, s):
+            raise KubernetesException(
+                'Invalid value: "%s"\n'
+                "A valid label must be an empty string or one that\n"
+                "  - Consist of alphanumeric, '-', '_' or '.' characters\n"
+                "  - Begins and ends with an alphanumeric character\n"
+                "  - Is at most 63 characters" % s
+            )
+        return True
+
+    return all([validate_label(v) for v in labels.values()]) if labels else True
+
+
+def parse_kube_keyvalue_list(items: List[str], requires_both: bool = True):
+    try:
+        ret = {}
+        for item_str in items:
+            item = item_str.split("=", 1)
+            if requires_both:
+                item[1]  # raise IndexError
+            if str(item[0]) in ret:
+                raise KubernetesException("Duplicate key found: %s" % str(item[0]))
+            ret[str(item[0])] = str(item[1]) if len(item) > 1 else None
+        return ret
+    except KubernetesException as e:
+        raise e
+    except (AttributeError, IndexError):
+        raise KubernetesException("Unable to parse kubernetes list: %s" % items)
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_cli.py` & `ob-metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import sys
 import time
 import traceback
 
-from metaflow import util, JSONTypeClass
+from metaflow import JSONTypeClass, util
 from metaflow._vendor import click
 from metaflow.exception import METAFLOW_EXIT_DISALLOW_RETRY, CommandException
 from metaflow.metadata.util import sync_local_metadata_from_datastore
-from metaflow.metaflow_config import DATASTORE_LOCAL_DIR
+from metaflow.metaflow_config import DATASTORE_LOCAL_DIR, KUBERNETES_LABELS
 from metaflow.mflog import TASK_LOG_SOURCE
 import metaflow.tracing as tracing
 
-from .kubernetes import Kubernetes, KubernetesKilledException
+from .kubernetes import Kubernetes, KubernetesKilledException, parse_kube_keyvalue_list
 from .kubernetes_decorator import KubernetesDecorator
 
 
 @click.group()
 def cli():
     pass
 
@@ -36,14 +36,19 @@
 @click.argument("code-package-url")
 @click.option(
     "--executable",
     help="Executable requirement for Kubernetes pod.",
 )
 @click.option("--image", help="Docker image requirement for Kubernetes pod.")
 @click.option(
+    "--image-pull-policy",
+    default=None,
+    help="Optional Docker Image Pull Policy for Kubernetes pod.",
+)
+@click.option(
     "--service-account",
     help="IRSA requirement for Kubernetes pod.",
 )
 @click.option(
     "--secrets",
     multiple=True,
     default=None,
@@ -106,14 +111,15 @@
 def step(
     ctx,
     step_name,
     code_package_sha,
     code_package_url,
     executable=None,
     image=None,
+    image_pull_policy=None,
     service_account=None,
     secrets=None,
     node_selector=None,
     k8s_namespace=None,
     cpu=None,
     disk=None,
     memory=None,
@@ -187,15 +193,15 @@
         task_id=kwargs["task_id"],
         attempt=int(retry_count),
     )
     stdout_location = ds.get_log_location(TASK_LOG_SOURCE, "stdout")
     stderr_location = ds.get_log_location(TASK_LOG_SOURCE, "stderr")
 
     # `node_selector` is a tuple of strings, convert it to a dictionary
-    node_selector = KubernetesDecorator.parse_node_selector(node_selector)
+    node_selector = parse_kube_keyvalue_list(node_selector)
 
     def _sync_metadata():
         if ctx.obj.metadata.TYPE == "local":
             sync_local_metadata_from_datastore(
                 DATASTORE_LOCAL_DIR,
                 ctx.obj.flow_datastore.get_task_datastore(
                     kwargs["run_id"], step_name, kwargs["task_id"]
@@ -218,14 +224,15 @@
                 attempt=str(retry_count),
                 user=util.get_username(),
                 code_package_sha=code_package_sha,
                 code_package_url=code_package_url,
                 code_package_ds=ctx.obj.flow_datastore.TYPE,
                 step_cli=step_cli,
                 docker_image=image,
+                docker_image_pull_policy=image_pull_policy,
                 service_account=service_account,
                 secrets=secrets,
                 node_selector=node_selector,
                 namespace=k8s_namespace,
                 cpu=cpu,
                 disk=disk,
                 memory=memory,
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_client.py` & `ob-metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_decorator.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,29 @@
 from metaflow.exception import MetaflowException
 from metaflow.metadata import MetaDatum
 from metaflow.metadata.util import sync_local_metadata_to_datastore
 from metaflow.metaflow_config import (
     DATASTORE_LOCAL_DIR,
     KUBERNETES_CONTAINER_IMAGE,
     KUBERNETES_CONTAINER_REGISTRY,
+    KUBERNETES_FETCH_EC2_METADATA,
+    KUBERNETES_IMAGE_PULL_POLICY,
     KUBERNETES_GPU_VENDOR,
     KUBERNETES_NAMESPACE,
     KUBERNETES_NODE_SELECTOR,
+    KUBERNETES_PERSISTENT_VOLUME_CLAIMS,
     KUBERNETES_TOLERATIONS,
     KUBERNETES_SERVICE_ACCOUNT,
-    KUBERNETES_SECRETS,
-    KUBERNETES_FETCH_EC2_METADATA,
-    KUBERNETES_PERSISTENT_VOLUME_CLAIMS,
 )
 from metaflow.plugins.resources_decorator import ResourcesDecorator
 from metaflow.plugins.timeout_decorator import get_run_time_limit_for_task
 from metaflow.sidecar import Sidecar
 
 from ..aws.aws_utils import get_docker_registry, get_ec2_instance_metadata
-
-from .kubernetes import KubernetesException
+from .kubernetes import KubernetesException, parse_kube_keyvalue_list
 
 from metaflow.metaflow_config import MAX_MEMORY_PER_TASK, MAX_CPU_PER_TASK
 
 try:
     unicode
 except NameError:
     unicode = str
@@ -75,22 +74,26 @@
         sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
     tmpfs_size: int, optional
         The value for the size (in MiB) of the tmpfs mount for this step.
         This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
         memory allocated for this step.
     tmpfs_path: string, optional
         Path to tmpfs mount for this step. Defaults to /metaflow_temp.
+    persistent_volume_claims: Dict[str, str], optional
+        A map (dictionary) of persistent volumes to be mounted to the pod for this step. The map is from persistent
+        volumes to the path to which the volume is to be mounted, e.g., `{'pvc-name': '/path/to/mount/on'}`.
     """
 
     name = "kubernetes"
     defaults = {
         "cpu": "2",
         "memory": "8192",
         "disk": "10240",
         "image": None,
+        "image_pull_policy": None,
         "service_account": None,
         "secrets": None,  # e.g., mysecret
         "node_selector": None,  # e.g., kubernetes.io/os=linux
         "namespace": None,
         "gpu": None,  # value of 0 implies that the scheduled node should not have GPUs
         "gpu_vendor": None,
         "tolerations": None,  # e.g., [{"key": "arch", "operator": "Equal", "value": "amd"},
@@ -121,17 +124,19 @@
         if (
             not self.attributes["persistent_volume_claims"]
             and KUBERNETES_PERSISTENT_VOLUME_CLAIMS
         ):
             self.attributes["persistent_volume_claims"] = json.loads(
                 KUBERNETES_PERSISTENT_VOLUME_CLAIMS
             )
+        if not self.attributes["image_pull_policy"] and KUBERNETES_IMAGE_PULL_POLICY:
+            self.attributes["image_pull_policy"] = KUBERNETES_IMAGE_PULL_POLICY
 
         if isinstance(self.attributes["node_selector"], str):
-            self.attributes["node_selector"] = self.parse_node_selector(
+            self.attributes["node_selector"] = parse_kube_keyvalue_list(
                 self.attributes["node_selector"].split(",")
             )
 
         if self.attributes["tolerations"]:
             try:
                 from kubernetes.client import V1Toleration
 
@@ -333,18 +338,19 @@
             cli_args.command_args.append(self.package_url)
 
             # --namespace is used to specify Metaflow namespace (a different
             # concept from k8s namespace).
             for k, v in self.attributes.items():
                 if k == "namespace":
                     cli_args.command_options["k8s_namespace"] = v
-                elif k == "node_selector" and v:
-                    cli_args.command_options[k] = ",".join(
-                        ["=".join([key, str(val)]) for key, val in v.items()]
-                    )
+                elif k in {"node_selector"} and v:
+                    cli_args.command_options[k] = [
+                        "=".join([key, str(val)]) if val else key
+                        for key, val in v.items()
+                    ]
                 elif k in ["tolerations", "persistent_volume_claims"]:
                     cli_args.command_options[k] = json.dumps(v)
                 else:
                     cli_args.command_options[k] = v
             cli_args.command_options["run-time-limit"] = self.run_time_limit
             cli_args.entrypoint[0] = sys.executable
 
@@ -448,19 +454,7 @@
 
     @classmethod
     def _save_package_once(cls, flow_datastore, package):
         if cls.package_url is None:
             cls.package_url, cls.package_sha = flow_datastore.save_data(
                 [package.blob], len_hint=1
             )[0]
-
-    @staticmethod
-    def parse_node_selector(node_selector: list):
-        try:
-            return {
-                str(k.split("=", 1)[0]): str(k.split("=", 1)[1])
-                for k in node_selector or []
-            }
-        except (AttributeError, IndexError):
-            raise KubernetesException(
-                "Unable to parse node_selector: %s" % node_selector
-            )
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_job.py` & `ob-metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
                                         )
                                     )
                                     for k in list(self._kwargs.get("secrets", []))
                                     + KUBERNETES_SECRETS.split(",")
                                     if k
                                 ],
                                 image=self._kwargs["image"],
+                                image_pull_policy=self._kwargs["image_pull_policy"],
                                 name=self._kwargs["step_name"].replace("_", "-"),
                                 resources=client.V1ResourceRequirements(
                                     requests={
                                         "cpu": str(self._kwargs["cpu"]),
                                         "memory": "%sM" % str(self._kwargs["memory"]),
                                         "ephemeral-storage": "%sM"
                                         % str(self._kwargs["disk"]),
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/metadata/local.py` & `ob-metaflow-2.9.4/metaflow/plugins/metadata/local.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/metadata/service.py` & `ob-metaflow-2.9.4/metaflow/plugins/metadata/service.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/package_cli.py` & `ob-metaflow-2.9.4/metaflow/plugins/package_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/parallel_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/parallel_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/project_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/project_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/resources_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/resources_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/retry_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/secrets/secrets_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/secrets/secrets_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import re
 
 from metaflow.exception import MetaflowException
 from metaflow.decorators import StepDecorator
+from metaflow.metaflow_config import DEFAULT_SECRETS_ROLE
 from metaflow.unbounded_foreach import UBF_CONTROL
 
 from typing import Any, Dict, List, Union
 
 DISALLOWED_SECRETS_ENV_VAR_PREFIXES = ["METAFLOW_"]
 
 
@@ -18,44 +19,50 @@
             "No default secrets backend type configured, but needed by @secrets. "
             "Set METAFLOW_DEFAULT_SECRETS_BACKEND_TYPE."
         )
     return DEFAULT_SECRETS_BACKEND_TYPE
 
 
 class SecretSpec:
-    def __init__(self, secrets_backend_type, secret_id, options={}):
+    def __init__(self, secrets_backend_type, secret_id, options={}, role=None):
         self._secrets_backend_type = secrets_backend_type
         self._secret_id = secret_id
         self._options = options
+        self._role = role
 
     @property
     def secrets_backend_type(self):
         return self._secrets_backend_type
 
     @property
     def secret_id(self):
         return self._secret_id
 
     @property
     def options(self):
         return self._options
 
+    @property
+    def role(self):
+        return self._role
+
     def to_json(self):
         """Mainly used for testing... not the same as the input dict in secret_spec_from_dict()!"""
         return {
             "secrets_backend_type": self.secrets_backend_type,
             "secret_id": self.secret_id,
             "options": self.options,
+            "role": self.role,
         }
 
     def __str__(self):
         return "%s (%s)" % (self._secret_id, self._secrets_backend_type)
 
     @staticmethod
-    def secret_spec_from_str(secret_spec_str):
+    def secret_spec_from_str(secret_spec_str, role):
         # "." may be used in secret_id one day (provider specific). HOWEVER, it provides the best UX for
         # non-conflicting cases (i.e. for secret ids that don't contain "."). This is true for all AWS
         # Secrets Manager secrets.
         #
         # So we skew heavily optimize for best upfront UX for the present (1/2023).
         #
         # If/when a certain secret backend supports "." secret names, we can figure out a solution at that time.
@@ -70,18 +77,20 @@
         parts = secret_spec_str.split(".", maxsplit=1)
         if len(parts) == 1:
             secrets_backend_type = get_default_secrets_backend_type()
             secret_id = parts[0]
         else:
             secrets_backend_type = parts[0]
             secret_id = parts[1]
-        return SecretSpec(secrets_backend_type, secret_id=secret_id)
+        return SecretSpec(
+            secrets_backend_type, secret_id=secret_id, options={}, role=role
+        )
 
     @staticmethod
-    def secret_spec_from_dict(secret_spec_dict):
+    def secret_spec_from_dict(secret_spec_dict, role):
         if "type" not in secret_spec_dict:
             secrets_backend_type = get_default_secrets_backend_type()
         else:
             secrets_backend_type = secret_spec_dict["type"]
             if not isinstance(secrets_backend_type, str):
                 raise MetaflowException(
                     "Bad @secrets specification - 'type' must be a string - found %s"
@@ -95,15 +104,25 @@
             )
         options = secret_spec_dict.get("options", {})
         if not isinstance(options, dict):
             raise MetaflowException(
                 "Bad @secrets specification - 'option' must be a dict - found %s"
                 % type(options)
             )
-        return SecretSpec(secrets_backend_type, secret_id=secret_id, options=options)
+        role_for_source = secret_spec_dict.get("role", None)
+        if role_for_source is not None:
+            if not isinstance(role_for_source, str):
+                raise MetaflowException(
+                    "Bad @secrets specification - 'role' must be a str - found %s"
+                    % type(role_for_source)
+                )
+            role = role_for_source
+        return SecretSpec(
+            secrets_backend_type, secret_id=secret_id, options=options, role=role
+        )
 
 
 def validate_env_vars_across_secrets(all_secrets_env_vars):
     vars_injected_by = {}
     for secret_spec, env_vars in all_secrets_env_vars:
         for k in env_vars:
             if k in vars_injected_by:
@@ -168,15 +187,18 @@
     Parameters
     ----------
     sources : List[Union[str, Dict[str, Any]]], default: []
         List of secret specs, defining how the secrets are to be retrieved
     """
 
     name = "secrets"
-    defaults = {"sources": []}
+    defaults = {
+        "sources": [],
+        "role": None,
+    }
 
     def task_pre_step(
         self,
         step_name,
         task_datastore,
         metadata,
         run_id,
@@ -191,35 +213,49 @@
         if ubf_context == UBF_CONTROL:
             """control tasks (as used in "unbounded for each") don't need secrets"""
             return
         # List of pairs (secret_spec, env_vars_from_this_spec)
         all_secrets_env_vars = []
         secret_specs = []
 
+        # Role (in terms of RBAC) to use when retrieving secrets.
+        # This is a general concept applicable to multiple backends
+        # E.g in AWS, this would be an IAM Role ARN.
+        #
+        # Config precedence (decreasing):
+        # - Source level: @secrets(source=[{"role": ...}])
+        # - Decorator level: @secrets(role=...)
+        # - Metaflow config key DEFAULT_SECRETS_ROLE
+        role = self.attributes["role"]
+        if role is None:
+            role = DEFAULT_SECRETS_ROLE
+
         for secret_spec_str_or_dict in self.attributes["sources"]:
             if isinstance(secret_spec_str_or_dict, str):
                 secret_specs.append(
-                    SecretSpec.secret_spec_from_str(secret_spec_str_or_dict)
+                    SecretSpec.secret_spec_from_str(secret_spec_str_or_dict, role=role)
                 )
             elif isinstance(secret_spec_str_or_dict, dict):
                 secret_specs.append(
-                    SecretSpec.secret_spec_from_dict(secret_spec_str_or_dict)
+                    SecretSpec.secret_spec_from_dict(secret_spec_str_or_dict, role=role)
                 )
             else:
                 raise MetaflowException(
                     "@secrets sources items must be either a string or a dict"
                 )
 
         for secret_spec in secret_specs:
             secrets_backend_provider = get_secrets_backend_provider(
                 secret_spec.secrets_backend_type
             )
             try:
                 env_vars_for_secret = secrets_backend_provider.get_secret_as_dict(
-                    secret_spec.secret_id, options=secret_spec.options
+                    secret_spec.secret_id,
+                    options=secret_spec.options,
+                    role=secret_spec.role,
                 )
             except Exception as e:
                 raise MetaflowException(
                     "Failed to retrieve secret '%s': %s" % (secret_spec.secret_id, e)
                 )
             try:
                 validate_env_vars(env_vars_for_secret)
```

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/storage_executor.py` & `ob-metaflow-2.9.4/metaflow/plugins/storage_executor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/tag_cli.py` & `ob-metaflow-2.9.4/metaflow/plugins/tag_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/test_unbounded_foreach_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/test_unbounded_foreach_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/plugins/timeout_decorator.py` & `ob-metaflow-2.9.4/metaflow/plugins/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/procpoll.py` & `ob-metaflow-2.9.4/metaflow/procpoll.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/pylint_wrapper.py` & `ob-metaflow-2.9.4/metaflow/pylint_wrapper.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/runtime.py` & `ob-metaflow-2.9.4/metaflow/runtime.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar.py` & `ob-metaflow-2.9.4/metaflow/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar_messages.py` & `ob-metaflow-2.9.4/metaflow/sidecar/sidecar_messages.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar_subprocess.py` & `ob-metaflow-2.9.4/metaflow/sidecar/sidecar_subprocess.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar_worker.py` & `ob-metaflow-2.9.4/metaflow/sidecar/sidecar_worker.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tagging_util.py` & `ob-metaflow-2.9.4/metaflow/tagging_util.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/task.py` & `ob-metaflow-2.9.4/metaflow/task.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tracing.py` & `ob-metaflow-2.9.4/metaflow/tracing.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tracing_noop.py` & `ob-metaflow-2.9.4/metaflow/tracing_noop.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tracing_otel.py` & `ob-metaflow-2.9.4/metaflow/tracing_otel.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tracing_propagator.py` & `ob-metaflow-2.9.4/metaflow/tracing_propagator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/00-helloworld/helloworld.py` & `ob-metaflow-2.9.4/metaflow/tutorials/00-helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/README.md` & `ob-metaflow-2.9.4/metaflow/tutorials/01-playlist/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/movies.csv` & `ob-metaflow-2.9.4/metaflow/tutorials/01-playlist/movies.csv`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/playlist.ipynb` & `ob-metaflow-2.9.4/metaflow/tutorials/01-playlist/playlist.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/playlist.py` & `ob-metaflow-2.9.4/metaflow/tutorials/01-playlist/playlist.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/README.md` & `ob-metaflow-2.9.4/metaflow/tutorials/02-statistics/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/movies.csv` & `ob-metaflow-2.9.4/metaflow/tutorials/02-statistics/movies.csv`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/stats.ipynb` & `ob-metaflow-2.9.4/metaflow/tutorials/02-statistics/stats.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/stats.py` & `ob-metaflow-2.9.4/metaflow/tutorials/02-statistics/stats.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/03-playlist-redux/README.md` & `ob-metaflow-2.9.4/metaflow/tutorials/03-playlist-redux/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/03-playlist-redux/playlist.py` & `ob-metaflow-2.9.4/metaflow/tutorials/03-playlist-redux/playlist.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/04-playlist-plus/README.md` & `ob-metaflow-2.9.4/metaflow/tutorials/04-playlist-plus/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/04-playlist-plus/playlist.py` & `ob-metaflow-2.9.4/metaflow/tutorials/04-playlist-plus/playlist.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/README.md` & `ob-metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb` & `ob-metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/hello-cloud.py` & `ob-metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/hello-cloud.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/06-statistics-redux/README.md` & `ob-metaflow-2.9.4/metaflow/tutorials/06-statistics-redux/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/06-statistics-redux/stats.ipynb` & `ob-metaflow-2.9.4/metaflow/tutorials/06-statistics-redux/stats.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/07-worldview/worldview.ipynb` & `ob-metaflow-2.9.4/metaflow/tutorials/07-worldview/worldview.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/08-autopilot/README.md` & `ob-metaflow-2.9.4/metaflow/tutorials/08-autopilot/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/tutorials/08-autopilot/autopilot.ipynb` & `ob-metaflow-2.9.4/metaflow/tutorials/08-autopilot/autopilot.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/util.py` & `ob-metaflow-2.9.4/metaflow/util.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/metaflow/vendor.py` & `ob-metaflow-2.9.4/metaflow/vendor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/ob_metaflow.egg-info/SOURCES.txt` & `ob-metaflow-2.9.4/ob_metaflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.9.1.3/setup.py` & `ob-metaflow-2.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "2.9.1.3"
+version = "2.9.4"
 
 setup(
     include_package_data=True,
     name="ob-metaflow",
     version=version,
     description="Metaflow: More Data Science, Less Engineering",
     long_description=open("README.md").read(),
```

