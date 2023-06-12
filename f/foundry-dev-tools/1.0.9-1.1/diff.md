# Comparing `tmp/foundry-dev-tools-1.0.9.tar.gz` & `tmp/foundry-dev-tools-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundry-dev-tools-1.0.9.tar", last modified: Thu Apr 27 12:23:55 2023, max compression
+gzip compressed data, was "foundry-dev-tools-1.1.tar", last modified: Mon Jun 12 09:26:18 2023, max compression
```

## Comparing `foundry-dev-tools-1.0.9.tar` & `foundry-dev-tools-1.1.tar`

### file list

```diff
@@ -1,107 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.788965 foundry-dev-tools-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.740965 foundry-dev-tools-1.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.740965 foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/blank_issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.744965 foundry-dev-tools-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-27 12:23:55.788965 foundry-dev-tools-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.752965 foundry-dev-tools-1.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/Configuration_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/FoundryFileSystem_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/FoundryRestClient_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/SSO_usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.752965 foundry-dev-tools-1.0.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/contributors.md
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/develop.md
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.756965 foundry-dev-tools-1.0.9/docs/pictures/
--rw-r--r--   0 runner    (1001) docker     (123)    28579 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-already-cached-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33149 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-already-cached-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-new-transaction-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41514 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-new-transaction-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    87463 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/pictures/tpa_config.png
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/usage_and_examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-27 12:23:55.788965 foundry-dev-tools-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.756965 foundry-dev-tools-1.0.9/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.760965 foundry-dev-tools-1.0.9/src/foundry_dev_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/cached_foundry_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    86863 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/foundry_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/fsspec_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.764965 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.768965 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/caches/metadata_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/caches/spark_caches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.768965 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/converter/foundry_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/spark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.768965 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/token_provider/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/token_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/token_provider/foundry_token_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.764965 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.772965 foundry-dev-tools-1.0.9/src/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.772965 foundry-dev-tools-1.0.9/src/transforms/api/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/transforms/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/transforms/api/_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/transforms/api/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/transforms/api/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/transforms/api/_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.784965 foundry-dev-tools-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/foundry_mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_cached_foundry_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_cached_foundry_client_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.732965 foundry-dev-tools-1.0.9/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.784965 foundry-dev-tools-1.0.9/tests/test_data/binary_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_data/binary_dataset/bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.784965 foundry-dev-tools-1.0.9/tests/test_data/iris/
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_data/iris/iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)    29252 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_foundry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_foundry_local_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_foundry_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_foundry_spark_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_foundry_sql_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33551 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_fsspec_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_multipass_tpa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_spark_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_token_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_transforms_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.595722 foundry-dev-tools-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.571722 foundry-dev-tools-1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.575722 foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/blank_issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.575722 foundry-dev-tools-1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-12 09:26:18.595722 foundry-dev-tools-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.579722 foundry-dev-tools-1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/Configuration_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/FoundryFileSystem_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/FoundryRestClient_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/SSO_usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.579722 foundry-dev-tools-1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/contributors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/develop.md
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.579722 foundry-dev-tools-1.1/docs/pictures/
+-rw-r--r--   0 runner    (1001) docker     (123)    28579 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-already-cached-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33149 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-already-cached-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-new-transaction-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41514 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-new-transaction-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    87463 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/pictures/tpa_config.png
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/usage_and_examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:26:18.595722 foundry-dev-tools-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.571722 foundry-dev-tools-1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.579722 foundry-dev-tools-1.1/src/foundry_dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/cached_foundry_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.583722 foundry-dev-tools-1.1/src/foundry_dev_tools/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90644 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/foundry_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19898 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/fsspec_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.583722 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.583722 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/caches/metadata_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/caches/spark_caches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.583722 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/converter/foundry_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/token_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.583722 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.587722 foundry-dev-tools-1.1/src/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.587722 foundry-dev-tools-1.1/src/transforms/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/transforms/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/transforms/api/_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/transforms/api/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/transforms/api/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/transforms/api/_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.591722 foundry-dev-tools-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22978 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/foundry_mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_cached_foundry_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_cached_foundry_client_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_cli_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.571722 foundry-dev-tools-1.1/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.595722 foundry-dev-tools-1.1/tests/test_data/binary_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_data/binary_dataset/bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.595722 foundry-dev-tools-1.1/tests/test_data/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_data/iris/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    29547 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_foundry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_foundry_local_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_foundry_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_foundry_spark_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_foundry_sql_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33976 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_fsspec_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_multipass_tpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_spark_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20200 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_transforms_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_utils_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tox.ini
```

### Comparing `foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/blank_issue.yml` & `foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/blank_issue.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/bug_report.yml` & `foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/feature_request.yml` & `foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/.github/pull_request_template.md` & `foundry-dev-tools-1.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/.github/workflows/ci.yml` & `foundry-dev-tools-1.1/.github/workflows/ci.yml`

 * *Files 19% similar despite different names*

```diff
@@ -9,38 +9,37 @@
   workflow_dispatch:  # Allow manually triggering the workflow
   schedule:
     # Run roughly every 15 days at 00:00 UTC
     # (useful to check if updates on dependencies break the package)
     - cron: '0 0 1,16 * *'
 
 concurrency:
-  group: >-
-    ${{ github.workflow }}-${{ github.ref_type }}-
-    ${{ github.event.pull_request.number || github.sha }}
+  group: check-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
   prepare:
     runs-on: ubuntu-latest
     outputs:
       wheel-distribution: ${{ steps.wheel-distribution.outputs.path }}
     steps:
       - uses: actions/checkout@v3
         with: {fetch-depth: 0}  # deep clone for setuptools-scm
       - uses: actions/setup-python@v4
         id: setup-python
-        with: {python-version: "3.11"}
+        with: 
+          python-version: "3.11"
+          cache: "pip"
+          cache-dependency-path: "pyproject.toml"
       - name: Run static analysis and format checkers
         run: |
-          pip install .[testing,transforms]
-          pipx run --python '${{ steps.setup-python.outputs.python-path }}' tox -e lint
+          pip install .[testing,transforms] tox
+          tox -e lint
       - name: Build package distribution files
-        run: >-
-          pipx run --python '${{ steps.setup-python.outputs.python-path }}'
-          tox -e clean,build
+        run: tox -e clean,build
       - name: Record the path of wheel distribution
         id: wheel-distribution
         run: echo "path=$(ls dist/*.whl)" >> $GITHUB_OUTPUT
       - name: Store the distribution files for use in other stages
         # `tests` and `publish` will use the same pre-built distributions,
         # so we make sure to release the exact same package that was tested
         uses: actions/upload-artifact@v3
@@ -48,44 +47,53 @@
           name: python-distribution-files
           path: dist/
           retention-days: 1
 
   test:
     needs: prepare
     strategy:
+      fail-fast: false # always test both versions
       matrix:
         python:
         - "3.8"
         - "3.11"  # newest Python that is supported by pyspark
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         id: setup-python
         with:
           python-version: ${{ matrix.python }}
+          cache: "pip"
+          cache-dependency-path: "pyproject.toml"
       - name: Retrieve pre-built distribution files
         uses: actions/download-artifact@v3
         with: {name: python-distribution-files, path: dist/}
+      - name: Install tox
+        run: pip install tox
       - name: Run tests
         run: >-
-          pipx run --python '${{ steps.setup-python.outputs.python-path }}'
           tox --installpkg '${{ needs.prepare.outputs.wheel-distribution }}'
-          -- -rFEx --durations 10 --color yes  # pytest args
+          -- -rFEx --durations 10 --color yes -m "not integration"  # pytest args
 
   publish:
     needs: test
     if: ${{ github.event_name == 'push' && contains(github.ref, 'refs/tags/') }}
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
-        with: {python-version: "3.11"}
+        with:
+          python-version: "3.11"
+          cache: "pip"
+          cache-dependency-path: "pyproject.toml"
       - name: Retrieve pre-built distribution files
         uses: actions/download-artifact@v3
         with: {name: python-distribution-files, path: dist/}
+      - name: Install Tox
+        run: pip install tox
       - name: Publish Package
         env:
           TWINE_REPOSITORY: pypi
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
-        run: pipx run tox -e publish
+        run: tox -e publish
```

### Comparing `foundry-dev-tools-1.0.9/.github/workflows/docs.yml` & `foundry-dev-tools-1.1/.github/workflows/docs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,17 @@
       pages: write
       id-token: write
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with: {python-version: "3.11"}
       - name: Build Docs
-        run: >-
-          pipx run tox -e docs
+        run: |
+          pip install tox
+          tox -e docs
       - name: Upload docs artifact
         uses: actions/upload-pages-artifact@v1
         with:
           path: 'docs/_build/html'
 
   deploy:
     needs: build
```

### Comparing `foundry-dev-tools-1.0.9/.gitignore` & `foundry-dev-tools-1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/.pre-commit-config.yaml` & `foundry-dev-tools-1.1/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: mixed-line-ending
     args: ['--fix=lf']  # replace 'auto' with 'lf' to enforce Linux/Mac line endings or 'crlf' for Windows
-- repo: https://github.com/omnilib/ufmt
-  rev: v2.0.0
+- repo: https://github.com/charliermarsh/ruff-pre-commit
+  # Ruff version.
+  rev: 'v0.0.271'
   hooks:
-    - id: ufmt
-      additional_dependencies:
-        - black == 22.6.0
-        - usort == 1.0.4
--   repo: local
-    hooks:
-    -   id: pylint
-        name: pylint
-        entry: pylint
-        language: system
-        types: [python]
-        args: [
-        "-rn",
-       "-sn"
-        ]
-        exclude: "tests|docs"
+    - id: ruff
+      args: ["--fix","--exit-non-zero-on-fix","--show-fixes"]
+- repo: https://github.com/psf/black
+  rev: 23.3.0
+  hooks:
+    - id: black
+      # max support version of foundry-dev-tools
+      language_version: python3.11
```

### Comparing `foundry-dev-tools-1.0.9/LICENSE` & `foundry-dev-tools-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/PKG-INFO` & `foundry-dev-tools-1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: foundry-dev-tools
-Version: 1.0.9
+Version: 1.1
 Summary: Seamlessly run your Palantir Foundry Repository transforms code on your local machine.
-Home-page: https://github.com/emdgroup/foundry-dev-tools
-Author: Nicolas Renkamp, Jonas Wunderlich
-Author-email: nicolas.renkamp@merckgroup.com, jonas.wunderlich@merckgroup.com
-License: Apache License, Version 2.0
+Author-email: Nicolas Renkamp <nicolas.renkamp@merckgroup.com>, Jonas Wunderlich <jonas.wunderlich@merckgroup.com>
+License: Apache-2.0
+Project-URL: Homepage, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Documentation, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Source, https://github.com/emdgroup/foundry-dev-tools
 Project-URL: Tracker, https://github.com/emdgroup/foundry-dev-tools/issues
 Project-URL: Changelog, https://emdgroup.github.io/foundry-dev-tools/changelog.html
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -20,112 +19,116 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: <4.0,>=3.8
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: integration-testing
+Requires-Python: <4,>=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: integration
 Provides-Extra: testing
 Provides-Extra: transforms
+Provides-Extra: cli
 License-File: LICENSE
 
 <div align="center">
   <br/>
 
-  <a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/ci.yml?style=flat-square"/></img>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/docs.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/docs.yml?style=flat-square"/></img>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/pyversions/foundry-dev-tools?style=flat-square&label=Supported%20Python%20versions&color=%23ffb86c"/></a>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-square&label=PyPI%20version&color=%23bd93f9"/></a>
-  <a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/vn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Version&color=%23bd93f9" alt="Conda Version"/></a>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/dm/foundry-dev-tools?label=PyPI%20Downloads&style=flat-square&color=%236272a4"/></a>
-  <a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/dn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Downloads&color=%236272a4" alt="Conda Downloads"/></a>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/issues"><img src="https://img.shields.io/github/issues/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/pulls"><img src="https://img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
-  <a href="http://www.apache.org/licenses/LICENSE-2.0"><img src="https://shields.io/badge/License-Apache%202.0-green.svg?style=flat-square&color=%234c1"/></a>
+<a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/ci.yml?style=flat-square"/></img>
+<a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/docs.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/docs.yml?style=flat-square"/></img>
+<a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/pyversions/foundry-dev-tools?style=flat-square&label=Supported%20Python%20versions&color=%23ffb86c"/></a>
+<a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-square&label=PyPI%20version&color=%23bd93f9"/></a>
+<a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/vn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Version&color=%23bd93f9" alt="Conda Version"/></a>
+<a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/dm/foundry-dev-tools?label=PyPI%20Downloads&style=flat-square&color=%236272a4"/></a>
+<a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/dn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Downloads&color=%236272a4" alt="Conda Downloads"/></a>
+<a href="https://github.com/emdgroup/foundry-dev-tools/issues"><img src="https://img.shields.io/github/issues/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
+<a href="https://github.com/emdgroup/foundry-dev-tools/pulls"><img src="https://img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
+<a href="http://www.apache.org/licenses/LICENSE-2.0"><img src="https://shields.io/badge/License-Apache%202.0-green.svg?style=flat-square&color=%234c1"/></a>
+
   <p><a href="https://emdgroup.github.io/foundry-dev-tools">Documentation</a></p>
 
-  <a href="https://emdgroup.github.io/foundry-dev-tools/installation.html">Installation<a/>
-  &nbsp;•&nbsp;
-  <a href="https://emdgroup.github.io/foundry-dev-tools/usage_and_examples.html">Usage<a/>
-  &nbsp;•&nbsp;
-  <a href="https://emdgroup.github.io/foundry-dev-tools/develop.html">Development<a/>
+<a href="https://emdgroup.github.io/foundry-dev-tools/installation.html">Installation<a/>
+&nbsp;•&nbsp;
+<a href="https://emdgroup.github.io/foundry-dev-tools/usage_and_examples.html">Usage<a/>
+&nbsp;•&nbsp;
+<a href="https://emdgroup.github.io/foundry-dev-tools/develop.html">Development<a/>
 
 </div>
 
 # Foundry DevTools
 
 Seamlessly run your Palantir Foundry Repository transforms code and more on your local machine.
 Foundry DevTools is a set of useful libraries to interact with the Foundry APIs. There are currently three
 high level entrypoints to Foundry DevTools:
 
-* A [transforms](https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api/) implementation
+- A [transforms](https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api/) implementation
 
-  * An implementation of the Foundry `transforms` package that internally uses the `CachedFoundryClient`.
+  - An implementation of the Foundry `transforms` package that internally uses the `CachedFoundryClient`.
     This allows you to seamlessly run your Palantir Foundry Code Repository transforms code on your local machine.
-    Foundry DevTools does not cover all of Foundry's features, more on this [here](https://emdgroup.github.io/foundry-dev-tools/architecture.html#known-limitations).
+    Foundry DevTools does not cover all of Foundry's features, more on this [here](https://emdgroup.github.io/foundry-dev-tools/architecture.html#known-limitations-contributions-welcome).
 
-* [FoundryRestClient](https://emdgroup.github.io/foundry-dev-tools/FoundryRestClient_usage.html)
+- [FoundryRestClient](https://emdgroup.github.io/foundry-dev-tools/FoundryRestClient_usage.html)
 
-  * An API client that contains an opinionated client implementation to some of Foundry's APIs.
+  - An API client that contains an opinionated client implementation to some of Foundry's APIs.
 
-  * For example:
+  - For example:
 
     ```python
     from foundry_dev_tools import FoundryRestClient
 
     # Queries the Foundry SQL Server with spark SQL dialect
     rest_client = FoundryRestClient()
     df = rest_client.query_foundry_sql("SELECT * FROM `/Global/Foundry Training and Resources/Foundry Reference Project/Ontology Project: Aviation/airlines`", branch='master')
     df.shape
     # Out[2]: (17, 10)
     ```
 
-* [FoundryFileSystem](https://emdgroup.github.io/foundry-dev-tools/FoundryFileSystem_usage.html)
+- [FoundryFileSystem](https://emdgroup.github.io/foundry-dev-tools/FoundryFileSystem_usage.html)
 
-  * An implementation of `fsspec` for Foundry. Useful to interact with Foundry from popular data science libraries such as
-  `pandas` or `dask`.
+  - An implementation of `fsspec` for Foundry. Useful to interact with Foundry from popular data science libraries such as
+    `pandas` or `dask`.
 
-  * For example:
+  - For example:
 
     ```python
     import pandas as pd
     # /Global/Foundry Training and Resources/Foundry Reference Project/Ontology Project: Aviation/airlines
     df = pd.read_parquet("foundry://ri.foundry.main.dataset.5d78f3ae-a588-4fd8-9ba2-66827808c85f")
     df.shape
     # Out[2]: (17, 10)
     ```
 
-
 ## Quickstart
 
 With pip:
+
 ```shell
 pip install foundry-dev-tools
 ```
 
 With conda or mamba on the conda-forge channel:
+
 ```shell
 conda install -c conda-forge foundry-dev-tools
 ```
 
 [Further instructions](https://emdgroup.github.io/foundry-dev-tools/installation.html) can be found in our documentation.
 
 ## Why did we build this?
 
-* Local development experience in your favourite IDE (PyCharm, VSCode, ...)
-    * Access to modern developer tools and workflows such as pylint, black, isort, pre-commit hooks etc.
-* Quicker turnaround time when making changes
-    * Debug, change code and run in a matter of seconds instead of minutes
-* No accidental or auto commits
-    * Keep your git history clean
+- Local development experience in your favourite IDE (PyCharm, VSCode, ...)
+  - Access to modern developer tools and workflows such as pylint, black, isort, pre-commit hooks etc.
+- Quicker turnaround time when making changes
+  - Debug, change code and run in a matter of seconds instead of minutes
+- No accidental or auto commits
+  - Keep your git history clean
 
 # License
+
 Copyright (c) 2023 Merck KGaA, Darmstadt, Germany
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.0.9 Summary:
-Seamlessly run your Palantir Foundry Repository transforms code on your local
-machine. Home-page: https://github.com/emdgroup/foundry-dev-tools Author:
-Nicolas Renkamp, Jonas Wunderlich Author-email: nicolas.renkamp@merckgroup.com,
-jonas.wunderlich@merckgroup.com License: Apache License, Version 2.0 Project-
-URL: Documentation, https://emdgroup.github.io/foundry-dev-tools Project-URL:
-Source, https://github.com/emdgroup/foundry-dev-tools Project-URL: Tracker,
-https://github.com/emdgroup/foundry-dev-tools/issues Project-URL: Changelog,
-https://emdgroup.github.io/foundry-dev-tools/changelog.html Platform: any
-Classifier: Development Status :: 5 - Production/Stable Classifier: Programming
-Language :: Python Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Intended Audience ::
-Developers Classifier: Operating System :: POSIX :: Linux Classifier: Operating
-System :: MacOS Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Scientific/Engineering :: Information Analysis Requires-
-Python: <4.0,>=3.8 Description-Content-Type: text/markdown; charset=UTF-
-8 Provides-Extra: integration-testing Provides-Extra: testing Provides-Extra:
-transforms License-File: LICENSE
+Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.1 Summary: Seamlessly
+run your Palantir Foundry Repository transforms code on your local machine.
+Author-email: Nicolas Renkamp
+renkamp@merckgroup.com>, Jonas Wunderlich
+wunderlich@merckgroup.com> License: Apache-2.0 Project-URL: Homepage, https://
+emdgroup.github.io/foundry-dev-tools Project-URL: Documentation, https://
+emdgroup.github.io/foundry-dev-tools Project-URL: Source, https://github.com/
+emdgroup/foundry-dev-tools Project-URL: Tracker, https://github.com/emdgroup/
+foundry-dev-tools/issues Project-URL: Changelog, https://emdgroup.github.io/
+foundry-dev-tools/changelog.html Platform: any Classifier: Development Status
+:: 5 - Production/Stable Classifier: Programming Language :: Python Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Developers Classifier: Operating System ::
+POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Operating
+System :: Microsoft :: Windows Classifier: Topic :: Scientific/Engineering ::
+Information Analysis Requires-Python: <4,>=3.8 Description-Content-Type: text/
+markdown Provides-Extra: integration Provides-Extra: testing Provides-Extra:
+transforms Provides-Extra: cli License-File: LICENSE
 
  [https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-
                        tools/ci.yml?style=flat-square]
  [https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-
   tools/docs.yml?style=flat-square]_[https://img.shields.io/pypi/pyversions/
                          foundry-dev-tools?style=flat-
      square&label=Supported%20Python%20versions&color=%23ffb86c]_[https://
@@ -39,44 +39,45 @@
                                      â¢ 
                                      Usage
                                      â¢ 
                                   Development
 # Foundry DevTools Seamlessly run your Palantir Foundry Repository transforms
 code and more on your local machine. Foundry DevTools is a set of useful
 libraries to interact with the Foundry APIs. There are currently three high
-level entrypoints to Foundry DevTools: * A [transforms](https://
+level entrypoints to Foundry DevTools: - A [transforms](https://
 www.palantir.com/docs/foundry/transforms-python/transforms-python-api/
-) implementation * An implementation of the Foundry `transforms` package that
+) implementation - An implementation of the Foundry `transforms` package that
 internally uses the `CachedFoundryClient`. This allows you to seamlessly run
 your Palantir Foundry Code Repository transforms code on your local machine.
 Foundry DevTools does not cover all of Foundry's features, more on this [here]
 (https://emdgroup.github.io/foundry-dev-tools/architecture.html#known-
-limitations). * [FoundryRestClient](https://emdgroup.github.io/foundry-dev-
-tools/FoundryRestClient_usage.html) * An API client that contains an
-opinionated client implementation to some of Foundry's APIs. * For example:
-```python from foundry_dev_tools import FoundryRestClient # Queries the Foundry
-SQL Server with spark SQL dialect rest_client = FoundryRestClient() df =
-rest_client.query_foundry_sql("SELECT * FROM `/Global/Foundry Training and
-Resources/Foundry Reference Project/Ontology Project: Aviation/airlines`",
-branch='master') df.shape # Out[2]: (17, 10) ``` * [FoundryFileSystem](https://
-emdgroup.github.io/foundry-dev-tools/FoundryFileSystem_usage.html) * An
-implementation of `fsspec` for Foundry. Useful to interact with Foundry from
-popular data science libraries such as `pandas` or `dask`. * For example:
-```python import pandas as pd # /Global/Foundry Training and Resources/Foundry
-Reference Project/Ontology Project: Aviation/airlines df = pd.read_parquet
-("foundry://ri.foundry.main.dataset.5d78f3ae-a588-4fd8-9ba2-66827808c85f")
-df.shape # Out[2]: (17, 10) ``` ## Quickstart With pip: ```shell pip install
-foundry-dev-tools ``` With conda or mamba on the conda-forge channel: ```shell
-conda install -c conda-forge foundry-dev-tools ``` [Further instructions]
-(https://emdgroup.github.io/foundry-dev-tools/installation.html) can be found
-in our documentation. ## Why did we build this? * Local development experience
-in your favourite IDE (PyCharm, VSCode, ...) * Access to modern developer tools
-and workflows such as pylint, black, isort, pre-commit hooks etc. * Quicker
-turnaround time when making changes * Debug, change code and run in a matter of
-seconds instead of minutes * No accidental or auto commits * Keep your git
+limitations-contributions-welcome). - [FoundryRestClient](https://
+emdgroup.github.io/foundry-dev-tools/FoundryRestClient_usage.html) - An API
+client that contains an opinionated client implementation to some of Foundry's
+APIs. - For example: ```python from foundry_dev_tools import FoundryRestClient
+# Queries the Foundry SQL Server with spark SQL dialect rest_client =
+FoundryRestClient() df = rest_client.query_foundry_sql("SELECT * FROM `/Global/
+Foundry Training and Resources/Foundry Reference Project/Ontology Project:
+Aviation/airlines`", branch='master') df.shape # Out[2]: (17, 10) ``` -
+[FoundryFileSystem](https://emdgroup.github.io/foundry-dev-tools/
+FoundryFileSystem_usage.html) - An implementation of `fsspec` for Foundry.
+Useful to interact with Foundry from popular data science libraries such as
+`pandas` or `dask`. - For example: ```python import pandas as pd # /Global/
+Foundry Training and Resources/Foundry Reference Project/Ontology Project:
+Aviation/airlines df = pd.read_parquet("foundry://
+ri.foundry.main.dataset.5d78f3ae-a588-4fd8-9ba2-66827808c85f") df.shape # Out
+[2]: (17, 10) ``` ## Quickstart With pip: ```shell pip install foundry-dev-
+tools ``` With conda or mamba on the conda-forge channel: ```shell conda
+install -c conda-forge foundry-dev-tools ``` [Further instructions](https://
+emdgroup.github.io/foundry-dev-tools/installation.html) can be found in our
+documentation. ## Why did we build this? - Local development experience in your
+favourite IDE (PyCharm, VSCode, ...) - Access to modern developer tools and
+workflows such as pylint, black, isort, pre-commit hooks etc. - Quicker
+turnaround time when making changes - Debug, change code and run in a matter of
+seconds instead of minutes - No accidental or auto commits - Keep your git
 history clean # License Copyright (c) 2023 Merck KGaA, Darmstadt, Germany
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use
 this file except in compliance with the License. You may obtain a copy of the
 License at https://www.apache.org/licenses/LICENSE-2.0 Unless required by
 applicable law or agreed to in writing, software distributed under the License
 is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied. See the License for the specific language
```

### Comparing `foundry-dev-tools-1.0.9/README.md` & `foundry-dev-tools-1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,98 +1,101 @@
 <div align="center">
   <br/>
 
-  <a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/ci.yml?style=flat-square"/></img>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/docs.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/docs.yml?style=flat-square"/></img>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/pyversions/foundry-dev-tools?style=flat-square&label=Supported%20Python%20versions&color=%23ffb86c"/></a>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-square&label=PyPI%20version&color=%23bd93f9"/></a>
-  <a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/vn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Version&color=%23bd93f9" alt="Conda Version"/></a>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/dm/foundry-dev-tools?label=PyPI%20Downloads&style=flat-square&color=%236272a4"/></a>
-  <a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/dn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Downloads&color=%236272a4" alt="Conda Downloads"/></a>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/issues"><img src="https://img.shields.io/github/issues/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/pulls"><img src="https://img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
-  <a href="http://www.apache.org/licenses/LICENSE-2.0"><img src="https://shields.io/badge/License-Apache%202.0-green.svg?style=flat-square&color=%234c1"/></a>
+<a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/ci.yml?style=flat-square"/></img>
+<a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/docs.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/docs.yml?style=flat-square"/></img>
+<a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/pyversions/foundry-dev-tools?style=flat-square&label=Supported%20Python%20versions&color=%23ffb86c"/></a>
+<a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-square&label=PyPI%20version&color=%23bd93f9"/></a>
+<a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/vn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Version&color=%23bd93f9" alt="Conda Version"/></a>
+<a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/dm/foundry-dev-tools?label=PyPI%20Downloads&style=flat-square&color=%236272a4"/></a>
+<a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/dn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Downloads&color=%236272a4" alt="Conda Downloads"/></a>
+<a href="https://github.com/emdgroup/foundry-dev-tools/issues"><img src="https://img.shields.io/github/issues/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
+<a href="https://github.com/emdgroup/foundry-dev-tools/pulls"><img src="https://img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
+<a href="http://www.apache.org/licenses/LICENSE-2.0"><img src="https://shields.io/badge/License-Apache%202.0-green.svg?style=flat-square&color=%234c1"/></a>
+
   <p><a href="https://emdgroup.github.io/foundry-dev-tools">Documentation</a></p>
 
-  <a href="https://emdgroup.github.io/foundry-dev-tools/installation.html">Installation<a/>
-  &nbsp;•&nbsp;
-  <a href="https://emdgroup.github.io/foundry-dev-tools/usage_and_examples.html">Usage<a/>
-  &nbsp;•&nbsp;
-  <a href="https://emdgroup.github.io/foundry-dev-tools/develop.html">Development<a/>
+<a href="https://emdgroup.github.io/foundry-dev-tools/installation.html">Installation<a/>
+&nbsp;•&nbsp;
+<a href="https://emdgroup.github.io/foundry-dev-tools/usage_and_examples.html">Usage<a/>
+&nbsp;•&nbsp;
+<a href="https://emdgroup.github.io/foundry-dev-tools/develop.html">Development<a/>
 
 </div>
 
 # Foundry DevTools
 
 Seamlessly run your Palantir Foundry Repository transforms code and more on your local machine.
 Foundry DevTools is a set of useful libraries to interact with the Foundry APIs. There are currently three
 high level entrypoints to Foundry DevTools:
 
-* A [transforms](https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api/) implementation
+- A [transforms](https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api/) implementation
 
-  * An implementation of the Foundry `transforms` package that internally uses the `CachedFoundryClient`.
+  - An implementation of the Foundry `transforms` package that internally uses the `CachedFoundryClient`.
     This allows you to seamlessly run your Palantir Foundry Code Repository transforms code on your local machine.
-    Foundry DevTools does not cover all of Foundry's features, more on this [here](https://emdgroup.github.io/foundry-dev-tools/architecture.html#known-limitations).
+    Foundry DevTools does not cover all of Foundry's features, more on this [here](https://emdgroup.github.io/foundry-dev-tools/architecture.html#known-limitations-contributions-welcome).
 
-* [FoundryRestClient](https://emdgroup.github.io/foundry-dev-tools/FoundryRestClient_usage.html)
+- [FoundryRestClient](https://emdgroup.github.io/foundry-dev-tools/FoundryRestClient_usage.html)
 
-  * An API client that contains an opinionated client implementation to some of Foundry's APIs.
+  - An API client that contains an opinionated client implementation to some of Foundry's APIs.
 
-  * For example:
+  - For example:
 
     ```python
     from foundry_dev_tools import FoundryRestClient
 
     # Queries the Foundry SQL Server with spark SQL dialect
     rest_client = FoundryRestClient()
     df = rest_client.query_foundry_sql("SELECT * FROM `/Global/Foundry Training and Resources/Foundry Reference Project/Ontology Project: Aviation/airlines`", branch='master')
     df.shape
     # Out[2]: (17, 10)
     ```
 
-* [FoundryFileSystem](https://emdgroup.github.io/foundry-dev-tools/FoundryFileSystem_usage.html)
+- [FoundryFileSystem](https://emdgroup.github.io/foundry-dev-tools/FoundryFileSystem_usage.html)
 
-  * An implementation of `fsspec` for Foundry. Useful to interact with Foundry from popular data science libraries such as
-  `pandas` or `dask`.
+  - An implementation of `fsspec` for Foundry. Useful to interact with Foundry from popular data science libraries such as
+    `pandas` or `dask`.
 
-  * For example:
+  - For example:
 
     ```python
     import pandas as pd
     # /Global/Foundry Training and Resources/Foundry Reference Project/Ontology Project: Aviation/airlines
     df = pd.read_parquet("foundry://ri.foundry.main.dataset.5d78f3ae-a588-4fd8-9ba2-66827808c85f")
     df.shape
     # Out[2]: (17, 10)
     ```
 
-
 ## Quickstart
 
 With pip:
+
 ```shell
 pip install foundry-dev-tools
 ```
 
 With conda or mamba on the conda-forge channel:
+
 ```shell
 conda install -c conda-forge foundry-dev-tools
 ```
 
 [Further instructions](https://emdgroup.github.io/foundry-dev-tools/installation.html) can be found in our documentation.
 
 ## Why did we build this?
 
-* Local development experience in your favourite IDE (PyCharm, VSCode, ...)
-    * Access to modern developer tools and workflows such as pylint, black, isort, pre-commit hooks etc.
-* Quicker turnaround time when making changes
-    * Debug, change code and run in a matter of seconds instead of minutes
-* No accidental or auto commits
-    * Keep your git history clean
+- Local development experience in your favourite IDE (PyCharm, VSCode, ...)
+  - Access to modern developer tools and workflows such as pylint, black, isort, pre-commit hooks etc.
+- Quicker turnaround time when making changes
+  - Debug, change code and run in a matter of seconds instead of minutes
+- No accidental or auto commits
+  - Keep your git history clean
 
 # License
+
 Copyright (c) 2023 Merck KGaA, Darmstadt, Germany
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

#### html2text {}

```diff
@@ -18,44 +18,45 @@
                                      â¢ 
                                      Usage
                                      â¢ 
                                   Development
 # Foundry DevTools Seamlessly run your Palantir Foundry Repository transforms
 code and more on your local machine. Foundry DevTools is a set of useful
 libraries to interact with the Foundry APIs. There are currently three high
-level entrypoints to Foundry DevTools: * A [transforms](https://
+level entrypoints to Foundry DevTools: - A [transforms](https://
 www.palantir.com/docs/foundry/transforms-python/transforms-python-api/
-) implementation * An implementation of the Foundry `transforms` package that
+) implementation - An implementation of the Foundry `transforms` package that
 internally uses the `CachedFoundryClient`. This allows you to seamlessly run
 your Palantir Foundry Code Repository transforms code on your local machine.
 Foundry DevTools does not cover all of Foundry's features, more on this [here]
 (https://emdgroup.github.io/foundry-dev-tools/architecture.html#known-
-limitations). * [FoundryRestClient](https://emdgroup.github.io/foundry-dev-
-tools/FoundryRestClient_usage.html) * An API client that contains an
-opinionated client implementation to some of Foundry's APIs. * For example:
-```python from foundry_dev_tools import FoundryRestClient # Queries the Foundry
-SQL Server with spark SQL dialect rest_client = FoundryRestClient() df =
-rest_client.query_foundry_sql("SELECT * FROM `/Global/Foundry Training and
-Resources/Foundry Reference Project/Ontology Project: Aviation/airlines`",
-branch='master') df.shape # Out[2]: (17, 10) ``` * [FoundryFileSystem](https://
-emdgroup.github.io/foundry-dev-tools/FoundryFileSystem_usage.html) * An
-implementation of `fsspec` for Foundry. Useful to interact with Foundry from
-popular data science libraries such as `pandas` or `dask`. * For example:
-```python import pandas as pd # /Global/Foundry Training and Resources/Foundry
-Reference Project/Ontology Project: Aviation/airlines df = pd.read_parquet
-("foundry://ri.foundry.main.dataset.5d78f3ae-a588-4fd8-9ba2-66827808c85f")
-df.shape # Out[2]: (17, 10) ``` ## Quickstart With pip: ```shell pip install
-foundry-dev-tools ``` With conda or mamba on the conda-forge channel: ```shell
-conda install -c conda-forge foundry-dev-tools ``` [Further instructions]
-(https://emdgroup.github.io/foundry-dev-tools/installation.html) can be found
-in our documentation. ## Why did we build this? * Local development experience
-in your favourite IDE (PyCharm, VSCode, ...) * Access to modern developer tools
-and workflows such as pylint, black, isort, pre-commit hooks etc. * Quicker
-turnaround time when making changes * Debug, change code and run in a matter of
-seconds instead of minutes * No accidental or auto commits * Keep your git
+limitations-contributions-welcome). - [FoundryRestClient](https://
+emdgroup.github.io/foundry-dev-tools/FoundryRestClient_usage.html) - An API
+client that contains an opinionated client implementation to some of Foundry's
+APIs. - For example: ```python from foundry_dev_tools import FoundryRestClient
+# Queries the Foundry SQL Server with spark SQL dialect rest_client =
+FoundryRestClient() df = rest_client.query_foundry_sql("SELECT * FROM `/Global/
+Foundry Training and Resources/Foundry Reference Project/Ontology Project:
+Aviation/airlines`", branch='master') df.shape # Out[2]: (17, 10) ``` -
+[FoundryFileSystem](https://emdgroup.github.io/foundry-dev-tools/
+FoundryFileSystem_usage.html) - An implementation of `fsspec` for Foundry.
+Useful to interact with Foundry from popular data science libraries such as
+`pandas` or `dask`. - For example: ```python import pandas as pd # /Global/
+Foundry Training and Resources/Foundry Reference Project/Ontology Project:
+Aviation/airlines df = pd.read_parquet("foundry://
+ri.foundry.main.dataset.5d78f3ae-a588-4fd8-9ba2-66827808c85f") df.shape # Out
+[2]: (17, 10) ``` ## Quickstart With pip: ```shell pip install foundry-dev-
+tools ``` With conda or mamba on the conda-forge channel: ```shell conda
+install -c conda-forge foundry-dev-tools ``` [Further instructions](https://
+emdgroup.github.io/foundry-dev-tools/installation.html) can be found in our
+documentation. ## Why did we build this? - Local development experience in your
+favourite IDE (PyCharm, VSCode, ...) - Access to modern developer tools and
+workflows such as pylint, black, isort, pre-commit hooks etc. - Quicker
+turnaround time when making changes - Debug, change code and run in a matter of
+seconds instead of minutes - No accidental or auto commits - Keep your git
 history clean # License Copyright (c) 2023 Merck KGaA, Darmstadt, Germany
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use
 this file except in compliance with the License. You may obtain a copy of the
 License at https://www.apache.org/licenses/LICENSE-2.0 Unless required by
 applicable law or agreed to in writing, software distributed under the License
 is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied. See the License for the specific language
```

### Comparing `foundry-dev-tools-1.0.9/docs/Configuration_usage.md` & `foundry-dev-tools-1.1/docs/Configuration_usage.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # Configuration
 
-By default, the code loads the configuration from the `~/.foundry-dev-tools/config` file.  
-If a project [specific config file](#Project-specific-configuration) exists in `your-project-dir/.foundry_dev_tools`, it takes precedence.  
+By default, the code loads the configuration from the '~/.foundry-dev-tools/config' file.  
+If a project [specific config file](#project-specific-configuration) exists in `your-project-dir/.foundry_dev_tools`, it takes precedence.  
 If a environment variable like `FOUNDRY_DEV_TOOLS_config_key` exists, `config_key` gets overwritten by this environment variable.  
-Afterwards, the logic falls back to a default value: ( overwrites > environment variable > project config file > config file > default)  
+Afterwards, the logic falls back to a default value: ( overwrites > environment variable > project config file > config file > default)
 
 In the standard setup, the configuration should contain either the Foundry Token (`jwt`) or the Foundry Client
 ID (`client_id`) for SSO.
 
 ## Configuration options
 
-| Name                                   | Description                                                                                                                                       | Values                                 | 
-|----------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------|
+| Name                                   | Description                                                                                                                                       | Values                                 |
+| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------- |
 | foundry_url                            | Url of the foundry instance.                                                                                                                      | e.g. https://foundry.example.com       |
 | jwt                                    | The Bearer Token copied from the Foundry Token Page                                                                                               | eyJhb...                               |
 | client_id                              | The client_id of the Foundry Third Party application for SSO Authentication.                                                                      | ...                                    |
 | client_secret                          | The client_secret of the Foundry Third Party application.                                                                                         | ...                                    |
 | grant_type                             | Set this to client_credentials if you use Foundry Third Party application client_credentials flow. Default is authorization_code                  | authorization_code, client_credentials |
 | requests_ca_bundle                     | Path to custom ca bundle file, useful in corporate networks with SSL inspection                                                                   | not set                                |
-| transforms_sql_sample_row_limit        | Number of rows that are retrieved for each dataset when sql is used                                                                               | 5000                                   | 
-| transforms_sql_dataset_size_threshold  | Maximal size of a dataset up to which file gets downloaded. If dataset is larger, sql with limit query will be used to download a partial dataset | 500                                    | 
+| transforms_sql_sample_row_limit        | Number of rows that are retrieved for each dataset when sql is used                                                                               | 5000                                   |
+| transforms_sql_dataset_size_threshold  | Maximal size of a dataset up to which file gets downloaded. If dataset is larger, sql with limit query will be used to download a partial dataset | 500                                    |
 | transforms_sql_sample_select_random    | True or False, if data is randomly sampled when SQL mode is used (query takes more time)                                                          | True or False                          |
 | transforms_force_full_dataset_download | if file_download is True, all files of datasets are downloaded                                                                                    | True or False                          |
 | cache_dir                              | Point cache directory to other directory than default                                                                                             | ~/.foundry-dev-tools/cache             |
 | transforms_freeze_cache                | Uses offline cache as is; no Foundry connection needed                                                                                            | True or False (default: False)         |
 | transforms_output_folder               | When @transform in combination with TransformOutput.filesystem() is used, files are written to this folder.                                       | /projectA/local_files                  |
 | enable_runtime_token_providers         | Enables the token providers, Default is True                                                                                                      | True or False                          |
```

### Comparing `foundry-dev-tools-1.0.9/docs/FoundryFileSystem_usage.md` & `foundry-dev-tools-1.1/docs/FoundryFileSystem_usage.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # Foundry DevTools fsspec implementation
 
 ## In combination with fsspec:
+
 ```pycon
 >>> import fsspec
 >>> dataset_rid = 'ri.foundry.main.dataset.15461bb5-be92-4ad9-aa3e-07c16175e713'
 >>> with fsspec.open(f"foundry://{dataset_rid}/test.txt", "r") as f:
 >>>    print(f.read())
 >>> 'content'
 ```
 
 ## Use in combination with pandas:
+
 ```pycon
 >>> import pandas as pd
 >>> df = pd.read_csv(f"foundry://{dataset_rid}/test1.csv")
 >>> df.shape
 (1, 1)
 ```
```

### Comparing `foundry-dev-tools-1.0.9/docs/FoundryRestClient_usage.md` & `foundry-dev-tools-1.1/docs/FoundryRestClient_usage.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 transaction_rid = rest_client.open_transaction(dataset_rid=dataset_rid,
                                                mode='UPDATE',
                                                branch='master')
 rest_client.upload_dataset_files(dataset_rid=dataset_rid,
                                  transaction_rid=transaction_rid,
                                  path_file_dict=path_file_dict)
 rest_client.commit_transaction(dataset_rid, transaction_rid)
-````
+```
 
 ### Save model or other type of file
 
 ```python
 from foundry_dev_tools import CachedFoundryClient
 import pickle
 
@@ -120,23 +120,24 @@
 df = cached_client.load_dataset('/path/to/test_dataset', branch='master')
 df.toPandas().to_string()
 ```
 
 ### Download only few files from dataset
 
 You can simply specify the list of files you want to download in download_dataset_files
+
 ```python
 rid = "ri.foundry.main.dataset.xxxxxxx-xxxx-xxx-xxx-xxxxxxxxx"
 rest_client.download_dataset_files(dataset_rid=rid, output_directory='/paht/to/only_few_files', files=['file1.png', 'file2.png'], branch='master')
 ```
 
 [Third Party Application in Foundry]: https://www.palantir.com/docs/foundry/platform-security-third-party/third-party-apps-overview/
 
+### Polars DataFrame from Spark SQL dialect
 
-### Polars DataFrame from Spark SQL dialect 
 Queries the Foundry SQL server with Spark SQL dialect, load arrow stream using [polars](https://www.pola.rs/).
 
 ```python
 from foundry_dev_tools import FoundryRestClient
 
 rest_client = FoundryRestClient()
 arrow_table = rest_client.query_foundry_sql(
@@ -146,15 +147,16 @@
 )
 import polars as pl
 
 df = pl.from_arrow(arrow_table)
 print(df)
 ```
 
-### DuckDB Table from Spark SQL dialect 
+### DuckDB Table from Spark SQL dialect
+
 Queries the Foundry SQL server with Spark SQL dialect, load arrow stream using [duckdb](https://duckdb.org/).
 
 ```python
 from foundry_dev_tools import FoundryRestClient
 
 rest_client = FoundryRestClient()
 arrow_table = rest_client.query_foundry_sql(
@@ -164,8 +166,8 @@
 )
 import duckdb
 
 # Get an in-memory DuckDB database and create a new table from the result arrow table.
 # Note that the python variable is automatically determined from the query string.
 con = duckdb.connect()
 con.execute("CREATE TABLE my_table AS SELECT * FROM arrow_table")
-```
+```
```

### Comparing `foundry-dev-tools-1.0.9/docs/SSO_usage.md` & `foundry-dev-tools-1.1/docs/SSO_usage.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,13 +22,14 @@
 from foundry_dev_tools import FoundryRestClient
 
 rest_client = FoundryRestClient()
 rest_client.get_user_info()
 ```
 
 Steps:
+
 1. Execute the above lines - a message with a URL will appear - visit this URL in your browser
-2. Once opened, log in to Foundry (if necessary) using your account and allow  application
+2. Once opened, log in to Foundry (if necessary) using your account and allow application
 3. Copy the authorization code to the prompt of your Python commands and press Enter
 
 The result of `get_user_info()` should appear, showing your Foundry user information.
 At this point your temporary credentials are stored locally and will be used for future calls to Foundry.
```

### Comparing `foundry-dev-tools-1.0.9/docs/architecture.md` & `foundry-dev-tools-1.1/docs/architecture.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # Architecture
 
 ## How the transforms library that exists on Foundry is stubbed in Foundry DevTools
 
-* Input datasets < 500MB are retrieved with the Foundry Dataproxy File Download API
-* Input datasets > 500MB are retrieved as partial subsets with the Foundry Dataproxy SQL API (SELECT * FROM .. LIMIT
-  
-* Both of these limits can be changed with the corresponding config option
-  * `transforms_sql_dataset_size_threshold` size in MB, default 500
-  * `transforms_sql_sample_row_limit`, default 5000
-* Datasets are cached locally in a folder (`~/.foundry-dev-tools/.cache`)
-* Datasets are automatically passed to transform functions
-* Output datasets can be visualized using IDE or Notebook functionality
-* Output dataset files can be stored to a local folder for inspection
-* Foundry `transforms` library is stubbed
-* Dataset branch is detected automatically from the local git branch
+- Input datasets < 500MB are retrieved with the Foundry Dataproxy File Download API
+- Input datasets > 500MB are retrieved as partial subsets with the Foundry Dataproxy SQL API (SELECT \* FROM .. LIMIT
+- Both of these limits can be changed with the corresponding config option
+  - `transforms_sql_dataset_size_threshold` size in MB, default 500
+  - `transforms_sql_sample_row_limit`, default 5000
+- Datasets are cached locally in a folder (`~/.foundry-dev-tools/.cache`)
+- Datasets are automatically passed to transform functions
+- Output datasets can be visualized using IDE or Notebook functionality
+- Output dataset files can be stored to a local folder for inspection
+- Foundry `transforms` library is stubbed
+- Dataset branch is detected automatically from the local git branch
 
-
-The following sequence diagrams show  
+The following sequence diagrams show
 
 a) what happens when the `Input` dataset is already cached.
+
 ```{image} pictures/mermaid-diagram-already-cached-light.svg
 ---
 class: only-light
 ---
 ```
+
 ```{image} pictures/mermaid-diagram-already-cached-dark.svg
 ---
 class: only-dark
 ---
-```  
+```
 
-b) what happens when the `Input` dataset has a new transaction  
+b) what happens when the `Input` dataset has a new transaction
 
 ```{image} pictures/mermaid-diagram-new-transaction-light.svg
 ---
 class: only-light
 ---
 ```
+
 ```{image} pictures/mermaid-diagram-new-transaction-dark.svg
 ---
 class: only-dark
 ---
 ```
 
-
 ### Known limitations (Contributions Welcome 🤗)
 
-* CSV format settings are not taken over from the Foundry Schema. Advised to use datasets in parquet format.
-* transforms Output not written back to foundry
-* @incremental not implemented
-* @configure not implemented
+- CSV format settings are not taken over from the Foundry Schema. Advised to use datasets in parquet format.
+- transforms Output not written back to foundry
+- @incremental not implemented
+- @configure not implemented
```

### Comparing `foundry-dev-tools-1.0.9/docs/changelog.md` & `foundry-dev-tools-1.1/docs/changelog.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,50 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog],
 and this project adheres to [Semantic Versioning].
 
+## [1.1] - 2023-06-12
+
+### Added
+
+- foundry-dev-tools build CLI (#22) (#23)
+
+## [1.0.12] - 2023-06-01
+
+### Added
+- SQLReturnType enum (#21)
+
+### Changed
+- move to arrow_v1 for sql queries (#21)
+
+### Removed
+- FoundrySQLClient (#21)
+
+## [1.0.11] - 2023-05-23
+
+### Changed
+- better SQL exceptions (#20)
+
+### Fixed
+- pip installation documentation for zsh users (#19)
+
+## [1.0.10] - 2023-05-16
+
+### Changed
+
+- use ruff and black instead of pylint and ufmt (#15)
+- converted the subprocess calls with git to python only imitations (#15)
+
+### Fixed
+
+- environment variables didn't take precedence (#15)
+
 ## [1.0.9] - 2023-04-27
 
 ### Fixed
 
 - file upload for files greater than 2GB (#16)
 
 ## [1.0.8] - 2023-04-17
@@ -22,15 +58,14 @@
 
 - typo in docs (#12)
 
 ### Removed
 
 - pandas<2 restriction, as pyspark 3.4 supports it (#13)
 
-
 ## [1.0.7] - 2023-04-05
 
 ### Added
 
 - skip_instance_cache kwarg to FoundryFileSystem, which gets passed to fsspec
   it should be set to True in a multithreaded environment (e.g. Streamlit),
   as the same filesystem instance gets reused by default,
@@ -98,14 +133,18 @@
 
 ## [1.0] - 2023-02-28 [YANKED]
 
 - First public Open Source Release of Foundry DevTools.
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/spec/v2.0.0.html
+[1.1]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.12...v1.1
+[1.0.12]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.11...v1.0.12
+[1.0.11]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.10...v1.0.11
+[1.0.10]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.9...v1.0.10
 [1.0.9]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.8...v1.0.9
 [1.0.8]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.7...v1.0.8
 [1.0.7]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.6...v1.0.7
 [1.0.6]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.5...v1.0.6
 [1.0.5]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.4...v1.0.5
 [1.0.4]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.3...v1.0.4
 [1.0.3]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.2...v1.0.3
```

### Comparing `foundry-dev-tools-1.0.9/docs/conf.py` & `foundry-dev-tools-1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,25 +38,26 @@
 transforms_module_dir = os.path.join(__location__, "../src/transforms")
 try:
     shutil.rmtree(output_dir)
 except FileNotFoundError:
     pass
 
 try:
-    import sphinx
-
     args = ["--implicit-namespaces", "-M", "-T", "-f", "-o", output_dir]
 
     apidoc.main(
-        args
-        + [foundry_dev_tools_module_dir, foundry_dev_tools_module_dir + "/__init__.py"]
+        [
+            *args,
+            foundry_dev_tools_module_dir,
+            foundry_dev_tools_module_dir + "/__init__.py",
+        ]
     )
-    apidoc.main(args + [transforms_module_dir])
+    apidoc.main([*args, transforms_module_dir])
 except Exception as e:
-    print("Running `sphinx-apidoc` failed!\n{}".format(e))
+    print(f"Running `sphinx-apidoc` failed!\n{e}")
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
@@ -112,15 +113,15 @@
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # version: The short X.Y version.
 # release: The full version, including alpha/beta/rc tags.
-# If you don’t need the separation provided between version and release,
+# If you don`t need the separation provided between version and release,
 # just set them both to the same value.
 try:
     from foundry_dev_tools import __version__ as version
 except ImportError:
     version = ""
 
 if not version or version.lower() == "unknown":
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `foundry-dev-tools-1.0.9/docs/develop.md` & `foundry-dev-tools-1.1/docs/develop.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Every change you make in the code is instantly applied.
 
 ## Run unit tests
 
 Install the test dependencies and execute pytest.
 
 ```shell
-pip install -e .[testing] 
+pip install -e ".[testing,transforms]"
 pytest
 ```
 
 or use [tox]
 
 ```shell
 tox
@@ -33,35 +33,28 @@
 
 To run the integration tests, make sure to have a valid `config` file in your `~/.foundry_dev_tools/` folder
 and have the environment variables `INTEGRATION_TEST_COMPASS_ROOT_PATH` and `INTEGRATION_TEST_COMPASS_ROOT_RID` set.
 These environment variables should point to an empty folder on palantir foundry you have permissions to,
 the tests will create the datasets automatically.
 
 ```shell
-pip install -e [integration-testing]
+pip install -e ".[integration,testing,transforms]"
 pytest --integration
 ```
 
 or use [tox]
-```shell
-tox -- --integration
-```
-
-## Run pylint
-
-To run [pylint] locally, execute the following code:
 
 ```shell
-pylint src
+tox -- --integration
 ```
 
 ## Pre-Commit hooks & formatting
 
 To format the code and make it ready for a commit we use pre-commit.
-Currently, we run [ufmt] which uses black and usort, [pylint] and force the line endings to linux/mac ones.
+Currently, we run [black], [ruff] and force the line endings to linux/mac ones.
 After a commit gets pushed it will automatically check if it is correctly formatted.
 If not, the checks will fail, and we will not be able to merge your changes.
 
 To set up [pre-commit] hooks run:
 
 ```shell
 # after this everytime you commit in this repo, it will run the hooks
@@ -74,16 +67,17 @@
 
 ```shell
 pre-commit run --all-files
 ```
 
 To check if it is correctly formatted according
 to the pre-commit hooks, we run in our pipeline:
+
 ```shell
 tox -e lint
 ```
 
 [pyscaffold]: https://pyscaffold.org/en/stable/
 [tox]: https://tox.wiki/en/latest/
 [pre-commit]: https://pre-commit.com/
-[ufmt]: https://github.com/omnilib/ufmt
-[pylint]: https://github.com/PyCQA/pylint
+[black]: https://github.com/psf/black
+[ruff]: https://github.com/charliermarsh/ruff
```

### Comparing `foundry-dev-tools-1.0.9/docs/index.md` & `foundry-dev-tools-1.1/docs/index.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 00000000: 6060 607b 696e 636c 7564 657d 202e 2e2f  ```{include} ../
 00000010: 5245 4144 4d45 2e6d 640a 3a72 656c 6174  README.md.:relat
 00000020: 6976 652d 646f 6373 3a20 646f 6373 2f0a  ive-docs: docs/.
 00000030: 3a72 656c 6174 6976 652d 696d 6167 6573  :relative-images
-00000040: 3a0a 6060 600a 0a0a 2323 2043 6f6e 7465  :.```...## Conte
-00000050: 6e74 730a 0a60 6060 7b74 6f63 7472 6565  nts..```{toctree
-00000060: 7d0a 3a6d 6178 6465 7074 683a 2032 0a3a  }.:maxdepth: 2.:
-00000070: 6361 7074 696f 6e3a 2043 6f6e 7465 6e74  caption: Content
-00000080: 730a 0a4f 7665 7276 6965 7720 3c73 656c  s..Overview <sel
-00000090: 663e 0a49 6e73 7461 6c6c 6174 696f 6e20  f>.Installation 
-000000a0: 3c69 6e73 7461 6c6c 6174 696f 6e3e 0a55  <installation>.U
-000000b0: 7361 6765 2061 6e64 2045 7861 6d70 6c65  sage and Example
-000000c0: 7320 3c75 7361 6765 5f61 6e64 5f65 7861  s <usage_and_exa
-000000d0: 6d70 6c65 733e 0a44 6576 656c 6f70 6d65  mples>.Developme
-000000e0: 6e74 203c 6465 7665 6c6f 703e 0a41 7263  nt <develop>.Arc
-000000f0: 6869 7465 6374 7572 6520 3c61 7263 6869  hitecture <archi
-00000100: 7465 6374 7572 653e 0a4c 6963 656e 7365  tecture>.License
-00000110: 203c 6c69 6365 6e73 653e 0a43 6f6e 7472   <license>.Contr
-00000120: 6962 7574 6f72 7320 3c63 6f6e 7472 6962  ibutors <contrib
-00000130: 7574 6f72 733e 0a43 6861 6e67 656c 6f67  utors>.Changelog
-00000140: 203c 6368 616e 6765 6c6f 673e 0a60 6060   <changelog>.```
-00000150: 0a0a 2320 5265 6665 7265 6e63 650a 6060  ..# Reference.``
-00000160: 607b 746f 6374 7265 657d 0a3a 6d61 7864  `{toctree}.:maxd
-00000170: 6570 7468 3a20 320a 3a74 6974 6c65 736f  epth: 2.:titleso
-00000180: 6e6c 793a 0a3a 6361 7074 696f 6e3a 2052  nly:.:caption: R
-00000190: 6566 6572 656e 6365 0a0a 666f 756e 6472  eference..foundr
-000001a0: 792d 6465 762d 746f 6f6c 7320 7265 6665  y-dev-tools refe
-000001b0: 7265 6e63 6520 3c61 7069 2f66 6f75 6e64  rence <api/found
-000001c0: 7279 5f64 6576 5f74 6f6f 6c73 3e0a 7472  ry_dev_tools>.tr
-000001d0: 616e 7366 6f72 6d73 2072 6566 6572 656e  ansforms referen
-000001e0: 6365 203c 6170 692f 7472 616e 7366 6f72  ce <api/transfor
-000001f0: 6d73 3e0a 0a60 6060 0a0a 2323 2049 6e64  ms>..```..## Ind
-00000200: 6963 6573 2061 6e64 2074 6162 6c65 730a  ices and tables.
-00000210: 0a2a 207b 7265 667d 6067 656e 696e 6465  .* {ref}`geninde
-00000220: 7860 0a2a 207b 7265 667d 606d 6f64 696e  x`.* {ref}`modin
-00000230: 6465 7860 0a2a 207b 7265 667d 6073 6561  dex`.* {ref}`sea
-00000240: 7263 6860 0a0a 5b53 7068 696e 785d 3a20  rch`..[Sphinx]: 
-00000250: 6874 7470 3a2f 2f77 7777 2e73 7068 696e  http://www.sphin
-00000260: 782d 646f 632e 6f72 672f 0a5b 4d61 726b  x-doc.org/.[Mark
-00000270: 646f 776e 5d3a 2068 7474 7073 3a2f 2f64  down]: https://d
-00000280: 6172 696e 6766 6972 6562 616c 6c2e 6e65  aringfireball.ne
-00000290: 742f 7072 6f6a 6563 7473 2f6d 6172 6b64  t/projects/markd
-000002a0: 6f77 6e2f 0a5b 7265 5374 7275 6374 7572  own/.[reStructur
-000002b0: 6564 5465 7874 5d3a 2068 7474 703a 2f2f  edText]: http://
-000002c0: 7777 772e 7370 6869 6e78 2d64 6f63 2e6f  www.sphinx-doc.o
-000002d0: 7267 2f65 6e2f 6d61 7374 6572 2f75 7361  rg/en/master/usa
-000002e0: 6765 2f72 6573 7472 7563 7475 7265 6474  ge/restructuredt
-000002f0: 6578 742f 6261 7369 6373 2e68 746d 6c0a  ext/basics.html.
-00000300: 5b4d 7953 545d 3a20 6874 7470 733a 2f2f  [MyST]: https://
-00000310: 6d79 7374 2d70 6172 7365 722e 7265 6164  myst-parser.read
-00000320: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00000330: 7465 7374 2f0a                           test/.
+00000040: 3a0a 6060 600a 0a23 2320 436f 6e74 656e  :.```..## Conten
+00000050: 7473 0a0a 6060 607b 746f 6374 7265 657d  ts..```{toctree}
+00000060: 0a3a 6d61 7864 6570 7468 3a20 320a 3a63  .:maxdepth: 2.:c
+00000070: 6170 7469 6f6e 3a20 436f 6e74 656e 7473  aption: Contents
+00000080: 0a0a 4f76 6572 7669 6577 203c 7365 6c66  ..Overview <self
+00000090: 3e0a 496e 7374 616c 6c61 7469 6f6e 203c  >.Installation <
+000000a0: 696e 7374 616c 6c61 7469 6f6e 3e0a 5573  installation>.Us
+000000b0: 6167 6520 616e 6420 4578 616d 706c 6573  age and Examples
+000000c0: 203c 7573 6167 655f 616e 645f 6578 616d   <usage_and_exam
+000000d0: 706c 6573 3e0a 434c 4920 3c63 6c69 3e0a  ples>.CLI <cli>.
+000000e0: 4465 7665 6c6f 706d 656e 7420 3c64 6576  Development <dev
+000000f0: 656c 6f70 3e0a 4172 6368 6974 6563 7475  elop>.Architectu
+00000100: 7265 203c 6172 6368 6974 6563 7475 7265  re <architecture
+00000110: 3e0a 4c69 6365 6e73 6520 3c6c 6963 656e  >.License <licen
+00000120: 7365 3e0a 436f 6e74 7269 6275 746f 7273  se>.Contributors
+00000130: 203c 636f 6e74 7269 6275 746f 7273 3e0a   <contributors>.
+00000140: 4368 616e 6765 6c6f 6720 3c63 6861 6e67  Changelog <chang
+00000150: 656c 6f67 3e0a 6060 600a 0a23 2052 6566  elog>.```..# Ref
+00000160: 6572 656e 6365 0a0a 6060 607b 746f 6374  erence..```{toct
+00000170: 7265 657d 0a3a 6d61 7864 6570 7468 3a20  ree}.:maxdepth: 
+00000180: 320a 3a74 6974 6c65 736f 6e6c 793a 0a3a  2.:titlesonly:.:
+00000190: 6361 7074 696f 6e3a 2052 6566 6572 656e  caption: Referen
+000001a0: 6365 0a0a 666f 756e 6472 792d 6465 762d  ce..foundry-dev-
+000001b0: 746f 6f6c 7320 7265 6665 7265 6e63 6520  tools reference 
+000001c0: 3c61 7069 2f66 6f75 6e64 7279 5f64 6576  <api/foundry_dev
+000001d0: 5f74 6f6f 6c73 3e0a 7472 616e 7366 6f72  _tools>.transfor
+000001e0: 6d73 2072 6566 6572 656e 6365 203c 6170  ms reference <ap
+000001f0: 692f 7472 616e 7366 6f72 6d73 3e0a 0a60  i/transforms>..`
+00000200: 6060 0a0a 2323 2049 6e64 6963 6573 2061  ``..## Indices a
+00000210: 6e64 2074 6162 6c65 730a 0a2d 207b 7265  nd tables..- {re
+00000220: 667d 6067 656e 696e 6465 7860 0a2d 207b  f}`genindex`.- {
+00000230: 7265 667d 606d 6f64 696e 6465 7860 0a2d  ref}`modindex`.-
+00000240: 207b 7265 667d 6073 6561 7263 6860 0a0a   {ref}`search`..
+00000250: 5b53 7068 696e 785d 3a20 6874 7470 3a2f  [Sphinx]: http:/
+00000260: 2f77 7777 2e73 7068 696e 782d 646f 632e  /www.sphinx-doc.
+00000270: 6f72 672f 0a5b 4d61 726b 646f 776e 5d3a  org/.[Markdown]:
+00000280: 2068 7474 7073 3a2f 2f64 6172 696e 6766   https://daringf
+00000290: 6972 6562 616c 6c2e 6e65 742f 7072 6f6a  ireball.net/proj
+000002a0: 6563 7473 2f6d 6172 6b64 6f77 6e2f 0a5b  ects/markdown/.[
+000002b0: 7265 5374 7275 6374 7572 6564 5465 7874  reStructuredText
+000002c0: 5d3a 2068 7474 703a 2f2f 7777 772e 7370  ]: http://www.sp
+000002d0: 6869 6e78 2d64 6f63 2e6f 7267 2f65 6e2f  hinx-doc.org/en/
+000002e0: 6d61 7374 6572 2f75 7361 6765 2f72 6573  master/usage/res
+000002f0: 7472 7563 7475 7265 6474 6578 742f 6261  tructuredtext/ba
+00000300: 7369 6373 2e68 746d 6c0a 5b4d 7953 545d  sics.html.[MyST]
+00000310: 3a20 6874 7470 733a 2f2f 6d79 7374 2d70  : https://myst-p
+00000320: 6172 7365 722e 7265 6164 7468 6564 6f63  arser.readthedoc
+00000330: 732e 696f 2f65 6e2f 6c61 7465 7374 2f0a  s.io/en/latest/.
```

### Comparing `foundry-dev-tools-1.0.9/docs/installation.md` & `foundry-dev-tools-1.1/docs/installation.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Installation
 
 ## Prerequisites
 
-* Python >=3.8
-* Git
-* Apache Spark (optional)
+- Python >=3.8
+- Git
+- Apache Spark (optional)
 
 ## Get the Foundry JSON Web Token
 
 Go to https://\<foundrystack\>/workspace/settings/tokens and generate a new token.
 Copy it for later use in the config.
 
 ## Create Basic Config File
@@ -30,19 +30,21 @@
 
 ## Install the latest version of Foundry DevTools
 
 We recommend using a new [conda environment] or [python environment],
 after you activated it, just run:
 
 With pip:
+
 ```shell
 pip install foundry-dev-tools
 ```
 
 With conda or mamba on the conda-forge channel:
+
 ```shell
 conda install -c conda-forge foundry-dev-tools
 ```
 
 or, if you have the repository locally available and want to tinker with the source code
 you could install it in "editable"/"develop mode". Run the following command in
 the Foundry DevTools root directory:
@@ -52,20 +54,20 @@
 ```
 
 ## PySpark
 
 The python package [PySpark](https://pypi.org/project/pyspark/) is an optional dependency of Foundry DevTools.
 It is required to run `transforms` and the `CachedFoundryClient`, the PySpark version needs to be at least 3.0.
 
-If you install `foundry-dev-tools[tranforms]`, it will install pyspark as well:
+If you use `foundry-dev-tools[transforms]` to install, it will install the pyspark dependency as well:
 
 ```bash
-pip install foundry-dev-tools[transforms]
+pip install 'foundry-dev-tools[transforms]'
 ```
 
 Alternative installation methods, or more information on how to get Spark running,
 can be found in the [PySpark Documenation] and the [Spark Documentation].
 
 [PySpark Documentation]: https://spark.apache.org/docs/latest/api/python/getting_started/install.html
 [Spark Documentation]: https://spark.apache.org/docs/latest/
 [conda environment]: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html
-[python environment]: https://docs.python.org/3/library/venv.html
+[python environment]: https://docs.python.org/3/library/venv.html
```

### Comparing `foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-already-cached-dark.svg` & `foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-already-cached-dark.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-already-cached-light.svg` & `foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-already-cached-light.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-new-transaction-dark.svg` & `foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-new-transaction-dark.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-new-transaction-light.svg` & `foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-new-transaction-light.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/docs/pictures/tpa_config.png` & `foundry-dev-tools-1.1/docs/pictures/tpa_config.png`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/docs/usage_and_examples.md` & `foundry-dev-tools-1.1/docs/usage_and_examples.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 After adding this, you just need to run the file.
 
 #### Using Foundry DevTools inside a Jupyter Notebook
 
 You can run your transform code from jupyter with very minimal, non-breaking changes to your repository.
 
-Open the `transforms-python/src/setup.py` file of your repository and change line 8 and 9 by adding a default value 
+Open the `transforms-python/src/setup.py` file of your repository and change line 8 and 9 by adding a default value
 for package name and package version:
 
 ```diff
 -      name=os.environ['PKG_NAME'],
 +      name=os.getenv('PKG_NAME', 'your-package-name'),
 -      version=os.environ['PKG_VERSION'],
 +      version=os.getenv('PKG_VERSION', 'your-package-version'),
@@ -68,16 +68,15 @@
 
 # run the function by calling compute
 output = apply_the_schema.compute()
 # output in pandas format
 output.toPandas()
 ```
 
-
 ## More specific Foundry DevTools usage
 
 ```{toctree}
 The FoundryRestClient <FoundryRestClient_usage>
 The fsspec implementation <FoundryFileSystem_usage>
 Configuration <Configuration_usage>
 SSO <SSO_usage>
-```
+```
```

### Comparing `foundry-dev-tools-1.0.9/setup.py` & `foundry-dev-tools-1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""
-    Setup file for Foundry DevTools.
-    Use setup.cfg to configure your project.
+"""Setup file for Foundry DevTools.
+
+Use setup.cfg to configure your project.
 
-    This file was generated with PyScaffold 4.4.
-    PyScaffold helps you to put up the scaffold of your new Python project.
-    Learn more under: https://pyscaffold.org/
+This file was generated with PyScaffold 4.4.
+PyScaffold helps you to put up the scaffold of your new Python project.
+Learn more under: https://pyscaffold.org/
 """
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
         setup(use_scm_version={"version_scheme": "no-guess-dev"})
-    except:  # noqa
+    except:
         print(
             "\n\nAn error occurred while building the project, "
             "please ensure you have the most updated version of setuptools, "
             "setuptools_scm and wheel with:\n"
             "   pip install -U setuptools setuptools_scm wheel\n\n"
         )
         raise
```

### Comparing `foundry-dev-tools-1.0.9/src/foundry_dev_tools/cached_foundry_client.py` & `foundry-dev-tools-1.1/src/foundry_dev_tools/cached_foundry_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 """Cached Foundry Client, high level client to work with Foundry."""
 import logging
 import os
 import pickle
 import tempfile
 import time
-from typing import Tuple, Union
+from pathlib import Path
+from typing import TYPE_CHECKING
 
-import foundry_dev_tools
+import foundry_dev_tools.config
 from foundry_dev_tools.foundry_api_client import (
     BranchNotFoundError,
     DatasetHasNoSchemaError,
     DatasetNotFoundError,
+    FoundryRestClient,
 )
 from foundry_dev_tools.utils.caches.spark_caches import DiskPersistenceBackedSparkCache
 from foundry_dev_tools.utils.converter.foundry_spark import (
     infer_dataset_format_from_foundry_schema,
 )
 
-from .foundry_api_client import FoundryRestClient
-
 LOGGER = logging.getLogger(__name__)
 
+if TYPE_CHECKING:
+    import pandas as pd
+    import pyspark.sql
+
 
 class CachedFoundryClient:
     """A Foundry Client that offers a high level API to Foundry.
 
     Methods to save, load datasets are implemented.
     """
 
-    def __init__(self, config: dict = None):
+    def __init__(self, config: "dict | None" = None):
         """Initialize `CachedFoundryClient`.
 
         Possible to pass overwrite config and
         uses `Configuration` to read it from the
         ~/.foundry-dev-tools/config file.
 
         Args:
             config (dict): config dict to overwrite values from config file
         """
         self.overwrite_config = config
-        self.config = foundry_dev_tools.Configuration.get_config(self.overwrite_config)
+        self.config = foundry_dev_tools.config.Configuration.get_config(
+            self.overwrite_config
+        )
         self.cache = DiskPersistenceBackedSparkCache(**self.config)
 
     @property
     def api(self) -> FoundryRestClient:
         """We are creating a new instance of the client everytime it is used.
 
         Because it might be used in a request or session context in the AppService where
@@ -72,15 +78,15 @@
 
         """
         _, dataset_identity = self.fetch_dataset(dataset_path_or_rid, branch)
         return self.cache[dataset_identity]
 
     def fetch_dataset(
         self, dataset_path_or_rid: str, branch: str = "master"
-    ) -> Tuple[str, dict]:
+    ) -> "tuple[str, dict]":
         """Downloads complete dataset from Foundry and stores in cache.
 
         Returns local path to dataset
 
         Args:
             dataset_path_or_rid (str): Path to dataset or the rid of the dataset
             branch (str): The branch of the dataset
@@ -129,24 +135,22 @@
         # even though the branch might be different to that requested.
         return self.cache.get_dataset_identity_not_branch_aware(dataset_path_or_rid)
 
     def _return_local_path_of_cached_dataset(self, dataset_identity, branch) -> str:
         LOGGER.debug(
             "Returning data for %s on branch %s from cache", dataset_identity, branch
         )
-        path = self.cache.get_path_to_local_dataset(dataset_identity)
-        return path
+        return self.cache.get_path_to_local_dataset(dataset_identity)
 
     def _download_dataset_and_return_local_path(
         self, dataset_identity, branch, foundry_schema
     ) -> str:
         LOGGER.debug("Caching data for %s on branch %s", dataset_identity, branch)
         self._download_dataset_to_cache_dir(dataset_identity, branch, foundry_schema)
-        path = self.cache.get_path_to_local_dataset(dataset_identity)
-        return path
+        return self.cache.get_path_to_local_dataset(dataset_identity)
 
     def _download_dataset_to_cache_dir(self, dataset_identity, branch, foundry_schema):
         list_of_files = self.api.list_dataset_files(
             dataset_identity["dataset_rid"], exclude_hidden_files=True, view=branch
         )
         params = {
             "dataset_rid": dataset_identity["dataset_rid"],
@@ -169,21 +173,20 @@
         )
         params["output_directory"] = path
         self.api.download_dataset_files(**params)
         self.cache.set_item_metadata(path, dataset_identity, foundry_schema)
 
     def save_dataset(
         self,
-        df: Union["pd.DataFrame", "pyspark.sql.DataFrame"],
+        df: "pd.DataFrame | pyspark.sql.DataFrame",
         dataset_path_or_rid: str,
         branch: str = "master",
         exists_ok: bool = False,
         mode: str = "SNAPSHOT",
-    ) -> Tuple[str, str]:
-        # pylint: disable=invalid-name,too-many-arguments,too-many-locals
+    ) -> "tuple[str, str]":
         """Saves a dataframe to Foundry. If the dataset in Foundry does not exist it is created.
 
         If the branch does not exist, it is created. If the dataset exists, an exception is thrown.
         If exists_ok=True is passed, the dataset is overwritten.
         Creates SNAPSHOT transactions by default.
 
         Args:
@@ -212,15 +215,14 @@
                 "Please provide a spark or pandas dataframe "
                 "object with parameter 'df'"
             )
         if branch is None:
             raise ValueError("Please provide a dataset branch with parameter 'branch'")
 
         with tempfile.TemporaryDirectory() as path:
-            # pylint: disable=import-outside-toplevel
             import pandas as pd
 
             if isinstance(df, pd.DataFrame):
                 df.to_parquet(
                     os.sep.join([path + "/dataset.parquet"]),
                     engine="pyarrow",
                     compression="snappy",
@@ -230,24 +232,19 @@
                 df.write.format("parquet").option("compression", "snappy").save(
                     path=path, mode="overwrite"
                 )
 
             filenames = list(
                 filter(lambda file: not file.endswith(".crc"), os.listdir(path))
             )
-            filepaths = list(map(lambda file: os.sep.join([path, file]), filenames))
-            if mode == "APPEND":
-                folder = round(time.time() * 1000)
-            else:
-                # to be backwards compatible to most readers, that expect files
-                # to be under spark/
-                folder = "spark"
-            dataset_paths_in_foundry = list(
-                map(lambda file: f"{folder}/" + file, filenames)
-            )
+            filepaths = [os.sep.join([path, file]) for file in filenames]
+            # to be backwards compatible to most readers, that expect files
+            # to be under spark/
+            folder = round(time.time() * 1000) if mode == "APPEND" else "spark"
+            dataset_paths_in_foundry = [f"{folder}/" + file for file in filenames]
             path_file_dict = dict(zip(dataset_paths_in_foundry, filepaths))
             dataset_rid, transaction_id = self._save_objects(
                 path_file_dict, dataset_path_or_rid, branch, exists_ok, mode
             )
 
         foundry_schema = self.api.infer_dataset_schema(dataset_rid, branch)
         self.api.upload_dataset_schema(
@@ -258,16 +255,15 @@
     def _save_objects(
         self,
         path_file_dict: dict,
         dataset_path_or_rid: str,
         branch: str,
         exists_ok: bool = False,
         mode: str = "SNAPSHOT",
-    ) -> Tuple[str, str]:
-        # pylint: disable=too-many-arguments
+    ) -> "tuple[str, str]":
         if path_file_dict is None or len(path_file_dict) == 0:
             raise ValueError(
                 "Please provide at least one file like object in dict 'path_file_dict"
             )
         if branch is None:
             raise ValueError("Please provide a dataset branch with parameter 'branch'")
 
@@ -317,16 +313,15 @@
     def save_model(
         self,
         model_obj: object,
         dataset_path_or_rid: str,
         branch: str = "master",
         exists_ok: bool = False,
         mode: str = "SNAPSHOT",
-    ) -> Tuple[str, str]:
-        # pylint: disable=too-many-arguments
+    ) -> "tuple[str, str]":
         """Saves a python object to a foundry dataset.
 
         The python object is pickled and uploaded to path model.pickle.
         The uploaded model can be loaded for performing predictions inside foundry
         pipelines.
 
         Args:
@@ -349,19 +344,17 @@
         """
         if model_obj is None:
             raise ValueError("Please provide a model object with parameter 'model_obj'")
         if branch is None:
             raise ValueError("Please provide a dataset branch with parameter 'branch'")
 
         with tempfile.TemporaryDirectory() as path:
-            model_path = os.sep.join([path, "model.pickle"])
-            with open(model_path, "wb") as file:
+            model_path = Path(path).joinpath("model.pickle")
+            with model_path.open(mode="wb") as file:
                 pickle.dump(model_obj, file)
-            result = self._save_objects(
-                {"model.pickle": model_path},
+            return self._save_objects(
+                {"model.pickle": os.fspath(model_path)},
                 dataset_path_or_rid,
                 branch,
                 exists_ok,
                 mode,
             )
-
-        return result
```

### Comparing `foundry-dev-tools-1.0.9/src/foundry_dev_tools/config.py` & `foundry-dev-tools-1.1/src/foundry_dev_tools/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,26 +8,25 @@
     Configuration.set('transforms_sql_sample_row_limit', 500)
     Configuration.get('transforms_sql_sample_row_limit')
 
 """
 import inspect
 import logging
 import os
-import pathlib
-import subprocess
 import warnings
 from collections import UserDict
 from configparser import ConfigParser
-from os import sep
 from pathlib import Path
+from typing import TYPE_CHECKING, Any
 
-import foundry_dev_tools
-from foundry_dev_tools.utils.token_provider.foundry_token_provider import (
-    TOKEN_PROVIDERS,
-)
+from foundry_dev_tools.utils.repo import find_project_config_file
+from foundry_dev_tools.utils.token_provider import TOKEN_PROVIDERS
+
+if TYPE_CHECKING:
+    import pathlib
 
 warnings.filterwarnings(
     "default", category=DeprecationWarning, module="foundry_dev_tools"
 )
 
 LOGGER = logging.getLogger(__name__)
 
@@ -42,14 +41,15 @@
     "transforms_sql_dataset_size_threshold": int,
     "transforms_sql_sample_select_random": bool,
     "transforms_force_full_dataset_download": bool,
     "cache_dir": os.path.expanduser,
     "transforms_freeze_cache": bool,
     "transforms_output_folder": os.path.expanduser,
     "enable_runtime_token_providers": bool,
+    "scopes": str,
 }
 
 
 def type_convert(config: dict) -> dict:
     """Type conversion for the config.
 
     Each config key has a defined type in :py:data:`TYPES`.
@@ -62,24 +62,21 @@
         dict:
             a dict with the same values except
             removed None values
             casted the types for defined keys in `TYPES`
     """
     return_config = {}
     for key, value in config.items():
-        if value is not None:
-            # convert value to its type
-            if key in TYPES:
-                value = TYPES[key](value)
-
-        return_config[key] = value
+        return_config[key] = (
+            TYPES[key](value) if value is not None and key in TYPES else None
+        )
     return return_config
 
 
-def initial_config() -> (dict, dict, pathlib.Path):
+def initial_config() -> "tuple[dict, pathlib.Path]":
     """Parses the config file and applies defaults.
 
     The order of config values and how they are applied are:
     defaults < global config file < project specific config < env variables
     < overwrites by :py:class:`~foundry_dev_tools.config.Config`
 
     Returns:
@@ -110,65 +107,59 @@
     config = {
         "jwt": None,
         "client_id": None,
         "client_secret": None,
         "grant_type": "authorization_code",
         "scopes": None,
         "foundry_url": None,
-        "cache_dir": os.path.join(foundry_dev_tools_directory, "cache"),
+        "cache_dir": foundry_dev_tools_directory / "cache",
         "transforms_output_folder": None,
         "transforms_sql_sample_select_random": False,
         "transforms_force_full_dataset_download": False,
         "enable_runtime_token_providers": True,
         "transforms_freeze_cache": False,
         "transforms_sql_sample_row_limit": 5000,
         "transforms_sql_dataset_size_threshold": 500,
     }
 
-    return_config = {}
-
-    for key in config:
-        if f"FOUNDRY_DEV_TOOLS_{key.upper()}" in os.environ:
-            return_config[key] = os.getenv(f"FOUNDRY_DEV_TOOLS_{key.upper()}")
-        elif f"FOUNDRY_LOCAL_{key.upper()}" in os.environ:
-            warnings.warn(
-                "Foundrylocal has been renamed to Foundry DevTools.\n"
-                "Rename your environment variables accordingly:\n"
-                f"FOUNDRY_LOCAL_{key.upper()} to FOUNDRY_DEV_TOOLS_{key.upper()}\n"
-                "The fallback to the old environment variables will be removed in the future!\n",
-                category=DeprecationWarning,
-            )
-            return_config[key] = os.getenv(f"FOUNDRY_LOCAL_{key.upper()}")
-
+    return_config: "dict[str, Any]" = {}
     if foundry_dev_tools_config_file.exists():
         config_parser = ConfigParser()
-        with open(
-            foundry_dev_tools_config_file.absolute(), "r", encoding="UTF-8"
-        ) as file:
+        with foundry_dev_tools_config_file.open(encoding="UTF-8") as file:
             config_parser.read_file(file)
             if "default" in config_parser:
                 return_config.update(config_parser["default"])
-    try:
-        caller_filename = getattr(inspect.stack()[1], "filename")
-        project_config_file = _find_project_config_file(
-            os.path.dirname(caller_filename)
-        )
+
+    caller_filename = inspect.stack()[-1].filename
+    project_config_file = find_project_config_file(Path(caller_filename).parent)
+    if project_config_file:
         project_config_parser = ConfigParser()
-        with open(str(project_config_file), "r", encoding="UTF-8") as file:
+        with project_config_file.open(encoding="UTF-8") as file:
             project_config_parser.read_file(file)
         if "default" in project_config_parser:
             LOGGER.debug(
                 "Using project based configuration file %s "
                 "on top of global configuration.",
                 project_config_file,
             )
             for key, value in project_config_parser.items("default"):
                 return_config[key] = value
-    except ValueError:
-        pass
+
+    for key in config:
+        if f"FOUNDRY_DEV_TOOLS_{key.upper()}" in os.environ:
+            return_config[key] = os.getenv(f"FOUNDRY_DEV_TOOLS_{key.upper()}")
+        elif f"FOUNDRY_LOCAL_{key.upper()}" in os.environ:
+            warnings.warn(
+                "Foundrylocal has been renamed to Foundry DevTools.\n"
+                "Rename your environment variables accordingly:\n"
+                f"FOUNDRY_LOCAL_{key.upper()} to FOUNDRY_DEV_TOOLS_{key.upper()}\n"
+                "The fallback to the old environment variables will be removed in the future!\n",
+                category=DeprecationWarning,
+            )
+            return_config[key] = os.getenv(f"FOUNDRY_LOCAL_{key.upper()}")
 
     config.update(return_config)
     return_config = type_convert(config)
     return return_config, foundry_dev_tools_directory
 
 
 class Config(UserDict):
@@ -183,21 +174,26 @@
 
     If you set a value to `None` it will not return `None`,
     but behave like the key doesn't exist.
 
     """
 
     def __init__(self, *args, **kwargs):
+        """The constructor is the same as for a dict.
+
+        The only difference is, that the config keys
+        get casted to their type.
+        """
         super().__init__(*args, **kwargs)
 
         # convert the dict to their types
         self.data = type_convert(self.data)
 
     def _combined(self) -> dict:
-        ___data = dict(foundry_dev_tools.INITIAL_CONFIG)
+        ___data = dict(INITIAL_CONFIG)
         ___data.update(self.data)
         __data = dict(___data)
         # if keys are none, they are "deleted"
         for key, value in ___data.items():
             if value is None:
                 del __data[key]
 
@@ -218,34 +214,35 @@
     def __repr__(self):
         return self._combined().__repr__()
 
     def __iter__(self):
         return iter(self._combined())
 
     def items(self):
+        """ItemsView of config dictionary."""
         return self._combined().items()
 
     def values(self):
+        """ValuesView of config dictionary."""
         return self._combined().values()
 
     def __len__(self):
         return len(self._combined())
 
     def __getitem__(self, key):
-        if key in self.data:
-            if self.data[key] is not None:
-                return self.data[key]
+        if key in self.data and self.data[key] is not None:
+            return self.data[key]
         return self.__missing__(key)
 
     def __delitem__(self, key):
         if key not in self:
             raise KeyError(key)
         self.data[key] = None
 
-    def set(self, key, value):
+    def set(self, key, value):  # noqa: A003
         """Deprecated: Stores value in config.
 
         Args:
             key (str): config key
             value (any): config value
         """
         warnings.warn(
@@ -271,43 +268,43 @@
     def _get_token_from_token_provider(self):
         """Tries to get a token from a token provider."""
         for tp in TOKEN_PROVIDERS:
             if token := tp().get_token():
                 return token
         return None
 
-    def get_config(self, overwrite_config: dict = None):
+    def get_config(self, overwrite_config: "dict | None" = None):
         """Returns the Foundry DevTools config.
 
         Merges the overwrite config from :py:class:`Config` with `overwrite_config` and returns a dict.
         If needed, jwt is fetched from a token provider.
 
         This method gets used by :py:class:`~foundry_dev_tools.foundry_api_client.FoundryRestClient`,
         :py:class:`~foundry_dev_tools.cached_foundry_client.CachedFoundryClient`
         and :py:class:`~foundry_dev_tools.foundry_api_client.FoundrySqlClient`,
         otherwise their internal config would change, if you changed the global configuration.
 
 
         Args:
-            overwrite_config (Optional[dict]): This is an overwrite config only for the returned dict
+            overwrite_config (dict | None): This is an overwrite config only for the returned dict
                               It will get applied above the overwrite config in `self`.
 
         Returns:
             dict:
         """
         cnf = dict(self)
         if overwrite_config:
             cnf.update(overwrite_config)
 
-        if (
-            ("jwt" not in cnf)
-            and "enable_runtime_token_providers" in cnf
-            and cnf["enable_runtime_token_providers"]
-        ):
-            if token := self._get_token_from_token_provider():
+        if "jwt" not in cnf:  # noqa: SIM102
+            if (
+                (token := self._get_token_from_token_provider())
+                and "enable_runtime_token_providers" in cnf
+                and cnf["enable_runtime_token_providers"]
+            ):
                 cnf["jwt"] = token
 
         if "foundry_url" not in cnf:
             raise ValueError(
                 "Please add your foundry url to the  config. (e.g. foundry_url=https://foundry.example.com)"
             )
 
@@ -318,60 +315,13 @@
                 "Foundry Third Party Application client_id (config key: 'client_id') \n"
                 "in configuration."
             )
 
         return cnf
 
 
-def _traverse_to_git_project_top_level_dir(git_dir: Path) -> str:
-    return execute_as_subprocess(["git", "rev-parse", "--show-toplevel"], git_dir)
-
-
-def execute_as_subprocess(args: list, cwd: Path) -> str:
-    """Wrapper around subprocess.
-
-    Args:
-        args (list): list of arguments for running
-        cwd (pathlib.Path): directory in where to run the command.
-
-    Returns:
-        :py:class:`str`:
-            stripped stdout of the output
-
-    """
-    return subprocess.run(
-        args, check=True, stdout=-1, stderr=-1, cwd=cwd, universal_newlines=True
-    ).stdout.strip()
-
-
-def _find_project_config_file(project_directory: Path) -> str:
-    try:
-        if os.path.isdir(project_directory):
-            git_directory = _traverse_to_git_project_top_level_dir(project_directory)
-            project_config_file = sep.join([git_directory, ".foundry_dev_tools"])
-
-            if os.path.isfile(project_config_file):
-                return project_config_file
-
-            foundry_local_project_config_file = sep.join(
-                [git_directory, ".foundry_local_config"]
-            )
-
-            if os.path.isfile(foundry_local_project_config_file):
-                warnings.warn(
-                    "Foundrylocal has been renamed to Foundry DevTools.\n"
-                    f"Move the old config file {foundry_local_project_config_file} to {project_config_file}\n"
-                    "The fallback to the old config file will be removed in the future!",
-                    category=DeprecationWarning,
-                )
-                return foundry_local_project_config_file
-        raise ValueError()
-    except FileNotFoundError as exc:
-        LOGGER.debug(
-            "Project-based config file could not be loaded due to missing git installation"
-        )
-        raise ValueError from exc
-    except subprocess.CalledProcessError as exc:
-        LOGGER.debug(
-            "Project-based config file could not be loaded, is project not managed with git?"
-        )
-        raise ValueError from exc
+(
+    INITIAL_CONFIG,
+    FOUNDRY_DEV_TOOLS_DIRECTORY,
+) = initial_config()
+Configuration = Config()
+__all__ = ["INITIAL_CONFIG", "FOUNDRY_DEV_TOOLS_DIRECTORY", "Configuration"]
```

### Comparing `foundry-dev-tools-1.0.9/src/foundry_dev_tools/foundry_api_client.py` & `foundry-dev-tools-1.1/src/foundry_dev_tools/foundry_api_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,66 +1,115 @@
-# pylint: disable=too-many-lines
 """Contains FoundryRestClient and FoundrySqlClient and exception classes.
 
 One of the gaols of this module is to be self-contained so that it can be
 dropped into any python installation with minimal dependency to 'requests'
 Optional dependencies for the SQL functionality to work are pandas and pyarrow.
 
 """
 import base64
 import builtins
 import functools
 import io
-import json
 import logging
 import multiprocessing
 import os
 import platform
 import shutil
+import sys
 import tempfile
 import time
 import warnings
 from contextlib import contextmanager
+from enum import Enum, EnumMeta
+from importlib.metadata import PackageNotFoundError, version
 from itertools import repeat
-from os import makedirs, path, remove, sep
 from pathlib import Path
-from typing import AnyStr, IO, Iterator, List, Optional, Tuple, Union
+from typing import IO, TYPE_CHECKING, AnyStr, List
 from urllib.parse import quote, quote_plus
 
+import palantir_oauth_client
 import requests
 
-import foundry_dev_tools
-from foundry_dev_tools import __version__ as fdt_version
+import foundry_dev_tools.config
 
+DEFAULT_REQUESTS_CONNECT_TIMEOUT = 10
+
+if TYPE_CHECKING:
+    from collections.abc import Iterator
+
+    import pandas as pd
+    import pyarrow as pa
+    import pyspark
 # On Python 3.8 on macOS, the default start method for new processes was
 #  switched to 'spawn' by default due to 'fork' potentially causing crashes.
 # These crashes haven't yet been observed with libE, but with 'spawn' runs,
 #  warnings about leaked semaphore objects are displayed instead.
 # The next several statements enforce 'fork' on macOS (Python 3.8)
 if platform.system() == "Darwin":
     from multiprocessing import set_start_method
 
     set_start_method("fork", force=True)
 
 LOGGER = logging.getLogger(__name__)
 
+# duplicate code from __init__.py
+# if we import __version__ from __init__.py
+# we will have a circular import
+# which may have unintended side effects
+try:
+    FDT_VERSION = version(__name__)
+except PackageNotFoundError:  # pragma: no cover
+    FDT_VERSION = "unknown"
+
 
 @contextmanager
 def _poolcontext(*args, **kwargs):
-    # pylint: disable=missing-function-docstring,consider-using-with
     pool = multiprocessing.Pool(*args, **kwargs)
     yield pool
     pool.terminate()
 
 
+class EnumContainsMeta(EnumMeta):
+    """Metaclass for the SQLReturnType.
+
+    It implements a proper __contains__ like 3.12 does.
+    """
+
+    def __contains__(cls, value):
+        """Backported a __contains__ from 3.12."""
+        if sys.version_info >= (3, 12):
+            return EnumMeta.__contains__(cls, value)
+        if isinstance(value, cls) and value._name_ in cls._member_map_:
+            return True
+        return value in cls._value2member_map_
+
+
+class SQLReturnType(str, Enum, metaclass=EnumContainsMeta):
+    """The return_types for sql queries.
+
+    PANDAS, PD: :external+pandas:py:class:`pandas.DataFrame` (pandas)
+    ARROW, PYARROW, PA: :external+pyarrow:py:class:`pyarrow.Table` (arrow)
+    SPARK, PYSPARK: :external+spark:py:class:`~pyspark.sql.DataFrame` (spark)
+    RAW: Tuple of (foundry_schema, data) (raw) (can only be used in legacy)
+    """
+
+    PANDAS = "pandas"
+    PD = PANDAS
+    SPARK = "spark"
+    PYSPARK = SPARK
+    ARROW = "arrow"
+    PYARROW = ARROW
+    PA = ARROW
+    RAW = "raw"
+
+
 class FoundryRestClient:
-    # pylint: disable=too-many-public-methods, too-many-instance-attributes
     """Zero dependency python client for Foundry's REST APIs."""
 
-    def __init__(self, config: dict = None):
+    def __init__(self, config: "dict | None" = None):
         """Create an instance of FoundryRestClient.
 
         Args:
             config (dict):^
              A dictionary containing basic configuration how to authenticate with Foundry.
              If config=None is passed, the Configuration class from foundry_dev_tools.config
              will be used to automatically apply a config based on the
@@ -72,29 +121,31 @@
              'client_id' (in case you have a third-party-app registration):
 
         Examples:
             >>> fc = FoundryRestClient()
             >>> fc = FoundryRestClient(config={'jwt': '<token>'})
             >>> fc = FoundryRestClient(config={'client_id': '<client_id>'})
         """
-        self._config = foundry_dev_tools.Configuration.get_config(config)
-        api_base = self._config["foundry_url"]
-        self.catalog = f"{api_base}/foundry-catalog/api"
-        self.compass = f"{api_base}/compass/api"
-        self.metadata = f"{api_base}/foundry-metadata/api"
-        self.data_proxy = f"{api_base}/foundry-data-proxy/api"
-        self.schema_inference = f"{api_base}/foundry-schema-inference/api"
-        self.multipass = f"{api_base}/multipass/api"
-        self._api_base = api_base
+        self._config = foundry_dev_tools.config.Configuration.get_config(config)
+        self._api_base = self._config["foundry_url"]
+        self.catalog = f"{self._api_base}/foundry-catalog/api"
+        self.compass = f"{self._api_base}/compass/api"
+        self.metadata = f"{self._api_base}/foundry-metadata/api"
+        self.data_proxy = f"{self._api_base}/foundry-data-proxy/api"
+        self.schema_inference = f"{self._api_base}/foundry-schema-inference/api"
+        self.multipass = f"{self._api_base}/multipass/api"
+        self.foundry_sql_server_api = f"{self._api_base}/foundry-sql-server/api"
+        self.jemma = f"{self._api_base}/jemma/api"
+        self.builds2 = f"{self._api_base}/build2/api"
         self._requests_verify_value = _determine_requests_verify_value(self._config)
 
     def _headers(self):
         return {
             "User-Agent": requests.utils.default_user_agent(
-                f"foundry-dev-tools/{fdt_version}/python-requests"
+                f"foundry-dev-tools/{FDT_VERSION}/python-requests"
             ),
             "Content-Type": "application/json",
             "Authorization": f"Bearer {_get_auth_token(self._config)}",
         }
 
     def _verify(self):
         return self._requests_verify_value
@@ -115,15 +166,18 @@
         response = _request(
             "POST",
             f"{self.catalog}/catalog/datasets",
             headers=self._headers(),
             verify=self._verify(),
             json={"path": dataset_path},
         )
-        if response.status_code == 400 and "DuplicateDatasetName" in response.text:
+        if (
+            response.status_code == requests.codes.bad
+            and "DuplicateDatasetName" in response.text
+        ):
             rid = self.get_dataset_rid(dataset_path=dataset_path)
             raise DatasetAlreadyExistsError(dataset_path=dataset_path, dataset_rid=rid)
         _raise_for_status_verbose(response)
         return response.json()
 
     def get_dataset(self, dataset_rid: str) -> dict:
         """Gets dataset_rid and fileSystemId.
@@ -140,15 +194,15 @@
         """
         response = _request(
             "GET",
             f"{self.catalog}/catalog/datasets/{dataset_rid}",
             headers=self._headers(),
             verify=self._verify(),
         )
-        if response.status_code == 204 and response.text == "":
+        if response.status_code == requests.codes.no_content and not response.text:
             raise DatasetNotFoundError(dataset_rid, response=response)
         _raise_for_status_verbose(response)
         return response.json()
 
     def delete_dataset(self, dataset_rid: str):
         """Deletes a dataset in Foundry and moves it to trash.
 
@@ -162,15 +216,18 @@
         response = _request(
             "DELETE",
             f"{self.catalog}/catalog/datasets",
             headers=self._headers(),
             verify=self._verify(),
             json={"rid": dataset_rid},
         )
-        if response.status_code == 400 and "DatasetsNotFound" in response.text:
+        if (
+            response.status_code == requests.codes.bad
+            and "DatasetsNotFound" in response.text
+        ):
             raise DatasetNotFoundError(dataset_rid, response=response)
         _raise_for_status_verbose(response)
         self.move_resource_to_trash(resource_id=dataset_rid)
 
     def move_resource_to_trash(self, resource_id: str):
         """Moves a Compass resource (e.g. dataset or folder) to trash.
 
@@ -181,26 +238,26 @@
         response_trash = _request(
             "POST",
             f"{self.compass}/batch/trash/add",
             headers=self._headers(),
             verify=self._verify(),
             data=f'["{resource_id}"]',
         )
-        if response_trash.status_code != 204:
+        if response_trash.status_code != requests.codes.no_content:
             raise KeyError(
                 f"Issue while moving resource '{resource_id}' to foundry trash."
             )
         _raise_for_status_verbose(response_trash)
 
     def create_branch(
         self,
         dataset_rid: str,
         branch: str,
-        parent_branch: str = None,
-        parent_branch_id: str = None,
+        parent_branch: "str | None" = None,
+        parent_branch_id: "str | None" = None,
     ) -> dict:
         """Creates a new branch in a dataset.
 
         If dataset is 'new', only parameter dataset_rid and branch are required.
 
         Args:
             dataset_rid (str): Unique identifier of the dataset
@@ -217,21 +274,24 @@
             "POST",
             f"{self.catalog}/catalog/datasets/{dataset_rid}/"
             f"branchesUnrestricted2/{quote_plus(branch)}",
             headers=self._headers(),
             verify=self._verify(),
             json={"parentBranchId": parent_branch, "parentRef": parent_branch_id},
         )
-        if response.status_code == 400 and "BranchesAlreadyExist" in response.text:
+        if (
+            response.status_code == requests.codes.bad
+            and "BranchesAlreadyExist" in response.text
+        ):
             raise BranchesAlreadyExistError(dataset_rid, branch, response=response)
         _raise_for_status_verbose(response)
         return response.json()
 
     def update_branch(
-        self, dataset_rid: str, branch: str, parent_branch: str = None
+        self, dataset_rid: str, branch: str, parent_branch: "str | None" = None
     ) -> dict:
         """Updates the latest transaction of branch 'branch' to the latest transaction of branch 'parent_branch'.
 
         Args:
             dataset_rid (str): Unique identifier of the dataset
             branch (str): The branch to update (e.g. master)
             parent_branch (str): the name of the branch to copy the last transaction from
@@ -279,15 +339,15 @@
         response = _request(
             "GET",
             f"{self.catalog}/catalog/datasets/{dataset_rid}/"
             f"branches2/{quote_plus(branch)}",
             headers=self._headers(),
             verify=self._verify(),
         )
-        if response.status_code == 204 and response.text == "":
+        if response.status_code == requests.codes.no_content and not response.text:
             raise BranchNotFoundError(dataset_rid, branch, response=None)
         _raise_for_status_verbose(response)
         return response.json()
 
     def open_transaction(
         self, dataset_rid: str, mode: str = "SNAPSHOT", branch: str = "master"
     ) -> str:
@@ -313,20 +373,26 @@
         response = _request(
             "POST",
             f"{self.catalog}/catalog/datasets/{dataset_rid}/" f"transactions",
             headers=self._headers(),
             verify=self._verify(),
             json={"branchId": f"{branch}", "record": {}},
         )
-        if response.status_code == 400 and "BranchesNotFound" in response.text:
+        if (
+            response.status_code == requests.codes.bad
+            and "BranchesNotFound" in response.text
+        ):
             raise BranchNotFoundError(dataset_rid, branch, response=response)
-        if response.status_code == 400 and "InvalidArgument" in response.text:
+        if (
+            response.status_code == requests.codes.bad
+            and "InvalidArgument" in response.text
+        ):
             raise DatasetNotFoundError(dataset_rid, response=response)
         if (
-            response.status_code == 400
+            response.status_code == requests.codes.bad
             and "SimultaneousOpenTransactionsNotAllowed" in response.text
         ):
             open_transaction_rid = response.json()["parameters"]["openTransactionRid"]
             raise DatasetHasOpenTransactionError(
                 dataset_rid=dataset_rid,
                 open_transaction_rid=open_transaction_rid,
                 response=response,
@@ -380,15 +446,15 @@
             headers=self._headers(),
             verify=self._verify(),
             params={"logicalPath": logical_path, "recursive": recursive},
         )
         _raise_for_status_verbose(response)
 
     def add_files_to_delete_transaction(
-        self, dataset_rid: str, transaction_id: str, logical_paths: List[str]
+        self, dataset_rid: str, transaction_id: str, logical_paths: "list[str]"
     ):
         """Adds files in an open DELETE transaction.
 
         Files added to DELETE transactions affect
         the dataset view by removing files from the view.
 
         Args:
@@ -422,15 +488,15 @@
             f"{self.catalog}/catalog/datasets/{dataset_rid}/"
             f"transactions/{transaction_id}/commit",
             headers=self._headers(),
             verify=self._verify(),
             json={"record": {}},
         )
         _raise_for_status_verbose(response)
-        if response.status_code != 204:
+        if response.status_code != requests.codes.no_content:
             raise KeyError(
                 f"{dataset_rid} issue while committing transaction {transaction_id}"
             )
 
     def abort_transaction(self, dataset_rid: str, transaction_id: str):
         """Aborts a transaction. Dataset will remain on transaction N-1.
 
@@ -447,15 +513,15 @@
             f"{self.catalog}/catalog/datasets/{dataset_rid}/"
             f"transactions/{transaction_id}/abortWithMetadata",
             headers=self._headers(),
             verify=self._verify(),
             json={"record": {}},
         )
         _raise_for_status_verbose(response)
-        if response.status_code != 204:
+        if response.status_code != requests.codes.no_content:
             raise KeyError(
                 f"{dataset_rid} issue while aborting transaction {transaction_id}"
             )
 
     def get_dataset_transactions(
         self,
         dataset_rid: str,
@@ -499,36 +565,36 @@
         as_json = response.json()
         if "values" in as_json and len(response.json()["values"]) > 0:
             return response.json()["values"]
         raise DatasetHasNoTransactionsError(dataset_rid, response=response)
 
     def get_dataset_last_transaction_rid(
         self, dataset_rid: str, branch: str = "master"
-    ) -> Optional[str]:
+    ) -> "str | None":
         """Returns the last transaction of a dataset / branch combination.
 
         Args:
             dataset_rid (str): Unique identifier of the dataset
             branch (str): Branch
 
         Returns:
-            Optional[str]:
+            str | None:
                 last_transaction_rid as string or None if dataset has no transaction.
 
         """
         try:
             return self.get_dataset_transactions(dataset_rid, branch)[0]["rid"]
         except DatasetHasNoTransactionsError:
             return None
 
     def upload_dataset_file(
         self,
         dataset_rid: str,
         transaction_rid: str,
-        path_or_buf: Union[str, Path, IO[AnyStr]],
+        path_or_buf: "str | Path | IO[AnyStr]",
         path_in_foundry_dataset: str,
     ):
         """Uploads a file like object to a path in a foundry dataset.
 
         Args:
             dataset_rid (str): Unique identifier of the dataset
             transaction_rid (str): transaction id
@@ -540,50 +606,50 @@
         """
         original_open = open
         builtins.open = (
             lambda f, *args, **kwargs: f
             if hasattr(f, "read")
             else original_open(f, *args, **kwargs)
         )
-        with open(path_or_buf, "rb") as file:
+        with open(path_or_buf, "rb") as file:  # noqa: PTH123
             response = _request(
                 "POST",
                 f"{self.data_proxy}/dataproxy/datasets/{dataset_rid}/"
                 f"transactions/{transaction_rid}/putFile",
                 params={"logicalPath": path_in_foundry_dataset},
                 data=file,
                 headers={
                     "Content-Type": "application/octet-stream",
                     "Authorization": self._headers()["Authorization"],
                 },
             )
         builtins.open = original_open
         _raise_for_status_verbose(response)
-        if response.status_code != 204:
+        if response.status_code != requests.codes.no_content:
             raise ValueError(
                 f"Issue while uploading file {path_or_buf} "
                 f"to dataset: {dataset_rid}, "
                 f"transaction_rid: {transaction_rid}. "
                 f"Response status: {response.status_code},"
                 f"Response text: {response.text}"
             )
 
     def upload_dataset_files(
         self,
         dataset_rid: str,
         transaction_rid: str,
         path_file_dict: dict,
-        parallel_processes: int = None,
+        parallel_processes: "int | None" = None,
     ):
         """Uploads multiple local files to a foundry dataset.
 
         Args:
             dataset_rid (str): Unique identifier of the dataset
             transaction_rid (str): transaction id
-            parallel_processes (Optional[int): Set number of threads for upload
+            parallel_processes (int | None): Set number of threads for upload
             path_file_dict (dict): A dictionary with the following structure:
 
         .. code-block:: python
 
          {
          '<path_in_foundry_dataset>': '<local_file_path>',
          ...
@@ -643,24 +709,24 @@
                 "GET",
                 f"{self.compass}/resources",
                 headers=self._headers(),
                 verify=self._verify(),
                 params={"path": dataset_path_or_rid, "decoration": "path"},
             )
         _raise_for_status_verbose(response)
-        if response.status_code != 200:
+        if response.status_code != requests.codes.ok:
             raise DatasetNotFoundError(dataset_path_or_rid, response=response)
         as_json = response.json()
         if as_json["directlyTrashed"]:
             warnings.warn(f"Dataset '{dataset_path_or_rid}' is in foundry trash.")
         return as_json
 
     def get_child_objects_of_folder(
-        self, folder_rid: str, page_size: int = None
-    ) -> Iterator[dict]:
+        self, folder_rid: str, page_size: "int | None" = None
+    ) -> "Iterator[dict]":
         """Returns the child objects of a compass folder.
 
         Args:
             folder_rid (str): Compass folder rid,
                 e.g. ri.compass.main.folder.f549ae09-9534-44c7-967a-6c86b2339231
             page_size (int): to control the pageSize manually
 
@@ -676,20 +742,19 @@
             response = _request(
                 "GET",
                 f"{self.compass}/folders/{folder_rid}/children",
                 headers=self._headers(),
                 params=query_params,
                 verify=self._verify(),
             )
-            if response.status_code == 404:
+            if response.status_code == requests.codes.not_found:
                 raise FolderNotFoundError(folder_rid, response=response)
             _raise_for_status_verbose(response)
             response_as_json = response.json()
-            for value in response_as_json["values"]:
-                yield value
+            yield from response_as_json["values"]
             if response_as_json["nextPageToken"] is None:
                 break
 
             query_params["pageToken"] = response_as_json["nextPageToken"]
 
     def create_folder(self, name: str, parent_id: str) -> dict:
         """Creates an empty folder in compass.
@@ -816,27 +881,27 @@
             "GET",
             f"{self.metadata}/schemas/datasets/"
             f"{dataset_rid}/branches/{quote_plus(branch)}",
             params={"endTransactionRid": transaction_rid},
             headers=self._headers(),
             verify=self._verify(),
         )
-        if response.status_code == 403:
+        if response.status_code == requests.codes.forbidden:
             raise DatasetNotFoundError(dataset_rid, response=response)
-        if response.status_code == 204:
+        if response.status_code == requests.codes.no_content:
             # here we don't know if schema does not exist or branch does not exist
             # we ask api for branch information, if branch does not exist, exception is thrown
             self.get_branch(dataset_rid, branch)
             raise DatasetHasNoSchemaError(dataset_rid, transaction_rid, branch)
-        if response.status_code == 404 or (
+        if response.status_code == requests.codes.not_found or (
             "errorName" in response.json()
             and response.json()["errorName"] == "Catalog:BranchesNotFound"
         ):
             raise BranchNotFoundError(dataset_rid, branch, response=response)
-        if response.status_code != 200:
+        if response.status_code != requests.codes.ok:
             raise KeyError(
                 f"{dataset_rid}, {branch}, {transaction_rid} combination not found"
             )
         return response.json()["schema"]
 
     def upload_dataset_schema(
         self,
@@ -926,36 +991,37 @@
         Raises:
             DatasetNoReadAccessError: if you have no read access for that dataset
 
         """
         dataset_details = self.get_dataset_details(dataset_path_or_rid)
         dataset_rid = dataset_details["rid"]
         dataset_path = dataset_details["path"]
-        if check_read_access:
-            if "gatekeeper:view-resource" not in dataset_details["operations"]:
-                raise DatasetNoReadAccessError(dataset_rid)
+        if (
+            check_read_access
+            and "gatekeeper:view-resource" not in dataset_details["operations"]
+        ):
+            raise DatasetNoReadAccessError(dataset_rid)
         return {
             "dataset_path": dataset_path,
             "dataset_rid": dataset_rid,
             "last_transaction_rid": self.get_dataset_last_transaction_rid(
                 dataset_rid, branch
             ),
         }
 
     def list_dataset_files(
         self,
         dataset_rid: str,
         exclude_hidden_files: bool = True,
         view: str = "master",
-        logical_path: str = None,
+        logical_path: "str | None" = None,
         detail: bool = False,
         *,
         include_open_exclusive_transaction: bool = False,
     ) -> list:
-        # pylint: disable=too-many-arguments
         """Returns list of internal filenames of a dataset.
 
         Args:
             dataset_rid (str): the dataset rid
             exclude_hidden_files (bool): if hidden files should be excluded (e.g. _log files)
             view (str): branch or transaction rid of the dataset
             logical_path (str): If logical_path is absent, returns all files in the view.
@@ -987,18 +1053,17 @@
                     "includeOpenExclusiveTransaction": include_open_exclusive_transaction,
                     "logicalPath": logical_path,
                     "excludeHiddenFiles": exclude_hidden_files,
                     "pageStartLogicalPath": next_page_token,
                 },
             )
             _raise_for_status_verbose(response)
-            if response.status_code != 200:
+            if response.status_code != requests.codes.ok:
                 raise DatasetNotFoundError(dataset_rid, response=response)
-            response_json = response.json()
-            return response_json
+            return response.json()
 
         result = []
         batch_result = _inner_get(next_page_token=None)
         result.extend(batch_result["values"])
         while batch_result["nextPageToken"] is not None:
             batch_result = _inner_get(next_page_token=batch_result["nextPageToken"])
             result.extend(batch_result["values"])
@@ -1028,73 +1093,60 @@
         )
         _raise_for_status_verbose(response)
         return response.json()
 
     def download_dataset_file(
         self,
         dataset_rid: str,
-        output_directory: Optional[str],
+        output_directory: "str | None",
         foundry_file_path: str,
         view: str = "master",
-    ) -> Union[str, bytes]:
+    ) -> "str | bytes":
         """Downloads a single foundry dataset file into a directory.
 
         Creates sub folder if necessary.
 
         Args:
             dataset_rid (str): the dataset rid
-            output_directory (Optional[str]): the local output directory for the file or None
+            output_directory (str | None): the local output directory for the file or None
                 if None is passed, byte content of file is returned
             foundry_file_path (str): the file_path on the foundry file system
             view (str): branch or transaction rid of the dataset
 
         Returns:
             str | bytes:
                 local file path in case output_directory was passed
                 or file content as bytes
 
         Raises:
             ValueError: If download failed
 
         """
-
         if output_directory is None:
             return self._download_dataset_file(
                 dataset_rid, view, foundry_file_path, stream=False
             ).content
-        file_directory = sep.join(
-            [output_directory, path.sep.join(foundry_file_path.split("/")[0:-1])]
-        )
-        makedirs(output_directory, exist_ok=True)
-        if "/" in foundry_file_path:
-            # check if file exists and is empty, in that case replace with folder
-            # can happen with empty s3 keys
-            if path.isfile(file_directory) and path.getsize(file_directory) == 0:
-                remove(file_directory)
-            makedirs(file_directory, exist_ok=True)
-        file_name = foundry_file_path.split("/")[-1]
-        local_file_path = os.path.normpath(sep.join([file_directory, file_name]))
+
+        local_path = Path(output_directory).joinpath(foundry_file_path)
+        file_dir = local_path.parent
+        if file_dir.is_file() and file_dir.stat().st_size == 0:
+            file_dir.unlink()
+        file_dir.mkdir(exist_ok=True, parents=True)
+        if local_path.is_dir():
+            return ""
         resp = self._download_dataset_file(
             dataset_rid, view, foundry_file_path, stream=True
         )
-        if path.isdir(local_file_path):
-            resp.close()
-            return ""
-        with open(local_file_path, "wb") as out_file:
-            if resp.status_code != 200:
-                raise ValueError(
-                    f"Issue while downloading {dataset_rid}, "
-                    f"file {foundry_file_path}, branch/transaction_rid {view}."
-                    f"Response status was {resp.status_code}"
-                )
+        _raise_for_status_verbose(resp)
+        with local_path.open(mode="wb") as out_file:
             resp.raw.decode_content = True
             shutil.copyfileobj(resp.raw, out_file)
 
         resp.close()
-        return local_file_path
+        return os.fspath(local_path)
 
     def _download_dataset_file(self, dataset_rid, view, foundry_file_path, stream=True):
         response = _request(
             "GET",
             f"{self.data_proxy}/dataproxy/datasets/"
             f"{dataset_rid}/views/{quote_plus(view)}/{quote(foundry_file_path)}",
             headers=self._headers(),
@@ -1103,28 +1155,27 @@
         _raise_for_status_verbose(response)
         return response
 
     def download_dataset_files(
         self,
         dataset_rid: str,
         output_directory: str,
-        files: list = None,
+        files: "list | None" = None,
         view: str = "master",
-        parallel_processes: int = None,
-    ) -> List[str]:
-        # pylint: disable=too-many-arguments, unused-argument
+        parallel_processes: "int | None" = None,
+    ) -> "list[str]":
         """Downloads files of a dataset (in parallel) to a local output directory.
 
         Args:
             dataset_rid (str): the dataset rid
-            files (Optional[list]): list of files or None, in which case all files are downloaded
+            files (list | None): list of files or None, in which case all files are downloaded
             output_directory (str): the output directory for the files
                 default value is calculated: multiprocessing.cpu_count() - 1
             view (str): branch or transaction rid of the dataset
-            parallel_processes (Optional[int]): Set number of threads for upload
+            parallel_processes (int | None): Set number of threads for upload
 
         Returns:
             List[str]:
                 path to downloaded files
 
         """
         if files is None:
@@ -1154,45 +1205,47 @@
                             repeat(dataset_rid),
                             repeat(output_directory),
                             files,
                             repeat(view),
                         ),
                     )
                 )
-        return list(filter(lambda p: p != "", local_paths))
+        return list(filter(lambda p: p != "", local_paths))  # noqa: PLC1901
 
     @contextmanager
     def download_dataset_files_temporary(
         self,
         dataset_rid: str,
-        files: list = None,
+        files: "list | None" = None,
         view: str = "master",
-        parallel_processes: Optional[int] = None,
-    ) -> str:
+        parallel_processes: "int | None" = None,
+    ) -> "Iterator[str]":
         """Downloads all files of a dataset to a temporary directory.
 
         Which is deleted when the context is closed. Function returns the temporary directory.
         Example usage:
 
+        >>> import parquet
+        >>> import pandas as pd
+        >>> from pathlib import Path
         >>> with client.download_dataset_files_temporary(dataset_rid='ri.foundry.main.dataset.1', view='master') as \
-            temp_folder:
+        >>> temp_folder:
         >>>     # Read using Pandas
         >>>     df = pd.read_parquet(temp_folder)
         >>>     # Read using pyarrow, here we pass only the files, which are normally in subfolder 'spark'
-        >>>     from pathlib import Path
         >>>     pq = parquet.ParquetDataset(path_or_paths=[x for x in Path(temp_dir).glob('**/*') if x.is_file()])
 
         Args:
             dataset_rid (str): the dataset rid
             files (List[str]): list of files or None, in which case all files are downloaded
             view (str): branch or transaction rid of the dataset
             parallel_processes (int): Set number of threads for download
 
-        Returns:
-            str:
+        Yields:
+            Iterator[str]:
                 path to temporary folder containing root of dataset files
 
         """
         temp_output_directory = tempfile.mkdtemp(
             suffix=f"foundry_dev_tools-{dataset_rid}"
         )
         _ = self.download_dataset_files(
@@ -1233,130 +1286,179 @@
             stream=True,
         )
 
         _raise_for_status_verbose(response)
         return response
 
     def query_foundry_sql_legacy(
-        self, query: str, branch: str = "master"
-    ) -> (dict, list):
+        self,
+        query: str,
+        branch: str = "master",
+        return_type: SQLReturnType = SQLReturnType.RAW,
+        timeout: int = 600,
+    ) -> "tuple[dict, List[List]] | pd.core.frame.DataFrame | pyspark.sql.DataFrame | pa.Table":
         """Queries the dataproxy query API with spark SQL.
 
         Example:
             client.query_foundry_sql_legacy(query="SELECT * FROM `/Global/Foundry Operations/Foundry Support/iris`",
                                             branch="master")
 
         Args:
             query (str): the sql query
             branch (str): the branch of the dataset / query
+            return_type (SQLReturnType): See :py:class:foundry_dev_tools.foundry_api_client.SQLReturnType
+            timeout (int): the query timeout, default value is 600 seconds
 
         Returns:
             Tuple (dict, list):
                 foundry_schema, data.
                 data contains the data matrix,
                 foundry_schema the foundry schema (fieldSchemaList key).
                 Can be converted to a pandas Dataframe, see below
 
             .. code-block:: python
 
              foundry_schema, data = self.query_foundry_sql_legacy(query, branch)
              df = pd.DataFrame(data=data, columns=[e['name'] for e in foundry_schema['fieldSchemaList']])
 
         Raises:
+            ValueError: if return_type is not in :py:class:SQLReturnType
             DatasetHasNoSchemaError: if dataset has no schema
             BranchNotFoundError: if branch was not found
         """
+        # if return_type is a str this will also work, this will get fixed in python 3.12
+        # where we would be able to use `return_type not in SQLReturnType`
+        if return_type not in SQLReturnType:
+            raise ValueError(
+                f"return_type ({return_type}) should be a member of foundry_dev_tools.foundry_api_client.SQLReturnType"
+            )
         response = _request(
             "POST",
             f"{self.data_proxy}/dataproxy/queryWithFallbacks",
             headers=self._headers(),
             verify=self._verify(),
             params={"fallbackBranchIds": [branch]},
             json={"query": query},
+            read_timeout=timeout,
         )
 
         if (
-            response.status_code == 404
+            response.status_code == requests.codes.not_found
             and response.json()["errorName"] == "DataProxy:SchemaNotFound"
         ):
             dataset_rid = response.json()["parameters"]["datasetRid"]
             raise DatasetHasNoSchemaError(dataset_rid, branch=branch)
         if (
-            response.status_code == 400
+            response.status_code == requests.codes.bad
             and response.json()["errorName"]
             == "DataProxy:FallbackBranchesNotSpecifiedInQuery"
         ):
             # FallbackBranchesNotSpecifiedInQuery does not sound right,
             # but this indicates that the branch does not exist
             raise BranchNotFoundError(
                 response.json()["parameters"]["datasetRid"],
                 branch,
                 response=response,
             )
 
         _raise_for_status_verbose(response)
         response_json = response.json()
-        return response_json["foundrySchema"], response_json["rows"]
+        if return_type == SQLReturnType.RAW:
+            return response_json["foundrySchema"], response_json["rows"]
+        if return_type == SQLReturnType.PANDAS:
+            import pandas as pd
+
+            return pd.DataFrame(
+                data=response_json["rows"],
+                columns=[
+                    e["name"] for e in response_json["foundrySchema"]["fieldSchemaList"]
+                ],
+            )
+        if return_type == SQLReturnType.ARROW:
+            import pyarrow as pa
+
+            return pa.table(
+                data=response_json["rows"],
+                names=[
+                    e["name"] for e in response_json["foundrySchema"]["fieldSchemaList"]
+                ],
+            )
+        if return_type == SQLReturnType.SPARK:
+            from foundry_dev_tools.utils.converter.foundry_spark import (
+                foundry_schema_to_spark_schema,
+                foundry_sql_data_to_spark_dataframe,
+            )
+
+            return foundry_sql_data_to_spark_dataframe(
+                data=response_json["rows"],
+                spark_schema=foundry_schema_to_spark_schema(
+                    response_json["foundrySchema"]
+                ),
+            )
+        return None
 
     def query_foundry_sql(
-        self, query, branch="master", return_type="pandas"
-    ) -> "pandas.core.frame.DataFrame | pyarrow.Table | pyspark.sql.DataFrame":
-        # pylint: disable=line-too-long
+        self,
+        query: str,
+        branch: str = "master",
+        return_type: SQLReturnType = SQLReturnType.PANDAS,
+        timeout: int = 600,
+    ) -> "pd.core.frame.DataFrame | pa.Table | pyspark.sql.DataFrame":
         """Queries the Foundry SQL server with spark SQL dialect.
 
         Uses Arrow IPC to communicate with the Foundry SQL Server Endpoint.
+
+        Falls back to query_foundry_sql_legacy in case pyarrow is not installed or the query does not return
+        Arrow Format.
+
         Example:
-            client.query_foundry_sql("SELECT * FROM `/Global/Foundry Operations/Foundry Support/iris`")
+            df1 = client.query_foundry_sql("SELECT * FROM `/Global/Foundry Operations/Foundry Support/iris`")
+            query = ("SELECT col1 FROM `{start_transaction_rid}:{end_transaction_rid}@{branch}`.`{dataset_path_or_rid}` WHERE filterColumns = 'value1' LIMIT 1")
+            df2 = client.query_foundry_sql(query)
 
         Args:
-            query (str): the sql query
-            branch (str): the branch of the dataset / query
-            return_type (str, pandas | arrow | spark): Whether to return
-                :external+pandas:py:class:`pandas.DataFrame`, :external+pyarrow:py:class:`pyarrow.Table` or
-                :external+spark:py:class:`~pyspark.sql.DataFrame`
+            query (str): The SQL Query in Foundry Spark Dialect (use backticks instead of quotes)
+            branch (str): The branch of the dataset / query
+            return_type (SQLReturnType): See :py:class:foundry_dev_tools.foundry_api_client.SQLReturnType
+            timeout (int): Query Timeout, default value is 600 seconds
 
         Returns:
             :external+pandas:py:class:`~pandas.DataFrame` | :external+pyarrow:py:class:`~pyarrow.Table` | :external+spark:py:class:`~pyspark.sql.DataFrame`:
 
             A pandas DataFrame, Spark DataFrame or pyarrow.Table with the result.
 
         Raises:
             ValueError: Only direct read eligible queries can be returned as arrow Table.
 
-        """
-        assert return_type in {"pandas", "arrow", "spark"}
-        foundry_sql_client = FoundrySqlClient(config=self._config, branch=branch)
-        try:
-            return foundry_sql_client.query(query=query, return_type=return_type)
-        except FoundrySqlSerializationFormatNotImplementedError as exc:
-            if return_type == "arrow":
-                raise ValueError(
-                    "Only direct read eligible queries can be returned as arrow Table. "
-                    "Consider using setting return_type to 'pandas'."
-                ) from exc
-            foundry_schema, data = self.query_foundry_sql_legacy(query, branch)
-
-            if return_type == "pandas":
-                # pylint: disable=import-outside-toplevel
-                import pandas as pd
-
-                return pd.DataFrame(
-                    data=data,
-                    columns=[e["name"] for e in foundry_schema["fieldSchemaList"]],
-                )
-            # pylint: disable=import-outside-toplevel
-            from foundry_dev_tools.utils.converter.foundry_spark import (
-                foundry_schema_to_spark_schema,
-                foundry_sql_data_to_spark_dataframe,
-            )
-
-            return foundry_sql_data_to_spark_dataframe(
-                data=data,
-                spark_schema=foundry_schema_to_spark_schema(foundry_schema),
+        """  # noqa: E501
+        # if return_type is a str this will also work, this will get fixed in python 3.12
+        # where we would be able to use `return_type not in SQLReturnType`
+        if return_type not in SQLReturnType:
+            raise ValueError(
+                f"return_type ({return_type}) should be a member of foundry_dev_tools.foundry_api_client.SQLReturnType"
             )
+        if return_type != SQLReturnType.RAW:
+            try:
+                return self._query_fsql(
+                    query=query, branch=branch, return_type=return_type
+                )
+            except (
+                FoundrySqlSerializationFormatNotImplementedError,
+                ImportError,
+            ) as exc:
+                if return_type == SQLReturnType.ARROW:
+                    raise ValueError(
+                        "Only direct read eligible queries can be returned as arrow Table. "
+                        "Consider using setting return_type to 'pandas'."
+                    ) from exc
+
+        warnings.warn("Falling back to query_foundry_sql_legacy!")
+        return self.query_foundry_sql_legacy(
+            query=query, branch=branch, return_type=return_type, timeout=timeout
+        )
 
     def get_user_info(self) -> dict:
         """Returns the multipass user info.
 
         Returns:
             dict:
 
@@ -1433,31 +1535,30 @@
         client_type: str,
         display_name: str,
         description: "str | None",
         grant_types: list,
         redirect_uris: "list | None",
         logo_uri: "str | None",
         organization_rid: str,
-        allowed_organization_rids: list = None,
+        allowed_organization_rids: "list | None" = None,
     ) -> dict:
-        # pylint: disable=too-many-arguments
         """Creates Foundry Third Party application (TPA).
 
         https://www.palantir.com/docs/foundry/platform-security-third-party/third-party-apps-overview/
         User must have 'Manage OAuth 2.0 clients' workflow permissions.
 
         Args:
             client_type (str): Server Application (CONFIDENTIAL) or
                 Native or single-page application (PUBLIC)
             display_name (str): Display name of the TPA
-            description (Optional[str]): Long description of the TPA
+            description (str | None): Long description of the TPA
             grant_types (list): Usually, ["AUTHORIZATION_CODE", "REFRESH_TOKEN"] (authorization code grant)
                 or ["REFRESH_TOKEN", "CLIENT_CREDENTIALS"] (client credentials grant)
-            redirect_uris (Optional[list]): Redirect URLs of TPA, used in combination with AUTHORIZATION_CODE grant
-            logo_uri (Optional[str]): URI or embedded image 'data:image/png;base64,<...>'
+            redirect_uris (list | None): Redirect URLs of TPA, used in combination with AUTHORIZATION_CODE grant
+            logo_uri (str | None): URI or embedded image 'data:image/png;base64,<...>'
             organization_rid (str): Parent Organization of this TPA
             allowed_organization_rids (list): Passing None or empty list means TPA is activated for all
                 Foundry organizations
 
         Returns:
             dict:
                 See below for the structure
@@ -1474,21 +1575,28 @@
                 "logoUri":null,
                 "grantTypes":[<"AUTHORIZATION_CODE","REFRESH_TOKEN","CLIENT_CREDENTIALS">],
                 "redirectUris":[],
                 "allowedOrganizationRids":[]
             }
 
         """
-        assert client_type in ["CONFIDENTIAL", "PUBLIC"]
+        if client_type not in ["CONFIDENTIAL", "PUBLIC"]:
+            raise AssertionError(
+                f"client_type ({client_type}) needs to be one of CONFIDENTIAL or PUBLIC"
+            )
         for grant in grant_types:
-            assert grant in [
+            if grant not in [
                 "AUTHORIZATION_CODE",
                 "REFRESH_TOKEN",
                 "CLIENT_CREDENTIALS",
-            ]
+            ]:
+                raise AssertionError(
+                    f"grant ({grant}) needs to be one of "
+                    "AUTHORIZATION_CODE, REFRESH_TOKEN or CLIENT_CREDENTIALS"
+                )
         if allowed_organization_rids is None:
             allowed_organization_rids = []
         response = _request(
             "POST",
             f"{self.multipass}/clients",
             headers=self._headers(),
             verify=self._verify(),
@@ -1526,17 +1634,16 @@
         client_type: str,
         display_name: str,
         description: "str | None",
         grant_types: list,
         redirect_uris: "list | None",
         logo_uri: "str | None",
         organization_rid: str,
-        allowed_organization_rids: list = None,
+        allowed_organization_rids: "list | None" = None,
     ) -> dict:
-        # pylint: disable=too-many-arguments
         """Updates Foundry Third Party application (TPA).
 
         https://www.palantir.com/docs/foundry/platform-security-third-party/third-party-apps-overview/
         User must have 'Manage OAuth 2.0 clients' workflow permissions.
 
         Args:
             client_id (str): The unique identifier of the TPA.
@@ -1567,21 +1674,28 @@
                 "logoUri":null,
                 "grantTypes":[<"AUTHORIZATION_CODE","REFRESH_TOKEN","CLIENT_CREDENTIALS">],
                 "redirectUris":[],
                 "allowedOrganizationRids":[]
             }
 
         """
-        assert client_type in ["CONFIDENTIAL", "PUBLIC"]
+        if client_type not in ["CONFIDENTIAL", "PUBLIC"]:
+            raise AssertionError(
+                f"client_type ({client_type}) needs to be one of CONFIDENTIAL or PUBLIC"
+            )
         for grant in grant_types:
-            assert grant in [
+            if grant not in [
                 "AUTHORIZATION_CODE",
                 "REFRESH_TOKEN",
                 "CLIENT_CREDENTIALS",
-            ]
+            ]:
+                raise AssertionError(
+                    f"grant ({grant}) needs to be one of "
+                    "AUTHORIZATION_CODE, REFRESH_TOKEN or CLIENT_CREDENTIALS"
+                )
         if allowed_organization_rids is None:
             allowed_organization_rids = []
         response = _request(
             "PUT",
             f"{self.multipass}/clients/{client_id}",
             headers=self._headers(),
             verify=self._verify(),
@@ -1677,135 +1791,170 @@
             headers=self._headers(),
             verify=self._verify(),
             json={"operations": operations, "resources": resources},
         )
         _raise_for_status_verbose(response)
         return response.json()
 
+    def start_checks_and_build(
+        self,
+        repository_id: str,
+        ref_name: str,
+        commit_hash: str,
+        file_paths: "List[str]",
+    ) -> dict:
+        """Starts checks and builds.
 
-class FoundrySqlClient:
-    # pylint: disable=too-few-public-methods
-    """Class to interact with Foundry's SQL Server using ARROW IPC Protocol."""
+        Args:
+            repository_id (str): the repository id where the transform is located
+            ref_name (str): the git ref_name for the branch
+            commit_hash (str): the git commit hash
+            file_paths (List[str]): a list of python transform files
 
-    def __init__(self, config: dict = None, branch="master"):
-        """Construct an instance of FoundrySqlClient.
+        Returns:
+            dict: the JSON API response
+        """
+        response = _request(
+            "POST",
+            f"{self.jemma}/builds",
+            headers=self._headers(),
+            verify=self._verify(),
+            json={
+                "jobs": [
+                    {
+                        "name": "Checks",
+                        "type": "exec",
+                        "parameters": {
+                            "repositoryTarget": {
+                                "repositoryRid": repository_id,
+                                "refName": ref_name,
+                                "commitHash": commit_hash,
+                            }
+                        },
+                        "reuseExistingJob": True,
+                    },
+                    {
+                        "name": "Build initialization",
+                        "type": "foundry-run-build",
+                        "parameters": {
+                            "fallbackBranches": [],
+                            "filePaths": file_paths,
+                            "rids": [],
+                            "buildParameters": {},
+                        },
+                        "reuseExistingJob": True,
+                    },
+                ],
+                "reuseExistingJobs": True,
+            },
+        )
+        _raise_for_status_verbose(response)
+        return response.json()
+
+    def get_build(self, build_rid: str) -> dict:
+        """Get information about the build.
 
         Args:
-            config (dict): configuration dictionary, equivalent to FoundryRestClient
-            branch (str):  default = master, all queries will be executed against this default branch
+            build_rid (str): the build RID
 
+        Returns:
+            dict: the JSON API response
         """
-        self._config = foundry_dev_tools.Configuration.get_config(config)
-        self._requests_verify_value = _determine_requests_verify_value(self._config)
-        self.foundry_sql_server_api = (
-            f"{self._config['foundry_url']}/foundry-sql-server/api"
-        )
-        self._headers = self._get_initial_headers(session_authorization=None)
-        self.branch = branch
-        self.session_id, self.session_auth_token = self._establish_session(
-            branch=branch
-        )
-        self._headers = self._get_initial_headers(
-            session_authorization=self.session_auth_token
+        response = _request(
+            "GET",
+            f"{self.builds2}/info/builds2/{build_rid}",
+            headers=self._headers(),
+            verify=self._verify(),
         )
+        _raise_for_status_verbose(response)
+        return response.json()
 
-    def _get_initial_headers(self, session_authorization=None):
-        return {
-            "User-Agent": requests.utils.default_user_agent(
-                f"foundry-dev-tools/{fdt_version}/python-requests"
-            ),
-            "Accept": "application/json",
-            "Accept-Encoding": "gzip, deflate, br",
-            "Content-Type": "application/json",
-            "Session-Authorization": session_authorization,
-            "Authorization": f"Bearer {_get_auth_token(self._config)}",
-        }
+    def get_job_report(self, job_rid: str) -> dict:
+        """Get the report for a job.
+
+        Args:
+            job_rid (str): the job RID
 
-    def _establish_session(self, branch="master") -> Tuple[str, str]:
+        Returns:
+            dict: the job report response
+
+        """
         response = _request(
-            "POST",
-            f"{self.foundry_sql_server_api}/sessions",
-            headers=self._headers,
-            verify=self._requests_verify_value,
-            json={
-                "configuration": {
-                    "fallbackBranchIds": [branch],
-                    "queryTimeoutMillis": None,
-                },
-                "protocolVersion": None,
-            },
+            "GET",
+            f"{self.builds2}/info/jobs3/{job_rid}",
+            headers=self._headers(),
+            verify=self._verify(),
         )
         _raise_for_status_verbose(response)
-        response_json = response.json()
-        session_id = response_json["sessionId"]
-        session_auth_token = response_json["sessionAuthToken"]
-        return session_id, session_auth_token
+        return response.json()
 
-    def _prepare_and_execute(self, query: str) -> dict:
+    def _execute_fsql_query(self, query: str, branch="master", timeout=600) -> dict:
         response = _request(
             "POST",
-            f"{self.foundry_sql_server_api}/sessions/"
-            f"{self.session_id}/prepare-and-execute-statement",
-            headers=self._headers,
+            f"{self.foundry_sql_server_api}/queries/execute",
+            headers=self._headers(),
             verify=self._requests_verify_value,
             json={
                 "dialect": "SPARK",
+                "fallbackBranchIds": [branch],
                 "parameters": {
                     "type": "unnamedParameterValues",
                     "unnamedParameterValues": [],
                 },
                 "query": query,
-                "serializationProtocol": "ARROW",
+                "serializationProtocol": "ARROW_V1",
+                "timeout": timeout,
             },
         )
         _transform_bad_request_response_to_exception(response)
         _raise_for_status_verbose(response)
         return response.json()
 
-    def _poll_for_query_completion(self, initial_response_json: dict, timeout=600):
+    def _poll_fsql_query_status(self, initial_response_json: dict, timeout=600):
         start_time = time.time()
-        statement_id = initial_response_json["statementId"]
+        query_id = initial_response_json["queryId"]
         response_json = initial_response_json
         while response_json["status"]["type"] == "running":
             response = _request(
-                "POST",
-                f"{self.foundry_sql_server_api}/" f"statements/{statement_id}/status",
-                headers=self._headers,
+                "GET",
+                f"{self.foundry_sql_server_api}/queries/{query_id}/status",
+                headers=self._headers(),
                 verify=self._requests_verify_value,
                 json={},
             )
             _raise_for_status_verbose(response)
             response_json = response.json()
             if response_json["status"]["type"] == "failed":
                 raise FoundrySqlQueryFailedError(response=response)
             if time.time() > start_time + timeout:
                 raise FoundrySqlQueryClientTimedOutError(timeout)
             time.sleep(0.2)
 
-    def _read_results_arrow(
-        self, statement_id: str
-    ) -> "pyarrow.ipc.RecordBatchStreamReader":
-        headers = self._headers
+    def _read_fsql_query_results_arrow(
+        self, query_id: str
+    ) -> "pa.ipc.RecordBatchStreamReader":
+        import pyarrow as pa
+
+        headers = self._headers()
         headers["Accept"] = "application/octet-stream"
         headers["Content-Type"] = "application/json"
         # Couldn't get preload_content=False and gzip content-encoding to work together
         # If no bytesIO wrapper is used, response.read(1, cache_content=true)
         # does not return the first character but an empty byte (no idea why).
         # So it is essentially a trade-off between download time and memory consumption.
         # Download time seems to be a lot faster (2x) with gzip encoding turned on, while
         # memory consumption increases by the amount of raw bytes returned from the sql server.
         # I will optimize for faster downloads, for now. This decision can be revisited later.
         #
         # 01/2022: Moving to 'requests' instead of 'urllib3', did some experiments again
         # and noticed that preloading content is significantly faster than stream=True
 
         response = _request(
-            "POST",
-            f"{self.foundry_sql_server_api}/" f"statements/{statement_id}/results",
-            data=json.dumps({}).encode("utf-8"),
+            "GET",
+            f"{self.foundry_sql_server_api}/queries/{query_id}/results",
             headers=headers,
         )
         bytes_io = io.BytesIO(response.content)
         arrow_format = bytes_io.read(1).decode("UTF-8")
         if arrow_format != "A":
             # Queries are direct read eligible when:
             # The dataset files are in a supported format.
@@ -1813,112 +1962,88 @@
 
             # The query does not require SQL compute. Queries which contain aggregate, join, order by,
             # and filter predicates are not direct read eligible.
 
             # The query does not select from a column with a type that is ineligible for direct read.
             # Ineligible types are array, map, and struct.
 
+            # May 2023: ARROW_V1 seems to consistently return ARROW format and not fallback to JSON.
+
             raise FoundrySqlSerializationFormatNotImplementedError()
-        # pylint: disable=import-outside-toplevel
-        import pyarrow as pa
 
         return pa.ipc.RecordBatchStreamReader(bytes_io)
 
-    def query(
-        self, query: str, timeout=600, return_type="pandas"
-    ) -> "pandas.core.frame.DataFrame | pyarrow.Table | pyspark.sql.DataFrame":
-        """Queries the foundry sql endpoint. Current dialect is hard-coded to SPARK.
-
-        Example Queries:
-
-        .. code-block:: python
-
-         # direct read if dataset is backed by parquet files, no size limit
-         df1 = client.query(f'SELECT * FROM `{dataset_path}`')
-
-         query = ("SELECT col1 FROM `{start_transaction_rid}:{end_transaction_rid}@{branch}`.`{dataset_path_or_rid}`"
-                  "WHERE filterColumns = 'value1' LIMIT 1")
-         df2 = client.query(query)
-
-        Args:
-            query (str): Query
-            timeout (float): default value 600 seconds
-            return_type (str: pandas | arrow | spark): return type, one of pandas, arrow or spark.
-                Whether to return :external+pandas:py:class:`~pandas.DataFrame`,
-                :external+spark:py:class:`~pyspark.sql.DataFrame`
-                or :external+pyarrow:py:class:`~pyarrow.Table`
-
-        Returns:
-             :external+pandas:py:class:`~pandas.DataFrame` | :external+spark:py:class:`~pyspark.sql.DataFrame` |
-                :external+pyarrow:py:class:`~pyarrow.Table`:
-                A pandas dataframe, pyspark dataframe or pyarrow Table with the result
-
-
+    def _query_fsql(
+        self,
+        query: str,
+        branch: str = "master",
+        return_type: SQLReturnType = SQLReturnType.PANDAS,
+        timeout: int = 600,
+    ) -> "pd.core.frame.DataFrame | pa.Table | pyspark.sql.DataFrame":
+        # if return_type is a str this will also work, this will get fixed in python 3.12
+        # where we would be able to use `return_type not in SQLReturnType`
+        if return_type not in SQLReturnType:
+            raise ValueError(
+                f"return_type ({return_type}) should be a member of foundry_dev_tools.foundry_api_client.SQLReturnType"
+            )
 
-        """
-        assert return_type in {"pandas", "arrow", "spark"}
+        response_json = self._execute_fsql_query(query, branch=branch, timeout=timeout)
+        query_id = response_json["queryId"]
+        status = response_json["status"]
 
-        response_json = self._prepare_and_execute(query)
-        statement_id = response_json["statementId"]
+        if status != {"ready": {}, "type": "ready"}:
+            self._poll_fsql_query_status(
+                initial_response_json=response_json, timeout=timeout
+            )
 
-        self._poll_for_query_completion(
-            initial_response_json=response_json, timeout=timeout
-        )
-        arrow_stream_reader = self._read_results_arrow(statement_id)
-        if return_type == "pandas":
+        arrow_stream_reader = self._read_fsql_query_results_arrow(query_id=query_id)
+        if return_type == SQLReturnType.PANDAS:
             return arrow_stream_reader.read_pandas()
-        if return_type == "spark":
-            # pylint: disable=import-outside-toplevel
+        if return_type == SQLReturnType.SPARK:
             from foundry_dev_tools.utils.converter.foundry_spark import (
                 arrow_stream_to_spark_dataframe,
             )
 
             return arrow_stream_to_spark_dataframe(arrow_stream_reader)
         return arrow_stream_reader.read_all()
 
 
 def _transform_bad_request_response_to_exception(response):
     if (
-        response.status_code == 400
+        response.status_code == requests.codes.bad
         and response.json()["errorName"] == "FoundrySqlServer:InvalidDatasetNoSchema"
     ):
         raise DatasetHasNoSchemaError("SQL")
     if (
-        response.status_code == 400
+        response.status_code == requests.codes.bad
         and response.json()["errorName"]
         == "FoundrySqlServer:InvalidDatasetCannotAccess"
     ):
-        raise BranchNotFoundError("SQL", "SQL")
+        raise BranchNotFoundError(
+            response.json()["parameters"]["datasetRid"],
+            _extract_branch_from_sql_error(response),
+        )
     if (
-        response.status_code == 400
+        response.status_code == requests.codes.bad
         and response.json()["errorName"]
         == "FoundrySqlServer:InvalidDatasetPathNotFound"
     ):
-        raise DatasetNotFoundError("SQL")
+        raise DatasetNotFoundError(response.json()["parameters"]["path"])
 
 
-def _is_palantir_oauth_client_installed():
+def _extract_branch_from_sql_error(response):
     try:
-        # pylint: disable=import-outside-toplevel,unused-import,import-error
-        import palantir_oauth_client
-
-        return palantir_oauth_client
-    except ImportError:
-        try:
-            # pylint: disable=import-outside-toplevel,import-error
-            import pyfoundry_auth
-
-            warnings.warn(
-                "\nPyFoundry Auth has been renamed to Palantir Oauth Client\n"
-                "Please uninstall pyfoundry-auth and install palantir-oauth-client\n",
-                DeprecationWarning,
-            )
-            return pyfoundry_auth
-        except ImportError:
-            return False
+        return (
+            response.json()["parameters"]["userFriendlyMessage"]
+            .split("[")[1]
+            .replace("]", "")
+        )
+    except Exception as e:
+        print(e, file=sys.stderr)
+        return None
 
 
 def _raise_for_status_verbose(response: requests.Response):
     """Executes response.raise_for_status but shows more info.
 
     Args:
         response (requests.Response): request response
@@ -1933,16 +2058,16 @@
             LOGGER.debug(
                 "%s %s %s",
                 response.request.method,
                 response.url,
                 response.headers["Server-Timing"],
             )
     except requests.exceptions.HTTPError as error:
-        print(error)
-        print(error.response.text)
+        print(error, file=sys.stderr)
+        print(error.response.text, file=sys.stderr)
         raise error
 
 
 def _determine_requests_verify_value(config):
     if "requests_ca_bundle" in config:
         return config["requests_ca_bundle"]
     return True
@@ -1959,15 +2084,14 @@
         maxsize (int): Maximum size of the LRU cache (a functools.lru_cache argument)
 
     Returns:
         decorated:
     """
 
     def deco(wrapped_function):
-        # pylint: disable=unused-argument
         @functools.lru_cache(maxsize=maxsize)
         def cached_with_ttl(*args, ttl_hash, **kwargs):
             return wrapped_function(*args, **kwargs)
 
         def inner(*args, **kwargs):
             return cached_with_ttl(
                 *args, ttl_hash=round(time.time() / ttl_seconds), **kwargs
@@ -2044,15 +2168,15 @@
             'expires_in': 3600,
             'token_type': 'bearer'
        }
 
     """
     headers = {
         "User-Agent": requests.utils.default_user_agent(
-            f"foundry-dev-tools/{fdt_version}/python-requests"
+            f"foundry-dev-tools/{FDT_VERSION}/python-requests"
         ),
         "Authorization": "Basic "
         + base64.b64encode(bytes(client_id + ":" + client_secret, "ISO-8859-1")).decode(
             "ascii"
         ),
         "Content-Type": "application/x-www-form-urlencoded",
     }
@@ -2066,45 +2190,44 @@
     )
     _raise_for_status_verbose(response)
     return response.json()
 
 
 @lru_with_ttl(ttl_seconds=3600)
 def _get_palantir_oauth_token(
-    foundry_url: str, client_id: str, client_secret: str = None
+    foundry_url: str, client_id: str, client_secret: "str | None" = None
 ) -> str:
-    if oauth_provider := _is_palantir_oauth_client_installed():
-        credentials = oauth_provider.get_user_credentials(
-            scopes=[
-                "offline_access",
-                "compass:view",
-                "compass:edit",
-                "compass:discover",
-                "api:write-data",
-                "api:read-data",
-            ],
-            hostname=foundry_url,
-            client_id=client_id,
-            client_secret=client_secret,
-            use_local_webserver=False,
-        )
-
-    else:
-        raise ValueError(
-            "You provided a 'client_id' for Foundry SSO but "
-            "palantir-oauth-client is not installed.\n"
-        )
+    credentials = palantir_oauth_client.get_user_credentials(
+        scopes=[
+            "offline_access",
+            "compass:view",
+            "compass:edit",
+            "compass:discover",
+            "api:write-data",
+            "api:read-data",
+        ],
+        hostname=foundry_url,
+        client_id=client_id,
+        client_secret=client_secret,
+        use_local_webserver=False,
+    )
 
     return credentials.token
 
 
 def _request(*args, **kwargs):
-    kwargs["timeout"] = 599
-    # pylint: disable=missing-timeout
-    return requests.request(*args, **kwargs)
+    if "read_timeout" in kwargs:
+        read_timeout = kwargs["read_timeout"]
+        del kwargs["read_timeout"]
+        return requests.request(
+            *args,
+            **kwargs,
+            timeout=(DEFAULT_REQUESTS_CONNECT_TIMEOUT, read_timeout),
+        )
+    return requests.request(*args, **kwargs, timeout=DEFAULT_REQUESTS_CONNECT_TIMEOUT)
 
 
 class FoundryDevToolsError(Exception):
     """Metaclass for :class:`FoundryAPIError` and :class:`foundry_dev_tools.fsspec_impl.FoundryFileSystemError`.
 
     Catch all foundry_dev_tools errors:
 
@@ -2139,25 +2262,25 @@
 
 class DatasetHasNoSchemaError(FoundryAPIError):
     """Exception is thrown when dataset has no associated schema."""
 
     def __init__(
         self,
         dataset_rid: str,
-        transaction_rid: Optional[str] = None,
-        branch: Optional[str] = None,
-        response: Optional[requests.Response] = None,
+        transaction_rid: "str | None" = None,
+        branch: "str | None" = None,
+        response: "requests.Response | None" = None,
     ):
         """Pass parameters to constructor for later use and uniform error messages.
 
         Args:
              dataset_rid (str): dataset which has no schema
-             transaction_rid (Optional[str]): transaction_rid if available
-             branch (Optional[str]): dataset branch if available
-             response (Optional[requests.Response]): requests response if available
+             transaction_rid (str | None): transaction_rid if available
+             branch (str | None): dataset branch if available
+             response (requests.Response | None): requests response if available
         """
         super().__init__(
             f"Dataset {dataset_rid} "
             + (
                 f"on transaction {transaction_rid} "
                 if transaction_rid is not None
                 else ""
@@ -2175,24 +2298,24 @@
 class BranchNotFoundError(FoundryAPIError):
     """Exception is thrown when no transaction exists for a dataset in a specific branch."""
 
     def __init__(
         self,
         dataset_rid: str,
         branch: str,
-        transaction_rid: Optional[str] = None,
-        response: Optional[requests.Response] = None,
+        transaction_rid: "str | None" = None,
+        response: "requests.Response | None" = None,
     ):
         """Pass parameters to constructor for later use and uniform error messages.
 
         Args:
              dataset_rid (str): dataset_rid for the branch that does not exist
              transaction_rid (str): transaction_rid if available
-             branch (Optional[str]): dataset branch
-             response (Optional[requests.Response]): requests response if available
+             branch (str | None): dataset branch
+             response (requests.Response | None): requests response if available
         """
         super().__init__(
             f"Dataset {dataset_rid} "
             + (
                 f"on transaction {transaction_rid}"
                 if transaction_rid is not None
                 else ""
@@ -2209,41 +2332,41 @@
 class BranchesAlreadyExistError(FoundryAPIError):
     """Exception is thrown when branch exists already."""
 
     def __init__(
         self,
         dataset_rid: str,
         branch_rid: str,
-        response: Optional[requests.Response] = None,
+        response: "requests.Response | None" = None,
     ):
         """Pass parameters to constructor for later use and uniform error messages.
 
         Args:
              dataset_rid (str): dataset_rid for the branch that already exists
              branch_rid (str): dataset branch which already exists
-             response (Optional[requests.Response]): requests response if available
+             response (requests.Response | None): requests response if available
         """
         super().__init__(
             f"Branch {branch_rid} already exists in {dataset_rid}.\n"
             + (response.text if response is not None else "")
         )
         self.dataset_rid = dataset_rid
         self.branch_rid = branch_rid
         self.response = response
 
 
 class DatasetNotFoundError(FoundryAPIError):
     """Exception is thrown when dataset does not exist."""
 
-    def __init__(self, dataset_rid: str, response: Optional[requests.Response] = None):
+    def __init__(self, dataset_rid: str, response: "requests.Response | None" = None):
         """Pass parameters to constructor for later use and uniform error messages.
 
         Args:
              dataset_rid (str): dataset which can't be found
-             response (Optional[requests.Response]): requests response if available
+             response (requests.Response | None): requests response if available
         """
         super().__init__(
             f"Dataset {dataset_rid} not found.\n"
             + (response.text if response is not None else "")
         )
         self.dataset_rid = dataset_rid
         self.response = response
@@ -2257,59 +2380,58 @@
         self.dataset_rid = dataset_rid
         self.dataset_path = dataset_path
 
 
 class FolderNotFoundError(FoundryAPIError):
     """Exception is thrown when compass folder does not exist."""
 
-    def __init__(self, folder_rid: str, response: Optional[requests.Response] = None):
+    def __init__(self, folder_rid: str, response: "requests.Response | None" = None):
         """Pass parameters to constructor for later use and uniform error messages.
 
         Args:
              folder_rid (str): folder_rid which can't be found
-             response (Optional[requests.Response]): requests response if available
+             response (requests.Response | None): requests response if available
         """
         super().__init__(
             f"Compass folder {folder_rid} not found; "
             f"If you are sure your folder_rid is correct, "
             f"and you have access, check if your jwt token "
             f"is still valid!\n" + (response.text if response is not None else "")
         )
         self.folder_rid = folder_rid
         self.response = response
 
 
 class DatasetHasNoTransactionsError(FoundryAPIError):
     """Exception is thrown when dataset has no transactions."""
 
-    def __init__(self, dataset_rid: str, response: Optional[requests.Response] = None):
+    def __init__(self, dataset_rid: str, response: "requests.Response | None" = None):
         """Pass parameters to constructor for later use and uniform error messages.
 
         Args:
              dataset_rid (str): dataset which has no transactions
-             response (Optional[requests.Response]): requests response if available
+             response (requests.Response | None): requests response if available
         """
         super().__init__(
             f"Dataset {dataset_rid} has no transactions.\n"
             + (response.text if response is not None else "")
         )
         self.dataset_rid = dataset_rid
         self.response = response
 
 
 class DatasetNoReadAccessError(FoundryAPIError):
-    """Exception is thrown when user is missing 'gatekeeper:view-resource' on the dataset,
-    which normally comes with the Viewer role."""
+    """Exception is thrown when user is missing 'gatekeeper:view-resource' on the dataset, which normally comes with the Viewer role."""  # noqa: E501
 
-    def __init__(self, dataset_rid: str, response: Optional[requests.Response] = None):
+    def __init__(self, dataset_rid: str, response: "requests.Response | None" = None):
         """Pass parameters to constructor for later use and uniform error messages.
 
         Args:
              dataset_rid (str): dataset which can't be read
-             response (Optional[requests.Response]): requests response if available
+             response (requests.Response | None): requests response if available
         """
         super().__init__(
             f"No read access to dataset {dataset_rid}.\n"
             + (response.text if response is not None else "")
         )
         self.dataset_rid = dataset_rid
         self.response = response
@@ -2318,40 +2440,40 @@
 class DatasetHasOpenTransactionError(FoundryAPIError):
     """Exception is thrown when dataset has an open transaction already."""
 
     def __init__(
         self,
         dataset_rid: str,
         open_transaction_rid: str,
-        response: Optional[requests.Response] = None,
+        response: "requests.Response | None" = None,
     ):
         """Pass parameters to constructor for later use and uniform error messages.
 
         Args:
              dataset_rid (str): dataset which has an open transaction
              open_transaction_rid (str): transaction_rid which is open
-             response (Optional[requests.Response]): requests response if available
+             response (requests.Response | None): requests response if available
         """
         super().__init__(
             f"Dataset {dataset_rid} already has open transaction {open_transaction_rid}.\n"
             + (response.text if response is not None else "")
         )
         self.dataset_rid = dataset_rid
         self.open_transaction_rid = open_transaction_rid
         self.response = response
 
 
 class FoundrySqlQueryFailedError(FoundryAPIError):
     """Exception is thrown when SQL Query execution failed."""
 
-    def __init__(self, response: Optional[requests.Response] = None):
+    def __init__(self, response: "requests.Response | None" = None):
         """Pass parameters to constructor for later use and uniform error messages.
 
         Args:
-             response (Optional[requests.Response]): requests response if available
+             response (requests.Response | None): requests response if available
         """
         super().__init__(
             "Foundry SQL Query Failed\n"
             + (response.text if response is not None else "")
         )
         self.response = response
```

### Comparing `foundry-dev-tools-1.0.9/src/foundry_dev_tools/fsspec_impl.py` & `foundry-dev-tools-1.1/src/foundry_dev_tools/fsspec_impl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Module contains the fsspec implementation for Palantir Foundry."""
 import sys
 from datetime import datetime
-from typing import Optional, Union
+from urllib.parse import urlparse
 
 import backoff
 from fs.opener.parse import parse_fs_url
 from fsspec import AbstractFileSystem
 from fsspec.spec import AbstractBufferedFile
 
-from . import FoundryRestClient
-from .foundry_api_client import DatasetHasOpenTransactionError, FoundryDevToolsError
+from foundry_dev_tools.foundry_api_client import (
+    DatasetHasOpenTransactionError,
+    FoundryDevToolsError,
+    FoundryRestClient,
+)
 
 DEFAULT_BRANCH = "master"
 
 
-class FoundryFileSystem(AbstractFileSystem):  # noqa
-    # pylint:disable=abstract-method
+class FoundryFileSystem(AbstractFileSystem):
     """fsspec implementation for the Palantir Foundry Filesystem.
 
     Args:
         dataset (str): dataset_rid or dataset path
         branch (str): dataset branch. Defaults to 'master'.
         token (str): explicitely pass token. By default, FoundryFileSystem gets the token from the configuration file
             or using SSO.
@@ -32,20 +34,19 @@
 
     protocol = "foundry"
 
     def __init__(
         self,
         dataset: str,
         branch: str = DEFAULT_BRANCH,
-        token: str = None,
+        token: "str | None" = None,
         transaction_backoff: bool = True,
         skip_instance_cache: bool = False,
         **kwargs,
     ):
-        # pylint: disable=too-many-arguments
         super().__init__(skip_instance_cache=skip_instance_cache, **kwargs)
         self.token = token
         self.dataset_identity = self.api.get_dataset_identity(
             dataset_path_or_rid=dataset, branch=branch
         )
         self.dataset_identity["branch"] = branch
         self.transaction_rid = None
@@ -64,56 +65,49 @@
 
         """
         if self.token:
             return FoundryRestClient({"jwt": self.token})
         return FoundryRestClient()
 
     @classmethod
-    def _strip_protocol(cls, path):
+    def _strip_protocol(cls, path: str):
         """Return only subpath from foundry://<branch>:<token>@<dataset-rid>/<subpath e.g. test.txt>."""
-        if "foundry://" in path:
-            no_foundry = path.lstrip("foundry").lstrip("://")
-            if "/" in no_foundry:
-                return no_foundry[
-                    no_foundry.index("/") + 1 :
-                ]  # everything after dataset_rid/ is the path
-            return ""  # no subpath passed
+        if path.startswith("foundry://"):
+            parsed = urlparse(path)
+            return parsed.path.lstrip("/")
         return path
 
     @staticmethod
     def _get_kwargs_from_urls(path):
         parsed = parse_fs_url(path)
         return_kwargs = {"dataset": parsed.resource.split("/")[0]}
         if "ri.foundry.main.dataset" not in return_kwargs["dataset"]:
             raise FoundryDatasetPathInUrlNotSupportedError()
-        potential_token = parsed.password if parsed.password != "" else None
+        potential_token = parsed.password if parsed.password else None
         if potential_token:
             return_kwargs["token"] = potential_token
-        potential_branch = (
-            parsed.username if bool(parsed.username and parsed.username != "") else None
-        )
+        potential_branch = parsed.username if parsed.username else None
         if potential_branch:
             return_kwargs["branch"] = potential_branch
         return return_kwargs
 
-    def ls(self, path: str, detail: bool = True, **kwargs):
+    def ls(self, path: str, detail: bool = True, exclude_hidden_files: bool = True):
         """List files in the path specified.
 
         Args:
             path (str): path you want to list
             detail (bool):
                 returns the complete catalog api response, see also
                 :py:meth:`~foundry_dev_tools.foundry_api_client.FoundryRestClient.list_dataset_files`
             exclude_hidden_files (bool): to list also hidden files, set it to false
 
         Returns:
             list:
                 list of files in `path`
         """
-        exclude_hidden_files = kwargs.pop("exclude_hidden_files", True)
         if path in (self.dataset_identity["dataset_path"], "", "**/**", "/."):
             # root
             path = None
         if not self.dataset_identity[
             "last_transaction_rid"
         ]:  # empty dataset, no transaction
             raise FileNotFoundError(path)
@@ -150,15 +144,14 @@
         path,
         mode="rb",
         block_size=None,
         autocommit=True,
         cache_options=None,
         **kwargs,
     ):
-        # pylint: disable=too-many-arguments
         if "cache_type" in kwargs:
             kwargs.pop("cache_type")
         if self._intrans:
             autocommit = False
         return FoundryFile(
             self, path, mode=mode, autocommit=autocommit, cache_type="all", **kwargs
         )
@@ -167,27 +160,27 @@
         """Return the modified timestamp of a file as a datetime.datetime."""
         return datetime.fromisoformat(
             self.info(path)["time_modified"].replace("Z", "+00:00")
         )
 
     def rm(
         self,
-        path: Union[str, list],
+        path: "str | list",
         recursive: bool = False,
-        maxdepth: Optional[int] = None,
+        maxdepth: "int | None" = None,
     ):
         """Delete files.
 
         Args:
             path (Union[str,list]):
                 File(s) to delete.
             recursive (bool):
                 If file(s) are directories, recursively delete contents and then
                 also remove the directory
-            maxdepth (Optional[int]):
+            maxdepth (int | None):
                 Depth to pass to walk for finding files to delete, if recursive.
                 If None, there will be no limit and infinite recursion may be
                 possible.
 
         Raises:
             IsADirectoryError: when recursive is false and the path(s) provided is a directory
             FoundryDeleteInNotSupportedTransactionError:
@@ -205,57 +198,48 @@
         if not self._intrans:
             with self.start_transaction(transaction_type="DELETE") as transaction:
                 self.api.add_files_to_delete_transaction(
                     dataset_rid=self.dataset_identity["dataset_rid"],
                     transaction_id=transaction.transaction_rid,
                     logical_paths=expanded_path,
                 )
-        else:
-            if self.transaction.transaction_type == "DELETE":
-                self.api.add_files_to_delete_transaction(
+        elif self.transaction.transaction_type == "DELETE":
+            self.api.add_files_to_delete_transaction(
+                dataset_rid=self.dataset_identity["dataset_rid"],
+                transaction_id=self._transaction.transaction_rid,
+                logical_paths=expanded_path,
+            )
+        elif self.transaction.transaction_type == "UPDATE":
+            files_created_in_this_transaction = [f.path for f in self.transaction.files]
+            for path_to_delete in reversed(expanded_path):
+                if not any(
+                    bool(path_to_delete in file)
+                    for file in files_created_in_this_transaction
+                ):
+                    raise FoundryDeleteInNotSupportedTransactionError(path_to_delete)
+                self.api.remove_dataset_file(
                     dataset_rid=self.dataset_identity["dataset_rid"],
                     transaction_id=self._transaction.transaction_rid,
-                    logical_paths=expanded_path,
+                    logical_path=path_to_delete,
                 )
-            elif self.transaction.transaction_type == "UPDATE":
-                files_created_in_this_transaction = [
-                    f.path for f in self.transaction.files
-                ]
-                for path_to_delete in reversed(expanded_path):
-                    if not any(
-                        (
-                            bool(path_to_delete in file)
-                            for file in files_created_in_this_transaction
-                        )
-                    ):
-                        raise FoundryDeleteInNotSupportedTransactionError(
-                            path_to_delete
-                        )
-                    self.api.remove_dataset_file(
-                        dataset_rid=self.dataset_identity["dataset_rid"],
-                        transaction_id=self._transaction.transaction_rid,
-                        logical_path=path_to_delete,
-                    )
-            else:
-                raise FoundryDeleteInNotSupportedTransactionError(expanded_path)
+        else:
+            raise FoundryDeleteInNotSupportedTransactionError(expanded_path)
 
     @property
     def transaction(self):
         """A context within which files are committed together upon exit.
 
         Requires the file class to implement `.commit()` and `.discard()`
         for the normal and exception cases.
         """
         if self._transaction is None:
             self._transaction = FoundryTransaction(self)
         return self._transaction
 
-    def start_transaction(
-        self, transaction_type="UPDATE"
-    ):  # pylint: disable=arguments-differ
+    def start_transaction(self, transaction_type="UPDATE"):
         """Begin write transaction for deferring files, non-context version."""
         self._intrans = True
         self._transaction = FoundryTransaction(self, transaction_type=transaction_type)
         return self.transaction
 
 
 class FoundryFile(AbstractBufferedFile):
@@ -273,16 +257,18 @@
         block_size="default",
         autocommit=True,
         cache_type="all",
         cache_options=None,
         size=None,
         **kwargs,
     ):
-        # pylint: disable=too-many-arguments
-        assert cache_type == "all", "Only the AllBytes cache is supported"
+        if cache_type != "all":
+            raise ValueError(
+                "cache_type can only be 'all', Only the AllBytes cache is supported"
+            )
         if "a" in mode:
             raise NotImplementedError(
                 "appending to a file not implemented in FoundryFileSystem"
             )
         super().__init__(
             fs,
             path,
@@ -292,38 +278,42 @@
             cache_type=cache_type,
             cache_options=cache_options or {},
             size=size,
             **kwargs,
         )
 
     def _fetch_range(self, start, end):
-        assert start == 0, "Only reading of the complete file is supported"
+        if start != 0:
+            raise ValueError("Only reading of the complete file is supported")
         return self.fs.api.download_dataset_file(
             dataset_rid=self.fs.dataset_identity["dataset_rid"],
             output_directory=None,
             foundry_file_path=self.path,
             view=self.fs.dataset_identity["branch"],
         )
 
     def _initiate_upload(self):
         """Internal function to start a file upload."""
-        if not self.fs._intrans:  # pylint: disable=protected-access
+        if not self.fs._intrans:
             transaction = self.fs.start_transaction()
             transaction.start()
 
     def _upload_chunk(self, final=False):
         """Internal function to add a chunk of data to a started upload."""
-        assert final is True, "chunked uploading not supported"
+        if not final:
+            raise ValueError("chunked uploading not supported")
         self.buffer.seek(0)
-        assert (
-            self.fs._transaction is not None  # pylint: disable=protected-access
-        ), "multiple threads, same dataset? use skip_instance_cache"
+        if not self.fs._transaction:
+            raise AssertionError(
+                "multiple threads accessing the same dataset? "
+                "use skip_instance_cache when creating the FoundryFileSystem"
+            )
         self.fs.api.upload_dataset_file(
             dataset_rid=self.fs.dataset_identity["dataset_rid"],
-            transaction_rid=self.fs._transaction.transaction_rid,  # pylint: disable=protected-access
+            transaction_rid=self.fs._transaction.transaction_rid,
             path_in_foundry_dataset=self.path,
             path_or_buf=self.buffer,
         )
         if final is True and self.autocommit:
             self.fs.end_transaction()
 
         return False
@@ -334,35 +324,38 @@
 
     See also :class:`foundry_dev_tools.foundry_api_client.FoundryDevToolsError` and
         :class:`foundry_dev_tools.foundry_api_client.FoundryAPIError`
     """
 
 
 class FoundrySimultaneousOpenTransactionError(FoundryFileSystemError):
-    # pylint: disable=missing-class-docstring
+    """Thrown when a dataset already has an open tranasaction."""
+
     def __init__(self, dataset_rid: str, open_transaction_rid):
         super().__init__(
             f"Dataset {dataset_rid} already has open transaction {open_transaction_rid}"
         )
         self.dataset_rid = dataset_rid
         self.open_transaction_rid = open_transaction_rid
 
 
 class FoundryDeleteInNotSupportedTransactionError(FoundryFileSystemError):
-    # pylint: disable=missing-class-docstring
+    """Thrown when trying to delete files in an UPDATE/SNAPSHOT transaction."""
+
     def __init__(self, path: str):
         super().__init__(
             f"You are trying to delete the file(s) {path} while an UPDATE/SNAPSHOT transaction is open. "
             f"Deleting this file(s) is not supported since it was committed in a previous transaction."
         )
         self.path = path
 
 
 class FoundryDatasetPathInUrlNotSupportedError(FoundryFileSystemError):
-    # pylint: disable=missing-class-docstring
+    """Thrown when using the path to a dataset instead of the rid."""
+
     def __init__(self):
         super().__init__(
             "Using the dataset path in the fsspec url is not supported. Please pass the dataset rid, e.g. "
             "foundry://ri.foundry.main.dataset.aaaaaaaa-bbbb-cccc-dddd-eeeeeeeeeeee/<file-path-in-dataset>"
         )
 
 
@@ -406,15 +399,15 @@
             try:
                 self_i.transaction_rid = self_i.fs.api.open_transaction(
                     dataset_rid=self_i.fs.dataset_identity["dataset_rid"],
                     mode=self_i.transaction_type,
                     branch=self_i.fs.dataset_identity["branch"],
                 )
                 self_i.files = []  # clean up after previous failed completions
-                self_i.fs._intrans = True  # pylint: disable=protected-access
+                self_i.fs._intrans = True
             except DatasetHasOpenTransactionError as exception:
                 raise FoundrySimultaneousOpenTransactionError(
                     dataset_rid=exception.dataset_rid,
                     open_transaction_rid=exception.open_transaction_rid,
                 ) from exception
 
         if self.backoff:
@@ -438,15 +431,15 @@
             self.fs.dataset_identity["last_transaction_rid"] = self.transaction_rid
         else:
             self.fs.api.abort_transaction(
                 dataset_rid=self.fs.dataset_identity["dataset_rid"],
                 transaction_id=self.transaction_rid,
             )
         self.files = []
-        self.fs._intrans = False  # pylint: disable=protected-access
+        self.fs._intrans = False
 
 
 def _correct_directories(file_details, subfolder_prefix=""):
     if subfolder_prefix is None:
         subfolder_prefix = ""
     result = []
     visited_folders = []
```

### Comparing `foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/caches/metadata_store.py` & `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/caches/metadata_store.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """A Metadata store for cached datasets.
 
 Primary use is resolution of dataset_path and dataset_Rid for
 offline usage of Foundry DevTools
 """
-# pylint: disable=invalid-name
 import json
 import os.path
-from collections.abc import MutableMapping
+from collections.abc import Iterator, MutableMapping
+from pathlib import Path
 from shutil import rmtree
-from typing import Iterator
 
 
 class DatasetMetadataStore(MutableMapping):
     """A Metadata store for cached datasets.
 
     Primary use is resolution of dataset_path and dataset_rid for
     offline usage of Foundry DevTools
@@ -20,22 +19,22 @@
 
     def __init__(self, cache_dir: str):
         """Init meta data store.
 
         Args:
             cache_dir (str): cache directory path
         """
-        self._cache_dir = cache_dir
-        self._db_path = os.sep.join([self._cache_dir, "metadata.json"])
-        if not os.path.isfile(self._db_path):
+        self._cache_dir = Path(cache_dir)
+        self._db_path = self._cache_dir / "metadata.json"
+        if not self._db_path.is_file():
             # clear cache if metadata.json does not exist
             rmtree(self._cache_dir)
-            os.makedirs(self._cache_dir)
+            self._cache_dir.mkdir(parents=True, exist_ok=True)
             # create empty metadata.json
-            with open(self._db_path, "w", encoding="UTF-8") as file:
+            with self._db_path.open(mode="w", encoding="UTF-8") as file:
                 json.dump({}, file)
 
     def __setitem__(self, dataset_path: str, dataset_identity: dict) -> None:
         db = self._read_db()
         db[dataset_identity["dataset_path"]] = dataset_identity
         self._write_db(db)
 
@@ -51,22 +50,22 @@
         db = self._read_db()
         if dataset_path in db:
             return db[dataset_path]
         raise KeyError(dataset_path)
 
     def __len__(self) -> int:
         db = self._read_db()
-        return len([db[key] for key in db.keys()])
+        return len(db.keys())
 
-    def __iter__(self) -> Iterator[dict]:
+    def __iter__(self) -> "Iterator[dict]":
         db = self._read_db()
         yield from db.keys()
 
     def _read_db(self):
-        with open(self._db_path, "r", encoding="UTF-8") as file:
+        with self._db_path.open(encoding="UTF-8") as file:
             return json.load(file)
 
     def _write_db(self, db):
-        with open(self._db_path, "w", encoding="UTF-8") as file:
+        with self._db_path.open(mode="w", encoding="UTF-8") as file:
             json.dump(db, file, indent=4)
             file.flush()
             os.fsync(file.fileno())
```

### Comparing `foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/caches/spark_caches.py` & `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/caches/spark_caches.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 File based spark cache
 
 """
 import json
 import os
 import shutil
+import sys
 from collections.abc import MutableMapping
 from pathlib import Path
-from typing import Tuple
 
 from foundry_dev_tools.utils.caches.metadata_store import DatasetMetadataStore
 from foundry_dev_tools.utils.converter.foundry_spark import (
     foundry_schema_to_read_options,
     foundry_schema_to_spark_schema,
 )
 from foundry_dev_tools.utils.importer import import_optional_dependency
@@ -24,21 +24,19 @@
 class DiskPersistenceBackedSparkCache(MutableMapping):
     """A cache that stores spark dataframes inside a directory."""
 
     FORMATS = ["parquet", "csv", "unknown"]
     DEFAULT_FORMAT = "parquet"
     STORE_LAST_N_TRANSACTIONS = 2
 
-    def __init__(
-        self, cache_dir: str, clear_cache: bool = False, **kwargs
-    ):  # pylint: disable=unused-argument
+    def __init__(self, cache_dir: str, clear_cache: bool = False, **kwargs):
         self._cache_dir = cache_dir
         if clear_cache:
             shutil.rmtree(self._cache_dir, ignore_errors=True)
-        os.makedirs(self._cache_dir, exist_ok=True)
+        Path(self._cache_dir).mkdir(parents=True, exist_ok=True)
         self.metadata_store = DatasetMetadataStore(self._cache_dir)
 
     def __setitem__(self, key: dict, value: "pyspark.sql.dataframe.DataFrame") -> None:
         _validate_cache_key(key)
         path = self._get_storage_location(key, self.DEFAULT_FORMAT)
         value.write.format(self.DEFAULT_FORMAT).save(path=path, mode="overwrite")
         self.set_item_metadata(path, key, value.schema.jsonValue())
@@ -51,16 +49,16 @@
         Args:
             path (str): direct path to transaction folder, e.g. /.../dss-rid/transaction1.parquet
             dataset_identity (dict): dataset_identity with keys dataset_rid, last_transaction_rid, dataset_path
             schema (dict): spark schema or foundrySchema or None
 
         """
         if schema is not None:
-            with open(
-                os.sep.join([path, "_schema.json"]), "w", encoding="UTF-8"
+            with Path(path).joinpath("_schema.json").open(
+                mode="w", encoding="UTF-8"
             ) as file:
                 json.dump(schema, file)
         self.metadata_store[dataset_identity["dataset_path"]] = dataset_identity
         # cleanup old transactions
         self._cleanup_old_transactions(dataset_identity)
 
     def __delitem__(self, key: dict) -> None:
@@ -91,16 +89,16 @@
         if read_options:
             for dict_key, value in read_options.items():
                 reader = reader.option(dict_key, value)
         return reader.load(os.sep.join([path, "*"]), schema=schema)
 
     def _load_spark_schema(
         self, path: str
-    ) -> Tuple["pyspark.sql.types.StructType", dict]:
-        with open(os.sep.join([path, "_schema.json"]), "r", encoding="UTF-8") as file:
+    ) -> "tuple[pyspark.sql.types.StructType, dict]":
+        with Path(path).joinpath("_schema.json").open(encoding="UTF-8") as file:
             spark_or_foundry_schema = json.load(file)
         if "fieldSchemaList" not in spark_or_foundry_schema:
             legacy_read_options = {"header": "true"}
             return (
                 pyspark.sql.types.StructType.fromJson(spark_or_foundry_schema),
                 legacy_read_options,
             )
@@ -130,16 +128,15 @@
             dataset_identity (dict): with dataset_rid and last_transaction_rid
 
         Returns:
             :py:class:`~str`:
                 path to dataset in cache
 
         """
-        path = get_dataset_path(self.get_cache_dir(), dataset_identity)
-        return path
+        return get_dataset_path(self.get_cache_dir(), dataset_identity)
 
     def get_cache_dir(self) -> str:
         """Returns cache directory.
 
         Returns:
             :py:class:`~str`:
                 path to temporary cache directory
@@ -157,18 +154,19 @@
             :py:class:`~dict`:
                 dataset identity
 
         Raises:
             KeyError: if dataset with dataset_path_or_rid not in cache
 
         """
-        if "ri.foundry.main.dataset" in dataset_path_or_rid:
-            search_key = "dataset_rid"
-        else:
-            search_key = "dataset_path"
+        search_key = (
+            "dataset_rid"
+            if "ri.foundry.main.dataset" in dataset_path_or_rid
+            else "dataset_path"
+        )
         all_cache_entries = self.metadata_store.values()
         maybe_dataset = list(
             filter(
                 lambda dataset_identity: dataset_identity[search_key]
                 == dataset_path_or_rid,
                 all_cache_entries,
             )
@@ -186,35 +184,42 @@
 
         Returns:
             :py:class:`~bool`:
                 if dataset has schema return true
 
         """
         path = get_dataset_path(self.get_cache_dir(), dataset_identity)
-        if os.path.isfile(os.sep.join([path, "_schema.json"])):
+        if Path(path).joinpath("_schema.json").is_file():
             return True
         return False
 
     def _cleanup_old_transactions(self, dataset_identity: dict):
         dataset_root_folder = Path(
             self.get_path_to_local_dataset(dataset_identity)
         ).parent
         all_transactions = [x.name for x in dataset_root_folder.iterdir() if x.is_dir()]
         # transaction rid's are sortable by time
         all_transactions_sorted = sorted(all_transactions, reverse=True)
-        assert (
+        if (
             all_transactions_sorted[0].rsplit(".", 1)[0]
-            == dataset_identity["last_transaction_rid"]
-        ), "Cache dir not in sync with db."
+            != dataset_identity["last_transaction_rid"]
+        ):
+            print(all_transactions_sorted[0], file=sys.stderr)
+            print(dataset_identity["last_transaction_rid"], file=sys.stderr)
+            raise RuntimeError(
+                "Cache dir not in sync with db.\n"
+                f"Please delete the cache dir ({self.get_cache_dir()})"
+                "and restart the transform."
+            )
 
         transaction_to_delete = all_transactions_sorted[
             self.STORE_LAST_N_TRANSACTIONS :
         ]
         for transaction in transaction_to_delete:
-            directory_path = str(
+            directory_path = os.fspath(
                 Path(self.get_cache_dir())
                 / dataset_identity["dataset_rid"]
                 / transaction
             )
             shutil.rmtree(directory_path)
 
 
@@ -240,17 +245,16 @@
             f"Mandatory dict keys are 'dataset_rid', "
             f"'last_transaction_rid' and 'dataset_path'"
         )
 
 
 def _infer_dataset_format(cache_dir: str, dataset_identity: dict):
     path = os.sep.join([cache_dir, dataset_identity["dataset_rid"]])
-    last_transaction_rid = _filter_unknown_files((os.listdir(path)))[0]
-    file_format = last_transaction_rid.split(".")[-1]
-    return file_format
+    last_transaction_rid = _filter_unknown_files(os.listdir(path))[0]
+    return last_transaction_rid.split(".")[-1]
 
 
 def get_dataset_path(cache_dir: str, dataset_identity: dict) -> str:
     """Returns the local directory of the dataset of the last transaction.
 
     Args:
         cache_dir (str): the base directory of the cache
@@ -276,16 +280,16 @@
     path: str, dataset_format="parquet", schema=None, read_options=None
 ) -> "pyspark.sql.DataFrame":
     if dataset_format == "parquet":
         return _read_parquet(path)
     return _read_csv(path, schema=schema, read_options=read_options)
 
 
-def _load_spark_schema(path: str) -> Tuple["pyspark.sql.types.StructType", dict]:
-    with open(os.sep.join([path, "_schema.json"]), "r", encoding="UTF-8") as file:
+def _load_spark_schema(path: str) -> "tuple[pyspark.sql.types.StructType, dict]":
+    with Path(path).joinpath("_schema.json").open(encoding="UTF-8") as file:
         spark_or_foundry_schema = json.load(file)
     if "fieldSchemaList" not in spark_or_foundry_schema:
         legacy_read_options = {"header": "true"}
         return (
             pyspark.sql.types.StructType.fromJson(spark_or_foundry_schema),
             legacy_read_options,
         )
```

### Comparing `foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/converter/foundry_spark.py` & `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/converter/foundry_spark.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """Helper function for conversion of data structures."""
-from typing import Optional
+
+import tempfile
+from typing import TYPE_CHECKING, List
 
 from foundry_dev_tools.utils.importer import import_optional_dependency
 from foundry_dev_tools.utils.spark import get_spark_session
 
 pyspark = import_optional_dependency("pyspark")
 
+if TYPE_CHECKING:
+    import pyarrow as pa
+
 
 def foundry_schema_to_spark_schema(
     foundry_schema: dict,
 ) -> "pyspark.sql.types.StructType":
     """Converts foundry json schema format to spark StructType schema.
 
         See the table below for supported field types:
@@ -50,28 +55,26 @@
 def _parse_fields(fields: list):
     outer_struct_type = {"type": "struct", "fields": []}
     for field in fields:
         outer_struct_type["fields"].append(_parse_field(field))
     return outer_struct_type
 
 
-def _parse_field(field: dict) -> dict:  # pylint: disable=too-many-branches
-    spark_field = {"metadata": field["customMetadata"]}
+def _parse_field(field: dict) -> dict:
+    spark_field = {
+        "metadata": field["customMetadata"],
+        "nullable": True,
+        "type": field["type"].lower(),
+    }
     if "name" in field and field["name"] is not None:
         spark_field["name"] = field["name"]
     if "nullable" in field and field["nullable"] is not None:
         spark_field["nullable"] = field["nullable"]
-    else:
-        # nullable by default True from Foundry
-        spark_field["nullable"] = True
-    if "Noneable" in field:
-        if field["Noneable"] is None:
-            spark_field["nullable"] = True
-        else:
-            spark_field["nullable"] = field["Noneable"]
+    if "Noneable" in field and field["noneable"] is not None:
+        spark_field["nullable"] = field["Noneable"]
     if field["type"] == "DECIMAL":
         spark_field["type"] = f"decimal({field['precision']}, {field['scale']})"
     elif field["type"] == "STRING":
         spark_field["type"] = "string"
     elif field["type"] == "DATE":
         spark_field["type"] = "date"
     elif field["type"] == "STRUCT":
@@ -87,16 +90,14 @@
         map_value_type = _parse_field(field["mapValueType"])
         spark_field["type"] = {
             "type": "map",
             "keyType": _parse_field(field["mapKeyType"])["type"],
             "valueType": map_value_type["type"],
             "valueContainsNull": map_value_type["nullable"],
         }
-    else:
-        spark_field["type"] = field["type"].lower()
     return spark_field
 
 
 def spark_schema_to_foundry_schema(spark_schema, file_format="parquet") -> dict:
     """Converts spark_schema to foundry schema API compatible payload.
 
     Args:
@@ -130,24 +131,24 @@
         foundry_schema["customMetadata"] = {"format": "parquet"}
 
     return foundry_schema
 
 
 def infer_dataset_format_from_foundry_schema(
     foundry_schema: dict, list_of_files: list
-) -> Optional[str]:
+) -> "str | None":
     """Infers dataset format from Foundry Schema dict, looking at key dataFrameReaderClass.
 
     Args:
         foundry_schema (dict): Schema from foundry schema API
         list_of_files (list): files of dataset, as fallback option, first file will be checked
             for file ending
 
     Returns:
-        Optional[str]:
+        str | None:
             parquet, csv or unknown
 
     """
     default_format = "unknown"
     try:
         if "ParquetDataFrameReader" in foundry_schema["dataFrameReaderClass"]:
             default_format = "parquet"
@@ -200,20 +201,20 @@
     new_field["arraySubtype"]["nullable"] = field["type"]["containsNull"]
     if "customMetadata" not in new_field["arraySubtype"]:
         new_field["arraySubtype"]["customMetadata"] = {}
     return new_field
 
 
 def foundry_sql_data_to_spark_dataframe(
-    data: (list, list), spark_schema: "pyspark.sql.types.StructType"
+    data: "List[List]", spark_schema: "pyspark.sql.types.StructType"
 ) -> "pyspark.sql.DataFrame":
     """Converts the result of a foundry sql API query to a spark dataframe.
 
     Args:
-        data (list,list): list of list of data
+        data (List[List]): list of list of data
         spark_schema (:external+spark:py:class:`~pyspark.sql.types.StructType`): the spark schema to apply
 
     Returns:
         :external+spark:py:class:`~pyspark.sql.DataFrame`:
             spark dataframe from foundry sql data
 
     """
@@ -240,15 +241,14 @@
 
     spark_df = get_spark_session().createDataFrame(data, spark_schema)
     for col in timestamp_columns:
         spark_df = spark_df.withColumn(col, pyspark.sql.functions.to_timestamp(col))
     for col in date_columns:
         spark_df = spark_df.withColumn(col, pyspark.sql.functions.to_date(col))
     for col, dtype in decimal_columns.items():
-        # pylint: disable=no-member
         spark_df = spark_df.withColumn(col, pyspark.sql.functions.col(col).cast(dtype))
     return spark_df
 
 
 def foundry_schema_to_read_options(
     foundry_schema: dict,
 ) -> dict:
@@ -310,30 +310,26 @@
         and foundry_schema["customMetadata"]["format"] == "json"
     ):
         return "json"
     raise ValueError(f"Can not infer dataset format for schema {foundry_schema=}")
 
 
 def arrow_stream_to_spark_dataframe(
-    stream_reader: "pyarrow.ipc.RecordBatchStreamReader",
+    stream_reader: "pa.ipc.RecordBatchStreamReader",
 ) -> "pyspark.sql.DataFrame":
     """Dumps an arrow stream to a parquet file in a temporary directory.
 
     And reads the parquet file with spark.
 
     Args:
         stream_reader (:external+pyarrow:py:class:`~pyarrow.ipc.RecordBatchStreamReader`): Arrow Stream
 
     Returns:
         :external+spark:py:class:`~pyspark.sql.DataFrame`:
             converted to a Spark DataFrame
 
     """
-    # pylint: disable=import-outside-toplevel
-    import tempfile
-
-    # pylint: disable=import-outside-toplevel
     import pyarrow.parquet as pq
 
     temporary_parquet_file = f"{tempfile.mkdtemp(suffix='foundry_dev_tools_sql_temp_result_set')}/query-result.parquet"
     pq.write_table(stream_reader.read_all(), temporary_parquet_file, flavor="spark")
     return get_spark_session().read.format("parquet").load(temporary_parquet_file)
```

### Comparing `foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/importer.py` & `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """Helper code inspired by "import_optional_dependency" from pandas.
 
 https://github.com/pandas-dev/pandas/blob/e068f4ca368d1a392d8690b0a3c354503d169914/pandas/compat/_optional.py#L87
 to make pyspark an optional dependency
 """
 import importlib
 from types import ModuleType
-from typing import Optional
 
 
-def import_optional_dependency(name: str, extra: str = "") -> Optional[ModuleType]:
+def import_optional_dependency(name: str, extra: str = "") -> "ModuleType | None":
     """Import an optional dependency.
 
     By default, if a dependency is missing an ImportError with a nice
     message will be raised.
 
     Args:
         name (str): The module name.
         extra (str): Additional text to include in the ImportError message.
 
     Returns:
-        `Optional[ModuleType]`:
+        `ModuleType | None`:
             The imported module, when found.
 
     """
     msg = (
         f"Missing optional dependency '{name}'. {extra} "
         f"Use pip or conda to install {name}."
     )
```

### Comparing `foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/spark.py` & `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/spark.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/token_provider/foundry_token_provider.py` & `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/token_provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Token Provider for common UPTIMIZE AppService."""
 from abc import abstractmethod
-from typing import Optional
 
 from requests.structures import CaseInsensitiveDict
 
-APP_SERVICE_ACCESS_TOKEN_HEADER = "X-Foundry-AccessToken"
+APP_SERVICE_ACCESS_TOKEN_HEADER = "X-Foundry-AccessToken"  # noqa: S105
 
 
 class AbstractTokenProvider:
     """An abstract class for tokenprovider implementations."""
 
     @property
     @abstractmethod
@@ -21,39 +20,37 @@
         Returns:
             str:
                 a unique name for this token provider implementation
         """
         raise NotImplementedError
 
     @abstractmethod
-    def get_token(self) -> Optional[str]:
+    def get_token(self) -> "str | None":
         """This method returns the token from the token provider.
 
         This is an abstract method and needs to be overriden
         by a token provider implementation
 
         Returns:
-            Optional[str]:
+            str | None:
                 the token from the token provider implementation
         """
         raise NotImplementedError
 
 
-class AppServiceStreamlitTokenProvider(
-    AbstractTokenProvider
-):  # pylint: disable=too-few-public-methods,missing-class-docstring
+class AppServiceStreamlitTokenProvider(AbstractTokenProvider):
     """The streamlit token provider."""
 
     config_name = "streamlit"
 
-    def get_token(self) -> Optional[str]:
+    def get_token(self) -> "str | None":
         """Retrieves foundry user token from UPTIMIZE App Service header.
 
         Returns:
-            Optional[str]:
+            str | None:
                 Foundry token or None
         """
         try:
             return self.get_streamlit_request_headers()[APP_SERVICE_ACCESS_TOKEN_HEADER]
         except (ImportError, KeyError, RuntimeError, ModuleNotFoundError, TypeError):
             try:
                 return self.get_streamlit_request_headers_1_14_0()[
@@ -75,15 +72,14 @@
         and stopped working <=1.11.1
 
         Returns:
             :external+tornado:py:class:`tornado.httputil.HTTPHeaders`:
                 request headers
 
         """
-        # pylint: disable=import-outside-toplevel,import-error,protected-access,no-name-in-module
         from streamlit.scriptrunner.script_run_context import get_script_run_ctx
         from streamlit.server.server import Server
 
         session_info = Server.get_current()._get_session_info(
             get_script_run_ctx().session_id
         )
         return session_info.ws.request.headers
@@ -93,32 +89,29 @@
 
         This implementation works starting with streamlit>=1.14.0
 
         Returns:
             :py:class:`~requests.structures.CaseInsensitiveDict`:
                 case-insensitive dict with request headers
         """
-        # pylint: disable=import-outside-toplevel,import-error,protected-access,no-name-in-module
         from streamlit.web.server.websocket_headers import _get_websocket_headers
 
         return CaseInsensitiveDict(_get_websocket_headers())
 
 
-class AppServiceDashTokenProvider(
-    AbstractTokenProvider
-):  # pylint: disable=too-few-public-methods,missing-class-docstring
+class AppServiceDashTokenProvider(AbstractTokenProvider):
     """The flask/dash tokenprovider."""
 
     config_name = "dash"
 
-    def get_token(self) -> Optional[str]:
+    def get_token(self) -> "str | None":
         """Retrieves foundry user token from UPTIMIZE App Service header.
 
         Returns:
-            Optional[str]:
+            str | None:
                 Foundry token or None
 
         """
         try:
             return self.get_flask_request_headers()[APP_SERVICE_ACCESS_TOKEN_HEADER]
         except (ImportError, KeyError, RuntimeError):
             return None
@@ -127,14 +120,18 @@
         """Helper function for the request headers.
 
         Returns:
             :external+werkzeug:py:class:`~werkzeug.datastructures.EnvironHeaders`:
                 flask/dash request headers for the current request
 
         """
-        # pylint: disable=import-outside-toplevel,import-error,protected-access,no-name-in-module
         from flask import request
 
         return request.headers
 
 
 TOKEN_PROVIDERS = [AppServiceStreamlitTokenProvider, AppServiceDashTokenProvider]
+__all__ = [
+    "TOKEN_PROVIDERS",
+    "AppServiceStreamlitTokenProvider",
+    "AppServiceDashTokenProvider",
+]
```

### Comparing `foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/PKG-INFO` & `foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: foundry-dev-tools
-Version: 1.0.9
+Version: 1.1
 Summary: Seamlessly run your Palantir Foundry Repository transforms code on your local machine.
-Home-page: https://github.com/emdgroup/foundry-dev-tools
-Author: Nicolas Renkamp, Jonas Wunderlich
-Author-email: nicolas.renkamp@merckgroup.com, jonas.wunderlich@merckgroup.com
-License: Apache License, Version 2.0
+Author-email: Nicolas Renkamp <nicolas.renkamp@merckgroup.com>, Jonas Wunderlich <jonas.wunderlich@merckgroup.com>
+License: Apache-2.0
+Project-URL: Homepage, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Documentation, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Source, https://github.com/emdgroup/foundry-dev-tools
 Project-URL: Tracker, https://github.com/emdgroup/foundry-dev-tools/issues
 Project-URL: Changelog, https://emdgroup.github.io/foundry-dev-tools/changelog.html
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -20,112 +19,116 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: <4.0,>=3.8
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: integration-testing
+Requires-Python: <4,>=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: integration
 Provides-Extra: testing
 Provides-Extra: transforms
+Provides-Extra: cli
 License-File: LICENSE
 
 <div align="center">
   <br/>
 
-  <a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/ci.yml?style=flat-square"/></img>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/docs.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/docs.yml?style=flat-square"/></img>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/pyversions/foundry-dev-tools?style=flat-square&label=Supported%20Python%20versions&color=%23ffb86c"/></a>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-square&label=PyPI%20version&color=%23bd93f9"/></a>
-  <a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/vn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Version&color=%23bd93f9" alt="Conda Version"/></a>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/dm/foundry-dev-tools?label=PyPI%20Downloads&style=flat-square&color=%236272a4"/></a>
-  <a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/dn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Downloads&color=%236272a4" alt="Conda Downloads"/></a>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/issues"><img src="https://img.shields.io/github/issues/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/pulls"><img src="https://img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
-  <a href="http://www.apache.org/licenses/LICENSE-2.0"><img src="https://shields.io/badge/License-Apache%202.0-green.svg?style=flat-square&color=%234c1"/></a>
+<a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/ci.yml?style=flat-square"/></img>
+<a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/docs.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/docs.yml?style=flat-square"/></img>
+<a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/pyversions/foundry-dev-tools?style=flat-square&label=Supported%20Python%20versions&color=%23ffb86c"/></a>
+<a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-square&label=PyPI%20version&color=%23bd93f9"/></a>
+<a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/vn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Version&color=%23bd93f9" alt="Conda Version"/></a>
+<a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/dm/foundry-dev-tools?label=PyPI%20Downloads&style=flat-square&color=%236272a4"/></a>
+<a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/dn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Downloads&color=%236272a4" alt="Conda Downloads"/></a>
+<a href="https://github.com/emdgroup/foundry-dev-tools/issues"><img src="https://img.shields.io/github/issues/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
+<a href="https://github.com/emdgroup/foundry-dev-tools/pulls"><img src="https://img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
+<a href="http://www.apache.org/licenses/LICENSE-2.0"><img src="https://shields.io/badge/License-Apache%202.0-green.svg?style=flat-square&color=%234c1"/></a>
+
   <p><a href="https://emdgroup.github.io/foundry-dev-tools">Documentation</a></p>
 
-  <a href="https://emdgroup.github.io/foundry-dev-tools/installation.html">Installation<a/>
-  &nbsp;•&nbsp;
-  <a href="https://emdgroup.github.io/foundry-dev-tools/usage_and_examples.html">Usage<a/>
-  &nbsp;•&nbsp;
-  <a href="https://emdgroup.github.io/foundry-dev-tools/develop.html">Development<a/>
+<a href="https://emdgroup.github.io/foundry-dev-tools/installation.html">Installation<a/>
+&nbsp;•&nbsp;
+<a href="https://emdgroup.github.io/foundry-dev-tools/usage_and_examples.html">Usage<a/>
+&nbsp;•&nbsp;
+<a href="https://emdgroup.github.io/foundry-dev-tools/develop.html">Development<a/>
 
 </div>
 
 # Foundry DevTools
 
 Seamlessly run your Palantir Foundry Repository transforms code and more on your local machine.
 Foundry DevTools is a set of useful libraries to interact with the Foundry APIs. There are currently three
 high level entrypoints to Foundry DevTools:
 
-* A [transforms](https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api/) implementation
+- A [transforms](https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api/) implementation
 
-  * An implementation of the Foundry `transforms` package that internally uses the `CachedFoundryClient`.
+  - An implementation of the Foundry `transforms` package that internally uses the `CachedFoundryClient`.
     This allows you to seamlessly run your Palantir Foundry Code Repository transforms code on your local machine.
-    Foundry DevTools does not cover all of Foundry's features, more on this [here](https://emdgroup.github.io/foundry-dev-tools/architecture.html#known-limitations).
+    Foundry DevTools does not cover all of Foundry's features, more on this [here](https://emdgroup.github.io/foundry-dev-tools/architecture.html#known-limitations-contributions-welcome).
 
-* [FoundryRestClient](https://emdgroup.github.io/foundry-dev-tools/FoundryRestClient_usage.html)
+- [FoundryRestClient](https://emdgroup.github.io/foundry-dev-tools/FoundryRestClient_usage.html)
 
-  * An API client that contains an opinionated client implementation to some of Foundry's APIs.
+  - An API client that contains an opinionated client implementation to some of Foundry's APIs.
 
-  * For example:
+  - For example:
 
     ```python
     from foundry_dev_tools import FoundryRestClient
 
     # Queries the Foundry SQL Server with spark SQL dialect
     rest_client = FoundryRestClient()
     df = rest_client.query_foundry_sql("SELECT * FROM `/Global/Foundry Training and Resources/Foundry Reference Project/Ontology Project: Aviation/airlines`", branch='master')
     df.shape
     # Out[2]: (17, 10)
     ```
 
-* [FoundryFileSystem](https://emdgroup.github.io/foundry-dev-tools/FoundryFileSystem_usage.html)
+- [FoundryFileSystem](https://emdgroup.github.io/foundry-dev-tools/FoundryFileSystem_usage.html)
 
-  * An implementation of `fsspec` for Foundry. Useful to interact with Foundry from popular data science libraries such as
-  `pandas` or `dask`.
+  - An implementation of `fsspec` for Foundry. Useful to interact with Foundry from popular data science libraries such as
+    `pandas` or `dask`.
 
-  * For example:
+  - For example:
 
     ```python
     import pandas as pd
     # /Global/Foundry Training and Resources/Foundry Reference Project/Ontology Project: Aviation/airlines
     df = pd.read_parquet("foundry://ri.foundry.main.dataset.5d78f3ae-a588-4fd8-9ba2-66827808c85f")
     df.shape
     # Out[2]: (17, 10)
     ```
 
-
 ## Quickstart
 
 With pip:
+
 ```shell
 pip install foundry-dev-tools
 ```
 
 With conda or mamba on the conda-forge channel:
+
 ```shell
 conda install -c conda-forge foundry-dev-tools
 ```
 
 [Further instructions](https://emdgroup.github.io/foundry-dev-tools/installation.html) can be found in our documentation.
 
 ## Why did we build this?
 
-* Local development experience in your favourite IDE (PyCharm, VSCode, ...)
-    * Access to modern developer tools and workflows such as pylint, black, isort, pre-commit hooks etc.
-* Quicker turnaround time when making changes
-    * Debug, change code and run in a matter of seconds instead of minutes
-* No accidental or auto commits
-    * Keep your git history clean
+- Local development experience in your favourite IDE (PyCharm, VSCode, ...)
+  - Access to modern developer tools and workflows such as pylint, black, isort, pre-commit hooks etc.
+- Quicker turnaround time when making changes
+  - Debug, change code and run in a matter of seconds instead of minutes
+- No accidental or auto commits
+  - Keep your git history clean
 
 # License
+
 Copyright (c) 2023 Merck KGaA, Darmstadt, Germany
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.0.9 Summary:
-Seamlessly run your Palantir Foundry Repository transforms code on your local
-machine. Home-page: https://github.com/emdgroup/foundry-dev-tools Author:
-Nicolas Renkamp, Jonas Wunderlich Author-email: nicolas.renkamp@merckgroup.com,
-jonas.wunderlich@merckgroup.com License: Apache License, Version 2.0 Project-
-URL: Documentation, https://emdgroup.github.io/foundry-dev-tools Project-URL:
-Source, https://github.com/emdgroup/foundry-dev-tools Project-URL: Tracker,
-https://github.com/emdgroup/foundry-dev-tools/issues Project-URL: Changelog,
-https://emdgroup.github.io/foundry-dev-tools/changelog.html Platform: any
-Classifier: Development Status :: 5 - Production/Stable Classifier: Programming
-Language :: Python Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Intended Audience ::
-Developers Classifier: Operating System :: POSIX :: Linux Classifier: Operating
-System :: MacOS Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Scientific/Engineering :: Information Analysis Requires-
-Python: <4.0,>=3.8 Description-Content-Type: text/markdown; charset=UTF-
-8 Provides-Extra: integration-testing Provides-Extra: testing Provides-Extra:
-transforms License-File: LICENSE
+Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.1 Summary: Seamlessly
+run your Palantir Foundry Repository transforms code on your local machine.
+Author-email: Nicolas Renkamp
+renkamp@merckgroup.com>, Jonas Wunderlich
+wunderlich@merckgroup.com> License: Apache-2.0 Project-URL: Homepage, https://
+emdgroup.github.io/foundry-dev-tools Project-URL: Documentation, https://
+emdgroup.github.io/foundry-dev-tools Project-URL: Source, https://github.com/
+emdgroup/foundry-dev-tools Project-URL: Tracker, https://github.com/emdgroup/
+foundry-dev-tools/issues Project-URL: Changelog, https://emdgroup.github.io/
+foundry-dev-tools/changelog.html Platform: any Classifier: Development Status
+:: 5 - Production/Stable Classifier: Programming Language :: Python Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Developers Classifier: Operating System ::
+POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Operating
+System :: Microsoft :: Windows Classifier: Topic :: Scientific/Engineering ::
+Information Analysis Requires-Python: <4,>=3.8 Description-Content-Type: text/
+markdown Provides-Extra: integration Provides-Extra: testing Provides-Extra:
+transforms Provides-Extra: cli License-File: LICENSE
 
  [https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-
                        tools/ci.yml?style=flat-square]
  [https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-
   tools/docs.yml?style=flat-square]_[https://img.shields.io/pypi/pyversions/
                          foundry-dev-tools?style=flat-
      square&label=Supported%20Python%20versions&color=%23ffb86c]_[https://
@@ -39,44 +39,45 @@
                                      â¢ 
                                      Usage
                                      â¢ 
                                   Development
 # Foundry DevTools Seamlessly run your Palantir Foundry Repository transforms
 code and more on your local machine. Foundry DevTools is a set of useful
 libraries to interact with the Foundry APIs. There are currently three high
-level entrypoints to Foundry DevTools: * A [transforms](https://
+level entrypoints to Foundry DevTools: - A [transforms](https://
 www.palantir.com/docs/foundry/transforms-python/transforms-python-api/
-) implementation * An implementation of the Foundry `transforms` package that
+) implementation - An implementation of the Foundry `transforms` package that
 internally uses the `CachedFoundryClient`. This allows you to seamlessly run
 your Palantir Foundry Code Repository transforms code on your local machine.
 Foundry DevTools does not cover all of Foundry's features, more on this [here]
 (https://emdgroup.github.io/foundry-dev-tools/architecture.html#known-
-limitations). * [FoundryRestClient](https://emdgroup.github.io/foundry-dev-
-tools/FoundryRestClient_usage.html) * An API client that contains an
-opinionated client implementation to some of Foundry's APIs. * For example:
-```python from foundry_dev_tools import FoundryRestClient # Queries the Foundry
-SQL Server with spark SQL dialect rest_client = FoundryRestClient() df =
-rest_client.query_foundry_sql("SELECT * FROM `/Global/Foundry Training and
-Resources/Foundry Reference Project/Ontology Project: Aviation/airlines`",
-branch='master') df.shape # Out[2]: (17, 10) ``` * [FoundryFileSystem](https://
-emdgroup.github.io/foundry-dev-tools/FoundryFileSystem_usage.html) * An
-implementation of `fsspec` for Foundry. Useful to interact with Foundry from
-popular data science libraries such as `pandas` or `dask`. * For example:
-```python import pandas as pd # /Global/Foundry Training and Resources/Foundry
-Reference Project/Ontology Project: Aviation/airlines df = pd.read_parquet
-("foundry://ri.foundry.main.dataset.5d78f3ae-a588-4fd8-9ba2-66827808c85f")
-df.shape # Out[2]: (17, 10) ``` ## Quickstart With pip: ```shell pip install
-foundry-dev-tools ``` With conda or mamba on the conda-forge channel: ```shell
-conda install -c conda-forge foundry-dev-tools ``` [Further instructions]
-(https://emdgroup.github.io/foundry-dev-tools/installation.html) can be found
-in our documentation. ## Why did we build this? * Local development experience
-in your favourite IDE (PyCharm, VSCode, ...) * Access to modern developer tools
-and workflows such as pylint, black, isort, pre-commit hooks etc. * Quicker
-turnaround time when making changes * Debug, change code and run in a matter of
-seconds instead of minutes * No accidental or auto commits * Keep your git
+limitations-contributions-welcome). - [FoundryRestClient](https://
+emdgroup.github.io/foundry-dev-tools/FoundryRestClient_usage.html) - An API
+client that contains an opinionated client implementation to some of Foundry's
+APIs. - For example: ```python from foundry_dev_tools import FoundryRestClient
+# Queries the Foundry SQL Server with spark SQL dialect rest_client =
+FoundryRestClient() df = rest_client.query_foundry_sql("SELECT * FROM `/Global/
+Foundry Training and Resources/Foundry Reference Project/Ontology Project:
+Aviation/airlines`", branch='master') df.shape # Out[2]: (17, 10) ``` -
+[FoundryFileSystem](https://emdgroup.github.io/foundry-dev-tools/
+FoundryFileSystem_usage.html) - An implementation of `fsspec` for Foundry.
+Useful to interact with Foundry from popular data science libraries such as
+`pandas` or `dask`. - For example: ```python import pandas as pd # /Global/
+Foundry Training and Resources/Foundry Reference Project/Ontology Project:
+Aviation/airlines df = pd.read_parquet("foundry://
+ri.foundry.main.dataset.5d78f3ae-a588-4fd8-9ba2-66827808c85f") df.shape # Out
+[2]: (17, 10) ``` ## Quickstart With pip: ```shell pip install foundry-dev-
+tools ``` With conda or mamba on the conda-forge channel: ```shell conda
+install -c conda-forge foundry-dev-tools ``` [Further instructions](https://
+emdgroup.github.io/foundry-dev-tools/installation.html) can be found in our
+documentation. ## Why did we build this? - Local development experience in your
+favourite IDE (PyCharm, VSCode, ...) - Access to modern developer tools and
+workflows such as pylint, black, isort, pre-commit hooks etc. - Quicker
+turnaround time when making changes - Debug, change code and run in a matter of
+seconds instead of minutes - No accidental or auto commits - Keep your git
 history clean # License Copyright (c) 2023 Merck KGaA, Darmstadt, Germany
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use
 this file except in compliance with the License. You may obtain a copy of the
 License at https://www.apache.org/licenses/LICENSE-2.0 Unless required by
 applicable law or agreed to in writing, software distributed under the License
 is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied. See the License for the specific language
```

### Comparing `foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/SOURCES.txt` & `foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-.coveragerc
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 tox.ini
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/blank_issue.yml
 .github/ISSUE_TEMPLATE/bug_report.yml
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/feature_request.yml
@@ -16,71 +14,77 @@
 .github/workflows/docs.yml
 docs/Configuration_usage.md
 docs/FoundryFileSystem_usage.md
 docs/FoundryRestClient_usage.md
 docs/SSO_usage.md
 docs/architecture.md
 docs/changelog.md
+docs/cli.md
 docs/conf.py
 docs/contributors.md
 docs/develop.md
 docs/index.md
 docs/installation.md
 docs/license.md
 docs/requirements.txt
 docs/usage_and_examples.md
 docs/_static/.gitignore
 docs/pictures/mermaid-diagram-already-cached-dark.svg
 docs/pictures/mermaid-diagram-already-cached-light.svg
 docs/pictures/mermaid-diagram-new-transaction-dark.svg
 docs/pictures/mermaid-diagram-new-transaction-light.svg
 docs/pictures/tpa_config.png
-src/__init__.py
 src/foundry_dev_tools/__init__.py
 src/foundry_dev_tools/cached_foundry_client.py
 src/foundry_dev_tools/config.py
 src/foundry_dev_tools/foundry_api_client.py
 src/foundry_dev_tools/fsspec_impl.py
 src/foundry_dev_tools.egg-info/PKG-INFO
 src/foundry_dev_tools.egg-info/SOURCES.txt
 src/foundry_dev_tools.egg-info/dependency_links.txt
 src/foundry_dev_tools.egg-info/entry_points.txt
 src/foundry_dev_tools.egg-info/not-zip-safe
 src/foundry_dev_tools.egg-info/requires.txt
 src/foundry_dev_tools.egg-info/top_level.txt
+src/foundry_dev_tools/cli/__init__.py
+src/foundry_dev_tools/cli/build.py
+src/foundry_dev_tools/cli/main.py
 src/foundry_dev_tools/utils/__init__.py
 src/foundry_dev_tools/utils/importer.py
+src/foundry_dev_tools/utils/misc.py
+src/foundry_dev_tools/utils/repo.py
 src/foundry_dev_tools/utils/spark.py
+src/foundry_dev_tools/utils/token_provider.py
 src/foundry_dev_tools/utils/caches/__init__.py
 src/foundry_dev_tools/utils/caches/metadata_store.py
 src/foundry_dev_tools/utils/caches/spark_caches.py
 src/foundry_dev_tools/utils/converter/__init__.py
 src/foundry_dev_tools/utils/converter/foundry_spark.py
-src/foundry_dev_tools/utils/token_provider/__init__.py
-src/foundry_dev_tools/utils/token_provider/foundry_token_provider.py
 src/transforms/__init__.py
 src/transforms/api/__init__.py
 src/transforms/api/_configure.py
 src/transforms/api/_dataset.py
 src/transforms/api/_decorators.py
 src/transforms/api/_transform.py
 tests/__init__.py
 tests/conftest.py
 tests/foundry_mock_client.py
 tests/test_cached_foundry_client.py
 tests/test_cached_foundry_client_integration.py
+tests/test_cli_build.py
 tests/test_config.py
 tests/test_foundry_api.py
 tests/test_foundry_local_deprecation.py
 tests/test_foundry_mock.py
 tests/test_foundry_spark_converters.py
 tests/test_foundry_sql_client.py
 tests/test_fsspec_impl.py
 tests/test_importer.py
 tests/test_multipass_tpa.py
 tests/test_spark_caches.py
 tests/test_token_provider.py
 tests/test_transforms.py
 tests/test_transforms_integration.py
+tests/test_utils_repo.py
 tests/utils.py
 tests/test_data/binary_dataset/bin
 tests/test_data/iris/iris.csv
```

### Comparing `foundry-dev-tools-1.0.9/src/transforms/api/__init__.py` & `foundry-dev-tools-1.1/src/transforms/api/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The exposed Function definitions and docstrings is Copyright © 2023 Palantir Technologies Inc. and/or affiliates (“Palantir”). All rights reserved.
 
 https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api/
 https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api-classes/
 
-"""  # pylint: disable=line-too-long
+"""  # noqa: E501
 
 from ._configure import configure
 from ._dataset import Input, Markings, OrgMarkings, Output
 from ._decorators import incremental, transform, transform_df, transform_pandas
 from ._transform import TransformContext
 
 __all__ = (
```

### Comparing `foundry-dev-tools-1.0.9/src/transforms/api/_dataset.py` & `foundry-dev-tools-1.1/src/transforms/api/_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 """The exposed Function definitions and docstrings is Copyright © 2023 Palantir Technologies Inc. and/or affiliates (“Palantir”). All rights reserved.
 
 https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api/
 https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api-classes/
 
-"""  # pylint: disable=line-too-long
+"""  # noqa: E501
 
 import inspect
 import logging
-import pathlib
 import warnings
-from os import getcwd, path
-from subprocess import CalledProcessError
-from typing import Any, List, Optional, Tuple, Union
+from pathlib import Path
+from typing import Any
 
 import pyspark
 
-import foundry_dev_tools
-from foundry_dev_tools import CachedFoundryClient
-from foundry_dev_tools.config import execute_as_subprocess
+import foundry_dev_tools.config
+from foundry_dev_tools.cached_foundry_client import CachedFoundryClient
 from foundry_dev_tools.foundry_api_client import (
     BranchNotFoundError,
     DatasetHasNoSchemaError,
+    DatasetHasNoTransactionsError,
 )
 from foundry_dev_tools.utils.caches.spark_caches import DiskPersistenceBackedSparkCache
+from foundry_dev_tools.utils.repo import git_toplevel_dir
 
 LOGGER = logging.getLogger(__name__)
 
 
-def _as_list(list_or_single_item: Union[None, List[Any], Any]) -> List[Any]:
+def _as_list(list_or_single_item: "list[Any] | Any | None") -> "list[Any]":
     """Helper function turning single values or None into lists.
 
     Args:
-        list_or_single_item (Union[None, List[Any], Any]): item or list to return as a list
+        list_or_single_item (List[Any] | Any | None): item or list to return as a list
 
     Returns:
         list:
             either the single item as a list, or the list passed in list_or_single_item
 
     """
     if not list_or_single_item:
@@ -44,53 +43,52 @@
     return (
         list_or_single_item
         if isinstance(list_or_single_item, list)
         else [list_or_single_item]
     )
 
 
-class Input:  # pylint: disable=too-few-public-methods,too-many-instance-attributes
+class Input:
     """Specification of a transform dataset input.
 
     The actual download is initialized when the Input class is constructed.
     It is currently not lazy loaded.
 
     """
 
     def __init__(
         self,
-        alias: Optional[str] = None,
-        branch: Optional[str] = None,
+        alias: "str | None" = None,
+        branch: "str | None" = None,
         description=None,
         stop_propagating=None,
         stop_requiring=None,
         checks=None,
     ):
-        # pylint: disable=unused-argument,too-many-arguments
         """Specification of a transform dataset input.
 
         Args:
-            alias (Optional[str]): Dataset rid or the absolute Compass path of the dataset.
+            alias (str | None): Dataset rid or the absolute Compass path of the dataset.
                 If not specified, parameter is unbound.
-            branch (Optional[str]): Branch name to resolve the input dataset to.
+            branch (str | None): Branch name to resolve the input dataset to.
                 If not specified, resolved at build-time.
-            stop_propagating (Optional[Markings]): not implemented in Foundry DevTools
-            stop_requiring (Optional[OrgMarkings]): not implemented in Foundry DevTools
+            stop_propagating (Markings | None): not implemented in Foundry DevTools
+            stop_requiring (OrgMarkings | None): not implemented in Foundry DevTools
             checks (List[Check], Check): not implemented in foundry-dev-tools
             description (str): not implemented in foundry-dev-tools
 
         """
         # extract caller filename to retrieve git information
-        caller_filename = inspect.stack()[1].__getattribute__("filename")
+        caller_filename = inspect.stack()[1].filename
         LOGGER.debug("Input instantiated from %s", caller_filename)
-        self.config = foundry_dev_tools.Configuration.get_config()
+        self.config = foundry_dev_tools.config.Configuration.get_config()
         self._cached_client = CachedFoundryClient(self.config)
         self._cache = DiskPersistenceBackedSparkCache(**self.config)
         if branch is None:
-            branch = _get_branch(caller_filename)
+            branch = _get_branch(Path(caller_filename))
 
         if (
             "transforms_freeze_cache" not in self.config
             or self.config["transforms_freeze_cache"] is False
         ):
             self._spark_df, self._dataset_identity, self.branch = self._online(
                 alias, branch
@@ -98,15 +96,15 @@
         else:
             self._spark_df, self._dataset_identity, self.branch = self._offline(
                 alias, branch
             )
 
     def _online(
         self, alias, branch
-    ) -> Tuple[Optional[pyspark.sql.DataFrame], dict, str]:
+    ) -> "tuple[pyspark.sql.DataFrame | None, dict, str]":
         try:
             dataset_identity = self._cached_client.api.get_dataset_identity(
                 alias, branch
             )
         except BranchNotFoundError:
             LOGGER.debug(
                 "Dataset %s not found on branch %s, "
@@ -114,14 +112,16 @@
                 alias,
                 branch,
             )
             branch = "master"
             dataset_identity = self._cached_client.api.get_dataset_identity(
                 alias, branch
             )
+        if dataset_identity["last_transaction_rid"] is None:
+            raise DatasetHasNoTransactionsError(alias)
         if self._dataset_has_schema(dataset_identity, branch):
             return (
                 self._retrieve_spark_df(dataset_identity, branch),
                 dataset_identity,
                 branch,
             )
         LOGGER.debug(
@@ -133,15 +133,15 @@
             branch,
         )
         self._cached_client.fetch_dataset(dataset_identity["dataset_rid"], branch)
         return None, dataset_identity, branch
 
     def _offline(
         self, alias: str, branch: str
-    ) -> Tuple[Optional[pyspark.sql.DataFrame], dict, str]:
+    ) -> "tuple[pyspark.sql.DataFrame | None, dict, str]":
         dataset_identity = self._cache.get_dataset_identity_not_branch_aware(alias)
         if self._cache.dataset_has_schema(dataset_identity):
             return self._cache[dataset_identity], dataset_identity, branch
         return None, dataset_identity, branch
 
     def _dataset_has_schema(self, dataset_identity, branch):
         try:
@@ -164,15 +164,15 @@
             "Returning data for %s on branch %s from cache", dataset_identity, branch
         )
         return self._cache[dataset_identity]
 
     def _read_spark_df_with_sql_query(
         self, dataset_path: str, branch="master"
     ) -> pyspark.sql.DataFrame:
-        query = f"SELECT * FROM `{dataset_path}`"
+        query = f"SELECT * FROM `{dataset_path}`"  # noqa: S608
         if (
             "transforms_sql_sample_select_random" in self.config
             and self.config["transforms_sql_sample_select_random"] is True
         ):
             query = query + " ORDER BY RAND()"
         if (
             "transforms_sql_sample_row_limit" in self.config
@@ -206,15 +206,15 @@
                 dataset_identity["dataset_rid"], branch
             )
         else:
             dataset_name = dataset_identity["dataset_path"].split("/")[-1]
             warnings.warn(
                 f"Retrieving subset ({self.config['transforms_sql_sample_row_limit']} rows) of dataset '{dataset_name}'"
                 f" with rid '{dataset_identity['dataset_rid']}' "
-                f"because dataset size {size_in_mega_bytes_rounded} megabytes > "
+                f"because dataset size {size_in_mega_bytes_rounded} megabytes >= "
                 f"{self.config['transforms_sql_dataset_size_threshold']} megabytes "
                 f"(as defined in config['transforms_sql_dataset_size_threshold'])."
             )
             spark_df = self._read_spark_df_with_sql_query(
                 dataset_identity["dataset_path"], branch
             )
             self._cache[dataset_identity] = spark_df
@@ -236,86 +236,80 @@
             dict:
                 with the keys dataset_path, dataset_rid, last_transaction_rid
 
         """
         return self._dataset_identity
 
 
-def _get_branch(caller_filename: str) -> str:
-    git_dir = path.dirname(caller_filename)
-
-    if git_dir == "" or not path.exists(git_dir):
+def _get_branch(caller_filename: Path) -> str:
+    git_dir = git_toplevel_dir(caller_filename)
+    if not git_dir:
         # fallback for VS Interactive Console
         # or Jupyter lab on Windows
-        git_dir = getcwd()
+        git_dir = Path.cwd()
 
-    try:
-        branch = execute_as_subprocess(
-            ["git", "rev-parse", "--abbrev-ref", "HEAD"], cwd=pathlib.Path(git_dir)
-        )
-    except (FileNotFoundError, CalledProcessError):
-        warnings.warn(
-            "Could not detect git branch of project, falling back to 'master'."
-        )
-        branch = "master"
-    return branch
+    head_file = git_dir.joinpath(".git", "HEAD")
+    if head_file.is_file():
+        with head_file.open() as hf:
+            ref = hf.read().strip()
+
+        if ref.startswith("ref: refs/heads/"):
+            return ref[16:]
 
+        return "HEAD"  # immitate behaviour of `git rev-parse --abbrev-ref HEAD`
 
-class Output:  # pylint: disable=too-few-public-methods
+    warnings.warn("Could not detect git branch of project, falling back to 'master'.")
+    return "master"
+
+
+class Output:
     """Specification of a transform dataset output.
 
     Writing the Output back to Foundry is not implemented.
 
     """
 
     def __init__(
         self,
-        alias: Optional[str] = None,
-        sever_permissions: Optional[bool] = False,
-        description: Optional[str] = None,
+        alias: "str | None" = None,
+        sever_permissions: "bool | None" = False,
+        description: "str | None" = None,
         checks=None,
     ):
-        # pylint: disable=unused-argument,too-many-arguments
         """Specification of a transform output.
 
         Args:
-            alias (Optional[str]): Dataset rid or the absolute Compass path of the dataset.
+            alias (str | None): Dataset rid or the absolute Compass path of the dataset.
                 If not specified, parameter is unbound.
-            sever_permissions (Optional[bool]): not implemented in foundry-dev-tools
-            description (Optional[str]): not implemented in foundry-dev-tools
+            sever_permissions (bool | None): not implemented in foundry-dev-tools
+            description (str | None): not implemented in foundry-dev-tools
             checks (List[Check], Check): not implemented in foundry-dev-tools
         """
         self.alias = alias
 
 
 class UnmarkingDef:
-    # pylint: disable=too-few-public-methods
     """Base class for unmarking datasets configuration."""
 
-    def __init__(
-        self, marking_ids: Union[List[str], str], on_branches: Union[List[str], str]
-    ):
-        # pylint: disable=unused-argument,too-many-arguments
+    def __init__(self, marking_ids: "list[str] | str", on_branches: "list[str] | str"):
         """Default constructor.
 
         Args:
             marking_ids (List[str], str): List of marking identifiers or single marking identifier.
             on_branches (List[str], str): Branch on which to apply unmarking.
         """
         self.marking_ids = _as_list(marking_ids)
         self.branches = _as_list(on_branches)
 
 
 class Markings(UnmarkingDef):
-    # pylint: disable=too-few-public-methods
     """Specification of a marking that stops propagating from input.
 
     The actual marking removal is not implemented.
     """
 
 
 class OrgMarkings(UnmarkingDef):
-    # pylint: disable=too-few-public-methods
     """Specification of a marking that is no longer required on the output.
 
     The actual marking requirement check is not implemented.
     """
```

### Comparing `foundry-dev-tools-1.0.9/src/transforms/api/_decorators.py` & `foundry-dev-tools-1.1/src/transforms/api/_decorators.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """The exposed Function definitions and docstrings is Copyright © 2023 Palantir Technologies Inc. and/or affiliates (“Palantir”). All rights reserved.
 
 https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api/
 https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api-classes/
 
-"""  # pylint: disable=line-too-long
+"""  # noqa: E501
+import warnings
 
-from transforms.api import Input, Output
+from transforms.api._dataset import Input, Output
 from transforms.api._transform import Transform
 
 
 def transform_df(output, **inputs):
     """Register the wrapped compute function as a dataframe transform.
 
     The ``transform_df`` decorator is used to construct a :class:`Transform` object from
     a compute function that accepts and returns :class:`pyspark.sql.DataFrame` objects. Similar
     to the :func:`transform` decorator, the input names become the compute function's parameter
     names. However, a ``transform_df`` accepts only a single :class:`Output` spec as a
     positional argument. The return value of the compute function is also a
     :class:`~pyspark.sql.DataFrame` that is automatically written out to the single output
     dataset.
 
+    >>> from transforms.api import transform_df, Input, Output
     >>> @transform_df(
     ...     Output('/path/to/output/dataset'),  # An unnamed Output spec
     ...     first_input=Input('/path/to/first/input/dataset'),
     ...     second_input=Input('/path/to/second/input/dataset'),
     ... )
     ... def my_compute_function(first_input, second_input):
     ...     # type: (pyspark.sql.DataFrame, pyspark.sql.DataFrame) -> pyspark.sql.DataFrame
@@ -48,14 +50,15 @@
     The ``transform_pandas`` decorator is used to construct a :class:`Transform` object from
     a compute function that accepts and returns :class:`pandas.DataFrame` objects. This
     decorator is similar to the :func:`transform_df` decorator,
     however the :class:`pyspark.sql.DataFrame`
     objects are converted to :class:`pandas.DataFrame` object before the computation,
     and converted back afterwards.
 
+    >>> from transforms.api import transform_pandas, Input, Output
     >>> @transform_pandas(
     ...     Output('/path/to/output/dataset'),  # An unnamed Output spec
     ...     first_input=Input('/path/to/first/input/dataset'),
     ...     second_input=Input('/path/to/second/input/dataset'),
     ... )
     ... def my_compute_function(first_input, second_input):
     ...     # type: (pandas.DataFrame, pandas.DataFrame) -> pandas.DataFrame
@@ -73,14 +76,15 @@
 
     return _transform_pandas
 
 
 def transform(**kwargs):
     """Wrap up a compute function as a Transform object.
 
+    >>> from transforms.api import transform, Input, Output
     >>> @transform(
     ...     first_input=Input('/path/to/first/input/dataset'),
     ...     second_input=Input('/path/to/second/input/dataset'),
     ...     first_output=Output('/path/to/first/output/dataset'),
     ...     second_output=Output('/path/to/second/output/dataset'),
     ... )
     ... def my_compute_function(first_input, second_input, first_output, second_output):
@@ -108,28 +112,24 @@
 
 def incremental(
     require_incremental=False,
     semantic_version=1,
     snapshot_inputs=None,
     allow_retention=False,
 ):
-    # pylint: disable=unused-argument
     """Not implemented in local.
 
     Args:
-        require_incremental:
-        semantic_version:
-        snapshot_inputs:
-        allow_retention:
+        require_incremental: not implemented
+        semantic_version: not implemented
+        snapshot_inputs: not implemented
+        allow_retention: not implemented
 
     Returns:
         _transform:
     """
-    # pylint: disable=import-outside-toplevel
-    import warnings
-
     warnings.warn("@incremental functionality not implemented in Foundry DevTools")
 
     def _transform(compute_func):
         return compute_func
 
     return _transform
```

### Comparing `foundry-dev-tools-1.0.9/src/transforms/api/_transform.py` & `foundry-dev-tools-1.1/src/transforms/api/_transform.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 """The exposed Function definitions and docstrings is Copyright © 2023 Palantir Technologies Inc. and/or affiliates (“Palantir”). All rights reserved.
 
 https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api/
 https://www.palantir.com/docs/foundry/transforms-python/transforms-python-api-classes/
 
-"""  # pylint: disable=line-too-long
+"""  # noqa: E501
 
 import collections
 import inspect
 import os
 import re
-from typing import Callable, Dict, Optional
+from collections.abc import Callable
+from os import PathLike
+from pathlib import Path
 
 import fs
 import pyspark
 
-from transforms.api import Input, Output
-
-import foundry_dev_tools
+import foundry_dev_tools.config
 from foundry_dev_tools.utils.caches.spark_caches import get_dataset_path
 from foundry_dev_tools.utils.spark import get_spark_session
+from transforms.api._dataset import Input, Output
 
 
 class Transform:
     """A Python Transform.
 
     Wraps a function and holds the Input and Output context.
     When the function is called, the Input and Output parameters
     are automatically passed.
     """
 
     def __init__(
         self,
         compute_func: Callable,
-        outputs: Dict[str, Output] = None,
-        inputs: Dict[str, Input] = None,
+        outputs: "dict[str, Output] | None" = None,
+        inputs: "dict[str, Input] | None" = None,
         decorator: str = "spark",
     ):
         """Initialize the `Transform`.
 
         Args:
             compute_func (Callable): The compute function to wrap.
             inputs (Dict[str, Input]): A dictionary mapping input names to :class:`Input` specs.
@@ -55,15 +56,15 @@
 
         for name, tinput in self.inputs.items():
             if not isinstance(tinput, Input):
                 raise ValueError(
                     f"Input '{name}' to transform {self} is not "
                     f"a transforms.api.Input"
                 )
-        for name, toutput in self.outputs.items():
+        for _, toutput in self.outputs.items():
             if not isinstance(toutput, Output):
                 raise ValueError(
                     f"Output '{compute_func.__name__}' of transform {self} is not "
                     f"a transforms.api.Output"
                 )
 
         self._use_context = "ctx" in inspect.getfullargspec(compute_func).args
@@ -72,25 +73,25 @@
         """Passthrough call to the underlying compute function."""
         try:
             return self._compute_func(*args, **kwargs)
         except Exception as exc:
             setattr(exc, "__transform_compute_error", True)
             raise
 
-    def compute(self):  # pylint: disable=arguments-differ
+    def compute(self):
         """Execute the wrapped transform function."""
         if self._type == "pandas":
             return self._compute_pandas()
         if self._type == "transform":
             return self._compute_transform()
         return self._compute_spark()
 
     def _compute_spark(
         self,
-    ) -> "pyspark.sql.DataFrame":  # pylint: disable=arguments-differ
+    ) -> "pyspark.sql.DataFrame":
         """Execute the wrapped transform function.
 
         Returns:
             :external+spark:py:class:`~pyspark.sql.DataFrame`:
                 the result of the transforms function
 
         """
@@ -103,28 +104,28 @@
         if not isinstance(output_df, pyspark.sql.DataFrame):
             raise ValueError(
                 f"Expected {self} to return a pyspark.sql.DataFrame, instead got {output_df}"
             )
 
         return output_df
 
-    def _compute_pandas(self):  # pylint: disable=arguments-differ
+    def _compute_pandas(self):
         """Execute the wrapped transform function.
 
         Returns:
             :external+spark:py:class:`~pyspark.sql.DataFrame`:
                 the result of the transforms function
 
         """
         kwargs = {name: i.dataframe().toPandas() for name, i in self.inputs.items()}
         if self._use_context:
             kwargs["ctx"] = TransformContext()
 
         output_df = self(**kwargs)
-        import pandas as pd  # pylint: disable=import-outside-toplevel
+        import pandas as pd
 
         if not isinstance(output_df, pd.DataFrame):
             raise ValueError(
                 f"Expected {self} to return a pandas.DataFrame, instead got {output_df}"
             )
 
         return output_df
@@ -144,15 +145,15 @@
             kwargs["ctx"] = TransformContext()
 
         self(**kwargs)
 
         return {name: i.dataframe() for name, i in outputs.items()}
 
 
-class TransformContext:  # pylint: disable=too-few-public-methods
+class TransformContext:
     """The TransformContext is passed to the transform function if ctx is the first argument."""
 
     def __init__(self):
         pass
 
     @property
     def spark_session(self) -> pyspark.sql.SparkSession:
@@ -169,15 +170,14 @@
         """Not implemented.
 
         Returns:
             bool:
                 false, as it is not implemented
 
         """
-        # pylint: disable=import-outside-toplevel
         import warnings
 
         warnings.warn(
             "is_incremental functionality not implemented in Foundry DevTools"
         )
         return False
 
@@ -216,15 +216,16 @@
 
         Returns:
             FileSystem:
                 A `FileSystem` object for reading from `Foundry`.
         """
         return FileSystem(
             base_path=get_dataset_path(
-                foundry_dev_tools.Configuration["cache_dir"], self._dataset_identity
+                foundry_dev_tools.config.Configuration["cache_dir"],
+                self._dataset_identity,
             )
         )
 
 
 class TransformOutput:
     """The output object passed into Transform objects at runtime."""
 
@@ -238,26 +239,25 @@
         self._fs = None
         self._df = None
         self._argument_name = argument_name
         self.branch = "no-implemented-in-foundry-dev-tools"
         self.path = output.alias
         self.rid = "no-implemented-in-foundry-dev-tools"
 
-    def dataframe(self) -> Optional[pyspark.sql.DataFrame]:
+    def dataframe(self) -> "pyspark.sql.DataFrame | None":
         """Returns pyspark DataFrame.
 
         Returns:
             :external+spark:py:class:`~pyspark.sql.DataFrame`:
                 the dataframe of this output or None
 
         """
         return self._df
 
     def write_dataframe(self, df: pyspark.sql.DataFrame, **kwargs):
-        # pylint: disable=invalid-name, unused-argument
         """Storing dataframe as variable.
 
         Args:
             df (:external+spark:py:class:`~pyspark.sql.DataFrame`): spark dataframe
             **kwargs: unused
 
         """
@@ -268,22 +268,19 @@
 
         Args:
             pandas_df (pandas.DataFrame): The dataframe to write.
         """
         return self.write_dataframe(get_spark_session().createDataFrame(pandas_df))
 
     def _make_filesystem(self):
-        if "transforms_output_folder" in foundry_dev_tools.Configuration:
-            base_path = os.sep.join(
-                [
-                    foundry_dev_tools.Configuration["transforms_output_folder"],
-                    self._argument_name,
-                ]
-            )
-            os.makedirs(base_path, exist_ok=True)
+        if "transforms_output_folder" in foundry_dev_tools.config.Configuration:
+            base_path = Path(
+                foundry_dev_tools.config.Configuration["transforms_output_folder"]
+            ).joinpath(self._argument_name)
+            base_path.mkdir(parents=True, exist_ok=True)
             return FileSystem(base_path=base_path)
         return FileSystem()
 
     def filesystem(self):
         """Returns a temporary filesystem for the output that can be written to.
 
         Returns:
@@ -304,30 +301,30 @@
 class FileStatus(collections.namedtuple("FileStatus", ["path", "size", "modified"])):
     """A :class:`collections.namedtuple` capturing details about a `FoundryFS` file."""
 
 
 class FileSystem:
     """File System for TransformOutput and TransformInput."""
 
-    def __init__(self, base_path=None):
+    def __init__(self, base_path: "str | PathLike | None" = None):
         if base_path:
-            self._fs = fs.open_fs(base_path)
+            self._fs = fs.open_fs(os.fspath(base_path))
         else:
             self._fs = fs.open_fs("mem://")
 
     def ls(
-        self, glob: Optional[str] = None, regex: str = ".*", show_hidden: bool = False
-    ):  # pylint: disable=invalid-name
+        self, glob: "str | None" = None, regex: str = ".*", show_hidden: bool = False
+    ):
         """Recurses through all directories and lists all files matching the given patterns.
 
         Starting from the root directory of the dataset.
 
         Args:
-            glob (Optional[str]): A unix file matching pattern. Also supports globstar.
-            regex (Optional[str]): A regex pattern against which to match filenames.
+            glob (str | None): A unix file matching pattern. Also supports globstar.
+            regex (str | None): A regex pattern against which to match filenames.
             show_hidden (bool): Include hidden files, those prefixed with '.' or '_'.
 
         Yields:
             :class:`~transforms.api.FileStatus`:
                 The logical path, file size (bytes),
                 modified timestamp (ms since January 1, 1970 UTC)
         """
@@ -335,24 +332,23 @@
             # need to remove trailing slash
             result = [glob.path[1:] for glob in self._fs.glob(glob)]
         else:
             result = [file[1:] for file in self._fs.walk.files(path="/")]
         pattern = re.compile(regex)
         result_after_regex_match = [s for s in result if pattern.match(s)]
         if show_hidden:
-            # pylint: disable=import-outside-toplevel
             import warnings
 
             warnings.warn("argument 'show_hidden' not implemented in foundry_dev_tools")
         for result_path in result_after_regex_match:
             yield FileStatus(
                 result_path, "size not implemented", "modified not implemented"
             )
 
-    def open(self, path, mode="w", **kwargs):
+    def open(self, path, mode="w", **kwargs):  # noqa: A003
         """Open file in this filesystem.
 
         Args:
             path (str): the path to the file
             mode (str): usual file modes
             **kwargs: pass through
```

### Comparing `foundry-dev-tools-1.0.9/tests/conftest.py` & `foundry-dev-tools-1.1/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-# -*- coding: utf-8 -*-
-"""
-    Dummy conftest.py for Foundry DevTools.
+"""Dummy conftest.py for Foundry DevTools.
 
-    If you don't know what this is for, just leave it empty.
-    Read more about conftest.py under:
-    https://pytest.org/latest/plugins.html
+If you don't know what this is for, just leave it empty.
+Read more about conftest.py under:
+https://pytest.org/latest/plugins.html
 """
 import copy
 import os
 import pathlib
 from random import choice
 from string import ascii_uppercase
 
 import fs
 import pytest
 
-import foundry_dev_tools
+import foundry_dev_tools.config
 from foundry_dev_tools.foundry_api_client import DatasetNotFoundError, FoundryRestClient
-
 from tests.test_foundry_mock import MockFoundryRestClient
 from tests.utils import (
     FOUNDRY_SCHEMA_COMPLEX_DATASET,
-    generate_test_dataset,
-    generic_upload_dataset_if_not_exists,
     INTEGRATION_TEST_COMPASS_ROOT_PATH,
     IRIS_SCHEMA,
     TEST_FOLDER,
+    generate_test_dataset,
+    generic_upload_dataset_if_not_exists,
 )
 
 
 def pytest_addoption(parser):
     parser.addoption(
         "--integration",
         action="store_true",
@@ -45,145 +42,129 @@
 def pytest_runtest_setup(item):
     if "integration" in item.keywords and not item.config.getoption("--integration"):
         pytest.skip("need --integration option to run this test")
     if "performance" in item.keywords and not item.config.getoption("--performance"):
         pytest.skip("need --performance option to run this test")
 
 
-def pytest_configure(config):
-    config.addinivalue_line(
-        "markers", "integration: mark test to run only integration tests"
-    )
-    config.addinivalue_line(
-        "markers", "performance: mark test to run only performance tests"
-    )
-
-
 def pytest_generate_tests(metafunc):
     if "is_integration_test" in metafunc.fixturenames:
-        if metafunc.config.getoption("--integration"):
-            is_integration_test = True
-        else:
-            is_integration_test = False
+        is_integration_test = bool(metafunc.config.getoption("--integration"))
         metafunc.parametrize("is_integration_test", [is_integration_test])
 
 
 class PatchConfig:
     def __init__(
         self,
-        config_overwrite: dict = None,
-        initial_config_overwrite: dict = None,
+        config_overwrite: "dict | None" = None,
+        initial_config_overwrite: "dict | None" = None,
         read_initial: bool = False,
     ):
         self.initial_config_overwrite = initial_config_overwrite
         self.config_overwrite = config_overwrite
         self.read_initial = read_initial
+        self.conf_save = None
 
     def __enter__(self):
         self.conf_save = override_config(
             initial_config_overwrite=self.initial_config_overwrite,
             config_overwrite=self.config_overwrite,
             read_initial=self.read_initial,
         )
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        (
-            foundry_dev_tools.INITIAL_CONFIG,
-            foundry_dev_tools.FOUNDRY_DEV_TOOLS_DIRECTORY,
-        ) = self.conf_save[0]
-        foundry_dev_tools.Configuration = self.conf_save[1]
+        if self.conf_save:
+            (
+                foundry_dev_tools.config.INITIAL_CONFIG,
+                foundry_dev_tools.config.FOUNDRY_DEV_TOOLS_DIRECTORY,
+            ) = self.conf_save[0]
+            foundry_dev_tools.config.Configuration = self.conf_save[1]
 
 
 def override_config(
-    initial_config_overwrite: dict = None,
-    config_overwrite: dict = None,
+    initial_config_overwrite: "dict | None" = None,
+    config_overwrite: "dict | None" = None,
     read_initial=False,
-) -> (
-    (dict, dict, pathlib.Path),
-    foundry_dev_tools.config.Config,
-    foundry_dev_tools.config.Config,
-):
+) -> "tuple[tuple[dict, pathlib.Path], foundry_dev_tools.config.Config]":
     save = (
-        copy.deepcopy(foundry_dev_tools.INITIAL_CONFIG),
-        copy.deepcopy(foundry_dev_tools.FOUNDRY_DEV_TOOLS_DIRECTORY),
+        copy.deepcopy(foundry_dev_tools.config.INITIAL_CONFIG),
+        copy.deepcopy(foundry_dev_tools.config.FOUNDRY_DEV_TOOLS_DIRECTORY),
     )
     if read_initial:
         (
-            foundry_dev_tools.INITIAL_CONFIG,
-            foundry_dev_tools.FOUNDRY_DEV_TOOLS_DIRECTORY,
+            foundry_dev_tools.config.INITIAL_CONFIG,
+            foundry_dev_tools.config.FOUNDRY_DEV_TOOLS_DIRECTORY,
         ) = foundry_dev_tools.config.initial_config()
 
     if initial_config_overwrite:
-        foundry_dev_tools.INITIAL_CONFIG.update(
+        foundry_dev_tools.config.INITIAL_CONFIG.update(
             foundry_dev_tools.config.type_convert(initial_config_overwrite)
         )
 
-    config_save = copy.deepcopy(foundry_dev_tools.Configuration)
+    config_save = copy.deepcopy(foundry_dev_tools.config.Configuration)
     if config_overwrite:
-        foundry_dev_tools.Configuration = foundry_dev_tools.config.Config(
+        foundry_dev_tools.config.Configuration = foundry_dev_tools.config.Config(
             config_overwrite
         )
 
     return save, config_save
 
 
 @pytest.fixture(autouse=True)
-def config_for_unit_tests(request, is_integration_test, tmp_path_factory):
+def _config_for_unit_tests(request, is_integration_test, tmp_path_factory):
     if "no_patch_conf" in request.keywords:
         yield
     else:
         rnd = "".join(choice(ascii_uppercase) for _ in range(5))
         temp_directory = tmp_path_factory.mktemp(f"foundry_dev_tools_test_{rnd}")
 
         if not is_integration_test:
             # Mandatory config keys
             with PatchConfig(
                 initial_config_overwrite={
-                    "cache_dir": str(temp_directory),
+                    "cache_dir": os.fspath(temp_directory),
                     "jwt": "123",
                     "foundry_url": "https://stack.palantirfoundry.com",
                 }
             ):
                 yield
         else:
             with PatchConfig(
-                initial_config_overwrite={"cache_dir": str(temp_directory)}
+                initial_config_overwrite={"cache_dir": os.fspath(temp_directory)}
             ):
                 yield
 
 
 @pytest.fixture()
 def client(is_integration_test):
     if is_integration_test:
         yield FoundryRestClient()
     else:
-        test_folder = pathlib.Path(__file__).parent.resolve()
-        root = f"{test_folder}/foundry_mock_root"
-        os.makedirs(root, exist_ok=True)
-        yield MockFoundryRestClient(fs=fs.open_fs(root))
+        root = pathlib.Path(__file__).parent.resolve() / "foundry_mock_root"
+        root.mkdir(parents=True, exist_ok=True)
+        yield MockFoundryRestClient(filesystem=fs.open_fs(os.fspath(root)))
 
 
 @pytest.fixture()
 def iris_dataset(client):
-    iris_dataset = generic_upload_dataset_if_not_exists(
+    return generic_upload_dataset_if_not_exists(
         client=client,
         name="iris_new",
-        upload_folder=str(TEST_FOLDER / "test_data" / "iris"),
+        upload_folder=TEST_FOLDER / "test_data" / "iris",
         foundry_schema=IRIS_SCHEMA,
     )
-    yield iris_dataset
 
 
 @pytest.fixture()
 def iris_no_schema_dataset(client, is_integration_test):
     if is_integration_test:
         iris_dataset = generic_upload_dataset_if_not_exists(
             client=client,
             name="iris_new_no_schema_v1",
-            upload_folder=str(TEST_FOLDER / "test_data" / "iris"),
+            upload_folder=TEST_FOLDER / "test_data" / "iris",
             foundry_schema=None,
         )
         yield iris_dataset
     else:
         yield "iris-rid", "iris-path", "iris_transaction", "iris-branch", False
 
 
@@ -205,14 +186,20 @@
     try:
         identity = client.get_dataset_identity(
             dataset_path_or_rid=ds_path, branch="master"
         )
         yield identity["dataset_rid"]
     except DatasetNotFoundError:
         generate_test_dataset(spark_session, output_folder=tmpdir, n_rows=5000)
-        (ds_rid, _, _, _, _,) = generic_upload_dataset_if_not_exists(
+        (
+            ds_rid,
+            _,
+            _,
+            _,
+            _,
+        ) = generic_upload_dataset_if_not_exists(
             client,
             name=DATASET_NAME,
-            upload_folder=str(tmpdir),
+            upload_folder=tmpdir,
             foundry_schema=FOUNDRY_SCHEMA_COMPLEX_DATASET,
         )
         yield ds_rid
```

### Comparing `foundry-dev-tools-1.0.9/tests/foundry_mock_client.py` & `foundry-dev-tools-1.1/tests/foundry_mock_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import datetime
 import io
 import json
 import os
 import shutil
-from typing import AnyStr, IO, List, Optional, Union
+from pathlib import Path
+from typing import IO, TYPE_CHECKING, AnyStr
 
 import fs
 import timeflake
+from fs.base import FS
 from fs.errors import DirectoryExists, ResourceNotFound
 
-from foundry_dev_tools import FoundryRestClient
 from foundry_dev_tools.foundry_api_client import (
     BranchesAlreadyExistError,
     BranchNotFoundError,
     DatasetHasNoSchemaError,
     DatasetHasOpenTransactionError,
     DatasetNotFoundError,
+    FoundryRestClient,
 )
 from foundry_dev_tools.utils.caches.spark_caches import _read
 from foundry_dev_tools.utils.converter.foundry_spark import (
     foundry_schema_to_dataset_format,
     foundry_schema_to_read_options,
     foundry_schema_to_spark_schema,
 )
 
+if TYPE_CHECKING:
+    import pandas as pd
+    import pyarrow as pa
+    import pyspark
+
 
 class MockFoundryRestClient(FoundryRestClient):
     def query_foundry_sql(
         self, query, branch="master", return_type="pandas"
-    ) -> "pandas.core.frame.DataFrame | pyarrow.Table | pyspark.sql.DataFrame":
+    ) -> "pd.core.frame.DataFrame | pa.Table | pyspark.sql.DataFrame":
         if return_type != "spark":
             raise NotImplementedError
         dataset_path_or_rid = query.split("`")[1]
         row_limit = int(query.split("`")[2].replace("LIMIT", "").strip())
         identity = self.get_dataset_identity(
             dataset_path_or_rid=dataset_path_or_rid, branch=branch
         )
@@ -90,50 +97,51 @@
             ),
             "numHiddenFiles": len(files_with_hidden) - len(files),
             "numTransactions": num_transactions,
         }
 
     def get_dataset_last_transaction_rid(
         self, dataset_rid: str, branch="master"
-    ) -> Optional[str]:
+    ) -> "str | None":
         transactions = self._load_transactions(dataset_rid=dataset_rid)
         if len(transactions) == 0:
             return None
         return transactions[0]["rid"]
 
     def get_dataset_identity(
         self, dataset_path_or_rid: str, branch="master", check_read_access=True
     ):
         if "ri.foundry.main.dataset" in dataset_path_or_rid:
             dataset_path = self._rid_to_fs_path(dataset_path_or_rid)
             dataset_rid = dataset_path_or_rid
         else:
             dataset_path = dataset_path_or_rid
             try:
-                dataset_files = self.fs.listdir(dataset_path)
-            except ResourceNotFound:
-                raise DatasetNotFoundError(dataset_path)
+                dataset_files = self.filesystem.listdir(dataset_path)
+            except ResourceNotFound as e:
+                raise DatasetNotFoundError(dataset_path) from e
             maybe_dataset_rid_file = [
                 file
                 for file in dataset_files
                 if file.startswith(".ri.foundry.main.dataset.")
             ]
             if len(maybe_dataset_rid_file) != 1:
                 raise DatasetNotFoundError(dataset_path_or_rid)
             dataset_rid = fs.path.basename(maybe_dataset_rid_file[0])[1:]
         transactions = self._load_transactions(dataset_rid=dataset_rid)
-        if len(transactions) == 0:
+        if (
+            len(transactions) == 0
+            or len(transactions) == 1
+            and transactions[0]["status"] == "OPEN"
+        ):
             last_transaction_rid = None
+        elif len(transactions) > 1 and transactions[0]["status"] == "OPEN":
+            last_transaction_rid = transactions[1]["rid"]
         else:
-            if len(transactions) == 1 and transactions[0]["status"] == "OPEN":
-                last_transaction_rid = None
-            elif len(transactions) > 1 and transactions[0]["status"] == "OPEN":
-                last_transaction_rid = transactions[1]["rid"]
-            else:
-                last_transaction_rid = transactions[0]["rid"]
+            last_transaction_rid = transactions[0]["rid"]
         return {
             "dataset_path": dataset_path,
             "dataset_rid": dataset_rid,
             "last_transaction_rid": last_transaction_rid,
         }
 
     def _get_transaction(self, dataset_rid: str, transaction_rid: str) -> dict:
@@ -153,15 +161,15 @@
         transaction = self._get_transaction(
             dataset_rid=dataset_rid, transaction_rid=transaction_rid
         )
         _ = self.get_branch(dataset_rid=dataset_rid, branch=branch)
         root_path = self._rid_to_fs_path(transaction_rid)
         if not transaction["schemaRid"]:
             raise DatasetHasNoSchemaError(dataset_rid, transaction_rid, branch)
-        with self.fs.open(
+        with self.filesystem.open(
             fs.path.join(root_path, f".{transaction['schemaRid']}"), "r"
         ) as f:
             return json.load(f)
 
     def upload_dataset_schema(
         self, dataset_rid: str, transaction_rid: str, schema: dict, branch="master"
     ):
@@ -171,101 +179,86 @@
         old_schema_rid = transaction["schemaRid"]
         root_path = self._rid_to_fs_path(transaction_rid)
         schema_rid = self._generate_resource_identifier(
             resource_type="ri.foundry.main.schema"
         )
         transaction["schemaRid"] = schema_rid
         schema_file_path = fs.path.join(root_path, f".{schema_rid}")
-        with self.fs.open(schema_file_path, "w") as f:
+        with self.filesystem.open(schema_file_path, "w") as f:
             json.dump(schema, f)
         self._upsert_transaction(dataset_rid=dataset_rid, transaction=transaction)
         if old_schema_rid:
             old_schema_file_path = fs.path.join(root_path, f".{old_schema_rid}")
-            self.fs.remove(old_schema_file_path)
+            self.filesystem.remove(old_schema_file_path)
 
     def download_dataset_files(
         self,
         dataset_rid: str,
         output_directory: str,
-        files: list = None,
+        files: "list | None" = None,
         view: str = "master",
-        parallel_processes: int = None,
-    ) -> List[str]:
+        parallel_processes: "int | None" = None,
+    ) -> "list[str]":
         return super().download_dataset_files(
             dataset_rid, output_directory, files, view, parallel_processes=1
         )
 
-    def download_dataset_files_temporary(
-        self,
-        dataset_rid: str,
-        files: list = None,
-        view: str = "master",
-        parallel_processes: Optional[int] = None,
-    ) -> str:
-        return super().download_dataset_files_temporary(
-            dataset_rid, files, view, parallel_processes
-        )
-
     def download_dataset_file(
         self,
         dataset_rid: str,
-        output_directory: Optional[str],
+        output_directory: "str | None",
         foundry_file_path: str,
         view: str = "master",
-    ) -> Union[str, bytes]:
+    ) -> "str | bytes":
         # view can be branch or transaction rid
-        if view.startswith("ri.foundry.main.transaction"):
-            transaction_rid = view
-        else:
-            transaction_rid = self.get_branch(dataset_rid=dataset_rid, branch=view)[
-                "transactionRid"
-            ]
+        transaction_rid = (
+            view
+            if view.startswith("ri.foundry.main.transaction")
+            else self.get_branch(dataset_rid=dataset_rid, branch=view)["transactionRid"]
+        )
         root_path = self._rid_to_fs_path(rid=transaction_rid)
         if output_directory:
-            file_directory = fs.path.join(
-                output_directory, fs.path.dirname(foundry_file_path)
-            )
-            os.makedirs(file_directory, exist_ok=True)
-            destination_path = fs.path.join(output_directory, foundry_file_path)
-            with open(destination_path, "wb") as fdst:
-                with self.fs.open(
-                    fs.path.join(root_path, foundry_file_path),
-                    "rb",
-                ) as fsrc:
-                    shutil.copyfileobj(fsrc=fsrc, fdst=fdst)
-            return destination_path
-        else:
-            with self.fs.open(
+            dest_path = Path(output_directory).joinpath(foundry_file_path)
+            dest_path.parent.mkdir(parents=True, exist_ok=True)
+            with dest_path.open("wb") as fdst, self.filesystem.open(
                 fs.path.join(root_path, foundry_file_path),
                 "rb",
             ) as fsrc:
-                return fsrc.read()
+                shutil.copyfileobj(fsrc=fsrc, fdst=fdst)
+            # TODO pathlib
+            return os.fspath(dest_path)
+
+        with self.filesystem.open(
+            fs.path.join(root_path, foundry_file_path),
+            "rb",
+        ) as fsrc:
+            return fsrc.read()
 
     def list_dataset_files(
         self,
         dataset_rid: str,
-        exclude_hidden_files=True,
+        exclude_hidden_files: bool = True,
         view: str = "master",
-        logical_path=None,
-        detail=False,
+        logical_path: "str | None" = None,
+        detail: bool = False,
         *,
         include_open_exclusive_transaction: bool = False,
-        branch: str = None,
+        branch: "str | None" = None,
     ) -> list:
         # view can be branch or transaction rid
         if view.startswith("ri.foundry.main.transaction"):
             transaction_rid = view
         else:
             transaction_rid = self.get_branch(dataset_rid=dataset_rid, branch=view)[
                 "transactionRid"
             ]
         root_path = self._rid_to_fs_path(rid=transaction_rid)
         result = []
 
-        walker = fs.walk.Walker.bind(self.fs)
+        walker = fs.walk.Walker.bind(self.filesystem)
         file_or_folder_infos = list(walker.info(path=root_path, namespaces=["details"]))
         files_info = [
             (
                 file_or_folder[0],
                 file_or_folder[1],
                 file_or_folder[0].replace(root_path + "/", ""),
             )
@@ -287,19 +280,17 @@
         ]
 
         if exclude_hidden_files:
             files_info = [
                 file
                 for file in files_info
                 if not any(
-                    (
-                        part
-                        for part in file[2].split("/")
-                        if (part.startswith(".") or part.startswith("_"))
-                    )
+                    part
+                    for part in file[2].split("/")
+                    if (part.startswith(".") or part.startswith("_"))
                 )
             ]
 
         for file in files_info:
             result.append(
                 {
                     "logicalPath": str(file[2]),
@@ -318,15 +309,15 @@
         return [file["logicalPath"] for file in result]
 
     def upload_dataset_files(
         self,
         dataset_rid: str,
         transaction_rid: str,
         path_file_dict: dict,
-        parallel_processes: int = None,
+        parallel_processes: "int | None" = None,
     ) -> None:
         super().upload_dataset_files(
             dataset_rid, transaction_rid, path_file_dict, parallel_processes=1
         )
 
     def get_dataset_path(self, dataset_rid: str) -> str:
         return self._rid_to_fs_path(rid=dataset_rid)
@@ -368,52 +359,54 @@
         ]
         self._write_branches(dataset_rid=dataset_rid, branches=branches)
 
     def upload_dataset_file(
         self,
         dataset_rid: str,
         transaction_rid,
-        path_or_buf: Union[str, str, IO[AnyStr]],
+        path_or_buf: "str | Path | IO[AnyStr]",
         path_in_foundry_dataset: str,
     ) -> None:
         transaction_path = self._rid_to_fs_path(rid=transaction_rid)
         if path_in_foundry_dataset[0] == "/":
             raise ValueError("path_in_foundry_dataset can not start with /")
         folder_path = fs.path.join(
             transaction_path, fs.path.split(path_in_foundry_dataset)[0]
         )
-        print(folder_path)
         if "/" in path_in_foundry_dataset:
             # check if file exists and is empty, in that case replace with folder
             # can happen with empty s3 keys
-            if self.fs.isfile(folder_path) and self.fs.getsize(folder_path) == 0:
-                self.fs.remove(folder_path)
-            self.fs.makedirs(folder_path, recreate=True)
+            if (
+                self.filesystem.isfile(folder_path)
+                and self.filesystem.getsize(folder_path) == 0
+            ):
+                self.filesystem.remove(folder_path)
+            self.filesystem.makedirs(folder_path, recreate=True)
         binary_flag = ""
         if isinstance(path_or_buf, io.IOBase) and not isinstance(
             path_or_buf, io.TextIOBase
         ):  # heuristic if BytesIO or StringIO ...
             binary_flag = "b"
         if not hasattr(path_or_buf, "read"):  # we read files always in binary mode
             binary_flag = "b"
-        with self.fs.open(
+        with self.filesystem.open(
             fs.path.join(folder_path, fs.path.split(path_in_foundry_dataset)[1]),
             mode=f"w{binary_flag}",
         ) as f:
             if hasattr(path_or_buf, "read"):
                 shutil.copyfileobj(fsrc=path_or_buf, fdst=f)
             else:
-                with open(path_or_buf, mode=f"r{binary_flag}") as fsrc:
+                with open(path_or_buf, mode=f"r{binary_flag}") as fsrc:  # noqa: PTH123
                     shutil.copyfileobj(fsrc=fsrc, fdst=f)
 
     def open_transaction(
         self, dataset_rid: str, mode: str = "SNAPSHOT", branch: str = "master"
     ) -> str:
         # Check if dataset_rid / branch combination exists
-        branch = self.get_branch(dataset_rid=dataset_rid, branch=branch)
+        got_branch = self.get_branch(dataset_rid=dataset_rid, branch=branch)
         # Check if dataset has open transaction
         transactions = self._load_transactions(dataset_rid)
         is_open = [
             transaction
             for transaction in transactions
             if transaction["status"] == "OPEN"
         ]
@@ -421,16 +414,16 @@
             raise DatasetHasOpenTransactionError(
                 dataset_rid=dataset_rid, open_transaction_rid=is_open[0]["rid"]
             )
         rid = self._generate_resource_identifier(
             resource_type="ri.foundry.main.transaction"
         )
         transaction_path = fs.path.join(self._rid_to_fs_path(dataset_rid), rid)
-        self.fs.makedir(transaction_path)
-        with self.fs.open(fs.path.join(transaction_path, f".{rid}"), "w") as f:
+        self.filesystem.makedir(transaction_path)
+        with self.filesystem.open(fs.path.join(transaction_path, f".{rid}"), "w") as f:
             f.write("")
         # I know this does not scale and runs in linear time
         transactions.insert(
             0,
             {
                 "rid": rid,
                 "datasetRid": dataset_rid,
@@ -440,157 +433,158 @@
                 "closeTime": None,
                 "schemaRid": None,
             },
         )
 
         self._write_transactions(dataset_rid, transactions)
         branches = self._load_branches(dataset_rid=dataset_rid)
-        branch["openTransactionRid"] = rid
+        got_branch["openTransactionRid"] = rid
         branches = [
-            branch if branch_inner["id"] == branch["id"] else branch_inner
+            got_branch if branch_inner["id"] == got_branch["id"] else branch_inner
             for branch_inner in branches
         ]
         self._write_branches(dataset_rid=dataset_rid, branches=branches)
         return rid
 
     def _load_transactions(self, dataset_rid: str) -> list:
         dataset_path = self._rid_to_fs_path(rid=dataset_rid)
         dataset_transactions = fs.path.join(dataset_path, ".transactions")
-        if self.fs.exists(dataset_transactions):
-            with self.fs.open(dataset_transactions, "r") as f:
+        if self.filesystem.exists(dataset_transactions):
+            with self.filesystem.open(dataset_transactions, "r") as f:
                 return json.load(f)
         else:
             return []
 
     def _write_transactions(self, dataset_rid: str, transactions: list):
         dataset_path = self._rid_to_fs_path(rid=dataset_rid)
-        with self.fs.open(fs.path.join(dataset_path, ".transactions"), "w") as f:
+        with self.filesystem.open(
+            fs.path.join(dataset_path, ".transactions"), "w"
+        ) as f:
             json.dump(transactions, f)
 
     def _load_branches(self, dataset_rid: str) -> list:
         dataset_path = self._rid_to_fs_path(rid=dataset_rid)
         dataset_branches = fs.path.join(dataset_path, ".branches")
-        if self.fs.exists(dataset_branches):
-            with self.fs.open(dataset_branches, "r") as f:
+        if self.filesystem.exists(dataset_branches):
+            with self.filesystem.open(dataset_branches, "r") as f:
                 return json.load(f)
         else:
             return []
 
     def _write_branches(self, dataset_rid: str, branches: list):
         dataset_path = self._rid_to_fs_path(rid=dataset_rid)
-        with self.fs.open(fs.path.join(dataset_path, ".branches"), "w") as f:
+        with self.filesystem.open(fs.path.join(dataset_path, ".branches"), "w") as f:
             json.dump(branches, f)
 
     def create_branch(
         self,
         dataset_rid: str,
         branch: str,
-        parent_branch: str = None,
-        parent_branch_id: str = None,
+        parent_branch: "str | None" = None,
+        parent_branch_id: "str | None" = None,
     ) -> dict:
         branch_rid = self._generate_resource_identifier(
             resource_type="ri.foundry.main.branch"
         )
         branches = self._load_branches(dataset_rid=dataset_rid)
         does_exists = [
             branch_inner for branch_inner in branches if branch_inner["id"] == branch
         ]
         if len(does_exists) != 0:
             raise BranchesAlreadyExistError(dataset_rid, branch)
-        branch = {
+        ret_branch = {
             "id": branch,
             "rid": branch_rid,
             "ancestorBranchIds": [],
             "creationTime": self._current_datetime(),
             "transactionRid": None,
         }
-        branches.append(branch)
+        branches.append(ret_branch)
         self._write_branches(dataset_rid=dataset_rid, branches=branches)
-        return branch
+        return ret_branch
 
     def get_branch(self, dataset_rid: str, branch: str) -> dict:
         _ = self.get_dataset(dataset_rid)
         branches = self._load_branches(dataset_rid=dataset_rid)
         branch_found = [
             branch_inner for branch_inner in branches if branch_inner["id"] == branch
         ]
         if len(branch_found) == 0:
             raise BranchNotFoundError(dataset_rid, branch)
         return branch_found[0]
 
     def _create_compass_folder_if_not_exists(self, folder_path: str):
-        if not self.fs.exists(folder_path):
-            self.fs.makedir(folder_path)
+        if not self.filesystem.exists(folder_path):
+            self.filesystem.makedir(folder_path)
             rid = self._generate_resource_identifier(
                 resource_type="ri.compass.main.folder"
             )
-            with self.fs.open(fs.path.join(folder_path, f".{rid}"), "w") as f:
+            with self.filesystem.open(fs.path.join(folder_path, f".{rid}"), "w") as f:
                 f.write("")
 
     def _create_parent_compass_folders(self, compass_path):
         split_path = compass_path.split("/")
         suffix = ""
         for i in range(1, len(split_path) - 1):
             suffix = suffix + "/" + split_path[i]
             self._create_compass_folder_if_not_exists(folder_path=suffix)
 
     def create_dataset(self, dataset_path: str) -> dict:
         rid = self._generate_resource_identifier()
         self._create_parent_compass_folders(compass_path=dataset_path)
         try:
-            self.fs.makedir(dataset_path)
+            self.filesystem.makedir(dataset_path)
         except DirectoryExists as exc:
             raise KeyError(f"Dataset '{dataset_path}' already exists.") from exc
-        with self.fs.open(fs.path.join(dataset_path, f".{rid}"), "w") as f:
+        with self.filesystem.open(fs.path.join(dataset_path, f".{rid}"), "w") as f:
             f.write("")
-        return {"rid": rid, "fileSystemId": str(self.fs)}
+        return {"rid": rid, "fileSystemId": str(self.filesystem)}
 
     def get_dataset(self, dataset_rid: str) -> dict:
-        files_count = self.fs.glob(f"**/*.{dataset_rid}").count().files
+        files_count = self.filesystem.glob(f"**/*.{dataset_rid}").count().files
         if files_count == 0:
             raise DatasetNotFoundError(dataset_rid)
         if files_count > 1:
             raise ValueError("This should not happen.")
-        return {"rid": dataset_rid, "fileSystemId": str(self.fs)}
+        return {"rid": dataset_rid, "fileSystemId": str(self.filesystem)}
 
     def delete_dataset(self, dataset_rid: str) -> None:
         dataset_path = self._rid_to_fs_path(rid=dataset_rid)
-        self.fs.removetree(dataset_path)
+        self.filesystem.removetree(dataset_path)
 
-    def __init__(self, fs: "fs.base.FS"):
+    def __init__(self, filesystem: FS):
         super().__init__()
-        self.fs: "fs.base.FS" = fs
-        if str(self.fs) == "<memfs>":
+        self.filesystem: FS = filesystem
+        if str(self.filesystem) == "<memfs>":
             raise ValueError(
                 "<memfs> not supported due to threading issues in multiprocessing."
             )
 
     def _filter_files_in_dataset(self, files: list) -> list:
         filter_1 = [
             file for file in files if not file.startswith(".ri.foundry.main.dataset")
         ]
         filter_2 = [file for file in filter_1 if not file.startswith(".branches")]
-        filter_3 = [
+        return [
             file
             for file in filter_2
             if not file.startswith("ri.foundry.main.transaction")
         ]
-        return filter_3
 
     @staticmethod
     def _generate_resource_identifier(resource_type="ri.foundry.main.dataset"):
         flake = timeflake.random().uuid
-        return f"{resource_type}.{str(flake)}"
+        return f"{resource_type}.{flake!s}"
 
     @staticmethod
     def _current_datetime():
         return datetime.datetime.utcnow().isoformat()[0:23] + "Z"
 
     def _rid_to_fs_path(self, rid: str) -> str:
-        glob_matches = list(self.fs.glob(f"**/*.{rid}"))
+        glob_matches = list(self.filesystem.glob(f"**/*.{rid}"))
         if len(glob_matches) == 0 and "ri.foundry.main.dataset" in rid:
             raise DatasetNotFoundError(rid)
-        elif len(glob_matches) == 0:
+        if len(glob_matches) == 0:
             raise KeyError(rid)
-        elif len(glob_matches) != 1:
+        if len(glob_matches) != 1:
             raise ValueError("This should not happen.")
         return fs.path.split(glob_matches[0].path)[0]
```

### Comparing `foundry-dev-tools-1.0.9/tests/test_cached_foundry_client.py` & `foundry-dev-tools-1.1/tests/test_cached_foundry_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import os
+from pathlib import Path
 from unittest import mock
 from unittest.mock import MagicMock, patch
 
 import fs
 import pandas as pd
 import pytest
 from pandas.testing import assert_frame_equal
 from pyspark.sql import SparkSession
 
-import foundry_dev_tools.config
-from foundry_dev_tools import CachedFoundryClient
+from foundry_dev_tools.cached_foundry_client import CachedFoundryClient
+from foundry_dev_tools.config import Configuration
 from foundry_dev_tools.foundry_api_client import (
     BranchNotFoundError,
     DatasetNotFoundError,
 )
 from foundry_dev_tools.utils.spark import get_spark_session
-
-from tests.test_foundry_mock import MockFoundryRestClient
+from tests.foundry_mock_client import MockFoundryRestClient
 
 DATASET_RID = "ri.foundry.main.dataset.12345de3-b916-46ba-b097-c4326ea4342e"
 DATASET_PATH = "/mock/path/ds1"
 TRANSACTION_RID = "transaction1"
-API = "foundry_dev_tools.FoundryRestClient"
+API = "foundry_dev_tools.foundry_api_client.FoundryRestClient"
 
 
 @pytest.fixture()
 def mock_client(tmpdir):
-    yield MockFoundryRestClient(fs=fs.open_fs(str(tmpdir)))
+    return MockFoundryRestClient(filesystem=fs.open_fs(os.fspath(tmpdir)))
 
 
 def test_config():
     fdt = CachedFoundryClient({"jwt": "secret"})
 
     assert fdt.api._headers()["Authorization"] == "Bearer secret"
     assert fdt.api._requests_verify_value is not None
@@ -61,15 +61,14 @@
         dataset_path_or_rid=DATASET_PATH,
         branch="master",
         exists_ok=True,
         mode="SNAPSHOT",
     )
 
     args = upload_dataset_files.call_args[0]
-    kwargs = upload_dataset_files.call_args[1]
 
     assert args[0] == DATASET_RID
     assert args[1] == TRANSACTION_RID
     # 1 file uploaded
     assert len(args[2]) == 1
 
     assert dataset_rid == "ri.foundry.main.dataset.12345de3-b916-46ba-b097-c4326ea4342e"
@@ -106,15 +105,14 @@
         dataset_path_or_rid=DATASET_PATH,
         branch="master",
         exists_ok=True,
         mode="SNAPSHOT",
     )
 
     args = upload_dataset_files.call_args[0]
-    kwargs = upload_dataset_files.call_args[1]
 
     assert args[0] == DATASET_RID
     assert args[1] == TRANSACTION_RID
     # at least two files uploaded, one parquet and one _SUCCESS
     assert len(args[2]) >= 2
 
     assert dataset_rid == "ri.foundry.main.dataset.12345de3-b916-46ba-b097-c4326ea4342e"
@@ -146,22 +144,20 @@
         dataset_path_or_rid=DATASET_PATH,
         branch="master",
         exists_ok=True,
         mode="SNAPSHOT",
     )
 
     args = upload_dataset_files.call_args[0]
-    kwargs = upload_dataset_files.call_args[1]
 
     assert args[0] == DATASET_RID
     assert args[1] == TRANSACTION_RID
     # one model object should be uploaded
     assert len(args[2]) == 1
-    assert "model.pickle" in args[2].keys()
-    assert "model.pickle" in args[2]["model.pickle"]
+    assert "model.pickle" in args[2]
 
     assert dataset_rid == "ri.foundry.main.dataset.12345de3-b916-46ba-b097-c4326ea4342e"
     assert transaction_id == "transaction1"
 
 
 @patch(API + ".abort_transaction")
 @patch(API + ".create_branch")
@@ -186,15 +182,15 @@
     upload_dataset_schema,
     upload_dataset_files,
     create_dataset,
     create_branch,
     abort_transaction,
 ):
     fdt = CachedFoundryClient()
-    path_file_dict = {"path-in/foundry.pickle": os.getcwd()}
+    path_file_dict = {"path-in/foundry.pickle": Path.cwd()}
 
     # happy path, dataset does not exist!
     get_dataset_identity.side_effect = DatasetNotFoundError("dataset_rid")
     create_dataset.return_value = {"rid": DATASET_RID}
     is_dataset_in_trash.return_value = False
     open_transaction.return_value = TRANSACTION_RID
     dataset_rid, transaction_id = fdt._save_objects(
@@ -210,40 +206,40 @@
     get_dataset_identity.side_effect = None
     get_dataset_identity.return_value = {
         "dataset_rid": DATASET_RID,
         "dataset_path": DATASET_PATH,
     }
 
     # Error in upload files -> verify abort transaction is called
-    upload_dataset_files.side_effect = IOError()
-    with pytest.raises(ValueError):
+    upload_dataset_files.side_effect = OSError()
+    with pytest.raises(ValueError):  # noqa: PT011
         fdt._save_objects(
             path_file_dict,
             DATASET_PATH,
             "master",
             exists_ok=True,
             mode="SNAPSHOT",
         )
     commit_transaction.assert_not_called()
     abort_transaction.assert_called_once()
     upload_dataset_files.side_effect = None
 
     # ValueError is thrown when dataset exists already
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError):  # noqa: PT011
         fdt._save_objects(
             path_file_dict,
             DATASET_PATH,
             "master",
             exists_ok=False,
             mode="SNAPSHOT",
         )
 
     # ValueError is thrown when dataset is in trash
     is_dataset_in_trash.return_value = True
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError):  # noqa: PT011
         fdt._save_objects(
             path_file_dict,
             DATASET_PATH,
             "master",
             exists_ok=True,
             mode="SNAPSHOT",
         )
@@ -282,19 +278,29 @@
     get_dataset_last_transaction_rid,
     is_dataset_in_trash,
     list_dataset_files,
     get_dataset_schema,
     mocker,
 ):
     from_foundry_and_cache = mocker.spy(
-        CachedFoundryClient, "_download_dataset_and_return_local_path"
+        CachedFoundryClient,
+        "_download_dataset_and_return_local_path",
+    )
+    from_cache = mocker.spy(
+        CachedFoundryClient,
+        "_return_local_path_of_cached_dataset",
+    )
+    online = mocker.spy(
+        CachedFoundryClient,
+        "_get_dataset_identity_online",
+    )
+    offline = mocker.spy(
+        CachedFoundryClient,
+        "_get_dataset_identity_offline",
     )
-    from_cache = mocker.spy(CachedFoundryClient, "_return_local_path_of_cached_dataset")
-    online = mocker.spy(CachedFoundryClient, "_get_dataset_identity_online")
-    offline = mocker.spy(CachedFoundryClient, "_get_dataset_identity_offline")
 
     get_dataset_rid.return_value = DATASET_RID
     get_dataset_last_transaction_rid.return_value = TRANSACTION_RID
     is_dataset_in_trash.return_value = False
     df = get_spark_session().createDataFrame([[1]], "col1:int")
     get_dataset_schema.return_value = {
         "fieldSchemaList": [
@@ -308,28 +314,28 @@
     def download_dataset_files_mock(
         self,
         dataset_rid: str,
         output_directory: str,
         files: list,
         view="master",
     ):
-        path = os.sep.join([output_directory, "spark"])
-        os.makedirs(path, exist_ok=True)
+        path = Path(output_directory).joinpath("spark")
+        path.mkdir(parents=True, exist_ok=True)
         df.write.format("parquet").option("compression", "snappy").save(
-            path=path, mode="overwrite"
+            path=os.fspath(path), mode="overwrite"
         )
 
-    from foundry_dev_tools import FoundryRestClient
+    from foundry_dev_tools.foundry_api_client import FoundryRestClient
 
     backup = FoundryRestClient.download_dataset_files
     FoundryRestClient.download_dataset_files = download_dataset_files_mock
 
     fdt = CachedFoundryClient()
     path, dataset_identity = fdt.fetch_dataset(DATASET_PATH, "master")
-    assert path.split(os.sep)[-1] == TRANSACTION_RID + ".parquet"
+    assert path.split(os.sep, maxsplit=-1)[-1] == TRANSACTION_RID + ".parquet"
     assert dataset_identity == {
         "dataset_rid": DATASET_RID,
         "last_transaction_rid": TRANSACTION_RID,
         "dataset_path": DATASET_PATH,
     }
 
     online.assert_called()
@@ -388,17 +394,21 @@
     get_dataset_last_transaction_rid,
     is_dataset_in_trash,
     list_dataset_files,
     get_dataset_schema,
     mocker,
 ):
     from_foundry_and_cache = mocker.spy(
-        CachedFoundryClient, "_download_dataset_and_return_local_path"
+        CachedFoundryClient,
+        "_download_dataset_and_return_local_path",
+    )
+    from_cache = mocker.spy(
+        CachedFoundryClient,
+        "_return_local_path_of_cached_dataset",
     )
-    from_cache = mocker.spy(CachedFoundryClient, "_return_local_path_of_cached_dataset")
     fdt = CachedFoundryClient()
 
     get_dataset_rid.return_value = DATASET_RID
     get_dataset_last_transaction_rid.return_value = TRANSACTION_RID
     is_dataset_in_trash.return_value = False
     df = get_spark_session().createDataFrame([[1]], "col1:int")
     list_dataset_files.return_value = ["pandas/dataset.parquet"]
@@ -415,21 +425,21 @@
         dataset_rid: str,
         output_directory: str,
         files: list,
         view="master",
         *,
         branch: str = "master",
     ):
-        path = os.sep.join([output_directory, "spark"])
-        os.makedirs(path, exist_ok=True)
+        path = Path(output_directory).joinpath("spark")
+        path.mkdir(parents=True, exist_ok=True)
         df.write.format("parquet").option("compression", "snappy").save(
-            path=path, mode="overwrite"
+            path=os.fspath(path), mode="overwrite"
         )
 
-    from foundry_dev_tools import FoundryRestClient
+    from foundry_dev_tools.foundry_api_client import FoundryRestClient
 
     backup = FoundryRestClient.download_dataset_files
     FoundryRestClient.download_dataset_files = download_dataset_files_mock
 
     spark_df = fdt.load_dataset(DATASET_PATH, "master")
 
     from_foundry_and_cache.assert_called()
@@ -442,43 +452,43 @@
     from_foundry_and_cache.assert_not_called()
     from_cache.assert_called()
 
     FoundryRestClient.download_dataset_files = backup
 
 
 def test_api_client_not_cached(mocker):
-    with mocker.patch(
-        "foundry_dev_tools.Configuration.get_config",
+    mocker.patch(
+        "foundry_dev_tools.config.Configuration.get_config",
         side_effect=[
             {
                 "jwt": "secret-token-CACHED-FOUNDRY",
                 "foundry_url": "https://test.com",
-                "cache_dir": foundry_dev_tools.Configuration["cache_dir"],
+                "cache_dir": Configuration["cache_dir"],
             },
             {
                 "jwt": "secret-token-ONE",
                 "foundry_url": "https://test.com",
-                "cache_dir": foundry_dev_tools.Configuration["cache_dir"],
+                "cache_dir": Configuration["cache_dir"],
             },
             {
                 "jwt": "secret-token-TWO",
                 "foundry_url": "https://test.com",
-                "cache_dir": foundry_dev_tools.Configuration["cache_dir"],
+                "cache_dir": Configuration["cache_dir"],
             },
         ],
-    ):
-        fs = CachedFoundryClient()
-        assert fs.config["jwt"] == "secret-token-CACHED-FOUNDRY"
-        assert fs.api._config["jwt"] == "secret-token-ONE"
-        assert fs.api._config["jwt"] == "secret-token-TWO"
+    )
+    fs = CachedFoundryClient()
+    assert fs.config["jwt"] == "secret-token-CACHED-FOUNDRY"
+    assert fs.api._config["jwt"] == "secret-token-ONE"
+    assert fs.api._config["jwt"] == "secret-token-TWO"
 
 
 def test_save_string_model(mock_client):
     with mock.patch(
-        "foundry_dev_tools.CachedFoundryClient.api",
+        "foundry_dev_tools.cached_foundry_client.CachedFoundryClient.api",
         mock_client,
     ):
         cfc = CachedFoundryClient()
 
         model = "simplestring"
         rid, transaction = cfc.save_model(
             model,
@@ -487,11 +497,11 @@
             exists_ok=True,
             mode="SNAPSHOT",
         )
 
         from_foundry = cfc.fetch_dataset("/Namespace1/project1/save_model_test")
         import pickle
 
-        with open(f"{from_foundry[0]}/model.pickle", "rb") as f:
-            model_returned = pickle.load(f)
+        with Path(from_foundry[0]).joinpath("model.pickle").open(mode="rb") as f:
+            model_returned = pickle.load(f)  # noqa: S301, trusted, we are mocking
 
         assert model == model_returned
```

### Comparing `foundry-dev-tools-1.0.9/tests/test_cached_foundry_client_integration.py` & `foundry-dev-tools-1.1/tests/test_cached_foundry_client_integration.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import pandas as pd
 import pytest
 from pandas._testing import assert_frame_equal
 
-from foundry_dev_tools import CachedFoundryClient, FoundryRestClient
-
+from foundry_dev_tools.cached_foundry_client import CachedFoundryClient
+from foundry_dev_tools.foundry_api_client import FoundryRestClient
 from tests.utils import generic_upload_dataset_if_not_exists
 
 
 @pytest.fixture()
 def append_test_dataset():
-    empty_dataset = generic_upload_dataset_if_not_exists(
+    return generic_upload_dataset_if_not_exists(
         client=FoundryRestClient(),
         name="append_test_dataset_v1",
         upload_folder=None,
         foundry_schema=None,
     )
-    yield empty_dataset
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_cached_foundry_client_append(append_test_dataset):
     cfc = CachedFoundryClient()
 
     df = pd.DataFrame(data={"Name": ["max"]})
 
     rid1, transaction1 = cfc.save_dataset(
         df,
```

### Comparing `foundry-dev-tools-1.0.9/tests/test_config.py` & `foundry-dev-tools-1.1/tests/test_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 import os
 import pathlib
 import random
 import tempfile
 from unittest import mock
 
-import foundry_dev_tools
+import foundry_dev_tools.config
 from foundry_dev_tools.config import Config
-
 from tests.conftest import PatchConfig
 
 # fake home for full control over all config files and variables
 # without modifying or deleting the users config files
 FAKE_HOME = pathlib.Path(tempfile.mkdtemp())
 RANDOM_NUMBER1 = random.randint(1, 12345)
 RANDOM_NUMBER2 = random.randint(1, 12345)
 RANDOM_NUMBER3 = random.randint(1, 12345)
 
 
 @mock.patch("pathlib.Path.home", return_value=FAKE_HOME)
 def test_config_precedence(tmp):
+    MAGIC = 999
     with PatchConfig(
         initial_config_overwrite={
             "jwt": "123",
             "foundry_url": "precedence-test-url",
-            "transforms_sql_dataset_size_threshold": "999",
+            "transforms_sql_dataset_size_threshold": str(MAGIC),
         }
     ):
         # test initial config overwrite
         assert (
-            foundry_dev_tools.INITIAL_CONFIG["jwt"]
-            == foundry_dev_tools.Configuration["jwt"]
+            foundry_dev_tools.config.INITIAL_CONFIG["jwt"]
+            == foundry_dev_tools.config.Configuration["jwt"]
             == "123"
         )
 
         # test type conversion
         assert (
-            foundry_dev_tools.INITIAL_CONFIG["transforms_sql_dataset_size_threshold"]
-            == foundry_dev_tools.Configuration["transforms_sql_dataset_size_threshold"]
-            == 999
+            foundry_dev_tools.config.INITIAL_CONFIG[
+                "transforms_sql_dataset_size_threshold"
+            ]
+            == foundry_dev_tools.config.Configuration[
+                "transforms_sql_dataset_size_threshold"
+            ]
+            == MAGIC
         )
 
         # test dynamic overwrite config, not overwriting static configs
         config_overwrite = Config({"jwt": "456"})
         assert config_overwrite["jwt"] == "456"
 
         # initial configs and static configs stay untouched
         assert (
-            foundry_dev_tools.INITIAL_CONFIG["jwt"]
-            == foundry_dev_tools.Configuration["jwt"]
+            foundry_dev_tools.config.INITIAL_CONFIG["jwt"]
+            == foundry_dev_tools.config.Configuration["jwt"]
             == "123"
         )
 
         # change static config directly
-        foundry_dev_tools.Configuration["jwt"] = "789"
+        foundry_dev_tools.config.Configuration["jwt"] = "789"
         # initial config and the transforms config stay untouched
-        assert foundry_dev_tools.INITIAL_CONFIG["jwt"] == "123"
+        assert foundry_dev_tools.config.INITIAL_CONFIG["jwt"] == "123"
 
         # the dynamic config overwrites with its own supplied value
         assert config_overwrite["jwt"] == "456"
 
 
 @mock.patch("pathlib.Path.home", return_value=FAKE_HOME)
 @mock.patch.dict(
@@ -73,18 +77,40 @@
             "jwt": "whatever",
             "foundry_url": "foundry_config_env_takes_precedence",
             "transforms_sql_sample_row_limit": RANDOM_NUMBER2,
         },
         read_initial=True,
     ):
         assert (
-            foundry_dev_tools.INITIAL_CONFIG["transforms_sql_sample_row_limit"]
+            foundry_dev_tools.config.INITIAL_CONFIG["transforms_sql_sample_row_limit"]
             == RANDOM_NUMBER1
         )
 
         # overwrite config supplied takes precedence over env variable
         assert (
             Config({"transforms_sql_sample_row_limit": RANDOM_NUMBER3})[
                 "transforms_sql_sample_row_limit"
             ]
             == RANDOM_NUMBER3
         )
+
+
+@mock.patch("pathlib.Path.home", return_value=FAKE_HOME)
+@mock.patch.dict(
+    os.environ, {"FOUNDRY_DEV_TOOLS_JWT": "env_jwt_takes_precedence_over_config_files"}
+)
+def test_env_varibale_takes_precedence_over_config_files(tmp):
+    FDT_DIR = pathlib.Path.home().joinpath(".foundry-dev-tools")
+    FDT_DIR.mkdir(parents=True)
+    with FDT_DIR.joinpath("config").open(mode="w+") as fdt_conf_file:
+        fdt_conf_file.write(
+            "[default]\njwt=123456789\nfoundry_url=https://env_take_prec.lan/"
+        )
+    with PatchConfig(read_initial=True):
+        assert (
+            foundry_dev_tools.config.Configuration["jwt"]
+            == "env_jwt_takes_precedence_over_config_files"
+        )
+        assert (
+            foundry_dev_tools.config.INITIAL_CONFIG["jwt"]
+            == "env_jwt_takes_precedence_over_config_files"
+        )
```

### Comparing `foundry-dev-tools-1.0.9/tests/test_data/binary_dataset/bin` & `foundry-dev-tools-1.1/tests/test_data/binary_dataset/bin`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/tests/test_data/iris/iris.csv` & `foundry-dev-tools-1.1/tests/test_data/iris/iris.csv`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/tests/test_foundry_api.py` & `foundry-dev-tools-1.1/tests/test_foundry_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,26 @@
 
 import pandas as pd
 import pytest
 import requests_mock
 from requests import HTTPError
 from requests_mock.adapter import ANY
 
-import foundry_dev_tools
-from foundry_dev_tools import FoundryRestClient
+import foundry_dev_tools.config
 from foundry_dev_tools.foundry_api_client import (
     BranchesAlreadyExistError,
     BranchNotFoundError,
     DatasetAlreadyExistsError,
     DatasetHasNoSchemaError,
     DatasetHasOpenTransactionError,
     DatasetNoReadAccessError,
     DatasetNotFoundError,
     FolderNotFoundError,
+    FoundryRestClient,
 )
-
 from tests.conftest import PatchConfig
 from tests.utils import (
     INTEGRATION_TEST_COMPASS_ROOT_PATH,
     INTEGRATION_TEST_COMPASS_ROOT_RID,
     TEST_FOLDER,
 )
 
@@ -40,41 +39,41 @@
         assert client._headers()["Authorization"] == "Bearer 123"
         assert client._verify() is not None
     assert "transforms_sql_sample_row_limit" in client._config
     assert "transforms_sql_dataset_size_threshold" in client._config
     assert "foundry_url" in client._config
 
 
-@pytest.mark.no_patch_conf
+@pytest.mark.no_patch_conf()
 def test_sso_config(mocker, tmpdir):
     with PatchConfig(
         config_overwrite={
             "client_id": "1234",
             "foundry_url": "https://foundry.example.com",
             "grant_type": "authorization_code",
         }
     ):
-        if "jwt" in foundry_dev_tools.Configuration:
-            del foundry_dev_tools.Configuration["jwt"]
+        if "jwt" in foundry_dev_tools.config.Configuration:
+            del foundry_dev_tools.config.Configuration["jwt"]
         client = FoundryRestClient()
 
         mock_get_user_credentials = mocker.patch(
             "palantir_oauth_client.get_user_credentials"
         )
-        mock_get_user_credentials.return_value.token = "access-token"
+        mock_get_user_credentials.return_value.token = "access-token"  # noqa: S105
 
         assert client._headers()["Authorization"] == "Bearer access-token"
         assert client._headers()["User-Agent"].startswith("foundry-dev-tools")
 
 
-@pytest.mark.integration
-def test_monster_integration_test(client):
+@pytest.mark.integration()
+def test_monster_integration_test(client):  # noqa: PLR0915, TODO?
     BRANCH = "master/with/slash"
     rnd = "".join(choice(ascii_uppercase) for i in range(5))
-    dataset_path = str(INTEGRATION_TEST_COMPASS_ROOT_PATH / f"test_api_{rnd}")
+    dataset_path = os.fspath(INTEGRATION_TEST_COMPASS_ROOT_PATH / f"test_api_{rnd}")
 
     ds = client.create_dataset(dataset_path)
     assert "rid" in ds
     assert "fileSystemId" in ds
     with pytest.raises(DatasetAlreadyExistsError) as excinfo:
         client.create_dataset(dataset_path)
     assert excinfo.value.dataset_rid == ds["rid"]
@@ -180,25 +179,24 @@
     assert last_transaction_rid == last_good_transaction_rid
 
     client.create_branch(ds["rid"], "from-master", branch["id"], branch["rid"])
 
     client.delete_dataset(ds["rid"])
     assert client.is_dataset_in_trash(dataset_path) is True
 
-    with pytest.warns(UserWarning) as warning:
+    with pytest.warns(UserWarning):
         client.get_dataset_details(dataset_path_or_rid=dataset_path)
 
     with pytest.raises(DatasetNotFoundError):
         client.delete_dataset(ds["rid"])
 
 
 def test_get_dataset_rid(mocker, is_integration_test, client, iris_dataset):
     if not is_integration_test:
         mock_get = mocker.patch("requests.request")
-        # mock_get.return_value = Mock(ok=True)
         mock_get.return_value.status_code = 200
         mock_get.return_value.json.return_value = {
             "rid": iris_dataset[0],
             "name": "iris",
             "created": {
                 "time": "2020-01-30T11:18:00.130419Z",
                 "userId": "3c8fbda5-686e-4fcb-ad52-d95e4281d99f",
@@ -272,18 +270,20 @@
             "markings": None,
             "linkedItems": None,
         }
     rid = client.get_dataset_rid(iris_dataset[1])
     assert rid == iris_dataset[0]
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_schema_inference(client):
     rnd = "".join(choice(ascii_uppercase) for i in range(5))
-    dataset_path = str(INTEGRATION_TEST_COMPASS_ROOT_PATH / f"test_api_schema_{rnd}")
+    dataset_path = os.fspath(
+        INTEGRATION_TEST_COMPASS_ROOT_PATH / f"test_api_schema_{rnd}"
+    )
 
     ds = client.create_dataset(dataset_path)
     client.create_branch(ds["rid"], "master")
     transaction_rid = client.open_transaction(ds["rid"], "SNAPSHOT", "master")
     client.upload_dataset_file(
         ds["rid"], transaction_rid, io.StringIO("col1,col2\n1,2"), "test.csv"
     )
@@ -468,28 +468,28 @@
 
 
 def test_get_and_download_dataset_files(client, iris_dataset, tmpdir):
     list_of_files = client.list_dataset_files(iris_dataset[0])
     assert list_of_files == ["iris.csv"]
     client.download_dataset_files(
         iris_dataset[0],
-        str(tmpdir),
+        os.fspath(tmpdir),
         list_of_files,
     )
     assert "iris.csv" in os.listdir(tmpdir)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_get_csv_of_dataset(client, iris_dataset):
     response = client.get_dataset_as_raw_csv(iris_dataset[0])
     iris = pd.read_csv(io.BytesIO(response.content))
     assert iris.shape == (150, 5)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_query_legacy_sql(client, iris_dataset, iris_no_schema_dataset):
     foundry_schema, data = client.query_foundry_sql_legacy(
         f"SELECT * FROM `{iris_dataset[0]}` LIMIT 100"
     )
     iris = pd.DataFrame(
         data=data, columns=[e["name"] for e in foundry_schema["fieldSchemaList"]]
     )
@@ -504,15 +504,15 @@
     with pytest.raises(DatasetHasNoSchemaError):
         client.query_foundry_sql_legacy(
             f"SELECT * FROM `{iris_no_schema_dataset[1]}` LIMIT 100",
             branch=iris_no_schema_dataset[3],
         )
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_query_sql(client, mocker, iris_dataset):
     iris_rid = iris_dataset[0]
     spy = mocker.spy(FoundryRestClient, "query_foundry_sql_legacy")
 
     iris_pdf = client.query_foundry_sql(f"SELECT * FROM `{iris_rid}` LIMIT 100")
     assert iris_pdf.shape == (100, 5)
 
@@ -526,28 +526,40 @@
 
     iris_fallback = client.query_foundry_sql(
         f"SELECT * FROM `{iris_rid}` order by sepal_width LIMIT 100"
     )
     assert iris_fallback.shape == (100, 5)
     # The order by should trigger a computation in spark and today 18/10/2022
     # the Foundry SQL server does not return ARROW but JSON
-    spy.assert_called()
+    spy.assert_not_called()
 
     spy.reset_mock()
 
     iris_where = client.query_foundry_sql(
         f"SELECT * FROM `{iris_rid}` where is_setosa = 'Iris-setosa'"
     )
     assert all(
         iris_where["is_setosa"] == "Iris-setosa"
     ), f"Still multiple classes: {iris_where['is_setosa'].unique()}"
     # The order by should trigger a computation in spark and today 18/10/2022
     # the Foundry SQL server does not return ARROW but JSON
+    spy.assert_not_called()
+
+    spy.reset_mock()
+    import sys
+
+    pyarrow = sys.modules["pyarrow"]
+    sys.modules["pyarrow"] = None
+
+    iris = client.query_foundry_sql(f"SELECT * FROM `{iris_dataset[1]}`")
+    assert iris.shape == (150, 5)
     spy.assert_called()
 
+    sys.modules["pyarrow"] = pyarrow
+
 
 def test_raise_for_status_prints_details(mocker, capsys):
     client = FoundryRestClient()
     from requests.models import Response
 
     the_response = mocker.Mock(spec=Response)
     the_response.text = "issue_text"
@@ -555,19 +567,19 @@
     the_response.raise_for_status.side_effect = HTTPError(
         "message", response=the_response
     )
     mocker.patch("requests.request").return_value = the_response
     with pytest.raises(HTTPError):
         client.get_dataset("test")
     captured = capsys.readouterr()
-    assert captured.out == "message\nissue_text\n"
-    assert captured.err == ""
+    assert captured.err == "message\nissue_text\n"
+    assert not captured.out
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_get_folder_children(client, mocker, iris_dataset):
     children = client.get_child_objects_of_folder(
         folder_rid=INTEGRATION_TEST_COMPASS_ROOT_RID
     )
     assert (
         len(
             list(
@@ -622,46 +634,46 @@
     # Download single file, list call is not triggered
     spy = mocker.spy(type(client), "list_dataset_files")
 
     with client.download_dataset_files_temporary(
         dataset_rid=complex_dataset_fixture,
         view="master",
     ) as temp_dir:
-        assert os.path.exists(temp_dir) is True
+        assert Path(temp_dir).exists()
         _ = pd.read_parquet(temp_dir)
         _ = parquet.ParquetDataset(
             [x for x in Path(temp_dir).glob("**/*") if x.is_file()]
         ).read()
-    assert os.path.exists(temp_dir) is False
+    assert not Path(temp_dir).exists()
     spy.assert_called()
     spy.reset_mock()
 
     with client.download_dataset_files_temporary(
         dataset_rid=iris_dataset[0],
         view="master",
     ) as temp_dir:
-        assert os.path.exists(temp_dir) is True
+        assert Path(temp_dir).exists()
         _ = pd.read_csv(os.sep.join([temp_dir, "iris.csv"]))
-    assert os.path.exists(temp_dir) is False
+    assert not Path(temp_dir).exists()
     spy.assert_called()
     spy.reset_mock()
 
     with client.download_dataset_files_temporary(
         dataset_rid=iris_dataset[0],
         files=["iris.csv"],
         view="master",
     ) as temp_dir:
-        assert os.path.exists(temp_dir) is True
+        assert Path(temp_dir).exists()
         iris = pd.read_csv(os.sep.join([temp_dir, "iris.csv"]))
-    assert os.path.exists(temp_dir) is False
+    assert Path(temp_dir).exists() is False
     assert iris.shape == (150, 5)
     spy.assert_not_called()
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_remove_file_in_open_transaction(client, empty_dataset):
     rid = empty_dataset[0]
 
     transaction_rid = client.open_transaction(rid, "UPDATE", empty_dataset[3])
 
     client.upload_dataset_file(
         rid, transaction_rid, io.StringIO("col1,col2\n1,2"), "test.csv"
@@ -677,15 +689,15 @@
         rid, view=empty_dataset[3], include_open_exclusive_transaction=True
     )
     assert "test.csv" not in files
 
     client.abort_transaction(rid, transaction_rid)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_remove_file_from_previous_transaction(client, empty_dataset):
     rid = empty_dataset[0]
 
     transaction_rid = client.open_transaction(rid, "SNAPSHOT", empty_dataset[3])
 
     client.upload_dataset_file(
         rid, transaction_rid, io.StringIO("col1,col2\n1,2"), "test.csv"
@@ -716,26 +728,26 @@
         output_directory=None,
         foundry_file_path="iris.csv",
     )
     iris = pd.read_csv(io.BytesIO(raw_bytes))
     assert iris.shape == (150, 5)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_get_dataset_details_identical_path_rid(client, iris_dataset):
     by_path = client.get_dataset_details(dataset_path_or_rid=iris_dataset[1])
 
     by_rid = client.get_dataset_details(dataset_path_or_rid=iris_dataset[0])
 
     assert by_path["rid"] == by_rid["rid"]
     assert by_path["path"] == by_rid["path"]
 
 
 @patch(
-    "foundry_dev_tools.FoundryRestClient.get_dataset_details",
+    "foundry_dev_tools.foundry_api_client.FoundryRestClient.get_dataset_details",
     MagicMock(
         return_value={
             "rid": "ri.foundry.main.dataset.1234",
             "name": "data1",
             "created": {
                 "time": "2022-04-19T14:03:24.072061923Z",
                 "userId": "1234",
@@ -780,15 +792,15 @@
             "classification": None,
             "disableInheritedPermissions": None,
             "propagatePermissions": None,
         }
     ),
 )
 def test_get_dataset_details_throws_on_no_read_permissions():
-    from foundry_dev_tools import FoundryRestClient
+    from foundry_dev_tools.foundry_api_client import FoundryRestClient
 
     client = FoundryRestClient()
     with pytest.raises(DatasetNoReadAccessError):
         _ = client.get_dataset_identity(
             dataset_path_or_rid="ri.foundry.main.dataset.1234"
         )
 
@@ -819,15 +831,15 @@
             history[0].query
             == "logicalPath=prod2_api_v2_reports_query%3F%232022-06-27T22_24_18.528205Z.json"
         )
         assert (
             history[1].query
             == "logicalPath=All+123+-+BLUB+Extract_new+%28Export+2021-12-21+18_25%29-20211221.140314.csv"
         )
-        m.get(url=ANY, status_code=200, body=io.BytesIO("some-content".encode("UTF-8")))
+        m.get(url=ANY, status_code=200, body=io.BytesIO(b"some-content"))
         client.download_dataset_file(
             dataset_rid="rid",
             output_directory=None,
             view="master",
             foundry_file_path=needs_quotation,
         )
         client.download_dataset_file(
```

### Comparing `foundry-dev-tools-1.0.9/tests/test_foundry_local_deprecation.py` & `foundry-dev-tools-1.1/tests/test_foundry_local_deprecation.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,147 +4,146 @@
 import tempfile
 from unittest import mock
 
 import pytest
 
 import foundry_dev_tools
 import foundry_dev_tools.config
-from foundry_dev_tools.config import execute_as_subprocess
-
 from tests.conftest import PatchConfig
 
 # fake home for full control over all config files and variables
 # without modifying or deleting the users config files
 FAKE_HOME = pathlib.Path(tempfile.mkdtemp())
 
 
-@pytest.mark.no_patch_conf
+@pytest.mark.no_patch_conf()
 @mock.patch("pathlib.Path.home", return_value=FAKE_HOME)
 @mock.patch.dict(
     os.environ,
     {
         "FOUNDRY_LOCAL_TRANSFORMS_SQL_SAMPLE_ROW_LIMIT": "8888",
         "FOUNDRY_DEV_TOOLS_TRANSFORMS_SQL_SAMPLE_ROW_LIMIT": "9999",
     },
 )
 def test_new_env_variable_takes_precedence(tmp):
     with PatchConfig(
         initial_config_overwrite={
             "jwt": "whatever",
             "foundry_url": "foundry_local_deprecation",
-            "disable_token_providers": True,
+            "enable_runtime_token_providers": False,
         },
         read_initial=True,
     ):
         assert (
-            foundry_dev_tools.Configuration["transforms_sql_sample_row_limit"] == 9999
+            foundry_dev_tools.config.Configuration["transforms_sql_sample_row_limit"]
+            == 9999
         )
 
 
-@pytest.mark.no_patch_conf
+@pytest.mark.no_patch_conf()
 @mock.patch("pathlib.Path.home", return_value=FAKE_HOME)
 @mock.patch.dict(os.environ, {"FOUNDRY_LOCAL_TRANSFORMS_SQL_SAMPLE_ROW_LIMIT": "123"})
 def test_old_env_variable_fallback(tmp):
-    with pytest.deprecated_call():
-        with PatchConfig(
-            initial_config_overwrite={
-                "jwt": "whatever",
-                "foundry_url": "foundry_local_deprecation",
-                "disable_token_providers": True,
-            },
-            read_initial=True,
-        ):
-            assert (
-                foundry_dev_tools.Configuration["transforms_sql_sample_row_limit"]
-                == 123
-            )
+    with pytest.deprecated_call(), PatchConfig(
+        initial_config_overwrite={
+            "jwt": "whatever",
+            "foundry_url": "foundry_local_deprecation",
+            "enable_runtime_token_providers": False,
+        },
+        read_initial=True,
+    ):
+        assert (
+            foundry_dev_tools.config.Configuration["transforms_sql_sample_row_limit"]
+            == 123
+        )
 
 
-@pytest.mark.no_patch_conf
+@pytest.mark.no_patch_conf()
 @mock.patch("pathlib.Path.home", return_value=FAKE_HOME)
 def test_old_config_directory_or_file_warning(tmp):
     FL_DIR = pathlib.Path.home() / ".foundry-local"
-    os.mkdir(FL_DIR)
-    with open(FL_DIR / "config", "w+") as fl_config:
+    FL_DIR.mkdir()
+    with FL_DIR.joinpath("config").open(mode="w+") as fl_config:
         fl_config.write(
             "[default]\nfoundry_url=foundry_local_deprecation\njwt=old_config_directory\n"
         )
 
-    with pytest.deprecated_call():
-        with PatchConfig(
-            initial_config_overwrite={"disable_token_providers": True},
-            read_initial=True,
-        ):
-            assert foundry_dev_tools.Configuration["jwt"] == "old_config_directory"
+    with pytest.deprecated_call(), PatchConfig(
+        initial_config_overwrite={"enable_runtime_token_providers": False},
+        read_initial=True,
+    ):
+        assert foundry_dev_tools.config.Configuration["jwt"] == "old_config_directory"
 
     FDT_DIR = pathlib.Path.home() / ".foundry-dev-tools"
-    os.mkdir(FDT_DIR)
-    with open(FDT_DIR / "config", "w+") as fl_config:
+    FDT_DIR.mkdir()
+    with FDT_DIR.joinpath("config").open(mode="w+") as fl_config:
         fl_config.write(
             "[default]\nfoundry_url=foundry_local_deprecation\njwt=new_config_directory\n"
         )
 
     with PatchConfig(
-        initial_config_overwrite={"disable_token_providers": True}, read_initial=True
+        initial_config_overwrite={"enable_runtime_token_providers": False},
+        read_initial=True,
     ):
-        assert foundry_dev_tools.Configuration["jwt"] == "new_config_directory"
+        assert foundry_dev_tools.config.Configuration["jwt"] == "new_config_directory"
 
     FAKE_GIT_DIR = pathlib.Path.home() / "supercool-transform-git-repo"
-    os.mkdir(FAKE_GIT_DIR)
-    with open(FAKE_GIT_DIR / ".foundry_local_config", "w+") as old_git_cfg:
+    FAKE_GIT_DIR.mkdir()
+    with FAKE_GIT_DIR.joinpath(".foundry_local_config").open(mode="w+") as old_git_cfg:
         old_git_cfg.write("[default]\njwt=old_git_config_file\n")
     with mock.patch(
-        "foundry_dev_tools.config._traverse_to_git_project_top_level_dir",
-        return_value=str(FAKE_GIT_DIR),
+        "foundry_dev_tools.utils.repo.git_toplevel_dir",
+        return_value=FAKE_GIT_DIR,
     ):
-        with pytest.deprecated_call():
-            with PatchConfig(
-                initial_config_overwrite={"disable_token_providers": True},
-                read_initial=True,
-            ):
-                assert foundry_dev_tools.Configuration["jwt"] == "old_git_config_file"
+        with pytest.deprecated_call(), PatchConfig(
+            initial_config_overwrite={"enable_runtime_token_providers": False},
+            read_initial=True,
+        ):
+            assert (
+                foundry_dev_tools.config.Configuration["jwt"] == "old_git_config_file"
+            )
 
-        with open(FAKE_GIT_DIR / ".foundry_dev_tools", "w+") as old_git_cfg:
+        with FAKE_GIT_DIR.joinpath(".foundry_dev_tools").open(mode="w+") as old_git_cfg:
             old_git_cfg.write("[default]\njwt=new_git_config_file\n")
 
         with PatchConfig(
-            initial_config_overwrite={"disable_token_providers": True},
+            initial_config_overwrite={"enable_runtime_token_providers": False},
             read_initial=True,
         ):
-            assert foundry_dev_tools.Configuration["jwt"] == "new_git_config_file"
-            # TODO: This breaks the global config that is present in integration tests and overwrites the real
-            # jwt, after this test, all other tests fail.
-
+            assert (
+                foundry_dev_tools.config.Configuration["jwt"] == "new_git_config_file"
+            )
     shutil.rmtree(FAKE_HOME)
 
 
-@pytest.mark.no_patch_conf
+@pytest.mark.no_patch_conf()
 @mock.patch("pathlib.Path.home", return_value=FAKE_HOME)
 @mock.patch.dict(os.environ, {})
 def test_old_set_method(tmp):
     with PatchConfig(
         initial_config_overwrite={
             "jwt": "whatever",
             "foundry_url": "https://test.com",
-            "disable_token_providers": True,
+            "enable_runtime_token_providers": False,
         },
         read_initial=True,
     ):
         with pytest.warns(expected_warning=DeprecationWarning) as record1:
-            foundry_dev_tools.Configuration.set("test_key", "value")
+            foundry_dev_tools.config.Configuration.set("test_key", "value")
         assert "deprecated" in record1.pop(DeprecationWarning).message.args[0]
 
-        assert foundry_dev_tools.Configuration.get("test_key") == "value"
-        config = foundry_dev_tools.Configuration.get_config()
-        assert "jwt" in config and config["jwt"] == "whatever"
-        assert "foundry_url" in config and config["foundry_url"] == "https://test.com"
-        assert (
-            "disable_token_providers" in config
-            and config["disable_token_providers"] is True
-        )
-        assert "test_key" in config and config["test_key"] == "value"
+        assert foundry_dev_tools.config.Configuration.get("test_key") == "value"
+        config = foundry_dev_tools.config.Configuration.get_config()
+        assert "jwt" in config
+        assert config["jwt"] == "whatever"
+        assert "foundry_url" in config
+        assert config["foundry_url"] == "https://test.com"
+        assert "enable_runtime_token_providers" in config
+        assert not config["enable_runtime_token_providers"]
+        assert "test_key" in config
+        assert config["test_key"] == "value"
 
         with pytest.warns(expected_warning=DeprecationWarning) as record:
-            foundry_dev_tools.Configuration.delete("test_key")
+            foundry_dev_tools.config.Configuration.delete("test_key")
 
         assert "deprecated" in record.pop(DeprecationWarning).message.args[0]
-        assert "Test" not in foundry_dev_tools.Configuration
+        assert "Test" not in foundry_dev_tools.config.Configuration
```

### Comparing `foundry-dev-tools-1.0.9/tests/test_foundry_mock.py` & `foundry-dev-tools-1.1/tests/test_foundry_mock.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 import io
 import os
-import pathlib
 import shutil
 import time
+from pathlib import Path
 
 import fs
 import pytest
 
 from foundry_dev_tools.foundry_api_client import (
     BranchesAlreadyExistError,
     DatasetHasOpenTransactionError,
     DatasetNotFoundError,
 )
-
 from tests.foundry_mock_client import MockFoundryRestClient
 
 
 @pytest.fixture()
 def root_dir():
-    TEST_FOLDER = pathlib.Path(__file__).parent.resolve().as_posix()
-    root = f"{TEST_FOLDER}/foundry_mock_root"
+    root = Path(__file__).parent.joinpath("foundry_mock_root")
     shutil.rmtree(root, ignore_errors=True)
-    os.mkdir(root)
-    yield root
+    root.mkdir()
+    return root
 
 
 def test_create_rids_time_ordered(tmpdir, root_dir):
-    bases = [
-        str(tmpdir),
-        root_dir,
-    ]
+    bases = [tmpdir, root_dir]
     for base in bases:
-        filesystem = fs.open_fs(base)
-        client = MockFoundryRestClient(fs=filesystem)
+        filesystem = fs.open_fs(os.fspath(base))
+        client = MockFoundryRestClient(filesystem=filesystem)
 
         dataset = client.create_dataset("/path/to/ds")
         assert "rid" in dataset
         assert "fileSystemId" in dataset
         get_result = client.get_dataset(dataset_rid=dataset["rid"])
         assert dataset == get_result
 
@@ -49,45 +44,36 @@
         ):
             rids.append(client.create_dataset(f"/path/to/ds{i}")["rid"])
             time.sleep(0.001)
         assert rids == sorted(rids)
 
 
 def test_dataset_not_found(tmpdir, root_dir):
-    bases = [
-        str(tmpdir),
-        root_dir,
-    ]
+    bases = [tmpdir, root_dir]
     for base in bases:
-        filesystem = fs.open_fs(base)
-        client = MockFoundryRestClient(fs=filesystem)
+        filesystem = fs.open_fs(os.fspath(base))
+        client = MockFoundryRestClient(filesystem=filesystem)
         with pytest.raises(DatasetNotFoundError):
             _ = client.get_dataset(dataset_rid="blarid")
 
 
 def test_create_delete(tmpdir, root_dir):
-    bases = [
-        str(tmpdir),
-        root_dir,
-    ]
+    bases = [tmpdir, root_dir]
     for base in bases:
-        filesystem = fs.open_fs(base)
-        client = MockFoundryRestClient(fs=filesystem)
+        filesystem = fs.open_fs(os.fspath(base))
+        client = MockFoundryRestClient(filesystem=filesystem)
         dataset = client.create_dataset("/path/to/to_be_deleted")
         client.delete_dataset(dataset["rid"])
 
 
 def test_create_delete_branch(tmpdir, root_dir):
-    bases = [
-        root_dir,
-        str(tmpdir),
-    ]
+    bases = [root_dir, tmpdir]
     for base in bases:
-        filesystem = fs.open_fs(base)
-        client = MockFoundryRestClient(fs=filesystem)
+        filesystem = fs.open_fs(os.fspath(base))
+        client = MockFoundryRestClient(filesystem=filesystem)
         dataset = client.create_dataset("/path/to/ds_with_branch")
         branch = client.create_branch(dataset_rid=dataset["rid"], branch="main")
         assert branch["id"] == "main"
         assert "rid" in branch
         assert "ancestorBranchIds" in branch
         assert "creationTime" in branch
         assert branch["transactionRid"] is None
@@ -95,39 +81,35 @@
         branch_returned = client.get_branch(dataset_rid=dataset["rid"], branch="main")
 
         assert branch == branch_returned
 
         with pytest.raises(BranchesAlreadyExistError):
             _ = client.create_branch(dataset_rid=dataset["rid"], branch="main")
 
-        master = client.create_branch(dataset_rid=dataset["rid"], branch="master")
+        client.create_branch(dataset_rid=dataset["rid"], branch="master")
 
         client.delete_dataset(dataset["rid"])
 
 
-def test_transactions(tmp_path_factory, root_dir):
-    temp_directory = tmp_path_factory.mktemp(f"foundry_dev_tools_test_1").as_posix()
-    print(temp_directory)
-    bases = [
-        root_dir,
-        str(temp_directory),
-    ]
+def test_transactions(tmp_path_factory, root_dir):  # noqa: PLR0915, TODO?
+    temp_directory = tmp_path_factory.mktemp("foundry_dev_tools_test_1").as_posix()
+    bases = [root_dir, temp_directory]
     for base in bases:
-        filesystem = fs.open_fs(base)
-        client = MockFoundryRestClient(fs=filesystem)
+        filesystem = fs.open_fs(os.fspath(base))
+        client = MockFoundryRestClient(filesystem=filesystem)
 
         BRANCH = "master"
 
         ds = client.create_dataset("/path/to/ds")
         identity_by_path = client.get_dataset_identity(
             dataset_path_or_rid="/path/to/ds"
         )
         identity_by_rid = client.get_dataset_identity(dataset_path_or_rid=ds["rid"])
         assert identity_by_path == identity_by_rid
-        assert identity_by_path["last_transaction_rid"] == None
+        assert identity_by_path["last_transaction_rid"] is None
         branch = client.create_branch(dataset_rid=ds["rid"], branch=BRANCH)
 
         with pytest.raises(DatasetNotFoundError):
             client.get_dataset_identity(dataset_path_or_rid="doesnotExists")
         with pytest.raises(DatasetNotFoundError):
             client.get_dataset_identity(
                 dataset_path_or_rid="ri.foundry.main.dataset.12342ede-1530-0cf3-8f56-9a4b2231404c"
@@ -148,23 +130,23 @@
         )
 
         with pytest.raises(DatasetHasOpenTransactionError) as exc_info:
             client.open_transaction(ds["rid"], "SNAPSHOT", BRANCH)
         assert exc_info.value.dataset_rid == ds["rid"]
         assert exc_info.value.open_transaction_rid == transaction_rid
 
-        tmpdir = tmp_path_factory.mktemp(f"foundry_dev_tools_test_2").as_posix()
-        path1 = fs.path.join(tmpdir, "test1.csv")
-        with open(path1, "w") as f:
+        tmpdir = tmp_path_factory.mktemp("foundry_dev_tools_test_2")
+        path1 = tmpdir.joinpath("test1.csv")
+        with path1.open(mode="w") as f:
             f.write("col1,col2\n1,2")
-        path2 = fs.path.join(tmpdir, "test2.csv")
-        with open(path2, "w") as f:
+        path2 = tmpdir.joinpath("test2.csv")
+        with path2.open(mode="w") as f:
             f.write("col1,col2\n1,2")
-        path3 = fs.path.join(tmpdir, "test3.csv")
-        with open(path3, "w") as f:
+        path3 = tmpdir.joinpath("test3.csv")
+        with path3.open(mode="w") as f:
             f.write("col1,col2\n1,2")
         client.upload_dataset_file(ds["rid"], transaction_rid, path1, "test1.csv")
 
         client.upload_dataset_files(
             ds["rid"],
             transaction_rid,
             path_file_dict={"test2.csv": path2, "test3.csv": path3},
@@ -263,74 +245,73 @@
             "test1.csv",
             "test2.csv",
             "test3.csv",
             "test4.csv",
             "test7.csv",
         ] == sorted([file["logicalPath"] for file in files_hidden_included])
 
-        tmp_output_dir = tmp_path_factory.mktemp(f"foundry_dev_tools_test_3").as_posix()
+        tmp_output_dir = tmp_path_factory.mktemp("foundry_dev_tools_test_3").as_posix()
         path = client.download_dataset_file(
             dataset_rid=ds["rid"],
             view=BRANCH,
-            output_directory=str(tmp_output_dir),
+            output_directory=os.fspath(tmp_output_dir),
             foundry_file_path="test7.csv",
         )
         _ = client.download_dataset_file(
             dataset_rid=ds["rid"],
             view=BRANCH,
-            output_directory=str(tmp_output_dir),
+            output_directory=os.fspath(tmp_output_dir),
             foundry_file_path="spark/test6.csv",
         )
         assert sorted(
             [
                 file.as_posix().replace(tmp_output_dir, "")[1:]
-                for file in pathlib.Path(tmp_output_dir).glob("**/*")
+                for file in Path(tmp_output_dir).glob("**/*")
                 if file.is_file()
             ]
         ) == ["spark/test6.csv", "test7.csv"]
-        with open(path, "r") as f:
+        with Path(path).open(encoding="UTF-8") as f:
             assert f.read() == "col1,col2\n5,6"
 
         tmp_output_dir_2 = tmp_path_factory.mktemp(
-            f"foundry_dev_tools_test_4"
+            "foundry_dev_tools_test_4"
         ).as_posix()
         client.download_dataset_files(
-            dataset_rid=ds["rid"], output_directory=str(tmp_output_dir_2), view=BRANCH
+            dataset_rid=ds["rid"],
+            output_directory=os.fspath(tmp_output_dir_2),
+            view=BRANCH,
         )
         assert sorted(
             [
                 file.as_posix().replace(tmp_output_dir_2, "")[1:]
-                for file in pathlib.Path(tmp_output_dir_2).glob("**/*")
+                for file in Path(tmp_output_dir_2).glob("**/*")
                 if file.is_file()
             ]
         ) == [
             "spark/test5.csv",
             "spark/test6.csv",
             "test1.csv",
             "test2.csv",
             "test3.csv",
             "test4.csv",
             "test7.csv",
         ]
 
 
 def test_dataset_schema(tmp_path_factory, root_dir):
-    temp_directory = tmp_path_factory.mktemp(f"foundry_dev_tools_test_100").as_posix()
-    bases = [
-        root_dir,
-        str(temp_directory),
-    ]
+    temp_directory = tmp_path_factory.mktemp("foundry_dev_tools_test_100").as_posix()
+    bases = [root_dir, temp_directory]
     for base in bases:
-        filesystem = fs.open_fs(base)
-        client = MockFoundryRestClient(fs=filesystem)
+        filesystem = fs.open_fs(os.fspath(base))
+        client = MockFoundryRestClient(filesystem=filesystem)
 
         BRANCH = "master"
 
         ds = client.create_dataset("/path/to/ds")
-        branch = client.create_branch(dataset_rid=ds["rid"], branch=BRANCH)
+        client.create_branch(dataset_rid=ds["rid"], branch=BRANCH)
 
         with pytest.raises(KeyError):
             client.upload_dataset_schema(
                 dataset_rid=ds["rid"],
                 transaction_rid=None,
                 schema={"test": "schema"},
             )
```

### Comparing `foundry-dev-tools-1.0.9/tests/test_foundry_spark_converters.py` & `foundry-dev-tools-1.1/tests/test_foundry_spark_converters.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.9/tests/test_foundry_sql_client.py` & `foundry-dev-tools-1.1/tests/test_foundry_sql_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,193 +2,135 @@
 from requests_mock import Mocker
 from requests_mock.adapter import ANY
 
 from foundry_dev_tools.foundry_api_client import (
     BranchNotFoundError,
     DatasetHasNoSchemaError,
     DatasetNotFoundError,
-    FoundrySqlClient,
+    FoundryRestClient,
     FoundrySqlQueryClientTimedOutError,
     FoundrySqlQueryFailedError,
     FoundrySqlSerializationFormatNotImplementedError,
 )
 
 
-def mock_initiate_session(
-    requests_mock: Mocker,
-    session_id="96bbd062-b5c1-428d-95f3-739683955ff8",
-    session_auth_token="Zu+eMIE1Unlr7vvgZ2kHkg==",
-):
-    requests_mock.post(
-        url=ANY,
-        status_code=200,
-        json={"sessionId": session_id, "sessionAuthToken": session_auth_token},
-    )
-
-
-@pytest.fixture()
-def sql_client(requests_mock: Mocker):
-    mock_initiate_session(requests_mock)
-    return FoundrySqlClient()
-
-
-def test_session_is_established(
-    requests_mock: Mocker,
-):
-    mock_initiate_session(
-        requests_mock,
-        "96bbd062-b5c1-428d-95f3-739683955ff8",
-        "Zu+eMIE1Unlr7vvgZ2kHkg==",
-    )
-
-    client = FoundrySqlClient()
-    assert client.session_auth_token == "Zu+eMIE1Unlr7vvgZ2kHkg=="
-    assert client.session_id == "96bbd062-b5c1-428d-95f3-739683955ff8"
-    assert client._headers["Session-Authorization"] == "Zu+eMIE1Unlr7vvgZ2kHkg=="
-
-
-def test_prepare_and_execute(requests_mock: Mocker, sql_client):
+def test_execute_query(requests_mock: Mocker):
+    client = FoundryRestClient()
     requests_mock.post(
         url=ANY,
         status_code=200,
         json={
-            "jobId": "217984f8-8a30-45a8-ba08-0e4a8c3f2e7c",
-            "status": {
-                "type": "ready",
-                "ready": {"jobId": "217984f8-8a30-45a8-ba08-0e4a8c3f2e7c"},
-            },
-            "statementId": "de928220-61c1-4aa7-acd0-91e5b9d4ae95",
+            "queryId": "b343c6c1-a35f-4cc5-88e8-041c84974de6",
+            "status": {"ready": {}, "type": "ready"},
         },
     )
-    response_dict = sql_client._prepare_and_execute("SELECT * FROM `blub`")
+    response_dict = client._execute_fsql_query("SELECT * FROM `blub`")
     assert response_dict == {
-        "jobId": "217984f8-8a30-45a8-ba08-0e4a8c3f2e7c",
-        "status": {
-            "type": "ready",
-            "ready": {"jobId": "217984f8-8a30-45a8-ba08-0e4a8c3f2e7c"},
-        },
-        "statementId": "de928220-61c1-4aa7-acd0-91e5b9d4ae95",
+        "queryId": "b343c6c1-a35f-4cc5-88e8-041c84974de6",
+        "status": {"ready": {}, "type": "ready"},
     }
 
 
-def test_poll_for_query_completion(requests_mock: Mocker, sql_client):
-    requests_mock.post(
-        url=ANY,
-        status_code=200,
-        json={
-            "status": {
-                "type": "ready",
-                "ready": {"jobId": "2c1d6597-77ea-41ac-9651-b86e19799800"},
-            }
-        },
-    )
-
-    sql_client._poll_for_query_completion(
-        {
-            "jobId": "2c1d6597-77ea-41ac-9651-b86e19799800",
-            "status": {
-                "type": "running",
-                "running": {"jobId": "2c1d6597-77ea-41ac-9651-b86e19799800"},
-            },
-            "statementId": "57977172-8a57-4f62-91d1-094c35c0a78b",
-        }
-    )
-
-
-def test_poll_for_query_completion_timeout(mocker, requests_mock: Mocker, sql_client):
+def test_poll_for_query_completion_timeout(mocker, requests_mock: Mocker):
     mocker.patch("time.sleep")  # we do not want to wait 500 ms in a test ;)
 
-    requests_mock.post(
+    requests_mock.get(
         url=ANY,
         status_code=200,
         json={
-            "jobId": "2c1d6597-77ea-41ac-9651-b86e19799800",
-            "status": {
-                "type": "running",
-                "running": {"jobId": "2c1d6597-77ea-41ac-9651-b86e19799800"},
-            },
-            "statementId": "57977172-8a57-4f62-91d1-094c35c0a78b",
+            "queryId": "26f444dc-822d-4be7-9c8f-3be52779bea5",
+            "status": {"running": {}, "type": "running"},
         },
     )
 
+    client = FoundryRestClient()
     with pytest.raises(FoundrySqlQueryClientTimedOutError):
-        sql_client._poll_for_query_completion(
+        client._poll_fsql_query_status(
             {
-                "jobId": "2c1d6597-77ea-41ac-9651-b86e19799800",
-                "status": {
-                    "type": "running",
-                    "running": {"jobId": "2c1d6597-77ea-41ac-9651-b86e19799800"},
-                },
-                "statementId": "57977172-8a57-4f62-91d1-094c35c0a78b",
+                "queryId": "26f444dc-822d-4be7-9c8f-3be52779bea5",
+                "status": {"running": {}, "type": "running"},
             },
             0.001,
         )
 
 
-def test_non_arrow_format_throws_exception(requests_mock: Mocker, sql_client):
-    response_data = b'S{"metadata":{"computedTime":1627978857810,"resultComputationMetadata":{"submitTimeMillis":1627978856578,"startTimeMillis":1627978856580,"finishResolveDataFrameTimeMillis":1627978857302,"finishTimeMillis":1627978857763,"estimatedResultSizeOnHeapInBytes":32296,"cacheType":"NO_CACHE","initialDataframeResolutionType":"BUILT_INITIAL_SPARK_SET_AND_DF","complexDataframeResolutionType":"NO_COMPLEX_TRANSFORMATIONS","setDescription":{"type":"sql","parentsByParam":{"/Global/Foundry Operations/Foundry Support/iris-167312679":{"type":"initialwithtransaction","identifier":"ri.foundry.main.dataset.14703427-09ab-4c9c-b036-6926b34d150b:master","transaction":"ri.foundry.main.transaction.0000003a-a437-fec8-95b1-0872dc6a0991","schemaId":"00000003-d596-797c-9663-e8970c07d296","viewMetadataId":null,"maybeStartTransaction":"ri.foundry.main.transaction.0000003a-a437-fec8-95b1-0872dc6a0991"}},"sqlQuery":"SELECT * FROM ${/Global/Foundry Operations/Foundry Support/iris-167312679}"},"queryMetricMetadata":{"queueSubmittedTimeMillis":1627978856263,"wasPunted":false},"traceId":"65a45518d71a3922","saveTraceId":"1ae3ca3cbb85ca39","latitudeQueryDescription":{"humanReadableDescription":null,"metadata":{"Skip the non-contour backend cache":"false","UserId":"3c8fbda5-686e-4fcb-ad52-d95e4281d99f","GraphId":"","NodeId":"","RefRid":"","SourceId":"foundry-sql-server"},"sourceMetadata":{"graphId":null,"nodeId":null,"refRid":null,"refParentRid":null,"sourceId":"foundry-sql-server","sparkReporterOwningRid":null,"resourceManagementAttributionRid":null,"userId":"3c8fbda5-686e-4fcb-ad52-d95e4281d99f","datasetRids":["ri.foundry.main.dataset.14703427-09ab-4c9c-b036-6926b34d150b"],"lsdHash":"01b919b1f5528a8895d161da41b4d55d","lsdHashWithMetadataScrubbed":"9c4501650954bcc765e2c8b6fd2920c5","lsdHashWithDatasetAndMetadataScrubbed":"38d9cc6b14c2d21ac287b53050ebc9aa","unresolvedLsdHash":null,"unresolvedLsdHashWithMetadataScrubbed":null,"unresolvedLsdHashWithDatasetAndMetadataScrubbed":null},"trimmedDatasetRids":[],"requestTraceId":"b2a7f6e4f8e68d97","requestTimeMillis":1627978856150},"backendMetricsTag":"foundrysqlserver-contour-backend-foundry-0","backendGroupMetricsTag":"foundry-sql-server-modules","groupProducerMetricsTag":"foundrysqlserver","numberOfTasks":null,"numberOfStages":null},"computedVersion":"9.206.0","warningMessage":null,"resultId":null,"rowCount":150,"columns":["id","is_setosa","species","sepal_length","sepal_width","petal_length","petal_width"],"columnTypes":[{"type":"INTEGER","name":"id","nullable":true,"customMetadata":{}},{"type":"INTEGER","name":"is_setosa","nullable":true,"customMetadata":{}},{"type":"STRING","name":"species","nullable":true,"customMetadata":{}},{"type":"DOUBLE","name":"sepal_length","nullable":true,"customMetadata":{}},{"type":"DOUBLE","name":"sepal_width","nullable":true,"customMetadata":{}},{"type":"DOUBLE","name":"petal_length","nullable":true,"customMetadata":{}},{"type":"DOUBLE","name":"petal_width","nullable":true,"customMetadata":{}}]},"rows":[[1,1,"setosa",5.1,3.5,1.4,0.2],[2,1,"setosa",4.9,3.0,1.4,0.2],[3,1,"setosa",4.7,3.2,1.3,0.2],[4,1,"setosa",4.6,3.1,1.5,0.2],[5,1,"setosa",5.0,3.6,1.4,0.2],[6,1,"setosa",5.0,3.4,1.5,0.2],[7,1,"setosa",4.4,2.9,1.4,0.2],[8,1,"setosa",5.4,3.7,1.5,0.2],[9,1,"setosa",4.8,3.4,1.6,0.2],[10,1,"setosa",5.8,4.0,1.2,0.2],[11,1,"setosa",5.4,3.4,1.7,0.2],[12,1,"setosa",4.6,3.6,1.0,0.2],[13,1,"setosa",4.8,3.4,1.9,0.2],[14,1,"setosa",5.0,3.0,1.6,0.2],[15,1,"setosa",5.2,3.5,1.5,0.2],[16,1,"setosa",5.2,3.4,1.4,0.2],[17,1,"setosa",4.7,3.2,1.6,0.2],[18,1,"setosa",4.8,3.1,1.6,0.2],[19,1,"setosa",5.5,4.2,1.4,0.2],[20,1,"setosa",4.9,3.1,1.5,0.2],[21,1,"setosa",5.0,3.2,1.2,0.2],[22,1,"setosa",5.5,3.5,1.3,0.2],[23,1,"setosa",4.4,3.0,1.3,0.2],[24,1,"setosa",5.1,3.4,1.5,0.2],[25,1,"setosa",4.4,3.2,1.3,0.2],[26,1,"setosa",5.1,3.8,1.6,0.2],[27,1,"setosa",4.6,3.2,1.4,0.2],[28,1,"setosa",5.3,3.7,1.5,0.2],[29,1,"setosa",5.0,3.3,1.4,0.2],[30,0,"versicolor",6.4,3.2,4.5,1.5],[31,0,"versicolor",6.9,3.1,4.9,1.5],[32,0,"versicolor",6.5,2.8,4.6,1.5],[33,0,"versicolor",5.9,3.0,4.2,1.5],[34,0,"versicolor",5.6,3.0,4.5,1.5],[35,0,"versicolor",6.2,2.2,4.5,1.5],[36,0,"versicolor",6.3,2.5,4.9,1.5],[37,0,"versicolor",6.0,2.9,4.5,1.5],[38,0,"versicolor",5.4,3.0,4.5,1.5],[39,0,"versicolor",6.7,3.1,4.7,1.5],[40,0,"virginica",6.0,2.2,5.0,1.5],[41,0,"virginica",6.3,2.8,5.1,1.5],[42,0,"versicolor",5.9,3.2,4.8,1.8],[43,0,"virginica",6.3,2.9,5.6,1.8],[44,0,"virginica",7.3,2.9,6.3,1.8],[45,0,"virginica",6.7,2.5,5.8,1.8],[46,0,"virginica",6.5,3.0,5.5,1.8],[47,0,"virginica",6.3,2.7,4.9,1.8],[48,0,"virginica",7.2,3.2,6.0,1.8],[49,0,"virginica",6.2,2.8,4.8,1.8],[50,0,"virginica",6.1,3.0,4.9,1.8],[51,0,"virginica",6.4,3.1,5.5,1.8],[52,0,"virginica",6.0,3.0,4.8,1.8],[53,0,"virginica",5.9,3.0,5.1,1.8],[54,0,"versicolor",5.5,2.3,4.0,1.3],[55,0,"versicolor",5.7,2.8,4.5,1.3],[56,0,"versicolor",6.6,2.9,4.6,1.3],[57,0,"versicolor",5.6,2.9,3.6,1.3],[58,0,"versicolor",6.1,2.8,4.0,1.3],[59,0,"versicolor",6.4,2.9,4.3,1.3],[60,0,"versicolor",6.3,2.3,4.4,1.3],[61,0,"versicolor",5.6,3.0,4.1,1.3],[62,0,"versicolor",5.5,2.5,4.0,1.3],[63,0,"versicolor",5.6,2.7,4.2,1.3],[64,0,"versicolor",5.7,2.9,4.2,1.3],[65,0,"versicolor",6.2,2.9,4.3,1.3],[66,0,"versicolor",5.7,2.8,4.1,1.3],[67,0,"versicolor",7.0,3.2,4.7,1.4],[68,0,"versicolor",5.2,2.7,3.9,1.4],[69,0,"versicolor",6.1,2.9,4.7,1.4],[70,0,"versicolor",6.7,3.1,4.4,1.4],[71,0,"versicolor",6.6,3.0,4.4,1.4],[72,0,"versicolor",6.8,2.8,4.8,1.4],[73,0,"versicolor",6.1,3.0,4.6,1.4],[74,0,"virginica",6.1,2.6,5.6,1.4],[75,0,"versicolor",4.9,2.4,3.3,1.0],[76,0,"versicolor",5.0,2.0,3.5,1.0],[77,0,"versicolor",6.0,2.2,4.0,1.0],[78,0,"versicolor",5.8,2.7,4.1,1.0],[79,0,"versicolor",5.7,2.6,3.5,1.0],[80,0,"versicolor",5.5,2.4,3.7,1.0],[81,0,"versicolor",5.0,2.3,3.3,1.0],[82,0,"virginica",6.4,3.2,5.3,2.3],[83,0,"virginica",7.7,2.6,6.9,2.3],[84,0,"virginica",6.9,3.2,5.7,2.3],[85,0,"virginica",7.7,3.0,6.1,2.3],[86,0,"virginica",6.9,3.1,5.1,2.3],[87,0,"virginica",6.8,3.2,5.9,2.3],[88,0,"virginica",6.7,3.0,5.2,2.3],[89,0,"virginica",6.2,3.4,5.4,2.3],[90,1,"setosa",5.4,3.9,1.7,0.4],[91,1,"setosa",5.7,4.4,1.5,0.4],[92,1,"setosa",5.4,3.9,1.3,0.4],[93,1,"setosa",5.1,3.7,1.5,0.4],[94,1,"setosa",5.0,3.4,1.6,0.4],[95,1,"setosa",5.4,3.4,1.5,0.4],[96,1,"setosa",5.1,3.8,1.9,0.4],[97,1,"setosa",4.6,3.4,1.4,0.3],[98,1,"setosa",5.1,3.5,1.4,0.3],[99,1,"setosa",5.7,3.8,1.7,0.3],[100,1,"setosa",5.1,3.8,1.5,0.3],[101,1,"setosa",5.0,3.5,1.3,0.3],[102,1,"setosa",4.5,2.3,1.3,0.3],[103,1,"setosa",4.8,3.0,1.4,0.3],[104,0,"virginica",6.5,3.2,5.1,2.0],[105,0,"virginica",5.7,2.5,5.0,2.0],[106,0,"virginica",5.6,2.8,4.9,2.0],[107,0,"virginica",7.7,2.8,6.7,2.0],[108,0,"virginica",7.9,3.8,6.4,2.0],[109,0,"virginica",6.5,3.0,5.2,2.0],[110,0,"versicolor",6.1,2.8,4.7,1.2],[111,0,"versicolor",5.8,2.7,3.9,1.2],[112,0,"versicolor",5.5,2.6,4.4,1.2],[113,0,"versicolor",5.8,2.6,4.0,1.2],[114,0,"versicolor",5.7,3.0,4.2,1.2],[115,0,"virginica",5.8,2.7,5.1,1.9],[116,0,"virginica",6.4,2.7,5.3,1.9],[117,0,"virginica",7.4,2.8,6.1,1.9],[118,0,"virginica",5.8,2.7,5.1,1.9],[119,0,"virginica",6.3,2.5,5.0,1.9],[120,0,"virginica",7.1,3.0,5.9,2.1],[121,0,"virginica",7.6,3.0,6.6,2.1],[122,0,"virginica",6.8,3.0,5.5,2.1],[123,0,"virginica",6.7,3.3,5.7,2.1],[124,0,"virginica",6.4,2.8,5.6,2.1],[125,0,"virginica",6.9,3.1,5.4,2.1],[126,1,"setosa",4.9,3.1,1.5,0.1],[127,1,"setosa",4.8,3.0,1.4,0.1],[128,1,"setosa",4.3,3.0,1.1,0.1],[129,1,"setosa",5.2,4.1,1.5,0.1],[130,1,"setosa",4.9,3.6,1.4,0.1],[131,0,"versicolor",6.3,3.3,4.7,1.6],[132,0,"versicolor",6.0,2.7,5.1,1.6],[133,0,"versicolor",6.0,3.4,4.5,1.6],[134,0,"virginica",7.2,3.0,5.8,1.6],[135,0,"versicolor",5.6,2.5,3.9,1.1],[136,0,"versicolor",5.5,2.4,3.8,1.1],[137,0,"versicolor",5.1,2.5,3.0,1.1],[138,0,"virginica",6.3,3.3,6.0,2.5],[139,0,"virginica",7.2,3.6,6.1,2.5],[140,0,"virginica",6.7,3.3,5.7,2.5],[141,0,"virginica",5.8,2.8,5.1,2.4],[142,0,"virginica",6.3,3.4,5.6,2.4],[143,0,"virginica",6.7,3.1,5.6,2.4],[144,0,"virginica",6.5,3.0,5.8,2.2],[145,0,"virginica",7.7,3.8,6.7,2.2],[146,0,"virginica",6.4,2.8,5.6,2.2],[147,0,"versicolor",6.7,3.0,5.0,1.7],[148,0,"virginica",4.9,2.5,4.5,1.7],[149,1,"setosa",5.0,3.5,1.6,0.6],[150,1,"setosa",5.1,3.3,1.7,0.5]]}'
-
-    requests_mock.post(url=ANY, content=response_data)
+def test_non_arrow_format_throws_exception(requests_mock: Mocker):
+    response_data = b'S{"metadata":{"computedTime":1627978857810,"resultComputationMetadata":{"submitTimeMillis":1627978856578,"startTimeMillis":1627978856580,"finishResolveDataFrameTimeMillis":1627978857302,"finishTimeMillis":1627978857763,"estimatedResultSizeOnHeapInBytes":32296,"cacheType":"NO_CACHE","initialDataframeResolutionType":"BUILT_INITIAL_SPARK_SET_AND_DF","complexDataframeResolutionType":"NO_COMPLEX_TRANSFORMATIONS","setDescription":{"type":"sql","parentsByParam":{"/Global/Foundry Operations/Foundry Support/iris-167312679":{"type":"initialwithtransaction","identifier":"ri.foundry.main.dataset.14703427-09ab-4c9c-b036-6926b34d150b:master","transaction":"ri.foundry.main.transaction.0000003a-a437-fec8-95b1-0872dc6a0991","schemaId":"00000003-d596-797c-9663-e8970c07d296","viewMetadataId":null,"maybeStartTransaction":"ri.foundry.main.transaction.0000003a-a437-fec8-95b1-0872dc6a0991"}},"sqlQuery":"SELECT * FROM ${/Global/Foundry Operations/Foundry Support/iris-167312679}"},"queryMetricMetadata":{"queueSubmittedTimeMillis":1627978856263,"wasPunted":false},"traceId":"65a45518d71a3922","saveTraceId":"1ae3ca3cbb85ca39","latitudeQueryDescription":{"humanReadableDescription":null,"metadata":{"Skip the non-contour backend cache":"false","UserId":"3c8fbda5-686e-4fcb-ad52-d95e4281d99f","GraphId":"","NodeId":"","RefRid":"","SourceId":"foundry-sql-server"},"sourceMetadata":{"graphId":null,"nodeId":null,"refRid":null,"refParentRid":null,"sourceId":"foundry-sql-server","sparkReporterOwningRid":null,"resourceManagementAttributionRid":null,"userId":"3c8fbda5-686e-4fcb-ad52-d95e4281d99f","datasetRids":["ri.foundry.main.dataset.14703427-09ab-4c9c-b036-6926b34d150b"],"lsdHash":"01b919b1f5528a8895d161da41b4d55d","lsdHashWithMetadataScrubbed":"9c4501650954bcc765e2c8b6fd2920c5","lsdHashWithDatasetAndMetadataScrubbed":"38d9cc6b14c2d21ac287b53050ebc9aa","unresolvedLsdHash":null,"unresolvedLsdHashWithMetadataScrubbed":null,"unresolvedLsdHashWithDatasetAndMetadataScrubbed":null},"trimmedDatasetRids":[],"requestTraceId":"b2a7f6e4f8e68d97","requestTimeMillis":1627978856150},"backendMetricsTag":"foundrysqlserver-contour-backend-foundry-0","backendGroupMetricsTag":"foundry-sql-server-modules","groupProducerMetricsTag":"foundrysqlserver","numberOfTasks":null,"numberOfStages":null},"computedVersion":"9.206.0","warningMessage":null,"resultId":null,"rowCount":150,"columns":["id","is_setosa","species","sepal_length","sepal_width","petal_length","petal_width"],"columnTypes":[{"type":"INTEGER","name":"id","nullable":true,"customMetadata":{}},{"type":"INTEGER","name":"is_setosa","nullable":true,"customMetadata":{}},{"type":"STRING","name":"species","nullable":true,"customMetadata":{}},{"type":"DOUBLE","name":"sepal_length","nullable":true,"customMetadata":{}},{"type":"DOUBLE","name":"sepal_width","nullable":true,"customMetadata":{}},{"type":"DOUBLE","name":"petal_length","nullable":true,"customMetadata":{}},{"type":"DOUBLE","name":"petal_width","nullable":true,"customMetadata":{}}]},"rows":[[1,1,"setosa",5.1,3.5,1.4,0.2],[2,1,"setosa",4.9,3.0,1.4,0.2],[3,1,"setosa",4.7,3.2,1.3,0.2],[4,1,"setosa",4.6,3.1,1.5,0.2],[5,1,"setosa",5.0,3.6,1.4,0.2],[6,1,"setosa",5.0,3.4,1.5,0.2],[7,1,"setosa",4.4,2.9,1.4,0.2],[8,1,"setosa",5.4,3.7,1.5,0.2],[9,1,"setosa",4.8,3.4,1.6,0.2],[10,1,"setosa",5.8,4.0,1.2,0.2],[11,1,"setosa",5.4,3.4,1.7,0.2],[12,1,"setosa",4.6,3.6,1.0,0.2],[13,1,"setosa",4.8,3.4,1.9,0.2],[14,1,"setosa",5.0,3.0,1.6,0.2],[15,1,"setosa",5.2,3.5,1.5,0.2],[16,1,"setosa",5.2,3.4,1.4,0.2],[17,1,"setosa",4.7,3.2,1.6,0.2],[18,1,"setosa",4.8,3.1,1.6,0.2],[19,1,"setosa",5.5,4.2,1.4,0.2],[20,1,"setosa",4.9,3.1,1.5,0.2],[21,1,"setosa",5.0,3.2,1.2,0.2],[22,1,"setosa",5.5,3.5,1.3,0.2],[23,1,"setosa",4.4,3.0,1.3,0.2],[24,1,"setosa",5.1,3.4,1.5,0.2],[25,1,"setosa",4.4,3.2,1.3,0.2],[26,1,"setosa",5.1,3.8,1.6,0.2],[27,1,"setosa",4.6,3.2,1.4,0.2],[28,1,"setosa",5.3,3.7,1.5,0.2],[29,1,"setosa",5.0,3.3,1.4,0.2],[30,0,"versicolor",6.4,3.2,4.5,1.5],[31,0,"versicolor",6.9,3.1,4.9,1.5],[32,0,"versicolor",6.5,2.8,4.6,1.5],[33,0,"versicolor",5.9,3.0,4.2,1.5],[34,0,"versicolor",5.6,3.0,4.5,1.5],[35,0,"versicolor",6.2,2.2,4.5,1.5],[36,0,"versicolor",6.3,2.5,4.9,1.5],[37,0,"versicolor",6.0,2.9,4.5,1.5],[38,0,"versicolor",5.4,3.0,4.5,1.5],[39,0,"versicolor",6.7,3.1,4.7,1.5],[40,0,"virginica",6.0,2.2,5.0,1.5],[41,0,"virginica",6.3,2.8,5.1,1.5],[42,0,"versicolor",5.9,3.2,4.8,1.8],[43,0,"virginica",6.3,2.9,5.6,1.8],[44,0,"virginica",7.3,2.9,6.3,1.8],[45,0,"virginica",6.7,2.5,5.8,1.8],[46,0,"virginica",6.5,3.0,5.5,1.8],[47,0,"virginica",6.3,2.7,4.9,1.8],[48,0,"virginica",7.2,3.2,6.0,1.8],[49,0,"virginica",6.2,2.8,4.8,1.8],[50,0,"virginica",6.1,3.0,4.9,1.8],[51,0,"virginica",6.4,3.1,5.5,1.8],[52,0,"virginica",6.0,3.0,4.8,1.8],[53,0,"virginica",5.9,3.0,5.1,1.8],[54,0,"versicolor",5.5,2.3,4.0,1.3],[55,0,"versicolor",5.7,2.8,4.5,1.3],[56,0,"versicolor",6.6,2.9,4.6,1.3],[57,0,"versicolor",5.6,2.9,3.6,1.3],[58,0,"versicolor",6.1,2.8,4.0,1.3],[59,0,"versicolor",6.4,2.9,4.3,1.3],[60,0,"versicolor",6.3,2.3,4.4,1.3],[61,0,"versicolor",5.6,3.0,4.1,1.3],[62,0,"versicolor",5.5,2.5,4.0,1.3],[63,0,"versicolor",5.6,2.7,4.2,1.3],[64,0,"versicolor",5.7,2.9,4.2,1.3],[65,0,"versicolor",6.2,2.9,4.3,1.3],[66,0,"versicolor",5.7,2.8,4.1,1.3],[67,0,"versicolor",7.0,3.2,4.7,1.4],[68,0,"versicolor",5.2,2.7,3.9,1.4],[69,0,"versicolor",6.1,2.9,4.7,1.4],[70,0,"versicolor",6.7,3.1,4.4,1.4],[71,0,"versicolor",6.6,3.0,4.4,1.4],[72,0,"versicolor",6.8,2.8,4.8,1.4],[73,0,"versicolor",6.1,3.0,4.6,1.4],[74,0,"virginica",6.1,2.6,5.6,1.4],[75,0,"versicolor",4.9,2.4,3.3,1.0],[76,0,"versicolor",5.0,2.0,3.5,1.0],[77,0,"versicolor",6.0,2.2,4.0,1.0],[78,0,"versicolor",5.8,2.7,4.1,1.0],[79,0,"versicolor",5.7,2.6,3.5,1.0],[80,0,"versicolor",5.5,2.4,3.7,1.0],[81,0,"versicolor",5.0,2.3,3.3,1.0],[82,0,"virginica",6.4,3.2,5.3,2.3],[83,0,"virginica",7.7,2.6,6.9,2.3],[84,0,"virginica",6.9,3.2,5.7,2.3],[85,0,"virginica",7.7,3.0,6.1,2.3],[86,0,"virginica",6.9,3.1,5.1,2.3],[87,0,"virginica",6.8,3.2,5.9,2.3],[88,0,"virginica",6.7,3.0,5.2,2.3],[89,0,"virginica",6.2,3.4,5.4,2.3],[90,1,"setosa",5.4,3.9,1.7,0.4],[91,1,"setosa",5.7,4.4,1.5,0.4],[92,1,"setosa",5.4,3.9,1.3,0.4],[93,1,"setosa",5.1,3.7,1.5,0.4],[94,1,"setosa",5.0,3.4,1.6,0.4],[95,1,"setosa",5.4,3.4,1.5,0.4],[96,1,"setosa",5.1,3.8,1.9,0.4],[97,1,"setosa",4.6,3.4,1.4,0.3],[98,1,"setosa",5.1,3.5,1.4,0.3],[99,1,"setosa",5.7,3.8,1.7,0.3],[100,1,"setosa",5.1,3.8,1.5,0.3],[101,1,"setosa",5.0,3.5,1.3,0.3],[102,1,"setosa",4.5,2.3,1.3,0.3],[103,1,"setosa",4.8,3.0,1.4,0.3],[104,0,"virginica",6.5,3.2,5.1,2.0],[105,0,"virginica",5.7,2.5,5.0,2.0],[106,0,"virginica",5.6,2.8,4.9,2.0],[107,0,"virginica",7.7,2.8,6.7,2.0],[108,0,"virginica",7.9,3.8,6.4,2.0],[109,0,"virginica",6.5,3.0,5.2,2.0],[110,0,"versicolor",6.1,2.8,4.7,1.2],[111,0,"versicolor",5.8,2.7,3.9,1.2],[112,0,"versicolor",5.5,2.6,4.4,1.2],[113,0,"versicolor",5.8,2.6,4.0,1.2],[114,0,"versicolor",5.7,3.0,4.2,1.2],[115,0,"virginica",5.8,2.7,5.1,1.9],[116,0,"virginica",6.4,2.7,5.3,1.9],[117,0,"virginica",7.4,2.8,6.1,1.9],[118,0,"virginica",5.8,2.7,5.1,1.9],[119,0,"virginica",6.3,2.5,5.0,1.9],[120,0,"virginica",7.1,3.0,5.9,2.1],[121,0,"virginica",7.6,3.0,6.6,2.1],[122,0,"virginica",6.8,3.0,5.5,2.1],[123,0,"virginica",6.7,3.3,5.7,2.1],[124,0,"virginica",6.4,2.8,5.6,2.1],[125,0,"virginica",6.9,3.1,5.4,2.1],[126,1,"setosa",4.9,3.1,1.5,0.1],[127,1,"setosa",4.8,3.0,1.4,0.1],[128,1,"setosa",4.3,3.0,1.1,0.1],[129,1,"setosa",5.2,4.1,1.5,0.1],[130,1,"setosa",4.9,3.6,1.4,0.1],[131,0,"versicolor",6.3,3.3,4.7,1.6],[132,0,"versicolor",6.0,2.7,5.1,1.6],[133,0,"versicolor",6.0,3.4,4.5,1.6],[134,0,"virginica",7.2,3.0,5.8,1.6],[135,0,"versicolor",5.6,2.5,3.9,1.1],[136,0,"versicolor",5.5,2.4,3.8,1.1],[137,0,"versicolor",5.1,2.5,3.0,1.1],[138,0,"virginica",6.3,3.3,6.0,2.5],[139,0,"virginica",7.2,3.6,6.1,2.5],[140,0,"virginica",6.7,3.3,5.7,2.5],[141,0,"virginica",5.8,2.8,5.1,2.4],[142,0,"virginica",6.3,3.4,5.6,2.4],[143,0,"virginica",6.7,3.1,5.6,2.4],[144,0,"virginica",6.5,3.0,5.8,2.2],[145,0,"virginica",7.7,3.8,6.7,2.2],[146,0,"virginica",6.4,2.8,5.6,2.2],[147,0,"versicolor",6.7,3.0,5.0,1.7],[148,0,"virginica",4.9,2.5,4.5,1.7],[149,1,"setosa",5.0,3.5,1.6,0.6],[150,1,"setosa",5.1,3.3,1.7,0.5]]}'  # noqa: E501
 
+    requests_mock.get(url=ANY, content=response_data)
+    client = FoundryRestClient()
     with pytest.raises(FoundrySqlSerializationFormatNotImplementedError):
-        sql_client._read_results_arrow("statement-id")
+        client._read_fsql_query_results_arrow("queryId")
 
 
-def test_read_arrow_optional_polars(requests_mock: Mocker, sql_client):
-    response_data = b'A\xff\xff\xff\xff\xb0\x01\x00\x00\x10\x00\x00\x00\x00\x00\n\x00\x0e\x00\x06\x00\r\x00\x08\x00\n\x00\x00\x00\x00\x00\x04\x00\x10\x00\x00\x00\x00\x01\n\x00\x0c\x00\x00\x00\x08\x00\x04\x00\n\x00\x00\x00\x08\x00\x00\x00,\x01\x00\x00\x01\x00\x00\x00\x0c\x00\x00\x00\x08\x00\x0c\x00\x08\x00\x04\x00\x08\x00\x00\x00\x08\x00\x00\x00\x00\x01\x00\x00\xf5\x00\x00\x00{"computedTime":1627977691184,"resultComputationMetadata":null,"computedVersion":null,"warningMessage":null,"resultId":null,"rowCount":null,"columns":["MATNR"],"columnTypes":[{"type":"STRING","name":"MATNR","nullable":true,"customMetadata":{}}]}\x00\x00\x00\x08\x00\x00\x00metadata\x00\x00\x00\x00\x01\x00\x00\x00\x18\x00\x00\x00\x00\x00\x12\x00\x18\x00\x14\x00\x13\x00\x12\x00\x0c\x00\x00\x00\x08\x00\x04\x00\x12\x00\x00\x00\x14\x00\x00\x00\x14\x00\x00\x00\x18\x00\x00\x00\x00\x00\x05\x01\x14\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x04\x00\x04\x00\x04\x00\x00\x00\x05\x00\x00\x00MATNR\x00\x00\x00\x00\x00\x00\x00\xff\xff\xff\xff\x98\x00\x00\x00\x14\x00\x00\x00\x00\x00\x00\x00\x0c\x00\x16\x00\x0e\x00\x15\x00\x10\x00\x04\x00\x0c\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x04\x00\x10\x00\x00\x00\x00\x03\n\x00\x18\x00\x0c\x00\x08\x00\x04\x00\n\x00\x00\x00\x14\x00\x00\x00H\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x03\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x08\x00\x00\x00\x00\x00\x00\x00\x08\x00\x00\x00\x00\x00\x00\x00\x10\x00\x00\x00\x00\x00\x00\x00\x10\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x10\x00\x00\x0000062106-RNA-5UG\xff\xff\xff\xff\x00\x00\x00\x00E'
+def test_read_arrow_optional_polars(requests_mock: Mocker):
+    response_data = b'A\xff\xff\xff\xff\xb0\x01\x00\x00\x10\x00\x00\x00\x00\x00\n\x00\x0e\x00\x06\x00\r\x00\x08\x00\n\x00\x00\x00\x00\x00\x04\x00\x10\x00\x00\x00\x00\x01\n\x00\x0c\x00\x00\x00\x08\x00\x04\x00\n\x00\x00\x00\x08\x00\x00\x00,\x01\x00\x00\x01\x00\x00\x00\x0c\x00\x00\x00\x08\x00\x0c\x00\x08\x00\x04\x00\x08\x00\x00\x00\x08\x00\x00\x00\x00\x01\x00\x00\xf5\x00\x00\x00{"computedTime":1627977691184,"resultComputationMetadata":null,"computedVersion":null,"warningMessage":null,"resultId":null,"rowCount":null,"columns":["MATNR"],"columnTypes":[{"type":"STRING","name":"MATNR","nullable":true,"customMetadata":{}}]}\x00\x00\x00\x08\x00\x00\x00metadata\x00\x00\x00\x00\x01\x00\x00\x00\x18\x00\x00\x00\x00\x00\x12\x00\x18\x00\x14\x00\x13\x00\x12\x00\x0c\x00\x00\x00\x08\x00\x04\x00\x12\x00\x00\x00\x14\x00\x00\x00\x14\x00\x00\x00\x18\x00\x00\x00\x00\x00\x05\x01\x14\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x04\x00\x04\x00\x04\x00\x00\x00\x05\x00\x00\x00MATNR\x00\x00\x00\x00\x00\x00\x00\xff\xff\xff\xff\x98\x00\x00\x00\x14\x00\x00\x00\x00\x00\x00\x00\x0c\x00\x16\x00\x0e\x00\x15\x00\x10\x00\x04\x00\x0c\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x04\x00\x10\x00\x00\x00\x00\x03\n\x00\x18\x00\x0c\x00\x08\x00\x04\x00\n\x00\x00\x00\x14\x00\x00\x00H\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x03\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x08\x00\x00\x00\x00\x00\x00\x00\x08\x00\x00\x00\x00\x00\x00\x00\x10\x00\x00\x00\x00\x00\x00\x00\x10\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x10\x00\x00\x0000062106-RNA-5UG\xff\xff\xff\xff\x00\x00\x00\x00E'  # noqa: E501
+    client = FoundryRestClient()
+    requests_mock.get(url=ANY, content=response_data)
 
-    requests_mock.post(url=ANY, content=response_data)
-
-    arrow_stream = sql_client._read_results_arrow("statement-id")
+    arrow_stream = client._read_fsql_query_results_arrow("queryId")
     pdf = arrow_stream.read_pandas()
     assert pdf.shape == (1, 1)
 
     try:
         import polars as pl
 
-        arrow_stream = sql_client._read_results_arrow("statement-id")
+        arrow_stream = client._read_fsql_query_results_arrow("queryId")
         pa_table = arrow_stream.read_all()
         df = pl.from_arrow(pa_table)
         assert df.shape == (1, 1)
-    except:
-        pass
+    except ImportError:
+        pytest.skip("Polars not installed")
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_smoke(iris_dataset):
-    sql_client = FoundrySqlClient()
-    one_row_one_column = sql_client.query(
+    client = FoundryRestClient()
+    one_row_one_column = client._query_fsql(
         f"SELECT sepal_width FROM `{iris_dataset[1]}` LIMIT 1"
     )
     assert one_row_one_column.shape == (1, 1)
 
 
-@pytest.mark.integration
-def test_legacy_fallback(mocker, iris_dataset, client):
-    from foundry_dev_tools import FoundryRestClient as frc_class
-
-    spy = mocker.spy(frc_class, "query_foundry_sql_legacy")
-    # The query does require SQL compute.
-    # Queries which contain aggregate, join, order by, and filter predicates are not direct read eligible.
-    # and unfortunately returned in JSON Format, not ARROW
-    iris = client.query_foundry_sql(
-        f"SELECT * FROM `{iris_dataset[1]}` order by sepal_width LIMIT 100"
-    )
-    assert iris.shape == (100, 5)
-    spy.assert_called()
-
-
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_exceptions(iris_dataset, iris_no_schema_dataset):
-    with pytest.raises(BranchNotFoundError):
-        sql_client1 = FoundrySqlClient(branch="doesNotExist")
-        sql_client1.query(f"SELECT * FROM `{iris_dataset[1]}` LIMIT 100")
+    client = FoundryRestClient()
+    with pytest.raises(BranchNotFoundError) as exc:
+        client._query_fsql(
+            f"SELECT * FROM `{iris_dataset[1]}` LIMIT 100", branch="doesNotExist"
+        )
+    assert exc.value.dataset_rid == iris_dataset[0]
+    assert exc.value.branch == "doesNotExist"
 
-    client = FoundrySqlClient()
     with pytest.raises(DatasetHasNoSchemaError):
-        client.query(f"SELECT * FROM `{iris_no_schema_dataset[1]}` LIMIT 100")
+        client._query_fsql(f"SELECT * FROM `{iris_no_schema_dataset[1]}` LIMIT 100")
 
-    with pytest.raises(DatasetNotFoundError):
-        client.query("SELECT * FROM `/namespace1/does-not_exists/` LIMIT 100")
+    with pytest.raises(DatasetNotFoundError) as exc:
+        client._query_fsql("SELECT * FROM `/namespace1/does-not_exists/` LIMIT 100")
+    assert exc.value.dataset_rid == "/namespace1/does-not_exists/"
+
+    with pytest.raises(BranchNotFoundError) as exc:
+        client._query_fsql(
+            "SELECT * FROM `ri.foundry.main.dataset.1337fb9d-1234-43c7-b83f-768f2b843b94` LIMIT 100"
+        )
+    assert (
+        exc.value.dataset_rid
+        == "ri.foundry.main.dataset.1337fb9d-1234-43c7-b83f-768f2b843b94"
+    )
+    assert exc.value.branch == "master"
 
     with pytest.raises(FoundrySqlQueryFailedError):
-        client.query(f"SELECT foo, bar, FROM `{iris_dataset[1]}` LIMIT 100")
+        client._query_fsql(f"SELECT foo, bar, FROM `{iris_dataset[1]}` LIMIT 100")
+
+
+def test_legacy_fallback(mocker):
+    mocker.patch(
+        "foundry_dev_tools.foundry_api_client.FoundryRestClient._query_fsql"
+    ).side_effect = FoundrySqlSerializationFormatNotImplementedError()
+    query_foundry_sql_legacy_spy = mocker.patch(
+        "foundry_dev_tools.foundry_api_client.FoundryRestClient.query_foundry_sql_legacy"
+    )
+    client = FoundryRestClient()
+
+    client.query_foundry_sql("SELECT * FROM `test`")
+
+    query_foundry_sql_legacy_spy.assert_called()
```

### Comparing `foundry-dev-tools-1.0.9/tests/test_fsspec_impl.py` & `foundry-dev-tools-1.1/tests/test_fsspec_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 import fsspec
 import pandas as pd
 import pytest
 from fsspec import register_implementation
 from pandas._testing import assert_frame_equal
 
-import foundry_dev_tools.config
-from foundry_dev_tools import FoundryRestClient
-from foundry_dev_tools.foundry_api_client import DatasetHasOpenTransactionError
+from foundry_dev_tools.foundry_api_client import (
+    DatasetHasOpenTransactionError,
+    FoundryRestClient,
+)
 from foundry_dev_tools.fsspec_impl import (
-    _correct_directories,
-    _file_or_directory,
-    _get_top_level_folder,
     FoundryDatasetPathInUrlNotSupportedError,
     FoundryDeleteInNotSupportedTransactionError,
     FoundryFileSystem,
     FoundrySimultaneousOpenTransactionError,
+    _correct_directories,
+    _file_or_directory,
+    _get_top_level_folder,
 )
-
 from tests.utils import generic_upload_dataset_if_not_exists
 
 register_implementation("foundry", FoundryFileSystem)
 
 
 @pytest.fixture()
 def random_file():
@@ -67,15 +67,21 @@
             client=FoundryRestClient(),
             name="fsspec_write_test_folder_v1",
             upload_folder=None,
             foundry_schema=None,
         )
         yield fsspec_write_test_folder
     else:
-        yield "fsspec_write_test_folder-rid", "fsspec_write_test_folder-path", None, "fsspec_write_test_folder-branch", False
+        yield (
+            "fsspec_write_test_folder-rid",
+            "fsspec_write_test_folder-path",
+            None,
+            "fsspec_write_test_folder-branch",
+            False,
+        )
 
 
 def folder_setup(rid: str):
     fc = FoundryRestClient()
     try:
         transaction_id = fc.open_transaction(rid, mode="SNAPSHOT", branch="master")
     except DatasetHasOpenTransactionError as exc:
@@ -137,15 +143,15 @@
             "spark",
         )
         == "file"
     )
 
 
 def test_correct_for_folder():
-    input = [
+    _input = [
         {
             "logicalPath": "empty_file.txt",
             "physicalPath": "transaction-1",
             "physicalUri": None,
             "transactionRid": "t1",
             "fileMetadata": {"length": 0},
             "isOpen": False,
@@ -194,15 +200,15 @@
             "transactionRid": "t1",
             "fileMetadata": {"length": 7},
             "isOpen": False,
             "timeModified": "2022-03-18T19:32:18.364Z",
         },
     ]
 
-    res = _correct_directories(input)
+    res = _correct_directories(_input)
 
     assert {
         "name": "empty_file.txt",
         "size": 0,
         "type": "file",
         "time_modified": "2022-03-18T19:32:20.878Z",
         "transaction_rid": "t1",
@@ -228,19 +234,20 @@
         "name": "folder",
         "size": 0,
         "type": "directory",
         "time_modified": "2022-03-18T19:32:19.188Z",
         "transaction_rid": "t1",
         "is_open": False,
     } in res
-    assert len(res) == 4
+    EXPECTED_LENGTH = 4
+    assert len(res) == EXPECTED_LENGTH
 
 
 def test_correct_for_folder_in_subfolder_file():
-    input = [
+    _input = [
         {
             "logicalPath": "folder/sub_folder/1_in_folder.txt",
             "physicalPath": "93e9675d-1c5c-4cd7-ac01-a5a7d98ef25f/000000d5-c4e6-150d-a606-32540fd23fe2/",
             "physicalUri": None,
             "transactionRid": "t1",
             "fileMetadata": {"length": 0},
             "isOpen": False,
@@ -253,15 +260,15 @@
             "transactionRid": "t2",
             "fileMetadata": {"length": 42},
             "isOpen": False,
             "timeModified": "2022-03-21T11:27:01.858Z",
         },
     ]
 
-    res = _correct_directories(input, subfolder_prefix="folder/sub_folder")
+    res = _correct_directories(_input, subfolder_prefix="folder/sub_folder")
 
     assert {
         "name": "folder/sub_folder/1_in_folder.txt",
         "size": 0,
         "type": "file",
         "time_modified": "2022-03-21T11:26:56.819Z",
         "transaction_rid": "t1",
@@ -274,15 +281,15 @@
         "time_modified": "2022-03-21T11:27:01.858Z",
         "transaction_rid": "t2",
         "is_open": False,
     } in res
 
 
 def test_correct_subfolder():
-    input = [
+    _input = [
         {
             "logicalPath": "folder/sub_folder/1_in_folder.txt",
             "physicalPath": "93e9675d-1c5c-4cd7-ac01-a5a7d98ef25f/000000d5-c4e6-150d-a606-32540fd23fe2/",
             "physicalUri": None,
             "transactionRid": "t1",
             "fileMetadata": {"length": 0},
             "isOpen": False,
@@ -304,15 +311,15 @@
             "transactionRid": "t3",
             "fileMetadata": {"length": 0},
             "isOpen": False,
             "timeModified": "2022-03-21T11:28:01.858Z",
         },
     ]
 
-    res = _correct_directories(input, subfolder_prefix="folder")
+    res = _correct_directories(_input, subfolder_prefix="folder")
 
     assert {
         "name": "folder/sub_folder",
         "size": 0,
         "type": "directory",
         "time_modified": "2022-03-21T11:26:56.819Z",
         "transaction_rid": "t1",
@@ -326,54 +333,58 @@
         "time_modified": "2022-03-21T11:28:01.858Z",
         "transaction_rid": "t3",
         "is_open": False,
     } in res
 
 
 def test_correct_subfolder_removesuffix():
-    input = [
+    _input = [
         {
             "logicalPath": "data/LipidsDataset/test/biological_data.jbl",
-            "physicalPath": "d63c3ad9-89ef-49f4-a380-b7698ed7c978/0000013b-7c77-7852-997d-e7df7a003d49/ca2d4ed0-38b3-4fb5-937c-87925c76eb5a",
+            "physicalPath": "d63c3ad9-89ef-49f4-a380-b7698ed7c978/0000013b-7c77-7852-997d-e7df7a003d49/ca2d4ed0-38b3-4f"
+            "b5-937c-87925c76eb5a",
             "physicalUri": None,
             "transactionRid": "ri.foundry.main.transaction.0000013b-7c77-7852-997d-e7df7a003d49",
             "fileMetadata": {"length": 2939},
             "isOpen": False,
             "timeModified": "2023-01-30T09:23:55.302Z",
         },
         {
             "logicalPath": "data/LipidsDataset/test/experiment_definition.jbl",
-            "physicalPath": "d63c3ad9-89ef-49f4-a380-b7698ed7c978/0000013b-7c77-7852-997d-e7df7a003d49/623dab8f-8ded-45b2-bcf5-3363d4570fbf",
+            "physicalPath": "d63c3ad9-89ef-49f4-a380-b7698ed7c978/0000013b-7c77-7852-997d-e7df7a003d49/623dab8f-8ded-45"
+            "b2-bcf5-3363d4570fbf",
             "physicalUri": None,
             "transactionRid": "ri.foundry.main.transaction.0000013b-7c77-7852-997d-e7df7a003d49",
             "fileMetadata": {"length": 2710},
             "isOpen": False,
             "timeModified": "2023-01-30T09:23:54.323Z",
         },
         {
             "logicalPath": "data/LipidsDataset/test/ionisable_lipids.jbl",
-            "physicalPath": "d63c3ad9-89ef-49f4-a380-b7698ed7c978/0000013b-7c77-7852-997d-e7df7a003d49/c7c0d168-3369-41f6-9e23-8b5dafb7e238",
+            "physicalPath": "d63c3ad9-89ef-49f4-a380-b7698ed7c978/0000013b-7c77-7852-997d-e7df7a003d49/c7c0d168-3369-41"
+            "f6-9e23-8b5dafb7e238",
             "physicalUri": None,
             "transactionRid": "ri.foundry.main.transaction.0000013b-7c77-7852-997d-e7df7a003d49",
             "fileMetadata": {"length": 3005},
             "isOpen": False,
             "timeModified": "2023-01-30T09:23:53.735Z",
         },
         {
             "logicalPath": "data/LipidsDataset/test/pc_data.jbl",
-            "physicalPath": "d63c3ad9-89ef-49f4-a380-b7698ed7c978/0000013b-7c77-7852-997d-e7df7a003d49/db3aadbf-f892-4960-b23e-a8129f2afe0a",
+            "physicalPath": "d63c3ad9-89ef-49f4-a380-b7698ed7c978/0000013b-7c77-7852-997d-e7df7a003d49/db3aadbf-f892-49"
+            "60-b23e-a8129f2afe0a",
             "physicalUri": None,
             "transactionRid": "ri.foundry.main.transaction.0000013b-7c77-7852-997d-e7df7a003d49",
             "fileMetadata": {"length": 1887},
             "isOpen": False,
             "timeModified": "2023-01-30T09:23:54.781Z",
         },
     ]
 
-    res = _correct_directories(input, subfolder_prefix="data/LipidsDataset")
+    res = _correct_directories(_input, subfolder_prefix="data/LipidsDataset")
     assert {
         "name": "data/LipidsDataset/test",
         "size": 0,
         "type": "directory",
         "time_modified": "2023-01-30T09:23:53.735Z",
         "transaction_rid": "ri.foundry.main.transaction.0000013b-7c77-7852-997d-e7df7a003d49",
         "is_open": False,
@@ -389,76 +400,70 @@
     )
     assert (
         FoundryFileSystem._strip_protocol(
             "foundry://ri.foundry.main.dataset.fee62053-77ed-4617-bd01-fc2538366c3f/test.csv"
         )
         == "test.csv"
     )
-    assert (
-        FoundryFileSystem._strip_protocol(
-            "foundry://ri.foundry.main.dataset.fee62053-77ed-4617-bd01-fc2538366c3f/"
-        )
-        == ""
+    assert not FoundryFileSystem._strip_protocol(
+        "foundry://ri.foundry.main.dataset.fee62053-77ed-4617-bd01-fc2538366c3f/"
     )
-    assert (
-        FoundryFileSystem._strip_protocol(
-            "foundry://ri.foundry.main.dataset.fee62053-77ed-4617-bd01-fc2538366c3f"
-        )
-        == ""
+    assert not FoundryFileSystem._strip_protocol(
+        "foundry://ri.foundry.main.dataset.fee62053-77ed-4617-bd01-fc2538366c3f"
     )
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_clean_snapshot_transaction(empty_dataset):
     rid = empty_dataset[0]
     fs = FoundryFileSystem(dataset=rid, branch="master")
     with fs.start_transaction(transaction_type="SNAPSHOT") as transaction:
         assert transaction.transaction_rid is not None
         assert transaction.transaction_type == "SNAPSHOT"
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_read_with_dataset_alias(fsspec_test_folder):
     base_path = fsspec_test_folder[1]
     fs = FoundryFileSystem(dataset=base_path, branch="master")
 
     with fs.open("folder/sub_folder/3_in_folder.txt") as f:
         assert f.read().decode("UTF-8") == "content"
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_write(fsspec_write_test_folder):
     with fsspec.open(
         f"foundry://{fsspec_write_test_folder[0]}/test.txt",
         "w",
     ) as f:
         f.write("content")
     with fsspec.open(
         f"foundry://{fsspec_write_test_folder[0]}/test.txt",
         "r",
     ) as f:
         content = f.read()
     assert content == "content"
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_read_single_csv(fsspec_test_folder):
     df = pd.read_csv(
         f"foundry://{fsspec_test_folder[0]}/test1.csv",
     )
     assert df.shape == (1, 1)
 
     df = pd.read_csv(
         f"foundry://{fsspec_test_folder[0]}/test1.csv",
         storage_options={"branch": "master"},
     )
     assert df.shape == (1, 1)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_read_dask_pyarrow(complex_dataset_fixture):
     import dask
     import dask.dataframe as dd
 
     dask.config.set(scheduler="synchronous")
 
     df = dd.read_parquet(
@@ -467,39 +472,39 @@
         engine="pyarrow",
     )
     unique = df["string_column"].unique().compute()
     print(unique)
     print(df.shape)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_read_dask_fastparquet(complex_dataset_fixture):
     import dask.dataframe as dd
 
     df = dd.read_parquet(
         f"foundry://{complex_dataset_fixture}/spark",
         storage_options={"branch": "master"},
         engine="fastparquet",
     )
     unique = df["string_column"].unique().compute()
     print(unique)
     print(df.shape)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_read_write_parquet(fsspec_write_test_folder):
     df = pd.DataFrame(data={"col1": ["row1", "row2"]})
     df.to_parquet(f"foundry://{fsspec_write_test_folder[0]}/test.parquet")
     from_foundry = pd.read_parquet(
         f"foundry://{fsspec_write_test_folder[0]}/test.parquet"
     )
     assert_frame_equal(from_foundry, df)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_write_transaction(random_file, fsspec_write_test_folder):
     random_file_1 = random_file.get()
     random_file_2 = random_file.get()
     random_file_3 = random_file.get()
     fs = FoundryFileSystem(
         dataset=fsspec_write_test_folder[0],
         branch="master",
@@ -524,15 +529,15 @@
             with fs.open(random_file_3, "w") as f:
                 f.write("content")
             raise KeyboardInterrupt
     except KeyboardInterrupt:
         assert not fs.exists(random_file_3)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_delete_simple(random_file, fsspec_write_test_folder):
     file = random_file.get()
     fs = FoundryFileSystem(
         dataset=fsspec_write_test_folder[0],
         branch="master",
     )
     with fs.open(file, "w") as f:
@@ -540,15 +545,15 @@
     assert fs.exists(file)
 
     fs.rm(file)
 
     assert not fs.exists(file)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_delete_simple_folder(random_file, fsspec_write_test_folder):
     random_folder = random_file.get()
     file1 = random_file.get()
     file1_in_folder = f"{random_folder}/{file1}"
     file2 = random_file.get()
     file2_in_folder = f"{random_folder}/{file2}"
     fs = FoundryFileSystem(
@@ -568,15 +573,15 @@
         fs.rm(random_folder)
     assert fs.exists(random_folder)
 
     fs.rm(random_folder, recursive=True)
     assert not fs.exists(random_folder)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_delete_from_open_transaction(fsspec_write_test_folder):
     from_previous_t = (
         "".join(random.choices(string.ascii_uppercase + string.digits, k=5)) + ".txt"
     )
     file = "".join(random.choices(string.ascii_uppercase + string.digits, k=5)) + ".txt"
     fs = FoundryFileSystem(
         dataset=fsspec_write_test_folder[0],
@@ -593,15 +598,15 @@
     assert not fs.exists(file)
     assert fs.exists(from_previous_t)
     with fs.start_transaction(transaction_type="DELETE"):
         fs.rm(from_previous_t)
     assert not fs.exists(from_previous_t)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_delete_folder(random_file, fsspec_write_test_folder):
     random_folder = random_file.get()
     random_file = random_file.get()
     file_in_folder = f"{random_folder}/test/{random_file}"
     fs = FoundryFileSystem(
         dataset=fsspec_write_test_folder[0],
         branch="master",
@@ -613,67 +618,68 @@
             fs.rm(random_folder)
         fs.rm(random_folder, recursive=True)
         with pytest.raises(FileNotFoundError):
             fs.rm(random_folder + "/nofile")
     assert not fs.exists(file_in_folder)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_transaction_already_open_throws(random_file, fsspec_write_test_folder):
     random_folder = random_file.get()
     fs = FoundryFileSystem(
         dataset=fsspec_write_test_folder[0],
         branch="master",
         transaction_backoff=False,
     )
     with fs.transaction:
         with fs.open(random_folder, "w") as f:
             f.write("content")
-        with pytest.raises(FoundrySimultaneousOpenTransactionError) as exc_info:
-            with fsspec.open(
-                f"foundry://{fsspec_write_test_folder[0]}/test.txt",
-                "w",
-            ) as f:
-                f.write("content")
+        with pytest.raises(
+            FoundrySimultaneousOpenTransactionError
+        ) as exc_info, fsspec.open(
+            f"foundry://{fsspec_write_test_folder[0]}/test.txt",
+            "w",
+        ) as f:
+            f.write("content")
         assert exc_info.value.dataset_rid == fsspec_write_test_folder[0]
         assert exc_info.value.open_transaction_rid == fs._transaction.transaction_rid
 
 
 @patch(
-    "foundry_dev_tools.FoundryRestClient.get_dataset_identity",
+    "foundry_dev_tools.foundry_api_client.FoundryRestClient.get_dataset_identity",
     MagicMock(),
 )
 def test_custom_token_is_used():
     fs = FoundryFileSystem(
         dataset="ri.foundry.main.dataset.fake1bb5-be92-4ad9-aa3e-07c161751234",
         branch="master",
-        token="super-secret-token",
+        token="super-secret-token",  # noqa: S106
     )
     assert fs.api._config["jwt"] == "super-secret-token"
     assert fs.api._headers()["Authorization"] == "Bearer super-secret-token"
 
     parsed = FoundryFileSystem._get_kwargs_from_urls(
         "foundry://:super-secret-token@ri.foundry.main.dataset.fake1bb5-be92-4ad9-aa3e-07c161751234/test.txt"
     )
-    assert parsed["token"] == "super-secret-token"
+    assert parsed["token"] == "super-secret-token"  # noqa: S105
     assert (
         parsed["dataset"]
         == "ri.foundry.main.dataset.fake1bb5-be92-4ad9-aa3e-07c161751234"
     )
 
 
 @patch(
-    "foundry_dev_tools.FoundryRestClient.get_dataset_identity",
+    "foundry_dev_tools.foundry_api_client.FoundryRestClient.get_dataset_identity",
     MagicMock(),
 )
 def test_branch_extracted():
     parsed = FoundryFileSystem._get_kwargs_from_urls(
         "foundry://dev-iteration:super-secret-token@ri.foundry.main.dataset.fake1bb5-be92-4ad9-aa3e-07c161751234/test.txt"
     )
-    assert parsed["token"] == "super-secret-token"
+    assert parsed["token"] == "super-secret-token"  # noqa: S105
     assert (
         parsed["dataset"]
         == "ri.foundry.main.dataset.fake1bb5-be92-4ad9-aa3e-07c161751234"
     )
     assert parsed["branch"] == "dev-iteration"
 
     parsed = FoundryFileSystem._get_kwargs_from_urls(
@@ -695,15 +701,15 @@
         == "ri.foundry.main.dataset.fake1bb5-be92-4ad9-aa3e-07c161751234"
     )
     assert parsed["branch"] == "dev-iteration"
 
     parsed = FoundryFileSystem._get_kwargs_from_urls(
         "foundry://:super-secret-token@ri.foundry.main.dataset.fake1bb5-be92-4ad9-aa3e-07c161751234/test.txt"
     )
-    assert parsed["token"] == "super-secret-token"
+    assert parsed["token"] == "super-secret-token"  # noqa: S105
     assert (
         parsed["dataset"]
         == "ri.foundry.main.dataset.fake1bb5-be92-4ad9-aa3e-07c161751234"
     )
     assert "branch" not in parsed
 
     parsed = FoundryFileSystem._get_kwargs_from_urls(
@@ -729,33 +735,33 @@
     with pytest.raises(FoundryDatasetPathInUrlNotSupportedError):
         FoundryFileSystem._get_kwargs_from_urls(
             "foundry:///path/to//fsspec_write_test_folder/test.txt"
         )
 
 
 @patch(
-    "foundry_dev_tools.FoundryRestClient.get_dataset_identity",
+    "foundry_dev_tools.foundry_api_client.FoundryRestClient.get_dataset_identity",
     MagicMock(),
 )
 def test_appending_not_implemented_raises():
     fs = FoundryFileSystem(
         dataset="ri.foundry.main.dataset.fake1bb5-be92-4ad9-aa3e-07c161751234",
         branch="master",
-        token="super-secret-token",
+        token="super-secret-token",  # noqa: S106
     )
     with pytest.raises(NotImplementedError):
         fs.open("test", mode="a")
 
 
 @patch(
-    "foundry_dev_tools.FoundryRestClient.get_dataset_identity",
+    "foundry_dev_tools.foundry_api_client.FoundryRestClient.get_dataset_identity",
     MagicMock(),
 )
 @patch(
-    "foundry_dev_tools.FoundryRestClient.list_dataset_files",
+    "foundry_dev_tools.foundry_api_client.FoundryRestClient.list_dataset_files",
     MagicMock(
         return_value=[
             {
                 "logicalPath": "empty_file.txt",
                 "physicalPath": "transaction-1",
                 "physicalUri": None,
                 "transactionRid": "t1",
@@ -772,30 +778,30 @@
     )
     assert fs.modified("empty_file.txt") == datetime.datetime(
         2022, 3, 18, 19, 32, 20, 878000, tzinfo=datetime.timezone.utc
     )
 
 
 @patch(
-    "foundry_dev_tools.FoundryRestClient.get_dataset_identity",
+    "foundry_dev_tools.foundry_api_client.FoundryRestClient.get_dataset_identity",
     MagicMock(
         return_value={
             "dataset_path": "/path/to/ds",
             "dataset_rid": "ri.foundry.main.dataset.1234",
             "last_transaction_rid": None,
         }
     ),
 )
 def test_listdir_in_empty_dataset():
     fs = FoundryFileSystem(dataset="ri.foundry.main.dataset.1234")
     with pytest.raises(FileNotFoundError):
         fs.listdir("bla/blubdoesnotexists")
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_two_instances(random_file, fsspec_write_test_folder):
     random_file = random_file.get()
     fs = FoundryFileSystem(
         dataset=fsspec_write_test_folder[0],
         branch="master",
     )
     fs_other_instance = FoundryFileSystem(
@@ -813,51 +819,56 @@
         assert fs_same_instance._intrans is True
         assert fs_same_instance.exists(random_file) is True
 
         assert fs_other_instance._intrans is False
         assert fs_other_instance.exists(random_file) is False
 
     fs.delete(random_file)
-    with pytest.raises(FileNotFoundError):
-        with fs_other_instance.open(random_file, "r") as f:
-            f.read()
+    with pytest.raises(FileNotFoundError), fs_other_instance.open(
+        random_file, "r"
+    ) as f:
+        f.read()
 
 
 def test_slash_at_end():
     file_details = [
         {
             "logicalPath": "data/blah/data.csv",
-            "physicalPath": "8324bd10-ffbe-411d-8d70-fe0ca752ab4d/000000e2-a25f-1c31-a804-8308b0d436dd/539aed08-a648-47d3-affc-51e4b6662203",
+            "physicalPath": "8324bd10-ffbe-411d-8d70-fe0ca752ab4d/000000e2-a25f-1c31-a804-8308b0d436dd/539aed08-a648-47"
+            "d3-affc-51e4b6662203",
             "physicalUri": None,
             "transactionRid": "ri.foundry.main.transaction.000000e2-a25f-1c31-a804-8308b0d436dd",
             "fileMetadata": {"length": 4},
             "isOpen": False,
             "timeModified": "2022-04-25T14:08:47.499Z",
         },
         {
             "logicalPath": "data/blub",
-            "physicalPath": "8324bd10-ffbe-411d-8d70-fe0ca752ab4d/000000e2-a395-4c0a-87ce-a60f4d687d55/4948123a-8416-46b5-85aa-aa114f1b43bf",
+            "physicalPath": "8324bd10-ffbe-411d-8d70-fe0ca752ab4d/000000e2-a395-4c0a-87ce-a60f4d687d55/4948123a-8416-46"
+            "b5-85aa-aa114f1b43bf",
             "physicalUri": None,
             "transactionRid": "ri.foundry.main.transaction.000000e2-a395-4c0a-87ce-a60f4d687d55",
             "fileMetadata": {"length": 0},
             "isOpen": False,
             "timeModified": "2022-04-25T14:25:01.722Z",
         },
         {
             "logicalPath": "data/blub/data.csv",
-            "physicalPath": "8324bd10-ffbe-411d-8d70-fe0ca752ab4d/000000e2-a396-ecf1-acaf-464bb5fe5a3e/675883b3-e481-4888-a12b-6707238f5a6a",
+            "physicalPath": "8324bd10-ffbe-411d-8d70-fe0ca752ab4d/000000e2-a396-ecf1-acaf-464bb5fe5a3e/675883b3-e481-48"
+            "88-a12b-6707238f5a6a",
             "physicalUri": None,
             "transactionRid": "ri.foundry.main.transaction.000000e2-a396-ecf1-acaf-464bb5fe5a3e",
             "fileMetadata": {"length": 4},
             "isOpen": False,
             "timeModified": "2022-04-25T14:25:05.420Z",
         },
         {
             "logicalPath": "data/blub/data2.csv",
-            "physicalPath": "8324bd10-ffbe-411d-8d70-fe0ca752ab4d/000000e2-a398-a6f1-ac25-c650ea6dc4c8/6c78deed-b401-4ec2-aab7-bd18d517d225",
+            "physicalPath": "8324bd10-ffbe-411d-8d70-fe0ca752ab4d/000000e2-a398-a6f1-ac25-c650ea6dc4c8/6c78deed-b401-4e"
+            "c2-aab7-bd18d517d225",
             "physicalUri": None,
             "transactionRid": "ri.foundry.main.transaction.000000e2-a398-a6f1-ac25-c650ea6dc4c8",
             "fileMetadata": {"length": 4},
             "isOpen": False,
             "timeModified": "2022-04-25T14:25:09.140Z",
         },
     ]
@@ -881,18 +892,18 @@
         "is_open": False,
     } in res
 
 
 def test_get_top_level_folder():
     assert _get_top_level_folder("data/dog", "data/") == "dog"
     assert _get_top_level_folder("data/dog", "data") == "dog"
-    assert _get_top_level_folder("data/hubabubba", "data/hubabubba") == ""
+    assert not _get_top_level_folder("data/hubabubba", "data/hubabubba")
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_transaction_retry(random_file, fsspec_write_test_folder):
     file_in_thread = random_file.get()
     file = random_file.get()
 
     def run_in_thread():
         fs_inner = FoundryFileSystem(
             dataset=fsspec_write_test_folder[0],
@@ -908,55 +919,54 @@
     # wait for thread to start transaction
     time.sleep(1)
     fs_no_backoff = FoundryFileSystem(
         dataset=fsspec_write_test_folder[0],
         branch="master",
         transaction_backoff=False,
     )
-    with pytest.raises(FoundrySimultaneousOpenTransactionError):
-        with fs_no_backoff.open(file, "w") as f:
-            f.write("content")
+    with pytest.raises(FoundrySimultaneousOpenTransactionError), fs_no_backoff.open(
+        file, "w"
+    ) as f:
+        f.write("content")
     fs = FoundryFileSystem(
         dataset=fsspec_write_test_folder[0],
         branch="master",
     )
     with fs.open(file, "w") as f:
         f.write("content")
 
     assert fs.exists(file_in_thread)
     assert fs.exists(file)
 
 
 @patch(
-    "foundry_dev_tools.FoundryRestClient.get_dataset_identity",
+    "foundry_dev_tools.foundry_api_client.FoundryRestClient.get_dataset_identity",
     MagicMock(
         return_value={
             "dataset_path": "/path/to/ds",
             "dataset_rid": "ri.foundry.main.dataset.1234",
             "last_transaction_rid": None,
         }
     ),
 )
 def test_fsspec_api_client_not_cached(mocker):
-    with mocker.patch(
-        "foundry_dev_tools.Configuration.get_config",
+    mocker.patch(
+        "foundry_dev_tools.config.Configuration.get_config",
         side_effect=[
             {"jwt": "secret-token-ONE", "foundry_url": "https://test.com"},
             {"jwt": "secret-token-TWO", "foundry_url": "https://test.com"},
             {"jwt": "secret-token-THREE", "foundry_url": "https://test.com"},
         ],
-    ):
-        fs = FoundryFileSystem(
-            dataset="ri.foundry.main.dataset.1234-not-in-instance-cache"
-        )
-        assert fs.api._config["jwt"] == "secret-token-TWO"
-        assert fs.api._config["jwt"] == "secret-token-THREE"
+    )
+    fs = FoundryFileSystem(dataset="ri.foundry.main.dataset.1234-not-in-instance-cache")
+    assert fs.api._config["jwt"] == "secret-token-TWO"
+    assert fs.api._config["jwt"] == "secret-token-THREE"
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_ls_trailing_slash_empty_folder(random_file, fsspec_write_test_folder):
     random_folder = random_file.get()
     file1 = random_file.get()
     file1_in_folder = f"{random_folder}/{file1}"
 
     fs = FoundryFileSystem(
         dataset=fsspec_write_test_folder[0],
@@ -970,44 +980,45 @@
             f.write("content2")
     ls_result_no_slash = fs.ls(random_folder, detail=False)
     ls_result_with_slash = fs.ls(random_folder + "/", detail=False)
     assert ls_result_no_slash == ls_result_with_slash
 
 
 @patch(
-    "foundry_dev_tools.FoundryRestClient.get_dataset_identity",
+    "foundry_dev_tools.foundry_api_client.FoundryRestClient.get_dataset_identity",
     MagicMock(),
 )
 def test_skip_instance_cache():
     fs = FoundryFileSystem(
         dataset="ri.foundry.main.dataset.fake1bb5-be92-4ad9-aa3e-07c161751234",
         branch="master",
-        token="super-secret-token",
+        token="super-secret-token",  # noqa: S106
         skip_instance_cache=True,
     )
     fs2 = FoundryFileSystem(
         dataset="ri.foundry.main.dataset.fake1bb5-be92-4ad9-aa3e-07c161751234",
         branch="master",
-        token="super-secret-token",
+        token="super-secret-token",  # noqa: S106
         skip_instance_cache=True,
     )
 
     fs3 = FoundryFileSystem(
         dataset="ri.foundry.main.dataset.fake1bb5-be92-4ad9-aa3e-07c161751234",
         branch="master",
-        token="super-secret-token",
+        token="super-secret-token",  # noqa: S106
         skip_instance_cache=False,
     )
     fs4 = FoundryFileSystem(
         dataset="ri.foundry.main.dataset.fake1bb5-be92-4ad9-aa3e-07c161751234",
         branch="master",
-        token="super-secret-token",
+        token="super-secret-token",  # noqa: S106
         skip_instance_cache=False,
     )
-    fs.x = 123
-    fs2.x = 4567
-    fs3.x = 8901
-    fs4.x = 2345
-    assert fs.x == 123
-    assert fs2.x == 4567
-    assert fs3.x == 2345
-    assert fs4.x == 2345
+    fs.x = FS1 = 123
+    fs2.x = FS2 = 4567
+    fs3.x = FS3 = 8901
+    fs4.x = FS4 = 2345
+    assert fs.x == FS1
+    assert fs2.x == FS2
+    assert fs3.x != FS3
+    assert fs3.x == FS4
+    assert fs4.x == FS4
```

### Comparing `foundry-dev-tools-1.0.9/tests/test_multipass_tpa.py` & `foundry-dev-tools-1.1/tests/test_multipass_tpa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""
-Enable enable_third_party_application
-Rotate Secret rotate_third_party_application_secret
+"""Enable enable_third_party_application
+Rotate Secret rotate_third_party_application_secret.
 
 """
 import json
 
 import pytest
+import requests
 from requests.exceptions import HTTPError
 from requests_mock.adapter import ANY
 from requests_mock.mocker import Mocker
 
-from foundry_dev_tools import FoundryRestClient
+from foundry_dev_tools.foundry_api_client import FoundryRestClient
 
 USER_INFO_RESPONSE = {
     "id": "3c8fbda5-686e-4fcb-ad52-d95e4281d99f",
     "username": "M12345@eu.orggroup.com",
     "attributes": {
         "multipass:organization": ["Org1"],
         "multipass:email:primary": ["firstname.lastname@orggroup.com"],
@@ -147,20 +147,20 @@
             [
                 {"text": None, "status_code": 200},
             ],
         )
         _test_crud_inner(mocker)
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_crud_integration(mocker):
     try:
         _test_crud_inner(mocker)
     except HTTPError as err:
-        if err.response.status_code == 403:
+        if err.response.status_code == requests.codes.forbidden:
             pytest.skip(
                 "To test integration for multipass tpa, you need permissions to manage third party applications!"
             )
         else:
             raise err
```

### Comparing `foundry-dev-tools-1.0.9/tests/test_spark_caches.py` & `foundry-dev-tools-1.1/tests/test_spark_caches.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         "last_transaction_rid": last_transaction_rid,
         "dataset_path": dataset_path,
     }
 
 
 @pytest.fixture(autouse=True)
 def provide_config():
-    from foundry_dev_tools import Configuration
+    from foundry_dev_tools.config import Configuration
 
-    yield Configuration
+    return Configuration
 
 
 def test_add_get_delete(spark_session, provide_config):
     pc = DiskPersistenceBackedSparkCache(**provide_config)
     assert len(pc) == 0
     with pytest.raises(KeyError):
         pc.get_dataset_identity_not_branch_aware("/d1")
@@ -57,15 +57,16 @@
     pc[to_dict("d3", "t31", "/d3")] = spark_session.createDataFrame(
         data=[[3, 4]], schema="c: int, d: int"
     )
 
     for key, value in pc.items():
         assert_frame_equal(pc[key].toPandas(), value.toPandas())
 
-    assert len(pc) == 3
+    EXPECTED_LENGTH = 3
+    assert len(pc) == EXPECTED_LENGTH
 
     del pc[to_dict("d1", "t11", "/d1")]
     del pc[to_dict("d2", "t21", "/d2")]
     del pc[to_dict("d3", "t31", "/d3")]
 
 
 def test_key_not_exists_throws_key_error(provide_config):
@@ -83,15 +84,15 @@
 def test_unicode(spark_session, provide_config):
     pc = DiskPersistenceBackedSparkCache(**provide_config)
     data = spark_session.createDataFrame(
         data=[["\ud800foo", 2]], schema="a: string, b: string"
     )
     pc[to_dict("d1", "t11", "/d1")] = data
 
-    for key, value in pc.items():
+    for key, _value in pc.items():
         assert_frame_equal(data.toPandas(), pc[key].toPandas())
 
     del pc[to_dict("d1", "t11", "/d1")]
 
 
 def test_reads_csv_files_format(spark_session, provide_config):
     pc = DiskPersistenceBackedSparkCache(**provide_config)
@@ -175,21 +176,22 @@
 
 
 def test_multiline_csv(spark_session, provide_config):
     pc = DiskPersistenceBackedSparkCache(**provide_config)
     dataset_directory = os.sep.join(
         [provide_config["cache_dir"], "ds_multiline", "t1.csv"]
     )
-    csv_content = """,Name,"Test Status (Current) 
+    csv_content = """,Name,"Test Status (Current)
 (Company :Bar/Territory : Status : Indication : Date)",Report_date
-0,"12345 asdf 1234 (asdf), Ba1234","Bawefawef Pharma International Ltd: Country: No Development Reported: Aram foo bar asdf: 16-Feb-2011
-",2020-01-28"""
+0,"12345 asdf 1234 (asdf), Ba1234","Bawefawef Pharma International Ltd: Country:
+ No Development Reported: Aram foo bar asdf: 16-Feb-2011",2020-01-28"""
 
-    os.makedirs(dataset_directory)
-    with open(dataset_directory + "/manual.csv", "w") as f:
+    ds_dir = Path(dataset_directory)
+    ds_dir.mkdir(parents=True)
+    with ds_dir.joinpath("manual.csv").open(mode="w", encoding="UTF-8") as f:
         f.write(csv_content)
 
     foundry_schema = {
         "fieldSchemaList": [
             {
                 "type": "INTEGER",
                 "name": "untitled_column",
@@ -293,18 +295,19 @@
         [provide_config["cache_dir"], "ds_multiline", "t1.csv"]
     )
     csv_content_1 = """given_name,family_name
 Hans,Doe"""
     csv_content_2 = """given_name,family_name
 Max,Mustermann"""
 
-    os.makedirs(dataset_directory)
-    with open(os.sep.join([dataset_directory, "1"]), "w") as f:
+    ds_dir = Path(dataset_directory)
+    ds_dir.mkdir(parents=True)
+    with ds_dir.joinpath("1").open(mode="w", encoding="UTF-8") as f:
         f.write(csv_content_1)
-    with open(os.sep.join([dataset_directory, "2"]), "w") as f:
+    with ds_dir.joinpath("2").open(mode="w", encoding="UTF-8") as f:
         f.write(csv_content_2)
 
     foundry_schema = {
         "fieldSchemaList": [
             {
                 "type": "STRING",
                 "name": "given_name",
```

### Comparing `foundry-dev-tools-1.0.9/tests/test_token_provider.py` & `foundry-dev-tools-1.1/tests/test_token_provider.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,72 @@
 """Tests for the tokenproviders."""
 import sys
 from unittest import mock
 
 import pytest
 
-import foundry_dev_tools
-from foundry_dev_tools.utils.token_provider.foundry_token_provider import (
-    APP_SERVICE_ACCESS_TOKEN_HEADER,
-)
-
+from foundry_dev_tools.utils.token_provider import APP_SERVICE_ACCESS_TOKEN_HEADER
 from tests.conftest import PatchConfig
 
 
 def test_token_provider_streamlit(mocker):
     """Tests the streamlit token provider."""
-    with mocker.patch(
+    mocker.patch(
         "foundry_dev_tools.utils.token_provider.AppServiceStreamlitTokenProvider.get_streamlit_request_headers",
-        # noqa: E501
         return_value={APP_SERVICE_ACCESS_TOKEN_HEADER: "secret-token"},
-    ), PatchConfig(config_overwrite={"jwt": None}):
-        from foundry_dev_tools import FoundryRestClient
+    )
+    with PatchConfig(config_overwrite={"jwt": None}):
+        from foundry_dev_tools.foundry_api_client import FoundryRestClient
 
         client = FoundryRestClient()
+        print(client._config)
         assert client._config["jwt"] == "secret-token"
 
 
 def test_token_provider_streamlit_114_case_insensitive():
     """Tests the case insenstivity of the headers."""
     mock_get_websocket_headers = mock.MagicMock()
     sys.modules["streamlit.web.server.websocket_headers"] = mock_get_websocket_headers
     mock_get_websocket_headers._get_websocket_headers.return_value = {
         APP_SERVICE_ACCESS_TOKEN_HEADER.lower(): "secret-token2"
     }
-    from foundry_dev_tools import FoundryRestClient
+    from foundry_dev_tools.foundry_api_client import FoundryRestClient
 
     with PatchConfig(config_overwrite={"jwt": None}):
         client = FoundryRestClient()
         assert client._config["jwt"] == "secret-token2"
 
     del sys.modules["streamlit.web.server.websocket_headers"]
 
 
 def test_token_provider_streamlit_arg_higher_preference(mocker):
     """Tests that a configured jwt takes precedence."""
-    with mocker.patch(
+    mocker.patch(
         "foundry_dev_tools.utils.token_provider.AppServiceStreamlitTokenProvider.get_streamlit_request_headers",
-        # noqa: E501
         return_value={APP_SERVICE_ACCESS_TOKEN_HEADER: "secret-token"},
-    ), PatchConfig(config_overwrite={"jwt": None}):
-        from foundry_dev_tools import FoundryRestClient
+    )
+    with PatchConfig(config_overwrite={"jwt": None}):
+        from foundry_dev_tools.foundry_api_client import FoundryRestClient
 
         client = FoundryRestClient({"jwt": "shouldtakePrecedence"})
         assert client._config["jwt"] == "shouldtakePrecedence"
 
 
-@pytest.mark.no_patch_conf
+@pytest.mark.no_patch_conf()
 def test_token_provider_streamlit_no_cache_on_config_class(mocker):
-    """We test that a new instantiation of FoundryRestClient grabs from the Configuration class."""  # noqa: E501
-    with mocker.patch(
+    """We test that a new instantiation of FoundryRestClient grabs from the Configuration class."""
+    mocker.patch(
         "foundry_dev_tools.utils.token_provider.AppServiceStreamlitTokenProvider.get_streamlit_request_headers",
-        # noqa: E501
         side_effect=[
             {APP_SERVICE_ACCESS_TOKEN_HEADER: "secret-token-ONE"},
             {APP_SERVICE_ACCESS_TOKEN_HEADER: "secret-token-TWO"},
         ],
-    ), PatchConfig(config_overwrite={"jwt": None}):
-        from foundry_dev_tools import FoundryRestClient
+    )
+    with PatchConfig(config_overwrite={"jwt": None}):
+        from foundry_dev_tools.foundry_api_client import FoundryRestClient
 
         client = FoundryRestClient(
             {"foundry_url": "https://loremipsum.palantirfoundry.com"}
         )
         assert client._config["jwt"] == "secret-token-ONE"
 
         client2 = FoundryRestClient(
@@ -78,29 +75,29 @@
 
         assert client2._config["jwt"] == "secret-token-TWO"
         assert client._config["jwt"] == "secret-token-ONE"
 
 
 def test_token_provider_dash(mocker):
     """Tests the flask/dash token provider."""
-    with mocker.patch(
+    mocker.patch(
         "foundry_dev_tools.utils.token_provider.AppServiceDashTokenProvider.get_flask_request_headers",
-        # noqa: E501
         return_value={APP_SERVICE_ACCESS_TOKEN_HEADER: "secret-token-dash"},
-    ), PatchConfig(config_overwrite={"jwt": None}):
-        from foundry_dev_tools import FoundryRestClient
+    )
+    with PatchConfig(config_overwrite={"jwt": None}):
+        from foundry_dev_tools.foundry_api_client import FoundryRestClient
 
         client = FoundryRestClient()
         assert client._config["jwt"] == "secret-token-dash"
 
 
 def test_token_provider_dash_arg_higher_preference(mocker):
     """Tests that a configured jwt takes precedence."""
-    with mocker.patch(
+    mocker.patch(
         "foundry_dev_tools.utils.token_provider.AppServiceDashTokenProvider.get_flask_request_headers",
-        # noqa: E501
         return_value={APP_SERVICE_ACCESS_TOKEN_HEADER: "secret-token"},
-    ), PatchConfig(config_overwrite={"jwt": None}):
-        from foundry_dev_tools import FoundryRestClient
+    )
+    with PatchConfig(config_overwrite={"jwt": None}):
+        from foundry_dev_tools.foundry_api_client import FoundryRestClient
 
         client = FoundryRestClient({"jwt": "shouldtakePrecedence"})
         assert client._config["jwt"] == "shouldtakePrecedence"
```

### Comparing `foundry-dev-tools-1.0.9/tests/test_transforms.py` & `foundry-dev-tools-1.1/tests/test_transforms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 import io
 import json
+import os
 import pathlib
 from unittest import mock
 
 import fs
 import pandas as pd
 import pyspark.sql.functions as F
 import pytest
 from pandas.testing import assert_frame_equal
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.types import StructType
+
+import foundry_dev_tools.config
+from foundry_dev_tools.utils.caches.spark_caches import DiskPersistenceBackedSparkCache
+from tests.conftest import PatchConfig
+from tests.test_foundry_mock import MockFoundryRestClient
 from transforms.api import (
-    configure,
-    incremental,
     Input,
     Markings,
     OrgMarkings,
     Output,
+    TransformContext,
+    configure,
+    incremental,
     transform,
     transform_df,
     transform_pandas,
-    TransformContext,
 )
 from transforms.api._transform import TransformInput, TransformOutput
 
-import foundry_dev_tools
-from foundry_dev_tools.utils.caches.spark_caches import DiskPersistenceBackedSparkCache
-
-from tests.conftest import PatchConfig
-from tests.test_foundry_mock import MockFoundryRestClient
-
 
 def get_dataset_identity_mock(self, dataset_path: str, branch="master"):
     return {
         "dataset_path": dataset_path,
         "dataset_rid": dataset_path.replace("/", "") + "rid1",
         "last_transaction_rid": dataset_path.replace("/", "") + "rid1" + "t1",
     }
 
 
 def get_dataset_stats_mock(self, dataset_rid, branch_or_transaction_rid):
     # we return a dataset that is of size 1 mb bigger than the limit to force sql execution and not file download
     return {
         "sizeInBytes": (
-            foundry_dev_tools.Configuration["transforms_sql_dataset_size_threshold"] + 1
+            foundry_dev_tools.config.Configuration[
+                "transforms_sql_dataset_size_threshold"
+            ]
+            + 1
         )
         * 1024
         * 1024,
         "numFiles": 1,
         "hiddenFilesSizeInBytes": 0,
         "numHiddenFiles": 0,
         "numTransactions": 1,
@@ -73,50 +76,50 @@
     )
     .withColumn("_importedAt", F.to_timestamp("_importedAt"))
     .withColumn("created_at", F.to_date("created_at"))
 )
 
 
 def return_df(one, dataset_path, branch):
-    if dataset_path == "/input1":
-        return spark_df_return_data_one
-    elif dataset_path == "/input2":
-        return spark_df_return_data_two
-    elif dataset_path == "/tsdate":
-        return spark_df_return_data_timestamp_date
+    return {
+        "/input1": spark_df_return_data_one,
+        "/input2": spark_df_return_data_two,
+        "/tsdate": spark_df_return_data_timestamp_date,
+    }.get(dataset_path)
 
 
 def get_spark_schema_mock(one, dataset_rid, last_transaction_rid, branch="master"):
     return return_df(one, dataset_rid.replace("rid1", ""), None).schema
 
 
 def dataset_has_schema_mock(one, two, three):
     return True
 
 
 @pytest.fixture()
-def run_around_tests(tmpdir):
+def _run_around_tests(tmpdir):
     with mock.patch(
         "transforms.api.Input._read_spark_df_with_sql_query", return_df
     ), mock.patch(
         "transforms.api.Input._dataset_has_schema", dataset_has_schema_mock
     ), mock.patch(
-        "foundry_dev_tools.FoundryRestClient.get_dataset_identity",
+        "foundry_dev_tools.foundry_api_client.FoundryRestClient.get_dataset_identity",
         get_dataset_identity_mock,
     ), mock.patch(
-        "foundry_dev_tools.FoundryRestClient.get_dataset_stats",
+        "foundry_dev_tools.foundry_api_client.FoundryRestClient.get_dataset_stats",
         get_dataset_stats_mock,
     ), mock.patch(
         "foundry_dev_tools.utils.converter.foundry_spark.foundry_schema_to_spark_schema",
         get_spark_schema_mock,
     ):
         yield
 
 
-def test_transform_one_input(run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transform_one_input():
     @transform(output1=Output("/output/to/dataset"), input1=Input("/input1"))
     def transform_me(output1, input1):
         assert isinstance(output1, TransformOutput)
         assert isinstance(input1, TransformInput)
         assert_frame_equal(
             input1.dataframe().toPandas(), spark_df_return_data_one.toPandas()
         )
@@ -139,25 +142,25 @@
 
         with output1.filesystem().open("output.json", "w") as f:
             f.write("test")
         assert "output.json" in [file.path for file in output1.filesystem().ls()]
         assert "output.json" in [
             file.path for file in output1.filesystem().ls(glob="*/**", regex=".*")
         ]
-        assert len([file.path for file in output1.filesystem().ls(glob="**/*.py")]) is 0
+        assert len([file.path for file in output1.filesystem().ls(glob="**/*.py")]) == 0
         assert (
             len(
                 [
                     file.path
                     for file in output1.filesystem().ls(
                         glob="**/*.json", regex=".*.csv"
                     )
                 ]
             )
-            is 0
+            == 0
         )
         with output1.filesystem().open("output.json", "r") as f:
             content = f.read()
         assert content == "test"
 
         assert input1.path == "/input1"
         assert input1.rid == "input1" + "rid1"
@@ -173,15 +176,16 @@
 
     result = transform_me.compute()
     assert "output1" in result
     assert isinstance(result["output1"], DataFrame)
     assert result["output1"].schema.names[0] == "col1"
 
 
-def test_transform_df_one_input(mocker, run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transform_df_one_input(mocker):
     from_foundry_and_cache = mocker.spy(Input, "_retrieve_from_foundry_and_cache")
     from_cache = mocker.spy(Input, "_retrieve_from_cache")
 
     with pytest.warns(UserWarning) as record:
 
         @transform_df(Output("/output/to/dataset"), input1=Input("/input1"))
         def transform_me(input1: DataFrame) -> DataFrame:
@@ -205,30 +209,32 @@
 
     _ = Input("/input1")
 
     from_foundry_and_cache.assert_not_called()
     from_cache.assert_called()
 
 
-def test_transform_df_one_input_with_ctx(run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transform_df_one_input_with_ctx():
     @transform_df(Output("/output/to/dataset"), input1=Input("/input1"))
     def transform_me(ctx, input1: DataFrame) -> DataFrame:
         assert isinstance(input1, DataFrame)
         assert isinstance(ctx, TransformContext)  # ctx is our TransformContext
         assert isinstance(
             ctx.spark_session, SparkSession
         )  # ctx.spark_session is a SparkSession
         assert_frame_equal(input1.toPandas(), spark_df_return_data_one.toPandas())
         return input1.withColumn("col1", F.lit("replaced")).select("col1")
 
     df = transform_me.compute()
     assert df.schema.names[0] == "col1"
 
 
-def test_transform_df_two_inputs(run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transform_df_two_inputs():
     @transform_df(
         Output("/output/to/dataset"),
         input1=Input("/input1"),
         input2=Input("/input2"),
     )
     def transform_me(ctx, input1: DataFrame, input2: DataFrame) -> DataFrame:
         assert isinstance(input1, DataFrame)
@@ -237,18 +243,20 @@
         assert isinstance(ctx.spark_session, SparkSession)
         assert_frame_equal(input1.toPandas(), spark_df_return_data_one.toPandas())
         assert_frame_equal(input2.toPandas(), spark_df_return_data_two.toPandas())
         return input1.union(input2)
 
     df = transform_me.compute()
     assert df.columns == ["a", "b"]
-    assert df.count() == 2
+    EXPECTED_COUNT = 2
+    assert df.count() == EXPECTED_COUNT
 
 
-def test_transform_df_date_and_timestamp(run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transform_df_date_and_timestamp():
     def mock_schema(one):
         return StructType.fromJson(
             {
                 "type": "struct",
                 "fields": [
                     {
                         "name": "_importedAt",
@@ -278,15 +286,16 @@
         return input1
 
     df = transform_me.compute()
     assert df.columns == ["_importedAt", "created_at"]
     assert df.count() == 1
 
 
-def test_transform_pandas_one_input(mocker, run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transform_pandas_one_input(mocker):
     from_foundry_and_cache = mocker.spy(Input, "_retrieve_from_foundry_and_cache")
     from_cache = mocker.spy(Input, "_retrieve_from_cache")
 
     @transform_pandas(Output("/output/to/dataset"), input1=Input("/input1"))
     def transform_me(input1: pd.DataFrame) -> pd.DataFrame:
         assert isinstance(input1, pd.DataFrame)
         assert_frame_equal(input1, spark_df_return_data_one.toPandas())
@@ -297,21 +306,22 @@
 
     from_foundry_and_cache.assert_called()
     from_cache.assert_not_called()
 
     from_foundry_and_cache.reset_mock()
     from_cache.reset_mock()
 
-    input1 = Input("/input1")
+    Input("/input1")
 
     from_foundry_and_cache.assert_not_called()
     from_cache.assert_called()
 
 
-def test_transform_pandas_one_input_with_ctx(run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transform_pandas_one_input_with_ctx():
     @transform_pandas(Output("/output/to/dataset"), input1=Input("/input1"))
     def transform_me(ctx, input1: pd.DataFrame) -> pd.DataFrame:
         assert isinstance(input1, pd.DataFrame)
         assert isinstance(ctx, TransformContext)  # ctx is our TransformContext
         assert isinstance(
             ctx.spark_session, SparkSession
         )  # ctx.spark_session is a SparkSession
@@ -319,15 +329,16 @@
         return input1
 
     df = transform_me.compute()
     assert isinstance(df, pd.DataFrame)
     assert_frame_equal(df, spark_df_return_data_one.toPandas())
 
 
-def test_transform_pandas_two_inputs(run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transform_pandas_two_inputs():
     @transform_pandas(
         Output("/output/to/dataset"),
         input1=Input("/input1"),
         input2=Input("/input2"),
     )
     def transform_me(ctx, input1: pd.DataFrame, input2: pd.DataFrame) -> pd.DataFrame:
         assert isinstance(input1, pd.DataFrame)
@@ -339,15 +350,16 @@
         return input2
 
     df = transform_me.compute()
     assert isinstance(df, pd.DataFrame)
     assert_frame_equal(df, spark_df_return_data_two.toPandas())
 
 
-def test_transform_pandas_date_and_timestamp(run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transform_pandas_date_and_timestamp():
     def mock_schema(one):
         return StructType.fromJson(
             {
                 "type": "struct",
                 "fields": [
                     {
                         "name": "_importedAt",
@@ -377,15 +389,16 @@
         return input1
 
     df = transform_me.compute()
     assert list(df.columns) == ["_importedAt", "created_at"]
     assert df.shape[0] == 1
 
 
-def test_transform_freeze_cache(mocker, tmpdir, run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transform_freeze_cache(mocker, tmpdir):
     online = mocker.spy(Input, "_online")
     offline = mocker.spy(Input, "_offline")
 
     @transform(output1=Output("/output/to/dataset"), input1=Input("/input1"))
     def transform_me_data_from_online_cache(output1, input1):
         pass
 
@@ -412,45 +425,48 @@
         assert isinstance(result["output1"], DataFrame)
         assert result["output1"].schema.names[0] == "col1"
 
         online.assert_not_called()
         offline.assert_called()
 
 
-def test_transforms_with_configure(run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transforms_with_configure():
     with pytest.warns(UserWarning):
 
         @configure(someArg=1234)
         @transform(
             output1=Output("/output/to/dataset"),
             input1=Input("/input1"),
         )
         def transform_me_data_from_online_cache(output1, input1):
             pass
 
 
-def test_transforms_with_incremental(run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transforms_with_incremental():
     with pytest.warns(UserWarning):
 
         @incremental()
         @transform(
             output1=Output("/output/to/dataset"),
             input1=Input("/input1"),
         )
         def transform_me_data_from_online_cache(output1, input1):
             pass
 
 
-def test_transform_output_write_to_folder(tmp_path_factory, run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transform_output_write_to_folder(tmp_path_factory):
     transforms_output_folder = pathlib.Path(
         tmp_path_factory.mktemp("transforms_output_folder")
     )
     with PatchConfig(
         initial_config_overwrite={
-            "transforms_output_folder": str(transforms_output_folder)
+            "transforms_output_folder": os.fspath(transforms_output_folder)
         }
     ):
 
         @transform(
             output1=Output("/output/to/dataset"),
             # folders are only created if filesystem() is called at least once
             output2=Output("/output/to/dataset2"),
@@ -470,21 +486,24 @@
             assert output1.rid is not None
             assert output1.rid is not None
 
         result = transform_me.compute()
         assert "output1" in result
         assert "output2" in result
 
-        with open(transforms_output_folder / "output1" / "output.json", "r") as f:
+        with transforms_output_folder.joinpath("output1", "output.json").open(
+            encoding="UTF-8"
+        ) as f:
             assert f.read() == "test"
 
         assert pathlib.Path(transforms_output_folder / "output2").is_dir() is False
 
 
-def test_transform_works_in_no_git_repository(mocker, run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transform_works_in_no_git_repository(mocker):
     with pytest.warns(UserWarning):
         import subprocess
 
         run_mock = mocker.Mock()
         run_mock.side_effect = subprocess.CalledProcessError(
             128, ["git", "rev-parse", "--show-toplevel"]
         )
@@ -494,15 +513,16 @@
             output1=Output("/output/to/dataset"),
             input1=Input("/input1"),
         )
         def transform_me_data_from_online_cache(output1, input1):
             pass
 
 
-def test_transform_markings(run_around_tests):
+@pytest.mark.usefixtures("_run_around_tests")
+def test_transform_markings():
     @transform_df(
         Output("output1"),
         input1=Input(
             "/input1",
             stop_propagating=Markings(["a-b-c"], on_branches=["master"]),
             stop_requiring=OrgMarkings("a-b-c", on_branches=None),
         ),
@@ -512,17 +532,17 @@
 
     transform_me.compute()
 
 
 def test_binary_dataset_with_empty_folders(tmpdir):
     input_dataset = "/namespace/dataset1"
 
-    root = str(tmpdir)
+    root = os.fspath(tmpdir)
     filesystem = fs.open_fs(root)
-    client = MockFoundryRestClient(fs=filesystem)
+    client = MockFoundryRestClient(filesystem=filesystem)
 
     branch = "master"
 
     ds = client.create_dataset("/namespace/dataset1")
     client.create_branch(ds["rid"], branch)
 
     transaction_rid = client.open_transaction(ds["rid"], "SNAPSHOT", branch)
@@ -549,15 +569,17 @@
         dataset_rid=ds["rid"],
         transaction_rid=transaction_rid,
         path_or_buf=io.BytesIO(b"aa"),
         path_in_foundry_dataset="poseidon/features",
     )
     client.commit_transaction(dataset_rid=ds["rid"], transaction_id=transaction_rid)
 
-    with mock.patch("foundry_dev_tools.CachedFoundryClient.api", client):
+    with mock.patch(
+        "foundry_dev_tools.cached_foundry_client.CachedFoundryClient.api", client
+    ):
 
         @transform(
             output=Output("/path/to/output1"),
             input1=Input(input_dataset, branch="master"),
         )
         def transform_me(output, input1):
             assert input1.filesystem() is not None
@@ -569,10 +591,12 @@
             ]
             assert input1.dataframe() is None
 
         result = transform_me.compute()
         assert "output" in result
 
         # Check that _offline functions of cache work
-        cache = DiskPersistenceBackedSparkCache(**foundry_dev_tools.Configuration)
+        cache = DiskPersistenceBackedSparkCache(
+            **foundry_dev_tools.config.Configuration
+        )
         ds_identity = cache.get_dataset_identity_not_branch_aware(input_dataset)
         assert cache.dataset_has_schema(ds_identity) is False
```

### Comparing `foundry-dev-tools-1.0.9/tests/test_transforms_integration.py` & `foundry-dev-tools-1.1/tests/test_transforms_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import warnings
+from typing import TYPE_CHECKING
 from unittest import mock
 
 import pyspark.sql.functions as F
 import pytest
 from pyspark.sql import SparkSession
-from transforms.api import Input, Output, transform, transform_df, TransformContext
-from transforms.api._transform import TransformInput
 
-import foundry_dev_tools
-
-import tests.utils
-from foundry_dev_tools import FoundryRestClient
+import foundry_dev_tools.config
+from foundry_dev_tools.foundry_api_client import FoundryRestClient
 from foundry_dev_tools.utils.caches.spark_caches import DiskPersistenceBackedSparkCache
 from foundry_dev_tools.utils.converter.foundry_spark import (
     foundry_schema_to_spark_schema,
 )
-
 from tests.conftest import PatchConfig
+from tests.utils import TEST_FOLDER, generic_upload_dataset_if_not_exists
+from transforms.api import Input, Output, TransformContext, transform, transform_df
 
-from tests.utils import generic_upload_dataset_if_not_exists, TEST_FOLDER
+if TYPE_CHECKING:
+    import transforms
 
 
 @pytest.fixture()
 def iris_integration_test_csv_rid(iris_dataset):
-    yield iris_dataset[0]
+    return iris_dataset[0]
 
 
 @pytest.fixture()
 def iris_integration_test_csv_path(iris_dataset):
-    yield iris_dataset[1]
+    return iris_dataset[1]
 
 
 @pytest.mark.parametrize(
     "input_dataset_fixture",
     [
         "complex_dataset_fixture",
         # "ri.foundry.main.dataset.4be02f70-e771-4914-b6d6-8781179ae6b9",  # array, struct types test
@@ -51,17 +50,17 @@
         )
     )
 
     from_foundry_and_cache = mocker.spy(Input, "_retrieve_from_foundry_and_cache")
     from_cache = mocker.spy(Input, "_retrieve_from_cache")
     with_sql_query = mocker.spy(Input, "_read_spark_df_with_sql_query")
 
-    with mock.patch("foundry_dev_tools.CachedFoundryClient.api", client), PatchConfig(
-        config_overwrite={"transforms_sql_dataset_size_threshold": 0}
-    ) as pc:
+    with mock.patch(
+        "foundry_dev_tools.cached_foundry_client.CachedFoundryClient.api", client
+    ), PatchConfig(config_overwrite={"transforms_sql_dataset_size_threshold": 0}):
 
         @transform_df(
             Output("/path/to/output1"),
             input1=Input(input_dataset, branch="master"),
         )
         def transform_me(ctx, input1):
             assert schema == input1.schema
@@ -85,15 +84,17 @@
         df = input1.dataframe()
         assert schema == df.schema
 
         from_foundry_and_cache.assert_not_called()
         from_cache.assert_called()
 
         # Check that offline functions of cache work
-        cache = DiskPersistenceBackedSparkCache(**foundry_dev_tools.Configuration)
+        cache = DiskPersistenceBackedSparkCache(
+            **foundry_dev_tools.config.Configuration
+        )
         ds_identity = cache.get_dataset_identity_not_branch_aware(input_dataset)
         assert cache.dataset_has_schema(ds_identity) is True
 
 
 @pytest.mark.parametrize(
     "input_dataset_fixture",
     [
@@ -121,15 +122,17 @@
         # we expect no sql fallback warnings
         warnings.simplefilter("error")
         with PatchConfig(
             initial_config_overwrite={
                 "transforms_force_full_dataset_download": True,
                 "transforms_sql_dataset_size_threshold": 1,
             }
-        ), mock.patch("foundry_dev_tools.CachedFoundryClient.api", client):
+        ), mock.patch(
+            "foundry_dev_tools.cached_foundry_client.CachedFoundryClient.api", client
+        ):
 
             @transform_df(
                 Output("/path/to/output1"),
                 input1=Input(input_dataset, branch="master"),
             )
             def transform_me(ctx, input1):
                 assert schema == input1.schema
@@ -152,38 +155,40 @@
             df = input1.dataframe()
             assert schema == df.schema
 
             from_foundry_and_cache.assert_not_called()
             from_cache.assert_called()
 
             # Check that offline functions of cache work
-            cache = DiskPersistenceBackedSparkCache(**foundry_dev_tools.Configuration)
+            cache = DiskPersistenceBackedSparkCache(
+                **foundry_dev_tools.config.Configuration
+            )
             ds_identity = cache.get_dataset_identity_not_branch_aware(input_dataset)
             assert cache.dataset_has_schema(ds_identity) is True
 
 
-@pytest.mark.integration
+@pytest.mark.integration()
 def test_binary_dataset(mocker):
     upload_client = FoundryRestClient()
     uploaded_dataset = generic_upload_dataset_if_not_exists(
         upload_client, "bin", TEST_FOLDER / "test_data" / "binary_dataset"
     )
-    with open(
-        TEST_FOLDER / "test_data" / "binary_dataset" / "bin", "rb"
+    with TEST_FOLDER.joinpath("test_data", "binary_dataset", "bin").open(
+        mode="rb"
     ) as uploaded_file:
         uploaded_binary = uploaded_file.read()
 
     online = mocker.spy(Input, "_online")
     offline = mocker.spy(Input, "_offline")
 
     @transform(
         output=Output("/path/to/output1"),
         input1=Input(uploaded_dataset[0], branch="master"),
     )
-    def transform_me_online(output, input1: TransformInput):
+    def transform_me_online(output, input1: "transforms.api._transform.TransformInput"):
         assert input1.filesystem() is not None
         assert input1.dataframe() is None
         with input1.filesystem().open("bin", "rb") as bin_fd:
             assert uploaded_binary == bin_fd.read()
 
     result = transform_me_online.compute()
     assert "output" in result
@@ -191,15 +196,15 @@
     online.assert_called()
     offline.assert_not_called()
 
     online.reset_mock()
     offline.reset_mock()
 
     # Check that offline functions of cache work
-    cache = DiskPersistenceBackedSparkCache(**foundry_dev_tools.Configuration)
+    cache = DiskPersistenceBackedSparkCache(**foundry_dev_tools.config.Configuration)
     ds_identity = cache.get_dataset_identity_not_branch_aware(uploaded_dataset[0])
     assert cache.dataset_has_schema(ds_identity) is False
 
     with PatchConfig(config_overwrite={"transforms_freeze_cache": True}):
 
         @transform(
             output=Output("/path/to/output1"),
```

### Comparing `foundry-dev-tools-1.0.9/tests/utils.py` & `foundry-dev-tools-1.1/tests/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import datetime
+import glob
 import os
 import os.path
-import pathlib
 import random
 from decimal import Decimal
-from typing import Tuple
+from pathlib import Path, PurePosixPath
+from typing import TYPE_CHECKING
 
 import numpy as np
 
 from foundry_dev_tools.foundry_api_client import DatasetNotFoundError
 
-INTEGRATION_TEST_COMPASS_ROOT_PATH = pathlib.PurePosixPath(
+if TYPE_CHECKING:
+    import foundry_dev_tools
+    from tests.foundry_mock_client import MockFoundryRestClient
+
+INTEGRATION_TEST_COMPASS_ROOT_PATH = PurePosixPath(
     os.getenv(
         "INTEGRATION_TEST_COMPASS_ROOT_PATH",
         "/Global/global-use-case-public/Developer Experience/integration-test-folder",
     )
 )
 INTEGRATION_TEST_COMPASS_ROOT_RID = os.getenv(
     "INTEGRATION_TEST_COMPASS_ROOT_RID",
     "ri.compass.main.folder.c733ffcc-5a13-461e-8bdc-d1be925a0646",
 )
 
-TEST_FOLDER = pathlib.Path(__file__).parent.resolve()
+TEST_FOLDER = Path(__file__).parent.resolve()
 
 IRIS_SCHEMA = {
     "fieldSchemaList": [
         {
             "type": "DOUBLE",
             "name": "sepal_width",
             "nullable": None,
@@ -263,47 +268,43 @@
     "primaryKey": None,
     "dataFrameReaderClass": "com.palantir.foundry.spark.input.ParquetDataFrameReader",
     "customMetadata": {"format": "parquet"},
 }
 
 
 def generic_upload_dataset_if_not_exists(
-    client: "foundry_dev_tools.FoundryRestClient",
+    client: "foundry_dev_tools.foundry_api_client.FoundryRestClient | MockFoundryRestClient",
     name="iris_new",
-    upload_folder=None,
+    upload_folder: "Path | None" = None,
     foundry_schema=None,
-) -> Tuple[str, str, str, str, bool]:
+) -> "tuple[str, str, str, str, bool]":
     ds_path = f"{INTEGRATION_TEST_COMPASS_ROOT_PATH}/{name}"
     ds_branch = "master"
     newly_created = False
     try:
         identity = client.get_dataset_identity(
             dataset_path_or_rid=ds_path, branch=ds_branch
         )
         rid = identity["dataset_rid"]
         transaction_rid = identity["last_transaction_rid"]
     except DatasetNotFoundError:
         rid = client.create_dataset(ds_path)["rid"]
         _ = client.create_branch(rid, ds_branch)
         newly_created = True
         if upload_folder:
-            recursive_listing = pathlib.Path(upload_folder).rglob("*")
-            filenames_with_dirs = [
-                path.as_posix()
-                for path in recursive_listing
-                if not any(part.startswith(".") for part in path.parts)
-            ]
-            filepaths = [
-                str(file) for file in filenames_with_dirs if not os.path.isdir(file)
-            ]
-            dataset_paths_in_foundry = [
-                path.replace(pathlib.Path(upload_folder).as_posix(), "")[1:]
-                for path in filepaths
-            ]
-            path_file_dict = dict(zip(dataset_paths_in_foundry, filepaths))
+            recursive_listing = glob.glob(
+                os.fspath(upload_folder / "**"), recursive=True
+            )
+            path_file_dict = {}
+            for file in recursive_listing:
+                pfile = Path(file)
+                if not pfile.is_dir():
+                    path_file_dict[
+                        pfile.relative_to(upload_folder).as_posix().lstrip("/")
+                    ] = file
             transaction_rid = client.open_transaction(dataset_rid=rid, mode="SNAPSHOT")
             client.upload_dataset_files(
                 dataset_rid=rid,
                 transaction_rid=transaction_rid,
                 path_file_dict=path_file_dict,
             )
             client.commit_transaction(dataset_rid=rid, transaction_id=transaction_rid)
@@ -354,15 +355,14 @@
 def random_datetime_array(length):
     start = datetime.datetime(1988, 11, 29, tzinfo=datetime.timezone.utc)
     end = datetime.datetime(2022, 11, 30, tzinfo=datetime.timezone.utc)
     return [random.random() * (end - start) + start for _ in range(length)]
 
 
 def generate_test_dataset(spark_session, output_folder, n_rows=50000):
-    import numpy as np
     import pandas as pd
     import pyspark.sql.types as T
 
     schema = T.StructType(
         [
             T.StructField(
                 "struct_column", T.StructType([T.StructField("value", T.StringType())])
```

### Comparing `foundry-dev-tools-1.0.9/tox.ini` & `foundry-dev-tools-1.1/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 # Tox configuration file
 # Read more under https://tox.wiki/
-# THIS SCRIPT IS SUPPOSED TO BE AN EXAMPLE. MODIFY IT ACCORDING TO YOUR NEEDS!
 
 [tox]
 minversion = 3.24
 envlist = default
 isolated_build = True
 
-
 [testenv]
 description = Invoke pytest to run automated tests
 setenv =
     TOXINIDIR = {toxinidir}
 passenv =
     HOME
     SETUPTOOLS_*
 extras =
-    integration-testing
+    testing
+    transforms
+    cli
+    integration
 commands =
     pytest {posargs}
 
-
-# To run `tox -e lint` you need to make sure you have a
-# `.pre-commit-config.yaml` file. See https://pre-commit.com
 [testenv:lint]
 description = Perform static analysis and style checks
 skip_install = True
 deps = pre-commit
 passenv =
     HOMEPATH
     PROGRAMDATA
     SETUPTOOLS_*
 commands =
     pre-commit run --all-files {posargs:--show-diff-on-failure}
 
-
 [testenv:{build,clean}]
 description =
     build: Build the package in isolation according to PEP517, see https://github.com/pypa/build
     clean: Remove old distribution files and temporary build artifacts (./build and ./dist)
 # https://setuptools.pypa.io/en/stable/build_meta.html#how-to-use-it
 skip_install = True
 changedir = {toxinidir}
@@ -47,15 +44,14 @@
 passenv =
     SETUPTOOLS_*
 commands =
     clean: python -c 'import shutil; [shutil.rmtree(p, True) for p in ("build", "dist", "docs/_build")]'
     clean: python -c 'import pathlib, shutil; [shutil.rmtree(p, True) for p in pathlib.Path("src").glob("*.egg-info")]'
     build: python -m build {posargs}
 
-
 [testenv:{docs,doctests,linkcheck}]
 description =
     docs: Invoke sphinx-build to build the docs
     doctests: Invoke sphinx-build to run doctests
     linkcheck: Check for broken links in the documentation
 passenv =
     SETUPTOOLS_*
@@ -80,15 +76,14 @@
     DOCSDIR = {toxinidir}/docs
     BUILDDIR = {toxinidir}/docs/_build
 deps =
     -r {toxinidir}/docs/requirements.txt
 commands =
     sphinx-autobuild --ignore '{env:DOCSDIR}/api/**' "{env:DOCSDIR}" "{env:BUILDDIR}" {posargs}
 
-
 [testenv:publish]
 description =
     Publish the package you have been developing to a package index server.
     By default, it uses testpypi. If you really want to publish your package
     to be publicly accessible in PyPI, use the `-- --repository pypi` option.
 skip_install = True
 changedir = {toxinidir}
```

