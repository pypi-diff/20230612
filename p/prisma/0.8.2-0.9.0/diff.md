# Comparing `tmp/prisma-0.8.2.tar.gz` & `tmp/prisma-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prisma-0.8.2.tar", last modified: Sun Mar  5 18:53:08 2023, max compression
+gzip compressed data, was "prisma-0.9.0.tar", last modified: Mon Jun 12 02:14:09 2023, max compression
```

## Comparing `prisma-0.8.2.tar` & `prisma-0.9.0.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:53:08.576430 prisma-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-05 18:52:57.000000 prisma-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-05 18:52:57.000000 prisma-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-03-05 18:53:08.576430 prisma-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-03-05 18:52:57.000000 prisma-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-05 18:52:57.000000 prisma-0.8.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:53:08.568430 prisma-0.8.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-05 18:52:57.000000 prisma-0.8.2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-05 18:52:57.000000 prisma-0.8.2/requirements/node.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 18:53:08.576430 prisma-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-03-05 18:52:57.000000 prisma-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:53:08.568430 prisma-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:53:08.572430 prisma-0.8.2/src/prisma/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/_async_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/_raw_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/_sync_http.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:53:08.572430 prisma-0.8.2/src/prisma/binaries/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/binaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/binaries/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/binaries/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:53:08.572430 prisma-0.8.2/src/prisma/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/cli/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:53:08.572430 prisma-0.8.2/src/prisma/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/cli/commands/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/cli/commands/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/cli/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/cli/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/cli/prisma.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:53:08.572430 prisma-0.8.2/src/prisma/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/engine/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:53:08.572430 prisma-0.8.2/src/prisma/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/jsonrpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    32004 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:53:08.576430 prisma-0.8.2/src/prisma/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/_header.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/_utils.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    32282 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/actions.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/bases.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    22047 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/builder.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    18525 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/client.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:53:08.576430 prisma-0.8.2/src/prisma/generator/templates/engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/engine/abstract.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/engine/http.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/engine/query.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/enums.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/fields.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/http.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/models.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/partials.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/templates/types.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/generator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/http_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/mypy.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:53:08.572430 prisma-0.8.2/src/prisma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-03-05 18:53:08.000000 prisma-0.8.2/src/prisma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-03-05 18:53:08.000000 prisma-0.8.2/src/prisma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 18:53:08.000000 prisma-0.8.2/src/prisma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-05 18:53:08.000000 prisma-0.8.2/src/prisma.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 18:53:08.000000 prisma-0.8.2/src/prisma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-05 18:53:08.000000 prisma-0.8.2/src/prisma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-05 18:53:08.000000 prisma-0.8.2/src/prisma.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 18:53:08.576430 prisma-0.8.2/src/prisma_cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma_cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma_cleanup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma_cleanup/_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 18:52:57.000000 prisma-0.8.2/src/prisma_cleanup/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.599296 prisma-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 02:13:55.000000 prisma-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-12 02:13:55.000000 prisma-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-06-12 02:14:09.599296 prisma-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-06-12 02:13:55.000000 prisma-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-12 02:13:55.000000 prisma-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.591296 prisma-0.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-12 02:13:55.000000 prisma-0.9.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 02:13:55.000000 prisma-0.9.0/requirements/node.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 02:14:09.599296 prisma-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-12 02:13:55.000000 prisma-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.591296 prisma-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.591296 prisma-0.9.0/src/prisma/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_async_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_raw_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_sync_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.595296 prisma-0.9.0/src/prisma/binaries/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/binaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/binaries/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/binaries/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.595296 prisma-0.9.0/src/prisma/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.595296 prisma-0.9.0/src/prisma/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/commands/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/commands/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/prisma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.595296 prisma-0.9.0/src/prisma/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/engine/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/engine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.595296 prisma-0.9.0/src/prisma/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/jsonrpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32409 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.599296 prisma-0.9.0/src/prisma/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/_header.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/_utils.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    35089 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/actions.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/bases.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/builder.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    24425 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/client.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.599296 prisma-0.9.0/src/prisma/generator/templates/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/engine/abstract.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/engine/http.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/engine/query.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/enums.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/fields.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/http.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/models.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/partials.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/types.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/http_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.595296 prisma-0.9.0/src/prisma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.599296 prisma-0.9.0/src/prisma_cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma_cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma_cleanup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma_cleanup/_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma_cleanup/py.typed
```

### Comparing `prisma-0.8.2/LICENSE` & `prisma-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/PKG-INFO` & `prisma-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prisma
-Version: 0.8.2
+Version: 0.9.0
 Summary: Prisma Client Python is an auto-generated and fully type-safe database client
 Home-page: https://github.com/RobertCraigie/prisma-client-py
 Author: Robert Craigie
 Author-email: robert@craigie.dev
 Maintainer: Robert Craigie
 License: APACHE
 Project-URL: Documentation, https://prisma-client-py.readthedocs.io
@@ -40,15 +40,15 @@
     <h1>Prisma Client Python</h1>
     <p><h3 align="center">Type-safe database access for Python</h3></p>
     <div align="center">
     <a href="https://discord.gg/HpFaJbepBH">
         <img src="https://img.shields.io/discord/933860922039099444?color=blue&label=chat&logo=discord" alt="Chat on Discord">
     </a>
     <a href="https://prisma.io">
-        <img src="https://img.shields.io/static/v1?label=prisma&message=4.11.0&color=blue&logo=prisma" alt="Supported Prisma version is 4.11.0">
+        <img src="https://img.shields.io/static/v1?label=prisma&message=4.15.0&color=blue&logo=prisma" alt="Supported Prisma version is 4.15.0">
     </a>
     <a href="https://github.com/grantjenks/blue">
         <img src="https://camo.githubusercontent.com/dbdbcf26db37abfa1f2ab7e6c28c8b3a199f2dad98e4ef53a50e9c45c7e4ace8/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c75652d626c75652e737667" alt="Code style: blue">
     </a>
     <a href="https://robertcraigie.github.io/prisma-client-py/htmlcov/index.html">
         <img src="https://raw.githubusercontent.com/RobertCraigie/prisma-client-py/static/coverage/coverage.svg" alt="Code coverage report">
     </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prisma Version: 0.8.2 Summary: Prisma Client Python
+Metadata-Version: 2.1 Name: prisma Version: 0.9.0 Summary: Prisma Client Python
 is an auto-generated and fully type-safe database client Home-page: https://
 github.com/RobertCraigie/prisma-client-py Author: Robert Craigie Author-email:
 robert@craigie.dev Maintainer: Robert Craigie License: APACHE Project-URL:
 Documentation, https://prisma-client-py.readthedocs.io Project-URL: Source,
 https://github.com/RobertCraigie/prisma-client-py Project-URL: Tracker, https:/
 /github.com/RobertCraigie/prisma-client-py/issues Keywords:
 orm,mysql,typing,prisma,sqlite,database,postgresql Platform: UNKNOWN
@@ -17,15 +17,15 @@
 Python :: 3.11 Classifier: Operating System :: POSIX Classifier: Operating
 System :: MacOS Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Requires-Python: >=3.7.0 Description-
 Content-Type: text/markdown Provides-Extra: node Provides-Extra: all License-
 File: LICENSE
                       ****** Prisma Client Python ******
                 **** Type-safe database access for Python ****
-[Chat_on_Discord] [Supported_Prisma_version_is_4.11.0] [Code_style:_blue] [Code
+[Chat_on_Discord] [Supported_Prisma_version_is_4.15.0] [Code_style:_blue] [Code
  coverage_report] [GitHub Workflow Status (main)] [Supported python versions]
                            [Latest package version]
 ===============================================================================
 ## What is Prisma Client Python? Prisma Client Python is a next-generation ORM
 built on top of [Prisma](https://github.com/prisma/prisma) that has been
 designed from the ground up for ease of use and correctness. [Prisma](https://
 www.prisma.io/) is a TypeScript ORM with zero-cost type safety for your
```

### Comparing `prisma-0.8.2/README.md` & `prisma-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     <h1>Prisma Client Python</h1>
     <p><h3 align="center">Type-safe database access for Python</h3></p>
     <div align="center">
     <a href="https://discord.gg/HpFaJbepBH">
         <img src="https://img.shields.io/discord/933860922039099444?color=blue&label=chat&logo=discord" alt="Chat on Discord">
     </a>
     <a href="https://prisma.io">
-        <img src="https://img.shields.io/static/v1?label=prisma&message=4.11.0&color=blue&logo=prisma" alt="Supported Prisma version is 4.11.0">
+        <img src="https://img.shields.io/static/v1?label=prisma&message=4.15.0&color=blue&logo=prisma" alt="Supported Prisma version is 4.15.0">
     </a>
     <a href="https://github.com/grantjenks/blue">
         <img src="https://camo.githubusercontent.com/dbdbcf26db37abfa1f2ab7e6c28c8b3a199f2dad98e4ef53a50e9c45c7e4ace8/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c75652d626c75652e737667" alt="Code style: blue">
     </a>
     <a href="https://robertcraigie.github.io/prisma-client-py/htmlcov/index.html">
         <img src="https://raw.githubusercontent.com/RobertCraigie/prisma-client-py/static/coverage/coverage.svg" alt="Code coverage report">
     </a>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 
                       ****** Prisma Client Python ******
                 **** Type-safe database access for Python ****
-[Chat_on_Discord] [Supported_Prisma_version_is_4.11.0] [Code_style:_blue] [Code
+[Chat_on_Discord] [Supported_Prisma_version_is_4.15.0] [Code_style:_blue] [Code
  coverage_report] [GitHub Workflow Status (main)] [Supported python versions]
                            [Latest package version]
 ===============================================================================
 ## What is Prisma Client Python? Prisma Client Python is a next-generation ORM
 built on top of [Prisma](https://github.com/prisma/prisma) that has been
 designed from the ground up for ease of use and correctness. [Prisma](https://
 www.prisma.io/) is a TypeScript ORM with zero-cost type safety for your
```

### Comparing `prisma-0.8.2/pyproject.toml` & `prisma-0.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     "src",
     "tests",
     "scripts"
 ]
 ignore = [
     # these are type checked separately
     "databases/tests",
+    "databases/sync_tests",
     # TODO: this should not ignore tests/integrations/conftest.py
     "tests/integrations/**/*",
 ]
 pythonVersion = "3.9"
 
 # NOTE: whenever you update any of these values you will most likely also have to update `databases/constants.py::PYRIGHT_CONFIG`
 typeCheckingMode = "strict"
```

### Comparing `prisma-0.8.2/setup.py` & `prisma-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/__init__.py` & `prisma-0.9.0/src/prisma/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # -*- coding: utf-8 -*-
 
 __title__ = 'prisma'
 __author__ = 'RobertCraigie'
 __license__ = 'APACHE'
 __copyright__ = 'Copyright 2020-2023 RobertCraigie'
-__version__ = '0.8.2'
+__version__ = '0.9.0'
 
 from typing import TYPE_CHECKING
 
 from ._config import config as config
 from .utils import setup_logging
 from . import errors as errors
 from .validator import *
+from ._types import PrismaMethod as PrismaMethod
 
 
 try:
     from .client import *
     from .fields import *
     from . import (
         models as models,
         partials as partials,
         types as types,
+        bases as bases,
     )
 except ModuleNotFoundError:
     # code has not been generated yet
     # TODO: this could swallow unexpected errors
 
     # we only define this magic function when the client has not
     # been generated for performance reasons and we hide it from
```

### Comparing `prisma-0.8.2/src/prisma/_async_http.py` & `prisma-0.9.0/src/prisma/_async_http.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/_compat.py` & `prisma-0.9.0/src/prisma/_compat.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/_config.py` & `prisma-0.9.0/src/prisma/_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 
 class DefaultConfig(BaseSettings):
     # CLI version
     # TODO: if this version changes but the engine version
     #       doesn't change then the CLI is incorrectly cached
     prisma_version: str = Field(
         env='PRISMA_VERSION',
-        default='4.11.0',
+        default='4.15.0',
     )
 
     # Engine binary versions can be found under https://github.com/prisma/prisma-engine/commits/main
     expected_engine_version: str = Field(
         env='PRISMA_EXPECTED_ENGINE_VERSION',
-        default='8fde8fef4033376662cad983758335009d522acb',
+        default='8fbc245156db7124f997f4cecdd8d1219e360944',
     )
 
     # Home directory, used to build the `binary_cache_dir` option by default, useful in multi-user
     # or testing environments so that the binaries can be easily cached without having to worry
     # about versioning them.
     home_dir: Path = Field(
         env='PRISMA_HOME_DIR',
```

### Comparing `prisma-0.8.2/src/prisma/_proxy.py` & `prisma-0.9.0/src/prisma/_proxy.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/_raw_query.py` & `prisma-0.9.0/src/prisma/_raw_query.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/_sync_http.py` & `prisma-0.9.0/src/prisma/_sync_http.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/_types.py` & `prisma-0.9.0/src/prisma/_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,7 +22,31 @@
 @runtime_checkable
 class InheritsGeneric(Protocol):
     __orig_bases__: Tuple['_GenericAlias']
 
 
 class _GenericAlias(Protocol):
     __origin__: Type[object]
+
+
+PrismaMethod = Literal[
+    # raw queries
+    'query_raw',
+    'query_first',
+    'execute_raw',
+    # mutatitive queries
+    'create',
+    'delete',
+    'update',
+    'upsert',
+    'create_many',
+    'delete_many',
+    'update_many',
+    # read queries
+    'count',
+    'group_by',
+    'find_many',
+    'find_first',
+    'find_first_or_raise',
+    'find_unique',
+    'find_unique_or_raise',
+]
```

### Comparing `prisma-0.8.2/src/prisma/binaries/platform.py` & `prisma-0.9.0/src/prisma/binaries/platform.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/cli/_node.py` & `prisma-0.9.0/src/prisma/cli/_node.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/cli/cli.py` & `prisma-0.9.0/src/prisma/cli/cli.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/cli/commands/dev.py` & `prisma-0.9.0/src/prisma/cli/commands/dev.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Commands for developing Prisma Client Python"""
 
 
 # There are some weird false positives that `cli` being a `Group` introduces
 # for some reason. Fixing the errors for one type checker causes errors in an another
 # so just switch to Any for the time being as this is internal and only used once, directly
 # below this line.
-cli = cast(Any, _cli)
+cli: Any = cast(Any, _cli)
 
 
 @cli.command()  # type: ignore[misc]
 @options.schema
 @options.skip_generate
 def playground(schema: Optional[str], skip_generate: bool) -> None:
     """Run the GraphQL playground"""
```

### Comparing `prisma-0.8.2/src/prisma/cli/commands/fetch.py` & `prisma-0.9.0/src/prisma/cli/commands/fetch.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/cli/commands/generate.py` & `prisma-0.9.0/src/prisma/cli/commands/generate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import logging
 from pathlib import Path
-from typing import Optional, Dict, Any
+from typing import Optional, Dict, Any, Tuple
 
 import click
 import pydantic
 
 from .. import prisma, options
 from ..utils import EnumChoice, PathlibPath, warning
 from ...generator.models import InterfaceChoices
@@ -34,29 +34,40 @@
 )
 @click.option(
     '-t',
     '--type-depth',
     type=int,
     help='Depth to generate pseudo-recursive types to; -1 signifies fully recursive types',
 )
-def cli(schema: Optional[Path], watch: bool, **kwargs: Any) -> None:
+@click.option(
+    '--generator',
+    multiple=True,
+    help='Specifies which generator to use. Can be specified multiple times. By default, all generators will be ran',
+)
+def cli(
+    schema: Optional[Path], watch: bool, generator: Tuple[str], **kwargs: Any
+) -> None:
     """Generate prisma artifacts with modified config options"""
     if pydantic.VERSION.split('.') < ['1', '8']:
         warning(
             'Unsupported version of pydantic installed, this command may not work as intended\n'
             'Please update pydantic to 1.8 or greater.\n'
         )
 
     args = ['generate']
     if schema is not None:
         args.append(f'--schema={schema}')
 
     if watch:
         args.append('--watch')
 
+    if generator:
+        for name in generator:
+            args.append(f'--generator={name}')
+
     env: Dict[str, str] = {}
     prefix = 'PRISMA_PY_CONFIG_'
     for key, value in kwargs.items():
         if value is None:
             continue
 
         env[prefix + ARG_TO_CONFIG_KEY.get(key, key).upper()] = serialize(
```

### Comparing `prisma-0.8.2/src/prisma/cli/commands/version.py` & `prisma-0.9.0/src/prisma/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/cli/options.py` & `prisma-0.9.0/src/prisma/cli/options.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/cli/prisma.py` & `prisma-0.9.0/src/prisma/cli/prisma.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/cli/utils.py` & `prisma-0.9.0/src/prisma/cli/utils.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/engine/errors.py` & `prisma-0.9.0/src/prisma/engine/errors.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/engine/utils.py` & `prisma-0.9.0/src/prisma/engine/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,20 @@
     'P2010': prisma_errors.RawQueryError,
     'P2012': prisma_errors.MissingRequiredValueError,
     'P2019': prisma_errors.InputError,
     'P2021': prisma_errors.TableNotFoundError,
     'P2025': prisma_errors.RecordNotFoundError,
 }
 
+META_ERROR_MAPPING: dict[str, type[Exception]] = {
+    'UnknownArgument': prisma_errors.FieldNotFoundError,
+    'UnknownInputField': prisma_errors.FieldNotFoundError,
+    'UnknownSelectionField': prisma_errors.FieldNotFoundError,
+}
+
 
 def query_engine_name() -> str:
     return f'prisma-query-engine-{platform.check_for_extension(platform.binary_platform())}'
 
 
 def _resolve_from_binary_paths(binary_paths: dict[str, str]) -> Path | None:
     if config.binary_platform is not None:
@@ -105,15 +111,15 @@
     if not file:
         if file_from_paths is not None:
             expected = f'{local_path}, {global_path} or {file_from_paths} to exist but none'
         else:
             expected = f'{local_path} or {global_path} to exist but neither'
 
         raise errors.BinaryNotFoundError(
-            f'Expected {expected} were found.\n'
+            f'Expected {expected} were found or could not be executed.\n'
             + 'Try running prisma py fetch'
         )
 
     log.debug('Using Query Engine binary at %s', file)
 
     start_version = time.monotonic()
     process = subprocess.run(
@@ -145,33 +151,53 @@
     sock.close()
     return int(port)
 
 
 def handle_response_errors(resp: AbstractResponse[Any], data: Any) -> NoReturn:
     for error in data:
         try:
+            base_error_message = error.get('error', '')
             user_facing = error.get('user_facing_error', {})
             code = user_facing.get('error_code')
             if code is None:
                 continue
 
             # TODO: the order of these if statements is important because
             # the P2009 code can be returned for both: missing a required value
             # and an unknown field error. As we want to explicitly handle
             # the missing a required value error then we need to check for that first.
             # As we can only check for this error by searching the message then this
             # comes with performance concerns.
             message = user_facing.get('message', '')
+
+            if code == 'P2028':
+                if base_error_message.startswith('Transaction already closed'):
+                    raise prisma_errors.TransactionExpiredError(
+                        base_error_message
+                    )
+                raise prisma_errors.TransactionError(message)
+
             if 'A value is required but not set' in message:
                 raise prisma_errors.MissingRequiredValueError(error)
 
-            exc = ERROR_MAPPING.get(code)
+            exc: type[Exception] | None = None
+
+            kind = user_facing.get('meta', {}).get('kind')
+            if kind is not None:
+                exc = META_ERROR_MAPPING.get(kind)
+
+            if exc is None:
+                exc = ERROR_MAPPING.get(code)
+
             if exc is not None:
                 raise exc(error)
-        except (KeyError, TypeError):
+        except (KeyError, TypeError) as err:
+            log.debug(
+                'Ignoring error while constructing specialized error %s', err
+            )
             continue
 
     try:
         raise prisma_errors.DataError(data[0])
     except (IndexError, TypeError):
         pass
```

### Comparing `prisma-0.8.2/src/prisma/generator/generator.py` & `prisma-0.9.0/src/prisma/generator/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,16 +170,15 @@
             self.generate(data)
             response = jsonrpc.SuccessResponse(id=request.id, result=None)
         else:  # pragma: no cover
             raise RuntimeError(
                 f'JSON RPC received unexpected method: {request.method}'
             )
 
-        if response is not None:
-            jsonrpc.reply(response)
+        jsonrpc.reply(response)
 
     @cached_property
     def data_class(self) -> Type[BaseModelT]:
         """Return the BaseModel used to parse the Prisma DMMF"""
 
         # we need to cast to object as otherwise pyright correctly marks the code as unreachable,
         # this is because __orig_bases__ is not present in the typeshed stubs as it is
```

### Comparing `prisma-0.8.2/src/prisma/generator/jsonrpc.py` & `prisma-0.9.0/src/prisma/generator/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/generator/models.py` & `prisma-0.9.0/src/prisma/generator/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -576,14 +576,27 @@
     prisma_schema: Any = FieldInfo(alias='schema')
 
 
 class Datamodel(BaseModel):
     enums: List['Enum']
     models: List['Model']
 
+    # not implemented yet
+    types: List[object]
+
+    @validator('types')
+    @classmethod
+    def no_composite_types_validator(cls, types: List[object]) -> object:
+        if types:
+            raise ValueError(
+                'Composite types are not supported yet. Please indicate you need this here: https://github.com/RobertCraigie/prisma-client-py/issues/314'
+            )
+
+        return types
+
 
 class Enum(BaseModel):
     name: str
     db_name: Optional[str] = FieldInfo(alias='dbName')
     values: List['EnumValue']
```

### Comparing `prisma-0.8.2/src/prisma/generator/schema.py` & `prisma-0.9.0/src/prisma/generator/schema.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/generator/templates/_header.py.jinja` & `prisma-0.9.0/src/prisma/generator/templates/_header.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/generator/templates/actions.py.jinja` & `prisma-0.9.0/src/prisma/generator/templates/actions.py.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% set annotations = true %}
 {% include '_header.py.jinja' %}
-{% from '_utils.py.jinja' import is_async, maybe_async_def, maybe_await, methods, operations, recursive_types, active_provider with context %}
+{% from '_utils.py.jinja' import is_async, maybe_async_def, maybe_await, recursive_types, active_provider with context %}
 # -- template actions.py.jinja --
 from typing import TypeVar
 import warnings
 
 from . import types, errors, bases
 
 if TYPE_CHECKING:
@@ -167,16 +167,15 @@
                 {% endif %}
                 {% endfor %}
             },
         )
         ```
         """
         resp = {{ maybe_await }}self._client._execute(
-            operation='{{ operations.create }}',
-            method='{{ methods.create }}',
+            method='create',
             model=self._model,
             arguments={
                 'data': data,
                 'include': include,
             },
         )
         return self._model.parse_obj(resp['data']['result'])
@@ -232,16 +231,15 @@
         )
         ```
         """
         if self._client._active_provider == 'sqlite':
             raise errors.UnsupportedDatabaseError('sqlite', 'create_many()')
 
         resp = {{ maybe_await }}self._client._execute(
-            operation='{{ operations.create_many }}',
-            method='{{ methods.create_many }}',
+            method='create_many',
             model=self._model,
             arguments={
                 'data': data,
                 'skipDuplicates': skip_duplicates,
             },
             root_selection=['count'],
         )
@@ -281,16 +279,15 @@
                 {{ sample_where_unique(model) }}
             },
         )
         ```
         """
         try:
             resp = {{ maybe_await }}self._client._execute(
-                operation='{{ operations.delete }}',
-                method='{{ methods.delete }}',
+                method='delete',
                 model=self._model,
                 arguments={
                     'where': where,
                     'include': include,
                 },
             )
         except errors.RecordNotFoundError:
@@ -331,27 +328,72 @@
             where={
                 {{ sample_where_unique(model) }}
             },
         )
         ```
         """
         resp = {{ maybe_await }}self._client._execute(
-            operation='{{ operations.find_unique }}',
-            method='{{ methods.find_unique }}',
+            method='find_unique',
             model=self._model,
             arguments={
                 'where': where,
                 'include': include,
             },
         )
         result = resp['data']['result']
         if result is None:
             return None
         return self._model.parse_obj(result)
 
+    {{ maybe_async_def }}find_unique_or_raise(
+        self,
+        where: types.{{ model.name }}WhereUniqueInput,
+        include: Optional[types.{{ model.name}}Include] = None
+    ) -> {{ ModelType }}:
+        """Find a unique {{ model.name }} record. Raises `RecordNotFoundError` if no record is found.
+
+        Parameters
+        ----------
+        where
+            {{ model.name }} filter to find the record, must be unique
+        include
+            {{ include_doc }}
+
+        Returns
+        -------
+        {{ RawModelType }}
+            The found {{ model.name }} record
+
+        Raises
+        ------
+        prisma.errors.RecordNotFoundError
+            No record was found
+        {{ base_error_doc }}
+        {{ query_error_doc }}
+
+        Example
+        -------
+        ```py
+        {{ model.name.lower() }} = {{ maybe_await }}{{ model.name }}.prisma().find_unique_or_raise(
+            where={
+                {{ sample_where_unique(model) }}
+            },
+        )
+        ```
+        """
+        resp = {{ maybe_await }}self._client._execute(
+            method='find_unique_or_raise',
+            model=self._model,
+            arguments={
+                'where': where,
+                'include': include,
+            },
+        )
+        return self._model.parse_obj(resp['data']['result'])
+
     {{ maybe_async_def }}find_many(
         self,
         take: Optional[int] = None,
         skip: Optional[int] = None,
         where: Optional[types.{{ model.name }}WhereInput] = None,
         cursor: Optional[types.{{ model.name }}WhereUniqueInput] = None,
         include: Optional[types.{{ model.name }}Include] = None,
@@ -401,16 +443,15 @@
             order={
                 '{{ field.name }}': 'desc',
             },
         )
         ```
         """
         resp = {{ maybe_await }}self._client._execute(
-            operation='{{ operations.find_many }}',
-            method='{{ methods.find_many }}',
+            method='find_many',
             model=self._model,
             arguments={
                 'take': take,
                 'skip': skip,
                 'where': where,
                 'order_by': order,
                 'cursor': cursor,
@@ -467,16 +508,15 @@
             order={
                 '{{ field.name }}': 'desc',
             },
         )
         ```
         """
         resp = {{ maybe_await }}self._client._execute(
-            operation='{{ operations.find_first }}',
-            method='{{ methods.find_first }}',
+            method='find_first',
             model=self._model,
             arguments={
                 'skip': skip,
                 'where': where,
                 'order_by': order,
                 'cursor': cursor,
                 'include': include,
@@ -484,14 +524,78 @@
             },
         )
         result = resp['data']['result']
         if result is None:
             return None
         return self._model.parse_obj(result)
 
+    {{ maybe_async_def }}find_first_or_raise(
+        self,
+        skip: Optional[int] = None,
+        where: Optional[types.{{ model.name }}WhereInput] = None,
+        cursor: Optional[types.{{ model.name }}WhereUniqueInput] = None,
+        include: Optional[types.{{ model.name }}Include] = None,
+        order: Optional[Union[types.{{ model.name }}OrderByInput, List[types.{{ model.name }}OrderByInput]]] = None,
+        distinct: Optional[List[types.{{ model.name }}ScalarFieldKeys]] = None,
+    ) -> {{ ModelType }}:
+        """Find a single {{ model.name }} record. Raises `RecordNotFoundError` if no record was found.
+
+        Parameters
+        ----------
+        skip
+            Ignore the first N records
+        where
+            {{ model.name }} filter to select the record
+        cursor
+            Specifies the position in the list to start returning results from, (typically an ID field)
+        include
+            {{ include_doc }}
+        order
+            Order the returned {{ model.name }} records by any field
+        distinct
+            Filter {{ model.name }} records by either a single distinct field or distinct combinations of fields
+
+        Returns
+        -------
+        {{ RawModelType }}
+            The first {{ model.name }} record found, matching the given arguments
+
+        Raises
+        ------
+        prisma.errors.RecordNotFoundError
+            No record was found
+        {{ base_error_doc }}
+
+        Example
+        -------
+        ```py
+        {% set field = model.sampler().get_field() %}
+        # find the second {{ model.name }} record ordered by the {{ field.name }} field
+        {{ model.name.lower() }} = {{ maybe_await }}{{ model.name }}.prisma().find_first_or_raise(
+            skip=1,
+            order={
+                '{{ field.name }}': 'desc',
+            },
+        )
+        ```
+        """
+        resp = {{ maybe_await }}self._client._execute(
+            method='find_first_or_raise',
+            model=self._model,
+            arguments={
+                'skip': skip,
+                'where': where,
+                'order_by': order,
+                'cursor': cursor,
+                'include': include,
+                'distinct': distinct,
+            },
+        )
+        return self._model.parse_obj(resp['data']['result'])
+
     {{ maybe_async_def }}update(
         self,
         data: types.{{ model.name }}UpdateInput,
         where: types.{{ model.name }}WhereUniqueInput,
         include: Optional[types.{{ model.name}}Include] = None
     ) -> Optional[{{ ModelType }}]:
         """Update a single {{ model.name }} record.
@@ -527,16 +631,15 @@
                 # data to update the {{ model.name }} record to
             },
         )
         ```
         """
         try:
             resp = {{ maybe_await }}self._client._execute(
-                operation='{{ operations["update"] }}',
-                method='{{ methods["update"] }}',
+                method='update',
                 model=self._model,
                 arguments={
                     'data': data,
                     'where': where,
                     'include': include,
                 },
             )
@@ -613,16 +716,15 @@
                 },
             },
         )
         {% endif %}
         ```
         """
         resp = {{ maybe_await }}self._client._execute(
-            operation='{{ operations.upsert }}',
-            method='{{ methods.upsert }}',
+            method='upsert',
             model=self._model,
             arguments={
                 'where': where,
                 'include': include,
                 'create': data.get('create'),
                 'update': data.get('update'),
             },
@@ -662,16 +764,15 @@
                 '{{ field.name }}': {{ field.get_sample_data() }}
             },
             where={}
         )
         ```
         """
         resp = {{ maybe_await }}self._client._execute(
-            operation='{{ operations.update_many }}',
-            method='{{ methods.update_many }}',
+            method='update_many',
             model=self._model,
             arguments={'data': data, 'where': where,},
             root_selection=['count'],
         )
         return int(resp['data']['result']['count'])
 
     @overload
@@ -769,16 +870,15 @@
             {% raw %}
             root_selection = [
                 '_count {{ {0} }}'.format(' '.join(k for k, v in select.items() if v is True))
             ]
             {% endraw %}
 
         resp = {{ maybe_await }}self._client._execute(
-            operation='{{ operations.count }}',
-            method='{{ methods.count }}',
+            method='count',
             model=self._model,
             arguments={
                 'take': take,
                 'skip': skip,
                 'where': where,
                 'cursor': cursor,
             },
@@ -814,16 +914,15 @@
         -------
         ```py
         # delete all {{ model.name }} records
         total = {{ maybe_await }}{{ model.name }}.prisma().delete_many()
         ```
         """
         resp = {{ maybe_await }}self._client._execute(
-            operation='{{ operations.delete_many }}',
-            method='{{ methods.delete_many }}',
+            method='delete_many',
             model=self._model,
             arguments={'where': where},
             root_selection=['count'],
         )
         return int(resp['data']['result']['count'])
 
     # TODO: make this easier to work with safely, currently output fields are typed as
@@ -933,16 +1032,15 @@
         if count is not None:
             if count is True:
                 root_selection.append('_count { _all }')
             elif isinstance(count, dict):
                 root_selection.append(_select_fields('_count', count))
 
         resp = {{ maybe_await }}self._client._execute(
-            operation='{{ operations.group_by }}',
-            method='{{ methods.group_by }}',
+            method='group_by',
             model=self._model,
             arguments={
                 'by': by,
                 'take': take,
                 'skip': skip,
                 'where': where,
                 'having': having,
@@ -962,8 +1060,7 @@
     """
     {% raw %}
     return root + ' {{ {0} }}'.format(' '.join(k for k, v in select.items() if v is True))
     {% endraw %}
 
 
 from . import models
-
```

### Comparing `prisma-0.8.2/src/prisma/generator/templates/bases.py.jinja` & `prisma-0.9.0/src/prisma/generator/templates/bases.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/generator/templates/builder.py.jinja` & `prisma-0.9.0/src/prisma/generator/templates/builder.py.jinja`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 {% set annotations = true %}
 {% include '_header.py.jinja' %}
 {% from '_utils.py.jinja' import maybe_async_def, maybe_await with context %}
 # -- template builder.py.jinja --
 
-# TODO: the QueryBuilder should validate and add type information context.
-#       currently we just naively iterate through arguments and encode them
-#       using standard json when we don't have any special casing for it.
-#       this makes it more difficult to add support for non-standard types
-#       such as the `Json` type.
-# TODO: optimise for performance (switch to c / cython?)
-# TODO: pass context around differently, relying on the builder instance is
-#       not ideal, context should be local to each node
-
-
 import json
 import logging
 import inspect
 from textwrap import indent
 from datetime import timezone
 from abc import abstractmethod, ABC
 from functools import singledispatch
+from typing import ForwardRef
+from typing_extensions import TypeGuard
 
+from pydantic import BaseModel
 from pydantic.fields import ModelField
 
 from . import fields
 from .types import Serializable
 from .errors import UnknownModelError, UnknownRelationalFieldError, InvalidModelError
 from ._constants import QUERY_BUILDER_ALIASES
+from ._types import PrismaMethod
 
 if TYPE_CHECKING:
     from .bases import _PrismaModel as PrismaModel
 
 
 log: logging.Logger = logging.getLogger(__name__)
 
@@ -48,67 +42,126 @@
         {% for field in model.relational_fields %}
         '{{ field.name }}': '{{ field.get_relational_model().name }}',
         {% endfor %}
     },
     {% endfor %}
 }
 
+METHOD_OPERATION_MAPPING: dict[PrismaMethod, Operation] = {
+    'create': 'mutation',
+    'delete': 'mutation',
+    'update': 'mutation',
+    'upsert': 'mutation',
+    'query_raw': 'mutation',
+    'query_first': 'mutation',
+    'create_many': 'mutation',
+    'execute_raw': 'mutation',
+    'delete_many': 'mutation',
+    'update_many': 'mutation',
+
+    'count': 'query',
+    'group_by': 'query',
+    'find_many': 'query',
+    'find_first': 'query',
+    'find_first_or_raise': 'query',
+    'find_unique': 'query',
+    'find_unique_or_raise': 'query',
+}
+
+METHOD_FORMAT_MAPPING: dict[PrismaMethod, str] = {
+    'create': 'createOne{model}',
+    'delete': 'deleteOne{model}',
+    'update': 'updateOne{model}',
+    'upsert': 'upsertOne{model}',
+    'query_raw': 'queryRaw',
+    'query_first': 'queryRaw',
+    'create_many': 'createMany{model}',
+    'execute_raw': 'executeRaw',
+    'delete_many': 'deleteMany{model}',
+    'update_many': 'updateMany{model}',
+
+    'count': 'aggregate{model}',
+    'group_by': 'groupBy{model}',
+    'find_many': 'findMany{model}',
+    'find_first': 'findFirst{model}',
+    'find_first_or_raise': 'findFirst{model}OrThrow',
+    'find_unique': 'findUnique{model}',
+    'find_unique_or_raise': 'findUnique{model}OrThrow',
+}
+
 MISSING = object()
+Operation = Literal['query', 'mutation']
+
 
 
 class QueryBuilder:
-    # prisma method
-    method: str
+    method: PrismaMethod
+    """The name of the actions method that this query is for, e.g. `find_unique`"""
 
-    # GraphQL operation
-    operation: str
+    method_format: str
+    """Template denoting how the internal method name should be constructed, e.g. `findUnique{model}`"""
 
-    # prisma model
-    model: Optional[Type[PrismaModel]]
+    operation: Operation
+    """The GraphQL operatiom e.g. `query`, `mutation`"""
 
-    # mapping of relational fields to include in the result
-    include: Optional[Dict[str, Any]]
+    model: type[PrismaModel] | None
+    """The Pydantic model that will be used to parse the response.
 
-    # arguments to pass to the query
-    arguments: Dict[str, Any]
+    Used to extract the model name & build selections.
+    """
+
+    include: dict[str, Any] | None
+    """Mapping of relational fields to include in the result"""
 
-    # list of fields to select
-    root_selection: Optional[List[str]]
+    arguments: dict[str, Any]
+    """Arguments to pass to the query"""
+
+    root_selection: list[str] | None
+    """List of fields to select"""
 
     __slots__ = (
         'method',
+        'method_format',
         'operation',
         'model',
         'include',
         'arguments',
         'root_selection',
     )
 
     def __init__(
         self,
         *,
-        method: str,
-        operation: str,
-        arguments: Dict[str, Any],
-        model: Optional[Type[PrismaModel]] = None,
-        root_selection: Optional[List[str]] = None
+        method: PrismaMethod,
+        arguments: dict[str, Any],
+        model: type[BaseModel] | None = None,
+        root_selection: list[str] | None = None
     ) -> None:
-        self.model = model
         self.method = method
-        self.operation = operation
+        self.method_format = METHOD_FORMAT_MAPPING[method]
+        self.operation = METHOD_OPERATION_MAPPING[method]
         self.root_selection = root_selection
         self.arguments = args = self._transform_aliases(arguments)
         self.include = args.pop('include', None)
 
-        if model is not None and not hasattr(model, '__prisma_model__'):
-            raise InvalidModelError(model)
+        # Note: we ignore the `model` argument for raw queries as users may want to pass in a model
+        # that isn't a `PrismaModel` because they've defined it manually & enforcing that
+        # they subclass `PrismaModel` doesn't bring any real benefits.
+        if model is None or method in {'execute_raw', 'query_raw', 'query_first'}:
+            self.model = None
+        else:
+            if not _is_prisma_model_type(model) or not hasattr(model, '__prisma_model__'):
+                raise InvalidModelError(model)
+
+            self.model = model
+
 
     def build(self) -> str:
         """Build the payload that should be sent to the QueryEngine"""
-        data = {
+        data: dict[str, object] = {
             'variables': {},
             'operation_name': self.operation,
             'query': self.build_query(),
         }
         return dumps(data)
 
     def build_query(self) -> str:
@@ -147,15 +200,15 @@
                 model=self.model,
                 include=self.include,
                 root_selection=self.root_selection,
             )
         )
         return root
 
-    def get_default_fields(self, model: Type[PrismaModel]) -> List[str]:
+    def get_default_fields(self, model: type[PrismaModel]) -> list[str]:
         """Returns a list of all the scalar fields of a model
 
         Raises UnknownModelError if the current model cannot be found.
         """
         name = getattr(model, '__prisma_model__', MISSING)
         if name is MISSING:
             raise InvalidModelError(model)
@@ -165,15 +218,15 @@
             raise UnknownModelError(name)
 
         # by default we exclude every field that points to a PrismaModel as that indicates that it is a relational field
         # we explicitly keep fields that point to anything else, even other pydantic.BaseModel types, as they can be used to deserialize JSON
         return [
             field
             for field, info in model.__fields__.items()
-            if not _field_is_prisma_model(info)
+            if not _field_is_prisma_model(info, parent=model)
         ]
 
     def get_relational_model(self, current_model: Type[PrismaModel], field: str) -> Type[PrismaModel]:
         """Returns the model that the field is related to.
 
         Raises UnknownModelError if the current model is invalid.
         Raises UnknownRelationalFieldError if the field does not exist.
@@ -193,15 +246,15 @@
             raise UnknownRelationalFieldError(model=current_model.__name__, field=field)
 
         try:
             info = current_model.__fields__[field]
         except KeyError as exc:
             raise UnknownRelationalFieldError(model=current_model.__name__, field=field)
 
-        if not _field_is_prisma_model(info):
+        if not _field_is_prisma_model(info, parent=current_model):
             raise RuntimeError(
                 f'The `{field}` field doesn\'t appear to be a Prisma Model type. ' +
                 'Is the field a pydantic.BaseModel type and does it have a `__prisma_model__` class variable?'
             )
 
         return cast('Type[PrismaModel]', info.type_)
 
@@ -223,22 +276,34 @@
                     for data in value
                 ]
             else:
                 transformed[alias] = value
         return transformed
 
 
-def _field_is_prisma_model(field: ModelField) -> bool:
+def _field_is_prisma_model(field: ModelField, *, parent: type[BaseModel]) -> bool:
   """Whether or not the given field info represents a model at the database level.
 
   This will return `True` for cases where the field represents a list of models or a single model.
   """
+  if isinstance(field.type_, ForwardRef):
+      cls_name = parent.__name__
+      raise RuntimeError(
+        f'Encountered forward reference for {cls_name}.{field.name}; Forward references must be evaluated using {cls_name}.update_forward_refs()'
+      )
+
   return hasattr(field.type_, '__prisma_model__')
 
 
+def _is_prisma_model_type(type_: type[BaseModel]) -> TypeGuard[type[PrismaModel]]:
+    from .bases import _PrismaModel
+
+    return issubclass(type_, _PrismaModel)
+
+
 class AbstractNode(ABC):
     __slots__ = ()
 
     @abstractmethod
     def render(self) -> Optional[str]:
         """Render the node to a string
 
@@ -408,17 +473,20 @@
 
     def __init__(self, indent: str = '', **kwargs: Any) -> None:
         super().__init__(indent=indent, **kwargs)
 
     def enter(self) -> str:
         model = self.builder.model
         if model is not None:
-            return f'result: {self.builder.method}{model.__prisma_model__}'
+            model_name = model.__prisma_model__
+        else:
+            model_name = ''
 
-        return f'result: {self.builder.method}'
+        method = self.builder.method_format.format(model=model_name)
+        return f'result: {method}'
 
     def depart(self) -> Optional[str]:
         return None
 
     def create_children(self) -> List[ChildType]:
         return [
             Arguments.create(
@@ -466,19 +534,19 @@
                 continue
 
             if isinstance(value, dict):
                 children.append(
                     Key(arg, node=Data.create(self.builder, data=value))
                 )
             elif isinstance(value, ITERABLES):
-                # NOTE: we have a special case for execute_raw and query_raw
+                # NOTE: we have a special case for execute_raw, query_raw and query_first
                 # here as prisma expects parameters to be passed as a json string
                 # value like "[\"John\",\"123\"]", and we encode twice to ensure
                 # that only the inner quotes are escaped
-                if self.builder.method in {'queryRaw', 'executeRaw'}:
+                if self.builder.method in {'query_raw', 'query_first', 'execute_raw'}:
                     children.append(f'{arg}: {dumps(dumps(value))}')
                 else:
                     children.append(Key(arg, node=ListNode.create(self.builder, data=value)))
             else:
                 children.append(f'{arg}: {dumps(value)}')
 
         return children
@@ -593,29 +661,29 @@
         )
         {
             id
             title
         }
     }
     """
-    model: Optional[Type[PrismaModel]]
-    include: Optional[Dict[str, Any]]
-    root_selection: Optional[List[str]]
+    model: type[PrismaModel] | None
+    include: dict[str, Any] | None
+    root_selection: list[str] | None
 
     __slots__ = (
         'model',
         'include',
         'root_selection',
     )
 
     def __init__(
         self,
-        model: Optional[Type[PrismaModel]] = None,
-        include: Optional[Dict[str, Any]] = None,
-        root_selection: Optional[List[str]] = None,
+        model: type[PrismaModel] | None = None,
+        include: dict[str, Any] | None = None,
+        root_selection: list[str] | None = None,
         **kwargs: Any
     ) -> None:
         super().__init__(**kwargs)
         self.model = model
         self.include = include
         self.root_selection = root_selection
 
@@ -776,8 +844,7 @@
 def dumps(obj: Any, **kwargs: Any) -> str:
     kwargs.setdefault('default', serializer)
     kwargs.setdefault('ensure_ascii', False)
     return json.dumps(obj, **kwargs)
 
 # black does not respect the fmt: off comment without this
 # fmt: on
-
```

### Comparing `prisma-0.8.2/src/prisma/generator/templates/client.py.jinja` & `prisma-0.9.0/src/prisma/generator/templates/client.py.jinja`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 {% set annotations = true %}
 {% include '_header.py.jinja' %}
-{% from '_utils.py.jinja' import is_async, maybe_async_def, maybe_await, methods, operations, recursive_types, active_provider with context %}
+{% from '_utils.py.jinja' import is_async, maybe_async_def, maybe_await, maybe_async, recursive_types, active_provider with context %}
 # -- template client.py.jinja --
+import warnings
+import logging
 from pathlib import Path
 from types import TracebackType
 
+from pydantic import BaseModel
+
 from . import types, models, errors, actions
 from .types import DatasourceOverride, HttpConfig
-from ._types import BaseModelT
+from ._types import BaseModelT, PrismaMethod
 from .bases import _PrismaModel
-from .engine import AbstractEngine, QueryEngine
-from .builder import QueryBuilder
+from .engine import AbstractEngine, QueryEngine, TransactionId
+from .builder import QueryBuilder, dumps
 from .generator.models import EngineType, OptionalValueFromEnvVar, BinaryPaths
 from ._compat import removeprefix
 from ._raw_query import deserialize_raw_results
 
 __all__ = (
     'ENGINE_TYPE',
     'SCHEMA_PATH',
@@ -23,14 +27,16 @@
     'Prisma',
     'Client',
     'load_env',
     'register',
     'get_client',
 )
 
+log: logging.Logger = logging.getLogger(__name__)
+
 SCHEMA_PATH = Path('{{ schema_path.as_posix() }}')
 PACKAGED_SCHEMA_PATH = Path(__file__).parent.joinpath('schema.prisma')
 ENGINE_TYPE: EngineType = EngineType.{{ generator.config.engine_type }}
 BINARY_PATHS = BinaryPaths.parse_obj({{ binary_paths.dict(by_alias=True) }})
 
 RegisteredClient = Union['Prisma', Callable[[], 'Prisma']]
 _registered_client: Optional[RegisteredClient] = None
@@ -119,19 +125,21 @@
     {% endfor %}
 
     __slots__ = (
         {% for model in dmmf.datamodel.models %}
         '{{ model.name.lower() }}',
         {% endfor %}
         '__engine',
-        '_active_provider',
-        '_log_queries',
+        '__copied',
+        '_tx_id',
         '_datasource',
-        '_connect_timeout',
+        '_log_queries',
         '_http_config',
+        '_connect_timeout',
+        '_active_provider',
     )
 
     def __init__(
         self,
         *,
         use_dotenv: bool = True,
         log_queries: bool = False,
@@ -139,32 +147,42 @@
         datasource: Optional[DatasourceOverride] = None,
         connect_timeout: int = 10,
         http: Optional[HttpConfig] = None,
     ) -> None:
         {% for model in dmmf.datamodel.models %}
         self.{{ model.name.lower() }} = actions.{{ model.name }}Actions[models.{{ model.name }}](self, models.{{ model.name }})
         {% endfor %}
+
+        # NOTE: if you add any more properties here then you may also need to forward
+        # them in the `_copy()` method.
         self.__engine: Optional[AbstractEngine] = None
         self._active_provider = '{{ active_provider }}'
         self._log_queries = log_queries
         self._datasource = datasource
         self._connect_timeout = connect_timeout
         self._http_config: HttpConfig = http or {}
+        self._tx_id: Optional[TransactionId] = None
+        self.__copied: bool = False
 
         if use_dotenv:
             load_env()
 
         if auto_register:
             register(self)
 
     def __del__(self) -> None:
-        if self.__engine is not None:
-            self.__engine.stop()
+        # Note: as the transaction manager holds a reference to the original
+        # client as well as the transaction client the original client cannot
+        # be `free`d before the transaction is finished. So stopping the engine
+        # here should be safe.
+        if self.__engine is not None and not self.__copied:
+            log.debug('unclosed client - stopping engine')
+            engine = self.__engine
             self.__engine = None
-
+            engine.stop()
 
     {% if is_async %}
     async def __aenter__(self) -> 'Prisma':
         await self.connect()
         return self
 
     async def __aexit__(
@@ -224,31 +242,32 @@
             timeout=timeout,
             datasources=datasources,
         )
 
     {{ maybe_async_def }}disconnect(self, timeout: Optional[float] = None) -> None:
         """Disconnect the Prisma query engine."""
         if self.__engine is not None:
+            engine = self.__engine
+            self.__engine = None
             {% if is_async %}
-            {{ maybe_await }}self.__engine.aclose(timeout=timeout)
+            await engine.aclose(timeout=timeout)
             {% else %}
-            self.__engine.close(timeout=timeout)
+            engine.close(timeout=timeout)
             {% endif %}
-            self.__engine.stop(timeout=timeout)
-            self.__engine = None
+            engine.stop(timeout=timeout)
 
     {% if active_provider != 'mongodb' %}
     {{ maybe_async_def }}execute_raw(self, query: LiteralString, *args: Any) -> int:
         resp = {{ maybe_await }}self._execute(
-            operation='{{ operations.execute_raw }}',
-            method='{{ methods.execute_raw }}',
+            method='execute_raw',
             arguments={
                 'query': query,
                 'parameters': args,
-            }
+            },
+            model=None,
         )
         return int(resp['data']['result'])
 
     @overload
     {{ maybe_async_def }}query_first(
         self,
         query: LiteralString,
@@ -312,49 +331,95 @@
     ) -> Union[List[BaseModelT], List[dict[str, Any]]]:
         """Execute a raw SQL query against the database.
 
         If model is given, each returned record is converted to the pydantic model first,
         otherwise results will be raw dictionaries.
         """
         resp = {{ maybe_await }}self._execute(
-            operation='{{ operations.query_raw }}',
-            method='{{ methods.query_raw }}',
+            method='query_raw',
             arguments={
                 'query': query,
                 'parameters': args,
-            }
+            },
+            model=model,
         )
         result = resp['data']['result']
         if model is not None:
             return deserialize_raw_results(result, model=model)
 
         return deserialize_raw_results(result)
     {% endif %}
 
     def batch_(self) -> 'Batch':
         """Returns a context manager for grouping write queries into a single transaction."""
         return Batch(client=self)
 
+    def tx(self, *, max_wait: int = 2000, timeout: int = 5000) -> 'TransactionManager':
+        """Returns a context manager for executing queries within a database transaction.
+
+        Entering the context manager returns a new Prisma instance wrapping all
+        actions within a transaction, queries will be isolated to the Prisma instance and
+        will not be commited to the database until the context manager exits.
+
+        By default, Prisma will wait a maximum of 2 seconds to acquire a transaction from the database. You can modify this
+        defualt with the `max_wait` argument which accepts a value in milliseconds.
+
+        By default, Prisma will cancel and rollback ay transactions that last longer than 5 seconds. You can modify this timeout
+        with the `timeout` argument which accepts a value in milliseconds.
+
+        Example usage:
+
+        ```py
+        {{ maybe_async }}with client.tx() as transaction:
+            user1 = {{ maybe_await }}client.user.create({'name': 'Robert'})
+            user2 = {{ maybe_await }}client.user.create({'name': 'Tegan'})
+        ```
+
+        In the above example, if the first database call succeeds but the second does not then neither of the records will be created.
+        """
+        return TransactionManager(client=self, max_wait=max_wait, timeout=timeout)
+
+    def is_transaction(self) -> bool:
+        """Returns True if the client is wrapped within a transaction"""
+        return self._tx_id is not None
+
     # TODO: don't return Any
     {{ maybe_async_def }}_execute(
         self,
-        method: str,
-        operation: str,
-        arguments: Dict[str, Any],
-        model: Optional[Type['_PrismaModel']] = None,
-        root_selection: Optional[List[str]] = None
+        method: PrismaMethod,
+        arguments: dict[str, Any],
+        model: type[BaseModel] | None = None,
+        root_selection: list[str] | None = None
     ) -> Any:
         builder = QueryBuilder(
-            operation=operation,
             method=method,
             model=model,
             arguments=arguments,
             root_selection=root_selection,
         )
-        return {{ maybe_await }}self._engine.query(builder.build())
+        return {{ maybe_await }}self._engine.query(builder.build(), tx_id=self._tx_id)
+
+    def _copy(self) -> 'Prisma':
+        """Return a new Prisma instance using the same engine process (if connected).
+
+        This is only intended for private usage, there are no guarantees around this API.
+        """
+        new = Prisma(
+            use_dotenv=False,
+            http=self._http_config,
+            datasource=self._datasource,
+            log_queries=self._log_queries,
+            connect_timeout=self._connect_timeout,
+        )
+        new.__copied = True
+
+        if self.__engine is not None:
+            new._engine = self.__engine
+
+        return new
 
     def _create_engine(self, dml_path: Path = PACKAGED_SCHEMA_PATH) -> AbstractEngine:
         if ENGINE_TYPE == EngineType.binary:
             return QueryEngine(dml_path=dml_path, log_queries=self._log_queries, **self._http_config)
 
         raise NotImplementedError(f'Unsupported engine type: {ENGINE_TYPE}')
 
@@ -368,14 +433,18 @@
     @property
     def _engine(self) -> AbstractEngine:
         engine = self.__engine
         if engine is None:
             raise errors.ClientNotConnectedError()
         return engine
 
+    @_engine.setter
+    def _engine(self, engine: AbstractEngine) -> None:
+        self.__engine = engine
+
     def _make_sqlite_datasource(self) -> DatasourceOverride:
         return {
             'name': '{{ datasources[0].name }}',
             'url': self._make_sqlite_url(self._default_datasource['url']),
         }
 
     def _make_sqlite_url(self, url: str, *, relative_to: Path = SCHEMA_PATH.parent) -> str:
@@ -392,14 +461,116 @@
     def _default_datasource(self) -> DatasourceOverride:
         return {
             'name': '{{ datasources[0].name }}',
             'url': OptionalValueFromEnvVar(**{{ datasources[0].url.dict(by_alias=True) }}).resolve(),
         }
 
 
+class TransactionManager:
+    """Context manager for wrapping a Prisma instance within a transaction.
+
+    This should never be created manually, instead it should be used
+    through the Prisma.tx() method.
+    """
+
+    def __init__(self, *, client: Prisma, max_wait: int, timeout: int) -> None:
+        self.__client = client
+        self._max_wait = max_wait
+        self._timeout = timeout
+        self._tx_id: Optional[TransactionId] = None
+
+    {{ maybe_async_def }}start(self, *, _from_context: bool = False) -> Prisma:
+        """Start the transaction and return the wrapped Prisma instance"""
+        if self.__client.is_transaction():
+            # if we were called from the context manager then the stacklevel
+            # needs to be one higher to warn on the actual offending code
+            warnings.warn(
+                'The current client is already in a transaction. This can lead to surprising behaviour.',
+                UserWarning,
+                stacklevel=3 if _from_context else 2
+            )
+
+        tx_id = {{ maybe_await }}self.__client._engine.start_transaction(
+            content=dumps(
+                {
+                    'timeout': self._timeout,
+                    'max_wait': self._max_wait,
+                }
+            ),
+        )
+        self._tx_id = tx_id
+        client = self.__client._copy()
+        client._tx_id = tx_id
+        return client
+
+    {{ maybe_async_def }}commit(self) -> None:
+        """Commit the transaction to the database, this transaction will no longer be usable"""
+        if self._tx_id is None:
+            raise errors.TransactionNotStartedError()
+
+        {{ maybe_await }}self.__client._engine.commit_transaction(self._tx_id)
+
+    {{ maybe_async_def }}rollback(self) -> None:
+        """Do not commit the changes to the database, this transaction will no longer be usable"""
+        if self._tx_id is None:
+            raise errors.TransactionNotStartedError()
+
+        {{ maybe_await }}self.__client._engine.rollback_transaction(self._tx_id)
+
+    {% if is_async %}
+    async def __aenter__(self) -> Prisma:
+        return await self.start(_from_context=True)
+
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc: Optional[BaseException],
+        exc_tb: Optional[TracebackType],
+    ) -> None:
+        if exc is None:
+            log.debug('Transaction exited with no exception - commiting')
+            await self.commit()
+            return
+
+        log.debug('Transaction exited with exc type: %s - rolling back', exc_type)
+
+        try:
+            await self.rollback()
+        except Exception as exc:
+            log.warning(
+                'Encountered exc `%s` while rolling back a transaction. Ignoring and raising original exception',
+                exc
+            )
+    {% else %}
+    def __enter__(self) -> Prisma:
+        return self.start(_from_context=True)
+
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc: Optional[BaseException],
+        exc_tb: Optional[TracebackType],
+    ) -> None:
+        if exc is None:
+            log.debug('Transaction exited with no exception - commiting')
+            self.commit()
+            return
+
+        log.debug('Transaction exited with exc type: %s - rolling back', exc_type)
+
+        try:
+            self.rollback()
+        except Exception as exc:
+            log.warning(
+                'Encountered exc `%s` while rolling back a transaction. Ignoring and raising original exception',
+                exc
+            )
+    {% endif %}
+
+
 # TODO: this should return the results as well
 # TODO: don't require copy-pasting arguments between actions and batch actions
 class Batch:
     {% for model in dmmf.datamodel.models %}
     {{ model.name.lower() }}: '{{ model.name }}BatchActions'
     {% endfor %}
 
@@ -414,36 +585,36 @@
     def _add(self, **kwargs: Any) -> None:
         builder = QueryBuilder(**kwargs)
         self.__queries.append(builder.build_query())
 
     {{ maybe_async_def }}commit(self) -> None:
         """Execute the queries"""
         # TODO: normalise this, we should still call client._execute
-        from .builder import dumps
-
         queries = self.__queries
         self.__queries = []
 
         payload = {
             'batch': [
                 {
                     'query': query,
                     'variables': {},
                 }
                 for query in queries
             ],
             'transaction': True,
         }
-        {{ maybe_await }}self.__client._engine.query(dumps(payload))
+        {{ maybe_await }}self.__client._engine.query(
+            dumps(payload),
+            tx_id=self.__client._tx_id,
+        )
 
     {% if active_provider != 'mongodb' %}
     def execute_raw(self, query: LiteralString, *args: Any) -> None:
         self._add(
-            operation='{{ operations.execute_raw }}',
-            method='{{ methods.execute_raw }}',
+            method='execute_raw',
             arguments={
                 'query': query,
                 'parameters': args,
             }
         )
     {% endif %}
 
@@ -483,16 +654,15 @@
 
     def create(
         self,
         data: types.{{ model.name }}CreateInput,
         include: Optional[types.{{ model.name}}Include] = None
     ) -> None:
         self._batcher._add(
-            operation='{{ operations.create }}',
-            method='{{ methods.create }}',
+            method='create',
             model=models.{{ model.name }},
             arguments={
                 'data': data,
                 'include': include,
             },
         )
 
@@ -502,48 +672,45 @@
         *,
         skip_duplicates: Optional[bool] = None,
     ) -> None:
         if self._batcher._active_provider == 'sqlite':
             raise errors.UnsupportedDatabaseError('sqlite', 'create_many()')
 
         self._batcher._add(
-            operation='{{ operations.create_many }}',
-            method='{{ methods.create_many }}',
+            method='create_many',
             model=models.{{ model.name }},
             arguments={
                 'data': data,
                 'skipDuplicates': skip_duplicates,
             },
             root_selection=['count'],
         )
 
     def delete(
         self,
         where: types.{{ model.name }}WhereUniqueInput,
         include: Optional[types.{{ model.name}}Include] = None,
     ) -> None:
         self._batcher._add(
-            operation='{{ operations.delete }}',
-            method='{{ methods.delete }}',
+            method='delete',
             model=models.{{ model.name }},
             arguments={
                 'where': where,
                 'include': include,
             },
         )
 
     def update(
         self,
         data: types.{{ model.name }}UpdateInput,
         where: types.{{ model.name }}WhereUniqueInput,
         include: Optional[types.{{ model.name}}Include] = None
     ) -> None:
         self._batcher._add(
-            operation='{{ operations["update"] }}',
-            method='{{ methods["update"] }}',
+            method='update',
             model=models.{{ model.name }},
             arguments={
                 'data': data,
                 'where': where,
                 'include': include,
             },
         )
@@ -551,16 +718,15 @@
     def upsert(
         self,
         where: types.{{ model.name }}WhereUniqueInput,
         data: types.{{ model.name }}UpsertInput,
         include: Optional[types.{{ model.name}}Include] = None,
     ) -> None:
         self._batcher._add(
-            operation='{{ operations.upsert }}',
-            method='{{ methods.upsert }}',
+            method='upsert',
             model=models.{{ model.name }},
             arguments={
                 'where': where,
                 'include': include,
                 'create': data.get('create'),
                 'update': data.get('update'),
             },
@@ -568,28 +734,26 @@
 
     def update_many(
         self,
         data: types.{{ model.name }}UpdateManyMutationInput,
         where: types.{{ model.name }}WhereInput,
     ) -> None:
         self._batcher._add(
-            operation='{{ operations.update_many }}',
-            method='{{ methods.update_many }}',
+            method='update_many',
             model=models.{{ model.name }},
             arguments={'data': data, 'where': where,},
             root_selection=['count'],
         )
 
     def delete_many(
         self,
         where: Optional[types.{{ model.name }}WhereInput] = None,
     ) -> None:
         self._batcher._add(
-            operation='{{ operations.delete_many }}',
-            method='{{ methods.delete_many }}',
+            method='delete_many',
             model=models.{{ model.name }},
             arguments={'where': where},
             root_selection=['count'],
         )
 
 
 {% endfor %}
```

### Comparing `prisma-0.8.2/src/prisma/generator/templates/engine/http.py.jinja` & `prisma-0.9.0/src/prisma/generator/templates/engine/http.py.jinja`

 * *Files 12% similar despite different names*

```diff
@@ -25,58 +25,69 @@
 
     def __init__(
         self,
         url: Optional[str],
         headers: Optional[Dict[str, str]] = None,
         **kwargs: Any,
     ) -> None:
+        super().__init__()
         self.url = url
         self.session = HTTP(**kwargs)
         self.headers = headers if headers is not None else {}
 
-    def __del__(self) -> None:
-        self.stop()
-
     {% if is_async %}
     def close(self, *, timeout: Optional[float] = None) -> None:
         pass
 
     async def aclose(self, *, timeout: Optional[float] = None) -> None:
         await self._close_session()
     {% else %}
-    def close(self) -> None:
+    def close(self, *, timeout: Optional[float] = None) -> None:
         self._close_session()
 
-    async def aclose(self) -> None:
+    async def aclose(self, *, timeout: Optional[float] = None) -> None:
         pass
     {% endif %}
 
     {{ maybe_async_def }}_close_session(self) -> None:
         if self.session and not self.session.closed:
             {{ maybe_await }}self.session.close()
 
-    {{ maybe_async_def }}request(self, method: Method, path: str, *, content: Any = None) -> Any:
+    {{ maybe_async_def }}request(
+        self,
+        method: Method,
+        path: str,
+        *,
+        content: Any = None,
+        headers: Optional[Dict[str, str]] = None,
+    ) -> Any:
         if self.url is None:
             raise errors.NotConnectedError('Not connected to the query engine')
 
         kwargs = {
             'headers': {
                 'Content-Type': 'application/json',
                 'Accept': 'application/json',
                 **self.headers,
             }
         }
 
+        if headers is not None:
+            kwargs['headers'].update(headers)
+
         if content is not None:
             kwargs['content'] = content
 
         url = self.url + path
-        log.debug('Sending %s request to %s with content: %s', method, url, content)
+        log.debug('Sending %s request to %s', method, url)
+        log.debug('Request headers: %s', kwargs['headers'])
+        log.debug('Request content: %s', content)
 
         resp = {{ maybe_await }}self.session.request(method, url, **kwargs)
+        log.debug('%s %s returned status %s', method, url, resp.status)
 
         if 300 > resp.status >= 200:
             response = {{ maybe_await }}resp.json()
             log.debug('%s %s returned %s', method, url, response)
 
             errors_data = response.get('errors')
             if errors_data:
```

### Comparing `prisma-0.8.2/src/prisma/generator/templates/engine/query.py.jinja` & `prisma-0.9.0/src/prisma/generator/templates/engine/query.py.jinja`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .http import HTTPEngine
 from .. import config
 from ..utils import DEBUG
 from ..binaries import platform
 from ..utils import time_since, _env_bool
 from ..types import DatasourceOverride
 from ..builder import dumps
+from ._types import TransactionId
 
 
 __all__ = ('QueryEngine',)
 
 log: logging.Logger = logging.getLogger(__name__)
 
 
@@ -39,17 +40,14 @@
         self._log_queries = log_queries
         self.process = None
         self.file = None
 
         # ensure the query engine process is terminated when we are
         atexit.register(self.stop)
 
-    def __del__(self) -> None:
-        self.stop()
-
     def close(self, *, timeout: Optional[float] = None) -> None:
         log.debug('Disconnecting query engine...')
 
         if self.process is not None:
             if platform.name() == 'windows':
                 self.process.kill()
                 self.process.wait(timeout=timeout)
@@ -174,14 +172,45 @@
 
             break
         else:
             raise errors.EngineConnectionError(
                 'Could not connect to the query engine'
             ) from last_exc
 
-    {{ maybe_async_def }}query(self, content: str) -> Any:
-        return {{ maybe_await }}self.request('POST', '/', content=content)
+    {{ maybe_async_def }}query(
+        self,
+        content: str,
+        *,
+        tx_id: TransactionId | None,
+    ) -> Any:
+        headers: Dict[str, str] = {}
+        if tx_id is not None:
+            headers['X-transaction-id'] = tx_id
+
+        return {{ maybe_await }}self.request(
+            'POST',
+            '/',
+            content=content,
+            headers=headers,
+        )
+
+    {{ maybe_async_def }}start_transaction(self, *, content: str) -> TransactionId:
+        result = {{ maybe_await }}self.request(
+            'POST',
+            '/transaction/start',
+            content=content,
+        )
+        return TransactionId(result['id'])
+
+    {{ maybe_async_def }}commit_transaction(self, tx_id: TransactionId) -> None:
+        {{ maybe_await }}self.request(
+            'POST', f'/transaction/{tx_id}/commit'
+        )
 
+    {{ maybe_async_def }}rollback_transaction(self, tx_id: TransactionId) -> None:
+        {{ maybe_await }}self.request(
+            'POST', f'/transaction/{tx_id}/rollback'
+        )
 
 # black does not respect the fmt: off comment without this
 # fmt: on
```

### Comparing `prisma-0.8.2/src/prisma/generator/templates/fields.py.jinja` & `prisma-0.9.0/src/prisma/generator/templates/fields.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/generator/templates/models.py.jinja` & `prisma-0.9.0/src/prisma/generator/templates/models.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/generator/templates/partials.py.jinja` & `prisma-0.9.0/src/prisma/generator/templates/partials.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/generator/templates/types.py.jinja` & `prisma-0.9.0/src/prisma/generator/templates/types.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/generator/utils.py` & `prisma-0.9.0/src/prisma/generator/utils.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/http_abstract.py` & `prisma-0.9.0/src/prisma/http_abstract.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/mypy.py` & `prisma-0.9.0/src/prisma/mypy.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/testing.py` & `prisma-0.9.0/src/prisma/testing.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/utils.py` & `prisma-0.9.0/src/prisma/utils.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma/validator.py` & `prisma-0.9.0/src/prisma/validator.py`

 * *Files identical despite different names*

### Comparing `prisma-0.8.2/src/prisma.egg-info/PKG-INFO` & `prisma-0.9.0/src/prisma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prisma
-Version: 0.8.2
+Version: 0.9.0
 Summary: Prisma Client Python is an auto-generated and fully type-safe database client
 Home-page: https://github.com/RobertCraigie/prisma-client-py
 Author: Robert Craigie
 Author-email: robert@craigie.dev
 Maintainer: Robert Craigie
 License: APACHE
 Project-URL: Documentation, https://prisma-client-py.readthedocs.io
@@ -40,15 +40,15 @@
     <h1>Prisma Client Python</h1>
     <p><h3 align="center">Type-safe database access for Python</h3></p>
     <div align="center">
     <a href="https://discord.gg/HpFaJbepBH">
         <img src="https://img.shields.io/discord/933860922039099444?color=blue&label=chat&logo=discord" alt="Chat on Discord">
     </a>
     <a href="https://prisma.io">
-        <img src="https://img.shields.io/static/v1?label=prisma&message=4.11.0&color=blue&logo=prisma" alt="Supported Prisma version is 4.11.0">
+        <img src="https://img.shields.io/static/v1?label=prisma&message=4.15.0&color=blue&logo=prisma" alt="Supported Prisma version is 4.15.0">
     </a>
     <a href="https://github.com/grantjenks/blue">
         <img src="https://camo.githubusercontent.com/dbdbcf26db37abfa1f2ab7e6c28c8b3a199f2dad98e4ef53a50e9c45c7e4ace8/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c75652d626c75652e737667" alt="Code style: blue">
     </a>
     <a href="https://robertcraigie.github.io/prisma-client-py/htmlcov/index.html">
         <img src="https://raw.githubusercontent.com/RobertCraigie/prisma-client-py/static/coverage/coverage.svg" alt="Code coverage report">
     </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prisma Version: 0.8.2 Summary: Prisma Client Python
+Metadata-Version: 2.1 Name: prisma Version: 0.9.0 Summary: Prisma Client Python
 is an auto-generated and fully type-safe database client Home-page: https://
 github.com/RobertCraigie/prisma-client-py Author: Robert Craigie Author-email:
 robert@craigie.dev Maintainer: Robert Craigie License: APACHE Project-URL:
 Documentation, https://prisma-client-py.readthedocs.io Project-URL: Source,
 https://github.com/RobertCraigie/prisma-client-py Project-URL: Tracker, https:/
 /github.com/RobertCraigie/prisma-client-py/issues Keywords:
 orm,mysql,typing,prisma,sqlite,database,postgresql Platform: UNKNOWN
@@ -17,15 +17,15 @@
 Python :: 3.11 Classifier: Operating System :: POSIX Classifier: Operating
 System :: MacOS Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Requires-Python: >=3.7.0 Description-
 Content-Type: text/markdown Provides-Extra: node Provides-Extra: all License-
 File: LICENSE
                       ****** Prisma Client Python ******
                 **** Type-safe database access for Python ****
-[Chat_on_Discord] [Supported_Prisma_version_is_4.11.0] [Code_style:_blue] [Code
+[Chat_on_Discord] [Supported_Prisma_version_is_4.15.0] [Code_style:_blue] [Code
  coverage_report] [GitHub Workflow Status (main)] [Supported python versions]
                            [Latest package version]
 ===============================================================================
 ## What is Prisma Client Python? Prisma Client Python is a next-generation ORM
 built on top of [Prisma](https://github.com/prisma/prisma) that has been
 designed from the ground up for ease of use and correctness. [Prisma](https://
 www.prisma.io/) is a TypeScript ORM with zero-cost type safety for your
```

### Comparing `prisma-0.8.2/src/prisma.egg-info/SOURCES.txt` & `prisma-0.9.0/src/prisma.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 src/prisma/cli/utils.py
 src/prisma/cli/commands/__init__.py
 src/prisma/cli/commands/dev.py
 src/prisma/cli/commands/fetch.py
 src/prisma/cli/commands/generate.py
 src/prisma/cli/commands/version.py
 src/prisma/engine/__init__.py
+src/prisma/engine/_types.py
 src/prisma/engine/errors.py
 src/prisma/engine/utils.py
 src/prisma/generator/__init__.py
 src/prisma/generator/errors.py
 src/prisma/generator/filters.py
 src/prisma/generator/generator.py
 src/prisma/generator/jsonrpc.py
```

### Comparing `prisma-0.8.2/src/prisma_cleanup/_cleanup.py` & `prisma-0.9.0/src/prisma_cleanup/_cleanup.py`

 * *Files identical despite different names*

