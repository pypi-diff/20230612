# Comparing `tmp/winterapi-0.1.0.tar.gz` & `tmp/winterapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winterapi-0.1.0.tar", last modified: Sun Jun 11 19:21:47 2023, max compression
+gzip compressed data, was "winterapi-0.1.1.tar", last modified: Mon Jun 12 02:35:34 2023, max compression
```

## Comparing `winterapi-0.1.0.tar` & `winterapi-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 robertstein   (501) staff       (20)        0 2023-06-11 19:21:47.962148 winterapi-0.1.0/
-drwxr-xr-x   0 robertstein   (501) staff       (20)        0 2023-06-11 19:21:47.953989 winterapi-0.1.0/.github/
-drwxr-xr-x   0 robertstein   (501) staff       (20)        0 2023-06-11 19:21:47.956926 winterapi-0.1.0/.github/workflows/
--rw-r--r--   0 robertstein   (501) staff       (20)      573 2023-06-11 18:21:39.000000 winterapi-0.1.0/.github/workflows/black.yml
--rw-r--r--   0 robertstein   (501) staff       (20)     2617 2023-06-11 18:43:47.000000 winterapi-0.1.0/.github/workflows/continuous_integration.yml
--rw-r--r--   0 robertstein   (501) staff       (20)      522 2023-06-11 18:10:43.000000 winterapi-0.1.0/.github/workflows/isort.yml
--rw-r--r--   0 robertstein   (501) staff       (20)      599 2023-06-11 18:10:43.000000 winterapi-0.1.0/.github/workflows/pylint.yml
--rw-r--r--   0 robertstein   (501) staff       (20)     1806 2023-02-22 19:09:49.000000 winterapi-0.1.0/.gitignore
--rw-r--r--   0 robertstein   (501) staff       (20)      713 2023-06-07 23:11:11.000000 winterapi-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 robertstein   (501) staff       (20)     1063 2023-02-19 20:17:27.000000 winterapi-0.1.0/LICENSE
--rw-r--r--   0 robertstein   (501) staff       (20)     1388 2023-06-11 19:21:47.961900 winterapi-0.1.0/PKG-INFO
--rw-r--r--   0 robertstein   (501) staff       (20)      513 2023-06-11 18:52:17.000000 winterapi-0.1.0/README.md
-drwxr-xr-x   0 robertstein   (501) staff       (20)        0 2023-06-11 19:21:47.958079 winterapi-0.1.0/notebooks/
--rw-r--r--   0 robertstein   (501) staff       (20)    17962 2023-06-08 17:02:03.000000 winterapi-0.1.0/notebooks/0_intro_accounts.ipynb
--rw-r--r--   0 robertstein   (501) staff       (20)    22608 2023-06-08 17:03:52.000000 winterapi-0.1.0/notebooks/1_too_models.ipynb
--rw-r--r--   0 robertstein   (501) staff       (20)    23058 2023-06-08 17:14:35.000000 winterapi-0.1.0/notebooks/2_submitting_toos.ipynb
--rw-r--r--   0 robertstein   (501) staff       (20)     2170 2023-06-09 00:49:42.000000 winterapi-0.1.0/pyproject.toml
--rw-r--r--   0 robertstein   (501) staff       (20)       38 2023-06-11 19:21:47.962203 winterapi-0.1.0/setup.cfg
-drwxr-xr-x   0 robertstein   (501) staff       (20)        0 2023-06-11 19:21:47.958835 winterapi-0.1.0/tests/
--rw-r--r--   0 robertstein   (501) staff       (20)      445 2023-06-11 17:59:52.000000 winterapi-0.1.0/tests/test_login.py
--rw-r--r--   0 robertstein   (501) staff       (20)     2207 2023-06-11 18:01:00.000000 winterapi-0.1.0/tests/test_schedule.py
-drwxr-xr-x   0 robertstein   (501) staff       (20)        0 2023-06-11 19:21:47.959121 winterapi-0.1.0/tests/testdata/
--rw-r--r--   0 robertstein   (501) staff       (20)      820 2023-06-11 18:06:22.000000 winterapi-0.1.0/tests/testdata/test_schedule.csv
-drwxr-xr-x   0 robertstein   (501) staff       (20)        0 2023-06-11 19:21:47.960855 winterapi-0.1.0/winterapi/
--rw-r--r--   0 robertstein   (501) staff       (20)      117 2023-06-08 16:52:58.000000 winterapi-0.1.0/winterapi/__init__.py
--rw-r--r--   0 robertstein   (501) staff       (20)      611 2023-06-11 18:00:46.000000 winterapi-0.1.0/winterapi/configure_tests.py
--rw-r--r--   0 robertstein   (501) staff       (20)     4288 2023-06-08 16:54:51.000000 winterapi-0.1.0/winterapi/credentials.py
--rw-r--r--   0 robertstein   (501) staff       (20)      333 2023-06-09 20:59:35.000000 winterapi-0.1.0/winterapi/endpoints.py
--rw-r--r--   0 robertstein   (501) staff       (20)     4957 2023-06-09 00:48:40.000000 winterapi-0.1.0/winterapi/fidelius.py
--rw-r--r--   0 robertstein   (501) staff       (20)     9684 2023-06-10 00:35:34.000000 winterapi-0.1.0/winterapi/messenger.py
-drwxr-xr-x   0 robertstein   (501) staff       (20)        0 2023-06-11 19:21:47.961611 winterapi-0.1.0/winterapi.egg-info/
--rw-r--r--   0 robertstein   (501) staff       (20)     1388 2023-06-11 19:21:47.000000 winterapi-0.1.0/winterapi.egg-info/PKG-INFO
--rw-r--r--   0 robertstein   (501) staff       (20)      677 2023-06-11 19:21:47.000000 winterapi-0.1.0/winterapi.egg-info/SOURCES.txt
--rw-r--r--   0 robertstein   (501) staff       (20)        1 2023-06-11 19:21:47.000000 winterapi-0.1.0/winterapi.egg-info/dependency_links.txt
--rw-r--r--   0 robertstein   (501) staff       (20)      100 2023-06-11 19:21:47.000000 winterapi-0.1.0/winterapi.egg-info/requires.txt
--rw-r--r--   0 robertstein   (501) staff       (20)       10 2023-06-11 19:21:47.000000 winterapi-0.1.0/winterapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:35:34.481500 winterapi-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:35:34.477500 winterapi-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-12 02:33:59.000000 winterapi-0.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:35:34.477500 winterapi-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-12 02:33:59.000000 winterapi-0.1.1/.github/workflows/automerge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-12 02:33:59.000000 winterapi-0.1.1/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-12 02:33:59.000000 winterapi-0.1.1/.github/workflows/continuous_integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-12 02:33:59.000000 winterapi-0.1.1/.github/workflows/isort.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-12 02:33:59.000000 winterapi-0.1.1/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-12 02:33:59.000000 winterapi-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-12 02:33:59.000000 winterapi-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-12 02:33:59.000000 winterapi-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-12 02:35:34.481500 winterapi-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-12 02:33:59.000000 winterapi-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:35:34.481500 winterapi-0.1.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-06-12 02:33:59.000000 winterapi-0.1.1/notebooks/0_intro_accounts.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-06-12 02:33:59.000000 winterapi-0.1.1/notebooks/1_too_models.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-06-12 02:33:59.000000 winterapi-0.1.1/notebooks/2_submitting_toos.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-12 02:33:59.000000 winterapi-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 02:35:34.481500 winterapi-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:35:34.481500 winterapi-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-12 02:33:59.000000 winterapi-0.1.1/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-12 02:33:59.000000 winterapi-0.1.1/tests/test_schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:35:34.481500 winterapi-0.1.1/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-12 02:35:18.000000 winterapi-0.1.1/tests/testdata/test_schedule.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:35:34.481500 winterapi-0.1.1/winterapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 02:33:59.000000 winterapi-0.1.1/winterapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-12 02:33:59.000000 winterapi-0.1.1/winterapi/configure_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-06-12 02:33:59.000000 winterapi-0.1.1/winterapi/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-12 02:33:59.000000 winterapi-0.1.1/winterapi/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-12 02:33:59.000000 winterapi-0.1.1/winterapi/fidelius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-06-12 02:33:59.000000 winterapi-0.1.1/winterapi/messenger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:35:34.481500 winterapi-0.1.1/winterapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-12 02:35:34.000000 winterapi-0.1.1/winterapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-12 02:35:34.000000 winterapi-0.1.1/winterapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 02:35:34.000000 winterapi-0.1.1/winterapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 02:35:34.000000 winterapi-0.1.1/winterapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 02:35:34.000000 winterapi-0.1.1/winterapi.egg-info/top_level.txt
```

### Comparing `winterapi-0.1.0/.github/workflows/continuous_integration.yml` & `winterapi-0.1.1/.github/workflows/continuous_integration.yml`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         with:
           python-version: ${{ matrix.python-version }}
           cache: 'pip'
           cache-dependency-path: pyproject.toml
 
       - name: install packages
         run: |
-          pip install -e .
+          pip install --editable ".[dev]"
 
       # Set up keyring
       - name: Set up keyring
         run: |
           sudo apt-get update
           pip install keyrings.alt
 
@@ -58,15 +58,15 @@
         if: ${{ success() }}
         run: |
           coveralls --service=github
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Echo tag name
-        run: echo "Tag is ${{ github.ref }}, Tagged is ${{ startsWith(github.ref, 'refs/tags/')}}, Python Check is ${{matrix.python-version == 3.9}},  Deploy is ${{ startsWith(github.ref, 'refs/tags/') && matrix.python-version == 3.9}}"
+        run: echo "Tag is ${{ github.ref }}, Tagged is ${{ startsWith(github.ref, 'refs/tags/')}}, Python Check is ${{matrix.python-version == 3.11}},  Deploy is ${{ startsWith(github.ref, 'refs/tags/') && matrix.python-version == 3.9}}"
 
       - name: Install pypa/build
         run: >-
           python -m
           pip install
           build
           --user
@@ -76,11 +76,11 @@
           build
           --sdist
           --wheel
           --outdir dist/
           .
 
       - name: Publish distribution 📦 to PyPI
-        if: ${{ startsWith(github.ref, 'refs/tags/') && success() && matrix.python-version == 3.9 && github.event_name == 'push'}}
+        if: ${{ startsWith(github.ref, 'refs/tags/') && success() && matrix.python-version == 3.11 && github.event_name == 'push'}}
         uses: pypa/gh-action-pypi-publish@master
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `winterapi-0.1.0/.github/workflows/pylint.yml` & `winterapi-0.1.1/.github/workflows/black.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-name: Pylint
+name: Black
 
 on: [push, pull_request]
 
 jobs:
-  pylint:
+  black:
 
     runs-on: ubuntu-latest
-
     steps:
       - uses: actions/checkout@v3
-      - name: Install poetry
-        run: pipx install poetry
       - name: Set up Python 3.11
         uses: actions/setup-python@v4
         with:
           python-version: 3.11
           cache: 'pip'
           cache-dependency-path: pyproject.toml
       - name: Install dependencies
         run: |
           pip install --upgrade pip
-          pip install -e .
-      - name: Analysing the code with pylint
+          pip install --editable ".[dev]"
+      - name: Reformat the code with black
         run: |
-           pylint winterapi --fail-under=10.00
+          black . --check
```

### Comparing `winterapi-0.1.0/.gitignore` & `winterapi-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `winterapi-0.1.0/.pre-commit-config.yaml` & `winterapi-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `winterapi-0.1.0/LICENSE` & `winterapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `winterapi-0.1.0/PKG-INFO` & `winterapi-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winterapi
-Version: 0.1.0
+Version: 0.1.1
 Author-email: Robert Stein <rdstein@caltech.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/winter-telescope/winterapi
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
@@ -15,15 +15,30 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # winterapi
 API interactions for WINTER
 
 [![Coverage Status](https://coveralls.io/repos/github/winter-telescope/winterapi/badge.svg?branch=tests)](https://coveralls.io/github/winter-telescope/winterapi?branch=tests)
 [![CI](https://github.com/winter-telescope/winterapi/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/winter-telescope/winterapi/actions/workflows/continuous_integration.yml) 
 [![PyPI version](https://badge.fury.io/py/winterapi.svg)](https://badge.fury.io/py/winterapi)
+
+## Installation
+### Install from pypi
+```bash
+pip install winterapi
+```
+
+### Install from source
+```bash
+git clone git@github.com:winter-telescope/winterapi.git
+cd winterapi
+pip install --editable ".[dev]"
+pre-commit install
+```
```

### Comparing `winterapi-0.1.0/notebooks/0_intro_accounts.ipynb` & `winterapi-0.1.1/notebooks/0_intro_accounts.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-0.1.0/notebooks/1_too_models.ipynb` & `winterapi-0.1.1/notebooks/1_too_models.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-0.1.0/notebooks/2_submitting_toos.ipynb` & `winterapi-0.1.1/notebooks/2_submitting_toos.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-0.1.0/pyproject.toml` & `winterapi-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "winterapi"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = [
     {name = "Robert Stein", email = "rdstein@caltech.edu"}
 ]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
@@ -27,22 +27,26 @@
     'Operating System :: Unix',
     'Operating System :: MacOS',
 ]
 dependencies = [
     "pandas",
     "keyring",
     "cryptography",
-    "black",
-    "isort",
-    "pylint",
     "pre-commit",
     "jupyter",
     "backoff",
     "pydantic",
-    "wintertoo>=0.3.6"
+    "wintertoo>=0.3.8"
+]
+[project.optional-dependencies]
+dev = [
+    "black == 23.3.0",
+    "isort == 5.12.0",
+    "pylint == 2.17.4",
+    "coveralls",
 ]
 
 [project.urls]
 Homepage = "https://github.com/winter-telescope/winterapi"
 
 [tool.setuptools]
 packages = ["winterapi"]
```

### Comparing `winterapi-0.1.0/tests/test_schedule.py` & `winterapi-0.1.1/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `winterapi-0.1.0/tests/testdata/test_schedule.csv` & `winterapi-0.1.1/tests/testdata/test_schedule.csv`

 * *Files identical despite different names*

### Comparing `winterapi-0.1.0/winterapi/configure_tests.py` & `winterapi-0.1.1/winterapi/configure_tests.py`

 * *Files identical despite different names*

### Comparing `winterapi-0.1.0/winterapi/credentials.py` & `winterapi-0.1.1/winterapi/credentials.py`

 * *Files identical despite different names*

### Comparing `winterapi-0.1.0/winterapi/fidelius.py` & `winterapi-0.1.1/winterapi/fidelius.py`

 * *Files identical despite different names*

### Comparing `winterapi-0.1.0/winterapi/messenger.py` & `winterapi-0.1.1/winterapi/messenger.py`

 * *Files identical despite different names*

### Comparing `winterapi-0.1.0/winterapi.egg-info/PKG-INFO` & `winterapi-0.1.1/winterapi.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winterapi
-Version: 0.1.0
+Version: 0.1.1
 Author-email: Robert Stein <rdstein@caltech.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/winter-telescope/winterapi
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
@@ -15,15 +15,30 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # winterapi
 API interactions for WINTER
 
 [![Coverage Status](https://coveralls.io/repos/github/winter-telescope/winterapi/badge.svg?branch=tests)](https://coveralls.io/github/winter-telescope/winterapi?branch=tests)
 [![CI](https://github.com/winter-telescope/winterapi/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/winter-telescope/winterapi/actions/workflows/continuous_integration.yml) 
 [![PyPI version](https://badge.fury.io/py/winterapi.svg)](https://badge.fury.io/py/winterapi)
+
+## Installation
+### Install from pypi
+```bash
+pip install winterapi
+```
+
+### Install from source
+```bash
+git clone git@github.com:winter-telescope/winterapi.git
+cd winterapi
+pip install --editable ".[dev]"
+pre-commit install
+```
```

### Comparing `winterapi-0.1.0/winterapi.egg-info/SOURCES.txt` & `winterapi-0.1.1/winterapi.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
+.github/dependabot.yml
+.github/workflows/automerge.yml
 .github/workflows/black.yml
 .github/workflows/continuous_integration.yml
 .github/workflows/isort.yml
 .github/workflows/pylint.yml
 notebooks/0_intro_accounts.ipynb
 notebooks/1_too_models.ipynb
 notebooks/2_submitting_toos.ipynb
```

