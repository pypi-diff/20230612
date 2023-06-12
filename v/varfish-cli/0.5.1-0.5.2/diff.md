# Comparing `tmp/varfish_cli-0.5.1.tar.gz` & `tmp/varfish_cli-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varfish_cli-0.5.1.tar", last modified: Thu Feb  9 12:03:49 2023, max compression
+gzip compressed data, was "varfish_cli-0.5.2.tar", last modified: Mon Jun 12 16:26:03 2023, max compression
```

## Comparing `varfish_cli-0.5.1.tar` & `varfish_cli-0.5.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 12:03:49.489602 varfish_cli-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-02-09 12:03:49.489602 varfish_cli-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 12:03:49.485602 varfish_cli-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/docs/cli_docs.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5264 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 12:03:49.485602 varfish_cli-0.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/requirements/develop.txt
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/requirements/test_black.txt
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-09 12:03:49.489602 varfish_cli-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 12:03:49.485602 varfish_cli-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 12:03:49.481602 varfish_cli-0.5.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 12:03:49.485602 varfish_cli-0.5.1/tests/data/config/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/tests/data/config/varfishrc.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 12:03:49.485602 varfish_cli-0.5.1/tests/data/parse_ped/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/tests/data/parse_ped/trio.ped
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/tests/test_parse_ped.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/tests/test_run_case_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 12:03:49.489602 varfish_cli-0.5.1/varfish_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-09 12:03:49.489602 varfish_cli-0.5.1/varfish_cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 12:03:49.485602 varfish_cli-0.5.1/varfish_cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38452 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/api/case.py
--rw-r--r--   0 runner    (1001) docker     (123)    19635 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/api/varannos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 12:03:49.489602 varfish_cli-0.5.1/varfish_cli/case/
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/case/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    36213 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/case/create_case_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/case/list_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/case/list_case_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/case/small_var_query_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/case/small_var_query_fetch_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/case/small_var_query_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/case/small_var_query_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/case/small_var_query_settings_shortcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/case/small_var_query_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/case/small_var_query_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/parse_ped.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 12:03:49.489602 varfish_cli-0.5.1/varfish_cli/varannos/
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/varannos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/varannos/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/varannos/varannoset_destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/varannos/varannoset_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/varannos/varannoset_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/varannos/varannoset_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/varannos/varannosetentry_destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/varannos/varannosetentry_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/varannos/varannosetentry_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/varfish_cli/varannos/varannosetentry_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 12:03:49.485602 varfish_cli-0.5.1/varfish_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-02-09 12:03:49.000000 varfish_cli-0.5.1/varfish_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-02-09 12:03:49.000000 varfish_cli-0.5.1/varfish_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 12:03:49.000000 varfish_cli-0.5.1/varfish_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-09 12:03:49.000000 varfish_cli-0.5.1/varfish_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 12:03:49.000000 varfish_cli-0.5.1/varfish_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-09 12:03:49.000000 varfish_cli-0.5.1/varfish_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-09 12:03:49.000000 varfish_cli-0.5.1/varfish_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68448 2023-02-09 12:03:41.000000 varfish_cli-0.5.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.538033 varfish_cli-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-12 16:26:03.538033 varfish_cli-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.530033 varfish_cli-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/cli_docs.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5264 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.530033 varfish_cli-0.5.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/requirements/develop.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/requirements/test_black.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-12 16:26:03.538033 varfish_cli-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.534033 varfish_cli-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.530033 varfish_cli-0.5.2/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.534033 varfish_cli-0.5.2/tests/data/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/data/config/varfishrc.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.534033 varfish_cli-0.5.2/tests/data/parse_ped/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/data/parse_ped/trio.ped
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/test_parse_ped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/tests/test_run_case_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.538033 varfish_cli-0.5.2/varfish_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-12 16:26:03.538033 varfish_cli-0.5.2/varfish_cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.534033 varfish_cli-0.5.2/varfish_cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39072 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/api/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/api/varannos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.534033 varfish_cli-0.5.2/varfish_cli/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36213 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/create_case_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/list_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/list_case_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_fetch_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_settings_shortcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/case/small_var_query_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/parse_ped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.538033 varfish_cli-0.5.2/varfish_cli/varannos/
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannoset_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannoset_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannoset_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannoset_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:26:03.534033 varfish_cli-0.5.2/varfish_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 16:26:03.000000 varfish_cli-0.5.2/varfish_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68448 2023-06-12 16:26:00.000000 varfish_cli-0.5.2/versioneer.py
```

### Comparing `varfish_cli-0.5.1/CHANGELOG.md` & `varfish_cli-0.5.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+### [0.5.2](https://www.github.com/bihealth/varfish-cli/compare/v0.5.1...v0.5.2) (2023-06-12)
+
+
+### Bug Fixes
+
+* Fixing case list API ([#37](https://www.github.com/bihealth/varfish-cli/issues/37)) ([ccaccfc](https://www.github.com/bihealth/varfish-cli/commit/ccaccfcbec7fb209492f1855b5e740f20ac60bbc))
+
 ### [0.5.1](https://www.github.com/bihealth/varfish-cli/compare/v0.5.0...v0.5.1) (2023-02-09)
 
 
 ### Bug Fixes
 
 * manifest for readme and changelog ([#35](https://www.github.com/bihealth/varfish-cli/issues/35)) ([f14d647](https://www.github.com/bihealth/varfish-cli/commit/f14d6472728995b9e18726fbfb7c36e86319c999))
```

### Comparing `varfish_cli-0.5.1/LICENSE` & `varfish_cli-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/PKG-INFO` & `varfish_cli-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varfish_cli
-Version: 0.5.1
+Version: 0.5.2
 Summary: Command line interface client for VarFish Server.
 Home-page: https://github.com/bihealth/varfish-cli
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bihealth.de
 License: MIT license
 Keywords: varfish_cli
 Classifier: Development Status :: 4 - Beta
@@ -86,14 +86,21 @@
 varfish_api_token = "XXX"
 EOF
 ```
 
 
 # Changelog
 
+### [0.5.2](https://www.github.com/bihealth/varfish-cli/compare/v0.5.1...v0.5.2) (2023-06-12)
+
+
+### Bug Fixes
+
+* Fixing case list API ([#37](https://www.github.com/bihealth/varfish-cli/issues/37)) ([ccaccfc](https://www.github.com/bihealth/varfish-cli/commit/ccaccfcbec7fb209492f1855b5e740f20ac60bbc))
+
 ### [0.5.1](https://www.github.com/bihealth/varfish-cli/compare/v0.5.0...v0.5.1) (2023-02-09)
 
 
 ### Bug Fixes
 
 * manifest for readme and changelog ([#35](https://www.github.com/bihealth/varfish-cli/issues/35)) ([f14d647](https://www.github.com/bihealth/varfish-cli/commit/f14d6472728995b9e18726fbfb7c36e86319c999))
```

### Comparing `varfish_cli-0.5.1/README.md` & `varfish_cli-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/docs/Makefile` & `varfish_cli-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/docs/conf.py` & `varfish_cli-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/docs/make.bat` & `varfish_cli-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/requirements/base.txt` & `varfish_cli-0.5.2/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/requirements/test.txt` & `varfish_cli-0.5.2/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/requirements.txt` & `varfish_cli-0.5.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/setup.cfg` & `varfish_cli-0.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/setup.py` & `varfish_cli-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/tests/test_config.py` & `varfish_cli-0.5.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/tests/test_parse_ped.py` & `varfish_cli-0.5.2/tests/test_parse_ped.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/tests/test_run_case_list.py` & `varfish_cli-0.5.2/tests/test_run_case_list.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,32 +6,40 @@
 
 from varfish_cli.__main__ import main
 from varfish_cli.api import CONVERTER, models
 
 
 def test_run_case_list():
     url = "https://varfish.example.com"
-    address = "%s/variants/api/case/list/c3752df7-fa32-4784-8a48-e8f0e5a28790/" % url
+    address = "%s/cases/api/case/list/c3752df7-fa32-4784-8a48-e8f0e5a28790/" % url
     cases = CONVERTER.unstructure(
-        [
-            models.Case(
-                sodar_uuid=str(uuid.uuid4()),
-                date_created=datetime.datetime.now(),
-                date_modified=datetime.datetime.now(),
-                name="Case_Name",
-                index="index",
-                pedigree=[
-                    models.PedigreeMember(
-                        name="index", father="0", mother="0", sex=2, affected=2, has_gt_entries=True
-                    )
-                ],
-                num_small_vars=123,
-                num_svs=456,
-            )
-        ]
+        {
+            "next": None,
+            "results": [
+                models.Case(
+                    sodar_uuid=str(uuid.uuid4()),
+                    date_created=datetime.datetime.now(),
+                    date_modified=datetime.datetime.now(),
+                    name="Case_Name",
+                    index="index",
+                    pedigree=[
+                        models.PedigreeMember(
+                            name="index",
+                            father="0",
+                            mother="0",
+                            sex=2,
+                            affected=2,
+                            has_gt_entries=True,
+                        )
+                    ],
+                    num_small_vars=123,
+                    num_svs=456,
+                )
+            ],
+        }
     )
     with requests_mock.Mocker() as m:
         m.get(address, json=cases)
         base_dir = pathlib.Path(__file__).parent
         main(
             [
                 "--config",
```

### Comparing `varfish_cli-0.5.1/varfish_cli/__main__.py` & `varfish_cli-0.5.2/varfish_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/api/case.py` & `varfish_cli-0.5.2/varfish_cli/api/case.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 from ..exceptions import RestApiCallException
 
 ACCEPT_API_VARFISH = ""
 
 
 #: End point for listing cases.
-ENDPOINT_CASE_LIST = "/variants/api/case/list/{project_uuid}/"
+ENDPOINT_CASE_LIST = "/cases/api/case/list/{project_uuid}/"
 #: End point for fetching case information.
 ENDPOINT_CASE_RETRIEVE = "/variants/api/case/retrieve/{case_uuid}"
 #: End point for listing case import infos.
 ENDPOINT_CASE_IMPORT_INFO_LIST = "/importer/api/case-import-info/{project_uuid}/"
 #: End point for creating case import infos.
 ENDPOINT_CASE_IMPORT_INFO_CREATE = ENDPOINT_CASE_IMPORT_INFO_LIST
 #: End point for updating case import infos.
@@ -123,28 +123,49 @@
             " ".join([" ".join(v) for v in response.json().values()]),
         )
     except (JSONDecodeError, SimpleJSONDecodeError):
         msg = "REST API returned status code %d: %s" % (response.status_code, response.content)
     return RestApiCallException(msg)
 
 
+def _paginated_request(endpoint, result_data=None, **kwargs):
+    if not endpoint:
+        return result_data
+
+    if result_data is None:
+        result_data = []
+
+    result = requests.get(endpoint, **kwargs)
+    result.raise_for_status()
+
+    result_json = result.json()
+    if "results" in result_json and "next" in result_json:
+        result_data += result_json["results"]
+        return _paginated_request(result_json["next"], result_data=result_data, **kwargs)
+    else:
+        raise RestApiCallException(
+            f"Call against {endpoint} did not return paginated object: {result_json}"
+        )
+
+
 def case_list(
     server_url: str,
     api_token: str,
     project_uuid: typing.Union[str, uuid.UUID],
     verify_ssl: bool = True,
 ) -> typing.List[Case]:
     """Listing of cases from a project UUID."""
     server_url = strip_trailing_slash(server_url)
     endpoint = "%s%s" % (server_url, ENDPOINT_CASE_LIST.format(project_uuid=project_uuid))
     logger.debug("Sending GET request to end point %s", endpoint)
     headers = {"Authorization": "Token %s" % api_token}
-    result = requests.get(endpoint, headers=headers, verify=verify_ssl)
-    result.raise_for_status()
-    return CONVERTER.structure(result.json(), typing.List[Case])
+    result = _paginated_request(
+        endpoint, headers=headers, verify=verify_ssl, params={"page_size": 100}
+    )
+    return CONVERTER.structure(result, typing.List[Case])
 
 
 def case_retrieve(
     server_url: str,
     api_token: str,
     case_uuid: typing.Union[str, uuid.UUID],
     verify_ssl: bool = True,
```

### Comparing `varfish_cli-0.5.1/varfish_cli/api/models.py` & `varfish_cli-0.5.2/varfish_cli/api/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,18 @@
     index: str
     #: List of pedigree members.
     pedigree: typing.List[PedigreeMember]
     #: Number of small variants in case.
     num_small_vars: typing.Optional[int]
     #: Number of SVs in case.
     num_svs: typing.Optional[int]
+    #: Cusom User Notes
+    notes: typing.Optional[str] = None
+    #: Status of case. Can be either "active" "closed-<solved|unsolved>" or "initial"
+    status: typing.Optional[str] = None
 
 
 class CaseImportState(Enum):
     """Enumeration for the states."""
 
     #: Draft state, allows modification.
     DRAFT = "draft"
```

### Comparing `varfish_cli-0.5.1/varfish_cli/api/varannos.py` & `varfish_cli-0.5.2/varfish_cli/api/varannos.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/case/__init__.py` & `varfish_cli-0.5.2/varfish_cli/case/__init__.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/case/config.py` & `varfish_cli-0.5.2/varfish_cli/case/config.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/case/create_case_import.py` & `varfish_cli-0.5.2/varfish_cli/case/create_case_import.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/case/list_case.py` & `varfish_cli-0.5.2/varfish_cli/case/list_case.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/case/list_case_import.py` & `varfish_cli-0.5.2/varfish_cli/case/list_case_import.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/case/small_var_query_create.py` & `varfish_cli-0.5.2/varfish_cli/case/small_var_query_create.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/case/small_var_query_fetch_results.py` & `varfish_cli-0.5.2/varfish_cli/case/small_var_query_fetch_results.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/case/small_var_query_list.py` & `varfish_cli-0.5.2/varfish_cli/case/small_var_query_list.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/case/small_var_query_retrieve.py` & `varfish_cli-0.5.2/varfish_cli/case/small_var_query_retrieve.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/case/small_var_query_settings_shortcut.py` & `varfish_cli-0.5.2/varfish_cli/case/small_var_query_settings_shortcut.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/case/small_var_query_status.py` & `varfish_cli-0.5.2/varfish_cli/case/small_var_query_status.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/case/small_var_query_update.py` & `varfish_cli-0.5.2/varfish_cli/case/small_var_query_update.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/common.py` & `varfish_cli-0.5.2/varfish_cli/common.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/exceptions.py` & `varfish_cli-0.5.2/varfish_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/parse_ped.py` & `varfish_cli-0.5.2/varfish_cli/parse_ped.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/varannos/__init__.py` & `varfish_cli-0.5.2/varfish_cli/varannos/__init__.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/varannos/config.py` & `varfish_cli-0.5.2/varfish_cli/varannos/config.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/varannos/varannoset_destroy.py` & `varfish_cli-0.5.2/varfish_cli/varannos/varannoset_destroy.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/varannos/varannoset_list.py` & `varfish_cli-0.5.2/varfish_cli/varannos/varannoset_list.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/varannos/varannoset_retrieve.py` & `varfish_cli-0.5.2/varfish_cli/varannos/varannoset_retrieve.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/varannos/varannoset_update.py` & `varfish_cli-0.5.2/varfish_cli/varannos/varannoset_update.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/varannos/varannosetentry_destroy.py` & `varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_destroy.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/varannos/varannosetentry_list.py` & `varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_list.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/varannos/varannosetentry_retrieve.py` & `varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_retrieve.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli/varannos/varannosetentry_update.py` & `varfish_cli-0.5.2/varfish_cli/varannos/varannosetentry_update.py`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/varfish_cli.egg-info/PKG-INFO` & `varfish_cli-0.5.2/varfish_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varfish-cli
-Version: 0.5.1
+Version: 0.5.2
 Summary: Command line interface client for VarFish Server.
 Home-page: https://github.com/bihealth/varfish-cli
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bihealth.de
 License: MIT license
 Keywords: varfish_cli
 Classifier: Development Status :: 4 - Beta
@@ -86,14 +86,21 @@
 varfish_api_token = "XXX"
 EOF
 ```
 
 
 # Changelog
 
+### [0.5.2](https://www.github.com/bihealth/varfish-cli/compare/v0.5.1...v0.5.2) (2023-06-12)
+
+
+### Bug Fixes
+
+* Fixing case list API ([#37](https://www.github.com/bihealth/varfish-cli/issues/37)) ([ccaccfc](https://www.github.com/bihealth/varfish-cli/commit/ccaccfcbec7fb209492f1855b5e740f20ac60bbc))
+
 ### [0.5.1](https://www.github.com/bihealth/varfish-cli/compare/v0.5.0...v0.5.1) (2023-02-09)
 
 
 ### Bug Fixes
 
 * manifest for readme and changelog ([#35](https://www.github.com/bihealth/varfish-cli/issues/35)) ([f14d647](https://www.github.com/bihealth/varfish-cli/commit/f14d6472728995b9e18726fbfb7c36e86319c999))
```

### Comparing `varfish_cli-0.5.1/varfish_cli.egg-info/SOURCES.txt` & `varfish_cli-0.5.2/varfish_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `varfish_cli-0.5.1/versioneer.py` & `varfish_cli-0.5.2/versioneer.py`

 * *Files identical despite different names*

