# Comparing `tmp/pyatlan-0.1.0.tar.gz` & `tmp/pyatlan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.1.0.tar", last modified: Tue Jun  6 15:55:49 2023, max compression
+gzip compressed data, was "pyatlan-0.1.1.tar", last modified: Mon Jun 12 11:46:00 2023, max compression
```

## Comparing `pyatlan-0.1.0.tar` & `pyatlan-0.1.1.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.585760 pyatlan-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-06 15:55:33.000000 pyatlan-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-06 15:55:33.000000 pyatlan-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-06 15:55:33.000000 pyatlan-0.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-06 15:55:49.585760 pyatlan-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-06 15:55:33.000000 pyatlan-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.573760 pyatlan-0.1.0/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.577760 pyatlan-0.1.0/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.577760 pyatlan-0.1.0/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40989 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.577760 pyatlan-0.1.0/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.577760 pyatlan-0.1.0/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.581760 pyatlan-0.1.0/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   852385 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24335 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 15:55:33.000000 pyatlan-0.1.0/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.577760 pyatlan-0.1.0/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-06 15:55:49.000000 pyatlan-0.1.0/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-06 15:55:49.000000 pyatlan-0.1.0/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:55:49.000000 pyatlan-0.1.0/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:55:49.000000 pyatlan-0.1.0/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-06 15:55:49.000000 pyatlan-0.1.0/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 15:55:49.000000 pyatlan-0.1.0/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:55:49.585760 pyatlan-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-06 15:55:33.000000 pyatlan-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.581760 pyatlan-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.585760 pyatlan-0.1.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    38214 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23633 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34056 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/test_entity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/integration/test_index_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:55:49.585760 pyatlan-0.1.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    66551 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31770 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-06 15:55:33.000000 pyatlan-0.1.0/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.166763 pyatlan-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-12 11:45:48.000000 pyatlan-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 11:45:48.000000 pyatlan-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-12 11:45:48.000000 pyatlan-0.1.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-12 11:46:00.166763 pyatlan-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-12 11:45:48.000000 pyatlan-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.158763 pyatlan-0.1.1/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.158763 pyatlan-0.1.1/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.158763 pyatlan-0.1.1/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42383 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.158763 pyatlan-0.1.1/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.158763 pyatlan-0.1.1/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.162763 pyatlan-0.1.1/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   899802 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54041 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 11:45:48.000000 pyatlan-0.1.1/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.158763 pyatlan-0.1.1/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-12 11:46:00.000000 pyatlan-0.1.1/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-12 11:46:00.000000 pyatlan-0.1.1/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 11:46:00.000000 pyatlan-0.1.1/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 11:45:59.000000 pyatlan-0.1.1/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 11:46:00.000000 pyatlan-0.1.1/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 11:46:00.000000 pyatlan-0.1.1/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 11:46:00.166763 pyatlan-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-12 11:45:48.000000 pyatlan-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.162763 pyatlan-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.162763 pyatlan-0.1.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35609 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/integration/test_sql_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:00.166763 pyatlan-0.1.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64432 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31770 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-12 11:45:48.000000 pyatlan-0.1.1/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.1.0/LICENSE` & `pyatlan-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/PKG-INFO` & `pyatlan-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.1.0
+Version: 0.1.1
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.1.0/README.md` & `pyatlan-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/cache/classification_cache.py` & `pyatlan-0.1.1/pyatlan/cache/classification_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.1.1/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/cache/enum_cache.py` & `pyatlan-0.1.1/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/cache/group_cache.py` & `pyatlan-0.1.1/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/cache/role_cache.py` & `pyatlan-0.1.1/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/cache/user_cache.py` & `pyatlan-0.1.1/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/client/atlan.py` & `pyatlan-0.1.1/pyatlan/client/atlan.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import ClassVar, Generator, Optional, Type, TypeVar, Union
 
 import requests
 from pydantic import (
     BaseSettings,
     HttpUrl,
     PrivateAttr,
+    ValidationError,
     parse_obj_as,
     validate_arguments,
 )
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from pyatlan.client.constants import (
@@ -47,14 +48,15 @@
     PARSE_QUERY,
     PARTIAL_UPDATE_ENTITY_BY_ATTRIBUTE,
     REMOVE_USERS_FROM_GROUP,
     UPDATE_ENTITY_BY_ATTRIBUTE,
     UPDATE_GROUP,
     UPDATE_TYPE_DEFS,
     UPDATE_USER,
+    UPLOAD_IMAGE,
 )
 from pyatlan.error import AtlanError, NotFoundError
 from pyatlan.exceptions import AtlanServiceException, InvalidRequestException
 from pyatlan.model.assets import (
     Asset,
     AtlasGlossary,
     AtlasGlossaryCategory,
@@ -63,14 +65,15 @@
     Database,
     MaterialisedView,
     Referenceable,
     Schema,
     Table,
     View,
 )
+from pyatlan.model.atlan_image import AtlanImage
 from pyatlan.model.core import (
     Announcement,
     AssetRequest,
     AssetResponse,
     AtlanObject,
     BulkRequest,
     Classification,
@@ -113,14 +116,15 @@
     AddToGroupsRequest,
     AtlanUser,
     ChangeRoleRequest,
     CreateUserRequest,
     UserMinimalResponse,
     UserResponse,
 )
+from pyatlan.multipart_data_generator import MultipartDataGenerator
 from pyatlan.utils import HTTPStatus, get_logger
 
 LOGGER = get_logger()
 T = TypeVar("T", bound=Referenceable)
 A = TypeVar("A", bound=Asset)
 Assets = Union[
     AtlasGlossary,
@@ -189,15 +193,15 @@
             struct_defs=[],
             entity_defs=[],
             relationship_defs=[],
             custom_metadata_defs=[],
         )
     else:
         raise InvalidRequestException(
-            "Unable to update type definitions of category: " + typedef.category.value,
+            f"Unable to update type definitions of category: {typedef.category.value}",
             param="category",
         )
         # Throw an invalid request exception
     return payload
 
 
 def _refresh_caches(typedef: TypeDef) -> None:
@@ -277,25 +281,30 @@
             raise ValueError("client must be an instance of AtlanClient")
         cls._default_client = client
 
     @classmethod
     def get_default_client(cls) -> "Optional[AtlanClient]":
         return cls._default_client
 
+    @classmethod
+    def reset_default_client(cls):
+        """Sets the default_client to None"""
+        cls._default_client = None
+
     def __init__(self, **data):
         super().__init__(**data)
         self._request_params = {"headers": {"authorization": f"Bearer {self.api_key}"}}
 
-    def _call_api(
-        self, api, query_params=None, request_obj=None, exclude_unset: bool = True
-    ):
-        params, path = self._create_params(
-            api, query_params, request_obj, exclude_unset
-        )
-        response = self._session.request(api.method.value, path, **params)
+    def _call_api_internal(self, api, path, params, binary_data=None):
+        if binary_data:
+            response = self._session.request(
+                api.method.value, path, data=binary_data, **params
+            )
+        else:
+            response = self._session.request(api.method.value, path, **params)
         if response is not None:
             LOGGER.debug("HTTP Status: %s", response.status_code)
         if response is None:
             return None
         if response.status_code == api.expected_status:
             try:
                 if (
@@ -303,18 +312,17 @@
                     or response.content == "null"
                     or len(response.content) == 0
                     or response.status_code == HTTPStatus.NO_CONTENT
                 ):
                     return None
                 if LOGGER.isEnabledFor(logging.DEBUG):
                     LOGGER.debug(
-                        "<== __call_api(%s,%s,%s), result = %s",
+                        "<== __call_api(%s,%s), result = %s",
                         vars(api),
                         params,
-                        request_obj,
                         response,
                     )
                     LOGGER.debug(response.json())
                 return response.json()
             except Exception as e:
                 print(e)
                 LOGGER.exception(
@@ -337,14 +345,32 @@
                     raise AtlanError(
                         message=error_message,
                         code=error_code,
                         status_code=response.status_code,
                     )
             raise AtlanServiceException(api, response)
 
+    def _call_api(
+        self, api, query_params=None, request_obj=None, exclude_unset: bool = True
+    ):
+        params, path = self._create_params(
+            api, query_params, request_obj, exclude_unset
+        )
+        return self._call_api_internal(api, path, params)
+
+    def _upload_file(self, api, file=None, filename=None):
+        generator = MultipartDataGenerator()
+        generator.add_file(file=file, filename=filename)
+        post_data = generator.get_post_data()
+        api.produces = f"multipart/form-data; boundary={generator.boundary}"
+        params, path = self._create_params(
+            api, query_params=None, request_obj=None, exclude_unset=True
+        )
+        return self._call_api_internal(api, path, params, binary_data=post_data)
+
     def _create_params(
         self, api, query_params, request_obj, exclude_unset: bool = True
     ):
         params = copy.deepcopy(self._request_params)
         path = os.path.join(self.base_url, api.path)
         params["headers"]["Accept"] = api.consumes
         params["headers"]["content-type"] = api.produces
@@ -360,14 +386,18 @@
         if LOGGER.isEnabledFor(logging.DEBUG):
             LOGGER.debug("------------------------------------------------------")
             LOGGER.debug("Call         : %s %s", api.method, path)
             LOGGER.debug("Content-type_ : %s", api.consumes)
             LOGGER.debug("Accept       : %s", api.produces)
         return params, path
 
+    def upload_image(self, file, filename: str) -> AtlanImage:
+        raw_json = self._upload_file(UPLOAD_IMAGE, file=file, filename=filename)
+        return AtlanImage(**raw_json)
+
     def get_roles(
         self,
         limit: int,
         post_filter: Optional[str] = None,
         sort: Optional[str] = None,
         count: bool = True,
         offset: int = 0,
@@ -816,15 +846,19 @@
 
     def search(self, criteria: IndexSearchRequest) -> SearchResults:
         raw_json = self._call_api(
             INDEX_SEARCH,
             request_obj=criteria,
         )
         if "entities" in raw_json:
-            assets = parse_obj_as(list[Asset], raw_json["entities"])
+            try:
+                assets = parse_obj_as(list[Asset], raw_json["entities"])
+            except ValidationError as err:
+                LOGGER.error("Problem parsing JSON: %s", raw_json["entities"])
+                raise err
         else:
             assets = []
         count = raw_json["approximateCount"] if "approximateCount" in raw_json else 0
         return AtlanClient.SearchResults(
             client=self,
             criteria=criteria,
             start=criteria.dsl.from_,
```

### Comparing `pyatlan-0.1.0/pyatlan/client/constants.py` & `pyatlan-0.1.1/pyatlan/client/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     HTTPStatus,
 )
 
 ROLE_API = f"{ADMIN_URI}roles"
 GROUP_API = f"{ADMIN_URI}groups"
 USER_API = f"{ADMIN_URI}users"
 QUERY_API = f"{SQL_URI}query"
+IMAGE_API = f"{ADMIN_URI}images"
 
 # Role APIs
 GET_ROLES = API(ROLE_API, HTTPMethod.GET, HTTPStatus.OK)
 
 # Group APIs
 GET_GROUPS = API(GROUP_API, HTTPMethod.GET, HTTPStatus.OK)
 CREATE_GROUP = API(GROUP_API, HTTPMethod.POST, HTTPStatus.OK)
@@ -46,14 +47,17 @@
     USER_API + "/{user_guid}/roles/update", HTTPMethod.POST, HTTPStatus.OK
 )
 GET_CURRENT_USER = API(f"{USER_API}/current", HTTPMethod.GET, HTTPStatus.OK)
 
 # SQL parsing APIs
 PARSE_QUERY = API(f"{QUERY_API}/parse", HTTPMethod.POST, HTTPStatus.OK)
 
+# File upload APIs
+UPLOAD_IMAGE = API(IMAGE_API, HTTPMethod.POST, HTTPStatus.OK)
+
 ENTITY_API = f"{BASE_URI}entity/"
 PREFIX_ATTR = "attr:"
 PREFIX_ATTR_ = "attr_"
 ADMIN_API = f"{BASE_URI}admin/"
 ENTITY_PURGE_API = f"{ADMIN_API}purge/"
 ENTITY_BULK_API = f"{ENTITY_API}bulk/"
 BULK_SET_CLASSIFICATIONS = "bulk/setClassifications"
```

### Comparing `pyatlan-0.1.0/pyatlan/error.py` & `pyatlan-0.1.1/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/exceptions.py` & `pyatlan-0.1.1/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.1.1/pyatlan/generator/generate_from_typdefs.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
         >= datetime.date.today()
     ):
         with TYPE_DEF_FILE.open() as input_file:
             return TypeDefResponse(**json.load(input_file))
     else:
         client = AtlanClient()
         type_defs = client.get_all_typedefs()
+        if len(type_defs.entity_defs) == 0:
+            raise Exception("No entity definitions were returned.")
         with TYPE_DEF_FILE.open("w") as output_file:
             output_file.write(type_defs.json())
         return type_defs
 
 
 class Generator:
     def __init__(self) -> None:
```

### Comparing `pyatlan-0.1.0/pyatlan/model/assets.py` & `pyatlan-0.1.1/pyatlan/model/assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -323,14 +323,15 @@
         "admin_roles",
         "source_read_count",
         "source_read_user_count",
         "source_last_read_at",
         "last_row_changed_at",
         "source_total_cost",
         "source_cost_unit",
+        "source_read_query_cost",
         "source_read_recent_user_list",
         "source_read_recent_user_record_list",
         "source_read_top_user_list",
         "source_read_top_user_record_list",
         "source_read_popular_query_record_list",
         "source_read_expensive_query_record_list",
         "source_read_slow_query_record_list",
@@ -856,14 +857,24 @@
     @source_cost_unit.setter
     def source_cost_unit(self, source_cost_unit: Optional[SourceCostUnitType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_cost_unit = source_cost_unit
 
     @property
+    def source_read_query_cost(self) -> Optional[float]:
+        return self.attributes.source_read_query_cost
+
+    @source_read_query_cost.setter
+    def source_read_query_cost(self, source_read_query_cost: Optional[float]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.source_read_query_cost = source_read_query_cost
+
+    @property
     def source_read_recent_user_list(self) -> Optional[set[str]]:
         return self.attributes.source_read_recent_user_list
 
     @source_read_recent_user_list.setter
     def source_read_recent_user_list(
         self, source_read_recent_user_list: Optional[set[str]]
     ):
@@ -1886,14 +1897,17 @@
         )
         source_total_cost: Optional[float] = Field(
             None, description="", alias="sourceTotalCost"
         )
         source_cost_unit: Optional[SourceCostUnitType] = Field(
             None, description="", alias="sourceCostUnit"
         )
+        source_read_query_cost: Optional[float] = Field(
+            None, description="", alias="sourceReadQueryCost"
+        )
         source_read_recent_user_list: Optional[set[str]] = Field(
             None, description="", alias="sourceReadRecentUserList"
         )
         source_read_recent_user_record_list: Optional[list[PopularityInsights]] = Field(
             None, description="", alias="sourceReadRecentUserRecordList"
         )
         source_read_top_user_list: Optional[set[str]] = Field(
@@ -2504,28 +2518,14 @@
         connection_dbt_environments: Optional[set[str]] = Field(
             None, description="", alias="connectionDbtEnvironments"
         )
         connection_s_s_o_credential_guid: Optional[str] = Field(
             None, description="", alias="connectionSSOCredentialGuid"
         )
 
-        def validate_required(self):
-            if not self.name:
-                raise ValueError("name is required")
-            if not self.admin_roles and not self.admin_groups and not self.admin_users:
-                raise ValueError(
-                    "One of admin_user, admin_groups or admin_roles is required"
-                )
-            if not self.qualified_name:
-                raise ValueError("qualified_name is required")
-            if not self.category:
-                raise ValueError("category is required")
-            if not self.connector_name:
-                raise ValueError("connector_name is required")
-
     attributes: "Connection.Attributes" = Field(
         default_factory=lambda: Connection.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
     @classmethod
@@ -3720,16 +3720,16 @@
         "replacement_terms",
         "see_also",
         "translated_terms",
         "is_a",
         "anchor",
         "antonyms",
         "assigned_entities",
-        "categories",
         "classifies",
+        "categories",
         "preferred_to_terms",
         "preferred_terms",
     ]
 
     @property
     def short_description(self) -> Optional[str]:
         return self.attributes.short_description
@@ -3907,34 +3907,34 @@
     @assigned_entities.setter
     def assigned_entities(self, assigned_entities: Optional[list[Referenceable]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.assigned_entities = assigned_entities
 
     @property
-    def categories(self) -> Optional[list[AtlasGlossaryCategory]]:
-        return self.attributes.categories
-
-    @categories.setter
-    def categories(self, categories: Optional[list[AtlasGlossaryCategory]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.categories = categories
-
-    @property
     def classifies(self) -> Optional[list[AtlasGlossaryTerm]]:
         return self.attributes.classifies
 
     @classifies.setter
     def classifies(self, classifies: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.classifies = classifies
 
     @property
+    def categories(self) -> Optional[list[AtlasGlossaryCategory]]:
+        return self.attributes.categories
+
+    @categories.setter
+    def categories(self, categories: Optional[list[AtlasGlossaryCategory]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.categories = categories
+
+    @property
     def preferred_to_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
         return self.attributes.preferred_to_terms
 
     @preferred_to_terms.setter
     def preferred_to_terms(self, preferred_to_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -4003,20 +4003,20 @@
         )  # relationship
         antonyms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="antonyms"
         )  # relationship
         assigned_entities: Optional[list[Referenceable]] = Field(
             None, description="", alias="assignedEntities"
         )  # relationship
-        categories: Optional[list[AtlasGlossaryCategory]] = Field(
-            None, description="", alias="categories"
-        )  # relationship
         classifies: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="classifies"
         )  # relationship
+        categories: Optional[list[AtlasGlossaryCategory]] = Field(
+            None, description="", alias="categories"
+        )  # relationship
         preferred_to_terms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="preferredToTerms"
         )  # relationship
         preferred_terms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="preferredTerms"
         )  # relationship
 
@@ -6452,30 +6452,28 @@
     attributes: "S3.Attributes" = Field(
         default_factory=lambda: S3.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class ADLS(Azure):
+class ADLS(ObjectStore):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ADLS._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "adls_account_qualified_name",
         "azure_resource_id",
         "azure_location",
         "adls_account_secondary_location",
         "azure_tags",
-        "input_to_processes",
-        "output_from_processes",
     ]
 
     @property
     def adls_account_qualified_name(self) -> Optional[str]:
         return self.attributes.adls_account_qualified_name
 
     @adls_account_qualified_name.setter
@@ -6524,43 +6522,23 @@
 
     @azure_tags.setter
     def azure_tags(self, azure_tags: Optional[list[AzureTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_tags = azure_tags
 
-    @property
-    def input_to_processes(self) -> Optional[list[Process]]:
-        return self.attributes.input_to_processes
-
-    @input_to_processes.setter
-    def input_to_processes(self, input_to_processes: Optional[list[Process]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.input_to_processes = input_to_processes
-
-    @property
-    def output_from_processes(self) -> Optional[list[Process]]:
-        return self.attributes.output_from_processes
-
-    @output_from_processes.setter
-    def output_from_processes(self, output_from_processes: Optional[list[Process]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.output_from_processes = output_from_processes
-
     type_name: str = Field("ADLS", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ADLS":
             raise ValueError("must be ADLS")
         return v
 
-    class Attributes(Azure.Attributes):
+    class Attributes(ObjectStore.Attributes):
         adls_account_qualified_name: Optional[str] = Field(
             None, description="", alias="adlsAccountQualifiedName"
         )
         azure_resource_id: Optional[str] = Field(
             None, description="", alias="azureResourceId"
         )
         azure_location: Optional[str] = Field(
@@ -6568,20 +6546,14 @@
         )
         adls_account_secondary_location: Optional[str] = Field(
             None, description="", alias="adlsAccountSecondaryLocation"
         )
         azure_tags: Optional[list[AzureTag]] = Field(
             None, description="", alias="azureTags"
         )
-        input_to_processes: Optional[list[Process]] = Field(
-            None, description="", alias="inputToProcesses"
-        )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
 
     attributes: "ADLS.Attributes" = Field(
         default_factory=lambda: ADLS.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
@@ -7010,14 +6982,456 @@
     attributes: "Metric.Attributes" = Field(
         default_factory=lambda: Metric.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class Preset(BI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Preset._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "preset_workspace_id",
+        "preset_workspace_qualified_name",
+        "preset_dashboard_id",
+        "preset_dashboard_qualified_name",
+    ]
+
+    @property
+    def preset_workspace_id(self) -> Optional[int]:
+        return self.attributes.preset_workspace_id
+
+    @preset_workspace_id.setter
+    def preset_workspace_id(self, preset_workspace_id: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.preset_workspace_id = preset_workspace_id
+
+    @property
+    def preset_workspace_qualified_name(self) -> Optional[str]:
+        return self.attributes.preset_workspace_qualified_name
+
+    @preset_workspace_qualified_name.setter
+    def preset_workspace_qualified_name(
+        self, preset_workspace_qualified_name: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.preset_workspace_qualified_name = (
+            preset_workspace_qualified_name
+        )
+
+    @property
+    def preset_dashboard_id(self) -> Optional[int]:
+        return self.attributes.preset_dashboard_id
+
+    @preset_dashboard_id.setter
+    def preset_dashboard_id(self, preset_dashboard_id: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.preset_dashboard_id = preset_dashboard_id
+
+    @property
+    def preset_dashboard_qualified_name(self) -> Optional[str]:
+        return self.attributes.preset_dashboard_qualified_name
+
+    @preset_dashboard_qualified_name.setter
+    def preset_dashboard_qualified_name(
+        self, preset_dashboard_qualified_name: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.preset_dashboard_qualified_name = (
+            preset_dashboard_qualified_name
+        )
+
+    type_name: str = Field("Preset", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Preset":
+            raise ValueError("must be Preset")
+        return v
+
+    class Attributes(BI.Attributes):
+        preset_workspace_id: Optional[int] = Field(
+            None, description="", alias="presetWorkspaceId"
+        )
+        preset_workspace_qualified_name: Optional[str] = Field(
+            None, description="", alias="presetWorkspaceQualifiedName"
+        )
+        preset_dashboard_id: Optional[int] = Field(
+            None, description="", alias="presetDashboardId"
+        )
+        preset_dashboard_qualified_name: Optional[str] = Field(
+            None, description="", alias="presetDashboardQualifiedName"
+        )
+
+    attributes: "Preset.Attributes" = Field(
+        default_factory=lambda: Preset.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class Mode(BI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Mode._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "mode_id",
+        "mode_token",
+        "mode_workspace_name",
+        "mode_workspace_username",
+        "mode_workspace_qualified_name",
+        "mode_report_name",
+        "mode_report_qualified_name",
+        "mode_query_name",
+        "mode_query_qualified_name",
+    ]
+
+    @property
+    def mode_id(self) -> Optional[str]:
+        return self.attributes.mode_id
+
+    @mode_id.setter
+    def mode_id(self, mode_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_id = mode_id
+
+    @property
+    def mode_token(self) -> Optional[str]:
+        return self.attributes.mode_token
+
+    @mode_token.setter
+    def mode_token(self, mode_token: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_token = mode_token
+
+    @property
+    def mode_workspace_name(self) -> Optional[str]:
+        return self.attributes.mode_workspace_name
+
+    @mode_workspace_name.setter
+    def mode_workspace_name(self, mode_workspace_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_workspace_name = mode_workspace_name
+
+    @property
+    def mode_workspace_username(self) -> Optional[str]:
+        return self.attributes.mode_workspace_username
+
+    @mode_workspace_username.setter
+    def mode_workspace_username(self, mode_workspace_username: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_workspace_username = mode_workspace_username
+
+    @property
+    def mode_workspace_qualified_name(self) -> Optional[str]:
+        return self.attributes.mode_workspace_qualified_name
+
+    @mode_workspace_qualified_name.setter
+    def mode_workspace_qualified_name(
+        self, mode_workspace_qualified_name: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_workspace_qualified_name = mode_workspace_qualified_name
+
+    @property
+    def mode_report_name(self) -> Optional[str]:
+        return self.attributes.mode_report_name
+
+    @mode_report_name.setter
+    def mode_report_name(self, mode_report_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_report_name = mode_report_name
+
+    @property
+    def mode_report_qualified_name(self) -> Optional[str]:
+        return self.attributes.mode_report_qualified_name
+
+    @mode_report_qualified_name.setter
+    def mode_report_qualified_name(self, mode_report_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_report_qualified_name = mode_report_qualified_name
+
+    @property
+    def mode_query_name(self) -> Optional[str]:
+        return self.attributes.mode_query_name
+
+    @mode_query_name.setter
+    def mode_query_name(self, mode_query_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_query_name = mode_query_name
+
+    @property
+    def mode_query_qualified_name(self) -> Optional[str]:
+        return self.attributes.mode_query_qualified_name
+
+    @mode_query_qualified_name.setter
+    def mode_query_qualified_name(self, mode_query_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mode_query_qualified_name = mode_query_qualified_name
+
+    type_name: str = Field("Mode", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Mode":
+            raise ValueError("must be Mode")
+        return v
+
+    class Attributes(BI.Attributes):
+        mode_id: Optional[str] = Field(None, description="", alias="modeId")
+        mode_token: Optional[str] = Field(None, description="", alias="modeToken")
+        mode_workspace_name: Optional[str] = Field(
+            None, description="", alias="modeWorkspaceName"
+        )
+        mode_workspace_username: Optional[str] = Field(
+            None, description="", alias="modeWorkspaceUsername"
+        )
+        mode_workspace_qualified_name: Optional[str] = Field(
+            None, description="", alias="modeWorkspaceQualifiedName"
+        )
+        mode_report_name: Optional[str] = Field(
+            None, description="", alias="modeReportName"
+        )
+        mode_report_qualified_name: Optional[str] = Field(
+            None, description="", alias="modeReportQualifiedName"
+        )
+        mode_query_name: Optional[str] = Field(
+            None, description="", alias="modeQueryName"
+        )
+        mode_query_qualified_name: Optional[str] = Field(
+            None, description="", alias="modeQueryQualifiedName"
+        )
+
+    attributes: "Mode.Attributes" = Field(
+        default_factory=lambda: Mode.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class Sigma(BI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Sigma._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "sigma_workbook_qualified_name",
+        "sigma_workbook_name",
+        "sigma_page_qualified_name",
+        "sigma_page_name",
+        "sigma_data_element_qualified_name",
+        "sigma_data_element_name",
+    ]
+
+    @property
+    def sigma_workbook_qualified_name(self) -> Optional[str]:
+        return self.attributes.sigma_workbook_qualified_name
+
+    @sigma_workbook_qualified_name.setter
+    def sigma_workbook_qualified_name(
+        self, sigma_workbook_qualified_name: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_workbook_qualified_name = sigma_workbook_qualified_name
+
+    @property
+    def sigma_workbook_name(self) -> Optional[str]:
+        return self.attributes.sigma_workbook_name
+
+    @sigma_workbook_name.setter
+    def sigma_workbook_name(self, sigma_workbook_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_workbook_name = sigma_workbook_name
+
+    @property
+    def sigma_page_qualified_name(self) -> Optional[str]:
+        return self.attributes.sigma_page_qualified_name
+
+    @sigma_page_qualified_name.setter
+    def sigma_page_qualified_name(self, sigma_page_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_page_qualified_name = sigma_page_qualified_name
+
+    @property
+    def sigma_page_name(self) -> Optional[str]:
+        return self.attributes.sigma_page_name
+
+    @sigma_page_name.setter
+    def sigma_page_name(self, sigma_page_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_page_name = sigma_page_name
+
+    @property
+    def sigma_data_element_qualified_name(self) -> Optional[str]:
+        return self.attributes.sigma_data_element_qualified_name
+
+    @sigma_data_element_qualified_name.setter
+    def sigma_data_element_qualified_name(
+        self, sigma_data_element_qualified_name: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_data_element_qualified_name = (
+            sigma_data_element_qualified_name
+        )
+
+    @property
+    def sigma_data_element_name(self) -> Optional[str]:
+        return self.attributes.sigma_data_element_name
+
+    @sigma_data_element_name.setter
+    def sigma_data_element_name(self, sigma_data_element_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_data_element_name = sigma_data_element_name
+
+    type_name: str = Field("Sigma", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Sigma":
+            raise ValueError("must be Sigma")
+        return v
+
+    class Attributes(BI.Attributes):
+        sigma_workbook_qualified_name: Optional[str] = Field(
+            None, description="", alias="sigmaWorkbookQualifiedName"
+        )
+        sigma_workbook_name: Optional[str] = Field(
+            None, description="", alias="sigmaWorkbookName"
+        )
+        sigma_page_qualified_name: Optional[str] = Field(
+            None, description="", alias="sigmaPageQualifiedName"
+        )
+        sigma_page_name: Optional[str] = Field(
+            None, description="", alias="sigmaPageName"
+        )
+        sigma_data_element_qualified_name: Optional[str] = Field(
+            None, description="", alias="sigmaDataElementQualifiedName"
+        )
+        sigma_data_element_name: Optional[str] = Field(
+            None, description="", alias="sigmaDataElementName"
+        )
+
+    attributes: "Sigma.Attributes" = Field(
+        default_factory=lambda: Sigma.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class Tableau(BI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Tableau._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
+    type_name: str = Field("Tableau", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Tableau":
+            raise ValueError("must be Tableau")
+        return v
+
+
+class Looker(BI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Looker._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
+    type_name: str = Field("Looker", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Looker":
+            raise ValueError("must be Looker")
+        return v
+
+
+class Redash(BI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Redash._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "redash_is_published",
+    ]
+
+    @property
+    def redash_is_published(self) -> Optional[bool]:
+        return self.attributes.redash_is_published
+
+    @redash_is_published.setter
+    def redash_is_published(self, redash_is_published: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.redash_is_published = redash_is_published
+
+    type_name: str = Field("Redash", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Redash":
+            raise ValueError("must be Redash")
+        return v
+
+    class Attributes(BI.Attributes):
+        redash_is_published: Optional[bool] = Field(
+            None, description="", alias="redashIsPublished"
+        )
+
+    attributes: "Redash.Attributes" = Field(
+        default_factory=lambda: Redash.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class DataStudio(Google):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in DataStudio._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -7452,371 +7866,195 @@
     attributes: "PowerBI.Attributes" = Field(
         default_factory=lambda: PowerBI.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class Preset(BI):
+class MicroStrategy(BI):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in Preset._convience_properties:
+        if name in MicroStrategy._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "preset_workspace_id",
-        "preset_workspace_qualified_name",
-        "preset_dashboard_id",
-        "preset_dashboard_qualified_name",
+        "micro_strategy_project_qualified_name",
+        "micro_strategy_project_name",
+        "micro_strategy_cube_qualified_names",
+        "micro_strategy_cube_names",
+        "micro_strategy_report_qualified_names",
+        "micro_strategy_report_names",
+        "micro_strategy_is_certified",
+        "micro_strategy_certified_by",
+        "micro_strategy_certified_at",
+        "micro_strategy_location",
     ]
 
     @property
-    def preset_workspace_id(self) -> Optional[int]:
-        return self.attributes.preset_workspace_id
+    def micro_strategy_project_qualified_name(self) -> Optional[str]:
+        return self.attributes.micro_strategy_project_qualified_name
 
-    @preset_workspace_id.setter
-    def preset_workspace_id(self, preset_workspace_id: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.preset_workspace_id = preset_workspace_id
-
-    @property
-    def preset_workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.preset_workspace_qualified_name
-
-    @preset_workspace_qualified_name.setter
-    def preset_workspace_qualified_name(
-        self, preset_workspace_qualified_name: Optional[str]
+    @micro_strategy_project_qualified_name.setter
+    def micro_strategy_project_qualified_name(
+        self, micro_strategy_project_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.preset_workspace_qualified_name = (
-            preset_workspace_qualified_name
+        self.attributes.micro_strategy_project_qualified_name = (
+            micro_strategy_project_qualified_name
         )
 
     @property
-    def preset_dashboard_id(self) -> Optional[int]:
-        return self.attributes.preset_dashboard_id
+    def micro_strategy_project_name(self) -> Optional[str]:
+        return self.attributes.micro_strategy_project_name
 
-    @preset_dashboard_id.setter
-    def preset_dashboard_id(self, preset_dashboard_id: Optional[int]):
+    @micro_strategy_project_name.setter
+    def micro_strategy_project_name(self, micro_strategy_project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.preset_dashboard_id = preset_dashboard_id
+        self.attributes.micro_strategy_project_name = micro_strategy_project_name
 
     @property
-    def preset_dashboard_qualified_name(self) -> Optional[str]:
-        return self.attributes.preset_dashboard_qualified_name
+    def micro_strategy_cube_qualified_names(self) -> Optional[set[str]]:
+        return self.attributes.micro_strategy_cube_qualified_names
 
-    @preset_dashboard_qualified_name.setter
-    def preset_dashboard_qualified_name(
-        self, preset_dashboard_qualified_name: Optional[str]
+    @micro_strategy_cube_qualified_names.setter
+    def micro_strategy_cube_qualified_names(
+        self, micro_strategy_cube_qualified_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.preset_dashboard_qualified_name = (
-            preset_dashboard_qualified_name
-        )
-
-    type_name: str = Field("Preset", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Preset":
-            raise ValueError("must be Preset")
-        return v
-
-    class Attributes(BI.Attributes):
-        preset_workspace_id: Optional[int] = Field(
-            None, description="", alias="presetWorkspaceId"
-        )
-        preset_workspace_qualified_name: Optional[str] = Field(
-            None, description="", alias="presetWorkspaceQualifiedName"
-        )
-        preset_dashboard_id: Optional[int] = Field(
-            None, description="", alias="presetDashboardId"
+        self.attributes.micro_strategy_cube_qualified_names = (
+            micro_strategy_cube_qualified_names
         )
-        preset_dashboard_qualified_name: Optional[str] = Field(
-            None, description="", alias="presetDashboardQualifiedName"
-        )
-
-    attributes: "Preset.Attributes" = Field(
-        default_factory=lambda: Preset.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class Sigma(BI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in Sigma._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "sigma_workbook_qualified_name",
-        "sigma_workbook_name",
-        "sigma_page_qualified_name",
-        "sigma_page_name",
-        "sigma_data_element_qualified_name",
-        "sigma_data_element_name",
-    ]
-
-    @property
-    def sigma_workbook_qualified_name(self) -> Optional[str]:
-        return self.attributes.sigma_workbook_qualified_name
-
-    @sigma_workbook_qualified_name.setter
-    def sigma_workbook_qualified_name(
-        self, sigma_workbook_qualified_name: Optional[str]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_workbook_qualified_name = sigma_workbook_qualified_name
-
-    @property
-    def sigma_workbook_name(self) -> Optional[str]:
-        return self.attributes.sigma_workbook_name
-
-    @sigma_workbook_name.setter
-    def sigma_workbook_name(self, sigma_workbook_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_workbook_name = sigma_workbook_name
 
     @property
-    def sigma_page_qualified_name(self) -> Optional[str]:
-        return self.attributes.sigma_page_qualified_name
+    def micro_strategy_cube_names(self) -> Optional[set[str]]:
+        return self.attributes.micro_strategy_cube_names
 
-    @sigma_page_qualified_name.setter
-    def sigma_page_qualified_name(self, sigma_page_qualified_name: Optional[str]):
+    @micro_strategy_cube_names.setter
+    def micro_strategy_cube_names(self, micro_strategy_cube_names: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.sigma_page_qualified_name = sigma_page_qualified_name
+        self.attributes.micro_strategy_cube_names = micro_strategy_cube_names
 
     @property
-    def sigma_page_name(self) -> Optional[str]:
-        return self.attributes.sigma_page_name
-
-    @sigma_page_name.setter
-    def sigma_page_name(self, sigma_page_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_page_name = sigma_page_name
+    def micro_strategy_report_qualified_names(self) -> Optional[set[str]]:
+        return self.attributes.micro_strategy_report_qualified_names
 
-    @property
-    def sigma_data_element_qualified_name(self) -> Optional[str]:
-        return self.attributes.sigma_data_element_qualified_name
-
-    @sigma_data_element_qualified_name.setter
-    def sigma_data_element_qualified_name(
-        self, sigma_data_element_qualified_name: Optional[str]
+    @micro_strategy_report_qualified_names.setter
+    def micro_strategy_report_qualified_names(
+        self, micro_strategy_report_qualified_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.sigma_data_element_qualified_name = (
-            sigma_data_element_qualified_name
+        self.attributes.micro_strategy_report_qualified_names = (
+            micro_strategy_report_qualified_names
         )
 
     @property
-    def sigma_data_element_name(self) -> Optional[str]:
-        return self.attributes.sigma_data_element_name
-
-    @sigma_data_element_name.setter
-    def sigma_data_element_name(self, sigma_data_element_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_data_element_name = sigma_data_element_name
-
-    type_name: str = Field("Sigma", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Sigma":
-            raise ValueError("must be Sigma")
-        return v
-
-    class Attributes(BI.Attributes):
-        sigma_workbook_qualified_name: Optional[str] = Field(
-            None, description="", alias="sigmaWorkbookQualifiedName"
-        )
-        sigma_workbook_name: Optional[str] = Field(
-            None, description="", alias="sigmaWorkbookName"
-        )
-        sigma_page_qualified_name: Optional[str] = Field(
-            None, description="", alias="sigmaPageQualifiedName"
-        )
-        sigma_page_name: Optional[str] = Field(
-            None, description="", alias="sigmaPageName"
-        )
-        sigma_data_element_qualified_name: Optional[str] = Field(
-            None, description="", alias="sigmaDataElementQualifiedName"
-        )
-        sigma_data_element_name: Optional[str] = Field(
-            None, description="", alias="sigmaDataElementName"
-        )
-
-    attributes: "Sigma.Attributes" = Field(
-        default_factory=lambda: Sigma.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class Mode(BI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in Mode._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "mode_id",
-        "mode_token",
-        "mode_workspace_name",
-        "mode_workspace_username",
-        "mode_workspace_qualified_name",
-        "mode_report_name",
-        "mode_report_qualified_name",
-        "mode_query_name",
-        "mode_query_qualified_name",
-    ]
-
-    @property
-    def mode_id(self) -> Optional[str]:
-        return self.attributes.mode_id
-
-    @mode_id.setter
-    def mode_id(self, mode_id: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_id = mode_id
-
-    @property
-    def mode_token(self) -> Optional[str]:
-        return self.attributes.mode_token
-
-    @mode_token.setter
-    def mode_token(self, mode_token: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_token = mode_token
-
-    @property
-    def mode_workspace_name(self) -> Optional[str]:
-        return self.attributes.mode_workspace_name
-
-    @mode_workspace_name.setter
-    def mode_workspace_name(self, mode_workspace_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_workspace_name = mode_workspace_name
-
-    @property
-    def mode_workspace_username(self) -> Optional[str]:
-        return self.attributes.mode_workspace_username
-
-    @mode_workspace_username.setter
-    def mode_workspace_username(self, mode_workspace_username: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.mode_workspace_username = mode_workspace_username
-
-    @property
-    def mode_workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.mode_workspace_qualified_name
+    def micro_strategy_report_names(self) -> Optional[set[str]]:
+        return self.attributes.micro_strategy_report_names
 
-    @mode_workspace_qualified_name.setter
-    def mode_workspace_qualified_name(
-        self, mode_workspace_qualified_name: Optional[str]
+    @micro_strategy_report_names.setter
+    def micro_strategy_report_names(
+        self, micro_strategy_report_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.mode_workspace_qualified_name = mode_workspace_qualified_name
+        self.attributes.micro_strategy_report_names = micro_strategy_report_names
 
     @property
-    def mode_report_name(self) -> Optional[str]:
-        return self.attributes.mode_report_name
+    def micro_strategy_is_certified(self) -> Optional[bool]:
+        return self.attributes.micro_strategy_is_certified
 
-    @mode_report_name.setter
-    def mode_report_name(self, mode_report_name: Optional[str]):
+    @micro_strategy_is_certified.setter
+    def micro_strategy_is_certified(self, micro_strategy_is_certified: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.mode_report_name = mode_report_name
+        self.attributes.micro_strategy_is_certified = micro_strategy_is_certified
 
     @property
-    def mode_report_qualified_name(self) -> Optional[str]:
-        return self.attributes.mode_report_qualified_name
+    def micro_strategy_certified_by(self) -> Optional[str]:
+        return self.attributes.micro_strategy_certified_by
 
-    @mode_report_qualified_name.setter
-    def mode_report_qualified_name(self, mode_report_qualified_name: Optional[str]):
+    @micro_strategy_certified_by.setter
+    def micro_strategy_certified_by(self, micro_strategy_certified_by: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.mode_report_qualified_name = mode_report_qualified_name
+        self.attributes.micro_strategy_certified_by = micro_strategy_certified_by
 
     @property
-    def mode_query_name(self) -> Optional[str]:
-        return self.attributes.mode_query_name
+    def micro_strategy_certified_at(self) -> Optional[datetime]:
+        return self.attributes.micro_strategy_certified_at
 
-    @mode_query_name.setter
-    def mode_query_name(self, mode_query_name: Optional[str]):
+    @micro_strategy_certified_at.setter
+    def micro_strategy_certified_at(
+        self, micro_strategy_certified_at: Optional[datetime]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.mode_query_name = mode_query_name
+        self.attributes.micro_strategy_certified_at = micro_strategy_certified_at
 
     @property
-    def mode_query_qualified_name(self) -> Optional[str]:
-        return self.attributes.mode_query_qualified_name
+    def micro_strategy_location(self) -> Optional[list[dict[str, str]]]:
+        return self.attributes.micro_strategy_location
 
-    @mode_query_qualified_name.setter
-    def mode_query_qualified_name(self, mode_query_qualified_name: Optional[str]):
+    @micro_strategy_location.setter
+    def micro_strategy_location(
+        self, micro_strategy_location: Optional[list[dict[str, str]]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.mode_query_qualified_name = mode_query_qualified_name
+        self.attributes.micro_strategy_location = micro_strategy_location
 
-    type_name: str = Field("Mode", allow_mutation=False)
+    type_name: str = Field("MicroStrategy", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "Mode":
-            raise ValueError("must be Mode")
+        if v != "MicroStrategy":
+            raise ValueError("must be MicroStrategy")
         return v
 
     class Attributes(BI.Attributes):
-        mode_id: Optional[str] = Field(None, description="", alias="modeId")
-        mode_token: Optional[str] = Field(None, description="", alias="modeToken")
-        mode_workspace_name: Optional[str] = Field(
-            None, description="", alias="modeWorkspaceName"
+        micro_strategy_project_qualified_name: Optional[str] = Field(
+            None, description="", alias="microStrategyProjectQualifiedName"
         )
-        mode_workspace_username: Optional[str] = Field(
-            None, description="", alias="modeWorkspaceUsername"
+        micro_strategy_project_name: Optional[str] = Field(
+            None, description="", alias="microStrategyProjectName"
         )
-        mode_workspace_qualified_name: Optional[str] = Field(
-            None, description="", alias="modeWorkspaceQualifiedName"
+        micro_strategy_cube_qualified_names: Optional[set[str]] = Field(
+            None, description="", alias="microStrategyCubeQualifiedNames"
         )
-        mode_report_name: Optional[str] = Field(
-            None, description="", alias="modeReportName"
+        micro_strategy_cube_names: Optional[set[str]] = Field(
+            None, description="", alias="microStrategyCubeNames"
         )
-        mode_report_qualified_name: Optional[str] = Field(
-            None, description="", alias="modeReportQualifiedName"
+        micro_strategy_report_qualified_names: Optional[set[str]] = Field(
+            None, description="", alias="microStrategyReportQualifiedNames"
         )
-        mode_query_name: Optional[str] = Field(
-            None, description="", alias="modeQueryName"
+        micro_strategy_report_names: Optional[set[str]] = Field(
+            None, description="", alias="microStrategyReportNames"
         )
-        mode_query_qualified_name: Optional[str] = Field(
-            None, description="", alias="modeQueryQualifiedName"
+        micro_strategy_is_certified: Optional[bool] = Field(
+            None, description="", alias="microStrategyIsCertified"
+        )
+        micro_strategy_certified_by: Optional[str] = Field(
+            None, description="", alias="microStrategyCertifiedBy"
+        )
+        micro_strategy_certified_at: Optional[datetime] = Field(
+            None, description="", alias="microStrategyCertifiedAt"
+        )
+        micro_strategy_location: Optional[list[dict[str, str]]] = Field(
+            None, description="", alias="microStrategyLocation"
         )
 
-    attributes: "Mode.Attributes" = Field(
-        default_factory=lambda: Mode.Attributes(),
+    attributes: "MicroStrategy.Attributes" = Field(
+        default_factory=lambda: MicroStrategy.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class Qlik(BI):
     """Description"""
@@ -7944,94 +8182,14 @@
     attributes: "Qlik.Attributes" = Field(
         default_factory=lambda: Qlik.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class Tableau(BI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in Tableau._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
-    type_name: str = Field("Tableau", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Tableau":
-            raise ValueError("must be Tableau")
-        return v
-
-
-class Looker(BI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in Looker._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
-    type_name: str = Field("Looker", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Looker":
-            raise ValueError("must be Looker")
-        return v
-
-
-class Redash(BI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in Redash._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "redash_is_published",
-    ]
-
-    @property
-    def redash_is_published(self) -> Optional[bool]:
-        return self.attributes.redash_is_published
-
-    @redash_is_published.setter
-    def redash_is_published(self, redash_is_published: Optional[bool]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.redash_is_published = redash_is_published
-
-    type_name: str = Field("Redash", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Redash":
-            raise ValueError("must be Redash")
-        return v
-
-    class Attributes(BI.Attributes):
-        redash_is_published: Optional[bool] = Field(
-            None, description="", alias="redashIsPublished"
-        )
-
-    attributes: "Redash.Attributes" = Field(
-        default_factory=lambda: Redash.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
 class Salesforce(SaaS):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Salesforce._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -10537,16 +10695,16 @@
         "external_location_format",
         "is_partitioned",
         "partition_strategy",
         "partition_count",
         "partition_list",
         "partitions",
         "columns",
-        "facts",
         "queries",
+        "facts",
         "atlan_schema",
         "dimensions",
     ]
 
     @property
     def column_count(self) -> Optional[int]:
         return self.attributes.column_count
@@ -10704,34 +10862,34 @@
     @columns.setter
     def columns(self, columns: Optional[list[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.columns = columns
 
     @property
-    def facts(self) -> Optional[list[Table]]:
-        return self.attributes.facts
-
-    @facts.setter
-    def facts(self, facts: Optional[list[Table]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.facts = facts
-
-    @property
     def queries(self) -> Optional[list[Query]]:
         return self.attributes.queries
 
     @queries.setter
     def queries(self, queries: Optional[list[Query]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.queries = queries
 
     @property
+    def facts(self) -> Optional[list[Table]]:
+        return self.attributes.facts
+
+    @facts.setter
+    def facts(self, facts: Optional[list[Table]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.facts = facts
+
+    @property
     def atlan_schema(self) -> Optional[Schema]:
         return self.attributes.atlan_schema
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -10790,20 +10948,20 @@
         )
         partitions: Optional[list[TablePartition]] = Field(
             None, description="", alias="partitions"
         )  # relationship
         columns: Optional[list[Column]] = Field(
             None, description="", alias="columns"
         )  # relationship
-        facts: Optional[list[Table]] = Field(
-            None, description="", alias="facts"
-        )  # relationship
         queries: Optional[list[Query]] = Field(
             None, description="", alias="queries"
         )  # relationship
+        facts: Optional[list[Table]] = Field(
+            None, description="", alias="facts"
+        )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
         dimensions: Optional[list[Table]] = Field(
             None, description="", alias="dimensions"
         )  # relationship
 
@@ -11950,16 +12108,16 @@
         if name in Schema._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "table_count",
         "views_count",
-        "materialised_views",
         "snowflake_tags",
+        "materialised_views",
         "tables",
         "database",
         "snowflake_pipes",
         "snowflake_streams",
         "procedures",
         "views",
     ]
@@ -11981,34 +12139,34 @@
     @views_count.setter
     def views_count(self, views_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.views_count = views_count
 
     @property
-    def materialised_views(self) -> Optional[list[MaterialisedView]]:
-        return self.attributes.materialised_views
-
-    @materialised_views.setter
-    def materialised_views(self, materialised_views: Optional[list[MaterialisedView]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.materialised_views = materialised_views
-
-    @property
     def snowflake_tags(self) -> Optional[list[SnowflakeTag]]:
         return self.attributes.snowflake_tags
 
     @snowflake_tags.setter
     def snowflake_tags(self, snowflake_tags: Optional[list[SnowflakeTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_tags = snowflake_tags
 
     @property
+    def materialised_views(self) -> Optional[list[MaterialisedView]]:
+        return self.attributes.materialised_views
+
+    @materialised_views.setter
+    def materialised_views(self, materialised_views: Optional[list[MaterialisedView]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.materialised_views = materialised_views
+
+    @property
     def tables(self) -> Optional[list[Table]]:
         return self.attributes.tables
 
     @tables.setter
     def tables(self, tables: Optional[list[Table]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -12071,20 +12229,20 @@
         if v != "Schema":
             raise ValueError("must be Schema")
         return v
 
     class Attributes(SQL.Attributes):
         table_count: Optional[int] = Field(None, description="", alias="tableCount")
         views_count: Optional[int] = Field(None, description="", alias="viewsCount")
-        materialised_views: Optional[list[MaterialisedView]] = Field(
-            None, description="", alias="materialisedViews"
-        )  # relationship
         snowflake_tags: Optional[list[SnowflakeTag]] = Field(
             None, description="", alias="snowflakeTags"
         )  # relationship
+        materialised_views: Optional[list[MaterialisedView]] = Field(
+            None, description="", alias="materialisedViews"
+        )  # relationship
         tables: Optional[list[Table]] = Field(
             None, description="", alias="tables"
         )  # relationship
         database: Optional[Database] = Field(
             None, description="", alias="database"
         )  # relationship
         snowflake_pipes: Optional[list[SnowflakePipe]] = Field(
@@ -12141,115 +12299,14 @@
         )
         attributes = Schema.Attributes.create(
             name=name, database_qualified_name=database_qualified_name
         )
         return cls(attributes=attributes)
 
 
-class Database(SQL):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in Database._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "schema_count",
-        "schemas",
-    ]
-
-    @property
-    def schema_count(self) -> Optional[int]:
-        return self.attributes.schema_count
-
-    @schema_count.setter
-    def schema_count(self, schema_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.schema_count = schema_count
-
-    @property
-    def schemas(self) -> Optional[list[Schema]]:
-        return self.attributes.schemas
-
-    @schemas.setter
-    def schemas(self, schemas: Optional[list[Schema]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.schemas = schemas
-
-    type_name: str = Field("Database", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "Database":
-            raise ValueError("must be Database")
-        return v
-
-    class Attributes(SQL.Attributes):
-        schema_count: Optional[int] = Field(None, description="", alias="schemaCount")
-        schemas: Optional[list[Schema]] = Field(
-            None, description="", alias="schemas"
-        )  # relationship
-
-        @classmethod
-        # @validate_arguments()
-        def create(
-            cls, name: str, connection_qualified_name: str
-        ) -> Database.Attributes:
-            if not name:
-                raise ValueError("name cannot be blank")
-            validate_required_fields(
-                ["connection_qualified_name"], [connection_qualified_name]
-            )
-            fields = connection_qualified_name.split("/")
-            if len(fields) != 3:
-                raise ValueError("Invalid connection_qualified_name")
-            try:
-                connector_type = AtlanConnectorType(fields[1])  # type:ignore
-            except ValueError as e:
-                raise ValueError("Invalid connection_qualified_name") from e
-            return Database.Attributes(
-                name=name,
-                connection_qualified_name=connection_qualified_name,
-                qualified_name=f"{connection_qualified_name}/{name}",
-                connector_name=connector_type.value,
-            )
-
-    attributes: "Database.Attributes" = Field(
-        default_factory=lambda: Database.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-    @classmethod
-    # @validate_arguments()
-    def create(cls, *, name: str, connection_qualified_name: str) -> Database:
-        if not name:
-            raise ValueError("name cannot be blank")
-        validate_required_fields(
-            ["connection_qualified_name"], [connection_qualified_name]
-        )
-        fields = connection_qualified_name.split("/")
-        if len(fields) != 3:
-            raise ValueError("Invalid connection_qualified_name")
-        try:
-            connector_type = AtlanConnectorType(fields[1])  # type:ignore
-        except ValueError as e:
-            raise ValueError("Invalid connection_qualified_name") from e
-        attributes = Database.Attributes(
-            name=name,
-            connection_qualified_name=connection_qualified_name,
-            qualified_name=f"{connection_qualified_name}/{name}",
-            connector_name=connector_type.value,
-        )
-        return cls(attributes=attributes)
-
-
 class SnowflakeStream(SQL):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in SnowflakeStream._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -12446,14 +12503,115 @@
     attributes: "SnowflakePipe.Attributes" = Field(
         default_factory=lambda: SnowflakePipe.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class Database(SQL):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Database._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "schema_count",
+        "schemas",
+    ]
+
+    @property
+    def schema_count(self) -> Optional[int]:
+        return self.attributes.schema_count
+
+    @schema_count.setter
+    def schema_count(self, schema_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.schema_count = schema_count
+
+    @property
+    def schemas(self) -> Optional[list[Schema]]:
+        return self.attributes.schemas
+
+    @schemas.setter
+    def schemas(self, schemas: Optional[list[Schema]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.schemas = schemas
+
+    type_name: str = Field("Database", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Database":
+            raise ValueError("must be Database")
+        return v
+
+    class Attributes(SQL.Attributes):
+        schema_count: Optional[int] = Field(None, description="", alias="schemaCount")
+        schemas: Optional[list[Schema]] = Field(
+            None, description="", alias="schemas"
+        )  # relationship
+
+        @classmethod
+        # @validate_arguments()
+        def create(
+            cls, name: str, connection_qualified_name: str
+        ) -> Database.Attributes:
+            if not name:
+                raise ValueError("name cannot be blank")
+            validate_required_fields(
+                ["connection_qualified_name"], [connection_qualified_name]
+            )
+            fields = connection_qualified_name.split("/")
+            if len(fields) != 3:
+                raise ValueError("Invalid connection_qualified_name")
+            try:
+                connector_type = AtlanConnectorType(fields[1])  # type:ignore
+            except ValueError as e:
+                raise ValueError("Invalid connection_qualified_name") from e
+            return Database.Attributes(
+                name=name,
+                connection_qualified_name=connection_qualified_name,
+                qualified_name=f"{connection_qualified_name}/{name}",
+                connector_name=connector_type.value,
+            )
+
+    attributes: "Database.Attributes" = Field(
+        default_factory=lambda: Database.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+    @classmethod
+    # @validate_arguments()
+    def create(cls, *, name: str, connection_qualified_name: str) -> Database:
+        if not name:
+            raise ValueError("name cannot be blank")
+        validate_required_fields(
+            ["connection_qualified_name"], [connection_qualified_name]
+        )
+        fields = connection_qualified_name.split("/")
+        if len(fields) != 3:
+            raise ValueError("Invalid connection_qualified_name")
+        try:
+            connector_type = AtlanConnectorType(fields[1])  # type:ignore
+        except ValueError as e:
+            raise ValueError("Invalid connection_qualified_name") from e
+        attributes = Database.Attributes(
+            name=name,
+            connection_qualified_name=connection_qualified_name,
+            qualified_name=f"{connection_qualified_name}/{name}",
+            connector_name=connector_type.value,
+        )
+        return cls(attributes=attributes)
+
+
 class Procedure(SQL):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Procedure._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -15259,2269 +15417,14 @@
     attributes: "MCMonitor.Attributes" = Field(
         default_factory=lambda: MCMonitor.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class MetabaseQuestion(Metabase):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in MetabaseQuestion._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "metabase_dashboard_count",
-        "metabase_query_type",
-        "metabase_query",
-        "metabase_dashboards",
-        "metabase_collection",
-    ]
-
-    @property
-    def metabase_dashboard_count(self) -> Optional[int]:
-        return self.attributes.metabase_dashboard_count
-
-    @metabase_dashboard_count.setter
-    def metabase_dashboard_count(self, metabase_dashboard_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_dashboard_count = metabase_dashboard_count
-
-    @property
-    def metabase_query_type(self) -> Optional[str]:
-        return self.attributes.metabase_query_type
-
-    @metabase_query_type.setter
-    def metabase_query_type(self, metabase_query_type: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_query_type = metabase_query_type
-
-    @property
-    def metabase_query(self) -> Optional[str]:
-        return self.attributes.metabase_query
-
-    @metabase_query.setter
-    def metabase_query(self, metabase_query: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_query = metabase_query
-
-    @property
-    def metabase_dashboards(self) -> Optional[list[MetabaseDashboard]]:
-        return self.attributes.metabase_dashboards
-
-    @metabase_dashboards.setter
-    def metabase_dashboards(
-        self, metabase_dashboards: Optional[list[MetabaseDashboard]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_dashboards = metabase_dashboards
-
-    @property
-    def metabase_collection(self) -> Optional[MetabaseCollection]:
-        return self.attributes.metabase_collection
-
-    @metabase_collection.setter
-    def metabase_collection(self, metabase_collection: Optional[MetabaseCollection]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_collection = metabase_collection
-
-    type_name: str = Field("MetabaseQuestion", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MetabaseQuestion":
-            raise ValueError("must be MetabaseQuestion")
-        return v
-
-    class Attributes(Metabase.Attributes):
-        metabase_dashboard_count: Optional[int] = Field(
-            None, description="", alias="metabaseDashboardCount"
-        )
-        metabase_query_type: Optional[str] = Field(
-            None, description="", alias="metabaseQueryType"
-        )
-        metabase_query: Optional[str] = Field(
-            None, description="", alias="metabaseQuery"
-        )
-        metabase_dashboards: Optional[list[MetabaseDashboard]] = Field(
-            None, description="", alias="metabaseDashboards"
-        )  # relationship
-        metabase_collection: Optional[MetabaseCollection] = Field(
-            None, description="", alias="metabaseCollection"
-        )  # relationship
-
-    attributes: "MetabaseQuestion.Attributes" = Field(
-        default_factory=lambda: MetabaseQuestion.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class MetabaseCollection(Metabase):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in MetabaseCollection._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "metabase_slug",
-        "metabase_color",
-        "metabase_namespace",
-        "metabase_is_personal_collection",
-        "metabase_dashboards",
-        "metabase_questions",
-    ]
-
-    @property
-    def metabase_slug(self) -> Optional[str]:
-        return self.attributes.metabase_slug
-
-    @metabase_slug.setter
-    def metabase_slug(self, metabase_slug: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_slug = metabase_slug
-
-    @property
-    def metabase_color(self) -> Optional[str]:
-        return self.attributes.metabase_color
-
-    @metabase_color.setter
-    def metabase_color(self, metabase_color: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_color = metabase_color
-
-    @property
-    def metabase_namespace(self) -> Optional[str]:
-        return self.attributes.metabase_namespace
-
-    @metabase_namespace.setter
-    def metabase_namespace(self, metabase_namespace: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_namespace = metabase_namespace
-
-    @property
-    def metabase_is_personal_collection(self) -> Optional[bool]:
-        return self.attributes.metabase_is_personal_collection
-
-    @metabase_is_personal_collection.setter
-    def metabase_is_personal_collection(
-        self, metabase_is_personal_collection: Optional[bool]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_is_personal_collection = (
-            metabase_is_personal_collection
-        )
-
-    @property
-    def metabase_dashboards(self) -> Optional[list[MetabaseDashboard]]:
-        return self.attributes.metabase_dashboards
-
-    @metabase_dashboards.setter
-    def metabase_dashboards(
-        self, metabase_dashboards: Optional[list[MetabaseDashboard]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_dashboards = metabase_dashboards
-
-    @property
-    def metabase_questions(self) -> Optional[list[MetabaseQuestion]]:
-        return self.attributes.metabase_questions
-
-    @metabase_questions.setter
-    def metabase_questions(self, metabase_questions: Optional[list[MetabaseQuestion]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_questions = metabase_questions
-
-    type_name: str = Field("MetabaseCollection", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MetabaseCollection":
-            raise ValueError("must be MetabaseCollection")
-        return v
-
-    class Attributes(Metabase.Attributes):
-        metabase_slug: Optional[str] = Field(None, description="", alias="metabaseSlug")
-        metabase_color: Optional[str] = Field(
-            None, description="", alias="metabaseColor"
-        )
-        metabase_namespace: Optional[str] = Field(
-            None, description="", alias="metabaseNamespace"
-        )
-        metabase_is_personal_collection: Optional[bool] = Field(
-            None, description="", alias="metabaseIsPersonalCollection"
-        )
-        metabase_dashboards: Optional[list[MetabaseDashboard]] = Field(
-            None, description="", alias="metabaseDashboards"
-        )  # relationship
-        metabase_questions: Optional[list[MetabaseQuestion]] = Field(
-            None, description="", alias="metabaseQuestions"
-        )  # relationship
-
-    attributes: "MetabaseCollection.Attributes" = Field(
-        default_factory=lambda: MetabaseCollection.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class MetabaseDashboard(Metabase):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in MetabaseDashboard._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "metabase_question_count",
-        "metabase_questions",
-        "metabase_collection",
-    ]
-
-    @property
-    def metabase_question_count(self) -> Optional[int]:
-        return self.attributes.metabase_question_count
-
-    @metabase_question_count.setter
-    def metabase_question_count(self, metabase_question_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_question_count = metabase_question_count
-
-    @property
-    def metabase_questions(self) -> Optional[list[MetabaseQuestion]]:
-        return self.attributes.metabase_questions
-
-    @metabase_questions.setter
-    def metabase_questions(self, metabase_questions: Optional[list[MetabaseQuestion]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_questions = metabase_questions
-
-    @property
-    def metabase_collection(self) -> Optional[MetabaseCollection]:
-        return self.attributes.metabase_collection
-
-    @metabase_collection.setter
-    def metabase_collection(self, metabase_collection: Optional[MetabaseCollection]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.metabase_collection = metabase_collection
-
-    type_name: str = Field("MetabaseDashboard", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "MetabaseDashboard":
-            raise ValueError("must be MetabaseDashboard")
-        return v
-
-    class Attributes(Metabase.Attributes):
-        metabase_question_count: Optional[int] = Field(
-            None, description="", alias="metabaseQuestionCount"
-        )
-        metabase_questions: Optional[list[MetabaseQuestion]] = Field(
-            None, description="", alias="metabaseQuestions"
-        )  # relationship
-        metabase_collection: Optional[MetabaseCollection] = Field(
-            None, description="", alias="metabaseCollection"
-        )  # relationship
-
-    attributes: "MetabaseDashboard.Attributes" = Field(
-        default_factory=lambda: MetabaseDashboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class QuickSightFolder(QuickSight):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in QuickSightFolder._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "quick_sight_folder_type",
-        "quick_sight_folder_hierarchy",
-        "quick_sight_dashboards",
-        "quick_sight_analyses",
-        "quick_sight_datasets",
-    ]
-
-    @property
-    def quick_sight_folder_type(self) -> Optional[QuickSightFolderType]:
-        return self.attributes.quick_sight_folder_type
-
-    @quick_sight_folder_type.setter
-    def quick_sight_folder_type(
-        self, quick_sight_folder_type: Optional[QuickSightFolderType]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_folder_type = quick_sight_folder_type
-
-    @property
-    def quick_sight_folder_hierarchy(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.quick_sight_folder_hierarchy
-
-    @quick_sight_folder_hierarchy.setter
-    def quick_sight_folder_hierarchy(
-        self, quick_sight_folder_hierarchy: Optional[list[dict[str, str]]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_folder_hierarchy = quick_sight_folder_hierarchy
-
-    @property
-    def quick_sight_dashboards(self) -> Optional[list[QuickSightDashboard]]:
-        return self.attributes.quick_sight_dashboards
-
-    @quick_sight_dashboards.setter
-    def quick_sight_dashboards(
-        self, quick_sight_dashboards: Optional[list[QuickSightDashboard]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dashboards = quick_sight_dashboards
-
-    @property
-    def quick_sight_analyses(self) -> Optional[list[QuickSightAnalysis]]:
-        return self.attributes.quick_sight_analyses
-
-    @quick_sight_analyses.setter
-    def quick_sight_analyses(
-        self, quick_sight_analyses: Optional[list[QuickSightAnalysis]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analyses = quick_sight_analyses
-
-    @property
-    def quick_sight_datasets(self) -> Optional[list[QuickSightDataset]]:
-        return self.attributes.quick_sight_datasets
-
-    @quick_sight_datasets.setter
-    def quick_sight_datasets(
-        self, quick_sight_datasets: Optional[list[QuickSightDataset]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_datasets = quick_sight_datasets
-
-    type_name: str = Field("QuickSightFolder", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightFolder":
-            raise ValueError("must be QuickSightFolder")
-        return v
-
-    class Attributes(QuickSight.Attributes):
-        quick_sight_folder_type: Optional[QuickSightFolderType] = Field(
-            None, description="", alias="quickSightFolderType"
-        )
-        quick_sight_folder_hierarchy: Optional[list[dict[str, str]]] = Field(
-            None, description="", alias="quickSightFolderHierarchy"
-        )
-        quick_sight_dashboards: Optional[list[QuickSightDashboard]] = Field(
-            None, description="", alias="quickSightDashboards"
-        )  # relationship
-        quick_sight_analyses: Optional[list[QuickSightAnalysis]] = Field(
-            None, description="", alias="quickSightAnalyses"
-        )  # relationship
-        quick_sight_datasets: Optional[list[QuickSightDataset]] = Field(
-            None, description="", alias="quickSightDatasets"
-        )  # relationship
-
-    attributes: "QuickSightFolder.Attributes" = Field(
-        default_factory=lambda: QuickSightFolder.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class QuickSightDashboardVisual(QuickSight):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in QuickSightDashboardVisual._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "quick_sight_dashboard_qualified_name",
-        "quick_sight_dashboard",
-    ]
-
-    @property
-    def quick_sight_dashboard_qualified_name(self) -> Optional[str]:
-        return self.attributes.quick_sight_dashboard_qualified_name
-
-    @quick_sight_dashboard_qualified_name.setter
-    def quick_sight_dashboard_qualified_name(
-        self, quick_sight_dashboard_qualified_name: Optional[str]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dashboard_qualified_name = (
-            quick_sight_dashboard_qualified_name
-        )
-
-    @property
-    def quick_sight_dashboard(self) -> Optional[QuickSightDashboard]:
-        return self.attributes.quick_sight_dashboard
-
-    @quick_sight_dashboard.setter
-    def quick_sight_dashboard(
-        self, quick_sight_dashboard: Optional[QuickSightDashboard]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dashboard = quick_sight_dashboard
-
-    type_name: str = Field("QuickSightDashboardVisual", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightDashboardVisual":
-            raise ValueError("must be QuickSightDashboardVisual")
-        return v
-
-    class Attributes(QuickSight.Attributes):
-        quick_sight_dashboard_qualified_name: Optional[str] = Field(
-            None, description="", alias="quickSightDashboardQualifiedName"
-        )
-        quick_sight_dashboard: Optional[QuickSightDashboard] = Field(
-            None, description="", alias="quickSightDashboard"
-        )  # relationship
-
-    attributes: "QuickSightDashboardVisual.Attributes" = Field(
-        default_factory=lambda: QuickSightDashboardVisual.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class QuickSightAnalysis(QuickSight):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in QuickSightAnalysis._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "quick_sight_analysis_status",
-        "quick_sight_analysis_calculated_fields",
-        "quick_sight_analysis_parameter_declarations",
-        "quick_sight_analysis_filter_groups",
-        "quick_sight_analysis_visuals",
-        "quick_sight_analysis_folders",
-    ]
-
-    @property
-    def quick_sight_analysis_status(self) -> Optional[QuickSightAnalysisStatus]:
-        return self.attributes.quick_sight_analysis_status
-
-    @quick_sight_analysis_status.setter
-    def quick_sight_analysis_status(
-        self, quick_sight_analysis_status: Optional[QuickSightAnalysisStatus]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis_status = quick_sight_analysis_status
-
-    @property
-    def quick_sight_analysis_calculated_fields(self) -> Optional[set[str]]:
-        return self.attributes.quick_sight_analysis_calculated_fields
-
-    @quick_sight_analysis_calculated_fields.setter
-    def quick_sight_analysis_calculated_fields(
-        self, quick_sight_analysis_calculated_fields: Optional[set[str]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis_calculated_fields = (
-            quick_sight_analysis_calculated_fields
-        )
-
-    @property
-    def quick_sight_analysis_parameter_declarations(self) -> Optional[set[str]]:
-        return self.attributes.quick_sight_analysis_parameter_declarations
-
-    @quick_sight_analysis_parameter_declarations.setter
-    def quick_sight_analysis_parameter_declarations(
-        self, quick_sight_analysis_parameter_declarations: Optional[set[str]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis_parameter_declarations = (
-            quick_sight_analysis_parameter_declarations
-        )
-
-    @property
-    def quick_sight_analysis_filter_groups(self) -> Optional[set[str]]:
-        return self.attributes.quick_sight_analysis_filter_groups
-
-    @quick_sight_analysis_filter_groups.setter
-    def quick_sight_analysis_filter_groups(
-        self, quick_sight_analysis_filter_groups: Optional[set[str]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis_filter_groups = (
-            quick_sight_analysis_filter_groups
-        )
-
-    @property
-    def quick_sight_analysis_visuals(self) -> Optional[list[QuickSightAnalysisVisual]]:
-        return self.attributes.quick_sight_analysis_visuals
-
-    @quick_sight_analysis_visuals.setter
-    def quick_sight_analysis_visuals(
-        self, quick_sight_analysis_visuals: Optional[list[QuickSightAnalysisVisual]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis_visuals = quick_sight_analysis_visuals
-
-    @property
-    def quick_sight_analysis_folders(self) -> Optional[list[QuickSightFolder]]:
-        return self.attributes.quick_sight_analysis_folders
-
-    @quick_sight_analysis_folders.setter
-    def quick_sight_analysis_folders(
-        self, quick_sight_analysis_folders: Optional[list[QuickSightFolder]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis_folders = quick_sight_analysis_folders
-
-    type_name: str = Field("QuickSightAnalysis", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightAnalysis":
-            raise ValueError("must be QuickSightAnalysis")
-        return v
-
-    class Attributes(QuickSight.Attributes):
-        quick_sight_analysis_status: Optional[QuickSightAnalysisStatus] = Field(
-            None, description="", alias="quickSightAnalysisStatus"
-        )
-        quick_sight_analysis_calculated_fields: Optional[set[str]] = Field(
-            None, description="", alias="quickSightAnalysisCalculatedFields"
-        )
-        quick_sight_analysis_parameter_declarations: Optional[set[str]] = Field(
-            None, description="", alias="quickSightAnalysisParameterDeclarations"
-        )
-        quick_sight_analysis_filter_groups: Optional[set[str]] = Field(
-            None, description="", alias="quickSightAnalysisFilterGroups"
-        )
-        quick_sight_analysis_visuals: Optional[list[QuickSightAnalysisVisual]] = Field(
-            None, description="", alias="quickSightAnalysisVisuals"
-        )  # relationship
-        quick_sight_analysis_folders: Optional[list[QuickSightFolder]] = Field(
-            None, description="", alias="quickSightAnalysisFolders"
-        )  # relationship
-
-    attributes: "QuickSightAnalysis.Attributes" = Field(
-        default_factory=lambda: QuickSightAnalysis.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class QuickSightAnalysisVisual(QuickSight):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in QuickSightAnalysisVisual._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "quick_sight_analysis_qualified_name",
-        "quick_sight_analysis",
-    ]
-
-    @property
-    def quick_sight_analysis_qualified_name(self) -> Optional[str]:
-        return self.attributes.quick_sight_analysis_qualified_name
-
-    @quick_sight_analysis_qualified_name.setter
-    def quick_sight_analysis_qualified_name(
-        self, quick_sight_analysis_qualified_name: Optional[str]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis_qualified_name = (
-            quick_sight_analysis_qualified_name
-        )
-
-    @property
-    def quick_sight_analysis(self) -> Optional[QuickSightAnalysis]:
-        return self.attributes.quick_sight_analysis
-
-    @quick_sight_analysis.setter
-    def quick_sight_analysis(self, quick_sight_analysis: Optional[QuickSightAnalysis]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_analysis = quick_sight_analysis
-
-    type_name: str = Field("QuickSightAnalysisVisual", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightAnalysisVisual":
-            raise ValueError("must be QuickSightAnalysisVisual")
-        return v
-
-    class Attributes(QuickSight.Attributes):
-        quick_sight_analysis_qualified_name: Optional[str] = Field(
-            None, description="", alias="quickSightAnalysisQualifiedName"
-        )
-        quick_sight_analysis: Optional[QuickSightAnalysis] = Field(
-            None, description="", alias="quickSightAnalysis"
-        )  # relationship
-
-    attributes: "QuickSightAnalysisVisual.Attributes" = Field(
-        default_factory=lambda: QuickSightAnalysisVisual.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class QuickSightDatasetField(QuickSight):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in QuickSightDatasetField._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "quick_sight_dataset_field_type",
-        "quick_sight_dataset_qualified_name",
-        "quick_sight_dataset",
-    ]
-
-    @property
-    def quick_sight_dataset_field_type(self) -> Optional[QuickSightDatasetFieldType]:
-        return self.attributes.quick_sight_dataset_field_type
-
-    @quick_sight_dataset_field_type.setter
-    def quick_sight_dataset_field_type(
-        self, quick_sight_dataset_field_type: Optional[QuickSightDatasetFieldType]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dataset_field_type = quick_sight_dataset_field_type
-
-    @property
-    def quick_sight_dataset_qualified_name(self) -> Optional[str]:
-        return self.attributes.quick_sight_dataset_qualified_name
-
-    @quick_sight_dataset_qualified_name.setter
-    def quick_sight_dataset_qualified_name(
-        self, quick_sight_dataset_qualified_name: Optional[str]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dataset_qualified_name = (
-            quick_sight_dataset_qualified_name
-        )
-
-    @property
-    def quick_sight_dataset(self) -> Optional[QuickSightDataset]:
-        return self.attributes.quick_sight_dataset
-
-    @quick_sight_dataset.setter
-    def quick_sight_dataset(self, quick_sight_dataset: Optional[QuickSightDataset]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dataset = quick_sight_dataset
-
-    type_name: str = Field("QuickSightDatasetField", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightDatasetField":
-            raise ValueError("must be QuickSightDatasetField")
-        return v
-
-    class Attributes(QuickSight.Attributes):
-        quick_sight_dataset_field_type: Optional[QuickSightDatasetFieldType] = Field(
-            None, description="", alias="quickSightDatasetFieldType"
-        )
-        quick_sight_dataset_qualified_name: Optional[str] = Field(
-            None, description="", alias="quickSightDatasetQualifiedName"
-        )
-        quick_sight_dataset: Optional[QuickSightDataset] = Field(
-            None, description="", alias="quickSightDataset"
-        )  # relationship
-
-    attributes: "QuickSightDatasetField.Attributes" = Field(
-        default_factory=lambda: QuickSightDatasetField.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class QuickSightDashboard(QuickSight):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in QuickSightDashboard._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "quick_sight_dashboard_published_version_number",
-        "quick_sight_dashboard_last_published_time",
-        "quick_sight_dashboard_folders",
-        "quick_sight_dashboard_visuals",
-    ]
-
-    @property
-    def quick_sight_dashboard_published_version_number(self) -> Optional[int]:
-        return self.attributes.quick_sight_dashboard_published_version_number
-
-    @quick_sight_dashboard_published_version_number.setter
-    def quick_sight_dashboard_published_version_number(
-        self, quick_sight_dashboard_published_version_number: Optional[int]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dashboard_published_version_number = (
-            quick_sight_dashboard_published_version_number
-        )
-
-    @property
-    def quick_sight_dashboard_last_published_time(self) -> Optional[datetime]:
-        return self.attributes.quick_sight_dashboard_last_published_time
-
-    @quick_sight_dashboard_last_published_time.setter
-    def quick_sight_dashboard_last_published_time(
-        self, quick_sight_dashboard_last_published_time: Optional[datetime]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dashboard_last_published_time = (
-            quick_sight_dashboard_last_published_time
-        )
-
-    @property
-    def quick_sight_dashboard_folders(self) -> Optional[list[QuickSightFolder]]:
-        return self.attributes.quick_sight_dashboard_folders
-
-    @quick_sight_dashboard_folders.setter
-    def quick_sight_dashboard_folders(
-        self, quick_sight_dashboard_folders: Optional[list[QuickSightFolder]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dashboard_folders = quick_sight_dashboard_folders
-
-    @property
-    def quick_sight_dashboard_visuals(
-        self,
-    ) -> Optional[list[QuickSightDashboardVisual]]:
-        return self.attributes.quick_sight_dashboard_visuals
-
-    @quick_sight_dashboard_visuals.setter
-    def quick_sight_dashboard_visuals(
-        self, quick_sight_dashboard_visuals: Optional[list[QuickSightDashboardVisual]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dashboard_visuals = quick_sight_dashboard_visuals
-
-    type_name: str = Field("QuickSightDashboard", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightDashboard":
-            raise ValueError("must be QuickSightDashboard")
-        return v
-
-    class Attributes(QuickSight.Attributes):
-        quick_sight_dashboard_published_version_number: Optional[int] = Field(
-            None, description="", alias="quickSightDashboardPublishedVersionNumber"
-        )
-        quick_sight_dashboard_last_published_time: Optional[datetime] = Field(
-            None, description="", alias="quickSightDashboardLastPublishedTime"
-        )
-        quick_sight_dashboard_folders: Optional[list[QuickSightFolder]] = Field(
-            None, description="", alias="quickSightDashboardFolders"
-        )  # relationship
-        quick_sight_dashboard_visuals: Optional[
-            list[QuickSightDashboardVisual]
-        ] = Field(
-            None, description="", alias="quickSightDashboardVisuals"
-        )  # relationship
-
-    attributes: "QuickSightDashboard.Attributes" = Field(
-        default_factory=lambda: QuickSightDashboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class QuickSightDataset(QuickSight):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in QuickSightDataset._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "quick_sight_dataset_import_mode",
-        "quick_sight_dataset_column_count",
-        "quick_sight_dataset_folders",
-        "quick_sight_dataset_fields",
-    ]
-
-    @property
-    def quick_sight_dataset_import_mode(self) -> Optional[QuickSightDatasetImportMode]:
-        return self.attributes.quick_sight_dataset_import_mode
-
-    @quick_sight_dataset_import_mode.setter
-    def quick_sight_dataset_import_mode(
-        self, quick_sight_dataset_import_mode: Optional[QuickSightDatasetImportMode]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dataset_import_mode = (
-            quick_sight_dataset_import_mode
-        )
-
-    @property
-    def quick_sight_dataset_column_count(self) -> Optional[int]:
-        return self.attributes.quick_sight_dataset_column_count
-
-    @quick_sight_dataset_column_count.setter
-    def quick_sight_dataset_column_count(
-        self, quick_sight_dataset_column_count: Optional[int]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dataset_column_count = (
-            quick_sight_dataset_column_count
-        )
-
-    @property
-    def quick_sight_dataset_folders(self) -> Optional[list[QuickSightFolder]]:
-        return self.attributes.quick_sight_dataset_folders
-
-    @quick_sight_dataset_folders.setter
-    def quick_sight_dataset_folders(
-        self, quick_sight_dataset_folders: Optional[list[QuickSightFolder]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dataset_folders = quick_sight_dataset_folders
-
-    @property
-    def quick_sight_dataset_fields(self) -> Optional[list[QuickSightDatasetField]]:
-        return self.attributes.quick_sight_dataset_fields
-
-    @quick_sight_dataset_fields.setter
-    def quick_sight_dataset_fields(
-        self, quick_sight_dataset_fields: Optional[list[QuickSightDatasetField]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.quick_sight_dataset_fields = quick_sight_dataset_fields
-
-    type_name: str = Field("QuickSightDataset", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "QuickSightDataset":
-            raise ValueError("must be QuickSightDataset")
-        return v
-
-    class Attributes(QuickSight.Attributes):
-        quick_sight_dataset_import_mode: Optional[QuickSightDatasetImportMode] = Field(
-            None, description="", alias="quickSightDatasetImportMode"
-        )
-        quick_sight_dataset_column_count: Optional[int] = Field(
-            None, description="", alias="quickSightDatasetColumnCount"
-        )
-        quick_sight_dataset_folders: Optional[list[QuickSightFolder]] = Field(
-            None, description="", alias="quickSightDatasetFolders"
-        )  # relationship
-        quick_sight_dataset_fields: Optional[list[QuickSightDatasetField]] = Field(
-            None, description="", alias="quickSightDatasetFields"
-        )  # relationship
-
-    attributes: "QuickSightDataset.Attributes" = Field(
-        default_factory=lambda: QuickSightDataset.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class ThoughtspotLiveboard(Thoughtspot):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in ThoughtspotLiveboard._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "thoughtspot_dashlets",
-    ]
-
-    @property
-    def thoughtspot_dashlets(self) -> Optional[list[ThoughtspotDashlet]]:
-        return self.attributes.thoughtspot_dashlets
-
-    @thoughtspot_dashlets.setter
-    def thoughtspot_dashlets(
-        self, thoughtspot_dashlets: Optional[list[ThoughtspotDashlet]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.thoughtspot_dashlets = thoughtspot_dashlets
-
-    type_name: str = Field("ThoughtspotLiveboard", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ThoughtspotLiveboard":
-            raise ValueError("must be ThoughtspotLiveboard")
-        return v
-
-    class Attributes(Thoughtspot.Attributes):
-        thoughtspot_dashlets: Optional[list[ThoughtspotDashlet]] = Field(
-            None, description="", alias="thoughtspotDashlets"
-        )  # relationship
-
-    attributes: "ThoughtspotLiveboard.Attributes" = Field(
-        default_factory=lambda: ThoughtspotLiveboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class ThoughtspotDashlet(Thoughtspot):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in ThoughtspotDashlet._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "thoughtspot_liveboard_name",
-        "thoughtspot_liveboard_qualified_name",
-        "thoughtspot_liveboard",
-    ]
-
-    @property
-    def thoughtspot_liveboard_name(self) -> Optional[str]:
-        return self.attributes.thoughtspot_liveboard_name
-
-    @thoughtspot_liveboard_name.setter
-    def thoughtspot_liveboard_name(self, thoughtspot_liveboard_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.thoughtspot_liveboard_name = thoughtspot_liveboard_name
-
-    @property
-    def thoughtspot_liveboard_qualified_name(self) -> Optional[str]:
-        return self.attributes.thoughtspot_liveboard_qualified_name
-
-    @thoughtspot_liveboard_qualified_name.setter
-    def thoughtspot_liveboard_qualified_name(
-        self, thoughtspot_liveboard_qualified_name: Optional[str]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.thoughtspot_liveboard_qualified_name = (
-            thoughtspot_liveboard_qualified_name
-        )
-
-    @property
-    def thoughtspot_liveboard(self) -> Optional[ThoughtspotLiveboard]:
-        return self.attributes.thoughtspot_liveboard
-
-    @thoughtspot_liveboard.setter
-    def thoughtspot_liveboard(
-        self, thoughtspot_liveboard: Optional[ThoughtspotLiveboard]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.thoughtspot_liveboard = thoughtspot_liveboard
-
-    type_name: str = Field("ThoughtspotDashlet", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ThoughtspotDashlet":
-            raise ValueError("must be ThoughtspotDashlet")
-        return v
-
-    class Attributes(Thoughtspot.Attributes):
-        thoughtspot_liveboard_name: Optional[str] = Field(
-            None, description="", alias="thoughtspotLiveboardName"
-        )
-        thoughtspot_liveboard_qualified_name: Optional[str] = Field(
-            None, description="", alias="thoughtspotLiveboardQualifiedName"
-        )
-        thoughtspot_liveboard: Optional[ThoughtspotLiveboard] = Field(
-            None, description="", alias="thoughtspotLiveboard"
-        )  # relationship
-
-    attributes: "ThoughtspotDashlet.Attributes" = Field(
-        default_factory=lambda: ThoughtspotDashlet.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class ThoughtspotAnswer(Thoughtspot):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in ThoughtspotAnswer._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = []
-
-    type_name: str = Field("ThoughtspotAnswer", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "ThoughtspotAnswer":
-            raise ValueError("must be ThoughtspotAnswer")
-        return v
-
-
-class PowerBIReport(PowerBI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in PowerBIReport._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "workspace_qualified_name",
-        "dataset_qualified_name",
-        "web_url",
-        "page_count",
-        "workspace",
-        "tiles",
-        "pages",
-        "dataset",
-    ]
-
-    @property
-    def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
-
-    @workspace_qualified_name.setter
-    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace_qualified_name = workspace_qualified_name
-
-    @property
-    def dataset_qualified_name(self) -> Optional[str]:
-        return self.attributes.dataset_qualified_name
-
-    @dataset_qualified_name.setter
-    def dataset_qualified_name(self, dataset_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dataset_qualified_name = dataset_qualified_name
-
-    @property
-    def web_url(self) -> Optional[str]:
-        return self.attributes.web_url
-
-    @web_url.setter
-    def web_url(self, web_url: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.web_url = web_url
-
-    @property
-    def page_count(self) -> Optional[int]:
-        return self.attributes.page_count
-
-    @page_count.setter
-    def page_count(self, page_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.page_count = page_count
-
-    @property
-    def workspace(self) -> Optional[PowerBIWorkspace]:
-        return self.attributes.workspace
-
-    @workspace.setter
-    def workspace(self, workspace: Optional[PowerBIWorkspace]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace = workspace
-
-    @property
-    def tiles(self) -> Optional[list[PowerBITile]]:
-        return self.attributes.tiles
-
-    @tiles.setter
-    def tiles(self, tiles: Optional[list[PowerBITile]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.tiles = tiles
-
-    @property
-    def pages(self) -> Optional[list[PowerBIPage]]:
-        return self.attributes.pages
-
-    @pages.setter
-    def pages(self, pages: Optional[list[PowerBIPage]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.pages = pages
-
-    @property
-    def dataset(self) -> Optional[PowerBIDataset]:
-        return self.attributes.dataset
-
-    @dataset.setter
-    def dataset(self, dataset: Optional[PowerBIDataset]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dataset = dataset
-
-    type_name: str = Field("PowerBIReport", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIReport":
-            raise ValueError("must be PowerBIReport")
-        return v
-
-    class Attributes(PowerBI.Attributes):
-        workspace_qualified_name: Optional[str] = Field(
-            None, description="", alias="workspaceQualifiedName"
-        )
-        dataset_qualified_name: Optional[str] = Field(
-            None, description="", alias="datasetQualifiedName"
-        )
-        web_url: Optional[str] = Field(None, description="", alias="webUrl")
-        page_count: Optional[int] = Field(None, description="", alias="pageCount")
-        workspace: Optional[PowerBIWorkspace] = Field(
-            None, description="", alias="workspace"
-        )  # relationship
-        tiles: Optional[list[PowerBITile]] = Field(
-            None, description="", alias="tiles"
-        )  # relationship
-        pages: Optional[list[PowerBIPage]] = Field(
-            None, description="", alias="pages"
-        )  # relationship
-        dataset: Optional[PowerBIDataset] = Field(
-            None, description="", alias="dataset"
-        )  # relationship
-
-    attributes: "PowerBIReport.Attributes" = Field(
-        default_factory=lambda: PowerBIReport.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class PowerBIMeasure(PowerBI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in PowerBIMeasure._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "workspace_qualified_name",
-        "dataset_qualified_name",
-        "power_b_i_measure_expression",
-        "power_b_i_is_external_measure",
-        "table",
-    ]
-
-    @property
-    def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
-
-    @workspace_qualified_name.setter
-    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace_qualified_name = workspace_qualified_name
-
-    @property
-    def dataset_qualified_name(self) -> Optional[str]:
-        return self.attributes.dataset_qualified_name
-
-    @dataset_qualified_name.setter
-    def dataset_qualified_name(self, dataset_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dataset_qualified_name = dataset_qualified_name
-
-    @property
-    def power_b_i_measure_expression(self) -> Optional[str]:
-        return self.attributes.power_b_i_measure_expression
-
-    @power_b_i_measure_expression.setter
-    def power_b_i_measure_expression(self, power_b_i_measure_expression: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.power_b_i_measure_expression = power_b_i_measure_expression
-
-    @property
-    def power_b_i_is_external_measure(self) -> Optional[bool]:
-        return self.attributes.power_b_i_is_external_measure
-
-    @power_b_i_is_external_measure.setter
-    def power_b_i_is_external_measure(
-        self, power_b_i_is_external_measure: Optional[bool]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.power_b_i_is_external_measure = power_b_i_is_external_measure
-
-    @property
-    def table(self) -> Optional[PowerBITable]:
-        return self.attributes.table
-
-    @table.setter
-    def table(self, table: Optional[PowerBITable]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.table = table
-
-    type_name: str = Field("PowerBIMeasure", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIMeasure":
-            raise ValueError("must be PowerBIMeasure")
-        return v
-
-    class Attributes(PowerBI.Attributes):
-        workspace_qualified_name: Optional[str] = Field(
-            None, description="", alias="workspaceQualifiedName"
-        )
-        dataset_qualified_name: Optional[str] = Field(
-            None, description="", alias="datasetQualifiedName"
-        )
-        power_b_i_measure_expression: Optional[str] = Field(
-            None, description="", alias="powerBIMeasureExpression"
-        )
-        power_b_i_is_external_measure: Optional[bool] = Field(
-            None, description="", alias="powerBIIsExternalMeasure"
-        )
-        table: Optional[PowerBITable] = Field(
-            None, description="", alias="table"
-        )  # relationship
-
-    attributes: "PowerBIMeasure.Attributes" = Field(
-        default_factory=lambda: PowerBIMeasure.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class PowerBIColumn(PowerBI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in PowerBIColumn._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "workspace_qualified_name",
-        "dataset_qualified_name",
-        "power_b_i_column_data_category",
-        "power_b_i_column_data_type",
-        "power_b_i_sort_by_column",
-        "power_b_i_column_summarize_by",
-        "table",
-    ]
-
-    @property
-    def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
-
-    @workspace_qualified_name.setter
-    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace_qualified_name = workspace_qualified_name
-
-    @property
-    def dataset_qualified_name(self) -> Optional[str]:
-        return self.attributes.dataset_qualified_name
-
-    @dataset_qualified_name.setter
-    def dataset_qualified_name(self, dataset_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dataset_qualified_name = dataset_qualified_name
-
-    @property
-    def power_b_i_column_data_category(self) -> Optional[str]:
-        return self.attributes.power_b_i_column_data_category
-
-    @power_b_i_column_data_category.setter
-    def power_b_i_column_data_category(
-        self, power_b_i_column_data_category: Optional[str]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.power_b_i_column_data_category = power_b_i_column_data_category
-
-    @property
-    def power_b_i_column_data_type(self) -> Optional[str]:
-        return self.attributes.power_b_i_column_data_type
-
-    @power_b_i_column_data_type.setter
-    def power_b_i_column_data_type(self, power_b_i_column_data_type: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.power_b_i_column_data_type = power_b_i_column_data_type
-
-    @property
-    def power_b_i_sort_by_column(self) -> Optional[str]:
-        return self.attributes.power_b_i_sort_by_column
-
-    @power_b_i_sort_by_column.setter
-    def power_b_i_sort_by_column(self, power_b_i_sort_by_column: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.power_b_i_sort_by_column = power_b_i_sort_by_column
-
-    @property
-    def power_b_i_column_summarize_by(self) -> Optional[str]:
-        return self.attributes.power_b_i_column_summarize_by
-
-    @power_b_i_column_summarize_by.setter
-    def power_b_i_column_summarize_by(
-        self, power_b_i_column_summarize_by: Optional[str]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.power_b_i_column_summarize_by = power_b_i_column_summarize_by
-
-    @property
-    def table(self) -> Optional[PowerBITable]:
-        return self.attributes.table
-
-    @table.setter
-    def table(self, table: Optional[PowerBITable]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.table = table
-
-    type_name: str = Field("PowerBIColumn", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIColumn":
-            raise ValueError("must be PowerBIColumn")
-        return v
-
-    class Attributes(PowerBI.Attributes):
-        workspace_qualified_name: Optional[str] = Field(
-            None, description="", alias="workspaceQualifiedName"
-        )
-        dataset_qualified_name: Optional[str] = Field(
-            None, description="", alias="datasetQualifiedName"
-        )
-        power_b_i_column_data_category: Optional[str] = Field(
-            None, description="", alias="powerBIColumnDataCategory"
-        )
-        power_b_i_column_data_type: Optional[str] = Field(
-            None, description="", alias="powerBIColumnDataType"
-        )
-        power_b_i_sort_by_column: Optional[str] = Field(
-            None, description="", alias="powerBISortByColumn"
-        )
-        power_b_i_column_summarize_by: Optional[str] = Field(
-            None, description="", alias="powerBIColumnSummarizeBy"
-        )
-        table: Optional[PowerBITable] = Field(
-            None, description="", alias="table"
-        )  # relationship
-
-    attributes: "PowerBIColumn.Attributes" = Field(
-        default_factory=lambda: PowerBIColumn.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class PowerBITile(PowerBI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in PowerBITile._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "workspace_qualified_name",
-        "dashboard_qualified_name",
-        "report",
-        "dataset",
-        "dashboard",
-    ]
-
-    @property
-    def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
-
-    @workspace_qualified_name.setter
-    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace_qualified_name = workspace_qualified_name
-
-    @property
-    def dashboard_qualified_name(self) -> Optional[str]:
-        return self.attributes.dashboard_qualified_name
-
-    @dashboard_qualified_name.setter
-    def dashboard_qualified_name(self, dashboard_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dashboard_qualified_name = dashboard_qualified_name
-
-    @property
-    def report(self) -> Optional[PowerBIReport]:
-        return self.attributes.report
-
-    @report.setter
-    def report(self, report: Optional[PowerBIReport]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.report = report
-
-    @property
-    def dataset(self) -> Optional[PowerBIDataset]:
-        return self.attributes.dataset
-
-    @dataset.setter
-    def dataset(self, dataset: Optional[PowerBIDataset]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dataset = dataset
-
-    @property
-    def dashboard(self) -> Optional[PowerBIDashboard]:
-        return self.attributes.dashboard
-
-    @dashboard.setter
-    def dashboard(self, dashboard: Optional[PowerBIDashboard]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dashboard = dashboard
-
-    type_name: str = Field("PowerBITile", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBITile":
-            raise ValueError("must be PowerBITile")
-        return v
-
-    class Attributes(PowerBI.Attributes):
-        workspace_qualified_name: Optional[str] = Field(
-            None, description="", alias="workspaceQualifiedName"
-        )
-        dashboard_qualified_name: Optional[str] = Field(
-            None, description="", alias="dashboardQualifiedName"
-        )
-        report: Optional[PowerBIReport] = Field(
-            None, description="", alias="report"
-        )  # relationship
-        dataset: Optional[PowerBIDataset] = Field(
-            None, description="", alias="dataset"
-        )  # relationship
-        dashboard: Optional[PowerBIDashboard] = Field(
-            None, description="", alias="dashboard"
-        )  # relationship
-
-    attributes: "PowerBITile.Attributes" = Field(
-        default_factory=lambda: PowerBITile.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class PowerBITable(PowerBI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in PowerBITable._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "workspace_qualified_name",
-        "dataset_qualified_name",
-        "power_b_i_table_source_expressions",
-        "power_b_i_table_column_count",
-        "power_b_i_table_measure_count",
-        "measures",
-        "columns",
-        "dataset",
-    ]
-
-    @property
-    def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
-
-    @workspace_qualified_name.setter
-    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace_qualified_name = workspace_qualified_name
-
-    @property
-    def dataset_qualified_name(self) -> Optional[str]:
-        return self.attributes.dataset_qualified_name
-
-    @dataset_qualified_name.setter
-    def dataset_qualified_name(self, dataset_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dataset_qualified_name = dataset_qualified_name
-
-    @property
-    def power_b_i_table_source_expressions(self) -> Optional[set[str]]:
-        return self.attributes.power_b_i_table_source_expressions
-
-    @power_b_i_table_source_expressions.setter
-    def power_b_i_table_source_expressions(
-        self, power_b_i_table_source_expressions: Optional[set[str]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.power_b_i_table_source_expressions = (
-            power_b_i_table_source_expressions
-        )
-
-    @property
-    def power_b_i_table_column_count(self) -> Optional[int]:
-        return self.attributes.power_b_i_table_column_count
-
-    @power_b_i_table_column_count.setter
-    def power_b_i_table_column_count(self, power_b_i_table_column_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.power_b_i_table_column_count = power_b_i_table_column_count
-
-    @property
-    def power_b_i_table_measure_count(self) -> Optional[int]:
-        return self.attributes.power_b_i_table_measure_count
-
-    @power_b_i_table_measure_count.setter
-    def power_b_i_table_measure_count(
-        self, power_b_i_table_measure_count: Optional[int]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.power_b_i_table_measure_count = power_b_i_table_measure_count
-
-    @property
-    def measures(self) -> Optional[list[PowerBIMeasure]]:
-        return self.attributes.measures
-
-    @measures.setter
-    def measures(self, measures: Optional[list[PowerBIMeasure]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.measures = measures
-
-    @property
-    def columns(self) -> Optional[list[PowerBIColumn]]:
-        return self.attributes.columns
-
-    @columns.setter
-    def columns(self, columns: Optional[list[PowerBIColumn]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.columns = columns
-
-    @property
-    def dataset(self) -> Optional[PowerBIDataset]:
-        return self.attributes.dataset
-
-    @dataset.setter
-    def dataset(self, dataset: Optional[PowerBIDataset]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dataset = dataset
-
-    type_name: str = Field("PowerBITable", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBITable":
-            raise ValueError("must be PowerBITable")
-        return v
-
-    class Attributes(PowerBI.Attributes):
-        workspace_qualified_name: Optional[str] = Field(
-            None, description="", alias="workspaceQualifiedName"
-        )
-        dataset_qualified_name: Optional[str] = Field(
-            None, description="", alias="datasetQualifiedName"
-        )
-        power_b_i_table_source_expressions: Optional[set[str]] = Field(
-            None, description="", alias="powerBITableSourceExpressions"
-        )
-        power_b_i_table_column_count: Optional[int] = Field(
-            None, description="", alias="powerBITableColumnCount"
-        )
-        power_b_i_table_measure_count: Optional[int] = Field(
-            None, description="", alias="powerBITableMeasureCount"
-        )
-        measures: Optional[list[PowerBIMeasure]] = Field(
-            None, description="", alias="measures"
-        )  # relationship
-        columns: Optional[list[PowerBIColumn]] = Field(
-            None, description="", alias="columns"
-        )  # relationship
-        dataset: Optional[PowerBIDataset] = Field(
-            None, description="", alias="dataset"
-        )  # relationship
-
-    attributes: "PowerBITable.Attributes" = Field(
-        default_factory=lambda: PowerBITable.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class PowerBIDatasource(PowerBI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in PowerBIDatasource._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "connection_details",
-        "datasets",
-    ]
-
-    @property
-    def connection_details(self) -> Optional[dict[str, str]]:
-        return self.attributes.connection_details
-
-    @connection_details.setter
-    def connection_details(self, connection_details: Optional[dict[str, str]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.connection_details = connection_details
-
-    @property
-    def datasets(self) -> Optional[list[PowerBIDataset]]:
-        return self.attributes.datasets
-
-    @datasets.setter
-    def datasets(self, datasets: Optional[list[PowerBIDataset]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.datasets = datasets
-
-    type_name: str = Field("PowerBIDatasource", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIDatasource":
-            raise ValueError("must be PowerBIDatasource")
-        return v
-
-    class Attributes(PowerBI.Attributes):
-        connection_details: Optional[dict[str, str]] = Field(
-            None, description="", alias="connectionDetails"
-        )
-        datasets: Optional[list[PowerBIDataset]] = Field(
-            None, description="", alias="datasets"
-        )  # relationship
-
-    attributes: "PowerBIDatasource.Attributes" = Field(
-        default_factory=lambda: PowerBIDatasource.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class PowerBIWorkspace(PowerBI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in PowerBIWorkspace._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "web_url",
-        "report_count",
-        "dashboard_count",
-        "dataset_count",
-        "dataflow_count",
-        "reports",
-        "datasets",
-        "dashboards",
-        "dataflows",
-    ]
-
-    @property
-    def web_url(self) -> Optional[str]:
-        return self.attributes.web_url
-
-    @web_url.setter
-    def web_url(self, web_url: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.web_url = web_url
-
-    @property
-    def report_count(self) -> Optional[int]:
-        return self.attributes.report_count
-
-    @report_count.setter
-    def report_count(self, report_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.report_count = report_count
-
-    @property
-    def dashboard_count(self) -> Optional[int]:
-        return self.attributes.dashboard_count
-
-    @dashboard_count.setter
-    def dashboard_count(self, dashboard_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dashboard_count = dashboard_count
-
-    @property
-    def dataset_count(self) -> Optional[int]:
-        return self.attributes.dataset_count
-
-    @dataset_count.setter
-    def dataset_count(self, dataset_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dataset_count = dataset_count
-
-    @property
-    def dataflow_count(self) -> Optional[int]:
-        return self.attributes.dataflow_count
-
-    @dataflow_count.setter
-    def dataflow_count(self, dataflow_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dataflow_count = dataflow_count
-
-    @property
-    def reports(self) -> Optional[list[PowerBIReport]]:
-        return self.attributes.reports
-
-    @reports.setter
-    def reports(self, reports: Optional[list[PowerBIReport]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.reports = reports
-
-    @property
-    def datasets(self) -> Optional[list[PowerBIDataset]]:
-        return self.attributes.datasets
-
-    @datasets.setter
-    def datasets(self, datasets: Optional[list[PowerBIDataset]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.datasets = datasets
-
-    @property
-    def dashboards(self) -> Optional[list[PowerBIDashboard]]:
-        return self.attributes.dashboards
-
-    @dashboards.setter
-    def dashboards(self, dashboards: Optional[list[PowerBIDashboard]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dashboards = dashboards
-
-    @property
-    def dataflows(self) -> Optional[list[PowerBIDataflow]]:
-        return self.attributes.dataflows
-
-    @dataflows.setter
-    def dataflows(self, dataflows: Optional[list[PowerBIDataflow]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dataflows = dataflows
-
-    type_name: str = Field("PowerBIWorkspace", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIWorkspace":
-            raise ValueError("must be PowerBIWorkspace")
-        return v
-
-    class Attributes(PowerBI.Attributes):
-        web_url: Optional[str] = Field(None, description="", alias="webUrl")
-        report_count: Optional[int] = Field(None, description="", alias="reportCount")
-        dashboard_count: Optional[int] = Field(
-            None, description="", alias="dashboardCount"
-        )
-        dataset_count: Optional[int] = Field(None, description="", alias="datasetCount")
-        dataflow_count: Optional[int] = Field(
-            None, description="", alias="dataflowCount"
-        )
-        reports: Optional[list[PowerBIReport]] = Field(
-            None, description="", alias="reports"
-        )  # relationship
-        datasets: Optional[list[PowerBIDataset]] = Field(
-            None, description="", alias="datasets"
-        )  # relationship
-        dashboards: Optional[list[PowerBIDashboard]] = Field(
-            None, description="", alias="dashboards"
-        )  # relationship
-        dataflows: Optional[list[PowerBIDataflow]] = Field(
-            None, description="", alias="dataflows"
-        )  # relationship
-
-    attributes: "PowerBIWorkspace.Attributes" = Field(
-        default_factory=lambda: PowerBIWorkspace.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class PowerBIDataset(PowerBI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in PowerBIDataset._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "workspace_qualified_name",
-        "web_url",
-        "reports",
-        "workspace",
-        "dataflows",
-        "tiles",
-        "tables",
-        "datasources",
-    ]
-
-    @property
-    def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
-
-    @workspace_qualified_name.setter
-    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace_qualified_name = workspace_qualified_name
-
-    @property
-    def web_url(self) -> Optional[str]:
-        return self.attributes.web_url
-
-    @web_url.setter
-    def web_url(self, web_url: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.web_url = web_url
-
-    @property
-    def reports(self) -> Optional[list[PowerBIReport]]:
-        return self.attributes.reports
-
-    @reports.setter
-    def reports(self, reports: Optional[list[PowerBIReport]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.reports = reports
-
-    @property
-    def workspace(self) -> Optional[PowerBIWorkspace]:
-        return self.attributes.workspace
-
-    @workspace.setter
-    def workspace(self, workspace: Optional[PowerBIWorkspace]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace = workspace
-
-    @property
-    def dataflows(self) -> Optional[list[PowerBIDataflow]]:
-        return self.attributes.dataflows
-
-    @dataflows.setter
-    def dataflows(self, dataflows: Optional[list[PowerBIDataflow]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.dataflows = dataflows
-
-    @property
-    def tiles(self) -> Optional[list[PowerBITile]]:
-        return self.attributes.tiles
-
-    @tiles.setter
-    def tiles(self, tiles: Optional[list[PowerBITile]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.tiles = tiles
-
-    @property
-    def tables(self) -> Optional[list[PowerBITable]]:
-        return self.attributes.tables
-
-    @tables.setter
-    def tables(self, tables: Optional[list[PowerBITable]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.tables = tables
-
-    @property
-    def datasources(self) -> Optional[list[PowerBIDatasource]]:
-        return self.attributes.datasources
-
-    @datasources.setter
-    def datasources(self, datasources: Optional[list[PowerBIDatasource]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.datasources = datasources
-
-    type_name: str = Field("PowerBIDataset", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIDataset":
-            raise ValueError("must be PowerBIDataset")
-        return v
-
-    class Attributes(PowerBI.Attributes):
-        workspace_qualified_name: Optional[str] = Field(
-            None, description="", alias="workspaceQualifiedName"
-        )
-        web_url: Optional[str] = Field(None, description="", alias="webUrl")
-        reports: Optional[list[PowerBIReport]] = Field(
-            None, description="", alias="reports"
-        )  # relationship
-        workspace: Optional[PowerBIWorkspace] = Field(
-            None, description="", alias="workspace"
-        )  # relationship
-        dataflows: Optional[list[PowerBIDataflow]] = Field(
-            None, description="", alias="dataflows"
-        )  # relationship
-        tiles: Optional[list[PowerBITile]] = Field(
-            None, description="", alias="tiles"
-        )  # relationship
-        tables: Optional[list[PowerBITable]] = Field(
-            None, description="", alias="tables"
-        )  # relationship
-        datasources: Optional[list[PowerBIDatasource]] = Field(
-            None, description="", alias="datasources"
-        )  # relationship
-
-    attributes: "PowerBIDataset.Attributes" = Field(
-        default_factory=lambda: PowerBIDataset.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class PowerBIDashboard(PowerBI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in PowerBIDashboard._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "workspace_qualified_name",
-        "web_url",
-        "tile_count",
-        "tiles",
-        "workspace",
-    ]
-
-    @property
-    def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
-
-    @workspace_qualified_name.setter
-    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace_qualified_name = workspace_qualified_name
-
-    @property
-    def web_url(self) -> Optional[str]:
-        return self.attributes.web_url
-
-    @web_url.setter
-    def web_url(self, web_url: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.web_url = web_url
-
-    @property
-    def tile_count(self) -> Optional[int]:
-        return self.attributes.tile_count
-
-    @tile_count.setter
-    def tile_count(self, tile_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.tile_count = tile_count
-
-    @property
-    def tiles(self) -> Optional[list[PowerBITile]]:
-        return self.attributes.tiles
-
-    @tiles.setter
-    def tiles(self, tiles: Optional[list[PowerBITile]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.tiles = tiles
-
-    @property
-    def workspace(self) -> Optional[PowerBIWorkspace]:
-        return self.attributes.workspace
-
-    @workspace.setter
-    def workspace(self, workspace: Optional[PowerBIWorkspace]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace = workspace
-
-    type_name: str = Field("PowerBIDashboard", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIDashboard":
-            raise ValueError("must be PowerBIDashboard")
-        return v
-
-    class Attributes(PowerBI.Attributes):
-        workspace_qualified_name: Optional[str] = Field(
-            None, description="", alias="workspaceQualifiedName"
-        )
-        web_url: Optional[str] = Field(None, description="", alias="webUrl")
-        tile_count: Optional[int] = Field(None, description="", alias="tileCount")
-        tiles: Optional[list[PowerBITile]] = Field(
-            None, description="", alias="tiles"
-        )  # relationship
-        workspace: Optional[PowerBIWorkspace] = Field(
-            None, description="", alias="workspace"
-        )  # relationship
-
-    attributes: "PowerBIDashboard.Attributes" = Field(
-        default_factory=lambda: PowerBIDashboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class PowerBIPage(PowerBI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in PowerBIPage._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "workspace_qualified_name",
-        "report_qualified_name",
-        "report",
-    ]
-
-    @property
-    def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
-
-    @workspace_qualified_name.setter
-    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace_qualified_name = workspace_qualified_name
-
-    @property
-    def report_qualified_name(self) -> Optional[str]:
-        return self.attributes.report_qualified_name
-
-    @report_qualified_name.setter
-    def report_qualified_name(self, report_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.report_qualified_name = report_qualified_name
-
-    @property
-    def report(self) -> Optional[PowerBIReport]:
-        return self.attributes.report
-
-    @report.setter
-    def report(self, report: Optional[PowerBIReport]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.report = report
-
-    type_name: str = Field("PowerBIPage", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIPage":
-            raise ValueError("must be PowerBIPage")
-        return v
-
-    class Attributes(PowerBI.Attributes):
-        workspace_qualified_name: Optional[str] = Field(
-            None, description="", alias="workspaceQualifiedName"
-        )
-        report_qualified_name: Optional[str] = Field(
-            None, description="", alias="reportQualifiedName"
-        )
-        report: Optional[PowerBIReport] = Field(
-            None, description="", alias="report"
-        )  # relationship
-
-    attributes: "PowerBIPage.Attributes" = Field(
-        default_factory=lambda: PowerBIPage.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class PowerBIDataflow(PowerBI):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in PowerBIDataflow._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "workspace_qualified_name",
-        "web_url",
-        "workspace",
-        "datasets",
-    ]
-
-    @property
-    def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
-
-    @workspace_qualified_name.setter
-    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace_qualified_name = workspace_qualified_name
-
-    @property
-    def web_url(self) -> Optional[str]:
-        return self.attributes.web_url
-
-    @web_url.setter
-    def web_url(self, web_url: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.web_url = web_url
-
-    @property
-    def workspace(self) -> Optional[PowerBIWorkspace]:
-        return self.attributes.workspace
-
-    @workspace.setter
-    def workspace(self, workspace: Optional[PowerBIWorkspace]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.workspace = workspace
-
-    @property
-    def datasets(self) -> Optional[list[PowerBIDataset]]:
-        return self.attributes.datasets
-
-    @datasets.setter
-    def datasets(self, datasets: Optional[list[PowerBIDataset]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.datasets = datasets
-
-    type_name: str = Field("PowerBIDataflow", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "PowerBIDataflow":
-            raise ValueError("must be PowerBIDataflow")
-        return v
-
-    class Attributes(PowerBI.Attributes):
-        workspace_qualified_name: Optional[str] = Field(
-            None, description="", alias="workspaceQualifiedName"
-        )
-        web_url: Optional[str] = Field(None, description="", alias="webUrl")
-        workspace: Optional[PowerBIWorkspace] = Field(
-            None, description="", alias="workspace"
-        )  # relationship
-        datasets: Optional[list[PowerBIDataset]] = Field(
-            None, description="", alias="datasets"
-        )  # relationship
-
-    attributes: "PowerBIDataflow.Attributes" = Field(
-        default_factory=lambda: PowerBIDataflow.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
 class PresetChart(Preset):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in PresetChart._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -18028,450 +15931,14 @@
     attributes: "PresetWorkspace.Attributes" = Field(
         default_factory=lambda: PresetWorkspace.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class SigmaDatasetColumn(Sigma):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in SigmaDatasetColumn._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "sigma_dataset_qualified_name",
-        "sigma_dataset_name",
-        "sigma_dataset",
-    ]
-
-    @property
-    def sigma_dataset_qualified_name(self) -> Optional[str]:
-        return self.attributes.sigma_dataset_qualified_name
-
-    @sigma_dataset_qualified_name.setter
-    def sigma_dataset_qualified_name(self, sigma_dataset_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_dataset_qualified_name = sigma_dataset_qualified_name
-
-    @property
-    def sigma_dataset_name(self) -> Optional[str]:
-        return self.attributes.sigma_dataset_name
-
-    @sigma_dataset_name.setter
-    def sigma_dataset_name(self, sigma_dataset_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_dataset_name = sigma_dataset_name
-
-    @property
-    def sigma_dataset(self) -> Optional[SigmaDataset]:
-        return self.attributes.sigma_dataset
-
-    @sigma_dataset.setter
-    def sigma_dataset(self, sigma_dataset: Optional[SigmaDataset]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_dataset = sigma_dataset
-
-    type_name: str = Field("SigmaDatasetColumn", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SigmaDatasetColumn":
-            raise ValueError("must be SigmaDatasetColumn")
-        return v
-
-    class Attributes(Sigma.Attributes):
-        sigma_dataset_qualified_name: Optional[str] = Field(
-            None, description="", alias="sigmaDatasetQualifiedName"
-        )
-        sigma_dataset_name: Optional[str] = Field(
-            None, description="", alias="sigmaDatasetName"
-        )
-        sigma_dataset: Optional[SigmaDataset] = Field(
-            None, description="", alias="sigmaDataset"
-        )  # relationship
-
-    attributes: "SigmaDatasetColumn.Attributes" = Field(
-        default_factory=lambda: SigmaDatasetColumn.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class SigmaDataset(Sigma):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in SigmaDataset._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "sigma_dataset_column_count",
-        "sigma_dataset_columns",
-    ]
-
-    @property
-    def sigma_dataset_column_count(self) -> Optional[int]:
-        return self.attributes.sigma_dataset_column_count
-
-    @sigma_dataset_column_count.setter
-    def sigma_dataset_column_count(self, sigma_dataset_column_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_dataset_column_count = sigma_dataset_column_count
-
-    @property
-    def sigma_dataset_columns(self) -> Optional[list[SigmaDatasetColumn]]:
-        return self.attributes.sigma_dataset_columns
-
-    @sigma_dataset_columns.setter
-    def sigma_dataset_columns(
-        self, sigma_dataset_columns: Optional[list[SigmaDatasetColumn]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_dataset_columns = sigma_dataset_columns
-
-    type_name: str = Field("SigmaDataset", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SigmaDataset":
-            raise ValueError("must be SigmaDataset")
-        return v
-
-    class Attributes(Sigma.Attributes):
-        sigma_dataset_column_count: Optional[int] = Field(
-            None, description="", alias="sigmaDatasetColumnCount"
-        )
-        sigma_dataset_columns: Optional[list[SigmaDatasetColumn]] = Field(
-            None, description="", alias="sigmaDatasetColumns"
-        )  # relationship
-
-    attributes: "SigmaDataset.Attributes" = Field(
-        default_factory=lambda: SigmaDataset.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class SigmaWorkbook(Sigma):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in SigmaWorkbook._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "sigma_page_count",
-        "sigma_pages",
-    ]
-
-    @property
-    def sigma_page_count(self) -> Optional[int]:
-        return self.attributes.sigma_page_count
-
-    @sigma_page_count.setter
-    def sigma_page_count(self, sigma_page_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_page_count = sigma_page_count
-
-    @property
-    def sigma_pages(self) -> Optional[list[SigmaPage]]:
-        return self.attributes.sigma_pages
-
-    @sigma_pages.setter
-    def sigma_pages(self, sigma_pages: Optional[list[SigmaPage]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_pages = sigma_pages
-
-    type_name: str = Field("SigmaWorkbook", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SigmaWorkbook":
-            raise ValueError("must be SigmaWorkbook")
-        return v
-
-    class Attributes(Sigma.Attributes):
-        sigma_page_count: Optional[int] = Field(
-            None, description="", alias="sigmaPageCount"
-        )
-        sigma_pages: Optional[list[SigmaPage]] = Field(
-            None, description="", alias="sigmaPages"
-        )  # relationship
-
-    attributes: "SigmaWorkbook.Attributes" = Field(
-        default_factory=lambda: SigmaWorkbook.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class SigmaDataElementField(Sigma):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in SigmaDataElementField._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "sigma_data_element_field_is_hidden",
-        "sigma_data_element_field_formula",
-        "sigma_data_element",
-    ]
-
-    @property
-    def sigma_data_element_field_is_hidden(self) -> Optional[bool]:
-        return self.attributes.sigma_data_element_field_is_hidden
-
-    @sigma_data_element_field_is_hidden.setter
-    def sigma_data_element_field_is_hidden(
-        self, sigma_data_element_field_is_hidden: Optional[bool]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_data_element_field_is_hidden = (
-            sigma_data_element_field_is_hidden
-        )
-
-    @property
-    def sigma_data_element_field_formula(self) -> Optional[str]:
-        return self.attributes.sigma_data_element_field_formula
-
-    @sigma_data_element_field_formula.setter
-    def sigma_data_element_field_formula(
-        self, sigma_data_element_field_formula: Optional[str]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_data_element_field_formula = (
-            sigma_data_element_field_formula
-        )
-
-    @property
-    def sigma_data_element(self) -> Optional[SigmaDataElement]:
-        return self.attributes.sigma_data_element
-
-    @sigma_data_element.setter
-    def sigma_data_element(self, sigma_data_element: Optional[SigmaDataElement]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_data_element = sigma_data_element
-
-    type_name: str = Field("SigmaDataElementField", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SigmaDataElementField":
-            raise ValueError("must be SigmaDataElementField")
-        return v
-
-    class Attributes(Sigma.Attributes):
-        sigma_data_element_field_is_hidden: Optional[bool] = Field(
-            None, description="", alias="sigmaDataElementFieldIsHidden"
-        )
-        sigma_data_element_field_formula: Optional[str] = Field(
-            None, description="", alias="sigmaDataElementFieldFormula"
-        )
-        sigma_data_element: Optional[SigmaDataElement] = Field(
-            None, description="", alias="sigmaDataElement"
-        )  # relationship
-
-    attributes: "SigmaDataElementField.Attributes" = Field(
-        default_factory=lambda: SigmaDataElementField.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class SigmaPage(Sigma):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in SigmaPage._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "sigma_data_element_count",
-        "sigma_data_elements",
-        "sigma_workbook",
-    ]
-
-    @property
-    def sigma_data_element_count(self) -> Optional[int]:
-        return self.attributes.sigma_data_element_count
-
-    @sigma_data_element_count.setter
-    def sigma_data_element_count(self, sigma_data_element_count: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_data_element_count = sigma_data_element_count
-
-    @property
-    def sigma_data_elements(self) -> Optional[list[SigmaDataElement]]:
-        return self.attributes.sigma_data_elements
-
-    @sigma_data_elements.setter
-    def sigma_data_elements(
-        self, sigma_data_elements: Optional[list[SigmaDataElement]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_data_elements = sigma_data_elements
-
-    @property
-    def sigma_workbook(self) -> Optional[SigmaWorkbook]:
-        return self.attributes.sigma_workbook
-
-    @sigma_workbook.setter
-    def sigma_workbook(self, sigma_workbook: Optional[SigmaWorkbook]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_workbook = sigma_workbook
-
-    type_name: str = Field("SigmaPage", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SigmaPage":
-            raise ValueError("must be SigmaPage")
-        return v
-
-    class Attributes(Sigma.Attributes):
-        sigma_data_element_count: Optional[int] = Field(
-            None, description="", alias="sigmaDataElementCount"
-        )
-        sigma_data_elements: Optional[list[SigmaDataElement]] = Field(
-            None, description="", alias="sigmaDataElements"
-        )  # relationship
-        sigma_workbook: Optional[SigmaWorkbook] = Field(
-            None, description="", alias="sigmaWorkbook"
-        )  # relationship
-
-    attributes: "SigmaPage.Attributes" = Field(
-        default_factory=lambda: SigmaPage.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
-class SigmaDataElement(Sigma):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in SigmaDataElement._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "sigma_data_element_query",
-        "sigma_data_element_type",
-        "sigma_data_element_field_count",
-        "sigma_page",
-        "sigma_data_element_fields",
-    ]
-
-    @property
-    def sigma_data_element_query(self) -> Optional[str]:
-        return self.attributes.sigma_data_element_query
-
-    @sigma_data_element_query.setter
-    def sigma_data_element_query(self, sigma_data_element_query: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_data_element_query = sigma_data_element_query
-
-    @property
-    def sigma_data_element_type(self) -> Optional[str]:
-        return self.attributes.sigma_data_element_type
-
-    @sigma_data_element_type.setter
-    def sigma_data_element_type(self, sigma_data_element_type: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_data_element_type = sigma_data_element_type
-
-    @property
-    def sigma_data_element_field_count(self) -> Optional[int]:
-        return self.attributes.sigma_data_element_field_count
-
-    @sigma_data_element_field_count.setter
-    def sigma_data_element_field_count(
-        self, sigma_data_element_field_count: Optional[int]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_data_element_field_count = sigma_data_element_field_count
-
-    @property
-    def sigma_page(self) -> Optional[SigmaPage]:
-        return self.attributes.sigma_page
-
-    @sigma_page.setter
-    def sigma_page(self, sigma_page: Optional[SigmaPage]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_page = sigma_page
-
-    @property
-    def sigma_data_element_fields(self) -> Optional[list[SigmaDataElementField]]:
-        return self.attributes.sigma_data_element_fields
-
-    @sigma_data_element_fields.setter
-    def sigma_data_element_fields(
-        self, sigma_data_element_fields: Optional[list[SigmaDataElementField]]
-    ):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.sigma_data_element_fields = sigma_data_element_fields
-
-    type_name: str = Field("SigmaDataElement", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "SigmaDataElement":
-            raise ValueError("must be SigmaDataElement")
-        return v
-
-    class Attributes(Sigma.Attributes):
-        sigma_data_element_query: Optional[str] = Field(
-            None, description="", alias="sigmaDataElementQuery"
-        )
-        sigma_data_element_type: Optional[str] = Field(
-            None, description="", alias="sigmaDataElementType"
-        )
-        sigma_data_element_field_count: Optional[int] = Field(
-            None, description="", alias="sigmaDataElementFieldCount"
-        )
-        sigma_page: Optional[SigmaPage] = Field(
-            None, description="", alias="sigmaPage"
-        )  # relationship
-        sigma_data_element_fields: Optional[list[SigmaDataElementField]] = Field(
-            None, description="", alias="sigmaDataElementFields"
-        )  # relationship
-
-    attributes: "SigmaDataElement.Attributes" = Field(
-        default_factory=lambda: SigmaDataElement.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
 class ModeReport(Mode):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ModeReport._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -18898,471 +16365,445 @@
     attributes: "ModeCollection.Attributes" = Field(
         default_factory=lambda: ModeCollection.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class QlikSpace(Qlik):
+class SigmaDatasetColumn(Sigma):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in QlikSpace._convience_properties:
+        if name in SigmaDatasetColumn._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "qlik_space_type",
-        "qlik_datasets",
-        "qlik_apps",
+        "sigma_dataset_qualified_name",
+        "sigma_dataset_name",
+        "sigma_dataset",
     ]
 
     @property
-    def qlik_space_type(self) -> Optional[str]:
-        return self.attributes.qlik_space_type
+    def sigma_dataset_qualified_name(self) -> Optional[str]:
+        return self.attributes.sigma_dataset_qualified_name
 
-    @qlik_space_type.setter
-    def qlik_space_type(self, qlik_space_type: Optional[str]):
+    @sigma_dataset_qualified_name.setter
+    def sigma_dataset_qualified_name(self, sigma_dataset_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_space_type = qlik_space_type
+        self.attributes.sigma_dataset_qualified_name = sigma_dataset_qualified_name
 
     @property
-    def qlik_datasets(self) -> Optional[list[QlikDataset]]:
-        return self.attributes.qlik_datasets
+    def sigma_dataset_name(self) -> Optional[str]:
+        return self.attributes.sigma_dataset_name
 
-    @qlik_datasets.setter
-    def qlik_datasets(self, qlik_datasets: Optional[list[QlikDataset]]):
+    @sigma_dataset_name.setter
+    def sigma_dataset_name(self, sigma_dataset_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_datasets = qlik_datasets
+        self.attributes.sigma_dataset_name = sigma_dataset_name
 
     @property
-    def qlik_apps(self) -> Optional[list[QlikApp]]:
-        return self.attributes.qlik_apps
+    def sigma_dataset(self) -> Optional[SigmaDataset]:
+        return self.attributes.sigma_dataset
 
-    @qlik_apps.setter
-    def qlik_apps(self, qlik_apps: Optional[list[QlikApp]]):
+    @sigma_dataset.setter
+    def sigma_dataset(self, sigma_dataset: Optional[SigmaDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_apps = qlik_apps
+        self.attributes.sigma_dataset = sigma_dataset
 
-    type_name: str = Field("QlikSpace", allow_mutation=False)
+    type_name: str = Field("SigmaDatasetColumn", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "QlikSpace":
-            raise ValueError("must be QlikSpace")
+        if v != "SigmaDatasetColumn":
+            raise ValueError("must be SigmaDatasetColumn")
         return v
 
-    class Attributes(Qlik.Attributes):
-        qlik_space_type: Optional[str] = Field(
-            None, description="", alias="qlikSpaceType"
+    class Attributes(Sigma.Attributes):
+        sigma_dataset_qualified_name: Optional[str] = Field(
+            None, description="", alias="sigmaDatasetQualifiedName"
         )
-        qlik_datasets: Optional[list[QlikDataset]] = Field(
-            None, description="", alias="qlikDatasets"
-        )  # relationship
-        qlik_apps: Optional[list[QlikApp]] = Field(
-            None, description="", alias="qlikApps"
+        sigma_dataset_name: Optional[str] = Field(
+            None, description="", alias="sigmaDatasetName"
+        )
+        sigma_dataset: Optional[SigmaDataset] = Field(
+            None, description="", alias="sigmaDataset"
         )  # relationship
 
-    attributes: "QlikSpace.Attributes" = Field(
-        default_factory=lambda: QlikSpace.Attributes(),
+    attributes: "SigmaDatasetColumn.Attributes" = Field(
+        default_factory=lambda: SigmaDatasetColumn.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class QlikApp(Qlik):
+class SigmaDataset(Sigma):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in QlikApp._convience_properties:
+        if name in SigmaDataset._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "qlik_has_section_access",
-        "qlik_origin_app_id",
-        "qlik_is_encrypted",
-        "qlik_is_direct_query_mode",
-        "qlik_app_static_byte_size",
-        "qlik_space",
-        "qlik_sheets",
+        "sigma_dataset_column_count",
+        "sigma_dataset_columns",
     ]
 
     @property
-    def qlik_has_section_access(self) -> Optional[bool]:
-        return self.attributes.qlik_has_section_access
+    def sigma_dataset_column_count(self) -> Optional[int]:
+        return self.attributes.sigma_dataset_column_count
 
-    @qlik_has_section_access.setter
-    def qlik_has_section_access(self, qlik_has_section_access: Optional[bool]):
+    @sigma_dataset_column_count.setter
+    def sigma_dataset_column_count(self, sigma_dataset_column_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_has_section_access = qlik_has_section_access
+        self.attributes.sigma_dataset_column_count = sigma_dataset_column_count
 
     @property
-    def qlik_origin_app_id(self) -> Optional[str]:
-        return self.attributes.qlik_origin_app_id
+    def sigma_dataset_columns(self) -> Optional[list[SigmaDatasetColumn]]:
+        return self.attributes.sigma_dataset_columns
 
-    @qlik_origin_app_id.setter
-    def qlik_origin_app_id(self, qlik_origin_app_id: Optional[str]):
+    @sigma_dataset_columns.setter
+    def sigma_dataset_columns(
+        self, sigma_dataset_columns: Optional[list[SigmaDatasetColumn]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_origin_app_id = qlik_origin_app_id
+        self.attributes.sigma_dataset_columns = sigma_dataset_columns
 
-    @property
-    def qlik_is_encrypted(self) -> Optional[bool]:
-        return self.attributes.qlik_is_encrypted
+    type_name: str = Field("SigmaDataset", allow_mutation=False)
 
-    @qlik_is_encrypted.setter
-    def qlik_is_encrypted(self, qlik_is_encrypted: Optional[bool]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.qlik_is_encrypted = qlik_is_encrypted
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SigmaDataset":
+            raise ValueError("must be SigmaDataset")
+        return v
 
-    @property
-    def qlik_is_direct_query_mode(self) -> Optional[bool]:
-        return self.attributes.qlik_is_direct_query_mode
+    class Attributes(Sigma.Attributes):
+        sigma_dataset_column_count: Optional[int] = Field(
+            None, description="", alias="sigmaDatasetColumnCount"
+        )
+        sigma_dataset_columns: Optional[list[SigmaDatasetColumn]] = Field(
+            None, description="", alias="sigmaDatasetColumns"
+        )  # relationship
 
-    @qlik_is_direct_query_mode.setter
-    def qlik_is_direct_query_mode(self, qlik_is_direct_query_mode: Optional[bool]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.qlik_is_direct_query_mode = qlik_is_direct_query_mode
+    attributes: "SigmaDataset.Attributes" = Field(
+        default_factory=lambda: SigmaDataset.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
 
-    @property
-    def qlik_app_static_byte_size(self) -> Optional[int]:
-        return self.attributes.qlik_app_static_byte_size
 
-    @qlik_app_static_byte_size.setter
-    def qlik_app_static_byte_size(self, qlik_app_static_byte_size: Optional[int]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.qlik_app_static_byte_size = qlik_app_static_byte_size
+class SigmaWorkbook(Sigma):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in SigmaWorkbook._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "sigma_page_count",
+        "sigma_pages",
+    ]
 
     @property
-    def qlik_space(self) -> Optional[QlikSpace]:
-        return self.attributes.qlik_space
+    def sigma_page_count(self) -> Optional[int]:
+        return self.attributes.sigma_page_count
 
-    @qlik_space.setter
-    def qlik_space(self, qlik_space: Optional[QlikSpace]):
+    @sigma_page_count.setter
+    def sigma_page_count(self, sigma_page_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_space = qlik_space
+        self.attributes.sigma_page_count = sigma_page_count
 
     @property
-    def qlik_sheets(self) -> Optional[list[QlikSheet]]:
-        return self.attributes.qlik_sheets
+    def sigma_pages(self) -> Optional[list[SigmaPage]]:
+        return self.attributes.sigma_pages
 
-    @qlik_sheets.setter
-    def qlik_sheets(self, qlik_sheets: Optional[list[QlikSheet]]):
+    @sigma_pages.setter
+    def sigma_pages(self, sigma_pages: Optional[list[SigmaPage]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_sheets = qlik_sheets
+        self.attributes.sigma_pages = sigma_pages
 
-    type_name: str = Field("QlikApp", allow_mutation=False)
+    type_name: str = Field("SigmaWorkbook", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "QlikApp":
-            raise ValueError("must be QlikApp")
+        if v != "SigmaWorkbook":
+            raise ValueError("must be SigmaWorkbook")
         return v
 
-    class Attributes(Qlik.Attributes):
-        qlik_has_section_access: Optional[bool] = Field(
-            None, description="", alias="qlikHasSectionAccess"
-        )
-        qlik_origin_app_id: Optional[str] = Field(
-            None, description="", alias="qlikOriginAppId"
-        )
-        qlik_is_encrypted: Optional[bool] = Field(
-            None, description="", alias="qlikIsEncrypted"
-        )
-        qlik_is_direct_query_mode: Optional[bool] = Field(
-            None, description="", alias="qlikIsDirectQueryMode"
-        )
-        qlik_app_static_byte_size: Optional[int] = Field(
-            None, description="", alias="qlikAppStaticByteSize"
+    class Attributes(Sigma.Attributes):
+        sigma_page_count: Optional[int] = Field(
+            None, description="", alias="sigmaPageCount"
         )
-        qlik_space: Optional[QlikSpace] = Field(
-            None, description="", alias="qlikSpace"
-        )  # relationship
-        qlik_sheets: Optional[list[QlikSheet]] = Field(
-            None, description="", alias="qlikSheets"
+        sigma_pages: Optional[list[SigmaPage]] = Field(
+            None, description="", alias="sigmaPages"
         )  # relationship
 
-    attributes: "QlikApp.Attributes" = Field(
-        default_factory=lambda: QlikApp.Attributes(),
+    attributes: "SigmaWorkbook.Attributes" = Field(
+        default_factory=lambda: SigmaWorkbook.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class QlikChart(Qlik):
+class SigmaDataElementField(Sigma):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in QlikChart._convience_properties:
+        if name in SigmaDataElementField._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "qlik_chart_subtitle",
-        "qlik_chart_footnote",
-        "qlik_chart_orientation",
-        "qlik_chart_type",
-        "qlik_sheet",
+        "sigma_data_element_field_is_hidden",
+        "sigma_data_element_field_formula",
+        "sigma_data_element",
     ]
 
     @property
-    def qlik_chart_subtitle(self) -> Optional[str]:
-        return self.attributes.qlik_chart_subtitle
-
-    @qlik_chart_subtitle.setter
-    def qlik_chart_subtitle(self, qlik_chart_subtitle: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.qlik_chart_subtitle = qlik_chart_subtitle
-
-    @property
-    def qlik_chart_footnote(self) -> Optional[str]:
-        return self.attributes.qlik_chart_footnote
-
-    @qlik_chart_footnote.setter
-    def qlik_chart_footnote(self, qlik_chart_footnote: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.qlik_chart_footnote = qlik_chart_footnote
-
-    @property
-    def qlik_chart_orientation(self) -> Optional[str]:
-        return self.attributes.qlik_chart_orientation
+    def sigma_data_element_field_is_hidden(self) -> Optional[bool]:
+        return self.attributes.sigma_data_element_field_is_hidden
 
-    @qlik_chart_orientation.setter
-    def qlik_chart_orientation(self, qlik_chart_orientation: Optional[str]):
+    @sigma_data_element_field_is_hidden.setter
+    def sigma_data_element_field_is_hidden(
+        self, sigma_data_element_field_is_hidden: Optional[bool]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_chart_orientation = qlik_chart_orientation
+        self.attributes.sigma_data_element_field_is_hidden = (
+            sigma_data_element_field_is_hidden
+        )
 
     @property
-    def qlik_chart_type(self) -> Optional[str]:
-        return self.attributes.qlik_chart_type
+    def sigma_data_element_field_formula(self) -> Optional[str]:
+        return self.attributes.sigma_data_element_field_formula
 
-    @qlik_chart_type.setter
-    def qlik_chart_type(self, qlik_chart_type: Optional[str]):
+    @sigma_data_element_field_formula.setter
+    def sigma_data_element_field_formula(
+        self, sigma_data_element_field_formula: Optional[str]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_chart_type = qlik_chart_type
+        self.attributes.sigma_data_element_field_formula = (
+            sigma_data_element_field_formula
+        )
 
     @property
-    def qlik_sheet(self) -> Optional[QlikSheet]:
-        return self.attributes.qlik_sheet
+    def sigma_data_element(self) -> Optional[SigmaDataElement]:
+        return self.attributes.sigma_data_element
 
-    @qlik_sheet.setter
-    def qlik_sheet(self, qlik_sheet: Optional[QlikSheet]):
+    @sigma_data_element.setter
+    def sigma_data_element(self, sigma_data_element: Optional[SigmaDataElement]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_sheet = qlik_sheet
+        self.attributes.sigma_data_element = sigma_data_element
 
-    type_name: str = Field("QlikChart", allow_mutation=False)
+    type_name: str = Field("SigmaDataElementField", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "QlikChart":
-            raise ValueError("must be QlikChart")
+        if v != "SigmaDataElementField":
+            raise ValueError("must be SigmaDataElementField")
         return v
 
-    class Attributes(Qlik.Attributes):
-        qlik_chart_subtitle: Optional[str] = Field(
-            None, description="", alias="qlikChartSubtitle"
-        )
-        qlik_chart_footnote: Optional[str] = Field(
-            None, description="", alias="qlikChartFootnote"
-        )
-        qlik_chart_orientation: Optional[str] = Field(
-            None, description="", alias="qlikChartOrientation"
+    class Attributes(Sigma.Attributes):
+        sigma_data_element_field_is_hidden: Optional[bool] = Field(
+            None, description="", alias="sigmaDataElementFieldIsHidden"
         )
-        qlik_chart_type: Optional[str] = Field(
-            None, description="", alias="qlikChartType"
+        sigma_data_element_field_formula: Optional[str] = Field(
+            None, description="", alias="sigmaDataElementFieldFormula"
         )
-        qlik_sheet: Optional[QlikSheet] = Field(
-            None, description="", alias="qlikSheet"
+        sigma_data_element: Optional[SigmaDataElement] = Field(
+            None, description="", alias="sigmaDataElement"
         )  # relationship
 
-    attributes: "QlikChart.Attributes" = Field(
-        default_factory=lambda: QlikChart.Attributes(),
+    attributes: "SigmaDataElementField.Attributes" = Field(
+        default_factory=lambda: SigmaDataElementField.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class QlikDataset(Qlik):
+class SigmaPage(Sigma):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in QlikDataset._convience_properties:
+        if name in SigmaPage._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "qlik_dataset_technical_name",
-        "qlik_dataset_type",
-        "qlik_dataset_uri",
-        "qlik_dataset_subtype",
-        "qlik_space",
+        "sigma_data_element_count",
+        "sigma_data_elements",
+        "sigma_workbook",
     ]
 
     @property
-    def qlik_dataset_technical_name(self) -> Optional[str]:
-        return self.attributes.qlik_dataset_technical_name
-
-    @qlik_dataset_technical_name.setter
-    def qlik_dataset_technical_name(self, qlik_dataset_technical_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.qlik_dataset_technical_name = qlik_dataset_technical_name
-
-    @property
-    def qlik_dataset_type(self) -> Optional[str]:
-        return self.attributes.qlik_dataset_type
-
-    @qlik_dataset_type.setter
-    def qlik_dataset_type(self, qlik_dataset_type: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.qlik_dataset_type = qlik_dataset_type
-
-    @property
-    def qlik_dataset_uri(self) -> Optional[str]:
-        return self.attributes.qlik_dataset_uri
+    def sigma_data_element_count(self) -> Optional[int]:
+        return self.attributes.sigma_data_element_count
 
-    @qlik_dataset_uri.setter
-    def qlik_dataset_uri(self, qlik_dataset_uri: Optional[str]):
+    @sigma_data_element_count.setter
+    def sigma_data_element_count(self, sigma_data_element_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_dataset_uri = qlik_dataset_uri
+        self.attributes.sigma_data_element_count = sigma_data_element_count
 
     @property
-    def qlik_dataset_subtype(self) -> Optional[str]:
-        return self.attributes.qlik_dataset_subtype
+    def sigma_data_elements(self) -> Optional[list[SigmaDataElement]]:
+        return self.attributes.sigma_data_elements
 
-    @qlik_dataset_subtype.setter
-    def qlik_dataset_subtype(self, qlik_dataset_subtype: Optional[str]):
+    @sigma_data_elements.setter
+    def sigma_data_elements(
+        self, sigma_data_elements: Optional[list[SigmaDataElement]]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_dataset_subtype = qlik_dataset_subtype
+        self.attributes.sigma_data_elements = sigma_data_elements
 
     @property
-    def qlik_space(self) -> Optional[QlikSpace]:
-        return self.attributes.qlik_space
+    def sigma_workbook(self) -> Optional[SigmaWorkbook]:
+        return self.attributes.sigma_workbook
 
-    @qlik_space.setter
-    def qlik_space(self, qlik_space: Optional[QlikSpace]):
+    @sigma_workbook.setter
+    def sigma_workbook(self, sigma_workbook: Optional[SigmaWorkbook]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_space = qlik_space
+        self.attributes.sigma_workbook = sigma_workbook
 
-    type_name: str = Field("QlikDataset", allow_mutation=False)
+    type_name: str = Field("SigmaPage", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "QlikDataset":
-            raise ValueError("must be QlikDataset")
+        if v != "SigmaPage":
+            raise ValueError("must be SigmaPage")
         return v
 
-    class Attributes(Qlik.Attributes):
-        qlik_dataset_technical_name: Optional[str] = Field(
-            None, description="", alias="qlikDatasetTechnicalName"
-        )
-        qlik_dataset_type: Optional[str] = Field(
-            None, description="", alias="qlikDatasetType"
-        )
-        qlik_dataset_uri: Optional[str] = Field(
-            None, description="", alias="qlikDatasetUri"
-        )
-        qlik_dataset_subtype: Optional[str] = Field(
-            None, description="", alias="qlikDatasetSubtype"
+    class Attributes(Sigma.Attributes):
+        sigma_data_element_count: Optional[int] = Field(
+            None, description="", alias="sigmaDataElementCount"
         )
-        qlik_space: Optional[QlikSpace] = Field(
-            None, description="", alias="qlikSpace"
+        sigma_data_elements: Optional[list[SigmaDataElement]] = Field(
+            None, description="", alias="sigmaDataElements"
+        )  # relationship
+        sigma_workbook: Optional[SigmaWorkbook] = Field(
+            None, description="", alias="sigmaWorkbook"
         )  # relationship
 
-    attributes: "QlikDataset.Attributes" = Field(
-        default_factory=lambda: QlikDataset.Attributes(),
+    attributes: "SigmaPage.Attributes" = Field(
+        default_factory=lambda: SigmaPage.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class QlikSheet(Qlik):
+class SigmaDataElement(Sigma):
     """Description"""
 
     def __setattr__(self, name, value):
-        if name in QlikSheet._convience_properties:
+        if name in SigmaDataElement._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
-        "qlik_sheet_is_approved",
-        "qlik_app",
-        "qlik_charts",
+        "sigma_data_element_query",
+        "sigma_data_element_type",
+        "sigma_data_element_field_count",
+        "sigma_page",
+        "sigma_data_element_fields",
     ]
 
     @property
-    def qlik_sheet_is_approved(self) -> Optional[bool]:
-        return self.attributes.qlik_sheet_is_approved
+    def sigma_data_element_query(self) -> Optional[str]:
+        return self.attributes.sigma_data_element_query
 
-    @qlik_sheet_is_approved.setter
-    def qlik_sheet_is_approved(self, qlik_sheet_is_approved: Optional[bool]):
+    @sigma_data_element_query.setter
+    def sigma_data_element_query(self, sigma_data_element_query: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_sheet_is_approved = qlik_sheet_is_approved
+        self.attributes.sigma_data_element_query = sigma_data_element_query
 
     @property
-    def qlik_app(self) -> Optional[QlikApp]:
-        return self.attributes.qlik_app
+    def sigma_data_element_type(self) -> Optional[str]:
+        return self.attributes.sigma_data_element_type
 
-    @qlik_app.setter
-    def qlik_app(self, qlik_app: Optional[QlikApp]):
+    @sigma_data_element_type.setter
+    def sigma_data_element_type(self, sigma_data_element_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_app = qlik_app
+        self.attributes.sigma_data_element_type = sigma_data_element_type
 
     @property
-    def qlik_charts(self) -> Optional[list[QlikChart]]:
-        return self.attributes.qlik_charts
+    def sigma_data_element_field_count(self) -> Optional[int]:
+        return self.attributes.sigma_data_element_field_count
 
-    @qlik_charts.setter
-    def qlik_charts(self, qlik_charts: Optional[list[QlikChart]]):
+    @sigma_data_element_field_count.setter
+    def sigma_data_element_field_count(
+        self, sigma_data_element_field_count: Optional[int]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.qlik_charts = qlik_charts
+        self.attributes.sigma_data_element_field_count = sigma_data_element_field_count
 
-    type_name: str = Field("QlikSheet", allow_mutation=False)
+    @property
+    def sigma_page(self) -> Optional[SigmaPage]:
+        return self.attributes.sigma_page
+
+    @sigma_page.setter
+    def sigma_page(self, sigma_page: Optional[SigmaPage]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_page = sigma_page
+
+    @property
+    def sigma_data_element_fields(self) -> Optional[list[SigmaDataElementField]]:
+        return self.attributes.sigma_data_element_fields
+
+    @sigma_data_element_fields.setter
+    def sigma_data_element_fields(
+        self, sigma_data_element_fields: Optional[list[SigmaDataElementField]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.sigma_data_element_fields = sigma_data_element_fields
+
+    type_name: str = Field("SigmaDataElement", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "QlikSheet":
-            raise ValueError("must be QlikSheet")
+        if v != "SigmaDataElement":
+            raise ValueError("must be SigmaDataElement")
         return v
 
-    class Attributes(Qlik.Attributes):
-        qlik_sheet_is_approved: Optional[bool] = Field(
-            None, description="", alias="qlikSheetIsApproved"
+    class Attributes(Sigma.Attributes):
+        sigma_data_element_query: Optional[str] = Field(
+            None, description="", alias="sigmaDataElementQuery"
         )
-        qlik_app: Optional[QlikApp] = Field(
-            None, description="", alias="qlikApp"
+        sigma_data_element_type: Optional[str] = Field(
+            None, description="", alias="sigmaDataElementType"
+        )
+        sigma_data_element_field_count: Optional[int] = Field(
+            None, description="", alias="sigmaDataElementFieldCount"
+        )
+        sigma_page: Optional[SigmaPage] = Field(
+            None, description="", alias="sigmaPage"
         )  # relationship
-        qlik_charts: Optional[list[QlikChart]] = Field(
-            None, description="", alias="qlikCharts"
+        sigma_data_element_fields: Optional[list[SigmaDataElementField]] = Field(
+            None, description="", alias="sigmaDataElementFields"
         )  # relationship
 
-    attributes: "QlikSheet.Attributes" = Field(
-        default_factory=lambda: QlikSheet.Attributes(),
+    attributes: "SigmaDataElement.Attributes" = Field(
+        default_factory=lambda: SigmaDataElement.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
 class TableauWorkbook(Tableau):
     """Description"""
@@ -20302,14 +17743,56 @@
     attributes: "TableauMetric.Attributes" = Field(
         default_factory=lambda: TableauMetric.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class TableauSite(Tableau):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in TableauSite._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "projects",
+    ]
+
+    @property
+    def projects(self) -> Optional[list[TableauProject]]:
+        return self.attributes.projects
+
+    @projects.setter
+    def projects(self, projects: Optional[list[TableauProject]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.projects = projects
+
+    type_name: str = Field("TableauSite", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "TableauSite":
+            raise ValueError("must be TableauSite")
+        return v
+
+    class Attributes(Tableau.Attributes):
+        projects: Optional[list[TableauProject]] = Field(
+            None, description="", alias="projects"
+        )  # relationship
+
+    attributes: "TableauSite.Attributes" = Field(
+        default_factory=lambda: TableauSite.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class TableauDatasource(Tableau):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in TableauDatasource._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -20554,56 +18037,14 @@
     attributes: "TableauDatasource.Attributes" = Field(
         default_factory=lambda: TableauDatasource.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
-class TableauSite(Tableau):
-    """Description"""
-
-    def __setattr__(self, name, value):
-        if name in TableauSite._convience_properties:
-            return object.__setattr__(self, name, value)
-        super().__setattr__(name, value)
-
-    _convience_properties: ClassVar[list[str]] = [
-        "projects",
-    ]
-
-    @property
-    def projects(self) -> Optional[list[TableauProject]]:
-        return self.attributes.projects
-
-    @projects.setter
-    def projects(self, projects: Optional[list[TableauProject]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.projects = projects
-
-    type_name: str = Field("TableauSite", allow_mutation=False)
-
-    @validator("type_name")
-    def validate_type_name(cls, v):
-        if v != "TableauSite":
-            raise ValueError("must be TableauSite")
-        return v
-
-    class Attributes(Tableau.Attributes):
-        projects: Optional[list[TableauProject]] = Field(
-            None, description="", alias="projects"
-        )  # relationship
-
-    attributes: "TableauSite.Attributes" = Field(
-        default_factory=lambda: TableauSite.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
-    )
-
-
 class TableauDashboard(Tableau):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in TableauDashboard._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -22656,14 +20097,3767 @@
     attributes: "RedashVisualization.Attributes" = Field(
         default_factory=lambda: RedashVisualization.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class MetabaseQuestion(Metabase):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MetabaseQuestion._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "metabase_dashboard_count",
+        "metabase_query_type",
+        "metabase_query",
+        "metabase_dashboards",
+        "metabase_collection",
+    ]
+
+    @property
+    def metabase_dashboard_count(self) -> Optional[int]:
+        return self.attributes.metabase_dashboard_count
+
+    @metabase_dashboard_count.setter
+    def metabase_dashboard_count(self, metabase_dashboard_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_dashboard_count = metabase_dashboard_count
+
+    @property
+    def metabase_query_type(self) -> Optional[str]:
+        return self.attributes.metabase_query_type
+
+    @metabase_query_type.setter
+    def metabase_query_type(self, metabase_query_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_query_type = metabase_query_type
+
+    @property
+    def metabase_query(self) -> Optional[str]:
+        return self.attributes.metabase_query
+
+    @metabase_query.setter
+    def metabase_query(self, metabase_query: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_query = metabase_query
+
+    @property
+    def metabase_dashboards(self) -> Optional[list[MetabaseDashboard]]:
+        return self.attributes.metabase_dashboards
+
+    @metabase_dashboards.setter
+    def metabase_dashboards(
+        self, metabase_dashboards: Optional[list[MetabaseDashboard]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_dashboards = metabase_dashboards
+
+    @property
+    def metabase_collection(self) -> Optional[MetabaseCollection]:
+        return self.attributes.metabase_collection
+
+    @metabase_collection.setter
+    def metabase_collection(self, metabase_collection: Optional[MetabaseCollection]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_collection = metabase_collection
+
+    type_name: str = Field("MetabaseQuestion", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MetabaseQuestion":
+            raise ValueError("must be MetabaseQuestion")
+        return v
+
+    class Attributes(Metabase.Attributes):
+        metabase_dashboard_count: Optional[int] = Field(
+            None, description="", alias="metabaseDashboardCount"
+        )
+        metabase_query_type: Optional[str] = Field(
+            None, description="", alias="metabaseQueryType"
+        )
+        metabase_query: Optional[str] = Field(
+            None, description="", alias="metabaseQuery"
+        )
+        metabase_dashboards: Optional[list[MetabaseDashboard]] = Field(
+            None, description="", alias="metabaseDashboards"
+        )  # relationship
+        metabase_collection: Optional[MetabaseCollection] = Field(
+            None, description="", alias="metabaseCollection"
+        )  # relationship
+
+    attributes: "MetabaseQuestion.Attributes" = Field(
+        default_factory=lambda: MetabaseQuestion.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class MetabaseCollection(Metabase):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MetabaseCollection._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "metabase_slug",
+        "metabase_color",
+        "metabase_namespace",
+        "metabase_is_personal_collection",
+        "metabase_dashboards",
+        "metabase_questions",
+    ]
+
+    @property
+    def metabase_slug(self) -> Optional[str]:
+        return self.attributes.metabase_slug
+
+    @metabase_slug.setter
+    def metabase_slug(self, metabase_slug: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_slug = metabase_slug
+
+    @property
+    def metabase_color(self) -> Optional[str]:
+        return self.attributes.metabase_color
+
+    @metabase_color.setter
+    def metabase_color(self, metabase_color: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_color = metabase_color
+
+    @property
+    def metabase_namespace(self) -> Optional[str]:
+        return self.attributes.metabase_namespace
+
+    @metabase_namespace.setter
+    def metabase_namespace(self, metabase_namespace: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_namespace = metabase_namespace
+
+    @property
+    def metabase_is_personal_collection(self) -> Optional[bool]:
+        return self.attributes.metabase_is_personal_collection
+
+    @metabase_is_personal_collection.setter
+    def metabase_is_personal_collection(
+        self, metabase_is_personal_collection: Optional[bool]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_is_personal_collection = (
+            metabase_is_personal_collection
+        )
+
+    @property
+    def metabase_dashboards(self) -> Optional[list[MetabaseDashboard]]:
+        return self.attributes.metabase_dashboards
+
+    @metabase_dashboards.setter
+    def metabase_dashboards(
+        self, metabase_dashboards: Optional[list[MetabaseDashboard]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_dashboards = metabase_dashboards
+
+    @property
+    def metabase_questions(self) -> Optional[list[MetabaseQuestion]]:
+        return self.attributes.metabase_questions
+
+    @metabase_questions.setter
+    def metabase_questions(self, metabase_questions: Optional[list[MetabaseQuestion]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_questions = metabase_questions
+
+    type_name: str = Field("MetabaseCollection", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MetabaseCollection":
+            raise ValueError("must be MetabaseCollection")
+        return v
+
+    class Attributes(Metabase.Attributes):
+        metabase_slug: Optional[str] = Field(None, description="", alias="metabaseSlug")
+        metabase_color: Optional[str] = Field(
+            None, description="", alias="metabaseColor"
+        )
+        metabase_namespace: Optional[str] = Field(
+            None, description="", alias="metabaseNamespace"
+        )
+        metabase_is_personal_collection: Optional[bool] = Field(
+            None, description="", alias="metabaseIsPersonalCollection"
+        )
+        metabase_dashboards: Optional[list[MetabaseDashboard]] = Field(
+            None, description="", alias="metabaseDashboards"
+        )  # relationship
+        metabase_questions: Optional[list[MetabaseQuestion]] = Field(
+            None, description="", alias="metabaseQuestions"
+        )  # relationship
+
+    attributes: "MetabaseCollection.Attributes" = Field(
+        default_factory=lambda: MetabaseCollection.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class MetabaseDashboard(Metabase):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MetabaseDashboard._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "metabase_question_count",
+        "metabase_questions",
+        "metabase_collection",
+    ]
+
+    @property
+    def metabase_question_count(self) -> Optional[int]:
+        return self.attributes.metabase_question_count
+
+    @metabase_question_count.setter
+    def metabase_question_count(self, metabase_question_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_question_count = metabase_question_count
+
+    @property
+    def metabase_questions(self) -> Optional[list[MetabaseQuestion]]:
+        return self.attributes.metabase_questions
+
+    @metabase_questions.setter
+    def metabase_questions(self, metabase_questions: Optional[list[MetabaseQuestion]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_questions = metabase_questions
+
+    @property
+    def metabase_collection(self) -> Optional[MetabaseCollection]:
+        return self.attributes.metabase_collection
+
+    @metabase_collection.setter
+    def metabase_collection(self, metabase_collection: Optional[MetabaseCollection]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.metabase_collection = metabase_collection
+
+    type_name: str = Field("MetabaseDashboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MetabaseDashboard":
+            raise ValueError("must be MetabaseDashboard")
+        return v
+
+    class Attributes(Metabase.Attributes):
+        metabase_question_count: Optional[int] = Field(
+            None, description="", alias="metabaseQuestionCount"
+        )
+        metabase_questions: Optional[list[MetabaseQuestion]] = Field(
+            None, description="", alias="metabaseQuestions"
+        )  # relationship
+        metabase_collection: Optional[MetabaseCollection] = Field(
+            None, description="", alias="metabaseCollection"
+        )  # relationship
+
+    attributes: "MetabaseDashboard.Attributes" = Field(
+        default_factory=lambda: MetabaseDashboard.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class QuickSightFolder(QuickSight):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in QuickSightFolder._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "quick_sight_folder_type",
+        "quick_sight_folder_hierarchy",
+        "quick_sight_dashboards",
+        "quick_sight_analyses",
+        "quick_sight_datasets",
+    ]
+
+    @property
+    def quick_sight_folder_type(self) -> Optional[QuickSightFolderType]:
+        return self.attributes.quick_sight_folder_type
+
+    @quick_sight_folder_type.setter
+    def quick_sight_folder_type(
+        self, quick_sight_folder_type: Optional[QuickSightFolderType]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_folder_type = quick_sight_folder_type
+
+    @property
+    def quick_sight_folder_hierarchy(self) -> Optional[list[dict[str, str]]]:
+        return self.attributes.quick_sight_folder_hierarchy
+
+    @quick_sight_folder_hierarchy.setter
+    def quick_sight_folder_hierarchy(
+        self, quick_sight_folder_hierarchy: Optional[list[dict[str, str]]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_folder_hierarchy = quick_sight_folder_hierarchy
+
+    @property
+    def quick_sight_dashboards(self) -> Optional[list[QuickSightDashboard]]:
+        return self.attributes.quick_sight_dashboards
+
+    @quick_sight_dashboards.setter
+    def quick_sight_dashboards(
+        self, quick_sight_dashboards: Optional[list[QuickSightDashboard]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dashboards = quick_sight_dashboards
+
+    @property
+    def quick_sight_analyses(self) -> Optional[list[QuickSightAnalysis]]:
+        return self.attributes.quick_sight_analyses
+
+    @quick_sight_analyses.setter
+    def quick_sight_analyses(
+        self, quick_sight_analyses: Optional[list[QuickSightAnalysis]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analyses = quick_sight_analyses
+
+    @property
+    def quick_sight_datasets(self) -> Optional[list[QuickSightDataset]]:
+        return self.attributes.quick_sight_datasets
+
+    @quick_sight_datasets.setter
+    def quick_sight_datasets(
+        self, quick_sight_datasets: Optional[list[QuickSightDataset]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_datasets = quick_sight_datasets
+
+    type_name: str = Field("QuickSightFolder", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightFolder":
+            raise ValueError("must be QuickSightFolder")
+        return v
+
+    class Attributes(QuickSight.Attributes):
+        quick_sight_folder_type: Optional[QuickSightFolderType] = Field(
+            None, description="", alias="quickSightFolderType"
+        )
+        quick_sight_folder_hierarchy: Optional[list[dict[str, str]]] = Field(
+            None, description="", alias="quickSightFolderHierarchy"
+        )
+        quick_sight_dashboards: Optional[list[QuickSightDashboard]] = Field(
+            None, description="", alias="quickSightDashboards"
+        )  # relationship
+        quick_sight_analyses: Optional[list[QuickSightAnalysis]] = Field(
+            None, description="", alias="quickSightAnalyses"
+        )  # relationship
+        quick_sight_datasets: Optional[list[QuickSightDataset]] = Field(
+            None, description="", alias="quickSightDatasets"
+        )  # relationship
+
+    attributes: "QuickSightFolder.Attributes" = Field(
+        default_factory=lambda: QuickSightFolder.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class QuickSightDashboardVisual(QuickSight):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in QuickSightDashboardVisual._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "quick_sight_dashboard_qualified_name",
+        "quick_sight_dashboard",
+    ]
+
+    @property
+    def quick_sight_dashboard_qualified_name(self) -> Optional[str]:
+        return self.attributes.quick_sight_dashboard_qualified_name
+
+    @quick_sight_dashboard_qualified_name.setter
+    def quick_sight_dashboard_qualified_name(
+        self, quick_sight_dashboard_qualified_name: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dashboard_qualified_name = (
+            quick_sight_dashboard_qualified_name
+        )
+
+    @property
+    def quick_sight_dashboard(self) -> Optional[QuickSightDashboard]:
+        return self.attributes.quick_sight_dashboard
+
+    @quick_sight_dashboard.setter
+    def quick_sight_dashboard(
+        self, quick_sight_dashboard: Optional[QuickSightDashboard]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dashboard = quick_sight_dashboard
+
+    type_name: str = Field("QuickSightDashboardVisual", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightDashboardVisual":
+            raise ValueError("must be QuickSightDashboardVisual")
+        return v
+
+    class Attributes(QuickSight.Attributes):
+        quick_sight_dashboard_qualified_name: Optional[str] = Field(
+            None, description="", alias="quickSightDashboardQualifiedName"
+        )
+        quick_sight_dashboard: Optional[QuickSightDashboard] = Field(
+            None, description="", alias="quickSightDashboard"
+        )  # relationship
+
+    attributes: "QuickSightDashboardVisual.Attributes" = Field(
+        default_factory=lambda: QuickSightDashboardVisual.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class QuickSightAnalysisVisual(QuickSight):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in QuickSightAnalysisVisual._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "quick_sight_analysis_qualified_name",
+        "quick_sight_analysis",
+    ]
+
+    @property
+    def quick_sight_analysis_qualified_name(self) -> Optional[str]:
+        return self.attributes.quick_sight_analysis_qualified_name
+
+    @quick_sight_analysis_qualified_name.setter
+    def quick_sight_analysis_qualified_name(
+        self, quick_sight_analysis_qualified_name: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis_qualified_name = (
+            quick_sight_analysis_qualified_name
+        )
+
+    @property
+    def quick_sight_analysis(self) -> Optional[QuickSightAnalysis]:
+        return self.attributes.quick_sight_analysis
+
+    @quick_sight_analysis.setter
+    def quick_sight_analysis(self, quick_sight_analysis: Optional[QuickSightAnalysis]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis = quick_sight_analysis
+
+    type_name: str = Field("QuickSightAnalysisVisual", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightAnalysisVisual":
+            raise ValueError("must be QuickSightAnalysisVisual")
+        return v
+
+    class Attributes(QuickSight.Attributes):
+        quick_sight_analysis_qualified_name: Optional[str] = Field(
+            None, description="", alias="quickSightAnalysisQualifiedName"
+        )
+        quick_sight_analysis: Optional[QuickSightAnalysis] = Field(
+            None, description="", alias="quickSightAnalysis"
+        )  # relationship
+
+    attributes: "QuickSightAnalysisVisual.Attributes" = Field(
+        default_factory=lambda: QuickSightAnalysisVisual.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class QuickSightDatasetField(QuickSight):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in QuickSightDatasetField._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "quick_sight_dataset_field_type",
+        "quick_sight_dataset_qualified_name",
+        "quick_sight_dataset",
+    ]
+
+    @property
+    def quick_sight_dataset_field_type(self) -> Optional[QuickSightDatasetFieldType]:
+        return self.attributes.quick_sight_dataset_field_type
+
+    @quick_sight_dataset_field_type.setter
+    def quick_sight_dataset_field_type(
+        self, quick_sight_dataset_field_type: Optional[QuickSightDatasetFieldType]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dataset_field_type = quick_sight_dataset_field_type
+
+    @property
+    def quick_sight_dataset_qualified_name(self) -> Optional[str]:
+        return self.attributes.quick_sight_dataset_qualified_name
+
+    @quick_sight_dataset_qualified_name.setter
+    def quick_sight_dataset_qualified_name(
+        self, quick_sight_dataset_qualified_name: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dataset_qualified_name = (
+            quick_sight_dataset_qualified_name
+        )
+
+    @property
+    def quick_sight_dataset(self) -> Optional[QuickSightDataset]:
+        return self.attributes.quick_sight_dataset
+
+    @quick_sight_dataset.setter
+    def quick_sight_dataset(self, quick_sight_dataset: Optional[QuickSightDataset]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dataset = quick_sight_dataset
+
+    type_name: str = Field("QuickSightDatasetField", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightDatasetField":
+            raise ValueError("must be QuickSightDatasetField")
+        return v
+
+    class Attributes(QuickSight.Attributes):
+        quick_sight_dataset_field_type: Optional[QuickSightDatasetFieldType] = Field(
+            None, description="", alias="quickSightDatasetFieldType"
+        )
+        quick_sight_dataset_qualified_name: Optional[str] = Field(
+            None, description="", alias="quickSightDatasetQualifiedName"
+        )
+        quick_sight_dataset: Optional[QuickSightDataset] = Field(
+            None, description="", alias="quickSightDataset"
+        )  # relationship
+
+    attributes: "QuickSightDatasetField.Attributes" = Field(
+        default_factory=lambda: QuickSightDatasetField.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class QuickSightAnalysis(QuickSight):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in QuickSightAnalysis._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "quick_sight_analysis_status",
+        "quick_sight_analysis_calculated_fields",
+        "quick_sight_analysis_parameter_declarations",
+        "quick_sight_analysis_filter_groups",
+        "quick_sight_analysis_visuals",
+        "quick_sight_analysis_folders",
+    ]
+
+    @property
+    def quick_sight_analysis_status(self) -> Optional[QuickSightAnalysisStatus]:
+        return self.attributes.quick_sight_analysis_status
+
+    @quick_sight_analysis_status.setter
+    def quick_sight_analysis_status(
+        self, quick_sight_analysis_status: Optional[QuickSightAnalysisStatus]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis_status = quick_sight_analysis_status
+
+    @property
+    def quick_sight_analysis_calculated_fields(self) -> Optional[set[str]]:
+        return self.attributes.quick_sight_analysis_calculated_fields
+
+    @quick_sight_analysis_calculated_fields.setter
+    def quick_sight_analysis_calculated_fields(
+        self, quick_sight_analysis_calculated_fields: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis_calculated_fields = (
+            quick_sight_analysis_calculated_fields
+        )
+
+    @property
+    def quick_sight_analysis_parameter_declarations(self) -> Optional[set[str]]:
+        return self.attributes.quick_sight_analysis_parameter_declarations
+
+    @quick_sight_analysis_parameter_declarations.setter
+    def quick_sight_analysis_parameter_declarations(
+        self, quick_sight_analysis_parameter_declarations: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis_parameter_declarations = (
+            quick_sight_analysis_parameter_declarations
+        )
+
+    @property
+    def quick_sight_analysis_filter_groups(self) -> Optional[set[str]]:
+        return self.attributes.quick_sight_analysis_filter_groups
+
+    @quick_sight_analysis_filter_groups.setter
+    def quick_sight_analysis_filter_groups(
+        self, quick_sight_analysis_filter_groups: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis_filter_groups = (
+            quick_sight_analysis_filter_groups
+        )
+
+    @property
+    def quick_sight_analysis_visuals(self) -> Optional[list[QuickSightAnalysisVisual]]:
+        return self.attributes.quick_sight_analysis_visuals
+
+    @quick_sight_analysis_visuals.setter
+    def quick_sight_analysis_visuals(
+        self, quick_sight_analysis_visuals: Optional[list[QuickSightAnalysisVisual]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis_visuals = quick_sight_analysis_visuals
+
+    @property
+    def quick_sight_analysis_folders(self) -> Optional[list[QuickSightFolder]]:
+        return self.attributes.quick_sight_analysis_folders
+
+    @quick_sight_analysis_folders.setter
+    def quick_sight_analysis_folders(
+        self, quick_sight_analysis_folders: Optional[list[QuickSightFolder]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_analysis_folders = quick_sight_analysis_folders
+
+    type_name: str = Field("QuickSightAnalysis", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightAnalysis":
+            raise ValueError("must be QuickSightAnalysis")
+        return v
+
+    class Attributes(QuickSight.Attributes):
+        quick_sight_analysis_status: Optional[QuickSightAnalysisStatus] = Field(
+            None, description="", alias="quickSightAnalysisStatus"
+        )
+        quick_sight_analysis_calculated_fields: Optional[set[str]] = Field(
+            None, description="", alias="quickSightAnalysisCalculatedFields"
+        )
+        quick_sight_analysis_parameter_declarations: Optional[set[str]] = Field(
+            None, description="", alias="quickSightAnalysisParameterDeclarations"
+        )
+        quick_sight_analysis_filter_groups: Optional[set[str]] = Field(
+            None, description="", alias="quickSightAnalysisFilterGroups"
+        )
+        quick_sight_analysis_visuals: Optional[list[QuickSightAnalysisVisual]] = Field(
+            None, description="", alias="quickSightAnalysisVisuals"
+        )  # relationship
+        quick_sight_analysis_folders: Optional[list[QuickSightFolder]] = Field(
+            None, description="", alias="quickSightAnalysisFolders"
+        )  # relationship
+
+    attributes: "QuickSightAnalysis.Attributes" = Field(
+        default_factory=lambda: QuickSightAnalysis.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class QuickSightDashboard(QuickSight):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in QuickSightDashboard._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "quick_sight_dashboard_published_version_number",
+        "quick_sight_dashboard_last_published_time",
+        "quick_sight_dashboard_folders",
+        "quick_sight_dashboard_visuals",
+    ]
+
+    @property
+    def quick_sight_dashboard_published_version_number(self) -> Optional[int]:
+        return self.attributes.quick_sight_dashboard_published_version_number
+
+    @quick_sight_dashboard_published_version_number.setter
+    def quick_sight_dashboard_published_version_number(
+        self, quick_sight_dashboard_published_version_number: Optional[int]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dashboard_published_version_number = (
+            quick_sight_dashboard_published_version_number
+        )
+
+    @property
+    def quick_sight_dashboard_last_published_time(self) -> Optional[datetime]:
+        return self.attributes.quick_sight_dashboard_last_published_time
+
+    @quick_sight_dashboard_last_published_time.setter
+    def quick_sight_dashboard_last_published_time(
+        self, quick_sight_dashboard_last_published_time: Optional[datetime]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dashboard_last_published_time = (
+            quick_sight_dashboard_last_published_time
+        )
+
+    @property
+    def quick_sight_dashboard_folders(self) -> Optional[list[QuickSightFolder]]:
+        return self.attributes.quick_sight_dashboard_folders
+
+    @quick_sight_dashboard_folders.setter
+    def quick_sight_dashboard_folders(
+        self, quick_sight_dashboard_folders: Optional[list[QuickSightFolder]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dashboard_folders = quick_sight_dashboard_folders
+
+    @property
+    def quick_sight_dashboard_visuals(
+        self,
+    ) -> Optional[list[QuickSightDashboardVisual]]:
+        return self.attributes.quick_sight_dashboard_visuals
+
+    @quick_sight_dashboard_visuals.setter
+    def quick_sight_dashboard_visuals(
+        self, quick_sight_dashboard_visuals: Optional[list[QuickSightDashboardVisual]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dashboard_visuals = quick_sight_dashboard_visuals
+
+    type_name: str = Field("QuickSightDashboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightDashboard":
+            raise ValueError("must be QuickSightDashboard")
+        return v
+
+    class Attributes(QuickSight.Attributes):
+        quick_sight_dashboard_published_version_number: Optional[int] = Field(
+            None, description="", alias="quickSightDashboardPublishedVersionNumber"
+        )
+        quick_sight_dashboard_last_published_time: Optional[datetime] = Field(
+            None, description="", alias="quickSightDashboardLastPublishedTime"
+        )
+        quick_sight_dashboard_folders: Optional[list[QuickSightFolder]] = Field(
+            None, description="", alias="quickSightDashboardFolders"
+        )  # relationship
+        quick_sight_dashboard_visuals: Optional[
+            list[QuickSightDashboardVisual]
+        ] = Field(
+            None, description="", alias="quickSightDashboardVisuals"
+        )  # relationship
+
+    attributes: "QuickSightDashboard.Attributes" = Field(
+        default_factory=lambda: QuickSightDashboard.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class QuickSightDataset(QuickSight):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in QuickSightDataset._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "quick_sight_dataset_import_mode",
+        "quick_sight_dataset_column_count",
+        "quick_sight_dataset_folders",
+        "quick_sight_dataset_fields",
+    ]
+
+    @property
+    def quick_sight_dataset_import_mode(self) -> Optional[QuickSightDatasetImportMode]:
+        return self.attributes.quick_sight_dataset_import_mode
+
+    @quick_sight_dataset_import_mode.setter
+    def quick_sight_dataset_import_mode(
+        self, quick_sight_dataset_import_mode: Optional[QuickSightDatasetImportMode]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dataset_import_mode = (
+            quick_sight_dataset_import_mode
+        )
+
+    @property
+    def quick_sight_dataset_column_count(self) -> Optional[int]:
+        return self.attributes.quick_sight_dataset_column_count
+
+    @quick_sight_dataset_column_count.setter
+    def quick_sight_dataset_column_count(
+        self, quick_sight_dataset_column_count: Optional[int]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dataset_column_count = (
+            quick_sight_dataset_column_count
+        )
+
+    @property
+    def quick_sight_dataset_folders(self) -> Optional[list[QuickSightFolder]]:
+        return self.attributes.quick_sight_dataset_folders
+
+    @quick_sight_dataset_folders.setter
+    def quick_sight_dataset_folders(
+        self, quick_sight_dataset_folders: Optional[list[QuickSightFolder]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dataset_folders = quick_sight_dataset_folders
+
+    @property
+    def quick_sight_dataset_fields(self) -> Optional[list[QuickSightDatasetField]]:
+        return self.attributes.quick_sight_dataset_fields
+
+    @quick_sight_dataset_fields.setter
+    def quick_sight_dataset_fields(
+        self, quick_sight_dataset_fields: Optional[list[QuickSightDatasetField]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.quick_sight_dataset_fields = quick_sight_dataset_fields
+
+    type_name: str = Field("QuickSightDataset", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QuickSightDataset":
+            raise ValueError("must be QuickSightDataset")
+        return v
+
+    class Attributes(QuickSight.Attributes):
+        quick_sight_dataset_import_mode: Optional[QuickSightDatasetImportMode] = Field(
+            None, description="", alias="quickSightDatasetImportMode"
+        )
+        quick_sight_dataset_column_count: Optional[int] = Field(
+            None, description="", alias="quickSightDatasetColumnCount"
+        )
+        quick_sight_dataset_folders: Optional[list[QuickSightFolder]] = Field(
+            None, description="", alias="quickSightDatasetFolders"
+        )  # relationship
+        quick_sight_dataset_fields: Optional[list[QuickSightDatasetField]] = Field(
+            None, description="", alias="quickSightDatasetFields"
+        )  # relationship
+
+    attributes: "QuickSightDataset.Attributes" = Field(
+        default_factory=lambda: QuickSightDataset.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class ThoughtspotLiveboard(Thoughtspot):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in ThoughtspotLiveboard._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "thoughtspot_dashlets",
+    ]
+
+    @property
+    def thoughtspot_dashlets(self) -> Optional[list[ThoughtspotDashlet]]:
+        return self.attributes.thoughtspot_dashlets
+
+    @thoughtspot_dashlets.setter
+    def thoughtspot_dashlets(
+        self, thoughtspot_dashlets: Optional[list[ThoughtspotDashlet]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.thoughtspot_dashlets = thoughtspot_dashlets
+
+    type_name: str = Field("ThoughtspotLiveboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ThoughtspotLiveboard":
+            raise ValueError("must be ThoughtspotLiveboard")
+        return v
+
+    class Attributes(Thoughtspot.Attributes):
+        thoughtspot_dashlets: Optional[list[ThoughtspotDashlet]] = Field(
+            None, description="", alias="thoughtspotDashlets"
+        )  # relationship
+
+    attributes: "ThoughtspotLiveboard.Attributes" = Field(
+        default_factory=lambda: ThoughtspotLiveboard.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class ThoughtspotDashlet(Thoughtspot):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in ThoughtspotDashlet._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "thoughtspot_liveboard_name",
+        "thoughtspot_liveboard_qualified_name",
+        "thoughtspot_liveboard",
+    ]
+
+    @property
+    def thoughtspot_liveboard_name(self) -> Optional[str]:
+        return self.attributes.thoughtspot_liveboard_name
+
+    @thoughtspot_liveboard_name.setter
+    def thoughtspot_liveboard_name(self, thoughtspot_liveboard_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.thoughtspot_liveboard_name = thoughtspot_liveboard_name
+
+    @property
+    def thoughtspot_liveboard_qualified_name(self) -> Optional[str]:
+        return self.attributes.thoughtspot_liveboard_qualified_name
+
+    @thoughtspot_liveboard_qualified_name.setter
+    def thoughtspot_liveboard_qualified_name(
+        self, thoughtspot_liveboard_qualified_name: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.thoughtspot_liveboard_qualified_name = (
+            thoughtspot_liveboard_qualified_name
+        )
+
+    @property
+    def thoughtspot_liveboard(self) -> Optional[ThoughtspotLiveboard]:
+        return self.attributes.thoughtspot_liveboard
+
+    @thoughtspot_liveboard.setter
+    def thoughtspot_liveboard(
+        self, thoughtspot_liveboard: Optional[ThoughtspotLiveboard]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.thoughtspot_liveboard = thoughtspot_liveboard
+
+    type_name: str = Field("ThoughtspotDashlet", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ThoughtspotDashlet":
+            raise ValueError("must be ThoughtspotDashlet")
+        return v
+
+    class Attributes(Thoughtspot.Attributes):
+        thoughtspot_liveboard_name: Optional[str] = Field(
+            None, description="", alias="thoughtspotLiveboardName"
+        )
+        thoughtspot_liveboard_qualified_name: Optional[str] = Field(
+            None, description="", alias="thoughtspotLiveboardQualifiedName"
+        )
+        thoughtspot_liveboard: Optional[ThoughtspotLiveboard] = Field(
+            None, description="", alias="thoughtspotLiveboard"
+        )  # relationship
+
+    attributes: "ThoughtspotDashlet.Attributes" = Field(
+        default_factory=lambda: ThoughtspotDashlet.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class ThoughtspotAnswer(Thoughtspot):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in ThoughtspotAnswer._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = []
+
+    type_name: str = Field("ThoughtspotAnswer", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "ThoughtspotAnswer":
+            raise ValueError("must be ThoughtspotAnswer")
+        return v
+
+
+class PowerBIReport(PowerBI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in PowerBIReport._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "workspace_qualified_name",
+        "dataset_qualified_name",
+        "web_url",
+        "page_count",
+        "workspace",
+        "tiles",
+        "pages",
+        "dataset",
+    ]
+
+    @property
+    def workspace_qualified_name(self) -> Optional[str]:
+        return self.attributes.workspace_qualified_name
+
+    @workspace_qualified_name.setter
+    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace_qualified_name = workspace_qualified_name
+
+    @property
+    def dataset_qualified_name(self) -> Optional[str]:
+        return self.attributes.dataset_qualified_name
+
+    @dataset_qualified_name.setter
+    def dataset_qualified_name(self, dataset_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataset_qualified_name = dataset_qualified_name
+
+    @property
+    def web_url(self) -> Optional[str]:
+        return self.attributes.web_url
+
+    @web_url.setter
+    def web_url(self, web_url: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.web_url = web_url
+
+    @property
+    def page_count(self) -> Optional[int]:
+        return self.attributes.page_count
+
+    @page_count.setter
+    def page_count(self, page_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.page_count = page_count
+
+    @property
+    def workspace(self) -> Optional[PowerBIWorkspace]:
+        return self.attributes.workspace
+
+    @workspace.setter
+    def workspace(self, workspace: Optional[PowerBIWorkspace]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace = workspace
+
+    @property
+    def tiles(self) -> Optional[list[PowerBITile]]:
+        return self.attributes.tiles
+
+    @tiles.setter
+    def tiles(self, tiles: Optional[list[PowerBITile]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tiles = tiles
+
+    @property
+    def pages(self) -> Optional[list[PowerBIPage]]:
+        return self.attributes.pages
+
+    @pages.setter
+    def pages(self, pages: Optional[list[PowerBIPage]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.pages = pages
+
+    @property
+    def dataset(self) -> Optional[PowerBIDataset]:
+        return self.attributes.dataset
+
+    @dataset.setter
+    def dataset(self, dataset: Optional[PowerBIDataset]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataset = dataset
+
+    type_name: str = Field("PowerBIReport", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIReport":
+            raise ValueError("must be PowerBIReport")
+        return v
+
+    class Attributes(PowerBI.Attributes):
+        workspace_qualified_name: Optional[str] = Field(
+            None, description="", alias="workspaceQualifiedName"
+        )
+        dataset_qualified_name: Optional[str] = Field(
+            None, description="", alias="datasetQualifiedName"
+        )
+        web_url: Optional[str] = Field(None, description="", alias="webUrl")
+        page_count: Optional[int] = Field(None, description="", alias="pageCount")
+        workspace: Optional[PowerBIWorkspace] = Field(
+            None, description="", alias="workspace"
+        )  # relationship
+        tiles: Optional[list[PowerBITile]] = Field(
+            None, description="", alias="tiles"
+        )  # relationship
+        pages: Optional[list[PowerBIPage]] = Field(
+            None, description="", alias="pages"
+        )  # relationship
+        dataset: Optional[PowerBIDataset] = Field(
+            None, description="", alias="dataset"
+        )  # relationship
+
+    attributes: "PowerBIReport.Attributes" = Field(
+        default_factory=lambda: PowerBIReport.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class PowerBIMeasure(PowerBI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in PowerBIMeasure._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "workspace_qualified_name",
+        "dataset_qualified_name",
+        "power_b_i_measure_expression",
+        "power_b_i_is_external_measure",
+        "table",
+    ]
+
+    @property
+    def workspace_qualified_name(self) -> Optional[str]:
+        return self.attributes.workspace_qualified_name
+
+    @workspace_qualified_name.setter
+    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace_qualified_name = workspace_qualified_name
+
+    @property
+    def dataset_qualified_name(self) -> Optional[str]:
+        return self.attributes.dataset_qualified_name
+
+    @dataset_qualified_name.setter
+    def dataset_qualified_name(self, dataset_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataset_qualified_name = dataset_qualified_name
+
+    @property
+    def power_b_i_measure_expression(self) -> Optional[str]:
+        return self.attributes.power_b_i_measure_expression
+
+    @power_b_i_measure_expression.setter
+    def power_b_i_measure_expression(self, power_b_i_measure_expression: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.power_b_i_measure_expression = power_b_i_measure_expression
+
+    @property
+    def power_b_i_is_external_measure(self) -> Optional[bool]:
+        return self.attributes.power_b_i_is_external_measure
+
+    @power_b_i_is_external_measure.setter
+    def power_b_i_is_external_measure(
+        self, power_b_i_is_external_measure: Optional[bool]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.power_b_i_is_external_measure = power_b_i_is_external_measure
+
+    @property
+    def table(self) -> Optional[PowerBITable]:
+        return self.attributes.table
+
+    @table.setter
+    def table(self, table: Optional[PowerBITable]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.table = table
+
+    type_name: str = Field("PowerBIMeasure", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIMeasure":
+            raise ValueError("must be PowerBIMeasure")
+        return v
+
+    class Attributes(PowerBI.Attributes):
+        workspace_qualified_name: Optional[str] = Field(
+            None, description="", alias="workspaceQualifiedName"
+        )
+        dataset_qualified_name: Optional[str] = Field(
+            None, description="", alias="datasetQualifiedName"
+        )
+        power_b_i_measure_expression: Optional[str] = Field(
+            None, description="", alias="powerBIMeasureExpression"
+        )
+        power_b_i_is_external_measure: Optional[bool] = Field(
+            None, description="", alias="powerBIIsExternalMeasure"
+        )
+        table: Optional[PowerBITable] = Field(
+            None, description="", alias="table"
+        )  # relationship
+
+    attributes: "PowerBIMeasure.Attributes" = Field(
+        default_factory=lambda: PowerBIMeasure.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class PowerBIColumn(PowerBI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in PowerBIColumn._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "workspace_qualified_name",
+        "dataset_qualified_name",
+        "power_b_i_column_data_category",
+        "power_b_i_column_data_type",
+        "power_b_i_sort_by_column",
+        "power_b_i_column_summarize_by",
+        "table",
+    ]
+
+    @property
+    def workspace_qualified_name(self) -> Optional[str]:
+        return self.attributes.workspace_qualified_name
+
+    @workspace_qualified_name.setter
+    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace_qualified_name = workspace_qualified_name
+
+    @property
+    def dataset_qualified_name(self) -> Optional[str]:
+        return self.attributes.dataset_qualified_name
+
+    @dataset_qualified_name.setter
+    def dataset_qualified_name(self, dataset_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataset_qualified_name = dataset_qualified_name
+
+    @property
+    def power_b_i_column_data_category(self) -> Optional[str]:
+        return self.attributes.power_b_i_column_data_category
+
+    @power_b_i_column_data_category.setter
+    def power_b_i_column_data_category(
+        self, power_b_i_column_data_category: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.power_b_i_column_data_category = power_b_i_column_data_category
+
+    @property
+    def power_b_i_column_data_type(self) -> Optional[str]:
+        return self.attributes.power_b_i_column_data_type
+
+    @power_b_i_column_data_type.setter
+    def power_b_i_column_data_type(self, power_b_i_column_data_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.power_b_i_column_data_type = power_b_i_column_data_type
+
+    @property
+    def power_b_i_sort_by_column(self) -> Optional[str]:
+        return self.attributes.power_b_i_sort_by_column
+
+    @power_b_i_sort_by_column.setter
+    def power_b_i_sort_by_column(self, power_b_i_sort_by_column: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.power_b_i_sort_by_column = power_b_i_sort_by_column
+
+    @property
+    def power_b_i_column_summarize_by(self) -> Optional[str]:
+        return self.attributes.power_b_i_column_summarize_by
+
+    @power_b_i_column_summarize_by.setter
+    def power_b_i_column_summarize_by(
+        self, power_b_i_column_summarize_by: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.power_b_i_column_summarize_by = power_b_i_column_summarize_by
+
+    @property
+    def table(self) -> Optional[PowerBITable]:
+        return self.attributes.table
+
+    @table.setter
+    def table(self, table: Optional[PowerBITable]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.table = table
+
+    type_name: str = Field("PowerBIColumn", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIColumn":
+            raise ValueError("must be PowerBIColumn")
+        return v
+
+    class Attributes(PowerBI.Attributes):
+        workspace_qualified_name: Optional[str] = Field(
+            None, description="", alias="workspaceQualifiedName"
+        )
+        dataset_qualified_name: Optional[str] = Field(
+            None, description="", alias="datasetQualifiedName"
+        )
+        power_b_i_column_data_category: Optional[str] = Field(
+            None, description="", alias="powerBIColumnDataCategory"
+        )
+        power_b_i_column_data_type: Optional[str] = Field(
+            None, description="", alias="powerBIColumnDataType"
+        )
+        power_b_i_sort_by_column: Optional[str] = Field(
+            None, description="", alias="powerBISortByColumn"
+        )
+        power_b_i_column_summarize_by: Optional[str] = Field(
+            None, description="", alias="powerBIColumnSummarizeBy"
+        )
+        table: Optional[PowerBITable] = Field(
+            None, description="", alias="table"
+        )  # relationship
+
+    attributes: "PowerBIColumn.Attributes" = Field(
+        default_factory=lambda: PowerBIColumn.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class PowerBITable(PowerBI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in PowerBITable._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "workspace_qualified_name",
+        "dataset_qualified_name",
+        "power_b_i_table_source_expressions",
+        "power_b_i_table_column_count",
+        "power_b_i_table_measure_count",
+        "measures",
+        "columns",
+        "dataset",
+    ]
+
+    @property
+    def workspace_qualified_name(self) -> Optional[str]:
+        return self.attributes.workspace_qualified_name
+
+    @workspace_qualified_name.setter
+    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace_qualified_name = workspace_qualified_name
+
+    @property
+    def dataset_qualified_name(self) -> Optional[str]:
+        return self.attributes.dataset_qualified_name
+
+    @dataset_qualified_name.setter
+    def dataset_qualified_name(self, dataset_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataset_qualified_name = dataset_qualified_name
+
+    @property
+    def power_b_i_table_source_expressions(self) -> Optional[set[str]]:
+        return self.attributes.power_b_i_table_source_expressions
+
+    @power_b_i_table_source_expressions.setter
+    def power_b_i_table_source_expressions(
+        self, power_b_i_table_source_expressions: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.power_b_i_table_source_expressions = (
+            power_b_i_table_source_expressions
+        )
+
+    @property
+    def power_b_i_table_column_count(self) -> Optional[int]:
+        return self.attributes.power_b_i_table_column_count
+
+    @power_b_i_table_column_count.setter
+    def power_b_i_table_column_count(self, power_b_i_table_column_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.power_b_i_table_column_count = power_b_i_table_column_count
+
+    @property
+    def power_b_i_table_measure_count(self) -> Optional[int]:
+        return self.attributes.power_b_i_table_measure_count
+
+    @power_b_i_table_measure_count.setter
+    def power_b_i_table_measure_count(
+        self, power_b_i_table_measure_count: Optional[int]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.power_b_i_table_measure_count = power_b_i_table_measure_count
+
+    @property
+    def measures(self) -> Optional[list[PowerBIMeasure]]:
+        return self.attributes.measures
+
+    @measures.setter
+    def measures(self, measures: Optional[list[PowerBIMeasure]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.measures = measures
+
+    @property
+    def columns(self) -> Optional[list[PowerBIColumn]]:
+        return self.attributes.columns
+
+    @columns.setter
+    def columns(self, columns: Optional[list[PowerBIColumn]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.columns = columns
+
+    @property
+    def dataset(self) -> Optional[PowerBIDataset]:
+        return self.attributes.dataset
+
+    @dataset.setter
+    def dataset(self, dataset: Optional[PowerBIDataset]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataset = dataset
+
+    type_name: str = Field("PowerBITable", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBITable":
+            raise ValueError("must be PowerBITable")
+        return v
+
+    class Attributes(PowerBI.Attributes):
+        workspace_qualified_name: Optional[str] = Field(
+            None, description="", alias="workspaceQualifiedName"
+        )
+        dataset_qualified_name: Optional[str] = Field(
+            None, description="", alias="datasetQualifiedName"
+        )
+        power_b_i_table_source_expressions: Optional[set[str]] = Field(
+            None, description="", alias="powerBITableSourceExpressions"
+        )
+        power_b_i_table_column_count: Optional[int] = Field(
+            None, description="", alias="powerBITableColumnCount"
+        )
+        power_b_i_table_measure_count: Optional[int] = Field(
+            None, description="", alias="powerBITableMeasureCount"
+        )
+        measures: Optional[list[PowerBIMeasure]] = Field(
+            None, description="", alias="measures"
+        )  # relationship
+        columns: Optional[list[PowerBIColumn]] = Field(
+            None, description="", alias="columns"
+        )  # relationship
+        dataset: Optional[PowerBIDataset] = Field(
+            None, description="", alias="dataset"
+        )  # relationship
+
+    attributes: "PowerBITable.Attributes" = Field(
+        default_factory=lambda: PowerBITable.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class PowerBITile(PowerBI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in PowerBITile._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "workspace_qualified_name",
+        "dashboard_qualified_name",
+        "report",
+        "dataset",
+        "dashboard",
+    ]
+
+    @property
+    def workspace_qualified_name(self) -> Optional[str]:
+        return self.attributes.workspace_qualified_name
+
+    @workspace_qualified_name.setter
+    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace_qualified_name = workspace_qualified_name
+
+    @property
+    def dashboard_qualified_name(self) -> Optional[str]:
+        return self.attributes.dashboard_qualified_name
+
+    @dashboard_qualified_name.setter
+    def dashboard_qualified_name(self, dashboard_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dashboard_qualified_name = dashboard_qualified_name
+
+    @property
+    def report(self) -> Optional[PowerBIReport]:
+        return self.attributes.report
+
+    @report.setter
+    def report(self, report: Optional[PowerBIReport]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.report = report
+
+    @property
+    def dataset(self) -> Optional[PowerBIDataset]:
+        return self.attributes.dataset
+
+    @dataset.setter
+    def dataset(self, dataset: Optional[PowerBIDataset]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataset = dataset
+
+    @property
+    def dashboard(self) -> Optional[PowerBIDashboard]:
+        return self.attributes.dashboard
+
+    @dashboard.setter
+    def dashboard(self, dashboard: Optional[PowerBIDashboard]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dashboard = dashboard
+
+    type_name: str = Field("PowerBITile", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBITile":
+            raise ValueError("must be PowerBITile")
+        return v
+
+    class Attributes(PowerBI.Attributes):
+        workspace_qualified_name: Optional[str] = Field(
+            None, description="", alias="workspaceQualifiedName"
+        )
+        dashboard_qualified_name: Optional[str] = Field(
+            None, description="", alias="dashboardQualifiedName"
+        )
+        report: Optional[PowerBIReport] = Field(
+            None, description="", alias="report"
+        )  # relationship
+        dataset: Optional[PowerBIDataset] = Field(
+            None, description="", alias="dataset"
+        )  # relationship
+        dashboard: Optional[PowerBIDashboard] = Field(
+            None, description="", alias="dashboard"
+        )  # relationship
+
+    attributes: "PowerBITile.Attributes" = Field(
+        default_factory=lambda: PowerBITile.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class PowerBIDatasource(PowerBI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in PowerBIDatasource._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "connection_details",
+        "datasets",
+    ]
+
+    @property
+    def connection_details(self) -> Optional[dict[str, str]]:
+        return self.attributes.connection_details
+
+    @connection_details.setter
+    def connection_details(self, connection_details: Optional[dict[str, str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.connection_details = connection_details
+
+    @property
+    def datasets(self) -> Optional[list[PowerBIDataset]]:
+        return self.attributes.datasets
+
+    @datasets.setter
+    def datasets(self, datasets: Optional[list[PowerBIDataset]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.datasets = datasets
+
+    type_name: str = Field("PowerBIDatasource", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIDatasource":
+            raise ValueError("must be PowerBIDatasource")
+        return v
+
+    class Attributes(PowerBI.Attributes):
+        connection_details: Optional[dict[str, str]] = Field(
+            None, description="", alias="connectionDetails"
+        )
+        datasets: Optional[list[PowerBIDataset]] = Field(
+            None, description="", alias="datasets"
+        )  # relationship
+
+    attributes: "PowerBIDatasource.Attributes" = Field(
+        default_factory=lambda: PowerBIDatasource.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class PowerBIWorkspace(PowerBI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in PowerBIWorkspace._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "web_url",
+        "report_count",
+        "dashboard_count",
+        "dataset_count",
+        "dataflow_count",
+        "reports",
+        "datasets",
+        "dashboards",
+        "dataflows",
+    ]
+
+    @property
+    def web_url(self) -> Optional[str]:
+        return self.attributes.web_url
+
+    @web_url.setter
+    def web_url(self, web_url: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.web_url = web_url
+
+    @property
+    def report_count(self) -> Optional[int]:
+        return self.attributes.report_count
+
+    @report_count.setter
+    def report_count(self, report_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.report_count = report_count
+
+    @property
+    def dashboard_count(self) -> Optional[int]:
+        return self.attributes.dashboard_count
+
+    @dashboard_count.setter
+    def dashboard_count(self, dashboard_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dashboard_count = dashboard_count
+
+    @property
+    def dataset_count(self) -> Optional[int]:
+        return self.attributes.dataset_count
+
+    @dataset_count.setter
+    def dataset_count(self, dataset_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataset_count = dataset_count
+
+    @property
+    def dataflow_count(self) -> Optional[int]:
+        return self.attributes.dataflow_count
+
+    @dataflow_count.setter
+    def dataflow_count(self, dataflow_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataflow_count = dataflow_count
+
+    @property
+    def reports(self) -> Optional[list[PowerBIReport]]:
+        return self.attributes.reports
+
+    @reports.setter
+    def reports(self, reports: Optional[list[PowerBIReport]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.reports = reports
+
+    @property
+    def datasets(self) -> Optional[list[PowerBIDataset]]:
+        return self.attributes.datasets
+
+    @datasets.setter
+    def datasets(self, datasets: Optional[list[PowerBIDataset]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.datasets = datasets
+
+    @property
+    def dashboards(self) -> Optional[list[PowerBIDashboard]]:
+        return self.attributes.dashboards
+
+    @dashboards.setter
+    def dashboards(self, dashboards: Optional[list[PowerBIDashboard]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dashboards = dashboards
+
+    @property
+    def dataflows(self) -> Optional[list[PowerBIDataflow]]:
+        return self.attributes.dataflows
+
+    @dataflows.setter
+    def dataflows(self, dataflows: Optional[list[PowerBIDataflow]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataflows = dataflows
+
+    type_name: str = Field("PowerBIWorkspace", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIWorkspace":
+            raise ValueError("must be PowerBIWorkspace")
+        return v
+
+    class Attributes(PowerBI.Attributes):
+        web_url: Optional[str] = Field(None, description="", alias="webUrl")
+        report_count: Optional[int] = Field(None, description="", alias="reportCount")
+        dashboard_count: Optional[int] = Field(
+            None, description="", alias="dashboardCount"
+        )
+        dataset_count: Optional[int] = Field(None, description="", alias="datasetCount")
+        dataflow_count: Optional[int] = Field(
+            None, description="", alias="dataflowCount"
+        )
+        reports: Optional[list[PowerBIReport]] = Field(
+            None, description="", alias="reports"
+        )  # relationship
+        datasets: Optional[list[PowerBIDataset]] = Field(
+            None, description="", alias="datasets"
+        )  # relationship
+        dashboards: Optional[list[PowerBIDashboard]] = Field(
+            None, description="", alias="dashboards"
+        )  # relationship
+        dataflows: Optional[list[PowerBIDataflow]] = Field(
+            None, description="", alias="dataflows"
+        )  # relationship
+
+    attributes: "PowerBIWorkspace.Attributes" = Field(
+        default_factory=lambda: PowerBIWorkspace.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class PowerBIDataset(PowerBI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in PowerBIDataset._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "workspace_qualified_name",
+        "web_url",
+        "reports",
+        "workspace",
+        "dataflows",
+        "tiles",
+        "tables",
+        "datasources",
+    ]
+
+    @property
+    def workspace_qualified_name(self) -> Optional[str]:
+        return self.attributes.workspace_qualified_name
+
+    @workspace_qualified_name.setter
+    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace_qualified_name = workspace_qualified_name
+
+    @property
+    def web_url(self) -> Optional[str]:
+        return self.attributes.web_url
+
+    @web_url.setter
+    def web_url(self, web_url: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.web_url = web_url
+
+    @property
+    def reports(self) -> Optional[list[PowerBIReport]]:
+        return self.attributes.reports
+
+    @reports.setter
+    def reports(self, reports: Optional[list[PowerBIReport]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.reports = reports
+
+    @property
+    def workspace(self) -> Optional[PowerBIWorkspace]:
+        return self.attributes.workspace
+
+    @workspace.setter
+    def workspace(self, workspace: Optional[PowerBIWorkspace]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace = workspace
+
+    @property
+    def dataflows(self) -> Optional[list[PowerBIDataflow]]:
+        return self.attributes.dataflows
+
+    @dataflows.setter
+    def dataflows(self, dataflows: Optional[list[PowerBIDataflow]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.dataflows = dataflows
+
+    @property
+    def tiles(self) -> Optional[list[PowerBITile]]:
+        return self.attributes.tiles
+
+    @tiles.setter
+    def tiles(self, tiles: Optional[list[PowerBITile]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tiles = tiles
+
+    @property
+    def tables(self) -> Optional[list[PowerBITable]]:
+        return self.attributes.tables
+
+    @tables.setter
+    def tables(self, tables: Optional[list[PowerBITable]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tables = tables
+
+    @property
+    def datasources(self) -> Optional[list[PowerBIDatasource]]:
+        return self.attributes.datasources
+
+    @datasources.setter
+    def datasources(self, datasources: Optional[list[PowerBIDatasource]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.datasources = datasources
+
+    type_name: str = Field("PowerBIDataset", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIDataset":
+            raise ValueError("must be PowerBIDataset")
+        return v
+
+    class Attributes(PowerBI.Attributes):
+        workspace_qualified_name: Optional[str] = Field(
+            None, description="", alias="workspaceQualifiedName"
+        )
+        web_url: Optional[str] = Field(None, description="", alias="webUrl")
+        reports: Optional[list[PowerBIReport]] = Field(
+            None, description="", alias="reports"
+        )  # relationship
+        workspace: Optional[PowerBIWorkspace] = Field(
+            None, description="", alias="workspace"
+        )  # relationship
+        dataflows: Optional[list[PowerBIDataflow]] = Field(
+            None, description="", alias="dataflows"
+        )  # relationship
+        tiles: Optional[list[PowerBITile]] = Field(
+            None, description="", alias="tiles"
+        )  # relationship
+        tables: Optional[list[PowerBITable]] = Field(
+            None, description="", alias="tables"
+        )  # relationship
+        datasources: Optional[list[PowerBIDatasource]] = Field(
+            None, description="", alias="datasources"
+        )  # relationship
+
+    attributes: "PowerBIDataset.Attributes" = Field(
+        default_factory=lambda: PowerBIDataset.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class PowerBIDashboard(PowerBI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in PowerBIDashboard._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "workspace_qualified_name",
+        "web_url",
+        "tile_count",
+        "tiles",
+        "workspace",
+    ]
+
+    @property
+    def workspace_qualified_name(self) -> Optional[str]:
+        return self.attributes.workspace_qualified_name
+
+    @workspace_qualified_name.setter
+    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace_qualified_name = workspace_qualified_name
+
+    @property
+    def web_url(self) -> Optional[str]:
+        return self.attributes.web_url
+
+    @web_url.setter
+    def web_url(self, web_url: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.web_url = web_url
+
+    @property
+    def tile_count(self) -> Optional[int]:
+        return self.attributes.tile_count
+
+    @tile_count.setter
+    def tile_count(self, tile_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tile_count = tile_count
+
+    @property
+    def tiles(self) -> Optional[list[PowerBITile]]:
+        return self.attributes.tiles
+
+    @tiles.setter
+    def tiles(self, tiles: Optional[list[PowerBITile]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tiles = tiles
+
+    @property
+    def workspace(self) -> Optional[PowerBIWorkspace]:
+        return self.attributes.workspace
+
+    @workspace.setter
+    def workspace(self, workspace: Optional[PowerBIWorkspace]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace = workspace
+
+    type_name: str = Field("PowerBIDashboard", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIDashboard":
+            raise ValueError("must be PowerBIDashboard")
+        return v
+
+    class Attributes(PowerBI.Attributes):
+        workspace_qualified_name: Optional[str] = Field(
+            None, description="", alias="workspaceQualifiedName"
+        )
+        web_url: Optional[str] = Field(None, description="", alias="webUrl")
+        tile_count: Optional[int] = Field(None, description="", alias="tileCount")
+        tiles: Optional[list[PowerBITile]] = Field(
+            None, description="", alias="tiles"
+        )  # relationship
+        workspace: Optional[PowerBIWorkspace] = Field(
+            None, description="", alias="workspace"
+        )  # relationship
+
+    attributes: "PowerBIDashboard.Attributes" = Field(
+        default_factory=lambda: PowerBIDashboard.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class PowerBIDataflow(PowerBI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in PowerBIDataflow._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "workspace_qualified_name",
+        "web_url",
+        "workspace",
+        "datasets",
+    ]
+
+    @property
+    def workspace_qualified_name(self) -> Optional[str]:
+        return self.attributes.workspace_qualified_name
+
+    @workspace_qualified_name.setter
+    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace_qualified_name = workspace_qualified_name
+
+    @property
+    def web_url(self) -> Optional[str]:
+        return self.attributes.web_url
+
+    @web_url.setter
+    def web_url(self, web_url: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.web_url = web_url
+
+    @property
+    def workspace(self) -> Optional[PowerBIWorkspace]:
+        return self.attributes.workspace
+
+    @workspace.setter
+    def workspace(self, workspace: Optional[PowerBIWorkspace]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace = workspace
+
+    @property
+    def datasets(self) -> Optional[list[PowerBIDataset]]:
+        return self.attributes.datasets
+
+    @datasets.setter
+    def datasets(self, datasets: Optional[list[PowerBIDataset]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.datasets = datasets
+
+    type_name: str = Field("PowerBIDataflow", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIDataflow":
+            raise ValueError("must be PowerBIDataflow")
+        return v
+
+    class Attributes(PowerBI.Attributes):
+        workspace_qualified_name: Optional[str] = Field(
+            None, description="", alias="workspaceQualifiedName"
+        )
+        web_url: Optional[str] = Field(None, description="", alias="webUrl")
+        workspace: Optional[PowerBIWorkspace] = Field(
+            None, description="", alias="workspace"
+        )  # relationship
+        datasets: Optional[list[PowerBIDataset]] = Field(
+            None, description="", alias="datasets"
+        )  # relationship
+
+    attributes: "PowerBIDataflow.Attributes" = Field(
+        default_factory=lambda: PowerBIDataflow.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class PowerBIPage(PowerBI):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in PowerBIPage._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "workspace_qualified_name",
+        "report_qualified_name",
+        "report",
+    ]
+
+    @property
+    def workspace_qualified_name(self) -> Optional[str]:
+        return self.attributes.workspace_qualified_name
+
+    @workspace_qualified_name.setter
+    def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.workspace_qualified_name = workspace_qualified_name
+
+    @property
+    def report_qualified_name(self) -> Optional[str]:
+        return self.attributes.report_qualified_name
+
+    @report_qualified_name.setter
+    def report_qualified_name(self, report_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.report_qualified_name = report_qualified_name
+
+    @property
+    def report(self) -> Optional[PowerBIReport]:
+        return self.attributes.report
+
+    @report.setter
+    def report(self, report: Optional[PowerBIReport]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.report = report
+
+    type_name: str = Field("PowerBIPage", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "PowerBIPage":
+            raise ValueError("must be PowerBIPage")
+        return v
+
+    class Attributes(PowerBI.Attributes):
+        workspace_qualified_name: Optional[str] = Field(
+            None, description="", alias="workspaceQualifiedName"
+        )
+        report_qualified_name: Optional[str] = Field(
+            None, description="", alias="reportQualifiedName"
+        )
+        report: Optional[PowerBIReport] = Field(
+            None, description="", alias="report"
+        )  # relationship
+
+    attributes: "PowerBIPage.Attributes" = Field(
+        default_factory=lambda: PowerBIPage.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class MicroStrategyReport(MicroStrategy):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MicroStrategyReport._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "micro_strategy_report_type",
+        "micro_strategy_metrics",
+        "micro_strategy_project",
+        "micro_strategy_attributes",
+    ]
+
+    @property
+    def micro_strategy_report_type(self) -> Optional[str]:
+        return self.attributes.micro_strategy_report_type
+
+    @micro_strategy_report_type.setter
+    def micro_strategy_report_type(self, micro_strategy_report_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_report_type = micro_strategy_report_type
+
+    @property
+    def micro_strategy_metrics(self) -> Optional[list[MicroStrategyMetric]]:
+        return self.attributes.micro_strategy_metrics
+
+    @micro_strategy_metrics.setter
+    def micro_strategy_metrics(
+        self, micro_strategy_metrics: Optional[list[MicroStrategyMetric]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_metrics = micro_strategy_metrics
+
+    @property
+    def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
+        return self.attributes.micro_strategy_project
+
+    @micro_strategy_project.setter
+    def micro_strategy_project(
+        self, micro_strategy_project: Optional[MicroStrategyProject]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_project = micro_strategy_project
+
+    @property
+    def micro_strategy_attributes(self) -> Optional[list[MicroStrategyAttribute]]:
+        return self.attributes.micro_strategy_attributes
+
+    @micro_strategy_attributes.setter
+    def micro_strategy_attributes(
+        self, micro_strategy_attributes: Optional[list[MicroStrategyAttribute]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_attributes = micro_strategy_attributes
+
+    type_name: str = Field("MicroStrategyReport", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyReport":
+            raise ValueError("must be MicroStrategyReport")
+        return v
+
+    class Attributes(MicroStrategy.Attributes):
+        micro_strategy_report_type: Optional[str] = Field(
+            None, description="", alias="microStrategyReportType"
+        )
+        micro_strategy_metrics: Optional[list[MicroStrategyMetric]] = Field(
+            None, description="", alias="microStrategyMetrics"
+        )  # relationship
+        micro_strategy_project: Optional[MicroStrategyProject] = Field(
+            None, description="", alias="microStrategyProject"
+        )  # relationship
+        micro_strategy_attributes: Optional[list[MicroStrategyAttribute]] = Field(
+            None, description="", alias="microStrategyAttributes"
+        )  # relationship
+
+    attributes: "MicroStrategyReport.Attributes" = Field(
+        default_factory=lambda: MicroStrategyReport.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class MicroStrategyProject(MicroStrategy):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MicroStrategyProject._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "micro_strategy_reports",
+        "micro_strategy_facts",
+        "micro_strategy_metrics",
+        "micro_strategy_visualizations",
+        "micro_strategy_documents",
+        "micro_strategy_cubes",
+        "micro_strategy_dossiers",
+        "micro_strategy_attributes",
+    ]
+
+    @property
+    def micro_strategy_reports(self) -> Optional[list[MicroStrategyReport]]:
+        return self.attributes.micro_strategy_reports
+
+    @micro_strategy_reports.setter
+    def micro_strategy_reports(
+        self, micro_strategy_reports: Optional[list[MicroStrategyReport]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_reports = micro_strategy_reports
+
+    @property
+    def micro_strategy_facts(self) -> Optional[list[MicroStrategyFact]]:
+        return self.attributes.micro_strategy_facts
+
+    @micro_strategy_facts.setter
+    def micro_strategy_facts(
+        self, micro_strategy_facts: Optional[list[MicroStrategyFact]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_facts = micro_strategy_facts
+
+    @property
+    def micro_strategy_metrics(self) -> Optional[list[MicroStrategyMetric]]:
+        return self.attributes.micro_strategy_metrics
+
+    @micro_strategy_metrics.setter
+    def micro_strategy_metrics(
+        self, micro_strategy_metrics: Optional[list[MicroStrategyMetric]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_metrics = micro_strategy_metrics
+
+    @property
+    def micro_strategy_visualizations(
+        self,
+    ) -> Optional[list[MicroStrategyVisualization]]:
+        return self.attributes.micro_strategy_visualizations
+
+    @micro_strategy_visualizations.setter
+    def micro_strategy_visualizations(
+        self, micro_strategy_visualizations: Optional[list[MicroStrategyVisualization]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_visualizations = micro_strategy_visualizations
+
+    @property
+    def micro_strategy_documents(self) -> Optional[list[MicroStrategyDocument]]:
+        return self.attributes.micro_strategy_documents
+
+    @micro_strategy_documents.setter
+    def micro_strategy_documents(
+        self, micro_strategy_documents: Optional[list[MicroStrategyDocument]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_documents = micro_strategy_documents
+
+    @property
+    def micro_strategy_cubes(self) -> Optional[list[MicroStrategyCube]]:
+        return self.attributes.micro_strategy_cubes
+
+    @micro_strategy_cubes.setter
+    def micro_strategy_cubes(
+        self, micro_strategy_cubes: Optional[list[MicroStrategyCube]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_cubes = micro_strategy_cubes
+
+    @property
+    def micro_strategy_dossiers(self) -> Optional[list[MicroStrategyDossier]]:
+        return self.attributes.micro_strategy_dossiers
+
+    @micro_strategy_dossiers.setter
+    def micro_strategy_dossiers(
+        self, micro_strategy_dossiers: Optional[list[MicroStrategyDossier]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_dossiers = micro_strategy_dossiers
+
+    @property
+    def micro_strategy_attributes(self) -> Optional[list[MicroStrategyAttribute]]:
+        return self.attributes.micro_strategy_attributes
+
+    @micro_strategy_attributes.setter
+    def micro_strategy_attributes(
+        self, micro_strategy_attributes: Optional[list[MicroStrategyAttribute]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_attributes = micro_strategy_attributes
+
+    type_name: str = Field("MicroStrategyProject", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyProject":
+            raise ValueError("must be MicroStrategyProject")
+        return v
+
+    class Attributes(MicroStrategy.Attributes):
+        micro_strategy_reports: Optional[list[MicroStrategyReport]] = Field(
+            None, description="", alias="microStrategyReports"
+        )  # relationship
+        micro_strategy_facts: Optional[list[MicroStrategyFact]] = Field(
+            None, description="", alias="microStrategyFacts"
+        )  # relationship
+        micro_strategy_metrics: Optional[list[MicroStrategyMetric]] = Field(
+            None, description="", alias="microStrategyMetrics"
+        )  # relationship
+        micro_strategy_visualizations: Optional[
+            list[MicroStrategyVisualization]
+        ] = Field(
+            None, description="", alias="microStrategyVisualizations"
+        )  # relationship
+        micro_strategy_documents: Optional[list[MicroStrategyDocument]] = Field(
+            None, description="", alias="microStrategyDocuments"
+        )  # relationship
+        micro_strategy_cubes: Optional[list[MicroStrategyCube]] = Field(
+            None, description="", alias="microStrategyCubes"
+        )  # relationship
+        micro_strategy_dossiers: Optional[list[MicroStrategyDossier]] = Field(
+            None, description="", alias="microStrategyDossiers"
+        )  # relationship
+        micro_strategy_attributes: Optional[list[MicroStrategyAttribute]] = Field(
+            None, description="", alias="microStrategyAttributes"
+        )  # relationship
+
+    attributes: "MicroStrategyProject.Attributes" = Field(
+        default_factory=lambda: MicroStrategyProject.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class MicroStrategyMetric(MicroStrategy):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MicroStrategyMetric._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "micro_strategy_metric_expression",
+        "micro_strategy_attribute_qualified_names",
+        "micro_strategy_attribute_names",
+        "micro_strategy_fact_qualified_names",
+        "micro_strategy_fact_names",
+        "micro_strategy_metric_parent_qualified_names",
+        "micro_strategy_metric_parent_names",
+        "micro_strategy_metric_parents",
+        "micro_strategy_facts",
+        "micro_strategy_reports",
+        "micro_strategy_cubes",
+        "micro_strategy_metric_children",
+        "micro_strategy_project",
+        "micro_strategy_attributes",
+    ]
+
+    @property
+    def micro_strategy_metric_expression(self) -> Optional[str]:
+        return self.attributes.micro_strategy_metric_expression
+
+    @micro_strategy_metric_expression.setter
+    def micro_strategy_metric_expression(
+        self, micro_strategy_metric_expression: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_metric_expression = (
+            micro_strategy_metric_expression
+        )
+
+    @property
+    def micro_strategy_attribute_qualified_names(self) -> Optional[set[str]]:
+        return self.attributes.micro_strategy_attribute_qualified_names
+
+    @micro_strategy_attribute_qualified_names.setter
+    def micro_strategy_attribute_qualified_names(
+        self, micro_strategy_attribute_qualified_names: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_attribute_qualified_names = (
+            micro_strategy_attribute_qualified_names
+        )
+
+    @property
+    def micro_strategy_attribute_names(self) -> Optional[set[str]]:
+        return self.attributes.micro_strategy_attribute_names
+
+    @micro_strategy_attribute_names.setter
+    def micro_strategy_attribute_names(
+        self, micro_strategy_attribute_names: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_attribute_names = micro_strategy_attribute_names
+
+    @property
+    def micro_strategy_fact_qualified_names(self) -> Optional[set[str]]:
+        return self.attributes.micro_strategy_fact_qualified_names
+
+    @micro_strategy_fact_qualified_names.setter
+    def micro_strategy_fact_qualified_names(
+        self, micro_strategy_fact_qualified_names: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_fact_qualified_names = (
+            micro_strategy_fact_qualified_names
+        )
+
+    @property
+    def micro_strategy_fact_names(self) -> Optional[set[str]]:
+        return self.attributes.micro_strategy_fact_names
+
+    @micro_strategy_fact_names.setter
+    def micro_strategy_fact_names(self, micro_strategy_fact_names: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_fact_names = micro_strategy_fact_names
+
+    @property
+    def micro_strategy_metric_parent_qualified_names(self) -> Optional[set[str]]:
+        return self.attributes.micro_strategy_metric_parent_qualified_names
+
+    @micro_strategy_metric_parent_qualified_names.setter
+    def micro_strategy_metric_parent_qualified_names(
+        self, micro_strategy_metric_parent_qualified_names: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_metric_parent_qualified_names = (
+            micro_strategy_metric_parent_qualified_names
+        )
+
+    @property
+    def micro_strategy_metric_parent_names(self) -> Optional[set[str]]:
+        return self.attributes.micro_strategy_metric_parent_names
+
+    @micro_strategy_metric_parent_names.setter
+    def micro_strategy_metric_parent_names(
+        self, micro_strategy_metric_parent_names: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_metric_parent_names = (
+            micro_strategy_metric_parent_names
+        )
+
+    @property
+    def micro_strategy_metric_parents(self) -> Optional[list[MicroStrategyMetric]]:
+        return self.attributes.micro_strategy_metric_parents
+
+    @micro_strategy_metric_parents.setter
+    def micro_strategy_metric_parents(
+        self, micro_strategy_metric_parents: Optional[list[MicroStrategyMetric]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_metric_parents = micro_strategy_metric_parents
+
+    @property
+    def micro_strategy_facts(self) -> Optional[list[MicroStrategyFact]]:
+        return self.attributes.micro_strategy_facts
+
+    @micro_strategy_facts.setter
+    def micro_strategy_facts(
+        self, micro_strategy_facts: Optional[list[MicroStrategyFact]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_facts = micro_strategy_facts
+
+    @property
+    def micro_strategy_reports(self) -> Optional[list[MicroStrategyReport]]:
+        return self.attributes.micro_strategy_reports
+
+    @micro_strategy_reports.setter
+    def micro_strategy_reports(
+        self, micro_strategy_reports: Optional[list[MicroStrategyReport]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_reports = micro_strategy_reports
+
+    @property
+    def micro_strategy_cubes(self) -> Optional[list[MicroStrategyCube]]:
+        return self.attributes.micro_strategy_cubes
+
+    @micro_strategy_cubes.setter
+    def micro_strategy_cubes(
+        self, micro_strategy_cubes: Optional[list[MicroStrategyCube]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_cubes = micro_strategy_cubes
+
+    @property
+    def micro_strategy_metric_children(self) -> Optional[list[MicroStrategyMetric]]:
+        return self.attributes.micro_strategy_metric_children
+
+    @micro_strategy_metric_children.setter
+    def micro_strategy_metric_children(
+        self, micro_strategy_metric_children: Optional[list[MicroStrategyMetric]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_metric_children = micro_strategy_metric_children
+
+    @property
+    def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
+        return self.attributes.micro_strategy_project
+
+    @micro_strategy_project.setter
+    def micro_strategy_project(
+        self, micro_strategy_project: Optional[MicroStrategyProject]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_project = micro_strategy_project
+
+    @property
+    def micro_strategy_attributes(self) -> Optional[list[MicroStrategyAttribute]]:
+        return self.attributes.micro_strategy_attributes
+
+    @micro_strategy_attributes.setter
+    def micro_strategy_attributes(
+        self, micro_strategy_attributes: Optional[list[MicroStrategyAttribute]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_attributes = micro_strategy_attributes
+
+    type_name: str = Field("MicroStrategyMetric", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyMetric":
+            raise ValueError("must be MicroStrategyMetric")
+        return v
+
+    class Attributes(MicroStrategy.Attributes):
+        micro_strategy_metric_expression: Optional[str] = Field(
+            None, description="", alias="microStrategyMetricExpression"
+        )
+        micro_strategy_attribute_qualified_names: Optional[set[str]] = Field(
+            None, description="", alias="microStrategyAttributeQualifiedNames"
+        )
+        micro_strategy_attribute_names: Optional[set[str]] = Field(
+            None, description="", alias="microStrategyAttributeNames"
+        )
+        micro_strategy_fact_qualified_names: Optional[set[str]] = Field(
+            None, description="", alias="microStrategyFactQualifiedNames"
+        )
+        micro_strategy_fact_names: Optional[set[str]] = Field(
+            None, description="", alias="microStrategyFactNames"
+        )
+        micro_strategy_metric_parent_qualified_names: Optional[set[str]] = Field(
+            None, description="", alias="microStrategyMetricParentQualifiedNames"
+        )
+        micro_strategy_metric_parent_names: Optional[set[str]] = Field(
+            None, description="", alias="microStrategyMetricParentNames"
+        )
+        micro_strategy_metric_parents: Optional[list[MicroStrategyMetric]] = Field(
+            None, description="", alias="microStrategyMetricParents"
+        )  # relationship
+        micro_strategy_facts: Optional[list[MicroStrategyFact]] = Field(
+            None, description="", alias="microStrategyFacts"
+        )  # relationship
+        micro_strategy_reports: Optional[list[MicroStrategyReport]] = Field(
+            None, description="", alias="microStrategyReports"
+        )  # relationship
+        micro_strategy_cubes: Optional[list[MicroStrategyCube]] = Field(
+            None, description="", alias="microStrategyCubes"
+        )  # relationship
+        micro_strategy_metric_children: Optional[list[MicroStrategyMetric]] = Field(
+            None, description="", alias="microStrategyMetricChildren"
+        )  # relationship
+        micro_strategy_project: Optional[MicroStrategyProject] = Field(
+            None, description="", alias="microStrategyProject"
+        )  # relationship
+        micro_strategy_attributes: Optional[list[MicroStrategyAttribute]] = Field(
+            None, description="", alias="microStrategyAttributes"
+        )  # relationship
+
+    attributes: "MicroStrategyMetric.Attributes" = Field(
+        default_factory=lambda: MicroStrategyMetric.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class MicroStrategyCube(MicroStrategy):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MicroStrategyCube._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "micro_strategy_cube_type",
+        "micro_strategy_cube_query",
+        "micro_strategy_metrics",
+        "micro_strategy_project",
+        "micro_strategy_attributes",
+    ]
+
+    @property
+    def micro_strategy_cube_type(self) -> Optional[str]:
+        return self.attributes.micro_strategy_cube_type
+
+    @micro_strategy_cube_type.setter
+    def micro_strategy_cube_type(self, micro_strategy_cube_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_cube_type = micro_strategy_cube_type
+
+    @property
+    def micro_strategy_cube_query(self) -> Optional[str]:
+        return self.attributes.micro_strategy_cube_query
+
+    @micro_strategy_cube_query.setter
+    def micro_strategy_cube_query(self, micro_strategy_cube_query: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_cube_query = micro_strategy_cube_query
+
+    @property
+    def micro_strategy_metrics(self) -> Optional[list[MicroStrategyMetric]]:
+        return self.attributes.micro_strategy_metrics
+
+    @micro_strategy_metrics.setter
+    def micro_strategy_metrics(
+        self, micro_strategy_metrics: Optional[list[MicroStrategyMetric]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_metrics = micro_strategy_metrics
+
+    @property
+    def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
+        return self.attributes.micro_strategy_project
+
+    @micro_strategy_project.setter
+    def micro_strategy_project(
+        self, micro_strategy_project: Optional[MicroStrategyProject]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_project = micro_strategy_project
+
+    @property
+    def micro_strategy_attributes(self) -> Optional[list[MicroStrategyAttribute]]:
+        return self.attributes.micro_strategy_attributes
+
+    @micro_strategy_attributes.setter
+    def micro_strategy_attributes(
+        self, micro_strategy_attributes: Optional[list[MicroStrategyAttribute]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_attributes = micro_strategy_attributes
+
+    type_name: str = Field("MicroStrategyCube", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyCube":
+            raise ValueError("must be MicroStrategyCube")
+        return v
+
+    class Attributes(MicroStrategy.Attributes):
+        micro_strategy_cube_type: Optional[str] = Field(
+            None, description="", alias="microStrategyCubeType"
+        )
+        micro_strategy_cube_query: Optional[str] = Field(
+            None, description="", alias="microStrategyCubeQuery"
+        )
+        micro_strategy_metrics: Optional[list[MicroStrategyMetric]] = Field(
+            None, description="", alias="microStrategyMetrics"
+        )  # relationship
+        micro_strategy_project: Optional[MicroStrategyProject] = Field(
+            None, description="", alias="microStrategyProject"
+        )  # relationship
+        micro_strategy_attributes: Optional[list[MicroStrategyAttribute]] = Field(
+            None, description="", alias="microStrategyAttributes"
+        )  # relationship
+
+    attributes: "MicroStrategyCube.Attributes" = Field(
+        default_factory=lambda: MicroStrategyCube.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class MicroStrategyDossier(MicroStrategy):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MicroStrategyDossier._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "micro_strategy_dossier_chapter_names",
+        "micro_strategy_project",
+        "micro_strategy_visualizations",
+    ]
+
+    @property
+    def micro_strategy_dossier_chapter_names(self) -> Optional[set[str]]:
+        return self.attributes.micro_strategy_dossier_chapter_names
+
+    @micro_strategy_dossier_chapter_names.setter
+    def micro_strategy_dossier_chapter_names(
+        self, micro_strategy_dossier_chapter_names: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_dossier_chapter_names = (
+            micro_strategy_dossier_chapter_names
+        )
+
+    @property
+    def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
+        return self.attributes.micro_strategy_project
+
+    @micro_strategy_project.setter
+    def micro_strategy_project(
+        self, micro_strategy_project: Optional[MicroStrategyProject]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_project = micro_strategy_project
+
+    @property
+    def micro_strategy_visualizations(
+        self,
+    ) -> Optional[list[MicroStrategyVisualization]]:
+        return self.attributes.micro_strategy_visualizations
+
+    @micro_strategy_visualizations.setter
+    def micro_strategy_visualizations(
+        self, micro_strategy_visualizations: Optional[list[MicroStrategyVisualization]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_visualizations = micro_strategy_visualizations
+
+    type_name: str = Field("MicroStrategyDossier", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyDossier":
+            raise ValueError("must be MicroStrategyDossier")
+        return v
+
+    class Attributes(MicroStrategy.Attributes):
+        micro_strategy_dossier_chapter_names: Optional[set[str]] = Field(
+            None, description="", alias="microStrategyDossierChapterNames"
+        )
+        micro_strategy_project: Optional[MicroStrategyProject] = Field(
+            None, description="", alias="microStrategyProject"
+        )  # relationship
+        micro_strategy_visualizations: Optional[
+            list[MicroStrategyVisualization]
+        ] = Field(
+            None, description="", alias="microStrategyVisualizations"
+        )  # relationship
+
+    attributes: "MicroStrategyDossier.Attributes" = Field(
+        default_factory=lambda: MicroStrategyDossier.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class MicroStrategyFact(MicroStrategy):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MicroStrategyFact._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "micro_strategy_fact_expressions",
+        "micro_strategy_metrics",
+        "micro_strategy_project",
+    ]
+
+    @property
+    def micro_strategy_fact_expressions(self) -> Optional[set[str]]:
+        return self.attributes.micro_strategy_fact_expressions
+
+    @micro_strategy_fact_expressions.setter
+    def micro_strategy_fact_expressions(
+        self, micro_strategy_fact_expressions: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_fact_expressions = (
+            micro_strategy_fact_expressions
+        )
+
+    @property
+    def micro_strategy_metrics(self) -> Optional[list[MicroStrategyMetric]]:
+        return self.attributes.micro_strategy_metrics
+
+    @micro_strategy_metrics.setter
+    def micro_strategy_metrics(
+        self, micro_strategy_metrics: Optional[list[MicroStrategyMetric]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_metrics = micro_strategy_metrics
+
+    @property
+    def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
+        return self.attributes.micro_strategy_project
+
+    @micro_strategy_project.setter
+    def micro_strategy_project(
+        self, micro_strategy_project: Optional[MicroStrategyProject]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_project = micro_strategy_project
+
+    type_name: str = Field("MicroStrategyFact", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyFact":
+            raise ValueError("must be MicroStrategyFact")
+        return v
+
+    class Attributes(MicroStrategy.Attributes):
+        micro_strategy_fact_expressions: Optional[set[str]] = Field(
+            None, description="", alias="microStrategyFactExpressions"
+        )
+        micro_strategy_metrics: Optional[list[MicroStrategyMetric]] = Field(
+            None, description="", alias="microStrategyMetrics"
+        )  # relationship
+        micro_strategy_project: Optional[MicroStrategyProject] = Field(
+            None, description="", alias="microStrategyProject"
+        )  # relationship
+
+    attributes: "MicroStrategyFact.Attributes" = Field(
+        default_factory=lambda: MicroStrategyFact.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class MicroStrategyDocument(MicroStrategy):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MicroStrategyDocument._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "micro_strategy_project",
+    ]
+
+    @property
+    def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
+        return self.attributes.micro_strategy_project
+
+    @micro_strategy_project.setter
+    def micro_strategy_project(
+        self, micro_strategy_project: Optional[MicroStrategyProject]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_project = micro_strategy_project
+
+    type_name: str = Field("MicroStrategyDocument", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyDocument":
+            raise ValueError("must be MicroStrategyDocument")
+        return v
+
+    class Attributes(MicroStrategy.Attributes):
+        micro_strategy_project: Optional[MicroStrategyProject] = Field(
+            None, description="", alias="microStrategyProject"
+        )  # relationship
+
+    attributes: "MicroStrategyDocument.Attributes" = Field(
+        default_factory=lambda: MicroStrategyDocument.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class MicroStrategyAttribute(MicroStrategy):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MicroStrategyAttribute._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "micro_strategy_attribute_forms",
+        "micro_strategy_reports",
+        "micro_strategy_metrics",
+        "micro_strategy_cubes",
+        "micro_strategy_project",
+    ]
+
+    @property
+    def micro_strategy_attribute_forms(self) -> Optional[str]:
+        return self.attributes.micro_strategy_attribute_forms
+
+    @micro_strategy_attribute_forms.setter
+    def micro_strategy_attribute_forms(
+        self, micro_strategy_attribute_forms: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_attribute_forms = micro_strategy_attribute_forms
+
+    @property
+    def micro_strategy_reports(self) -> Optional[list[MicroStrategyReport]]:
+        return self.attributes.micro_strategy_reports
+
+    @micro_strategy_reports.setter
+    def micro_strategy_reports(
+        self, micro_strategy_reports: Optional[list[MicroStrategyReport]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_reports = micro_strategy_reports
+
+    @property
+    def micro_strategy_metrics(self) -> Optional[list[MicroStrategyMetric]]:
+        return self.attributes.micro_strategy_metrics
+
+    @micro_strategy_metrics.setter
+    def micro_strategy_metrics(
+        self, micro_strategy_metrics: Optional[list[MicroStrategyMetric]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_metrics = micro_strategy_metrics
+
+    @property
+    def micro_strategy_cubes(self) -> Optional[list[MicroStrategyCube]]:
+        return self.attributes.micro_strategy_cubes
+
+    @micro_strategy_cubes.setter
+    def micro_strategy_cubes(
+        self, micro_strategy_cubes: Optional[list[MicroStrategyCube]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_cubes = micro_strategy_cubes
+
+    @property
+    def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
+        return self.attributes.micro_strategy_project
+
+    @micro_strategy_project.setter
+    def micro_strategy_project(
+        self, micro_strategy_project: Optional[MicroStrategyProject]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_project = micro_strategy_project
+
+    type_name: str = Field("MicroStrategyAttribute", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyAttribute":
+            raise ValueError("must be MicroStrategyAttribute")
+        return v
+
+    class Attributes(MicroStrategy.Attributes):
+        micro_strategy_attribute_forms: Optional[str] = Field(
+            None, description="", alias="microStrategyAttributeForms"
+        )
+        micro_strategy_reports: Optional[list[MicroStrategyReport]] = Field(
+            None, description="", alias="microStrategyReports"
+        )  # relationship
+        micro_strategy_metrics: Optional[list[MicroStrategyMetric]] = Field(
+            None, description="", alias="microStrategyMetrics"
+        )  # relationship
+        micro_strategy_cubes: Optional[list[MicroStrategyCube]] = Field(
+            None, description="", alias="microStrategyCubes"
+        )  # relationship
+        micro_strategy_project: Optional[MicroStrategyProject] = Field(
+            None, description="", alias="microStrategyProject"
+        )  # relationship
+
+    attributes: "MicroStrategyAttribute.Attributes" = Field(
+        default_factory=lambda: MicroStrategyAttribute.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class MicroStrategyVisualization(MicroStrategy):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MicroStrategyVisualization._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "micro_strategy_visualization_type",
+        "micro_strategy_dossier_qualified_name",
+        "micro_strategy_dossier_name",
+        "micro_strategy_dossier",
+        "micro_strategy_project",
+    ]
+
+    @property
+    def micro_strategy_visualization_type(self) -> Optional[str]:
+        return self.attributes.micro_strategy_visualization_type
+
+    @micro_strategy_visualization_type.setter
+    def micro_strategy_visualization_type(
+        self, micro_strategy_visualization_type: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_visualization_type = (
+            micro_strategy_visualization_type
+        )
+
+    @property
+    def micro_strategy_dossier_qualified_name(self) -> Optional[str]:
+        return self.attributes.micro_strategy_dossier_qualified_name
+
+    @micro_strategy_dossier_qualified_name.setter
+    def micro_strategy_dossier_qualified_name(
+        self, micro_strategy_dossier_qualified_name: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_dossier_qualified_name = (
+            micro_strategy_dossier_qualified_name
+        )
+
+    @property
+    def micro_strategy_dossier_name(self) -> Optional[str]:
+        return self.attributes.micro_strategy_dossier_name
+
+    @micro_strategy_dossier_name.setter
+    def micro_strategy_dossier_name(self, micro_strategy_dossier_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_dossier_name = micro_strategy_dossier_name
+
+    @property
+    def micro_strategy_dossier(self) -> Optional[MicroStrategyDossier]:
+        return self.attributes.micro_strategy_dossier
+
+    @micro_strategy_dossier.setter
+    def micro_strategy_dossier(
+        self, micro_strategy_dossier: Optional[MicroStrategyDossier]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_dossier = micro_strategy_dossier
+
+    @property
+    def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
+        return self.attributes.micro_strategy_project
+
+    @micro_strategy_project.setter
+    def micro_strategy_project(
+        self, micro_strategy_project: Optional[MicroStrategyProject]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.micro_strategy_project = micro_strategy_project
+
+    type_name: str = Field("MicroStrategyVisualization", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MicroStrategyVisualization":
+            raise ValueError("must be MicroStrategyVisualization")
+        return v
+
+    class Attributes(MicroStrategy.Attributes):
+        micro_strategy_visualization_type: Optional[str] = Field(
+            None, description="", alias="microStrategyVisualizationType"
+        )
+        micro_strategy_dossier_qualified_name: Optional[str] = Field(
+            None, description="", alias="microStrategyDossierQualifiedName"
+        )
+        micro_strategy_dossier_name: Optional[str] = Field(
+            None, description="", alias="microStrategyDossierName"
+        )
+        micro_strategy_dossier: Optional[MicroStrategyDossier] = Field(
+            None, description="", alias="microStrategyDossier"
+        )  # relationship
+        micro_strategy_project: Optional[MicroStrategyProject] = Field(
+            None, description="", alias="microStrategyProject"
+        )  # relationship
+
+    attributes: "MicroStrategyVisualization.Attributes" = Field(
+        default_factory=lambda: MicroStrategyVisualization.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class QlikSpace(Qlik):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in QlikSpace._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "qlik_space_type",
+        "qlik_datasets",
+        "qlik_apps",
+    ]
+
+    @property
+    def qlik_space_type(self) -> Optional[str]:
+        return self.attributes.qlik_space_type
+
+    @qlik_space_type.setter
+    def qlik_space_type(self, qlik_space_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_space_type = qlik_space_type
+
+    @property
+    def qlik_datasets(self) -> Optional[list[QlikDataset]]:
+        return self.attributes.qlik_datasets
+
+    @qlik_datasets.setter
+    def qlik_datasets(self, qlik_datasets: Optional[list[QlikDataset]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_datasets = qlik_datasets
+
+    @property
+    def qlik_apps(self) -> Optional[list[QlikApp]]:
+        return self.attributes.qlik_apps
+
+    @qlik_apps.setter
+    def qlik_apps(self, qlik_apps: Optional[list[QlikApp]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_apps = qlik_apps
+
+    type_name: str = Field("QlikSpace", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QlikSpace":
+            raise ValueError("must be QlikSpace")
+        return v
+
+    class Attributes(Qlik.Attributes):
+        qlik_space_type: Optional[str] = Field(
+            None, description="", alias="qlikSpaceType"
+        )
+        qlik_datasets: Optional[list[QlikDataset]] = Field(
+            None, description="", alias="qlikDatasets"
+        )  # relationship
+        qlik_apps: Optional[list[QlikApp]] = Field(
+            None, description="", alias="qlikApps"
+        )  # relationship
+
+    attributes: "QlikSpace.Attributes" = Field(
+        default_factory=lambda: QlikSpace.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class QlikApp(Qlik):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in QlikApp._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "qlik_has_section_access",
+        "qlik_origin_app_id",
+        "qlik_is_encrypted",
+        "qlik_is_direct_query_mode",
+        "qlik_app_static_byte_size",
+        "qlik_space",
+        "qlik_sheets",
+    ]
+
+    @property
+    def qlik_has_section_access(self) -> Optional[bool]:
+        return self.attributes.qlik_has_section_access
+
+    @qlik_has_section_access.setter
+    def qlik_has_section_access(self, qlik_has_section_access: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_has_section_access = qlik_has_section_access
+
+    @property
+    def qlik_origin_app_id(self) -> Optional[str]:
+        return self.attributes.qlik_origin_app_id
+
+    @qlik_origin_app_id.setter
+    def qlik_origin_app_id(self, qlik_origin_app_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_origin_app_id = qlik_origin_app_id
+
+    @property
+    def qlik_is_encrypted(self) -> Optional[bool]:
+        return self.attributes.qlik_is_encrypted
+
+    @qlik_is_encrypted.setter
+    def qlik_is_encrypted(self, qlik_is_encrypted: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_is_encrypted = qlik_is_encrypted
+
+    @property
+    def qlik_is_direct_query_mode(self) -> Optional[bool]:
+        return self.attributes.qlik_is_direct_query_mode
+
+    @qlik_is_direct_query_mode.setter
+    def qlik_is_direct_query_mode(self, qlik_is_direct_query_mode: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_is_direct_query_mode = qlik_is_direct_query_mode
+
+    @property
+    def qlik_app_static_byte_size(self) -> Optional[int]:
+        return self.attributes.qlik_app_static_byte_size
+
+    @qlik_app_static_byte_size.setter
+    def qlik_app_static_byte_size(self, qlik_app_static_byte_size: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_app_static_byte_size = qlik_app_static_byte_size
+
+    @property
+    def qlik_space(self) -> Optional[QlikSpace]:
+        return self.attributes.qlik_space
+
+    @qlik_space.setter
+    def qlik_space(self, qlik_space: Optional[QlikSpace]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_space = qlik_space
+
+    @property
+    def qlik_sheets(self) -> Optional[list[QlikSheet]]:
+        return self.attributes.qlik_sheets
+
+    @qlik_sheets.setter
+    def qlik_sheets(self, qlik_sheets: Optional[list[QlikSheet]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_sheets = qlik_sheets
+
+    type_name: str = Field("QlikApp", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QlikApp":
+            raise ValueError("must be QlikApp")
+        return v
+
+    class Attributes(Qlik.Attributes):
+        qlik_has_section_access: Optional[bool] = Field(
+            None, description="", alias="qlikHasSectionAccess"
+        )
+        qlik_origin_app_id: Optional[str] = Field(
+            None, description="", alias="qlikOriginAppId"
+        )
+        qlik_is_encrypted: Optional[bool] = Field(
+            None, description="", alias="qlikIsEncrypted"
+        )
+        qlik_is_direct_query_mode: Optional[bool] = Field(
+            None, description="", alias="qlikIsDirectQueryMode"
+        )
+        qlik_app_static_byte_size: Optional[int] = Field(
+            None, description="", alias="qlikAppStaticByteSize"
+        )
+        qlik_space: Optional[QlikSpace] = Field(
+            None, description="", alias="qlikSpace"
+        )  # relationship
+        qlik_sheets: Optional[list[QlikSheet]] = Field(
+            None, description="", alias="qlikSheets"
+        )  # relationship
+
+    attributes: "QlikApp.Attributes" = Field(
+        default_factory=lambda: QlikApp.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class QlikChart(Qlik):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in QlikChart._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "qlik_chart_subtitle",
+        "qlik_chart_footnote",
+        "qlik_chart_orientation",
+        "qlik_chart_type",
+        "qlik_sheet",
+    ]
+
+    @property
+    def qlik_chart_subtitle(self) -> Optional[str]:
+        return self.attributes.qlik_chart_subtitle
+
+    @qlik_chart_subtitle.setter
+    def qlik_chart_subtitle(self, qlik_chart_subtitle: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_chart_subtitle = qlik_chart_subtitle
+
+    @property
+    def qlik_chart_footnote(self) -> Optional[str]:
+        return self.attributes.qlik_chart_footnote
+
+    @qlik_chart_footnote.setter
+    def qlik_chart_footnote(self, qlik_chart_footnote: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_chart_footnote = qlik_chart_footnote
+
+    @property
+    def qlik_chart_orientation(self) -> Optional[str]:
+        return self.attributes.qlik_chart_orientation
+
+    @qlik_chart_orientation.setter
+    def qlik_chart_orientation(self, qlik_chart_orientation: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_chart_orientation = qlik_chart_orientation
+
+    @property
+    def qlik_chart_type(self) -> Optional[str]:
+        return self.attributes.qlik_chart_type
+
+    @qlik_chart_type.setter
+    def qlik_chart_type(self, qlik_chart_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_chart_type = qlik_chart_type
+
+    @property
+    def qlik_sheet(self) -> Optional[QlikSheet]:
+        return self.attributes.qlik_sheet
+
+    @qlik_sheet.setter
+    def qlik_sheet(self, qlik_sheet: Optional[QlikSheet]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_sheet = qlik_sheet
+
+    type_name: str = Field("QlikChart", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QlikChart":
+            raise ValueError("must be QlikChart")
+        return v
+
+    class Attributes(Qlik.Attributes):
+        qlik_chart_subtitle: Optional[str] = Field(
+            None, description="", alias="qlikChartSubtitle"
+        )
+        qlik_chart_footnote: Optional[str] = Field(
+            None, description="", alias="qlikChartFootnote"
+        )
+        qlik_chart_orientation: Optional[str] = Field(
+            None, description="", alias="qlikChartOrientation"
+        )
+        qlik_chart_type: Optional[str] = Field(
+            None, description="", alias="qlikChartType"
+        )
+        qlik_sheet: Optional[QlikSheet] = Field(
+            None, description="", alias="qlikSheet"
+        )  # relationship
+
+    attributes: "QlikChart.Attributes" = Field(
+        default_factory=lambda: QlikChart.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class QlikDataset(Qlik):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in QlikDataset._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "qlik_dataset_technical_name",
+        "qlik_dataset_type",
+        "qlik_dataset_uri",
+        "qlik_dataset_subtype",
+        "qlik_space",
+    ]
+
+    @property
+    def qlik_dataset_technical_name(self) -> Optional[str]:
+        return self.attributes.qlik_dataset_technical_name
+
+    @qlik_dataset_technical_name.setter
+    def qlik_dataset_technical_name(self, qlik_dataset_technical_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_dataset_technical_name = qlik_dataset_technical_name
+
+    @property
+    def qlik_dataset_type(self) -> Optional[str]:
+        return self.attributes.qlik_dataset_type
+
+    @qlik_dataset_type.setter
+    def qlik_dataset_type(self, qlik_dataset_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_dataset_type = qlik_dataset_type
+
+    @property
+    def qlik_dataset_uri(self) -> Optional[str]:
+        return self.attributes.qlik_dataset_uri
+
+    @qlik_dataset_uri.setter
+    def qlik_dataset_uri(self, qlik_dataset_uri: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_dataset_uri = qlik_dataset_uri
+
+    @property
+    def qlik_dataset_subtype(self) -> Optional[str]:
+        return self.attributes.qlik_dataset_subtype
+
+    @qlik_dataset_subtype.setter
+    def qlik_dataset_subtype(self, qlik_dataset_subtype: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_dataset_subtype = qlik_dataset_subtype
+
+    @property
+    def qlik_space(self) -> Optional[QlikSpace]:
+        return self.attributes.qlik_space
+
+    @qlik_space.setter
+    def qlik_space(self, qlik_space: Optional[QlikSpace]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_space = qlik_space
+
+    type_name: str = Field("QlikDataset", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QlikDataset":
+            raise ValueError("must be QlikDataset")
+        return v
+
+    class Attributes(Qlik.Attributes):
+        qlik_dataset_technical_name: Optional[str] = Field(
+            None, description="", alias="qlikDatasetTechnicalName"
+        )
+        qlik_dataset_type: Optional[str] = Field(
+            None, description="", alias="qlikDatasetType"
+        )
+        qlik_dataset_uri: Optional[str] = Field(
+            None, description="", alias="qlikDatasetUri"
+        )
+        qlik_dataset_subtype: Optional[str] = Field(
+            None, description="", alias="qlikDatasetSubtype"
+        )
+        qlik_space: Optional[QlikSpace] = Field(
+            None, description="", alias="qlikSpace"
+        )  # relationship
+
+    attributes: "QlikDataset.Attributes" = Field(
+        default_factory=lambda: QlikDataset.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class QlikSheet(Qlik):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in QlikSheet._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "qlik_sheet_is_approved",
+        "qlik_app",
+        "qlik_charts",
+    ]
+
+    @property
+    def qlik_sheet_is_approved(self) -> Optional[bool]:
+        return self.attributes.qlik_sheet_is_approved
+
+    @qlik_sheet_is_approved.setter
+    def qlik_sheet_is_approved(self, qlik_sheet_is_approved: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_sheet_is_approved = qlik_sheet_is_approved
+
+    @property
+    def qlik_app(self) -> Optional[QlikApp]:
+        return self.attributes.qlik_app
+
+    @qlik_app.setter
+    def qlik_app(self, qlik_app: Optional[QlikApp]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_app = qlik_app
+
+    @property
+    def qlik_charts(self) -> Optional[list[QlikChart]]:
+        return self.attributes.qlik_charts
+
+    @qlik_charts.setter
+    def qlik_charts(self, qlik_charts: Optional[list[QlikChart]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.qlik_charts = qlik_charts
+
+    type_name: str = Field("QlikSheet", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "QlikSheet":
+            raise ValueError("must be QlikSheet")
+        return v
+
+    class Attributes(Qlik.Attributes):
+        qlik_sheet_is_approved: Optional[bool] = Field(
+            None, description="", alias="qlikSheetIsApproved"
+        )
+        qlik_app: Optional[QlikApp] = Field(
+            None, description="", alias="qlikApp"
+        )  # relationship
+        qlik_charts: Optional[list[QlikChart]] = Field(
+            None, description="", alias="qlikCharts"
+        )  # relationship
+
+    attributes: "QlikSheet.Attributes" = Field(
+        default_factory=lambda: QlikSheet.Attributes(),
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class SalesforceObject(Salesforce):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in SalesforceObject._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -23420,38 +24614,40 @@
 
 GCS.Attributes.update_forward_refs()
 
 MonteCarlo.Attributes.update_forward_refs()
 
 Metric.Attributes.update_forward_refs()
 
+Preset.Attributes.update_forward_refs()
+
+Mode.Attributes.update_forward_refs()
+
+Sigma.Attributes.update_forward_refs()
+
+Tableau.Attributes.update_forward_refs()
+
+Looker.Attributes.update_forward_refs()
+
+Redash.Attributes.update_forward_refs()
+
 DataStudio.Attributes.update_forward_refs()
 
 Metabase.Attributes.update_forward_refs()
 
 QuickSight.Attributes.update_forward_refs()
 
 Thoughtspot.Attributes.update_forward_refs()
 
 PowerBI.Attributes.update_forward_refs()
 
-Preset.Attributes.update_forward_refs()
-
-Sigma.Attributes.update_forward_refs()
-
-Mode.Attributes.update_forward_refs()
+MicroStrategy.Attributes.update_forward_refs()
 
 Qlik.Attributes.update_forward_refs()
 
-Tableau.Attributes.update_forward_refs()
-
-Looker.Attributes.update_forward_refs()
-
-Redash.Attributes.update_forward_refs()
-
 Salesforce.Attributes.update_forward_refs()
 
 DbtModelColumn.Attributes.update_forward_refs()
 
 DbtModel.Attributes.update_forward_refs()
 
 DbtMetric.Attributes.update_forward_refs()
@@ -23480,20 +24676,20 @@
 
 Query.Attributes.update_forward_refs()
 
 Column.Attributes.update_forward_refs()
 
 Schema.Attributes.update_forward_refs()
 
-Database.Attributes.update_forward_refs()
-
 SnowflakeStream.Attributes.update_forward_refs()
 
 SnowflakePipe.Attributes.update_forward_refs()
 
+Database.Attributes.update_forward_refs()
+
 Procedure.Attributes.update_forward_refs()
 
 View.Attributes.update_forward_refs()
 
 MaterialisedView.Attributes.update_forward_refs()
 
 DataStudioAsset.Attributes.update_forward_refs()
@@ -23516,116 +24712,58 @@
 
 GCSBucket.Attributes.update_forward_refs()
 
 MCIncident.Attributes.update_forward_refs()
 
 MCMonitor.Attributes.update_forward_refs()
 
-MetabaseQuestion.Attributes.update_forward_refs()
-
-MetabaseCollection.Attributes.update_forward_refs()
-
-MetabaseDashboard.Attributes.update_forward_refs()
-
-QuickSightFolder.Attributes.update_forward_refs()
-
-QuickSightDashboardVisual.Attributes.update_forward_refs()
-
-QuickSightAnalysis.Attributes.update_forward_refs()
-
-QuickSightAnalysisVisual.Attributes.update_forward_refs()
-
-QuickSightDatasetField.Attributes.update_forward_refs()
-
-QuickSightDashboard.Attributes.update_forward_refs()
-
-QuickSightDataset.Attributes.update_forward_refs()
-
-ThoughtspotLiveboard.Attributes.update_forward_refs()
-
-ThoughtspotDashlet.Attributes.update_forward_refs()
-
-ThoughtspotAnswer.Attributes.update_forward_refs()
-
-PowerBIReport.Attributes.update_forward_refs()
-
-PowerBIMeasure.Attributes.update_forward_refs()
-
-PowerBIColumn.Attributes.update_forward_refs()
-
-PowerBITile.Attributes.update_forward_refs()
-
-PowerBITable.Attributes.update_forward_refs()
-
-PowerBIDatasource.Attributes.update_forward_refs()
-
-PowerBIWorkspace.Attributes.update_forward_refs()
-
-PowerBIDataset.Attributes.update_forward_refs()
-
-PowerBIDashboard.Attributes.update_forward_refs()
-
-PowerBIPage.Attributes.update_forward_refs()
-
-PowerBIDataflow.Attributes.update_forward_refs()
-
 PresetChart.Attributes.update_forward_refs()
 
 PresetDataset.Attributes.update_forward_refs()
 
 PresetDashboard.Attributes.update_forward_refs()
 
 PresetWorkspace.Attributes.update_forward_refs()
 
-SigmaDatasetColumn.Attributes.update_forward_refs()
-
-SigmaDataset.Attributes.update_forward_refs()
-
-SigmaWorkbook.Attributes.update_forward_refs()
-
-SigmaDataElementField.Attributes.update_forward_refs()
-
-SigmaPage.Attributes.update_forward_refs()
-
-SigmaDataElement.Attributes.update_forward_refs()
-
 ModeReport.Attributes.update_forward_refs()
 
 ModeQuery.Attributes.update_forward_refs()
 
 ModeChart.Attributes.update_forward_refs()
 
 ModeWorkspace.Attributes.update_forward_refs()
 
 ModeCollection.Attributes.update_forward_refs()
 
-QlikSpace.Attributes.update_forward_refs()
+SigmaDatasetColumn.Attributes.update_forward_refs()
 
-QlikApp.Attributes.update_forward_refs()
+SigmaDataset.Attributes.update_forward_refs()
 
-QlikChart.Attributes.update_forward_refs()
+SigmaWorkbook.Attributes.update_forward_refs()
 
-QlikDataset.Attributes.update_forward_refs()
+SigmaDataElementField.Attributes.update_forward_refs()
 
-QlikSheet.Attributes.update_forward_refs()
+SigmaPage.Attributes.update_forward_refs()
+
+SigmaDataElement.Attributes.update_forward_refs()
 
 TableauWorkbook.Attributes.update_forward_refs()
 
 TableauDatasourceField.Attributes.update_forward_refs()
 
 TableauCalculatedField.Attributes.update_forward_refs()
 
 TableauProject.Attributes.update_forward_refs()
 
 TableauMetric.Attributes.update_forward_refs()
 
-TableauDatasource.Attributes.update_forward_refs()
-
 TableauSite.Attributes.update_forward_refs()
 
+TableauDatasource.Attributes.update_forward_refs()
+
 TableauDashboard.Attributes.update_forward_refs()
 
 TableauFlow.Attributes.update_forward_refs()
 
 TableauWorksheet.Attributes.update_forward_refs()
 
 LookerLook.Attributes.update_forward_refs()
@@ -23650,14 +24788,90 @@
 
 RedashDashboard.Attributes.update_forward_refs()
 
 RedashQuery.Attributes.update_forward_refs()
 
 RedashVisualization.Attributes.update_forward_refs()
 
+MetabaseQuestion.Attributes.update_forward_refs()
+
+MetabaseCollection.Attributes.update_forward_refs()
+
+MetabaseDashboard.Attributes.update_forward_refs()
+
+QuickSightFolder.Attributes.update_forward_refs()
+
+QuickSightDashboardVisual.Attributes.update_forward_refs()
+
+QuickSightAnalysisVisual.Attributes.update_forward_refs()
+
+QuickSightDatasetField.Attributes.update_forward_refs()
+
+QuickSightAnalysis.Attributes.update_forward_refs()
+
+QuickSightDashboard.Attributes.update_forward_refs()
+
+QuickSightDataset.Attributes.update_forward_refs()
+
+ThoughtspotLiveboard.Attributes.update_forward_refs()
+
+ThoughtspotDashlet.Attributes.update_forward_refs()
+
+ThoughtspotAnswer.Attributes.update_forward_refs()
+
+PowerBIReport.Attributes.update_forward_refs()
+
+PowerBIMeasure.Attributes.update_forward_refs()
+
+PowerBIColumn.Attributes.update_forward_refs()
+
+PowerBITable.Attributes.update_forward_refs()
+
+PowerBITile.Attributes.update_forward_refs()
+
+PowerBIDatasource.Attributes.update_forward_refs()
+
+PowerBIWorkspace.Attributes.update_forward_refs()
+
+PowerBIDataset.Attributes.update_forward_refs()
+
+PowerBIDashboard.Attributes.update_forward_refs()
+
+PowerBIDataflow.Attributes.update_forward_refs()
+
+PowerBIPage.Attributes.update_forward_refs()
+
+MicroStrategyReport.Attributes.update_forward_refs()
+
+MicroStrategyProject.Attributes.update_forward_refs()
+
+MicroStrategyMetric.Attributes.update_forward_refs()
+
+MicroStrategyCube.Attributes.update_forward_refs()
+
+MicroStrategyDossier.Attributes.update_forward_refs()
+
+MicroStrategyFact.Attributes.update_forward_refs()
+
+MicroStrategyDocument.Attributes.update_forward_refs()
+
+MicroStrategyAttribute.Attributes.update_forward_refs()
+
+MicroStrategyVisualization.Attributes.update_forward_refs()
+
+QlikSpace.Attributes.update_forward_refs()
+
+QlikApp.Attributes.update_forward_refs()
+
+QlikChart.Attributes.update_forward_refs()
+
+QlikDataset.Attributes.update_forward_refs()
+
+QlikSheet.Attributes.update_forward_refs()
+
 SalesforceObject.Attributes.update_forward_refs()
 
 SalesforceField.Attributes.update_forward_refs()
 
 SalesforceOrganization.Attributes.update_forward_refs()
 
 SalesforceDashboard.Attributes.update_forward_refs()
```

### Comparing `pyatlan-0.1.0/pyatlan/model/core.py` & `pyatlan-0.1.1/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/model/custom_metadata.py` & `pyatlan-0.1.1/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/model/group.py` & `pyatlan-0.1.1/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/model/lineage.py` & `pyatlan-0.1.1/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/model/query.py` & `pyatlan-0.1.1/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/model/response.py` & `pyatlan-0.1.1/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/model/role.py` & `pyatlan-0.1.1/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/model/search.py` & `pyatlan-0.1.1/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/model/structs.py` & `pyatlan-0.1.1/pyatlan/model/structs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -37,43 +37,54 @@
         None, description="", alias="awsCloudWatchMetricName"
     )
     aws_cloud_watch_metric_scope: "str" = Field(
         None, description="", alias="awsCloudWatchMetricScope"
     )
 
 
-class Histogram(AtlanObject):
-    """Description"""
-
-    boundaries: "set[float]" = Field(None, description="", alias="boundaries")
-    frequencies: "set[float]" = Field(None, description="", alias="frequencies")
-
-
 class KafkaTopicConsumption(AtlanObject):
     """Description"""
 
     topic_name: Optional["str"] = Field(None, description="", alias="topicName")
     topic_partition: Optional["str"] = Field(
         None, description="", alias="topicPartition"
     )
     topic_lag: Optional["int"] = Field(None, description="", alias="topicLag")
     topic_current_offset: Optional["int"] = Field(
         None, description="", alias="topicCurrentOffset"
     )
 
 
+class Histogram(AtlanObject):
+    """Description"""
+
+    boundaries: "set[float]" = Field(None, description="", alias="boundaries")
+    frequencies: "set[float]" = Field(None, description="", alias="frequencies")
+
+
 class ColumnValueFrequencyMap(AtlanObject):
     """Description"""
 
     column_value: Optional["str"] = Field(None, description="", alias="columnValue")
     column_value_frequency: Optional["int"] = Field(
         None, description="", alias="columnValueFrequency"
     )
 
 
+class SourceTagAttachmentValue(AtlanObject):
+    """Description"""
+
+    tag_attachment_key: Optional["str"] = Field(
+        None, description="", alias="tagAttachmentKey"
+    )
+    tag_attachment_value: Optional["str"] = Field(
+        None, description="", alias="tagAttachmentValue"
+    )
+
+
 class BadgeCondition(AtlanObject):
     """Description"""
 
     @classmethod
     # @validate_arguments()
     def create(
         cls,
@@ -134,25 +145,14 @@
         None, description="", alias="sourceTagSyncTimestamp"
     )
     source_tag_sync_error: Optional["str"] = Field(
         None, description="", alias="sourceTagSyncError"
     )
 
 
-class SourceTagAttachmentValue(AtlanObject):
-    """Description"""
-
-    tag_attachment_key: Optional["str"] = Field(
-        None, description="", alias="tagAttachmentKey"
-    )
-    tag_attachment_value: Optional["str"] = Field(
-        None, description="", alias="tagAttachmentValue"
-    )
-
-
 class AzureTag(AtlanObject):
     """Description"""
 
     azure_tag_key: "str" = Field(None, description="", alias="azureTagKey")
     azure_tag_value: "str" = Field(None, description="", alias="azureTagValue")
```

### Comparing `pyatlan-0.1.0/pyatlan/model/typedef.py` & `pyatlan-0.1.1/pyatlan/model/typedef.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 import time
 from typing import Any, Dict, List, Optional
 
 from pydantic import Field
 
+from pyatlan.model.atlan_image import AtlanImage
 from pyatlan.model.core import AtlanObject
 from pyatlan.model.enums import (
     AtlanClassificationColor,
     AtlanCustomAttributePrimitiveType,
+    AtlanIcon,
     AtlanTypeCategory,
     Cardinality,
+    IconType,
     IndexType,
 )
 
 _complete_type_list = (
     '["ADLSAccount",'
     '"ADLSAccount",'
     '"ADLSContainer",'
@@ -487,27 +490,43 @@
     )
     service_type: Optional[str] = Field(
         description="Name used for display purposes (in user interfaces)."
     )
     skip_display_name_uniqueness_check: Optional[bool] = Field(description="TBC")
 
     @staticmethod
-    def create(name: str, color: AtlanClassificationColor) -> ClassificationDef:
+    def create(
+        name: str,
+        color: AtlanClassificationColor,
+        icon: AtlanIcon = AtlanIcon.ATLAN_TAG,
+        image: Optional[AtlanImage] = None,
+    ) -> ClassificationDef:
         from pyatlan.model.assets import validate_required_fields
 
         validate_required_fields(
             ["name", "color"],
             [name, color],
         )
+        cls_options = {
+            "color": color.value,
+            "iconName": icon.value,
+        }
+        if image:
+            cls_options["imageID"] = str(image.id)
+            cls_options["iconType"] = IconType.IMAGE.value
+        else:
+            cls_options["imageID"] = ""
+            cls_options["iconType"] = IconType.ICON.value
+
         # Explicitly set all defaults to ensure inclusion during pydantic serialization
         return ClassificationDef(
             category=AtlanTypeCategory.CLASSIFICATION,
             name=name,
             display_name=name,
-            options={"color": color.value},
+            options=cls_options,
             skip_display_name_uniqueness_check=False,
         )
 
 
 class EntityDef(TypeDef):
     attribute_defs: Optional[List[Dict[str, Any]]] = Field(
         [], description="Unused.", example=[]
```

### Comparing `pyatlan-0.1.0/pyatlan/model/user.py` & `pyatlan-0.1.1/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan/utils.py` & `pyatlan-0.1.1/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.1.1/pyatlan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.1.0
+Version: 0.1.1
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.1.0/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.1.1/pyatlan.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 NOTICE
 README.md
 setup.py
 pyatlan/__init__.py
 pyatlan/error.py
 pyatlan/exceptions.py
+pyatlan/multipart_data_generator.py
 pyatlan/utils.py
 pyatlan/version.txt
 pyatlan.egg-info/PKG-INFO
 pyatlan.egg-info/SOURCES.txt
 pyatlan.egg-info/dependency_links.txt
 pyatlan.egg-info/not-zip-safe
 pyatlan.egg-info/requires.txt
@@ -25,42 +26,43 @@
 pyatlan/client/atlan.py
 pyatlan/client/constants.py
 pyatlan/generator/__init__.py
 pyatlan/generator/generate_from_typdefs.py
 pyatlan/generator/templates/__init__.py
 pyatlan/model/__init__.py
 pyatlan/model/assets.py
+pyatlan/model/atlan_image.py
 pyatlan/model/core.py
 pyatlan/model/custom_metadata.py
 pyatlan/model/enums.py
 pyatlan/model/group.py
 pyatlan/model/internal.py
 pyatlan/model/lineage.py
 pyatlan/model/query.py
 pyatlan/model/response.py
 pyatlan/model/role.py
 pyatlan/model/search.py
 pyatlan/model/structs.py
 pyatlan/model/typedef.py
 pyatlan/model/user.py
 tests/__init__.py
-tests/conftest.py
 tests/integration/__init__.py
 tests/integration/admin_test.py
 tests/integration/classification_test.py
 tests/integration/client.py
+tests/integration/conftest.py
 tests/integration/connection_test.py
 tests/integration/custom_metadata_test.py
 tests/integration/glossary_test.py
 tests/integration/lineage_test.py
 tests/integration/query_parser_test.py
 tests/integration/s3_asset_test.py
 tests/integration/test_client.py
-tests/integration/test_entity_model.py
 tests/integration/test_index_search.py
+tests/integration/test_sql_assets.py
 tests/unit/__init__.py
 tests/unit/test_classification_name.py
 tests/unit/test_client.py
 tests/unit/test_custom_metadata.py
 tests/unit/test_glossary_term.py
 tests/unit/test_lineage.py
 tests/unit/test_model.py
```

### Comparing `pyatlan-0.1.0/setup.py` & `pyatlan-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/tests/integration/client.py` & `pyatlan-0.1.1/tests/integration/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 import logging
-from typing import Callable, Type
+from typing import Generator, Type
 
 import pytest
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.response import A
 
 LOGGER = logging.getLogger(__name__)
 
 
-@pytest.fixture(scope="session")
-def make_unique() -> Callable[[str], str]:
+class TestId:
     from nanoid import generate as generate_nanoid
 
     session_id = generate_nanoid(
         alphabet="1234567890abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ",
         size=5,
     )
 
-    def _get_unique_name(input: str) -> str:
-        return f"psdk_{input}_{session_id}"
-
-    return _get_unique_name
+    @classmethod
+    def make_unique(cls, input: str):
+        return f"psdk_{input}_{cls.session_id}"
 
 
 @pytest.fixture(scope="module")
-def client() -> AtlanClient:
-    return AtlanClient()
+def client() -> Generator[AtlanClient, None, None]:
+    client = AtlanClient()
+    client.register_client(client)
+
+    yield client
+
+    AtlanClient.reset_default_client()
 
 
 def delete_asset(client: AtlanClient, asset_type: Type[A], guid: str) -> None:
     # These assertions check the cleanup actually worked
     r = client.purge_entity_by_guid(guid)
     s = r is not None
     s = s and len(r.assets_deleted(asset_type)) == 1
```

### Comparing `pyatlan-0.1.0/tests/integration/connection_test.py` & `pyatlan-0.1.1/tests/integration/connection_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,69 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
-from typing import Callable
-
 import pytest
 
 from pyatlan.cache.role_cache import RoleCache
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.assets import Connection
 from pyatlan.model.enums import AtlanConnectorType
+from tests.integration.client import TestId
 
-MODULE_NAME = "CONN"
+MODULE_NAME = TestId.make_unique("CONN")
 
 
 def create_connection(
     client: AtlanClient, name: str, connector_type: AtlanConnectorType
 ) -> Connection:
     admin_role_guid = str(RoleCache.get_id_for_name("$admin"))
     to_create = Connection.create(
         name=name, connector_type=connector_type, admin_roles=[admin_role_guid]
     )
     response = client.upsert(to_create)
     result = response.assets_created(asset_type=Connection)[0]
-    resolved = client.get_asset_by_guid(result.guid, asset_type=Connection)
-    return resolved
+    return client.get_asset_by_guid(result.guid, asset_type=Connection)
 
 
-def test_invalid_connection(client: AtlanClient, make_unique: Callable[[str], str]):
+def test_invalid_connection(client: AtlanClient):
     with pytest.raises(
         ValueError, match="One of admin_user, admin_groups or admin_roles is required"
     ):
-        Connection.create(
-            name=make_unique(MODULE_NAME), connector_type=AtlanConnectorType.POSTGRES
-        )
+        Connection.create(name=MODULE_NAME, connector_type=AtlanConnectorType.POSTGRES)
 
 
 def test_invalid_connection_admin_role(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
 ):
     with pytest.raises(
         ValueError, match="Provided role ID abc123 was not found in Atlan."
     ):
         Connection.create(
-            name=make_unique(MODULE_NAME),
+            name=MODULE_NAME,
             connector_type=AtlanConnectorType.SAPHANA,
             admin_roles=["abc123"],
         )
 
 
 def test_invalid_connection_admin_group(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
 ):
     with pytest.raises(
         ValueError, match="Provided group name abc123 was not found in Atlan."
     ):
         Connection.create(
-            name=make_unique(MODULE_NAME),
+            name=MODULE_NAME,
             connector_type=AtlanConnectorType.SAPHANA,
             admin_groups=["abc123"],
         )
 
 
 def test_invalid_connection_admin_user(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
 ):
     with pytest.raises(
         ValueError, match="Provided username abc123 was not found in Atlan."
     ):
         Connection.create(
-            name=make_unique(MODULE_NAME),
+            name=MODULE_NAME,
             connector_type=AtlanConnectorType.SAPHANA,
             admin_users=["abc123"],
         )
```

### Comparing `pyatlan-0.1.0/tests/integration/custom_metadata_test.py` & `pyatlan-0.1.1/tests/integration/custom_metadata_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
-import logging
 import time
-from typing import Callable, Generator, List, Optional, Tuple
+from typing import Generator, List, Optional, Tuple
 
 import pytest
 
 from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.assets import AtlasGlossary, AtlasGlossaryTerm, Badge, BadgeCondition
 from pyatlan.model.custom_metadata import CustomMetadataDict
@@ -16,38 +15,45 @@
     BadgeComparisonOperator,
     BadgeConditionColor,
 )
 from pyatlan.model.group import AtlanGroup, CreateGroupResponse
 from pyatlan.model.search import DSL, Bool, Exists, IndexSearchRequest, Term
 from pyatlan.model.typedef import AttributeDef, CustomMetadataDef, EnumDef
 from tests.integration.admin_test import create_group, delete_group
-from tests.integration.client import delete_asset
+from tests.integration.client import TestId, delete_asset
 from tests.integration.glossary_test import create_glossary, create_term
 
-LOGGER = logging.getLogger(__name__)
+MODULE_NAME = TestId.make_unique("CM")
 
-MODULE_NAME = "CM"
 FIXED_USER = "ernest"
+GROUP_NAME1 = f"{MODULE_NAME}1"
+GROUP_NAME2 = f"{MODULE_NAME}2"
 
+CM_RACI = f"{MODULE_NAME}_RACI"
 CM_ATTR_RACI_RESPONSIBLE = "Responsible"
 CM_ATTR_RACI_ACCOUNTABLE = "Accountable"
 CM_ATTR_RACI_CONSULTED = "Consulted"
 CM_ATTR_RACI_INFORMED = "Informed"
 CM_ATTR_RACI_EXTRA = "Extra"
 
 
+CM_IPR = f"{MODULE_NAME}_IPR"
 CM_ATTR_IPR_LICENSE = "License"
 CM_ATTR_IPR_VERSION = "Version"
 CM_ATTR_IPR_MANDATORY = "Mandatory"
 CM_ATTR_IPR_DATE = "Date"
 CM_ATTR_IPR_URL = "URL"
 
+
+CM_QUALITY = f"{MODULE_NAME}_DQ"
 CM_ATTR_QUALITY_COUNT = "Count"
 CM_ATTR_QUALITY_SQL = "SQL"
 CM_ATTR_QUALITY_TYPE = "Type"
+
+DQ_ENUM = f"{MODULE_NAME}_DataQualityType"
 DQ_TYPE_LIST = [
     "Accuracy",
     "Completeness",
     "Consistency",
     "Timeliness",
     "Validity",
     "Uniqueness",
@@ -78,15 +84,14 @@
     r = client.create_typedef(enum_def)
     return r.enum_defs[0]
 
 
 @pytest.fixture(scope="module")
 def cm_ipr(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
 ) -> Generator[CustomMetadataDef, None, None]:
     attribute_defs = [
         AttributeDef.create(
             display_name=CM_ATTR_IPR_LICENSE,
             attribute_type=AtlanCustomAttributePrimitiveType.STRING,
         ),
         AttributeDef.create(
@@ -102,27 +107,25 @@
             attribute_type=AtlanCustomAttributePrimitiveType.DATE,
         ),
         AttributeDef.create(
             display_name=CM_ATTR_IPR_URL,
             attribute_type=AtlanCustomAttributePrimitiveType.URL,
         ),
     ]
-    cm_name = make_unique("IPR")
     cm = create_custom_metadata(
-        client, name=cm_name, attribute_defs=attribute_defs, logo="⚖️", locked=True
+        client, name=CM_IPR, attribute_defs=attribute_defs, logo="⚖️", locked=True
     )
     yield cm
-    client.purge_typedef(cm_name, CustomMetadataDef)
+    client.purge_typedef(CM_IPR, CustomMetadataDef)
 
 
 def test_cm_ipr(
     cm_ipr: CustomMetadataDef,
-    make_unique: Callable[[str], str],
 ):
-    cm_name = make_unique("IPR")
+    cm_name = CM_IPR
     assert cm_ipr.category == AtlanTypeCategory.CUSTOM_METADATA
     assert cm_ipr.guid
     assert cm_ipr.name != cm_name
     assert cm_ipr.display_name == cm_name
     attributes = cm_ipr.attribute_defs
     assert attributes
     assert len(attributes) == 5
@@ -159,15 +162,14 @@
     assert one.options
     assert not one.options.multi_value_select
 
 
 @pytest.fixture(scope="module")
 def cm_raci(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
 ) -> Generator[CustomMetadataDef, None, None]:
     attribute_defs = [
         AttributeDef.create(
             display_name=CM_ATTR_RACI_RESPONSIBLE,
             attribute_type=AtlanCustomAttributePrimitiveType.USERS,
             multi_valued=True,
         ),
@@ -186,30 +188,28 @@
             multi_valued=True,
         ),
         AttributeDef.create(
             display_name=CM_ATTR_RACI_EXTRA,
             attribute_type=AtlanCustomAttributePrimitiveType.STRING,
         ),
     ]
-    cm_name = make_unique("RACI")
     cm = create_custom_metadata(
-        client, name=cm_name, attribute_defs=attribute_defs, logo="👪", locked=False
+        client, name=CM_RACI, attribute_defs=attribute_defs, logo="👪", locked=False
     )
     yield cm
-    client.purge_typedef(cm_name, CustomMetadataDef)
+    client.purge_typedef(CM_RACI, CustomMetadataDef)
 
 
 def test_cm_raci(
     cm_raci: CustomMetadataDef,
-    make_unique: Callable[[str], str],
 ):
     assert cm_raci.category == AtlanTypeCategory.CUSTOM_METADATA
     assert cm_raci.name
     assert cm_raci.guid
-    cm_name = make_unique("RACI")
+    cm_name = CM_RACI
     assert cm_raci.name != cm_name
     assert cm_raci.display_name == cm_name
     attributes = cm_raci.attribute_defs
     assert attributes
     assert len(attributes) == 5
     one = attributes[0]
     assert one
@@ -244,72 +244,66 @@
     assert one.options
     assert not one.options.multi_value_select
 
 
 @pytest.fixture(scope="module")
 def cm_enum(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
 ) -> Generator[EnumDef, None, None]:
-    dq_enum_name = make_unique(f"{MODULE_NAME}_DataQualityType")
-    enum_def = create_enum(client, name=dq_enum_name, values=DQ_TYPE_LIST)
+    enum_def = create_enum(client, name=DQ_ENUM, values=DQ_TYPE_LIST)
     yield enum_def
-    client.purge_typedef(dq_enum_name, EnumDef)
+    client.purge_typedef(DQ_ENUM, EnumDef)
 
 
 def test_cm_enum(
     cm_enum: EnumDef,
-    make_unique: Callable[[str], str],
 ):
     assert cm_enum.category == AtlanTypeCategory.ENUM
-    assert cm_enum.name == make_unique(f"{MODULE_NAME}_DataQualityType")
+    assert cm_enum.name == DQ_ENUM
     assert cm_enum.guid
     assert cm_enum.element_defs
     assert len(cm_enum.element_defs) == len(DQ_TYPE_LIST)
 
 
 @pytest.fixture(scope="module")
 def cm_dq(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     cm_enum: EnumDef,
 ) -> Generator[CustomMetadataDef, None, None]:
     attribute_defs = [
         AttributeDef.create(
             display_name=CM_ATTR_QUALITY_COUNT,
             attribute_type=AtlanCustomAttributePrimitiveType.INTEGER,
         ),
         AttributeDef.create(
             display_name=CM_ATTR_QUALITY_SQL,
             attribute_type=AtlanCustomAttributePrimitiveType.SQL,
         ),
         AttributeDef.create(
             display_name=CM_ATTR_QUALITY_TYPE,
             attribute_type=AtlanCustomAttributePrimitiveType.OPTIONS,
-            options_name=make_unique(f"{MODULE_NAME}_DataQualityType"),
+            options_name=DQ_ENUM,
         ),
     ]
-    cm_name = make_unique("DQ")
     cm = create_custom_metadata(
         client,
-        name=cm_name,
+        name=CM_QUALITY,
         attribute_defs=attribute_defs,
         logo="https://github.com/great-expectations/great_expectations/raw/develop/docs/docusaurus/static/img/"
         "gx-mark-160.png",
         locked=True,
     )
     yield cm
-    client.purge_typedef(cm_name, CustomMetadataDef)
+    client.purge_typedef(CM_QUALITY, CustomMetadataDef)
 
 
 def test_cm_dq(
     cm_dq: CustomMetadataDef,
-    make_unique: Callable[[str], str],
 ):
-    cm_name = make_unique("DQ")
+    cm_name = CM_QUALITY
     assert cm_dq.category == AtlanTypeCategory.CUSTOM_METADATA
     assert cm_dq.name
     assert cm_dq.guid
     assert cm_dq.name != cm_name
     assert cm_dq.display_name == cm_name
     attributes = cm_dq.attribute_defs
     assert attributes
@@ -328,106 +322,100 @@
     assert one.type_name == AtlanCustomAttributePrimitiveType.STRING.value
     assert one.options
     assert not one.options.multi_value_select
     assert one.options.custom_type == AtlanCustomAttributePrimitiveType.SQL.value
     one = attributes[2]
     assert one.display_name == CM_ATTR_QUALITY_TYPE
     assert one.name != CM_ATTR_QUALITY_TYPE
-    assert one.type_name == make_unique(f"{MODULE_NAME}_DataQualityType")
+    assert one.type_name == DQ_ENUM
     assert one.options
     assert not one.options.multi_value_select
     assert one.options.primitive_type == AtlanCustomAttributePrimitiveType.OPTIONS.value
 
 
 @pytest.fixture(scope="module")
 def glossary(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
 ) -> Generator[AtlasGlossary, None, None]:
-    glossary_name = make_unique(MODULE_NAME)
+    glossary_name = MODULE_NAME
     g = create_glossary(client, name=glossary_name)
     yield g
     delete_asset(client, guid=g.guid, asset_type=AtlasGlossary)
 
 
 @pytest.fixture(scope="module")
 def term(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     glossary: AtlasGlossary,
     cm_raci: CustomMetadataDef,
     cm_ipr: CustomMetadataDef,
     cm_dq: CustomMetadataDef,
 ) -> Generator[AtlasGlossaryTerm, None, None]:
-    term_name = make_unique(MODULE_NAME)
+    term_name = MODULE_NAME
     t = create_term(client, name=term_name, glossary_guid=glossary.guid)
     yield t
     delete_asset(client, guid=t.guid, asset_type=AtlasGlossaryTerm)
 
 
 @pytest.fixture(scope="module")
 def groups(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     glossary: AtlasGlossary,
     term: AtlasGlossaryTerm,
     cm_raci: CustomMetadataDef,
     cm_ipr: CustomMetadataDef,
     cm_dq: CustomMetadataDef,
 ) -> Generator[List[CreateGroupResponse], None, None]:
-    g1 = create_group(client, make_unique(f"{MODULE_NAME}1"))
-    g2 = create_group(client, make_unique(f"{MODULE_NAME}2"))
+    g1 = create_group(client, GROUP_NAME1)
+    g2 = create_group(client, GROUP_NAME2)
     yield [g1, g2]
     delete_group(client, g1.group)
     delete_group(client, g2.group)
 
 
 def _get_groups(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
 ) -> Tuple[AtlanGroup, AtlanGroup]:
-    candidates = client.get_group_by_name(make_unique(f"{MODULE_NAME}1"))
+    candidates = client.get_group_by_name(GROUP_NAME1)
     assert candidates
     assert len(candidates) == 1
     group1 = candidates[0]
-    candidates = client.get_group_by_name(make_unique(f"{MODULE_NAME}2"))
+    candidates = client.get_group_by_name(GROUP_NAME2)
     assert candidates
     assert len(candidates) == 1
     group2 = candidates[0]
     return group1, group2
 
 
 def test_add_term_cm_raci(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     cm_raci: CustomMetadataDef,
     term: AtlasGlossaryTerm,
     groups: List[AtlanGroup],
 ):
-    cm_name = make_unique("RACI")
+    cm_name = CM_RACI
     raci_attrs = CustomMetadataDict(cm_name)
     _validate_raci_empty(raci_attrs)
-    group1, group2 = _get_groups(client, make_unique)
+    group1, group2 = _get_groups(client)
     raci_attrs[CM_ATTR_RACI_RESPONSIBLE] = [FIXED_USER]
     raci_attrs[CM_ATTR_RACI_ACCOUNTABLE] = FIXED_USER
     raci_attrs[CM_ATTR_RACI_CONSULTED] = [group1.name]
     raci_attrs[CM_ATTR_RACI_INFORMED] = [group1.name, group2.name]
     client.update_custom_metadata_attributes(term.guid, raci_attrs)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
-    _validate_raci_attributes(client, make_unique, t.get_custom_metadata(name=cm_name))
+    _validate_raci_attributes(client, t.get_custom_metadata(name=cm_name))
 
 
 def test_add_term_cm_ipr(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     cm_ipr: CustomMetadataDef,
     term: AtlasGlossaryTerm,
 ):
-    cm_name = make_unique("IPR")
+    cm_name = CM_IPR
     ipr_attrs = CustomMetadataDict(cm_name)
     _validate_ipr_empty(ipr_attrs)
     ipr_attrs[CM_ATTR_IPR_LICENSE] = "CC BY"
     ipr_attrs[CM_ATTR_IPR_VERSION] = 2.0
     ipr_attrs[CM_ATTR_IPR_MANDATORY] = True
     ipr_attrs[CM_ATTR_IPR_DATE] = 1659308400000
     ipr_attrs[CM_ATTR_IPR_URL] = "https://creativecommons.org/licenses/by/2.0/"
@@ -436,110 +424,93 @@
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
     _validate_ipr_attributes(t.get_custom_metadata(name=cm_name))
 
 
 def test_add_term_cm_dq(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     cm_dq: CustomMetadataDef,
     term: AtlasGlossaryTerm,
 ):
-    cm_name = make_unique("DQ")
+    cm_name = CM_QUALITY
     dq_attrs = CustomMetadataDict(cm_name)
     _validate_dq_empty(dq_attrs)
     dq_attrs[CM_ATTR_QUALITY_COUNT] = 42
     dq_attrs[CM_ATTR_QUALITY_SQL] = "SELECT * from SOMEWHERE;"
     dq_attrs[CM_ATTR_QUALITY_TYPE] = "Completeness"
     client.update_custom_metadata_attributes(term.guid, dq_attrs)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
     _validate_dq_attributes(t.get_custom_metadata(name=cm_name))
 
 
 @pytest.mark.order(after="test_add_term_cm_dq")
 def test_update_term_cm_ipr(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     cm_ipr: CustomMetadataDef,
     term: AtlasGlossaryTerm,
 ):
-    cm_name = make_unique("IPR")
+    cm_name = CM_IPR
     ipr = CustomMetadataDict(cm_name)
     # Note: MUST access the getter / setter, not the underlying store
     ipr[CM_ATTR_IPR_MANDATORY] = False
     client.update_custom_metadata_attributes(term.guid, ipr)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
     _validate_ipr_attributes(t.get_custom_metadata(name=cm_name), mandatory=False)
-    _validate_raci_attributes(
-        client, make_unique, t.get_custom_metadata(name=make_unique("RACI"))
-    )
-    _validate_dq_attributes(t.get_custom_metadata(name=make_unique("DQ")))
+    _validate_raci_attributes(client, t.get_custom_metadata(name=CM_RACI))
+    _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
 
 
 @pytest.mark.order(after="test_update_term_cm_ipr")
 def test_replace_term_cm_raci(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     cm_raci: CustomMetadataDef,
     term: AtlasGlossaryTerm,
 ):
-    CM_RACI = make_unique("RACI")
-    CM_IPR = make_unique("IPR")
-    CM_QUALITY = make_unique("DQ")
     raci = CustomMetadataDict(CM_RACI)
-    group1, group2 = _get_groups(client, make_unique)
+    group1, group2 = _get_groups(client)
     raci[CM_ATTR_RACI_RESPONSIBLE] = [FIXED_USER]
     raci[CM_ATTR_RACI_ACCOUNTABLE] = FIXED_USER
     raci[CM_ATTR_RACI_CONSULTED] = None
     raci[CM_ATTR_RACI_INFORMED] = [group1.name, group2.name]
     client.replace_custom_metadata(term.guid, raci)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
-    _validate_raci_attributes_replacement(
-        client, make_unique, t.get_custom_metadata(name=CM_RACI)
-    )
+    _validate_raci_attributes_replacement(client, t.get_custom_metadata(name=CM_RACI))
     _validate_ipr_attributes(t.get_custom_metadata(name=CM_IPR), mandatory=False)
     _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
 
 
 @pytest.mark.order(after="test_replace_term_cm_raci")
 def test_replace_term_cm_ipr(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     cm_ipr: CustomMetadataDef,
     term: AtlasGlossaryTerm,
 ):
-    CM_RACI = make_unique("RACI")
-    CM_IPR = make_unique("IPR")
-    CM_QUALITY = make_unique("DQ")
     term_cm_ipr = CustomMetadataDict(CM_IPR)
     client.replace_custom_metadata(term.guid, term_cm_ipr)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
-    _validate_raci_attributes_replacement(
-        client, make_unique, t.get_custom_metadata(name=CM_RACI)
-    )
+    _validate_raci_attributes_replacement(client, t.get_custom_metadata(name=CM_RACI))
     _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
     _validate_ipr_empty(t.get_custom_metadata(name=CM_IPR))
 
 
 @pytest.mark.order(after="test_replace_term_cm_ipr")
 def test_search_by_any_accountable(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     cm_raci: CustomMetadataDef,
     glossary: AtlasGlossary,
     term: AtlasGlossaryTerm,
 ):
     be_active = Term.with_state("ACTIVE")
     be_a_term = Term.with_type_name("AtlasGlossaryTerm")
     have_attr = Exists.with_custom_metadata(
-        set_name=make_unique("RACI"), attr_name=CM_ATTR_RACI_ACCOUNTABLE
+        set_name=CM_RACI, attr_name=CM_ATTR_RACI_ACCOUNTABLE
     )
     query = Bool(must=[be_active, be_a_term, have_attr])
     dsl = DSL(query=query)
     request = IndexSearchRequest(
         dsl=dsl, attributes=["name", "anchor"], relation_attributes=["name"]
     )
     response = client.search(criteria=request)
@@ -559,23 +530,22 @@
         assert anchor
         assert anchor.name == glossary.name
 
 
 @pytest.mark.order(after="test_replace_term_cm_ipr")
 def test_search_by_specific_accountable(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     cm_raci: CustomMetadataDef,
     glossary: AtlasGlossary,
     term: AtlasGlossaryTerm,
 ):
     be_active = Term.with_state("ACTIVE")
     be_a_term = Term.with_type_name("AtlasGlossaryTerm")
     have_attr = Term.with_custom_metadata(
-        set_name=make_unique("RACI"),
+        set_name=CM_RACI,
         attr_name=CM_ATTR_RACI_ACCOUNTABLE,
         value=FIXED_USER,
     )
     query = Bool(must=[be_active, be_a_term, have_attr])
     dsl = DSL(query=query)
     request = IndexSearchRequest(
         dsl=dsl, attributes=["name", "anchor"], relation_attributes=["name"]
@@ -599,53 +569,43 @@
 
 
 @pytest.mark.order(
     after=["test_search_by_any_accountable", "test_search_by_specific_accountable"]
 )
 def test_remove_term_cm_raci(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     cm_raci: CustomMetadataDef,
     term: AtlasGlossaryTerm,
 ):
-    CM_RACI = make_unique("RACI")
-    CM_IPR = make_unique("IPR")
-    CM_QUALITY = make_unique("DQ")
     client.remove_custom_metadata(term.guid, cm_name=CM_RACI)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
     _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
     _validate_ipr_empty(t.get_custom_metadata(name=CM_IPR))
     _validate_raci_empty(t.get_custom_metadata(name=CM_RACI))
 
 
 @pytest.mark.order(after="test_remove_term_cm_raci")
 def test_remove_term_cm_ipr(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     cm_ipr: CustomMetadataDef,
     term: AtlasGlossaryTerm,
 ):
-    CM_RACI = make_unique("RACI")
-    CM_IPR = make_unique("IPR")
-    CM_QUALITY = make_unique("DQ")
     client.remove_custom_metadata(term.guid, cm_name=CM_IPR)
     t = client.retrieve_minimal(guid=term.guid, asset_type=AtlasGlossaryTerm)
     assert t
     _validate_dq_attributes(t.get_custom_metadata(name=CM_QUALITY))
     _validate_ipr_empty(t.get_custom_metadata(name=CM_IPR))
     _validate_raci_empty(t.get_custom_metadata(name=CM_RACI))
 
 
 @pytest.mark.order(after="test_remove_term_cm_raci")
-def test_remove_attribute(
-    client: AtlanClient, make_unique: Callable[[str], str], cm_raci: CustomMetadataDef
-):
+def test_remove_attribute(client: AtlanClient, cm_raci: CustomMetadataDef):
     global _removal_epoch
-    cm_name = make_unique("RACI")
+    cm_name = CM_RACI
     existing = CustomMetadataCache.get_custom_metadata_def(name=cm_name)
     existing_attrs = existing.attribute_defs
     updated_attrs = []
     for existing_attr in existing_attrs:
         to_keep = existing_attr
         if existing_attr.display_name == CM_ATTR_RACI_EXTRA:
             to_keep = existing_attr.archive(by="test-automation")
@@ -670,22 +630,17 @@
     assert archived.name != CM_ATTR_RACI_EXTRA
     assert archived.type_name == AtlanCustomAttributePrimitiveType.STRING.value
     assert not archived.options.multi_value_select
     assert archived.is_archived()
 
 
 @pytest.mark.order(after="test_remove_attribute")
-def test_retrieve_structures(
-    client: AtlanClient, make_unique: Callable[[str], str], cm_raci: CustomMetadataDef
-):
+def test_retrieve_structures(client: AtlanClient, cm_raci: CustomMetadataDef):
     global _removal_epoch
     custom_attributes = CustomMetadataCache.get_all_custom_attributes()
-    CM_RACI = make_unique("RACI")
-    CM_IPR = make_unique("IPR")
-    CM_QUALITY = make_unique("DQ")
     assert custom_attributes
     assert len(custom_attributes) >= 3
     assert CM_RACI in custom_attributes.keys()
     assert CM_IPR in custom_attributes.keys()
     assert CM_QUALITY in custom_attributes.keys()
     extra = _validate_raci_structure(custom_attributes.get(CM_RACI), 4)
     assert not extra
@@ -703,18 +658,15 @@
     assert extra.type_name == AtlanCustomAttributePrimitiveType.STRING.value
     assert "Database" in extra.options.custom_applicable_entity_types
     assert not extra.options.multi_value_select
     assert extra.is_archived()
 
 
 @pytest.mark.order(after="test_retrieve_structures")
-def test_recreate_attribute(
-    client: AtlanClient, make_unique: Callable[[str], str], cm_raci: CustomMetadataDef
-):
-    CM_RACI = make_unique("RACI")
+def test_recreate_attribute(client: AtlanClient, cm_raci: CustomMetadataDef):
     existing = CustomMetadataCache.get_custom_metadata_def(name=CM_RACI)
     existing_attrs = existing.attribute_defs
     updated_attrs = []
     for existing_attr in existing_attrs:
         existing_attr.is_new = None
         updated_attrs.append(existing_attr)
     new_attr = AttributeDef.create(
@@ -739,19 +691,16 @@
     assert extra.type_name == AtlanCustomAttributePrimitiveType.STRING.value
     assert not extra.options.multi_value_select
     assert not extra.is_archived()
 
 
 @pytest.mark.order(after="test_recreate_attribute")
 def test_retrieve_structure_without_archived(
-    client: AtlanClient, make_unique: Callable[[str], str], cm_raci: CustomMetadataDef
+    client: AtlanClient, cm_raci: CustomMetadataDef
 ):
-    CM_RACI = make_unique("RACI")
-    CM_IPR = make_unique("IPR")
-    CM_QUALITY = make_unique("DQ")
     custom_attributes = CustomMetadataCache.get_all_custom_attributes()
     assert custom_attributes
     assert len(custom_attributes) >= 3
     assert CM_RACI in custom_attributes.keys()
     assert CM_IPR in custom_attributes.keys()
     assert CM_QUALITY in custom_attributes.keys()
     extra = _validate_raci_structure(custom_attributes.get(CM_RACI), 5)
@@ -761,19 +710,16 @@
     assert extra.type_name == AtlanCustomAttributePrimitiveType.STRING.value
     assert "Database" in extra.options.custom_applicable_entity_types
     assert not extra.is_archived()
 
 
 @pytest.mark.order(after="test_recreate_attribute")
 def test_retrieve_structure_with_archived(
-    client: AtlanClient, make_unique: Callable[[str], str], cm_raci: CustomMetadataDef
+    client: AtlanClient, cm_raci: CustomMetadataDef
 ):
-    CM_RACI = make_unique("RACI")
-    CM_IPR = make_unique("IPR")
-    CM_QUALITY = make_unique("DQ")
     custom_attributes = CustomMetadataCache.get_all_custom_attributes(
         include_deleted=True
     )
     assert custom_attributes
     assert len(custom_attributes) >= 3
     assert CM_RACI in custom_attributes.keys()
     assert CM_IPR in custom_attributes.keys()
@@ -791,21 +737,17 @@
 def test_update_replacing_cm(
     term: AtlasGlossaryTerm,
     glossary: AtlasGlossary,
     cm_raci: CustomMetadataDef,
     cm_ipr: CustomMetadataDef,
     cm_dq: CustomMetadataDef,
     client: AtlanClient,
-    make_unique: Callable[[str], str],
 ):
-    CM_RACI = make_unique("RACI")
-    CM_IPR = make_unique("IPR")
-    CM_QUALITY = make_unique("DQ")
     raci = CustomMetadataDict(CM_RACI)
-    group1, group2 = _get_groups(client, make_unique)
+    group1, group2 = _get_groups(client)
     raci[CM_ATTR_RACI_RESPONSIBLE] = [FIXED_USER]
     raci[CM_ATTR_RACI_ACCOUNTABLE] = FIXED_USER
     raci[CM_ATTR_RACI_CONSULTED] = [group1.name]
     raci[CM_ATTR_RACI_INFORMED] = [group1.name, group2.name]
     raci[CM_ATTR_RACI_EXTRA] = "something extra..."
     to_update = AtlasGlossaryTerm.create_for_modification(
         qualified_name=term.qualified_name, name=term.name, glossary_guid=glossary.guid
@@ -823,52 +765,48 @@
     x = client.get_asset_by_qualified_name(
         qualified_name=term.qualified_name, asset_type=AtlasGlossaryTerm
     )
     assert x
     assert not x.is_incomplete
     assert x.qualified_name == term.qualified_name
     raci = x.get_custom_metadata(CM_RACI)
-    _validate_raci_attributes(client, make_unique, raci)
+    _validate_raci_attributes(client, raci)
     assert raci[CM_ATTR_RACI_EXTRA] == "something extra..."
     _validate_ipr_empty(x.get_custom_metadata(CM_IPR))
     _validate_dq_empty(x.get_custom_metadata(CM_QUALITY))
 
 
 # TODO: test entity audit retrieval and parsing, once available
 
 
-def _validate_raci_attributes(
-    client: AtlanClient, make_unique: Callable[[str], str], cma: CustomMetadataDict
-):
+def _validate_raci_attributes(client: AtlanClient, cma: CustomMetadataDict):
     assert cma
     # Note: MUST access the getter / setter, not the underlying store
     responsible = cma[CM_ATTR_RACI_RESPONSIBLE]
     accountable = cma[CM_ATTR_RACI_ACCOUNTABLE]
     consulted = cma[CM_ATTR_RACI_CONSULTED]
     informed = cma[CM_ATTR_RACI_INFORMED]
-    group1, group2 = _get_groups(client, make_unique)
+    group1, group2 = _get_groups(client)
     assert responsible
     assert len(responsible) == 1
     assert FIXED_USER in responsible
     assert accountable
     assert accountable == FIXED_USER
     assert consulted == [group1.name]
     assert informed == [group1.name, group2.name]
 
 
-def _validate_raci_attributes_replacement(
-    client: AtlanClient, make_unique: Callable[[str], str], cma: CustomMetadataDict
-):
+def _validate_raci_attributes_replacement(client: AtlanClient, cma: CustomMetadataDict):
     assert cma
     # Note: MUST access the getter / setter, not the underlying store
     responsible = cma[CM_ATTR_RACI_RESPONSIBLE]
     accountable = cma[CM_ATTR_RACI_ACCOUNTABLE]
     consulted = cma[CM_ATTR_RACI_CONSULTED]
     informed = cma[CM_ATTR_RACI_INFORMED]
-    group1, group2 = _get_groups(client, make_unique)
+    group1, group2 = _get_groups(client)
     assert responsible
     assert responsible == [FIXED_USER]
     assert accountable
     assert accountable == FIXED_USER
     assert not consulted
     assert informed == [group1.name, group2.name]
 
@@ -1002,18 +940,16 @@
     if total_expected > 4:
         return attributes[total_expected - 1]
     return None
 
 
 def test_add_badge_cm_dq(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     cm_dq: CustomMetadataDef,
 ):
-    CM_QUALITY = make_unique("DQ")
     badge = Badge.create(
         name=CM_ATTR_QUALITY_COUNT,
         cm_name=CM_QUALITY,
         cm_attribute=CM_ATTR_QUALITY_COUNT,
         badge_conditions=[
             BadgeCondition.create(
                 badge_condition_operator=BadgeComparisonOperator.GTE,
```

### Comparing `pyatlan-0.1.0/tests/integration/glossary_test.py` & `pyatlan-0.1.1/tests/integration/glossary_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
-from typing import Callable, Generator
+from typing import Generator
 
 import pytest
 from pydantic import StrictStr
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.assets import AtlasGlossary, AtlasGlossaryTerm
-from tests.integration.client import delete_asset
+from tests.integration.client import TestId, delete_asset
 
-MODULE_NAME = "GLS"
+MODULE_NAME = TestId.make_unique("GLS")
+
+TERM_NAME1 = f"{MODULE_NAME}1"
+TERM_NAME2 = f"{MODULE_NAME}2"
 
 
 def create_glossary(client: AtlanClient, name: str) -> AtlasGlossary:
     g = AtlasGlossary.create(name=StrictStr(name))
     r = client.upsert(g)
     return r.assets_created(AtlasGlossary)[0]
 
@@ -27,79 +30,72 @@
     r = client.upsert(t)
     return r.assets_created(AtlasGlossaryTerm)[0]
 
 
 @pytest.fixture(scope="module")
 def glossary(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
 ) -> Generator[AtlasGlossary, None, None]:
-    glossary_name = make_unique(f"{MODULE_NAME}")
-    g = create_glossary(client, glossary_name)
+    g = create_glossary(client, MODULE_NAME)
     yield g
     delete_asset(client, guid=g.guid, asset_type=AtlasGlossary)
 
 
 def test_glossary(
     glossary: AtlasGlossary,
-    make_unique: Callable[[str], str],
 ):
     assert glossary.guid
-    assert glossary.name == make_unique(f"{MODULE_NAME}")
+    assert glossary.name == MODULE_NAME
     assert glossary.qualified_name
-    assert glossary.qualified_name != make_unique(f"{MODULE_NAME}")
+    assert glossary.qualified_name != MODULE_NAME
 
 
 @pytest.fixture(scope="module")
 def term1(
-    client: AtlanClient, make_unique: Callable[[str], str], glossary: AtlasGlossary
+    client: AtlanClient, glossary: AtlasGlossary
 ) -> Generator[AtlasGlossaryTerm, None, None]:
-    term_name1 = make_unique(f"{MODULE_NAME}1")
-    t = create_term(client, name=term_name1, glossary_guid=glossary.guid)
+    t = create_term(client, name=TERM_NAME1, glossary_guid=glossary.guid)
     yield t
     delete_asset(client, guid=t.guid, asset_type=AtlasGlossaryTerm)
 
 
 def test_term1(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     term1: AtlasGlossaryTerm,
     glossary: AtlasGlossary,
 ):
     assert term1.guid
-    assert term1.name == make_unique(f"{MODULE_NAME}1")
+    assert term1.name == TERM_NAME1
     assert term1.qualified_name
-    assert term1.qualified_name != make_unique(f"{MODULE_NAME}1")
+    assert term1.qualified_name != TERM_NAME1
     t = client.get_asset_by_guid(term1.guid, asset_type=AtlasGlossaryTerm)
     assert t
     assert t.guid == term1.guid
     assert t.attributes.anchor
     assert t.attributes.anchor.guid == glossary.guid
 
 
 @pytest.fixture(scope="module")
 def term2(
-    client: AtlanClient, make_unique: Callable[[str], str], glossary: AtlasGlossary
+    client: AtlanClient, glossary: AtlasGlossary
 ) -> Generator[AtlasGlossaryTerm, None, None]:
-    term_name2 = make_unique(f"{MODULE_NAME}2")
-    t = create_term(client, name=term_name2, glossary_guid=glossary.guid)
+    t = create_term(client, name=TERM_NAME2, glossary_guid=glossary.guid)
     yield t
     delete_asset(client, guid=t.guid, asset_type=AtlasGlossaryTerm)
 
 
 def test_term2(
     client: AtlanClient,
-    make_unique: Callable[[str], str],
     term2: AtlasGlossaryTerm,
     glossary: AtlasGlossary,
 ):
     assert term2.guid
-    assert term2.name == make_unique(f"{MODULE_NAME}2")
+    assert term2.name == TERM_NAME2
     assert term2.qualified_name
-    assert term2.qualified_name != make_unique(f"{MODULE_NAME}2")
+    assert term2.qualified_name != TERM_NAME2
     t = client.get_asset_by_guid(term2.guid, asset_type=AtlasGlossaryTerm)
     assert t
     assert t.guid == term2.guid
     assert t.attributes.anchor
     assert t.attributes.anchor.guid == glossary.guid
```

### Comparing `pyatlan-0.1.0/tests/integration/lineage_test.py` & `pyatlan-0.1.1/tests/integration/lineage_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 import time
-from typing import Callable, Generator
+from typing import Generator
 
 import pytest
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.assets import (
     Column,
     Connection,
@@ -15,129 +15,134 @@
     Schema,
     Table,
     View,
 )
 from pyatlan.model.enums import AtlanConnectorType, EntityStatus, LineageDirection
 from pyatlan.model.lineage import LineageListRequest, LineageRequest
 from pyatlan.model.search import DSL, Bool, IndexSearchRequest, Prefix, Term
-from tests.integration.client import delete_asset
+from tests.integration.client import TestId, delete_asset
 from tests.integration.connection_test import create_connection
 
-MODULE_NAME = "lineage"
+MODULE_NAME = TestId.make_unique("lineage")
+
+DATABASE_NAME = f"{MODULE_NAME}_db"
+SCHEMA_NAME = f"{MODULE_NAME}_schema"
+TABLE_NAME = f"{MODULE_NAME}_tbl"
+MVIEW_NAME = f"{MODULE_NAME}_mv"
+VIEW_NAME = f"{MODULE_NAME}_v"
+COLUMN_NAME1 = f"{MODULE_NAME}1"
+COLUMN_NAME2 = f"{MODULE_NAME}2"
+COLUMN_NAME3 = f"{MODULE_NAME}3"
+COLUMN_NAME4 = f"{MODULE_NAME}4"
+COLUMN_NAME5 = f"{MODULE_NAME}5"
+COLUMN_NAME6 = f"{MODULE_NAME}6"
+
 CONNECTOR_TYPE = AtlanConnectorType.VERTICA
 
 
 @pytest.fixture(scope="module")
-def connection(
-    client: AtlanClient, make_unique: Callable[[str], str]
-) -> Generator[Connection, None, None]:
-    connection_name = make_unique(MODULE_NAME)
+def connection(client: AtlanClient) -> Generator[Connection, None, None]:
     result = create_connection(
-        client=client, name=connection_name, connector_type=CONNECTOR_TYPE
+        client=client, name=MODULE_NAME, connector_type=CONNECTOR_TYPE
     )
     yield result
     # TODO: proper connection delete workflow
     delete_asset(client, guid=result.guid, asset_type=Connection)
 
 
 @pytest.fixture(scope="module")
 def database(
-    client: AtlanClient, connection: Connection, make_unique: Callable[[str], str]
+    client: AtlanClient, connection: Connection
 ) -> Generator[Database, None, None]:
-    database_name = make_unique(MODULE_NAME + "_db")
+    db = create_database(
+        client=client, connection=connection, database_name=DATABASE_NAME
+    )
+    yield db
+    delete_asset(client, guid=db.guid, asset_type=Database)
+
+
+def create_database(client, connection, database_name: str):
     to_create = Database.create(
         name=database_name, connection_qualified_name=connection.qualified_name
     )
     result = client.upsert(to_create)
-    db = result.assets_created(asset_type=Database)[0]
-    yield db
-    delete_asset(client, guid=db.guid, asset_type=Database)
+    return result.assets_created(asset_type=Database)[0]
 
 
 @pytest.fixture(scope="module")
 def schema(
     client: AtlanClient,
     connection: Connection,
     database: Database,
-    make_unique: Callable[[str], str],
 ) -> Generator[Schema, None, None]:
-    schema_name = make_unique(MODULE_NAME + "_schema")
     to_create = Schema.create(
-        name=schema_name, database_qualified_name=database.qualified_name
+        name=SCHEMA_NAME, database_qualified_name=database.qualified_name
     )
     result = client.upsert(to_create)
     sch = result.assets_created(asset_type=Schema)[0]
     yield sch
     delete_asset(client, guid=sch.guid, asset_type=Schema)
 
 
 @pytest.fixture(scope="module")
 def table(
     client: AtlanClient,
     connection: Connection,
     database: Database,
     schema: Schema,
-    make_unique: Callable[[str], str],
 ) -> Generator[Table, None, None]:
-    table_name = make_unique(MODULE_NAME + "_tbl")
     to_create = Table.create(
-        name=table_name, schema_qualified_name=schema.qualified_name
+        name=TABLE_NAME, schema_qualified_name=schema.qualified_name
     )
     result = client.upsert(to_create)
     tbl = result.assets_created(asset_type=Table)[0]
     yield tbl
     delete_asset(client, guid=tbl.guid, asset_type=Table)
 
 
 @pytest.fixture(scope="module")
 def mview(
     client: AtlanClient,
     connection: Connection,
     database: Database,
     schema: Schema,
-    make_unique: Callable[[str], str],
 ) -> Generator[MaterialisedView, None, None]:
-    mview_name = make_unique(MODULE_NAME + "_mv")
     to_create = MaterialisedView.create(
-        name=mview_name, schema_qualified_name=schema.qualified_name
+        name=MVIEW_NAME, schema_qualified_name=schema.qualified_name
     )
     result = client.upsert(to_create)
     mv = result.assets_created(asset_type=MaterialisedView)[0]
     yield mv
     delete_asset(client, guid=mv.guid, asset_type=MaterialisedView)
 
 
 @pytest.fixture(scope="module")
 def view(
     client: AtlanClient,
     connection: Connection,
     database: Database,
     schema: Schema,
-    make_unique: Callable[[str], str],
 ) -> Generator[View, None, None]:
-    view_name = make_unique(MODULE_NAME + "_v")
-    to_create = View.create(name=view_name, schema_qualified_name=schema.qualified_name)
+    to_create = View.create(name=VIEW_NAME, schema_qualified_name=schema.qualified_name)
     result = client.upsert(to_create)
     v = result.assets_created(asset_type=View)[0]
     yield v
     delete_asset(client, guid=v.guid, asset_type=View)
 
 
 @pytest.fixture(scope="module")
 def column1(
     client: AtlanClient,
     connection: Connection,
     database: Database,
     schema: Schema,
     table: Table,
-    make_unique: Callable[[str], str],
 ) -> Generator[Column, None, None]:
-    column_name = make_unique(MODULE_NAME + "1")
     to_create = Column.create(
-        name=column_name,
+        name=COLUMN_NAME1,
         parent_type=Table,
         parent_qualified_name=table.qualified_name,
         order=1,
     )
     result = client.upsert(to_create)
     c = result.assets_created(asset_type=Column)[0]
     yield c
@@ -147,19 +152,17 @@
 @pytest.fixture(scope="module")
 def column2(
     client: AtlanClient,
     connection: Connection,
     database: Database,
     schema: Schema,
     table: Table,
-    make_unique: Callable[[str], str],
 ) -> Generator[Column, None, None]:
-    column_name = make_unique(MODULE_NAME + "2")
     to_create = Column.create(
-        name=column_name,
+        name=COLUMN_NAME2,
         parent_type=Table,
         parent_qualified_name=table.qualified_name,
         order=2,
     )
     result = client.upsert(to_create)
     c = result.assets_created(asset_type=Column)[0]
     yield c
@@ -169,19 +172,17 @@
 @pytest.fixture(scope="module")
 def column3(
     client: AtlanClient,
     connection: Connection,
     database: Database,
     schema: Schema,
     mview: MaterialisedView,
-    make_unique: Callable[[str], str],
 ) -> Generator[Column, None, None]:
-    column_name = make_unique(MODULE_NAME + "3")
     to_create = Column.create(
-        name=column_name,
+        name=COLUMN_NAME3,
         parent_type=MaterialisedView,
         parent_qualified_name=mview.qualified_name,
         order=1,
     )
     result = client.upsert(to_create)
     c = result.assets_created(asset_type=Column)[0]
     yield c
@@ -191,19 +192,17 @@
 @pytest.fixture(scope="module")
 def column4(
     client: AtlanClient,
     connection: Connection,
     database: Database,
     schema: Schema,
     mview: MaterialisedView,
-    make_unique: Callable[[str], str],
 ) -> Generator[Column, None, None]:
-    column_name = make_unique(MODULE_NAME + "4")
     to_create = Column.create(
-        name=column_name,
+        name=COLUMN_NAME4,
         parent_type=MaterialisedView,
         parent_qualified_name=mview.qualified_name,
         order=2,
     )
     result = client.upsert(to_create)
     c = result.assets_created(asset_type=Column)[0]
     yield c
@@ -213,19 +212,17 @@
 @pytest.fixture(scope="module")
 def column5(
     client: AtlanClient,
     connection: Connection,
     database: Database,
     schema: Schema,
     view: View,
-    make_unique: Callable[[str], str],
 ) -> Generator[Column, None, None]:
-    column_name = make_unique(MODULE_NAME + "5")
     to_create = Column.create(
-        name=column_name,
+        name=COLUMN_NAME5,
         parent_type=View,
         parent_qualified_name=view.qualified_name,
         order=1,
     )
     result = client.upsert(to_create)
     c = result.assets_created(asset_type=Column)[0]
     yield c
@@ -235,19 +232,17 @@
 @pytest.fixture(scope="module")
 def column6(
     client: AtlanClient,
     connection: Connection,
     database: Database,
     schema: Schema,
     view: View,
-    make_unique: Callable[[str], str],
 ) -> Generator[Column, None, None]:
-    column_name = make_unique(MODULE_NAME + "6")
     to_create = Column.create(
-        name=column_name,
+        name=COLUMN_NAME6,
         parent_type=View,
         parent_qualified_name=view.qualified_name,
         order=2,
     )
     result = client.upsert(to_create)
     c = result.assets_created(asset_type=Column)[0]
     yield c
@@ -259,15 +254,14 @@
     client: AtlanClient,
     connection: Connection,
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
-    make_unique: Callable[[str], str],
 ) -> Generator[Process, None, None]:
     process_name = f"{table.name} >> {mview.name}"
     to_create = Process.create(
         name=process_name,
         connection_qualified_name=connection.qualified_name,
         inputs=[Table.ref_by_guid(table.guid)],
         outputs=[MaterialisedView.ref_by_guid(mview.guid)],
@@ -283,15 +277,14 @@
     connection: Connection,
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
-    make_unique: Callable[[str], str],
 ):
     assert lineage_start
     assert lineage_start.guid
     assert lineage_start.qualified_name
     assert lineage_start.name == f"{table.name} >> {mview.name}"
     assert lineage_start.inputs
     assert len(lineage_start.inputs) == 1
@@ -310,15 +303,14 @@
     client: AtlanClient,
     connection: Connection,
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
-    make_unique: Callable[[str], str],
 ) -> Generator[Process, None, None]:
     process_name = f"{mview.name} >> {view.name}"
     to_create = Process.create(
         name=process_name,
         connection_qualified_name=connection.qualified_name,
         inputs=[MaterialisedView.ref_by_guid(mview.guid)],
         outputs=[View.ref_by_guid(view.guid)],
@@ -334,15 +326,14 @@
     connection: Connection,
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
     lineage_end: Process,
-    make_unique: Callable[[str], str],
 ):
     assert lineage_end
     assert lineage_end.guid
     assert lineage_end.qualified_name
     assert lineage_end.name == f"{mview.name} >> {view.name}"
     assert lineage_end.inputs
     assert len(lineage_end.inputs) == 1
@@ -362,15 +353,14 @@
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
     lineage_end: Process,
-    make_unique: Callable[[str], str],
 ):
     lineage = LineageRequest(guid=table.guid, hide_process=True)
     response = client.get_lineage(lineage)
     assert response
     assert response.base_entity_guid == table.guid
     assert not response.get_upstream_asset_guids()
     downstream_guids = response.get_downstream_asset_guids()
@@ -402,15 +392,14 @@
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
     lineage_end: Process,
-    make_unique: Callable[[str], str],
 ):
     lineage = LineageListRequest.create(guid=table.guid)
     lineage.attributes = ["name"]
     response = client.get_lineage_list(lineage)
     assert response
     assert response.entities
     assert len(response.entities) == 4
@@ -435,15 +424,14 @@
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
     lineage_end: Process,
-    make_unique: Callable[[str], str],
 ):
     lineage = LineageRequest(guid=mview.guid, hide_process=True)
     response = client.get_lineage(lineage)
     assert response
     assert response.base_entity_guid == mview.guid
     upstream_guids = response.get_upstream_asset_guids()
     assert upstream_guids
@@ -495,15 +483,14 @@
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
     lineage_end: Process,
-    make_unique: Callable[[str], str],
 ):
     lineage = LineageListRequest.create(guid=mview.guid)
     lineage.attributes = ["name"]
     response = client.get_lineage_list(lineage)
     assert response
     assert response.entities
     assert len(response.entities) == 2
@@ -529,15 +516,14 @@
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
     lineage_end: Process,
-    make_unique: Callable[[str], str],
 ):
     lineage = LineageRequest(guid=view.guid, hide_process=True)
     response = client.get_lineage(lineage)
     assert response
     assert response.base_entity_guid == view.guid
     upstream_guids = response.get_upstream_asset_guids()
     assert upstream_guids
@@ -573,15 +559,14 @@
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
     lineage_end: Process,
-    make_unique: Callable[[str], str],
 ):
     lineage = LineageListRequest.create(guid=view.guid)
     lineage.attributes = ["name"]
     response = client.get_lineage_list(lineage)
     assert response
     assert not response.entities
     assert not response.has_more
@@ -606,15 +591,14 @@
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
     lineage_end: Process,
-    make_unique: Callable[[str], str],
 ):
     be_active = Term.with_state("ACTIVE")
     have_lineage = Term.with_has_lineage(True)
     be_a_sql_type = Term.with_super_type_names("SQL")
     with_qn_prefix = Prefix.with_qualified_name(connection.qualified_name)
     query = Bool(must=[be_active, have_lineage, be_a_sql_type, with_qn_prefix])
     dsl = DSL(query=query)
@@ -663,15 +647,14 @@
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
     lineage_end: Process,
-    make_unique: Callable[[str], str],
 ):
     response = client.delete_entity_by_guid(lineage_start.guid)
     assert response
     deleted = response.assets_deleted(asset_type=Process)
     assert len(deleted) == 1
     one = deleted[0]
     assert one
@@ -688,15 +671,14 @@
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
     lineage_end: Process,
-    make_unique: Callable[[str], str],
 ):
     to_restore = Process.create_for_modification(
         lineage_start.qualified_name, lineage_start.name
     )
     to_restore.status = EntityStatus.ACTIVE
     client.upsert(to_restore)
     restored = client.get_asset_by_guid(lineage_start.guid, asset_type=Process)
@@ -719,15 +701,14 @@
     database: Database,
     schema: Schema,
     table: Table,
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
     lineage_end: Process,
-    make_unique: Callable[[str], str],
 ):
     response = client.purge_entity_by_guid(lineage_start.guid)
     assert response
     purged = response.assets_deleted(asset_type=Process)
     assert len(purged) == 1
     one = purged[0]
     assert one
```

### Comparing `pyatlan-0.1.0/tests/integration/query_parser_test.py` & `pyatlan-0.1.1/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/tests/integration/s3_asset_test.py` & `pyatlan-0.1.1/tests/integration/s3_asset_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,56 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
-from typing import Callable, Generator
+from typing import Generator
 
 import pytest
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.assets import Connection, S3Bucket
 from pyatlan.model.enums import AtlanConnectorType
-from tests.integration.client import delete_asset
+from tests.integration.client import TestId, delete_asset
 from tests.integration.connection_test import create_connection
 
-MODULE_NAME = "S3"
+MODULE_NAME = TestId.make_unique("S3")
+
 CONNECTOR_TYPE = AtlanConnectorType.S3
 ARN = "arn:aws:s3:::"
+BUCKET_NAME = MODULE_NAME
+BUCKET_ARN = f"{ARN}{MODULE_NAME}"
 
 
 @pytest.fixture(scope="module")
-def connection(
-    client: AtlanClient, make_unique: Callable[[str], str]
-) -> Generator[Connection, None, None]:
-    connection_name = make_unique(MODULE_NAME)
+def connection(client: AtlanClient) -> Generator[Connection, None, None]:
     result = create_connection(
-        client=client, name=connection_name, connector_type=CONNECTOR_TYPE
+        client=client, name=MODULE_NAME, connector_type=CONNECTOR_TYPE
     )
     yield result
     # TODO: proper connection delete workflow
     delete_asset(client, guid=result.guid, asset_type=Connection)
 
 
 @pytest.fixture(scope="module")
 def bucket(
-    client: AtlanClient, connection: Connection, make_unique: Callable[[str], str]
+    client: AtlanClient, connection: Connection
 ) -> Generator[S3Bucket, None, None]:
-    bucket_name = make_unique(MODULE_NAME)
-    bucket_arn = make_unique(ARN + MODULE_NAME)
     to_create = S3Bucket.create(
-        name=bucket_name,
+        name=BUCKET_NAME,
         connection_qualified_name=connection.qualified_name,
-        aws_arn=bucket_arn,
+        aws_arn=BUCKET_ARN,
     )
     response = client.upsert(to_create)
     result = response.assets_created(asset_type=S3Bucket)[0]
     yield result
     delete_asset(client, guid=result.guid, asset_type=S3Bucket)
 
 
 def test_bucket(
     client: AtlanClient,
     connection: Connection,
     bucket: S3Bucket,
-    make_unique: Callable[[str], str],
 ):
     assert bucket
     assert bucket.guid
     assert bucket.qualified_name
-    assert bucket.name == make_unique(MODULE_NAME)
-    assert bucket.aws_arn == make_unique(ARN + MODULE_NAME)
+    assert bucket.name == BUCKET_NAME
+    assert bucket.aws_arn == BUCKET_ARN
     assert bucket.connector_name == AtlanConnectorType.S3.value
```

### Comparing `pyatlan-0.1.0/tests/integration/test_client.py` & `pyatlan-0.1.1/tests/integration/test_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,264 +1,315 @@
-from itertools import count
-from typing import Callable, Generator
+from typing import Generator
 
 import pytest
 
 from pyatlan.client.atlan import AtlanClient
-from pyatlan.model.assets import AtlasGlossary, AtlasGlossaryTerm, Connection, Database
-from pyatlan.model.enums import AtlanConnectorType
-from pyatlan.model.lineage import LineageRequest
+from pyatlan.error import NotFoundError
+from pyatlan.model.assets import (
+    Announcement,
+    AtlasGlossary,
+    AtlasGlossaryTerm,
+    Connection,
+    Database,
+    Table,
+)
+from pyatlan.model.enums import AnnouncementType, AtlanConnectorType, CertificateStatus
+from tests.integration.client import TestId
+from tests.integration.lineage_test import create_database, delete_asset
 
-iter_count = count(1)
+CLASSIFICATION_NAME = "Issue"
 
 
-@pytest.fixture(scope="module")
-def m_client() -> AtlanClient:
-    from os import environ
-
-    client = AtlanClient(
-        base_url=environ["MARK_BASE_URL"], api_key=environ["MARK_API_KEY"]
-    )
-    AtlanClient.register_client(client)
-    return client
-
-
-@pytest.fixture(scope="module")
-def connection(m_client) -> Connection:
-    return m_client.get_asset_by_guid(
-        "b3a5c49a-0c7c-4e66-8453-f4da8d9ce222", Connection
+@pytest.fixture()
+def announcement():
+    return Announcement(
+        announcement_title="Important Announcement",
+        announcement_message="Very important info",
+        announcement_type=AnnouncementType.ISSUE,
     )
 
 
-@pytest.fixture(scope="module")
-def glossary(m_client: AtlanClient) -> Generator[AtlasGlossary, None, None]:
-    glossary = AtlasGlossary.create(name="Integration Test Glossary")
-    glossary = m_client.upsert(glossary).assets_created(asset_type=AtlasGlossary)[0]
-    yield glossary
-    m_client.purge_entity_by_guid(guid=glossary.guid)
-
-
 @pytest.fixture()
 def database(
-    m_client: AtlanClient, connection: Connection
+    client: AtlanClient, connection: Connection
 ) -> Generator[Database, None, None]:
-    database = Database.create(
-        name=f"Integration_Test_Entity_DB{next(iter_count)}",
-        connection_qualified_name=connection.attributes.qualified_name,
-    )
-    database = m_client.upsert(database).assets_created(Database)[0]
-
-    yield database
-
-    m_client.purge_entity_by_guid(guid=database.guid)
-
-
-@pytest.fixture()
-def make_term(
-    m_client: AtlanClient, glossary
-) -> Generator[Callable[[str], AtlasGlossaryTerm], None, None]:
-    created_term_guids = []
-
-    def _make_term(name: str) -> AtlasGlossaryTerm:
-        term = AtlasGlossaryTerm.create(
-            name=f"Integration Test Glossary Term {name}", anchor=glossary
-        )
-        term = m_client.upsert(term).assets_created(AtlasGlossaryTerm)[0]
-        created_term_guids.append(term.guid)
-        return term
-
-    yield _make_term
-
-    for guid in created_term_guids:
-        m_client.purge_entity_by_guid(guid=guid)
-
-
-def test_register_client_with_bad_parameter_raises_valueerror():
-    with pytest.raises(ValueError, match="client must be an instance of AtlanClient"):
-        AtlanClient.register_client("")
-    assert AtlanClient.get_default_client() is None
-
-
-def test_register_client():
-    client = AtlanClient(base_url="http://mark.atlan.com", api_key="123")
-    AtlanClient.register_client(client)
-    assert AtlanClient.get_default_client() == client
+    """Get a database with function scope"""
+    database_name = TestId.make_unique("my_db")
+    db = create_database(client, connection, database_name)
+    yield db
+    delete_asset(client, guid=db.guid, asset_type=Database)
 
 
 def test_append_terms_with_guid(
-    m_client: AtlanClient,
-    make_term: Callable[[str], AtlasGlossaryTerm],
-    database: Database,
+    client: AtlanClient, term1: AtlasGlossaryTerm, database: Database
 ):
-    term = make_term("Term1")
 
     assert (
-        database := m_client.append_terms(
-            guid=database.guid, asset_type=Database, terms=[term]
+        database := client.append_terms(
+            guid=database.guid, asset_type=Database, terms=[term1]
         )
     )
-    database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
+    database = client.get_asset_by_guid(guid=database.guid, asset_type=Database)
     assert database.assigned_terms
     assert len(database.assigned_terms) == 1
-    assert database.assigned_terms[0].guid == term.guid
+    assert database.assigned_terms[0].guid == term1.guid
 
 
 def test_append_terms_with_qualified_name(
-    m_client: AtlanClient,
-    make_term: Callable[[str], AtlasGlossaryTerm],
+    client: AtlanClient,
+    term1: AtlasGlossaryTerm,
     database: Database,
 ):
-    term = make_term("Term1")
 
     assert (
-        database := m_client.append_terms(
-            qualified_name=database.qualified_name, asset_type=Database, terms=[term]
+        database := client.append_terms(
+            qualified_name=database.qualified_name, asset_type=Database, terms=[term1]
         )
     )
-    database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
+    database = client.get_asset_by_guid(guid=database.guid, asset_type=Database)
     assert database.assigned_terms
     assert len(database.assigned_terms) == 1
-    assert database.assigned_terms[0].guid == term.guid
+    assert database.assigned_terms[0].guid == term1.guid
 
 
 def test_append_terms_using_ref_by_guid_for_term(
-    m_client: AtlanClient,
-    make_term: Callable[[str], AtlasGlossaryTerm],
+    client: AtlanClient,
+    term1: AtlasGlossaryTerm,
     database: Database,
 ):
-    term = make_term("Term1")
 
     assert (
-        database := m_client.append_terms(
+        database := client.append_terms(
             qualified_name=database.qualified_name,
             asset_type=Database,
-            terms=[AtlasGlossaryTerm.ref_by_guid(guid=term.guid)],
+            terms=[AtlasGlossaryTerm.ref_by_guid(guid=term1.guid)],
         )
     )
-    database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
+    database = client.get_asset_by_guid(guid=database.guid, asset_type=Database)
     assert database.assigned_terms
     assert len(database.assigned_terms) == 1
-    assert database.assigned_terms[0].guid == term.guid
+    assert database.assigned_terms[0].guid == term1.guid
 
 
 def test_replace_a_term(
-    m_client: AtlanClient,
-    make_term: Callable[[str], AtlasGlossaryTerm],
+    client: AtlanClient,
+    term1: AtlasGlossaryTerm,
+    term2: AtlasGlossaryTerm,
     database: Database,
 ):
-    original_term = make_term("Term1")
     assert (
-        database := m_client.append_terms(
+        database := client.append_terms(
             qualified_name=database.qualified_name,
             asset_type=Database,
-            terms=[AtlasGlossaryTerm.ref_by_guid(guid=original_term.guid)],
+            terms=[AtlasGlossaryTerm.ref_by_guid(guid=term1.guid)],
         )
     )
 
-    replacemant_term = make_term("Term2")
     assert (
-        database := m_client.replace_terms(
-            guid=database.guid, asset_type=Database, terms=[replacemant_term]
+        database := client.replace_terms(
+            guid=database.guid, asset_type=Database, terms=[term2]
         )
     )
 
-    database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
+    database = client.get_asset_by_guid(guid=database.guid, asset_type=Database)
     assert database.assigned_terms
     assert len(database.assigned_terms) == 2
     deleted_terms = [
         t for t in database.assigned_terms if t.relationship_status == "DELETED"
     ]
     assert len(deleted_terms) == 1
-    assert deleted_terms[0].guid == original_term.guid
+    assert deleted_terms[0].guid == term1.guid
     active_terms = [
         t for t in database.assigned_terms if t.relationship_status != "DELETED"
     ]
     assert len(active_terms) == 1
-    assert active_terms[0].guid == replacemant_term.guid
+    assert active_terms[0].guid == term2.guid
 
 
 def test_replace_all_term(
-    m_client: AtlanClient,
-    make_term: Callable[[str], AtlasGlossaryTerm],
+    client: AtlanClient,
+    term1: AtlasGlossaryTerm,
     database: Database,
 ):
-    original_term = make_term("Term1")
+
     assert (
-        database := m_client.append_terms(
+        database := client.append_terms(
             qualified_name=database.qualified_name,
             asset_type=Database,
-            terms=[AtlasGlossaryTerm.ref_by_guid(guid=original_term.guid)],
+            terms=[AtlasGlossaryTerm.ref_by_guid(guid=term1.guid)],
         )
     )
 
     assert (
-        database := m_client.replace_terms(
+        database := client.replace_terms(
             guid=database.guid, asset_type=Database, terms=[]
         )
     )
 
-    database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
+    database = client.get_asset_by_guid(guid=database.guid, asset_type=Database)
     assert database.assigned_terms
     assert len(database.assigned_terms) == 1
     deleted_terms = [
         t for t in database.assigned_terms if t.relationship_status == "DELETED"
     ]
     assert len(deleted_terms) == 1
-    assert deleted_terms[0].guid == original_term.guid
+    assert deleted_terms[0].guid == term1.guid
 
 
 def test_remove_term(
-    m_client: AtlanClient,
-    make_term: Callable[[str], AtlasGlossaryTerm],
+    client: AtlanClient,
+    term1: AtlasGlossaryTerm,
+    term2: AtlasGlossaryTerm,
     database: Database,
 ):
-    original_term = make_term("Term1")
-    another_term = make_term("Term2")
+
     assert (
-        database := m_client.append_terms(
+        database := client.append_terms(
             qualified_name=database.qualified_name,
             asset_type=Database,
             terms=[
-                AtlasGlossaryTerm.ref_by_guid(guid=original_term.guid),
-                AtlasGlossaryTerm.ref_by_guid(guid=another_term.guid),
+                AtlasGlossaryTerm.ref_by_guid(guid=term1.guid),
+                AtlasGlossaryTerm.ref_by_guid(guid=term2.guid),
             ],
         )
     )
 
     assert (
-        database := m_client.remove_terms(
+        database := client.remove_terms(
             guid=database.guid,
             asset_type=Database,
-            terms=[AtlasGlossaryTerm.ref_by_guid(original_term.guid)],
+            terms=[AtlasGlossaryTerm.ref_by_guid(term1.guid)],
         )
     )
 
-    database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
+    database = client.get_asset_by_guid(guid=database.guid, asset_type=Database)
     assert database.assigned_terms
     assert len(database.assigned_terms) == 2
     deleted_terms = [
         t for t in database.assigned_terms if t.relationship_status == "DELETED"
     ]
     assert len(deleted_terms) == 1
-    assert deleted_terms[0].guid == original_term.guid
+    assert deleted_terms[0].guid == term1.guid
     active_terms = [
         t for t in database.assigned_terms if t.relationship_status != "DELETED"
     ]
-    assert active_terms[0].guid == another_term.guid
+    assert active_terms[0].guid == term2.guid
 
 
-def test_find_connections_by_name(m_client: AtlanClient):
-    connections = m_client.find_connections_by_name(
-        name="Test Connection",
+def test_find_connections_by_name(client: AtlanClient):
+    connections = client.find_connections_by_name(
+        name="development",
         connector_type=AtlanConnectorType.SNOWFLAKE,
         attributes=["connectorName"],
     )
     assert len(connections) == 1
     assert connections[0].connector_name == AtlanConnectorType.SNOWFLAKE.value
 
 
-def test_get_lineage(m_client: AtlanClient):
-    response = m_client.get_lineage(
-        LineageRequest(guid="75474eab-3105-4ef9-9f84-709e386a7d3e")
+def test_get_asset_by_guid_good_guid(client: AtlanClient, glossary: AtlasGlossary):
+    glossary = client.get_asset_by_guid(glossary.guid, AtlasGlossary)
+    assert isinstance(glossary, AtlasGlossary)
+
+
+def test_get_asset_by_guid_when_table_specified_and_glossary_returned_raises_not_found_error(
+    client: AtlanClient, glossary: AtlasGlossary
+):
+    with pytest.raises(NotFoundError) as ex_info:
+        guid = glossary.guid
+        client.get_asset_by_guid(guid, Table)
+    assert (
+        f"Asset with GUID {guid} is not of the type requested: Table."
+        in ex_info.value.args[0]
+    )
+
+
+def test_get_asset_by_guid_bad_with_non_existent_guid_raises_not_found_error(
+    client: AtlanClient,
+):
+    with pytest.raises(
+        NotFoundError, match="Given instance guid 76d54dd6 is invalid/not found"
+    ):
+        client.get_asset_by_guid("76d54dd6", AtlasGlossary)
+
+
+def test_upsert_when_no_changes(client: AtlanClient, glossary: AtlasGlossary):
+    response = client.upsert(glossary)
+    assert not response.guid_assignments
+    assert not response.mutated_entities
+
+
+def test_get_by_qualified_name(client: AtlanClient, glossary: AtlasGlossary):
+    qualified_name = glossary.qualified_name
+    glossary = client.get_asset_by_qualified_name(
+        qualified_name=qualified_name, asset_type=AtlasGlossary
+    )
+    assert glossary.attributes.qualified_name == qualified_name
+
+
+def test_add_classification(client: AtlanClient, term1: AtlasGlossaryTerm):
+    client.add_classifications(
+        AtlasGlossaryTerm, term1.qualified_name, [CLASSIFICATION_NAME]
+    )
+    glossary_term = client.get_asset_by_guid(term1.guid, asset_type=AtlasGlossaryTerm)
+    assert glossary_term.classifications
+    assert len(glossary_term.classifications) == 1
+    classification = glossary_term.classifications[0]
+    assert str(classification.type_name) == CLASSIFICATION_NAME
+
+
+@pytest.mark.order(after="test_add_classification")
+def test_remove_classification(client: AtlanClient, term1: AtlasGlossaryTerm):
+    client.remove_classification(
+        AtlasGlossaryTerm, term1.qualified_name, CLASSIFICATION_NAME
+    )
+    glossary_term = client.get_asset_by_guid(term1.guid, asset_type=AtlasGlossaryTerm)
+    assert not glossary_term.classifications
+
+
+def test_update_certificate(client: AtlanClient, glossary: AtlasGlossary):
+    message = "An important message"
+    client.update_certificate(
+        asset_type=AtlasGlossary,
+        qualified_name=glossary.qualified_name,
+        name=glossary.name,
+        certificate_status=CertificateStatus.DRAFT,
+        message=message,
+    )
+    glossary = client.get_asset_by_guid(guid=glossary.guid, asset_type=AtlasGlossary)
+    assert glossary.certificate_status == CertificateStatus.DRAFT
+    assert glossary.certificate_status_message == message
+
+
+@pytest.mark.order(after="test_update_certificate")
+def test_remove_certificate(client: AtlanClient, glossary: AtlasGlossary):
+    client.remove_certificate(
+        asset_type=AtlasGlossary,
+        qualified_name=glossary.qualified_name,
+        name=glossary.name,
+    )
+    glossary = client.get_asset_by_guid(guid=glossary.guid, asset_type=AtlasGlossary)
+    assert glossary.certificate_status is None
+    assert glossary.certificate_status_message is None
+
+
+def test_update_announcement(
+    client: AtlanClient, glossary: AtlasGlossary, announcement: Announcement
+):
+    client.update_announcement(
+        asset_type=AtlasGlossary,
+        qualified_name=glossary.qualified_name,
+        name=glossary.name,
+        announcement=announcement,
+    )
+    glossary = client.get_asset_by_guid(guid=glossary.guid, asset_type=AtlasGlossary)
+    assert glossary.get_announcment() == announcement
+
+
+@pytest.mark.order(after="test_update_certificate")
+def test_remove_announcement(client: AtlanClient, glossary: AtlasGlossary):
+    client.remove_announcement(
+        asset_type=AtlasGlossary,
+        qualified_name=glossary.qualified_name,
+        name=glossary.name,
     )
-    for guid, asset in response.guid_entity_map.items():
-        assert guid == asset.guid
+    glossary = client.get_asset_by_guid(guid=glossary.guid, asset_type=AtlasGlossary)
+    assert glossary.get_announcment() is None
```

### Comparing `pyatlan-0.1.0/tests/integration/test_index_search.py` & `pyatlan-0.1.1/tests/integration/test_index_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 from dataclasses import dataclass, field
+from datetime import datetime
+from time import time
 from typing import Generator
 
 import pytest
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.assets import Asset
 from pyatlan.model.enums import AtlanConnectorType
@@ -16,14 +18,17 @@
     Prefix,
     Range,
     Regexp,
     Term,
     Wildcard,
 )
 
+NOW_AS_TIMESTAMP = int(time() * 1000)
+NOW_AS_YYYY_MM_DD = datetime.today().strftime("%Y-%m-%d")
+
 VALUES_FOR_TERM_QUERIES = {
     "with_categories": "VBsYc9dUoEcAtDxZmjby6@mweSfpXBwfYWedQTvA3Gi",
     "with_classification_names": "RBmhFJqX50bl5RAeJhwt1a",
     "with_classifications_text": "VBsYc9dUoEcAtDxZmjby6@mweSfpXBwfYWedQTvA3Gi",
     "with_connector_name": AtlanConnectorType.SNOWFLAKE,
     "with_create_time_as_timestamp": 1665727666701,
     "with_created_by": "bryan",
@@ -74,25 +79,14 @@
 @dataclass()
 class AssetTracker:
     missing_types: set[str] = field(default_factory=set)
     found_types: set[str] = field(default_factory=set)
 
 
 @pytest.fixture(scope="module")
-def m_client() -> AtlanClient:
-    from os import environ
-
-    client = AtlanClient(
-        base_url=environ["MARK_BASE_URL"], api_key=environ["MARK_API_KEY"]
-    )
-    AtlanClient.register_client(client)
-    return client
-
-
-@pytest.fixture(scope="module")
 def asset_tracker() -> Generator[AssetTracker, None, None]:
     tracker = AssetTracker()
     yield tracker
     print("Total number of asset types found: ", len(tracker.found_types))
     print("Total number of asset types missing: ", len(tracker.missing_types))
     print("Assets were not found for the following types:")
     for name in sorted(tracker.missing_types):
@@ -109,84 +103,78 @@
         all_subclasses.append(subclass)
         all_subclasses.extend(get_all_subclasses(subclass))
 
     return all_subclasses
 
 
 @pytest.mark.parametrize("cls", [(cls) for cls in get_all_subclasses(Asset)])
-def test_search(m_client: AtlanClient, asset_tracker, cls):
+def test_search(client: AtlanClient, asset_tracker, cls):
     name = cls.__name__
     query = Term.with_state("ACTIVE")
     post_filter = Term.with_type_name(name)
     dsl = DSL(query=query, post_filter=post_filter)
     request = IndexSearchRequest(dsl=dsl, attributes=["name"])
-    results = m_client.search(criteria=request)
+    results = client.search(criteria=request)
     if results.count > 0:
         asset_tracker.found_types.add(name)
         counter = 0
         for asset in results:
             assert isinstance(asset, cls)
             counter += 1
             if counter > 3:
                 break
     else:
         asset_tracker.missing_types.add(name)
 
 
-def test_search_next_page(m_client: AtlanClient):
+def test_search_next_page(client: AtlanClient):
     size = 15
     dsl = DSL(
         query=Term.with_state("ACTIVE"),
-        post_filter=Term.with_type_name(value="Database"),
+        post_filter=Term.with_type_name(value="Table"),
         size=size,
     )
-    request = IndexSearchRequest(
-        dsl=dsl,
-        attributes=["databaseName"],
-    )
-    results = m_client.search(criteria=request)
+    request = IndexSearchRequest(dsl=dsl)
+    results = client.search(criteria=request)
     assert results.count > size
     assert len(results.current_page()) == size
     counter = 0
     while True:
         for _ in results.current_page():
             counter += 1
         if results.next_page() is not True:
             break
     assert counter == results.count
 
 
-def test_search_iter(m_client: AtlanClient):
+def test_search_iter(client: AtlanClient):
     size = 15
     dsl = DSL(
         query=Term.with_state("ACTIVE"),
-        post_filter=Term.with_type_name("Database"),
+        post_filter=Term.with_type_name("Table"),
         size=size,
     )
-    request = IndexSearchRequest(
-        dsl=dsl,
-        attributes=["databaseName"],
-    )
-    results = m_client.search(criteria=request)
+    request = IndexSearchRequest(dsl=dsl)
+    results = client.search(criteria=request)
     assert results.count > size
     assert len([a for a in results]) == results.count
 
 
-def test_search_next_when_start_changed_returns_remaining(m_client: AtlanClient):
+def test_search_next_when_start_changed_returns_remaining(client: AtlanClient):
     size = 2
     dsl = DSL(
         query=Term.with_state("ACTIVE"),
         post_filter=Term.with_type_name("Database"),
         size=size,
     )
     request = IndexSearchRequest(
         dsl=dsl,
         attributes=["databaseName"],
     )
-    results = m_client.search(criteria=request)
+    results = client.search(criteria=request)
     assert results.next_page(start=results.count - size) is True
     assert len(list(results)) == size
 
 
 @pytest.fixture()
 def term_query_value(request):
     return VALUES_FOR_TERM_QUERIES[request.param]
@@ -203,85 +191,86 @@
         (method, method, query)
         for query in [Term, Prefix, Regexp, Wildcard]
         for method in sorted(dir(query))
         if method.startswith("with_") and method != "with_custom_metadata"
     ],
     indirect=["term_query_value"],
 )
-def test_term_queries_factory(m_client: AtlanClient, term_query_value, method, clazz):
+def test_term_queries_factory(client: AtlanClient, term_query_value, method, clazz):
     assert hasattr(clazz, method)
     query = getattr(clazz, method)(term_query_value)
     filter = ~Term.with_type_name("__AtlasAuditEntry")
     dsl = DSL(query=query, post_filter=filter, size=1)
     request = IndexSearchRequest(
         dsl=dsl,
         attributes=["name"],
     )
-    results = m_client.search(criteria=request)
-    assert results.count > 0
+    results = client.search(criteria=request)
+    assert results.count >= 0
 
 
 @pytest.mark.parametrize(
     "with_name",
     [
         (method)
         for method in dir(Exists)
         if method.startswith("with_") and method != "with_custom_metadata"
     ],
 )
-def test_exists_query_factory(m_client: AtlanClient, with_name):
+def test_exists_query_factory(client: AtlanClient, with_name):
     assert hasattr(Exists, with_name)
     query = getattr(Exists, with_name)()
-    dsl = DSL(query=query, size=1)
+    filter = ~Term(field="__typeName.keyword", value="__AtlasAuditEntry")
+    dsl = DSL(query=query, post_filter=filter, size=1)
     request = IndexSearchRequest(
         dsl=dsl,
         attributes=["name"],
     )
-    results = m_client.search(criteria=request)
-    assert results.count > 0
+    results = client.search(criteria=request)
+    assert results.count >= 0
 
 
 @pytest.mark.parametrize(
     "text_query_value, method, clazz",
     [
         (method, method, query)
         for query in [Match]
         for method in sorted(dir(query))
         if method.startswith("with_")
     ],
     indirect=["text_query_value"],
 )
-def test_text_queries_factory(m_client: AtlanClient, text_query_value, method, clazz):
+def test_text_queries_factory(client: AtlanClient, text_query_value, method, clazz):
     assert hasattr(clazz, method)
     query = getattr(clazz, method)(text_query_value)
     filter = ~Term.with_type_name("__AtlasAuditEntry")
     dsl = DSL(query=query, post_filter=filter, size=1)
     request = IndexSearchRequest(
         dsl=dsl,
         attributes=["name"],
     )
     # print(request.json(by_alias=True, exclude_none=True))
-    results = m_client.search(criteria=request)
-    assert results.count > 0
+    results = client.search(criteria=request)
+    assert results.count >= 0
 
 
 @pytest.mark.parametrize(
     "value, method, format",
     [
         (0, "with_popularity_score", None),
-        (1665727666701, "with_create_time_as_timestamp", None),
-        ("2023-01", "with_create_time_as_date", "yyyy-MM"),
-        (1665727666701, "with_update_time_as_timestamp", None),
-        ("2023-01", "with_update_time_as_date", "yyyy-MM"),
+        (NOW_AS_TIMESTAMP, "with_create_time_as_timestamp", None),
+        (NOW_AS_YYYY_MM_DD, "with_create_time_as_date", "yyyy-MM-dd"),
+        (NOW_AS_TIMESTAMP, "with_update_time_as_timestamp", None),
+        (NOW_AS_YYYY_MM_DD, "with_update_time_as_date", "yyyy-MM-dd"),
     ],
 )
-def test_range_factory(m_client: AtlanClient, value, method, format):
+def test_range_factory(client: AtlanClient, value, method, format):
     assert hasattr(Range, method)
     query = getattr(Range, method)(lt=value, format=format)
-    filter = ~Term.with_type_name("__AtlasAuditEntry")
+    filter = ~Term(field="__typeName.keyword", value="__AtlasAuditEntry")
     dsl = DSL(query=query, post_filter=filter, size=1)
     request = IndexSearchRequest(
         dsl=dsl,
         attributes=["name"],
     )
-    results = m_client.search(criteria=request)
-    assert results.count > 0
+    results = client.search(criteria=request)
+    assert results.count >= 0
```

### Comparing `pyatlan-0.1.0/tests/unit/test_classification_name.py` & `pyatlan-0.1.1/tests/unit/test_classification_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/tests/unit/test_client.py` & `pyatlan-0.1.1/tests/unit/test_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -318,7 +318,26 @@
             asset := client.remove_terms(
                 guid=guid, asset_type=asset_type, terms=[exisiting_term]
             )
         )
         assert (updated_terms := asset.assigned_terms)
         assert len(updated_terms) == 1
         assert other_term in updated_terms
+
+
+def test_register_client_with_bad_parameter_raises_value_error():
+    with pytest.raises(ValueError, match="client must be an instance of AtlanClient"):
+        AtlanClient.register_client("")
+    assert AtlanClient.get_default_client() is None
+
+
+def test_register_client():
+    client = AtlanClient(base_url="http://mark.atlan.com", api_key="123")
+    AtlanClient.register_client(client)
+    assert AtlanClient.get_default_client() == client
+
+
+def test_reset_client():
+    client = AtlanClient(base_url="http://mark.atlan.com", api_key="123")
+    AtlanClient.register_client(client)
+    AtlanClient.reset_default_client()
+    assert AtlanClient.get_default_client() is None
```

### Comparing `pyatlan-0.1.0/tests/unit/test_custom_metadata.py` & `pyatlan-0.1.1/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/tests/unit/test_glossary_term.py` & `pyatlan-0.1.1/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/tests/unit/test_lineage.py` & `pyatlan-0.1.1/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/tests/unit/test_model.py` & `pyatlan-0.1.1/tests/unit/test_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,14 +71,23 @@
     MaterialisedView,
     MCIncident,
     MCMonitor,
     MetabaseCollection,
     MetabaseDashboard,
     MetabaseQuestion,
     Metric,
+    MicroStrategyAttribute,
+    MicroStrategyCube,
+    MicroStrategyDocument,
+    MicroStrategyDossier,
+    MicroStrategyFact,
+    MicroStrategyMetric,
+    MicroStrategyProject,
+    MicroStrategyReport,
+    MicroStrategyVisualization,
     ModeChart,
     ModeCollection,
     ModeQuery,
     ModeReport,
     ModeWorkspace,
     Namespace,
     PopularityInsights,
@@ -411,18 +420,28 @@
     "Optional[Database]": Database(),
     "Optional[list[MaterialisedView]]": [MaterialisedView()],
     "Optional[list[Procedure]]": [Procedure()],
     "Optional[list[SnowflakePipe]]": [SnowflakePipe()],
     "Optional[list[SnowflakeStream]]": [SnowflakeStream()],
     "Optional[list[SnowflakeTag]]": [SnowflakeTag()],
     "Optional[list[Schema]]": [Schema()],
+    "Optional[AuthPolicyType]": AuthPolicyType.ALLOW,
+    "Optional[list[MicroStrategyAttribute]]": [MicroStrategyAttribute()],
+    "Optional[list[MicroStrategyMetric]]": [MicroStrategyMetric()],
+    "Optional[MicroStrategyProject]": MicroStrategyProject(),
+    "Optional[list[MicroStrategyCube]]": [MicroStrategyCube()],
+    "Optional[list[MicroStrategyDocument]]": [MicroStrategyDocument()],
+    "Optional[list[MicroStrategyDossier]]": [MicroStrategyDossier()],
+    "Optional[list[MicroStrategyFact]]": [MicroStrategyFact()],
+    "Optional[list[MicroStrategyReport]]": [MicroStrategyReport()],
+    "Optional[list[MicroStrategyVisualization]]": [MicroStrategyVisualization()],
+    "Optional[MicroStrategyDossier]": MicroStrategyDossier(),
     "Optional[list[AuthPolicy]]": [AuthPolicy()],
     "Optional[AccessControl]": AccessControl(),
     "Optional[list[AuthPolicyCondition]]": [AuthPolicyCondition()],
-    "Optional[AuthPolicyType]": AuthPolicyType.ALLOW,
     "Optional[list[AuthPolicyValiditySchedule]]": [AuthPolicyValiditySchedule()],
 }
 
 
 def load_json(filename):
     with (DATA_DIR / filename).open() as input_file:
         return json.load(input_file)
@@ -679,37 +698,14 @@
             name="Integration Test Glossary", user_description="This a test glossary"
         )
     )
     assert "AtlasGlossary" == glossary.type_name
 
 
 @pytest.mark.parametrize(
-    "name, connector_type, admin_users, admin_groups, admin_roles, error",
-    [
-        (None, AtlanConnectorType.BIGQUERY, None, None, ["123"], ValueError),
-        ("", AtlanConnectorType.BIGQUERY, None, None, ["123"], ValueError),
-        ("query", None, None, None, ["123"], ValueError),
-        ("query", AtlanConnectorType.BIGQUERY, None, None, None, ValueError),
-        ("query", AtlanConnectorType.BIGQUERY, [], [], [], ValueError),
-    ],
-)
-def test_connection_attributes_create_without_required_parameters_raises_validation_error(
-    name, connector_type, admin_users, admin_groups, admin_roles, error
-):
-    with pytest.raises(error):
-        Connection.Attributes(
-            name=name,
-            connector_type=connector_type,
-            admin_users=admin_users,
-            admin_groups=admin_groups,
-            admin_roles=admin_roles,
-        ).validate_required()
-
-
-@pytest.mark.parametrize(
     "name, connector_type, admin_users, admin_groups, admin_roles",
     [
         ("query", AtlanConnectorType.BIGQUERY, {"bob"}, None, None),
         ("query", AtlanConnectorType.BIGQUERY, None, {"bob"}, None),
         ("query", AtlanConnectorType.BIGQUERY, None, None, {"bob"}),
         ("query", AtlanConnectorType.BIGQUERY, {"bob"}, {"ted"}, {"alice"}),
     ],
@@ -755,93 +751,14 @@
             admin_users=admin_users,
             admin_groups=admin_groups,
             admin_roles=admin_roles,
         )
 
 
 @pytest.mark.parametrize(
-    "name, qualified_name, connector_name, category, admin_users, admin_groups, admin_roles, msg",
-    [
-        (
-            "Bob",
-            AtlanConnectorType.BIGQUERY.to_qualified_name(),
-            AtlanConnectorType.BIGQUERY.value,
-            AtlanConnectorType.BIGQUERY.category.value,
-            None,
-            None,
-            None,
-            "One of admin_user, admin_groups or admin_roles is required",
-        ),
-        (
-            "Bob",
-            "",
-            AtlanConnectorType.BIGQUERY.value,
-            AtlanConnectorType.BIGQUERY.category.value,
-            ["Bob"],
-            None,
-            None,
-            "qualified_name is required",
-        ),
-        (
-            "Bob",
-            AtlanConnectorType.BIGQUERY.to_qualified_name(),
-            AtlanConnectorType.BIGQUERY.value,
-            "",
-            ["Bob"],
-            None,
-            None,
-            "category is required",
-        ),
-        (
-            "Bob",
-            AtlanConnectorType.BIGQUERY.to_qualified_name(),
-            "",
-            AtlanConnectorType.BIGQUERY.category.value,
-            ["Bob"],
-            None,
-            None,
-            "connector_name is required",
-        ),
-        (
-            "",
-            AtlanConnectorType.BIGQUERY.to_qualified_name(),
-            AtlanConnectorType.BIGQUERY.value,
-            AtlanConnectorType.BIGQUERY.category.value,
-            ["Bob"],
-            None,
-            None,
-            "name is required",
-        ),
-    ],
-)
-def test_connection_validate_required_when_fields_missing_raises_value_error(
-    name,
-    qualified_name,
-    connector_name,
-    category,
-    admin_users,
-    admin_groups,
-    admin_roles,
-    msg,
-):
-    a = Connection.Attributes(
-        name=name,
-        qualified_name=qualified_name,
-        connector_name=connector_name,
-        category=category,
-        admin_users=admin_users,
-        admin_groups=admin_groups,
-        admin_roles=admin_roles,
-    )
-    with pytest.raises(ValueError) as ve:
-        a.validate_required()
-    assert str(ve.value) == msg
-
-
-@pytest.mark.parametrize(
     "name, qualified_name, connector_name, category, admin_users, admin_groups, admin_roles",
     [
         (
             "Bob",
             AtlanConnectorType.BIGQUERY.to_qualified_name(),
             AtlanConnectorType.BIGQUERY.value,
             AtlanConnectorType.BIGQUERY.category.value,
```

### Comparing `pyatlan-0.1.0/tests/unit/test_search_model.py` & `pyatlan-0.1.1/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.0/tests/unit/test_typedef_model.py` & `pyatlan-0.1.1/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

