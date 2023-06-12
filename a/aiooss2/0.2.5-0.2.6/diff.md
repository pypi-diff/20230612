# Comparing `tmp/aiooss2-0.2.5.tar.gz` & `tmp/aiooss2-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiooss2-0.2.5.tar", last modified: Mon Apr 17 11:55:08 2023, max compression
+gzip compressed data, was "aiooss2-0.2.6.tar", last modified: Mon Jun 12 11:05:06 2023, max compression
```

## Comparing `aiooss2-0.2.5.tar` & `aiooss2-0.2.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 11:54:45.000000 aiooss2-0.2.5/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-17 11:54:45.000000 aiooss2-0.2.5/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-17 11:54:45.000000 aiooss2-0.2.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-17 11:54:45.000000 aiooss2-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 11:54:45.000000 aiooss2-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-17 11:55:08.979832 aiooss2-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-17 11:54:45.000000 aiooss2-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-17 11:54:45.000000 aiooss2-0.2.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-17 11:54:45.000000 aiooss2-0.2.5/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-17 11:54:45.000000 aiooss2-0.2.5/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 11:54:45.000000 aiooss2-0.2.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-17 11:54:45.000000 aiooss2-0.2.5/examples/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-17 11:54:45.000000 aiooss2-0.2.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-17 11:54:45.000000 aiooss2-0.2.5/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-17 11:54:45.000000 aiooss2-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-17 11:55:08.983832 aiooss2-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.975832 aiooss2-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/src/aiooss2/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29416 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/multipart.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/resumable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/src/aiooss2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-17 11:55:08.000000 aiooss2-0.2.5/src/aiooss2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-17 11:55:08.000000 aiooss2-0.2.5/src/aiooss2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:55:08.000000 aiooss2-0.2.5/src/aiooss2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:55:08.000000 aiooss2-0.2.5/src/aiooss2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-17 11:55:08.000000 aiooss2-0.2.5/src/aiooss2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 11:55:08.000000 aiooss2-0.2.5/src/aiooss2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/tests/func/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/func/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/func/test_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/func/test_resumable.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/test_aiooss2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/unit/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.028393 aiooss2-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.020393 aiooss2-0.2.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-12 11:04:42.000000 aiooss2-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-12 11:04:42.000000 aiooss2-0.2.6/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-12 11:04:42.000000 aiooss2-0.2.6/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-12 11:04:42.000000 aiooss2-0.2.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-12 11:04:42.000000 aiooss2-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 11:04:42.000000 aiooss2-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-12 11:05:06.028393 aiooss2-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-12 11:04:42.000000 aiooss2-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-12 11:04:42.000000 aiooss2-0.2.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-12 11:04:42.000000 aiooss2-0.2.6/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-12 11:04:42.000000 aiooss2-0.2.6/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 11:04:42.000000 aiooss2-0.2.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-12 11:04:42.000000 aiooss2-0.2.6/examples/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-12 11:04:42.000000 aiooss2-0.2.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-12 11:04:42.000000 aiooss2-0.2.6/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-12 11:04:42.000000 aiooss2-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-12 11:05:06.028393 aiooss2-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.020393 aiooss2-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/src/aiooss2/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29416 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/multipart.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/resumable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-12 11:04:42.000000 aiooss2-0.2.6/src/aiooss2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/src/aiooss2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-12 11:05:05.000000 aiooss2-0.2.6/src/aiooss2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-12 11:05:06.000000 aiooss2-0.2.6/src/aiooss2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 11:05:05.000000 aiooss2-0.2.6/src/aiooss2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 11:05:05.000000 aiooss2-0.2.6/src/aiooss2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-12 11:05:05.000000 aiooss2-0.2.6/src/aiooss2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 11:05:05.000000 aiooss2-0.2.6/src/aiooss2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.024393 aiooss2-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.028393 aiooss2-0.2.6/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/func/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/func/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/func/test_resumable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/test_aiooss2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:05:06.028393 aiooss2-0.2.6/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-12 11:04:42.000000 aiooss2-0.2.6/tests/unit/test_adapter.py
```

### Comparing `aiooss2-0.2.5/.cruft.json` & `aiooss2-0.2.6/.cruft.json`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/.github/dependabot.yml` & `aiooss2-0.2.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/.github/workflows/docs.yml` & `aiooss2-0.2.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/.github/workflows/release.yml` & `aiooss2-0.2.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/.github/workflows/tests.yml` & `aiooss2-0.2.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/.gitignore` & `aiooss2-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/.pre-commit-config.yaml` & `aiooss2-0.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/CODE_OF_CONDUCT.rst` & `aiooss2-0.2.6/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/CONTRIBUTING.rst` & `aiooss2-0.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/LICENSE` & `aiooss2-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/PKG-INFO` & `aiooss2-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiooss2
-Version: 0.2.5
+Version: 0.2.6
 Summary: Async client for aliyun OSS(Object Storage Service) using oss2 and aiohttp/asyncio
 Home-page: https://github.com/karajan1001/aiooss2
 Maintainer-email: mishanyo1001@gmail.com
 License: Apache-2.0
 Keywords: "oss,aio"
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiooss2-0.2.5/README.md` & `aiooss2-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/README.rst` & `aiooss2-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/docs/assets/logo.svg` & `aiooss2-0.2.6/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/docs/gen_ref_pages.py` & `aiooss2-0.2.6/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/examples/simple.py` & `aiooss2-0.2.6/examples/simple.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/mkdocs.yml` & `aiooss2-0.2.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/noxfile.py` & `aiooss2-0.2.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/pyproject.toml` & `aiooss2-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/setup.cfg` & `aiooss2-0.2.6/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 zip_safe = False
 packages = find:
 package_dir = 
 	=src
 include_package_data = True
 install_requires = 
 	aiohttp==3.8.4
-	oss2==2.17.0
+	oss2==2.18.0
 
 [options.extras_require]
 docs = 
 	mkdocs==1.3.1
 	mkdocs-gen-files==0.3.5
 	mkdocs-material==8.4.1
 	mkdocs-section-index==0.3.4
@@ -43,15 +43,15 @@
 	pytest-mock==3.8.2
 	pylint==2.15.0
 	pylint-pytest==1.1.2
 	mypy==0.971
 dev = 
 	%(tests)s
 	%(docs)s
-	nox==2022.11.21
+	nox==2023.4.22
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
 where = src
```

### Comparing `aiooss2-0.2.5/src/aiooss2/adapter.py` & `aiooss2-0.2.6/src/aiooss2/adapter.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/src/aiooss2/api.py` & `aiooss2-0.2.6/src/aiooss2/api.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/src/aiooss2/exceptions.py` & `aiooss2-0.2.6/src/aiooss2/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/src/aiooss2/http.py` & `aiooss2-0.2.6/src/aiooss2/http.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/src/aiooss2/iterators.py` & `aiooss2-0.2.6/src/aiooss2/iterators.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/src/aiooss2/models.py` & `aiooss2-0.2.6/src/aiooss2/models.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/src/aiooss2/multipart.py` & `aiooss2-0.2.6/src/aiooss2/multipart.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/src/aiooss2/resumable.py` & `aiooss2-0.2.6/src/aiooss2/resumable.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/src/aiooss2/utils.py` & `aiooss2-0.2.6/src/aiooss2/utils.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/src/aiooss2.egg-info/PKG-INFO` & `aiooss2-0.2.6/src/aiooss2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiooss2
-Version: 0.2.5
+Version: 0.2.6
 Summary: Async client for aliyun OSS(Object Storage Service) using oss2 and aiohttp/asyncio
 Home-page: https://github.com/karajan1001/aiooss2
 Maintainer-email: mishanyo1001@gmail.com
 License: Apache-2.0
 Keywords: "oss,aio"
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiooss2-0.2.5/src/aiooss2.egg-info/SOURCES.txt` & `aiooss2-0.2.6/src/aiooss2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/src/aiooss2.egg-info/requires.txt` & `aiooss2-0.2.6/src/aiooss2.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 aiohttp==3.8.4
-oss2==2.17.0
+oss2==2.18.0
 
 [dev]
 pytest==7.2.0
 pytest-sugar==0.9.5
 pytest-cov==3.0.0
 pytest-mock==3.8.2
 pylint==2.15.0
 pylint-pytest==1.1.2
 mypy==0.971
 mkdocs==1.3.1
 mkdocs-gen-files==0.3.5
 mkdocs-material==8.4.1
 mkdocs-section-index==0.3.4
 mkdocstrings-python==0.7.1
-nox==2022.11.21
+nox==2023.4.22
 
 [docs]
 mkdocs==1.3.1
 mkdocs-gen-files==0.3.5
 mkdocs-material==8.4.1
 mkdocs-section-index==0.3.4
 mkdocstrings-python==0.7.1
```

### Comparing `aiooss2-0.2.5/tests/conftest.py` & `aiooss2-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/tests/func/test_bucket.py` & `aiooss2-0.2.6/tests/func/test_bucket.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/tests/func/test_object.py` & `aiooss2-0.2.6/tests/func/test_object.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/tests/func/test_resumable.py` & `aiooss2-0.2.6/tests/func/test_resumable.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.5/tests/unit/test_adapter.py` & `aiooss2-0.2.6/tests/unit/test_adapter.py`

 * *Files identical despite different names*

