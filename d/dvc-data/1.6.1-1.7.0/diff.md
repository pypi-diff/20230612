# Comparing `tmp/dvc-data-1.6.1.tar.gz` & `tmp/dvc-data-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-data-1.6.1.tar", last modified: Mon Jun 12 00:45:46 2023, max compression
+gzip compressed data, was "dvc-data-1.7.0.tar", last modified: Mon Jun 12 06:54:14 2023, max compression
```

## Comparing `dvc-data-1.6.1.tar` & `dvc-data-1.7.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:46.333549 dvc-data-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-12 00:45:24.000000 dvc-data-1.6.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 00:45:24.000000 dvc-data-1.6.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:46.321548 dvc-data-1.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-12 00:45:24.000000 dvc-data-1.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:46.321548 dvc-data-1.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-12 00:45:24.000000 dvc-data-1.6.1/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-12 00:45:24.000000 dvc-data-1.6.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-12 00:45:24.000000 dvc-data-1.6.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-12 00:45:24.000000 dvc-data-1.6.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-12 00:45:24.000000 dvc-data-1.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-12 00:45:24.000000 dvc-data-1.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-12 00:45:24.000000 dvc-data-1.6.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-12 00:45:24.000000 dvc-data-1.6.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-12 00:45:24.000000 dvc-data-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-12 00:45:46.333549 dvc-data-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-12 00:45:24.000000 dvc-data-1.6.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-12 00:45:24.000000 dvc-data-1.6.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-12 00:45:24.000000 dvc-data-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-12 00:45:46.333549 dvc-data-1.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:46.317548 dvc-data-1.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:46.321548 dvc-data-1.6.1/src/dvc_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:46.325549 dvc-data-1.6.1/src/dvc_data/hashfile/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/_ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/checkout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:46.329549 dvc-data-1.6.1/src/dvc_data/hashfile/db/
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/db/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/db/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/db/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/gc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/hash_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/istextfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/hashfile/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:46.329549 dvc-data-1.6.1/src/dvc_data/index/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/index/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/index/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/index/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/index/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/index/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/index/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/index/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/index/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/index/view.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-12 00:45:24.000000 dvc-data-1.6.1/src/dvc_data/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:46.325549 dvc-data-1.6.1/src/dvc_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-12 00:45:46.000000 dvc-data-1.6.1/src/dvc_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-12 00:45:46.000000 dvc-data-1.6.1/src/dvc_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 00:45:46.000000 dvc-data-1.6.1/src/dvc_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 00:45:46.000000 dvc-data-1.6.1/src/dvc_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 00:45:46.000000 dvc-data-1.6.1/src/dvc_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-12 00:45:46.000000 dvc-data-1.6.1/src/dvc_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 00:45:46.000000 dvc-data-1.6.1/src/dvc_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:46.329549 dvc-data-1.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:46.329549 dvc-data-1.6.1/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/benchmarks/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:46.333549 dvc-data-1.6.1/tests/hashfile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/hashfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/hashfile/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/hashfile/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/hashfile/test_db_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/hashfile/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/hashfile/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/hashfile/test_hash_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/hashfile/test_istextfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/hashfile/test_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/hashfile/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/hashfile/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:46.333549 dvc-data-1.6.1/tests/index/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/index/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/index/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/index/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/index/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-12 00:45:24.000000 dvc-data-1.6.1/tests/test_dvc_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:54:14.710148 dvc-data-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-12 06:53:51.000000 dvc-data-1.7.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 06:53:51.000000 dvc-data-1.7.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:54:14.702148 dvc-data-1.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-12 06:53:51.000000 dvc-data-1.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:54:14.702148 dvc-data-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-12 06:53:51.000000 dvc-data-1.7.0/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-12 06:53:51.000000 dvc-data-1.7.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-12 06:53:51.000000 dvc-data-1.7.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-12 06:53:51.000000 dvc-data-1.7.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-12 06:53:51.000000 dvc-data-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-12 06:53:51.000000 dvc-data-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-12 06:53:51.000000 dvc-data-1.7.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-12 06:53:51.000000 dvc-data-1.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-12 06:53:51.000000 dvc-data-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-12 06:54:14.710148 dvc-data-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-12 06:53:51.000000 dvc-data-1.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-12 06:53:51.000000 dvc-data-1.7.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-12 06:53:51.000000 dvc-data-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-12 06:54:14.710148 dvc-data-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:54:14.702148 dvc-data-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:54:14.702148 dvc-data-1.7.0/src/dvc_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:54:14.706148 dvc-data-1.7.0/src/dvc_data/hashfile/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/checkout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:54:14.706148 dvc-data-1.7.0/src/dvc_data/hashfile/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/db/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/db/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/db/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/gc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/hash_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/istextfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/hashfile/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:54:14.710148 dvc-data-1.7.0/src/dvc_data/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/index/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/index/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/index/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/index/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/index/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18503 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/index/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/index/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/index/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/index/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-12 06:53:51.000000 dvc-data-1.7.0/src/dvc_data/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:54:14.706148 dvc-data-1.7.0/src/dvc_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-12 06:54:14.000000 dvc-data-1.7.0/src/dvc_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-12 06:54:14.000000 dvc-data-1.7.0/src/dvc_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 06:54:14.000000 dvc-data-1.7.0/src/dvc_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 06:54:14.000000 dvc-data-1.7.0/src/dvc_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 06:54:14.000000 dvc-data-1.7.0/src/dvc_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-12 06:54:14.000000 dvc-data-1.7.0/src/dvc_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 06:54:14.000000 dvc-data-1.7.0/src/dvc_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:54:14.710148 dvc-data-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:54:14.710148 dvc-data-1.7.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/benchmarks/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:54:14.710148 dvc-data-1.7.0/tests/hashfile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/hashfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/hashfile/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/hashfile/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/hashfile/test_db_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/hashfile/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/hashfile/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/hashfile/test_hash_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/hashfile/test_istextfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/hashfile/test_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/hashfile/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/hashfile/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:54:14.710148 dvc-data-1.7.0/tests/index/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/index/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/index/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/index/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/index/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-12 06:53:51.000000 dvc-data-1.7.0/tests/test_dvc_data.py
```

### Comparing `dvc-data-1.6.1/.cruft.json` & `dvc-data-1.7.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/.github/dependabot.yml` & `dvc-data-1.7.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/.github/workflows/benchmark.yml` & `dvc-data-1.7.0/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/.github/workflows/release.yml` & `dvc-data-1.7.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/.github/workflows/tests.yml` & `dvc-data-1.7.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/.gitignore` & `dvc-data-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/.pre-commit-config.yaml` & `dvc-data-1.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/CODE_OF_CONDUCT.rst` & `dvc-data-1.7.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/CONTRIBUTING.rst` & `dvc-data-1.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/LICENSE` & `dvc-data-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/PKG-INFO` & `dvc-data-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-data
-Version: 1.6.1
+Version: 1.7.0
 Summary: dvc data
 Home-page: https://github.com/iterative/dvc-data
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-data-1.6.1/README.rst` & `dvc-data-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/noxfile.py` & `dvc-data-1.7.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/pyproject.toml` & `dvc-data-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/setup.cfg` & `dvc-data-1.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/cli.py` & `dvc-data-1.7.0/src/dvc_data/cli.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/fs.py` & `dvc-data-1.7.0/src/dvc_data/fs.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/__init__.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/_progress.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/build.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/build.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/cache.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/checkout.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/db/__init__.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/db/index.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/db/index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/db/local.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/db/local.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/db/reference.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/db/reference.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/diff.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/gc.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/hash.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/hash.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/hash_info.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/hash_info.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/istextfile.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/istextfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/meta.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/meta.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/state.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/state.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/status.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/status.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/transfer.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/transfer.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/tree.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import posixpath
 from typing import TYPE_CHECKING, Any, Dict, Final, Iterable, Optional, Tuple
 
 from dvc_objects.errors import ObjectFormatError
 from funcy import cached_property
 
-from ..hashfile.hash import hash_file
+from ..hashfile.hash import DEFAULT_ALGORITHM, hash_file
 from ..hashfile.meta import Meta
 from ..hashfile.obj import HashFile
 
 if TYPE_CHECKING:
     from pygtrie import Trie
 
     from ..hashfile.db import HashFileDB
@@ -71,22 +71,22 @@
         self._dict[key] = (meta, oid)
 
     def get(
         self, key: Tuple[str, ...], default=None
     ) -> Optional[Tuple[Optional["Meta"], Optional["HashInfo"]]]:
         return self._dict.get(key, default)
 
-    def digest(self, with_meta: bool = False):
+    def digest(self, with_meta: bool = False, name: str = DEFAULT_ALGORITHM):
         from dvc_objects.fs import MemoryFileSystem
         from dvc_objects.fs.utils import tmp_fname
 
         memfs = MemoryFileSystem()
         path = "memory://{}".format(tmp_fname(""))
         memfs.pipe_file(path, self.as_bytes())
-        _, self.hash_info = hash_file(path, memfs, "md5")
+        _, self.hash_info = hash_file(path, memfs, name)
         assert self.hash_info.value
         self.fs = memfs
         if with_meta:
             self.path = path + ".with_meta"
             memfs.pipe_file(self.path, self.as_bytes(with_meta=True))
         else:
             self.path = path
```

### Comparing `dvc-data-1.6.1/src/dvc_data/hashfile/utils.py` & `dvc-data-1.7.0/src/dvc_data/hashfile/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/index/__init__.py` & `dvc-data-1.7.0/src/dvc_data/index/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/index/add.py` & `dvc-data-1.7.0/src/dvc_data/index/add.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/index/build.py` & `dvc-data-1.7.0/src/dvc_data/index/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional
 
-from ..hashfile.hash import hash_file
+from ..hashfile.hash import DEFAULT_ALGORITHM, hash_file
 from ..hashfile.meta import Meta
 from .index import DataIndex, DataIndexEntry, FileStorage
 
 if TYPE_CHECKING:
     from dvc_objects.fs.base import FileSystem
 
     from ..hashfile._ignore import Ignore
@@ -14,23 +14,26 @@
 
 def build_entry(
     path: str,
     fs: "FileSystem",
     info: Optional[Dict[str, Any]] = None,
     compute_hash: Optional[bool] = False,
     state: Optional["StateBase"] = None,
+    hash_name: str = DEFAULT_ALGORITHM,
 ):
     if info is None:
         try:
             info = fs.info(path)
         except FileNotFoundError:
             return DataIndexEntry()
 
     if compute_hash and info["type"] != "directory":
-        meta, hash_info = hash_file(path, fs, "md5", state=state, info=info)
+        meta, hash_info = hash_file(
+            path, fs, hash_name, state=state, info=info
+        )
     else:
         meta, hash_info = Meta.from_info(info, fs.protocol), None
 
     return DataIndexEntry(
         meta=meta,
         hash_info=hash_info,
         loaded=meta.isdir or None,
@@ -39,14 +42,15 @@
 
 def build_entries(
     path: str,
     fs: "FileSystem",
     ignore: Optional["Ignore"] = None,
     compute_hash: Optional[bool] = False,
     state: Optional["StateBase"] = None,
+    hash_name: str = DEFAULT_ALGORITHM,
 ) -> Iterable[DataIndexEntry]:
     # NOTE: can't use detail=True with walk, because that will make it error
     # out on broken symlinks.
     if ignore:
         walk_iter = ignore.walk(fs, path)
     else:
         walk_iter = fs.walk(path)
@@ -59,14 +63,15 @@
 
         for name in chain(dirs, files):
             entry = build_entry(
                 fs.path.join(root, name),
                 fs,
                 compute_hash=compute_hash,
                 state=state,
+                hash_name=hash_name,
             )
             entry.key = (*root_key, name)
             yield entry
 
 
 def build(
     path: str, fs: "FileSystem", ignore: Optional["Ignore"] = None
```

### Comparing `dvc-data-1.6.1/src/dvc_data/index/checkout.py` & `dvc-data-1.7.0/src/dvc_data/index/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/index/diff.py` & `dvc-data-1.7.0/src/dvc_data/index/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/index/fetch.py` & `dvc-data-1.7.0/src/dvc_data/index/fetch.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/index/index.py` & `dvc-data-1.7.0/src/dvc_data/index/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -474,15 +474,17 @@
         return self._info_from_entry(key, entry)
 
 
 def _load_from_object_storage(trie, root_entry, storage):
     if not root_entry.hash_info or not root_entry.hash_info.isdir:
         raise FileNotFoundError
 
-    obj = Tree.load(storage.odb, root_entry.hash_info, hash_name="md5")
+    obj = Tree.load(
+        storage.odb, root_entry.hash_info, hash_name=storage.odb.hash_name
+    )
 
     dirs = set()
     for ikey, (meta, hash_info) in obj.iteritems():
         if (
             not meta
             and root_entry.hash_info
             and root_entry.hash_info == hash_info
```

### Comparing `dvc-data-1.6.1/src/dvc_data/index/save.py` & `dvc-data-1.7.0/src/dvc_data/index/save.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import defaultdict
 from functools import wraps
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple
 
 from dvc_objects.fs.callbacks import DEFAULT_CALLBACK
 
+from ..hashfile.hash import DEFAULT_ALGORITHM
 from ..hashfile.hash_info import HashInfo
 from ..hashfile.meta import Meta
 from ..hashfile.tree import Tree
 
 if TYPE_CHECKING:
     from dvc_objects.fs.base import FileSystem
     from dvc_objects.fs.callbacks import Callback
@@ -17,15 +18,15 @@
     from .index import BaseDataIndex, DataIndexKey
 
 
 def md5(
     index: "BaseDataIndex",
     state: Optional["StateBase"] = None,
     storage: str = "data",
-    name: str = "md5",
+    name: str = DEFAULT_ALGORITHM,
     check_meta: bool = True,
 ) -> None:
     from ..hashfile.hash import fobj_md5
     from .index import DataIndexEntry
 
     entries = {}
 
@@ -73,26 +74,27 @@
     for key, entry in entries.items():
         index[key] = entry
 
 
 def build_tree(
     index: "BaseDataIndex",
     prefix: "DataIndexKey",
+    name: str = DEFAULT_ALGORITHM,
 ) -> Tuple["Meta", Tree]:
     tree_meta = Meta(size=0, nfiles=0, isdir=True)
     assert tree_meta.size is not None and tree_meta.nfiles is not None
     tree = Tree()
     for key, entry in index.iteritems(prefix=prefix):
         if key == prefix or entry.meta and entry.meta.isdir:
             continue
         tree_key = key[len(prefix) :]
         tree.add(tree_key, entry.meta, entry.hash_info)
         tree_meta.size += (entry.meta.size if entry.meta else 0) or 0
         tree_meta.nfiles += 1
-    tree.digest()
+    tree.digest(name=name)
     return tree_meta, tree
 
 
 def _save_dir_entry(
     index: "BaseDataIndex",
     key: "DataIndexKey",
     odb: Optional["HashFileDB"] = None,
```

### Comparing `dvc-data-1.6.1/src/dvc_data/index/serialize.py` & `dvc-data-1.7.0/src/dvc_data/index/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/index/view.py` & `dvc-data-1.7.0/src/dvc_data/index/view.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data/repo.py` & `dvc-data-1.7.0/src/dvc_data/repo.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data.egg-info/PKG-INFO` & `dvc-data-1.7.0/src/dvc_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-data
-Version: 1.6.1
+Version: 1.7.0
 Summary: dvc data
 Home-page: https://github.com/iterative/dvc-data
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-data-1.6.1/src/dvc_data.egg-info/SOURCES.txt` & `dvc-data-1.7.0/src/dvc_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/src/dvc_data.egg-info/requires.txt` & `dvc-data-1.7.0/src/dvc_data.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/tests/benchmarks/test_checkout.py` & `dvc-data-1.7.0/tests/benchmarks/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/tests/hashfile/test_cache.py` & `dvc-data-1.7.0/tests/hashfile/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/tests/hashfile/test_db_index.py` & `dvc-data-1.7.0/tests/hashfile/test_db_index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/tests/hashfile/test_diff.py` & `dvc-data-1.7.0/tests/hashfile/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/tests/hashfile/test_hash.py` & `dvc-data-1.7.0/tests/hashfile/test_hash.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/tests/hashfile/test_hash_stream.py` & `dvc-data-1.7.0/tests/hashfile/test_hash_stream.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/tests/hashfile/test_istextfile.py` & `dvc-data-1.7.0/tests/hashfile/test_istextfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/tests/hashfile/test_tree.py` & `dvc-data-1.7.0/tests/hashfile/test_tree.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/tests/hashfile/test_utils.py` & `dvc-data-1.7.0/tests/hashfile/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/tests/index/conftest.py` & `dvc-data-1.7.0/tests/index/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/tests/index/test_checkout.py` & `dvc-data-1.7.0/tests/index/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/tests/index/test_diff.py` & `dvc-data-1.7.0/tests/index/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.6.1/tests/index/test_index.py` & `dvc-data-1.7.0/tests/index/test_index.py`

 * *Files identical despite different names*

