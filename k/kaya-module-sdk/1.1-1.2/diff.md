# Comparing `tmp/kaya-module-sdk-1.1.tar.gz` & `tmp/kaya-module-sdk-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaya-module-sdk-1.1.tar", last modified: Sun Jun 11 22:02:44 2023, max compression
+gzip compressed data, was "kaya-module-sdk-1.2.tar", last modified: Sun Jun 11 23:31:26 2023, max compression
```

## Comparing `kaya-module-sdk-1.1.tar` & `kaya-module-sdk-1.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.362195 kaya-module-sdk-1.1/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)    11356 2023-06-11 20:49:29.000000 kaya-module-sdk-1.1/LICENSE
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     3390 2023-06-11 22:02:44.362032 kaya-module-sdk-1.1/PKG-INFO
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     2408 2023-05-30 22:52:01.000000 kaya-module-sdk-1.1/README.md
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.350229 kaya-module-sdk-1.1/kaya/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)       75 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/__init__.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.350594 kaya-module-sdk-1.1/kaya/kaya/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)       75 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/kaya/__init__.py
--rwxr-xr-x   0 cojocarudragos   (501) staff       (20)      595 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/sdk.py
--rwxr-xr-x   0 cojocarudragos   (501) staff       (20)     4209 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/setup.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.351185 kaya-module-sdk-1.1/kaya/src/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        1 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/__init__.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)      541 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/config.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.352843 kaya-module-sdk-1.1/kaya/src/data_types/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        1 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/data_types/__init__.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     5148 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/data_types/_k_number.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)      118 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/data_types/k_float.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)      151 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/data_types/k_int.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     3590 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/data_types/k_list.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)      491 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/data_types/k_string.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     1548 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/data_types/k_time_series.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.353533 kaya-module-sdk-1.1/kaya/src/module/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        1 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/module/__init__.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     1005 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/module/run.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     1602 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/module/template.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.354209 kaya-module-sdk-1.1/kaya/src/testing/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/testing/__init__.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     3526 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/testing/kit.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     1437 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/src/testing/run.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.354474 kaya-module-sdk-1.1/kaya/tst/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        1 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/tst/__init__.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.354971 kaya-module-sdk-1.1/kaya/tst/integration/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/tst/integration/__init__.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)      993 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/tst/integration/test_module.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.355888 kaya-module-sdk-1.1/kaya/tst/unit/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/tst/unit/__init__.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     1834 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/tst/unit/test_module.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)      553 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/tst/unit/test_sdk.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)    10935 2023-06-11 22:02:41.000000 kaya-module-sdk-1.1/kaya/tst/unit/test_types.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.357217 kaya-module-sdk-1.1/kaya_module_sdk.egg-info/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     3390 2023-06-11 22:02:44.000000 kaya-module-sdk-1.1/kaya_module_sdk.egg-info/PKG-INFO
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     1447 2023-06-11 22:02:44.000000 kaya-module-sdk-1.1/kaya_module_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        1 2023-06-11 22:02:44.000000 kaya-module-sdk-1.1/kaya_module_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 cojocarudragos   (501) staff       (20)       19 2023-06-11 22:02:44.000000 kaya-module-sdk-1.1/kaya_module_sdk.egg-info/requires.txt
--rw-r--r--   0 cojocarudragos   (501) staff       (20)       13 2023-06-11 22:02:44.000000 kaya-module-sdk-1.1/kaya_module_sdk.egg-info/top_level.txt
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        1 2023-06-11 22:02:44.000000 kaya-module-sdk-1.1/kaya_module_sdk.egg-info/zip-safe
--rw-r--r--   0 cojocarudragos   (501) staff       (20)       38 2023-06-11 22:02:44.362241 kaya-module-sdk-1.1/setup.cfg
--rwxr-xr-x   0 cojocarudragos   (501) staff       (20)     4209 2023-06-11 22:02:29.000000 kaya-module-sdk-1.1/setup.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.357613 kaya-module-sdk-1.1/src/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        1 2023-05-30 22:52:01.000000 kaya-module-sdk-1.1/src/__init__.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)      541 2023-06-06 01:28:55.000000 kaya-module-sdk-1.1/src/config.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.358978 kaya-module-sdk-1.1/src/data_types/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        1 2023-05-30 22:52:01.000000 kaya-module-sdk-1.1/src/data_types/__init__.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     5148 2023-05-30 22:52:01.000000 kaya-module-sdk-1.1/src/data_types/_k_number.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)      118 2023-05-30 22:52:01.000000 kaya-module-sdk-1.1/src/data_types/k_float.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)      151 2023-05-30 22:52:01.000000 kaya-module-sdk-1.1/src/data_types/k_int.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     3590 2023-05-30 22:52:01.000000 kaya-module-sdk-1.1/src/data_types/k_list.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)      491 2023-05-30 22:52:01.000000 kaya-module-sdk-1.1/src/data_types/k_string.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     1548 2023-05-30 22:52:01.000000 kaya-module-sdk-1.1/src/data_types/k_time_series.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.359655 kaya-module-sdk-1.1/src/module/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        1 2023-05-30 22:52:01.000000 kaya-module-sdk-1.1/src/module/__init__.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     1005 2023-03-16 00:09:23.000000 kaya-module-sdk-1.1/src/module/run.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     1602 2023-06-11 20:26:26.000000 kaya-module-sdk-1.1/src/module/template.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.360300 kaya-module-sdk-1.1/src/testing/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 20:26:26.000000 kaya-module-sdk-1.1/src/testing/__init__.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     3526 2023-06-11 20:26:26.000000 kaya-module-sdk-1.1/src/testing/kit.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     1437 2023-06-11 20:26:26.000000 kaya-module-sdk-1.1/src/testing/run.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.360527 kaya-module-sdk-1.1/tst/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        1 2023-05-30 22:52:01.000000 kaya-module-sdk-1.1/tst/__init__.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.360926 kaya-module-sdk-1.1/tst/integration/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 20:26:26.000000 kaya-module-sdk-1.1/tst/integration/__init__.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)      993 2023-06-11 20:26:26.000000 kaya-module-sdk-1.1/tst/integration/test_module.py
-drwxr-xr-x   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 22:02:44.361744 kaya-module-sdk-1.1/tst/unit/
--rw-r--r--   0 cojocarudragos   (501) staff       (20)        0 2023-06-11 20:26:26.000000 kaya-module-sdk-1.1/tst/unit/__init__.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)     1834 2023-06-11 20:26:26.000000 kaya-module-sdk-1.1/tst/unit/test_module.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)      553 2023-06-11 20:26:26.000000 kaya-module-sdk-1.1/tst/unit/test_sdk.py
--rw-r--r--   0 cojocarudragos   (501) staff       (20)    10935 2023-06-11 20:26:26.000000 kaya-module-sdk-1.1/tst/unit/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/kaya-module-sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/kaya-module-sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4209 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/_k_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_time_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/src/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/module/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/module/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/testing/kit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/testing/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/tst/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/tst/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/integration/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-11 23:31:26.000000 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-11 23:31:26.000000 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:31:26.000000 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-11 23:31:26.000000 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-11 23:31:26.000000 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:31:26.000000 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4209 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/src/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/_k_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/k_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/k_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/k_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/k_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/k_time_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/src/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/module/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/module/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/testing/kit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/testing/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/tst/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/tst/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/integration/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/tst/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/unit/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/unit/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/unit/test_types.py
```

### Comparing `kaya-module-sdk-1.1/LICENSE` & `kaya-module-sdk-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/PKG-INFO` & `kaya-module-sdk-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaya-module-sdk
-Version: 1.1
+Version: 1.2
 Summary: Provides the user a way to create custom strategy modules.
 Home-page: https://kaya.wanolabs.com
 Download-URL: http://pypi.python.org/pypi/kaya-module-sdk
 Author: Del:Tango
 Author-email: alvearesolutions@gmail.com
 License: BSD
 Project-URL: Documentation, https://kaya.wanolabs.com.readthedocs.io/en/latest
```

### Comparing `kaya-module-sdk-1.1/README.md` & `kaya-module-sdk-1.2/README.md`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya/sdk.py` & `kaya-module-sdk-1.2/kaya-module-sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya/setup.py` & `kaya-module-sdk-1.2/kaya-module-sdk/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 # TODO - Check type hints used or break compilation
 #MyPyCommand().run()
 
 add_package_dir_to_path()
 setup_info = dict(
     name='kaya-module-sdk',
-    version='1.1',
+    version='1.2',
     author='Del:Tango',
     author_email='alvearesolutions@gmail.com',
     url='https://kaya.wanolabs.com',
     download_url='http://pypi.python.org/pypi/kaya-module-sdk',
     project_urls={
         'Documentation': 'https://kaya.wanolabs.com.readthedocs.io/en/latest',
         'Source': 'https://github.com/WanoLabs/KayaModuleSDK',
```

### Comparing `kaya-module-sdk-1.1/kaya/src/config.py` & `kaya-module-sdk-1.2/kaya-module-sdk/src/config.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya/src/data_types/_k_number.py` & `kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/_k_number.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya/src/data_types/k_list.py` & `kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_list.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya/src/data_types/k_time_series.py` & `kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_time_series.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya/src/module/run.py` & `kaya-module-sdk-1.2/kaya-module-sdk/src/module/run.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya/src/module/template.py` & `kaya-module-sdk-1.2/kaya-module-sdk/src/module/template.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya/src/testing/kit.py` & `kaya-module-sdk-1.2/kaya-module-sdk/src/testing/kit.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya/src/testing/run.py` & `kaya-module-sdk-1.2/kaya-module-sdk/src/testing/run.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya/tst/integration/test_module.py` & `kaya-module-sdk-1.2/kaya-module-sdk/tst/integration/test_module.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya/tst/unit/test_module.py` & `kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/test_module.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya/tst/unit/test_sdk.py` & `kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/test_sdk.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya/tst/unit/test_types.py` & `kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/test_types.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/kaya_module_sdk.egg-info/PKG-INFO` & `kaya-module-sdk-1.2/kaya_module_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaya-module-sdk
-Version: 1.1
+Version: 1.2
 Summary: Provides the user a way to create custom strategy modules.
 Home-page: https://kaya.wanolabs.com
 Download-URL: http://pypi.python.org/pypi/kaya-module-sdk
 Author: Del:Tango
 Author-email: alvearesolutions@gmail.com
 License: BSD
 Project-URL: Documentation, https://kaya.wanolabs.com.readthedocs.io/en/latest
```

### Comparing `kaya-module-sdk-1.1/setup.py` & `kaya-module-sdk-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 # TODO - Check type hints used or break compilation
 #MyPyCommand().run()
 
 add_package_dir_to_path()
 setup_info = dict(
     name='kaya-module-sdk',
-    version='1.1',
+    version='1.2',
     author='Del:Tango',
     author_email='alvearesolutions@gmail.com',
     url='https://kaya.wanolabs.com',
     download_url='http://pypi.python.org/pypi/kaya-module-sdk',
     project_urls={
         'Documentation': 'https://kaya.wanolabs.com.readthedocs.io/en/latest',
         'Source': 'https://github.com/WanoLabs/KayaModuleSDK',
```

### Comparing `kaya-module-sdk-1.1/src/config.py` & `kaya-module-sdk-1.2/src/config.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/src/data_types/_k_number.py` & `kaya-module-sdk-1.2/src/data_types/_k_number.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/src/data_types/k_list.py` & `kaya-module-sdk-1.2/src/data_types/k_list.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/src/data_types/k_time_series.py` & `kaya-module-sdk-1.2/src/data_types/k_time_series.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/src/module/run.py` & `kaya-module-sdk-1.2/src/module/run.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/src/module/template.py` & `kaya-module-sdk-1.2/src/module/template.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/src/testing/kit.py` & `kaya-module-sdk-1.2/src/testing/kit.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/src/testing/run.py` & `kaya-module-sdk-1.2/src/testing/run.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/tst/integration/test_module.py` & `kaya-module-sdk-1.2/tst/integration/test_module.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/tst/unit/test_module.py` & `kaya-module-sdk-1.2/tst/unit/test_module.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/tst/unit/test_sdk.py` & `kaya-module-sdk-1.2/tst/unit/test_sdk.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.1/tst/unit/test_types.py` & `kaya-module-sdk-1.2/tst/unit/test_types.py`

 * *Files identical despite different names*

