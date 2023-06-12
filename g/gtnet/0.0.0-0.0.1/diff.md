# Comparing `tmp/gtnet-0.0.0.tar.gz` & `tmp/gtnet-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ajtritt/projects/exabiome/deep-taxon/gtnet.git/dist/tmpyx6h4iqg/gtnet-0.0.0.tar", last modified: Thu Oct  7 19:36:41 2021, max compression
+gzip compressed data, was "gtnet-0.0.1.tar", last modified: Mon Jun 12 18:16:05 2023, max compression
```

## Comparing `gtnet-0.0.0.tar` & `gtnet-0.0.1.tar`

### file list

```diff
@@ -1,15 +1,82 @@
-drwxr-xr-x   0 ajtritt    (501) staff       (20)        0 2021-10-07 19:36:41.000000 gtnet-0.0.0/
--rw-r--r--   0 ajtritt    (501) staff       (20)     1098 2021-10-07 19:36:41.000000 gtnet-0.0.0/PKG-INFO
--rw-r--r--   0 ajtritt    (501) staff       (20)       86 2021-08-18 00:50:51.000000 gtnet-0.0.0/README.md
-drwxr-xr-x   0 ajtritt    (501) staff       (20)        0 2021-10-07 19:36:41.000000 gtnet-0.0.0/bin/
--rw-r--r--   0 ajtritt    (501) staff       (20)      830 2021-10-05 19:59:20.000000 gtnet-0.0.0/bin/gtnet-predict
-drwxr-xr-x   0 ajtritt    (501) staff       (20)        0 2021-10-07 19:36:41.000000 gtnet-0.0.0/gtnet.egg-info/
--rw-r--r--   0 ajtritt    (501) staff       (20)     1098 2021-10-07 19:36:41.000000 gtnet-0.0.0/gtnet.egg-info/PKG-INFO
--rw-r--r--   0 ajtritt    (501) staff       (20)      223 2021-10-07 19:36:41.000000 gtnet-0.0.0/gtnet.egg-info/SOURCES.txt
--rw-r--r--   0 ajtritt    (501) staff       (20)        1 2021-10-07 19:36:41.000000 gtnet-0.0.0/gtnet.egg-info/dependency_links.txt
--rw-r--r--   0 ajtritt    (501) staff       (20)        1 2021-10-07 19:22:33.000000 gtnet-0.0.0/gtnet.egg-info/not-zip-safe
--rw-r--r--   0 ajtritt    (501) staff       (20)       41 2021-10-07 19:36:41.000000 gtnet-0.0.0/gtnet.egg-info/requires.txt
--rw-r--r--   0 ajtritt    (501) staff       (20)        1 2021-10-07 19:36:41.000000 gtnet-0.0.0/gtnet.egg-info/top_level.txt
--rw-r--r--   0 ajtritt    (501) staff       (20)      104 2021-10-07 19:26:59.000000 gtnet-0.0.0/pyproject.toml
--rw-r--r--   0 ajtritt    (501) staff       (20)       38 2021-10-07 19:36:41.000000 gtnet-0.0.0/setup.cfg
--rw-r--r--   0 ajtritt    (501) staff       (20)     1725 2021-10-07 19:36:24.000000 gtnet-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.787259 gtnet-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 18:15:53.000000 gtnet-0.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.767258 gtnet-0.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.767258 gtnet-0.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/workflows/codespell.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/workflows/deploy_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/workflows/ruff.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/workflows/run_coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-12 18:15:53.000000 gtnet-0.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-12 18:15:53.000000 gtnet-0.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-12 18:15:53.000000 gtnet-0.0.1/Legal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-06-12 18:16:05.787259 gtnet-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-12 18:15:53.000000 gtnet-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.775259 gtnet-0.0.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-12 18:15:53.000000 gtnet-0.0.1/data/GCA_000006155.2.fna
+-rw-r--r--   0 runner    (1001) docker     (123)    61553 2023-06-12 18:15:53.000000 gtnet-0.0.1/data/small.fna
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-12 18:15:53.000000 gtnet-0.0.1/data/small.raw.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-12 18:15:53.000000 gtnet-0.0.1/data/small.tax.0.05.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.775259 gtnet-0.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.775259 gtnet-0.0.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    35955 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/accuracy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/api_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/legal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18491 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/runtime.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/training.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-12 18:15:53.000000 gtnet-0.0.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-12 18:15:53.000000 gtnet-0.0.1/fetch_model.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-12 18:15:53.000000 gtnet-0.0.1/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-12 18:15:53.000000 gtnet-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-12 18:15:53.000000 gtnet-0.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-12 18:15:53.000000 gtnet-0.0.1/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 18:15:53.000000 gtnet-0.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:16:05.787259 gtnet-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.763258 gtnet-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.779259 gtnet-0.0.1/src/gtnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.779259 gtnet-0.0.1/src/gtnet/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/data/GCA_000006155.2.fna
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.787259 gtnet-0.0.1/src/gtnet/deploy_pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/class.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/class.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/domain.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/domain.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/family.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/family.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/genus.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/genus.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/last.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/order.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/order.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/phylum.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/phylum.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/species.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/species.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.779259 gtnet-0.0.1/src/gtnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-06-12 18:16:05.000000 gtnet-0.0.1/src/gtnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-12 18:16:05.000000 gtnet-0.0.1/src/gtnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:16:05.000000 gtnet-0.0.1/src/gtnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 18:16:05.000000 gtnet-0.0.1/src/gtnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 18:16:05.000000 gtnet-0.0.1/src/gtnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 18:16:05.000000 gtnet-0.0.1/src/gtnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.787259 gtnet-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/tests/test_lca.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-12 18:15:53.000000 gtnet-0.0.1/tests/test_sequence.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

