# Comparing `tmp/liquer-framework-0.9.0.tar.gz` & `tmp/liquer-framework-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/liquer-framework-0.9.0.tar", last modified: Sun Jun 11 17:47:25 2023, max compression
+gzip compressed data, was "dist/liquer-framework-0.9.1.tar", last modified: Mon Jun 12 20:44:37 2023, max compression
```

## Comparing `liquer-framework-0.9.0.tar` & `liquer-framework-0.9.1.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-11 17:47:25.458686 liquer-framework-0.9.0/
--rw-r--r--   0 orest     (1000) orest     (1000)       67 2023-05-18 20:29:33.000000 liquer-framework-0.9.0/MANIFEST.in
--rw-rw-r--   0 orest     (1000) orest     (1000)     7667 2023-06-11 17:47:25.458686 liquer-framework-0.9.0/PKG-INFO
--rw-rw-r--   0 orest     (1000) orest     (1000)     6456 2023-06-11 17:29:55.000000 liquer-framework-0.9.0/README.md
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-11 17:47:25.442685 liquer-framework-0.9.0/liquer/
--rw-r--r--   0 orest     (1000) orest     (1000)      185 2023-01-22 17:32:54.000000 liquer-framework-0.9.0/liquer/__init__.py
--rw-rw-r--   0 orest     (1000) orest     (1000)      259 2021-10-27 15:33:04.000000 liquer-framework-0.9.0/liquer/blueprint.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    30437 2023-04-22 13:59:35.000000 liquer-framework-0.9.0/liquer/cache.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    32155 2023-02-04 11:03:51.000000 liquer-framework-0.9.0/liquer/commands.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     3631 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/constants.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    41902 2023-05-18 22:09:05.000000 liquer-framework-0.9.0/liquer/context.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     3855 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/dependencies.py
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-11 17:47:25.450686 liquer-framework-0.9.0/liquer/ext/
--rw-r--r--   0 orest     (1000) orest     (1000)        0 2019-06-09 11:48:28.000000 liquer-framework-0.9.0/liquer/ext/__init__.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     9243 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/ext/basic.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    13175 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/ext/dataframe_batches.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     7937 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/ext/lq_datafusion.py
--rw-r--r--   0 orest     (1000) orest     (1000)     4381 2023-05-10 20:11:49.000000 liquer-framework-0.9.0/liquer/ext/lq_hxl.py
--rw-r--r--   0 orest     (1000) orest     (1000)     3933 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/ext/lq_keras.py
--rw-r--r--   0 orest     (1000) orest     (1000)     3686 2022-07-07 19:34:25.000000 liquer-framework-0.9.0/liquer/ext/lq_matplotlib.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     3447 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/ext/lq_openpyxl.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    16337 2023-05-10 20:10:02.000000 liquer-framework-0.9.0/liquer/ext/lq_pandas.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     3432 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/ext/lq_pil.py
--rw-r--r--   0 orest     (1000) orest     (1000)     2304 2021-10-27 15:33:04.000000 liquer-framework-0.9.0/liquer/ext/lq_plotly.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     2853 2023-01-21 20:13:08.000000 liquer-framework-0.9.0/liquer/ext/lq_polars.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     2244 2023-01-21 17:53:31.000000 liquer-framework-0.9.0/liquer/ext/lq_pptx.py
--rw-r--r--   0 orest     (1000) orest     (1000)      701 2021-10-27 15:33:04.000000 liquer-framework-0.9.0/liquer/ext/lq_pygments.py
--rw-r--r--   0 orest     (1000) orest     (1000)      368 2021-10-27 15:33:04.000000 liquer-framework-0.9.0/liquer/ext/lq_python.py
--rw-r--r--   0 orest     (1000) orest     (1000)     1805 2021-10-27 15:33:04.000000 liquer-framework-0.9.0/liquer/ext/lq_sklearn_regression.py
--rw-rw-r--   0 orest     (1000) orest     (1000)      712 2023-01-21 22:45:23.000000 liquer-framework-0.9.0/liquer/ext/lq_sweetviz.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     4300 2023-05-18 21:10:45.000000 liquer-framework-0.9.0/liquer/ext/lq_whoosh.py
--rw-r--r--   0 orest     (1000) orest     (1000)    16409 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/ext/meta.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     7326 2023-05-16 21:41:40.000000 liquer-framework-0.9.0/liquer/indexer.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     7020 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/metadata.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    34618 2023-05-10 20:15:46.000000 liquer-framework-0.9.0/liquer/parser.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     6273 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/pool.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     1199 2023-01-15 17:53:35.000000 liquer-framework-0.9.0/liquer/query.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    35940 2023-05-10 20:16:08.000000 liquer-framework-0.9.0/liquer/recipes.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     4122 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/remote_store.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     5713 2023-01-08 21:15:57.000000 liquer-framework-0.9.0/liquer/s3_store.py
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-11 17:47:25.454686 liquer-framework-0.9.0/liquer/server/
--rw-r--r--   0 orest     (1000) orest     (1000)        0 2019-06-09 11:48:28.000000 liquer-framework-0.9.0/liquer/server/__init__.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    14961 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/server/blueprint.py
--rw-r--r--   0 orest     (1000) orest     (1000)    19882 2023-05-18 22:06:45.000000 liquer-framework-0.9.0/liquer/server/handlers.py
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-11 17:47:25.454686 liquer-framework-0.9.0/liquer/server/static/
--rw-rw-r--   0 orest     (1000) orest     (1000)    26489 2021-01-31 21:05:09.000000 liquer-framework-0.9.0/liquer/server/static/index.html
--rw-rw-r--   0 orest     (1000) orest     (1000)    18057 2021-12-15 17:45:48.000000 liquer-framework-0.9.0/liquer/server/static/liquer.js
--rw-r--r--   0 orest     (1000) orest     (1000)     7371 2023-05-18 21:51:28.000000 liquer-framework-0.9.0/liquer/server/tornado_handlers.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     7656 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/state.py
--rw-r--r--   0 orest     (1000) orest     (1000)    17774 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/state_types.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    44447 2023-01-21 22:51:19.000000 liquer-framework-0.9.0/liquer/store.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    11266 2022-07-30 08:12:25.000000 liquer-framework-0.9.0/liquer/template.py
--rw-rw-r--   0 orest     (1000) orest     (1000)      621 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/tools.py
--rw-rw-r--   0 orest     (1000) orest     (1000)      521 2023-01-21 17:53:32.000000 liquer-framework-0.9.0/liquer/util.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     2721 2023-01-21 22:45:45.000000 liquer-framework-0.9.0/liquer/web.py
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-11 17:47:25.458686 liquer-framework-0.9.0/liquer_framework.egg-info/
--rw-r--r--   0 orest     (1000) orest     (1000)     7667 2023-06-11 17:47:24.000000 liquer-framework-0.9.0/liquer_framework.egg-info/PKG-INFO
--rw-r--r--   0 orest     (1000) orest     (1000)     1313 2023-06-11 17:47:24.000000 liquer-framework-0.9.0/liquer_framework.egg-info/SOURCES.txt
--rw-r--r--   0 orest     (1000) orest     (1000)        1 2023-06-11 17:47:24.000000 liquer-framework-0.9.0/liquer_framework.egg-info/dependency_links.txt
--rw-r--r--   0 orest     (1000) orest     (1000)        1 2019-12-07 17:16:04.000000 liquer-framework-0.9.0/liquer_framework.egg-info/not-zip-safe
--rw-r--r--   0 orest     (1000) orest     (1000)        6 2023-06-11 17:47:24.000000 liquer-framework-0.9.0/liquer_framework.egg-info/requires.txt
--rw-r--r--   0 orest     (1000) orest     (1000)        7 2023-06-11 17:47:24.000000 liquer-framework-0.9.0/liquer_framework.egg-info/top_level.txt
--rw-rw-r--   0 orest     (1000) orest     (1000)       38 2023-06-11 17:47:25.458686 liquer-framework-0.9.0/setup.cfg
--rw-r--r--   0 orest     (1000) orest     (1000)      702 2023-06-11 17:07:10.000000 liquer-framework-0.9.0/setup.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/
+-rw-r--r--   0 orest     (1000) orest     (1000)       77 2023-06-12 20:32:04.000000 liquer-framework-0.9.1/MANIFEST.in
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7755 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/PKG-INFO
+-rw-rw-r--   0 orest     (1000) orest     (1000)     6536 2023-06-12 20:43:18.000000 liquer-framework-0.9.1/README.md
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-12 20:44:37.041494 liquer-framework-0.9.1/liquer/
+-rw-r--r--   0 orest     (1000) orest     (1000)      185 2023-01-22 17:32:54.000000 liquer-framework-0.9.1/liquer/__init__.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)      259 2021-10-27 15:33:04.000000 liquer-framework-0.9.1/liquer/blueprint.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    30437 2023-04-22 13:59:35.000000 liquer-framework-0.9.1/liquer/cache.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    32155 2023-02-04 11:03:51.000000 liquer-framework-0.9.1/liquer/commands.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     3631 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/constants.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    41902 2023-05-18 22:09:05.000000 liquer-framework-0.9.1/liquer/context.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     3855 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/dependencies.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/liquer/ext/
+-rw-r--r--   0 orest     (1000) orest     (1000)        0 2019-06-09 11:48:28.000000 liquer-framework-0.9.1/liquer/ext/__init__.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     9243 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/ext/basic.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    13175 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/ext/dataframe_batches.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7937 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/ext/lq_datafusion.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     4381 2023-05-10 20:11:49.000000 liquer-framework-0.9.1/liquer/ext/lq_hxl.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     3933 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/ext/lq_keras.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     3686 2022-07-07 19:34:25.000000 liquer-framework-0.9.1/liquer/ext/lq_matplotlib.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     3447 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/ext/lq_openpyxl.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    16337 2023-05-10 20:10:02.000000 liquer-framework-0.9.1/liquer/ext/lq_pandas.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     3432 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/ext/lq_pil.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     2304 2021-10-27 15:33:04.000000 liquer-framework-0.9.1/liquer/ext/lq_plotly.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     2853 2023-01-21 20:13:08.000000 liquer-framework-0.9.1/liquer/ext/lq_polars.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     2244 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/ext/lq_pptx.py
+-rw-r--r--   0 orest     (1000) orest     (1000)      701 2021-10-27 15:33:04.000000 liquer-framework-0.9.1/liquer/ext/lq_pygments.py
+-rw-r--r--   0 orest     (1000) orest     (1000)      368 2021-10-27 15:33:04.000000 liquer-framework-0.9.1/liquer/ext/lq_python.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     1805 2021-10-27 15:33:04.000000 liquer-framework-0.9.1/liquer/ext/lq_sklearn_regression.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)      712 2023-01-21 22:45:23.000000 liquer-framework-0.9.1/liquer/ext/lq_sweetviz.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     4222 2023-05-18 21:10:33.000000 liquer-framework-0.9.1/liquer/ext/lq_whoosh.html
+-rw-rw-r--   0 orest     (1000) orest     (1000)     4300 2023-05-18 21:10:45.000000 liquer-framework-0.9.1/liquer/ext/lq_whoosh.py
+-rw-r--r--   0 orest     (1000) orest     (1000)    16409 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/ext/meta.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7326 2023-05-16 21:41:40.000000 liquer-framework-0.9.1/liquer/indexer.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7020 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/metadata.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    34618 2023-05-10 20:15:46.000000 liquer-framework-0.9.1/liquer/parser.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     6273 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/pool.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     1199 2023-01-15 17:53:35.000000 liquer-framework-0.9.1/liquer/query.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    35996 2023-06-12 20:39:36.000000 liquer-framework-0.9.1/liquer/recipes.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     4122 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/remote_store.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     5713 2023-01-08 21:15:57.000000 liquer-framework-0.9.1/liquer/s3_store.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/liquer/server/
+-rw-r--r--   0 orest     (1000) orest     (1000)        0 2019-06-09 11:48:28.000000 liquer-framework-0.9.1/liquer/server/__init__.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    14961 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/server/blueprint.py
+-rw-r--r--   0 orest     (1000) orest     (1000)    19882 2023-05-18 22:06:45.000000 liquer-framework-0.9.1/liquer/server/handlers.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/liquer/server/static/
+-rw-rw-r--   0 orest     (1000) orest     (1000)    26489 2021-01-31 21:05:09.000000 liquer-framework-0.9.1/liquer/server/static/index.html
+-rw-rw-r--   0 orest     (1000) orest     (1000)    18057 2021-12-15 17:45:48.000000 liquer-framework-0.9.1/liquer/server/static/liquer.js
+-rw-r--r--   0 orest     (1000) orest     (1000)     7371 2023-05-18 21:51:28.000000 liquer-framework-0.9.1/liquer/server/tornado_handlers.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7656 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/state.py
+-rw-r--r--   0 orest     (1000) orest     (1000)    17774 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/state_types.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    44541 2023-06-12 20:38:12.000000 liquer-framework-0.9.1/liquer/store.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    11266 2022-07-30 08:12:25.000000 liquer-framework-0.9.1/liquer/template.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)      621 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/tools.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)      521 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/util.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     2721 2023-01-21 22:45:45.000000 liquer-framework-0.9.1/liquer/web.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/liquer_framework.egg-info/
+-rw-r--r--   0 orest     (1000) orest     (1000)     7755 2023-06-12 20:44:36.000000 liquer-framework-0.9.1/liquer_framework.egg-info/PKG-INFO
+-rw-r--r--   0 orest     (1000) orest     (1000)     1339 2023-06-12 20:44:36.000000 liquer-framework-0.9.1/liquer_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 orest     (1000) orest     (1000)        1 2023-06-12 20:44:36.000000 liquer-framework-0.9.1/liquer_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 orest     (1000) orest     (1000)        1 2019-12-07 17:16:04.000000 liquer-framework-0.9.1/liquer_framework.egg-info/not-zip-safe
+-rw-r--r--   0 orest     (1000) orest     (1000)        6 2023-06-12 20:44:36.000000 liquer-framework-0.9.1/liquer_framework.egg-info/requires.txt
+-rw-r--r--   0 orest     (1000) orest     (1000)        7 2023-06-12 20:44:36.000000 liquer-framework-0.9.1/liquer_framework.egg-info/top_level.txt
+-rw-rw-r--   0 orest     (1000) orest     (1000)       38 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/setup.cfg
+-rw-r--r--   0 orest     (1000) orest     (1000)      702 2023-06-12 20:32:12.000000 liquer-framework-0.9.1/setup.py
```

### Comparing `liquer-framework-0.9.0/PKG-INFO` & `liquer-framework-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquer-framework
-Version: 0.9.0
+Version: 0.9.1
 Summary: LiQuer - Query in (URL) link
 Home-page: https://github.com/orest-d/liquer
 Author: Orest Dubay
 Author-email: orest3.dubay@gmail.com
 License: UNKNOWN
 Description: # LiQuer (Link Query) 
         
@@ -99,13 +99,14 @@
         - 2022-01-05 - v0.7.2  - several small fixes, e.g. fixing missing log in recipe-created metadata
         - 2022-01-06 - v0.7.3  - two bugfixes, recipe version
         - 2022-01-07 - v0.7.4  - more bugfixes
         - 2022-01-12 - v0.7.5  - more bugfixes, pandas_concat recipe
         - 2022-01-25 - v0.7.6  - bugfixes in recipe metadata, development of extra parameters to evaluate
         - 2023-01-22 - v0.8.0  - tools, indexers, S3 store, remote liquer as a store, 
         - 2023-06-11 - v0.9.0  - relative path in recipes, experimental search engine support (whoosh) 
+        - 2023-06-12 - v0.9.1  - fixing bugs in relative path and search engine support
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `liquer-framework-0.9.0/README.md` & `liquer-framework-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -91,7 +91,8 @@
 - 2022-01-05 - v0.7.2  - several small fixes, e.g. fixing missing log in recipe-created metadata
 - 2022-01-06 - v0.7.3  - two bugfixes, recipe version
 - 2022-01-07 - v0.7.4  - more bugfixes
 - 2022-01-12 - v0.7.5  - more bugfixes, pandas_concat recipe
 - 2022-01-25 - v0.7.6  - bugfixes in recipe metadata, development of extra parameters to evaluate
 - 2023-01-22 - v0.8.0  - tools, indexers, S3 store, remote liquer as a store, 
 - 2023-06-11 - v0.9.0  - relative path in recipes, experimental search engine support (whoosh) 
+- 2023-06-12 - v0.9.1  - fixing bugs in relative path and search engine support
```

### Comparing `liquer-framework-0.9.0/liquer/cache.py` & `liquer-framework-0.9.1/liquer/cache.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/commands.py` & `liquer-framework-0.9.1/liquer/commands.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/constants.py` & `liquer-framework-0.9.1/liquer/constants.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/context.py` & `liquer-framework-0.9.1/liquer/context.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/dependencies.py` & `liquer-framework-0.9.1/liquer/dependencies.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/basic.py` & `liquer-framework-0.9.1/liquer/ext/basic.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/dataframe_batches.py` & `liquer-framework-0.9.1/liquer/ext/dataframe_batches.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_datafusion.py` & `liquer-framework-0.9.1/liquer/ext/lq_datafusion.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_hxl.py` & `liquer-framework-0.9.1/liquer/ext/lq_hxl.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_keras.py` & `liquer-framework-0.9.1/liquer/ext/lq_keras.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_matplotlib.py` & `liquer-framework-0.9.1/liquer/ext/lq_matplotlib.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_openpyxl.py` & `liquer-framework-0.9.1/liquer/ext/lq_openpyxl.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_pandas.py` & `liquer-framework-0.9.1/liquer/ext/lq_pandas.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_pil.py` & `liquer-framework-0.9.1/liquer/ext/lq_pil.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_plotly.py` & `liquer-framework-0.9.1/liquer/ext/lq_plotly.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_polars.py` & `liquer-framework-0.9.1/liquer/ext/lq_polars.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_pptx.py` & `liquer-framework-0.9.1/liquer/ext/lq_pptx.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_pygments.py` & `liquer-framework-0.9.1/liquer/ext/lq_pygments.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_sklearn_regression.py` & `liquer-framework-0.9.1/liquer/ext/lq_sklearn_regression.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_sweetviz.py` & `liquer-framework-0.9.1/liquer/ext/lq_sweetviz.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/lq_whoosh.py` & `liquer-framework-0.9.1/liquer/ext/lq_whoosh.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/ext/meta.py` & `liquer-framework-0.9.1/liquer/ext/meta.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/indexer.py` & `liquer-framework-0.9.1/liquer/indexer.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/metadata.py` & `liquer-framework-0.9.1/liquer/metadata.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/parser.py` & `liquer-framework-0.9.1/liquer/parser.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/pool.py` & `liquer-framework-0.9.1/liquer/pool.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/query.py` & `liquer-framework-0.9.1/liquer/query.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/recipes.py` & `liquer-framework-0.9.1/liquer/recipes.py`

 * *Files 0% similar despite different names*

```diff
@@ -844,14 +844,15 @@
                     for directory, items in spec.items():
                         for i, r in enumerate(items):
                             cwd = (
                                 parent
                                 if directory == self.LOCAL_RECIPES
                                 else join_key(parent, directory)
                             )
+                            cwd = self.to_root_key(cwd)
                             d = resolve_recipe_definition(r, cwd, metadata)
                             if d is None:
                                 metadata.warning(
                                     f"Failed parsing the definition of recipe {i+1} in {directory}"
                                 )
                             d["recipe_name"] = (
                                 self.to_root_key(recipes_key)
```

### Comparing `liquer-framework-0.9.0/liquer/remote_store.py` & `liquer-framework-0.9.1/liquer/remote_store.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/s3_store.py` & `liquer-framework-0.9.1/liquer/s3_store.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/server/blueprint.py` & `liquer-framework-0.9.1/liquer/server/blueprint.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/server/handlers.py` & `liquer-framework-0.9.1/liquer/server/handlers.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/server/static/index.html` & `liquer-framework-0.9.1/liquer/server/static/index.html`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/server/static/liquer.js` & `liquer-framework-0.9.1/liquer/server/static/liquer.js`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/server/tornado_handlers.py` & `liquer-framework-0.9.1/liquer/server/tornado_handlers.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/state.py` & `liquer-framework-0.9.1/liquer/state.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/state_types.py` & `liquer-framework-0.9.1/liquer/state_types.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/store.py` & `liquer-framework-0.9.1/liquer/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -652,14 +652,15 @@
 
 
 class ProxyStore(Store):
     """Proxy to another store - can be used as a basis to override certain behaviour"""
 
     def __init__(self, store):
         self._store = store
+        self._store.parent_store = self
 
     def sync(self):
         self._store.sync()
 
     def get_bytes(self, key):
         return self._store.get_bytes(key)
 
@@ -723,15 +724,17 @@
         metadata = index(key=self.to_root_key(key), query=metadata.get("query"), data=data, metadata=metadata)
         self._store.store(key, data, metadata)
         self.on_data_changed(key)
         self.on_metadata_changed(key)
 
     def mount(self, key, store):
         """Mount a store in a mount-point"""
-        return self._store.mount(key, store)
+        r = self._store.mount(key, store)
+        self.sync()
+        return r
 
     def __str__(self):
         return f"Indexing {self._store}"
 
     def __repr__(self):
         return f"IndexerStore({repr(self._store)})"
 
@@ -1107,14 +1110,15 @@
         return self
 
     def mount(self, key, store):
         self.umount(key)
         prefix_store = PrefixStore(store, prefix=key)
         prefix_store.parent_store = self
         self.routing_table.append((key, prefix_store))
+        self.sync()
         return self
 
     def route_to(self, key):
         for prefix, store in reversed(self.routing_table):
             if key == prefix:
                 return store
             if not prefix.endswith("/"):
```

### Comparing `liquer-framework-0.9.0/liquer/template.py` & `liquer-framework-0.9.1/liquer/template.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/tools.py` & `liquer-framework-0.9.1/liquer/tools.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/util.py` & `liquer-framework-0.9.1/liquer/util.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer/web.py` & `liquer-framework-0.9.1/liquer/web.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.0/liquer_framework.egg-info/PKG-INFO` & `liquer-framework-0.9.1/liquer_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquer-framework
-Version: 0.9.0
+Version: 0.9.1
 Summary: LiQuer - Query in (URL) link
 Home-page: https://github.com/orest-d/liquer
 Author: Orest Dubay
 Author-email: orest3.dubay@gmail.com
 License: UNKNOWN
 Description: # LiQuer (Link Query) 
         
@@ -99,13 +99,14 @@
         - 2022-01-05 - v0.7.2  - several small fixes, e.g. fixing missing log in recipe-created metadata
         - 2022-01-06 - v0.7.3  - two bugfixes, recipe version
         - 2022-01-07 - v0.7.4  - more bugfixes
         - 2022-01-12 - v0.7.5  - more bugfixes, pandas_concat recipe
         - 2022-01-25 - v0.7.6  - bugfixes in recipe metadata, development of extra parameters to evaluate
         - 2023-01-22 - v0.8.0  - tools, indexers, S3 store, remote liquer as a store, 
         - 2023-06-11 - v0.9.0  - relative path in recipes, experimental search engine support (whoosh) 
+        - 2023-06-12 - v0.9.1  - fixing bugs in relative path and search engine support
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `liquer-framework-0.9.0/liquer_framework.egg-info/SOURCES.txt` & `liquer-framework-0.9.1/liquer_framework.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 liquer/ext/lq_plotly.py
 liquer/ext/lq_polars.py
 liquer/ext/lq_pptx.py
 liquer/ext/lq_pygments.py
 liquer/ext/lq_python.py
 liquer/ext/lq_sklearn_regression.py
 liquer/ext/lq_sweetviz.py
+liquer/ext/lq_whoosh.html
 liquer/ext/lq_whoosh.py
 liquer/ext/meta.py
 liquer/server/__init__.py
 liquer/server/blueprint.py
 liquer/server/handlers.py
 liquer/server/tornado_handlers.py
 liquer/server/static/index.html
```

### Comparing `liquer-framework-0.9.0/setup.py` & `liquer-framework-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="liquer-framework",
-    version="0.9.0",
+    version="0.9.1",
     author="Orest Dubay",
     author_email="orest3.dubay@gmail.com",
     description="LiQuer - Query in (URL) link",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/orest-d/liquer",
     packages=setuptools.find_packages(),
```

