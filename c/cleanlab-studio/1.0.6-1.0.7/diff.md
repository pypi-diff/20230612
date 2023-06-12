# Comparing `tmp/cleanlab-studio-1.0.6.tar.gz` & `tmp/cleanlab-studio-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-1.0.6.tar", last modified: Sat Jun  3 04:37:22 2023, max compression
+gzip compressed data, was "cleanlab-studio-1.0.7.tar", last modified: Mon Jun 12 18:54:34 2023, max compression
```

## Comparing `cleanlab-studio-1.0.6.tar` & `cleanlab-studio-1.0.7.tar`

### file list

```diff
@@ -1,84 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.291629 cleanlab-studio-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-06-03 04:37:22.291629 cleanlab-studio-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.271629 cleanlab-studio-1.0.6/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.275629 cleanlab-studio-1.0.6/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.279629 cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.279629 cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.279629 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/schema_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/upload_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.283629 cleanlab-studio-1.0.6/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.283629 cleanlab-studio-1.0.6/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.283629 cleanlab-studio-1.0.6/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.283629 cleanlab-studio-1.0.6/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.287629 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.287629 cleanlab-studio-1.0.6/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/studio/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/studio/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.275629 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-06-03 04:37:22.000000 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-03 04:37:22.000000 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 04:37:22.000000 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-03 04:37:22.000000 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-03 04:37:22.000000 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-03 04:37:22.000000 cleanlab-studio-1.0.6/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 04:37:22.291629 cleanlab-studio-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.287629 cleanlab-studio-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/bench.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:22.291629 cleanlab-studio-1.0.6/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/datasets/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/datasets/test_excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/datasets/test_json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-03 04:37:07.000000 cleanlab-studio-1.0.6/tests/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.324787 cleanlab-studio-1.0.7/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.324787 cleanlab-studio-1.0.7/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.324787 cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.324787 cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.324787 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/schema_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/upload_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/studio/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/studio/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.324787 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-06-12 18:54:34.000000 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-12 18:54:34.000000 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:54:34.000000 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 18:54:34.000000 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-12 18:54:34.000000 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 18:54:34.000000 cleanlab-studio-1.0.7/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:34.328787 cleanlab-studio-1.0.7/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/datasets/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/datasets/test_excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/datasets/test_json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-12 18:54:18.000000 cleanlab-studio-1.0.7/tests/datasets/utils.py
```

### Comparing `cleanlab-studio-1.0.6/LICENSE` & `cleanlab-studio-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/PKG-INFO` & `cleanlab-studio-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.6
+Version: 1.0.7
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://cleanlab-studio.readthedocs.io/en/latest/index.html
@@ -55,15 +55,15 @@
 
 ## Quickstart
 
 ### Python API
 
 You can find your API key at https://app.cleanlab.ai/account.
 ```python
-import cleanlab_studio
+from cleanlab_studio import Studio
 
 # create your Cleanlab Studio API client with your API key, found here: https://app.cleanlab.ai/account
 studio = Studio(<your api key>)
 
 # upload your dataset via a filepath, Pandas DataFrame, or PySpark DataFrame!
 dataset_id: str = studio.upload_dataset(<your dataset>, <your dataset name>)
```

### Comparing `cleanlab-studio-1.0.6/README.md` & `cleanlab-studio-1.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Quickstart
 
 ### Python API
 
 You can find your API key at https://app.cleanlab.ai/account.
 ```python
-import cleanlab_studio
+from cleanlab_studio import Studio
 
 # create your Cleanlab Studio API client with your API key, found here: https://app.cleanlab.ai/account
 studio = Studio(<your api key>)
 
 # upload your dataset via a filepath, Pandas DataFrame, or PySpark DataFrame!
 dataset_id: str = studio.upload_dataset(<your dataset>, <your dataset name>)
```

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/api_service.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/api_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import pathlib
 import asyncio
 from typing import List, Any, Optional, Tuple
 
 import aiohttp
 import requests
+import pandas as pd
 
 from cleanlab_studio.version import __version__
 from cleanlab_studio.cli.click_helpers import abort, warn, info
 from cleanlab_studio.cli.dataset.image_utils import get_image_filepath
 from cleanlab_studio.cli.dataset.schema_types import Schema
 from cleanlab_studio.cli.types import JSONDict, IDType, MEDIA_MODALITIES
 
@@ -251,30 +252,31 @@
                 await asyncio.sleep(wait)
                 wait *= 2
                 retries -= 1
             return False, original_filepath
     return None, original_filepath
 
 
-def download_cleanlab_columns(api_key: str, cleanset_id: str, all: bool = False) -> List[List[Any]]:
+def download_cleanlab_columns(api_key: str, cleanset_id: str, all: bool = False) -> pd.DataFrame:
     """
     Download all rows from specified Cleanlab columns
 
     :param api_key:
     :param cleanset_id:
     :param all: whether to download all Cleanlab columns or just the clean_label column
     :return: return (rows, id_column)
     """
     res = requests.get(
         cli_base_url + f"/cleansets/{cleanset_id}/columns?all={all}",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
-    rows: List[List[Any]] = res.json()["rows"]
-    return rows
+    cleanset_json: str = res.json()["cleanset_json"]
+    cleanset_df: pd.DataFrame = pd.read_json(cleanset_json, orient="table")
+    return cleanset_df
 
 
 def get_completion_status(api_key: str, dataset_id: str) -> bool:
     res = requests.get(
         cli_base_url + f"/datasets/{dataset_id}/complete",
         headers=_construct_headers(api_key),
     )
```

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/dataset.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/download.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from cleanlab_studio.cli.cleanset.download_helpers import combine_fields_with_dataset
 from cleanlab_studio.cli.click_helpers import log, progress
 from cleanlab_studio.cli.decorators import previous_state, auth_config
 from cleanlab_studio.cli.decorators.auth_config import AuthConfig
 from cleanlab_studio.cli.decorators.previous_state import PreviousState
 from cleanlab_studio.cli.types import RecordType, DatasetFileExtension
 from cleanlab_studio.internal.settings import CleanlabSettings
+from cleanlab_studio.internal.api import api
 
 
 @click.command(help="download Cleanlab columns")
 @click.option(
     "--id",
     type=str,
     prompt=True,
@@ -57,24 +58,22 @@
     filepath: Optional[str],
     output: Optional[str],
     all: bool,
 ) -> None:
     prev_state.init_state(dict(command="download labels", args=dict(id=id)))
     CleanlabSettings.init_cleanlab_dir()
     api_key = config.get_api_key()
-    progress("Downloading Cleanlab columns...")
-    rows = api_service.download_cleanlab_columns(api_key, cleanset_id=id, all=all)
+    id_column = api_service.get_id_column(api_key, cleanset_id=id)
 
-    if all:
-        clean_df_columns = ["id", "issue", "label_quality", "suggested_label", "clean_label"]
-    else:
-        clean_df_columns = ["id", "clean_label"]
+    progress("Downloading Cleanlab columns...")
+    clean_df = api_service.download_cleanlab_columns(api_key, cleanset_id=id, all=all)
+    clean_df = clean_df.set_index(id_column)
+    clean_df = drop_action_col(clean_df)
 
     if filepath:
-        id_column = api_service.get_id_column(api_key, cleanset_id=id)
         if not os.path.exists(filepath):
             log(f"Specified file {filepath} could not be found.")
             filepath = click_helpers.prompt_for_filepath("Specify your dataset filepath")
 
         filename = util.get_filename(filepath)
         while output is None:
             output = click.prompt(
@@ -83,25 +82,28 @@
             )
             if os.path.exists(output):
                 click_helpers.error(
                     "A file already exists at this filepath, use a different filepath."
                 )
                 output = None
 
-        clean_df = pd.DataFrame(rows, columns=clean_df_columns).set_index("id")
-
         ids_to_fields_to_values: Dict[str, RecordType] = defaultdict(dict)
         for row_id, row in clean_df.iterrows():
             fields_to_values = dict(row)
             ids_to_fields_to_values[str(row_id)] = fields_to_values
 
         combine_fields_with_dataset(filepath, id_column, ids_to_fields_to_values, output)
         click_helpers.success(f"Saved to {output}")
     else:
         while output is None or util.get_dataset_file_extension(output) != DatasetFileExtension.csv:
             output = click.prompt(
                 "Specify your output filepath (must be .csv). Leave blank to use default",
                 default=f"clean_labels.csv",
             )
-        clean_df = pd.DataFrame(rows, columns=clean_df_columns)
-        clean_df.to_csv(output, index=False)
+        clean_df.to_csv(output)
         click_helpers.success(f"Saved to {output}")
+
+
+def drop_action_col(dataframe: pd.DataFrame) -> pd.DataFrame:
+    if "action" in dataframe.columns:
+        return dataframe.drop("action", axis=1)
+    return dataframe
```

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/click_helpers.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/helpers.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/image_utils.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/image_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/schema_types.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/schema_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/upload.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/upload_helpers.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/dataset/upload_types.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/dataset/upload_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/login/login.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/main.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/types.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/cli/util.py` & `cleanlab-studio-1.0.7/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/errors.py` & `cleanlab-studio-1.0.7/cleanlab_studio/errors.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/internal/api/api.py` & `cleanlab-studio-1.0.7/cleanlab_studio/internal/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import time
-from typing import Any, Callable, List, Optional, Tuple
+from typing import Any, Callable, List, Optional, Tuple, Dict
 from cleanlab_studio.errors import APIError
 
 import requests
 from tqdm import tqdm
+import pandas as pd
 
 from cleanlab_studio.internal.types import JSONDict
 from cleanlab_studio.version import __version__
 
 base_url = os.environ.get("CLEANLAB_API_BASE_URL", "https://api.cleanlab.ai/api")
 cli_base_url = f"{base_url}/cli/v0"
 upload_base_url = f"{base_url}/upload/v0"
@@ -148,30 +149,31 @@
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     label_column: str = res.json()["label_column"]
     return label_column
 
 
-def download_cleanlab_columns(api_key: str, cleanset_id: str, all: bool = False) -> List[List[Any]]:
+def download_cleanlab_columns(api_key: str, cleanset_id: str, all: bool = False) -> pd.DataFrame:
     """
     Download all rows from specified Cleanlab columns
 
     :param api_key:
     :param cleanset_id:
     :param all: whether to download all Cleanlab columns or just the clean_label column
     :return: return (rows, id_column)
     """
     res = requests.get(
         cli_base_url + f"/cleansets/{cleanset_id}/columns?all={all}",
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
-    rows: List[List[Any]] = res.json()["rows"]
-    return rows
+    cleanset_json: str = res.json()["cleanset_json"]
+    cleanset_df: pd.DataFrame = pd.read_json(cleanset_json, orient="table")
+    return cleanset_df
 
 
 def get_id_column(api_key: str, cleanset_id: str) -> str:
     res = requests.get(
         cli_base_url + f"/cleansets/{cleanset_id}/id_column",
         headers=_construct_headers(api_key),
     )
```

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab-studio-1.0.7/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/internal/settings.py` & `cleanlab-studio-1.0.7/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/internal/upload_helpers.py` & `cleanlab-studio-1.0.7/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/internal/util.py` & `cleanlab-studio-1.0.7/cleanlab_studio/internal/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,16 +43,7 @@
         from .dataset_source import PySparkDatasetSource
 
         if dataset_name is None:
             raise ValueError("Must provide dataset name if uploading from a DataFrame")
         return PySparkDatasetSource(df=dataset_source, dataset_name=dataset_name)
     else:
         raise ValueError("Invalid dataset source provided")
-
-
-def as_numpy_type(field_type: str) -> Any:
-    return {
-        "string": str,
-        "integer": np.int64,  # XXX backend might use big integers
-        "float": np.float64,
-        "boolean": bool,
-    }[field_type]
```

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/studio/clean.py` & `cleanlab-studio-1.0.7/cleanlab_studio/studio/clean.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/studio/studio.py` & `cleanlab-studio-1.0.7/cleanlab_studio/studio/studio.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import Any, List, Literal, Optional
 
 import numpy as np
+import numpy.typing as npt
 import pandas as pd
 
 try:
     import pyspark.sql
 
     pyspark_exists = True
 except ImportError:
     pyspark_exists = False
 
 from . import clean, upload
 from cleanlab_studio.internal.api import api
-from cleanlab_studio.internal.util import init_dataset_source, as_numpy_type
+from cleanlab_studio.internal.util import init_dataset_source
 from cleanlab_studio.internal.settings import CleanlabSettings
 from cleanlab_studio.internal.types import FieldSchemaDict
 
 
 class Studio:
     _api_key: str
 
@@ -51,67 +52,29 @@
             self._api_key,
             ds,
             schema_overrides=schema_overrides,
             modality=modality,
             id_column=id_column,
         )
 
-    def download_cleanlab_columns(self, cleanset_id: str) -> pd.DataFrame:
-        project_id = api.get_project_of_cleanset(self._api_key, cleanset_id)
-        label_column = api.get_label_column_of_project(self._api_key, project_id)
-        return self._download_cleanlab_columns(cleanset_id, project_id, label_column)
-
-    def _download_cleanlab_columns(
+    def download_cleanlab_columns(
         self,
         cleanset_id: str,
-        project_id: str,
-        label_column: str,
         include_action: bool = False,
     ) -> pd.DataFrame:
-        rows = api.download_cleanlab_columns(self._api_key, cleanset_id, all=True)
-        id_col = api.get_id_column(self._api_key, cleanset_id)
-        # TODO actually get _all_ the columns incl e.g., cleanlab_top_labels
-        # and have the API give the column headers rather than this library hard-coding it
-        headers = [
-            id_col,
-            "cleanlab_issue",
-            "cleanlab_label_quality",
-            "cleanlab_suggested_label",
-            "cleanlab_clean_label",
-        ]
-        if include_action:
-            headers.append("action")
-        dataset_id = api.get_dataset_of_project(self._api_key, project_id)
-        schema = api.get_dataset_schema(self._api_key, dataset_id)
-        col_types = {
-            id_col: as_numpy_type(schema["fields"][id_col]["data_type"]),
-            "cleanlab_issue": bool,
-            "cleanlab_label_quality": np.float64,
-            "cleanlab_suggested_label": as_numpy_type(schema["fields"][label_column]["data_type"]),
-            "cleanlab_clean_label": as_numpy_type(schema["fields"][label_column]["data_type"]),
-        }
-        if include_action:
-            col_types["action"] = str
-
-        # convert to dict/column-major format
-        d = {
-            headers[j]: np.array(
-                [rows[i][j] for i in range(len(rows))], dtype=col_types[headers[j]]
-            )
-            for j in range(len(headers))
-        }
-        return pd.DataFrame(d)
+        rows_df: pd.DataFrame = api.download_cleanlab_columns(self._api_key, cleanset_id, all=True)
+        if not include_action:
+            rows_df.drop("action", inplace=True, axis=1)
+        return rows_df
 
     def apply_corrections(self, cleanset_id: str, dataset: Any) -> Any:
         project_id = api.get_project_of_cleanset(self._api_key, cleanset_id)
         label_column = api.get_label_column_of_project(self._api_key, project_id)
         id_col = api.get_id_column(self._api_key, cleanset_id)
-        cl_cols = self._download_cleanlab_columns(
-            cleanset_id, project_id, label_column, include_action=True
-        )
+        cl_cols = self.download_cleanlab_columns(cleanset_id, include_action=True)
         if pyspark_exists and isinstance(dataset, pyspark.sql.DataFrame):
             from pyspark.sql.functions import udf
 
             spark = dataset.sparkSession
             cl_cols_df = spark.createDataFrame(cl_cols)
             corrected_ds = dataset.alias("corrected_ds")
             if id_col not in corrected_ds.columns:
@@ -121,26 +84,26 @@
                 )
                 from pyspark.sql.window import Window
 
                 corrected_ds = corrected_ds.withColumn(
                     id_col,
                     row_number().over(Window.orderBy(monotonically_increasing_id())) - 1,
                 )
-            both = cl_cols_df.select([id_col, "action", "cleanlab_clean_label"]).join(
+            both = cl_cols_df.select([id_col, "action", "clean_label"]).join(
                 corrected_ds.select([id_col, label_column]),
                 on=id_col,
                 how="left",
             )
             final = both.withColumn(
                 "__cleanlab_final_label",
                 # XXX hacky, relies on no labels being "None" (the string)
                 # instead, use original JSON, which uses null values where it's not specified
                 udf(lambda original, clean: original if clean == "None" else clean)(
                     both[label_column],
-                    "cleanlab_clean_label",
+                    "clean_label",
                 ),
             )
             new_labels = final.select(
                 [id_col, "action", "__cleanlab_final_label"]
             ).withColumnRenamed("__cleanlab_final_label", label_column)
             return (
                 corrected_ds.drop(label_column)
@@ -150,16 +113,16 @@
             )
         elif isinstance(dataset, pd.DataFrame):
             joined_ds: pd.DataFrame
             if id_col in dataset.columns:
                 joined_ds = dataset.join(cl_cols.set_index(id_col), on=id_col)
             else:
                 joined_ds = dataset.join(cl_cols.set_index(id_col).sort_values(by=id_col))
-            joined_ds["__cleanlab_final_label"] = joined_ds["cleanlab_clean_label"].where(
-                joined_ds["cleanlab_clean_label"] != "None", dataset[label_column]
+            joined_ds["__cleanlab_final_label"] = joined_ds["clean_label"].where(
+                joined_ds["clean_label"] != "None", dataset[label_column]
             )
 
             corrected_ds = dataset.copy()
             corrected_ds[label_column] = joined_ds["__cleanlab_final_label"]
             corrected_ds = corrected_ds[joined_ds["action"] != "exclude"]
             return corrected_ds
```

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio/studio/upload.py` & `cleanlab-studio-1.0.7/cleanlab_studio/studio/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab-studio-1.0.7/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.6
+Version: 1.0.7
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://cleanlab-studio.readthedocs.io/en/latest/index.html
@@ -55,15 +55,15 @@
 
 ## Quickstart
 
 ### Python API
 
 You can find your API key at https://app.cleanlab.ai/account.
 ```python
-import cleanlab_studio
+from cleanlab_studio import Studio
 
 # create your Cleanlab Studio API client with your API key, found here: https://app.cleanlab.ai/account
 studio = Studio(<your api key>)
 
 # upload your dataset via a filepath, Pandas DataFrame, or PySpark DataFrame!
 dataset_id: str = studio.upload_dataset(<your dataset>, <your dataset name>)
```

### Comparing `cleanlab-studio-1.0.6/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab-studio-1.0.7/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,13 @@
 cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
 cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
 cleanlab_studio/studio/__init__.py
 cleanlab_studio/studio/clean.py
 cleanlab_studio/studio/studio.py
 cleanlab_studio/studio/upload.py
 tests/__init__.py
-tests/bench.py
 tests/datasets/__init__.py
 tests/datasets/constants.py
 tests/datasets/test_csv_dataset.py
 tests/datasets/test_excel_dataset.py
 tests/datasets/test_json_dataset.py
 tests/datasets/utils.py
```

### Comparing `cleanlab-studio-1.0.6/setup.py` & `cleanlab-studio-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/tests/datasets/test_csv_dataset.py` & `cleanlab-studio-1.0.7/tests/datasets/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/tests/datasets/test_excel_dataset.py` & `cleanlab-studio-1.0.7/tests/datasets/test_excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/tests/datasets/test_json_dataset.py` & `cleanlab-studio-1.0.7/tests/datasets/test_json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.6/tests/datasets/utils.py` & `cleanlab-studio-1.0.7/tests/datasets/utils.py`

 * *Files identical despite different names*

