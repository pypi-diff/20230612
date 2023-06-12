# Comparing `tmp/datalookup-1.0.0rc1.tar.gz` & `tmp/datalookup-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalookup-1.0.0rc1.tar", last modified: Fri Jun  9 20:48:17 2023, max compression
+gzip compressed data, was "datalookup-1.0.0rc3.tar", last modified: Mon Jun 12 13:08:39 2023, max compression
```

## Comparing `datalookup-1.0.0rc1.tar` & `datalookup-1.0.0rc3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 20:48:17.429335 datalookup-1.0.0rc1/
--rw-rw-rw-   0        0        0      106 2023-06-09 08:05:43.000000 datalookup-1.0.0rc1/.coveragerc
-drwxrwxrwx   0        0        0        0 2023-06-09 20:48:17.131336 datalookup-1.0.0rc1/.github/
-drwxrwxrwx   0        0        0        0 2023-06-09 20:48:17.241837 datalookup-1.0.0rc1/.github/workflows/
--rw-rw-rw-   0        0        0     1079 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/.github/workflows/coverage.yml
--rw-rw-rw-   0        0        0      747 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/.github/workflows/docs.yml
--rw-rw-rw-   0        0        0     1110 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/.github/workflows/linters.yml
--rw-rw-rw-   0        0        0      959 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/.github/workflows/tests.yml
--rw-rw-rw-   0        0        0      987 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/.gitignore
--rw-rw-rw-   0        0        0      709 2023-03-14 20:24:24.000000 datalookup-1.0.0rc1/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      383 2023-06-09 20:02:09.000000 datalookup-1.0.0rc1/.readthedocs.yml
--rw-rw-rw-   0        0        0      127 2023-06-05 15:31:40.000000 datalookup-1.0.0rc1/AUTHORS
--rw-rw-rw-   0        0        0     5352 2023-03-05 10:52:09.000000 datalookup-1.0.0rc1/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     9257 2023-06-06 15:59:32.000000 datalookup-1.0.0rc1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1091 2023-06-04 19:25:49.000000 datalookup-1.0.0rc1/LICENCE
--rw-rw-rw-   0        0        0    10001 2023-06-09 20:48:17.426337 datalookup-1.0.0rc1/PKG-INFO
--rw-rw-rw-   0        0        0     8765 2023-06-09 20:36:23.000000 datalookup-1.0.0rc1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-09 20:48:17.270337 datalookup-1.0.0rc1/datalookup/
--rw-rw-rw-   0        0        0    16179 2023-06-09 10:34:07.000000 datalookup-1.0.0rc1/datalookup/__init__.py
--rw-rw-rw-   0        0        0      167 2023-06-09 20:48:16.000000 datalookup-1.0.0rc1/datalookup/_version.py
--rw-rw-rw-   0        0        0      500 2023-06-09 07:34:13.000000 datalookup-1.0.0rc1/datalookup/exceptions.py
--rw-rw-rw-   0        0        0     5638 2023-06-08 19:20:21.000000 datalookup-1.0.0rc1/datalookup/fields.py
--rw-rw-rw-   0        0        0     8265 2023-06-08 19:39:46.000000 datalookup-1.0.0rc1/datalookup/lookup.py
--rw-rw-rw-   0        0        0     2106 2023-06-09 08:05:56.000000 datalookup-1.0.0rc1/datalookup/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 20:48:17.289836 datalookup-1.0.0rc1/datalookup.egg-info/
--rw-rw-rw-   0        0        0    10001 2023-06-09 20:48:16.000000 datalookup-1.0.0rc1/datalookup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1062 2023-06-09 20:48:17.000000 datalookup-1.0.0rc1/datalookup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 20:48:16.000000 datalookup-1.0.0rc1/datalookup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-09 20:48:16.000000 datalookup-1.0.0rc1/datalookup.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 20:48:17.348835 datalookup-1.0.0rc1/docs/
--rw-rw-rw-   0        0        0      654 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-06-09 20:48:17.353336 datalookup-1.0.0rc1/docs/_ext/
--rw-rw-rw-   0        0        0      205 2023-06-08 17:25:06.000000 datalookup-1.0.0rc1/docs/_ext/datalookup_docs.py
--rw-rw-rw-   0        0        0     3861 2023-06-09 07:24:11.000000 datalookup-1.0.0rc1/docs/conf.py
--rw-rw-rw-   0        0        0      307 2023-06-06 16:38:28.000000 datalookup-1.0.0rc1/docs/contents.rst
--rw-rw-rw-   0        0        0    15980 2023-06-09 20:02:09.000000 datalookup-1.0.0rc1/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-06-09 20:48:17.378836 datalookup-1.0.0rc1/docs/internals/
--rw-rw-rw-   0        0        0      443 2023-06-06 15:59:32.000000 datalookup-1.0.0rc1/docs/internals/changelog.rst
--rw-rw-rw-   0        0        0     2905 2023-06-06 15:59:32.000000 datalookup-1.0.0rc1/docs/internals/coding-style.rst
--rw-rw-rw-   0        0        0       58 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/docs/internals/contributing.rst
--rw-rw-rw-   0        0        0      449 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/docs/internals/deprecations.rst
--rw-rw-rw-   0        0        0      307 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/docs/internals/index.rst
--rw-rw-rw-   0        0        0     2395 2023-06-06 15:59:32.000000 datalookup-1.0.0rc1/docs/internals/release-process.rst
--rwxrwxrwx   0        0        0      800 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/docs/make.bat
--rw-rw-rw-   0        0        0       63 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/docs/requirements.txt
--rw-rw-rw-   0        0        0      202 2023-06-08 17:25:06.000000 datalookup-1.0.0rc1/docs/spelling_wordlist
-drwxrwxrwx   0        0        0        0 2023-06-09 20:48:17.383834 datalookup-1.0.0rc1/licenses/
--rw-rw-rw-   0        0        0     1579 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/licenses/django.license
--rw-rw-rw-   0        0        0     1497 2023-06-06 15:59:32.000000 datalookup-1.0.0rc1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 20:48:17.429836 datalookup-1.0.0rc1/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-06-05 15:31:49.000000 datalookup-1.0.0rc1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 20:48:17.405836 datalookup-1.0.0rc1/tests/
--rw-rw-rw-   0        0        0      439 2023-06-09 10:37:27.000000 datalookup-1.0.0rc1/tests/README.rst
--rw-rw-rw-   0        0        0        0 2022-04-23 14:09:47.000000 datalookup-1.0.0rc1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 20:48:17.418835 datalookup-1.0.0rc1/tests/data/
--rw-rw-rw-   0        0        0      956 2023-05-29 16:14:03.000000 datalookup-1.0.0rc1/tests/data/books.json
--rw-rw-rw-   0        0        0     1652 2023-05-30 19:23:32.000000 datalookup-1.0.0rc1/tests/data/recipe.json
--rw-rw-rw-   0        0        0      231 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/tests/lookup.py
--rw-rw-rw-   0        0        0       77 2023-05-11 15:53:03.000000 datalookup-1.0.0rc1/tests/pytest.ini
--rw-rw-rw-   0        0        0       62 2023-06-06 15:59:32.000000 datalookup-1.0.0rc1/tests/requirements.txt
--rw-rw-rw-   0        0        0    23841 2023-06-09 10:34:07.000000 datalookup-1.0.0rc1/tests/tests.py
--rw-rw-rw-   0        0        0     1406 2023-06-05 15:25:48.000000 datalookup-1.0.0rc1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.201708 datalookup-1.0.0rc3/
+-rw-rw-rw-   0        0        0      106 2023-06-09 08:05:43.000000 datalookup-1.0.0rc3/.coveragerc
+drwxrwxrwx   0        0        0        0 2023-06-12 13:08:38.887206 datalookup-1.0.0rc3/.github/
+drwxrwxrwx   0        0        0        0 2023-06-12 13:08:38.997206 datalookup-1.0.0rc3/.github/workflows/
+-rw-rw-rw-   0        0        0     1079 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/.github/workflows/coverage.yml
+-rw-rw-rw-   0        0        0      747 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/.github/workflows/docs.yml
+-rw-rw-rw-   0        0        0     1110 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/.github/workflows/linters.yml
+-rw-rw-rw-   0        0        0      959 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/.github/workflows/tests.yml
+-rw-rw-rw-   0        0        0      987 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/.gitignore
+-rw-rw-rw-   0        0        0      709 2023-03-14 20:24:24.000000 datalookup-1.0.0rc3/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      383 2023-06-09 20:02:09.000000 datalookup-1.0.0rc3/.readthedocs.yml
+-rw-rw-rw-   0        0        0      127 2023-06-05 15:31:40.000000 datalookup-1.0.0rc3/AUTHORS
+-rw-rw-rw-   0        0        0     5352 2023-03-05 10:52:09.000000 datalookup-1.0.0rc3/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     9257 2023-06-06 15:59:32.000000 datalookup-1.0.0rc3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1091 2023-06-04 19:25:49.000000 datalookup-1.0.0rc3/LICENCE
+-rw-rw-rw-   0        0        0    12690 2023-06-12 13:08:39.196705 datalookup-1.0.0rc3/PKG-INFO
+-rw-rw-rw-   0        0        0    11454 2023-06-12 07:25:37.000000 datalookup-1.0.0rc3/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.026207 datalookup-1.0.0rc3/datalookup/
+-rw-rw-rw-   0        0        0    16179 2023-06-09 10:34:07.000000 datalookup-1.0.0rc3/datalookup/__init__.py
+-rw-rw-rw-   0        0        0      167 2023-06-12 13:08:38.000000 datalookup-1.0.0rc3/datalookup/_version.py
+-rw-rw-rw-   0        0        0      500 2023-06-09 07:34:13.000000 datalookup-1.0.0rc3/datalookup/exceptions.py
+-rw-rw-rw-   0        0        0     5638 2023-06-08 19:20:21.000000 datalookup-1.0.0rc3/datalookup/fields.py
+-rw-rw-rw-   0        0        0     8265 2023-06-08 19:39:46.000000 datalookup-1.0.0rc3/datalookup/lookup.py
+-rw-rw-rw-   0        0        0     2106 2023-06-09 08:05:56.000000 datalookup-1.0.0rc3/datalookup/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.048205 datalookup-1.0.0rc3/datalookup.egg-info/
+-rw-rw-rw-   0        0        0    12690 2023-06-12 13:08:38.000000 datalookup-1.0.0rc3/datalookup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1051 2023-06-12 13:08:38.000000 datalookup-1.0.0rc3/datalookup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 13:08:38.000000 datalookup-1.0.0rc3/datalookup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 13:08:38.000000 datalookup-1.0.0rc3/datalookup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.109205 datalookup-1.0.0rc3/docs/
+-rw-rw-rw-   0        0        0      654 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.113707 datalookup-1.0.0rc3/docs/_ext/
+-rw-rw-rw-   0        0        0      205 2023-06-08 17:25:06.000000 datalookup-1.0.0rc3/docs/_ext/datalookup_docs.py
+-rw-rw-rw-   0        0        0     3861 2023-06-09 07:24:11.000000 datalookup-1.0.0rc3/docs/conf.py
+-rw-rw-rw-   0        0        0      307 2023-06-06 16:38:28.000000 datalookup-1.0.0rc3/docs/contents.rst
+-rw-rw-rw-   0        0        0    15980 2023-06-09 20:02:09.000000 datalookup-1.0.0rc3/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.141707 datalookup-1.0.0rc3/docs/internals/
+-rw-rw-rw-   0        0        0      443 2023-06-06 15:59:32.000000 datalookup-1.0.0rc3/docs/internals/changelog.rst
+-rw-rw-rw-   0        0        0     2905 2023-06-06 15:59:32.000000 datalookup-1.0.0rc3/docs/internals/coding-style.rst
+-rw-rw-rw-   0        0        0       58 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/docs/internals/contributing.rst
+-rw-rw-rw-   0        0        0      449 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/docs/internals/deprecations.rst
+-rw-rw-rw-   0        0        0      307 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/docs/internals/index.rst
+-rw-rw-rw-   0        0        0     2395 2023-06-06 15:59:32.000000 datalookup-1.0.0rc3/docs/internals/release-process.rst
+-rwxrwxrwx   0        0        0      800 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/docs/make.bat
+-rw-rw-rw-   0        0        0       63 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/docs/requirements.txt
+-rw-rw-rw-   0        0        0      202 2023-06-08 17:25:06.000000 datalookup-1.0.0rc3/docs/spelling_wordlist
+drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.147708 datalookup-1.0.0rc3/licenses/
+-rw-rw-rw-   0        0        0     1579 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/licenses/django.license
+-rw-rw-rw-   0        0        0     1497 2023-06-12 13:01:49.000000 datalookup-1.0.0rc3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 13:08:39.202206 datalookup-1.0.0rc3/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-06-05 15:31:49.000000 datalookup-1.0.0rc3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.175205 datalookup-1.0.0rc3/tests/
+-rw-rw-rw-   0        0        0      439 2023-06-09 10:37:27.000000 datalookup-1.0.0rc3/tests/README.rst
+-rw-rw-rw-   0        0        0        0 2022-04-23 14:09:47.000000 datalookup-1.0.0rc3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.188207 datalookup-1.0.0rc3/tests/data/
+-rw-rw-rw-   0        0        0      956 2023-05-29 16:14:03.000000 datalookup-1.0.0rc3/tests/data/books.json
+-rw-rw-rw-   0        0        0     1652 2023-05-30 19:23:32.000000 datalookup-1.0.0rc3/tests/data/recipe.json
+-rw-rw-rw-   0        0        0      231 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/tests/lookup.py
+-rw-rw-rw-   0        0        0       77 2023-05-11 15:53:03.000000 datalookup-1.0.0rc3/tests/pytest.ini
+-rw-rw-rw-   0        0        0       62 2023-06-06 15:59:32.000000 datalookup-1.0.0rc3/tests/requirements.txt
+-rw-rw-rw-   0        0        0    23841 2023-06-09 10:34:07.000000 datalookup-1.0.0rc3/tests/tests.py
+-rw-rw-rw-   0        0        0     1406 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/tox.ini
```

### Comparing `datalookup-1.0.0rc1/.github/workflows/coverage.yml` & `datalookup-1.0.0rc3/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/.github/workflows/docs.yml` & `datalookup-1.0.0rc3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/.github/workflows/linters.yml` & `datalookup-1.0.0rc3/.github/workflows/linters.yml`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/.github/workflows/tests.yml` & `datalookup-1.0.0rc3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/.gitignore` & `datalookup-1.0.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/.pre-commit-config.yaml` & `datalookup-1.0.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/CODE_OF_CONDUCT.md` & `datalookup-1.0.0rc3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/CONTRIBUTING.rst` & `datalookup-1.0.0rc3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/LICENCE` & `datalookup-1.0.0rc3/LICENCE`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/PKG-INFO` & `datalookup-1.0.0rc3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datalookup
-Version: 1.0.0rc1
+Version: 1.0.0rc3
 Summary: Deep nested data filtering library
 Author-email: Stephane Capponi <stephane.capponi@proton.me>
 License: MIT
 Project-URL: homepage, https://datalookup.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/pyshare/datalookup
-Project-URL: changelog, https://github.com/pyshare/datalookup/blob/master/docs/changelog.txt
+Project-URL: changelog, https://datalookup.readthedocs.io/en/latest/internals/changelog.html
 Keywords: filter,dictionary,nested,datalookup,data-filtering,deep-filtering,lookup
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
@@ -224,69 +224,47 @@
 
 .. code-block:: python
 
     # author is one of the field of the dictionary
     # '__contains' is the lookup
     books.filter(author__contains="Row")
 
-.. list-table:: Title
-    :widths: 25 25 50
-    :header-rows: 1
-
-    * - Lookup
-      - Case-insensitive lookup
-      - Description
-
-    * - exact
-      - iexact
-      - Exact match
-
-    * - contains
-      - icontains
-      - Containment test
-
-    * - in
-      -
-      - In a given iterable; strings (being iterables) are accepted.
-
-    * - gt
-      -
-      - Greater than
-
-    * - gte
-      -
-      - Greater than or equal to
-
-    * - lt
-      -
-      - Lower than
-
-    * - lte
-      -
-      - Lower than or equal to
-
-    * - startswith
-      - istartswith
-      - Starts with a speific string
-
-    * - endswith
-      - iendswith
-      - Ends with a speific string
-
-    * - range
-      -
-      - Range between two values. Integer only
-
-    * - isnull
-      -
-      - Check that a field is null. Takes either True or False
-
-    * - regex
-      - iregex
-      - Regular expression match
++--------------+-------------------------+-----------------------------------------------------------------+
+| Lookup       | Case-insensitive lookup | Description                                                     |
++==============+=========================+=================================================================+
+| exact        | iexact                  | Exact match                                                     |
++--------------+-------------------------+-----------------------------------------------------------------+
+| contains     | icontains               | Containment test                                                |
++--------------+-------------------------+-----------------------------------------------------------------+
+| startswtih   | istartswith             | Starts with a specific string                                   |
++--------------+-------------------------+-----------------------------------------------------------------+
+| endswith     | iendswith               | Ends with a specific string                                     |
++--------------+-------------------------+-----------------------------------------------------------------+
+| regex        | iregex                  | Regular expression match                                        |
++--------------+-------------------------+-----------------------------------------------------------------+
+| in           |                         | In a given iterable; strings (being iterables) are accepted     |
++--------------+-------------------------+-----------------------------------------------------------------+
+| gt           |                         | Grater than                                                     |
++--------------+-------------------------+-----------------------------------------------------------------+
+| gte          |                         | Greater that or equal                                           |
++--------------+-------------------------+-----------------------------------------------------------------+
+| lt           |                         | Lower than                                                      |
++--------------+-------------------------+-----------------------------------------------------------------+
+| lte          |                         | Lower than or equal to                                          |
++--------------+-------------------------+-----------------------------------------------------------------+
+| range        |                         | Range between two values. Integer only                          |
++--------------+-------------------------+-----------------------------------------------------------------+
+| isnull       |                         | Check that a field is null. Takes either True or False          |
++--------------+-------------------------+-----------------------------------------------------------------+
+| contained_by |                         | Check data is a subset of the passed values. ArrayField only    |
++--------------+-------------------------+-----------------------------------------------------------------+
+| overlap      |                         | Data shares any results with the passed values. ArrayField only |
++--------------+-------------------------+-----------------------------------------------------------------+
+| len          |                         | Check length of the array. ArrayField only                      |
++--------------+-------------------------+-----------------------------------------------------------------+
 
 Documentation
 =============
 
 Datalookup does not stop here. The full documentation is in the ``docs``
 directory or online at https://datalookup.readthedocs.io/en/latest/
```

### Comparing `datalookup-1.0.0rc1/README.rst` & `datalookup-1.0.0rc3/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -196,69 +196,47 @@
 
 .. code-block:: python
 
     # author is one of the field of the dictionary
     # '__contains' is the lookup
     books.filter(author__contains="Row")
 
-.. list-table:: Title
-    :widths: 25 25 50
-    :header-rows: 1
-
-    * - Lookup
-      - Case-insensitive lookup
-      - Description
-
-    * - exact
-      - iexact
-      - Exact match
-
-    * - contains
-      - icontains
-      - Containment test
-
-    * - in
-      -
-      - In a given iterable; strings (being iterables) are accepted.
-
-    * - gt
-      -
-      - Greater than
-
-    * - gte
-      -
-      - Greater than or equal to
-
-    * - lt
-      -
-      - Lower than
-
-    * - lte
-      -
-      - Lower than or equal to
-
-    * - startswith
-      - istartswith
-      - Starts with a speific string
-
-    * - endswith
-      - iendswith
-      - Ends with a speific string
-
-    * - range
-      -
-      - Range between two values. Integer only
-
-    * - isnull
-      -
-      - Check that a field is null. Takes either True or False
-
-    * - regex
-      - iregex
-      - Regular expression match
++--------------+-------------------------+-----------------------------------------------------------------+
+| Lookup       | Case-insensitive lookup | Description                                                     |
++==============+=========================+=================================================================+
+| exact        | iexact                  | Exact match                                                     |
++--------------+-------------------------+-----------------------------------------------------------------+
+| contains     | icontains               | Containment test                                                |
++--------------+-------------------------+-----------------------------------------------------------------+
+| startswtih   | istartswith             | Starts with a specific string                                   |
++--------------+-------------------------+-----------------------------------------------------------------+
+| endswith     | iendswith               | Ends with a specific string                                     |
++--------------+-------------------------+-----------------------------------------------------------------+
+| regex        | iregex                  | Regular expression match                                        |
++--------------+-------------------------+-----------------------------------------------------------------+
+| in           |                         | In a given iterable; strings (being iterables) are accepted     |
++--------------+-------------------------+-----------------------------------------------------------------+
+| gt           |                         | Grater than                                                     |
++--------------+-------------------------+-----------------------------------------------------------------+
+| gte          |                         | Greater that or equal                                           |
++--------------+-------------------------+-----------------------------------------------------------------+
+| lt           |                         | Lower than                                                      |
++--------------+-------------------------+-----------------------------------------------------------------+
+| lte          |                         | Lower than or equal to                                          |
++--------------+-------------------------+-----------------------------------------------------------------+
+| range        |                         | Range between two values. Integer only                          |
++--------------+-------------------------+-----------------------------------------------------------------+
+| isnull       |                         | Check that a field is null. Takes either True or False          |
++--------------+-------------------------+-----------------------------------------------------------------+
+| contained_by |                         | Check data is a subset of the passed values. ArrayField only    |
++--------------+-------------------------+-----------------------------------------------------------------+
+| overlap      |                         | Data shares any results with the passed values. ArrayField only |
++--------------+-------------------------+-----------------------------------------------------------------+
+| len          |                         | Check length of the array. ArrayField only                      |
++--------------+-------------------------+-----------------------------------------------------------------+
 
 Documentation
 =============
 
 Datalookup does not stop here. The full documentation is in the ``docs``
 directory or online at https://datalookup.readthedocs.io/en/latest/
```

### Comparing `datalookup-1.0.0rc1/datalookup/__init__.py` & `datalookup-1.0.0rc3/datalookup/__init__.py`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/datalookup/fields.py` & `datalookup-1.0.0rc3/datalookup/fields.py`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/datalookup/lookup.py` & `datalookup-1.0.0rc3/datalookup/lookup.py`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/datalookup/utils.py` & `datalookup-1.0.0rc3/datalookup/utils.py`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/datalookup.egg-info/PKG-INFO` & `datalookup-1.0.0rc3/datalookup.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datalookup
-Version: 1.0.0rc1
+Version: 1.0.0rc3
 Summary: Deep nested data filtering library
 Author-email: Stephane Capponi <stephane.capponi@proton.me>
 License: MIT
 Project-URL: homepage, https://datalookup.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/pyshare/datalookup
-Project-URL: changelog, https://github.com/pyshare/datalookup/blob/master/docs/changelog.txt
+Project-URL: changelog, https://datalookup.readthedocs.io/en/latest/internals/changelog.html
 Keywords: filter,dictionary,nested,datalookup,data-filtering,deep-filtering,lookup
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
@@ -224,69 +224,47 @@
 
 .. code-block:: python
 
     # author is one of the field of the dictionary
     # '__contains' is the lookup
     books.filter(author__contains="Row")
 
-.. list-table:: Title
-    :widths: 25 25 50
-    :header-rows: 1
-
-    * - Lookup
-      - Case-insensitive lookup
-      - Description
-
-    * - exact
-      - iexact
-      - Exact match
-
-    * - contains
-      - icontains
-      - Containment test
-
-    * - in
-      -
-      - In a given iterable; strings (being iterables) are accepted.
-
-    * - gt
-      -
-      - Greater than
-
-    * - gte
-      -
-      - Greater than or equal to
-
-    * - lt
-      -
-      - Lower than
-
-    * - lte
-      -
-      - Lower than or equal to
-
-    * - startswith
-      - istartswith
-      - Starts with a speific string
-
-    * - endswith
-      - iendswith
-      - Ends with a speific string
-
-    * - range
-      -
-      - Range between two values. Integer only
-
-    * - isnull
-      -
-      - Check that a field is null. Takes either True or False
-
-    * - regex
-      - iregex
-      - Regular expression match
++--------------+-------------------------+-----------------------------------------------------------------+
+| Lookup       | Case-insensitive lookup | Description                                                     |
++==============+=========================+=================================================================+
+| exact        | iexact                  | Exact match                                                     |
++--------------+-------------------------+-----------------------------------------------------------------+
+| contains     | icontains               | Containment test                                                |
++--------------+-------------------------+-----------------------------------------------------------------+
+| startswtih   | istartswith             | Starts with a specific string                                   |
++--------------+-------------------------+-----------------------------------------------------------------+
+| endswith     | iendswith               | Ends with a specific string                                     |
++--------------+-------------------------+-----------------------------------------------------------------+
+| regex        | iregex                  | Regular expression match                                        |
++--------------+-------------------------+-----------------------------------------------------------------+
+| in           |                         | In a given iterable; strings (being iterables) are accepted     |
++--------------+-------------------------+-----------------------------------------------------------------+
+| gt           |                         | Grater than                                                     |
++--------------+-------------------------+-----------------------------------------------------------------+
+| gte          |                         | Greater that or equal                                           |
++--------------+-------------------------+-----------------------------------------------------------------+
+| lt           |                         | Lower than                                                      |
++--------------+-------------------------+-----------------------------------------------------------------+
+| lte          |                         | Lower than or equal to                                          |
++--------------+-------------------------+-----------------------------------------------------------------+
+| range        |                         | Range between two values. Integer only                          |
++--------------+-------------------------+-----------------------------------------------------------------+
+| isnull       |                         | Check that a field is null. Takes either True or False          |
++--------------+-------------------------+-----------------------------------------------------------------+
+| contained_by |                         | Check data is a subset of the passed values. ArrayField only    |
++--------------+-------------------------+-----------------------------------------------------------------+
+| overlap      |                         | Data shares any results with the passed values. ArrayField only |
++--------------+-------------------------+-----------------------------------------------------------------+
+| len          |                         | Check length of the array. ArrayField only                      |
++--------------+-------------------------+-----------------------------------------------------------------+
 
 Documentation
 =============
 
 Datalookup does not stop here. The full documentation is in the ``docs``
 directory or online at https://datalookup.readthedocs.io/en/latest/
```

### Comparing `datalookup-1.0.0rc1/datalookup.egg-info/SOURCES.txt` & `datalookup-1.0.0rc3/datalookup.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .readthedocs.yml
 AUTHORS
 CODE_OF_CONDUCT.md
 CONTRIBUTING.rst
 LICENCE
 README.rst
 pyproject.toml
-readme.rst
 setup.py
 tox.ini
 .github/workflows/coverage.yml
 .github/workflows/docs.yml
 .github/workflows/linters.yml
 .github/workflows/tests.yml
 datalookup/__init__.py
```

### Comparing `datalookup-1.0.0rc1/docs/Makefile` & `datalookup-1.0.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/docs/conf.py` & `datalookup-1.0.0rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/docs/index.rst` & `datalookup-1.0.0rc3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/docs/internals/coding-style.rst` & `datalookup-1.0.0rc3/docs/internals/coding-style.rst`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/docs/internals/release-process.rst` & `datalookup-1.0.0rc3/docs/internals/release-process.rst`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/docs/make.bat` & `datalookup-1.0.0rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/licenses/django.license` & `datalookup-1.0.0rc3/licenses/django.license`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/pyproject.toml` & `datalookup-1.0.0rc3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Typing :: Typed"
 ]
 dynamic = ["version", "readme"]
 
 [project.urls]
 homepage = "https://datalookup.readthedocs.io/en/latest/"
 repository = "https://github.com/pyshare/datalookup"
-changelog = "https://github.com/pyshare/datalookup/blob/master/docs/changelog.txt"
+changelog = "https://datalookup.readthedocs.io/en/latest/internals/changelog.html"
 
 [tool.setuptools]
 packages = ["datalookup"]
 
 [tool.setuptools.dynamic]
 readme = {file = ["README.rst"]}
```

### Comparing `datalookup-1.0.0rc1/tests/data/books.json` & `datalookup-1.0.0rc3/tests/data/books.json`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/tests/data/recipe.json` & `datalookup-1.0.0rc3/tests/data/recipe.json`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/tests/tests.py` & `datalookup-1.0.0rc3/tests/tests.py`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc1/tox.ini` & `datalookup-1.0.0rc3/tox.ini`

 * *Files identical despite different names*

