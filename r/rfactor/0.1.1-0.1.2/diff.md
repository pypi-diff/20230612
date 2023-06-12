# Comparing `tmp/rfactor-0.1.1.tar.gz` & `tmp/rfactor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/stijnvh/repositories/rfactor/dist/tmp7hvs8jbg/rfactor-0.1.1.tar", last modified: Thu Dec  9 11:02:20 2021, max compression
+gzip compressed data, was "/home/runner/work/rfactor/rfactor/dist/.tmp-b54b_c7h/rfactor-0.1.2.tar", last modified: Mon Jun 12 13:22:02 2023, max compression
```

## Comparing `rfactor-0.1.1.tar` & `rfactor-0.1.2.tar`

### file list

```diff
@@ -1,92 +1,96 @@
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      590 2021-12-09 10:01:31.000000 rfactor-0.1.1/.coveragerc
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     1187 2021-12-09 10:01:31.000000 rfactor-0.1.1/.drone.yml
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      187 2021-12-09 10:32:55.000000 rfactor-0.1.1/.gitattributes
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/.github/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     3123 2021-12-09 10:01:31.000000 rfactor-0.1.1/.github/CODE_OF_CONDUCT.rst
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      490 2021-12-09 10:01:31.000000 rfactor-0.1.1/.github/ISSUE_TEMPLATE/documentation.md
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/.github/workflows/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      949 2021-12-09 10:01:31.000000 rfactor-0.1.1/.github/workflows/binder.yml
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     1233 2021-12-09 10:32:55.000000 rfactor-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     1070 2021-12-09 10:32:55.000000 rfactor-0.1.1/.github/workflows/deploy.yml
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      781 2021-12-09 10:32:55.000000 rfactor-0.1.1/.github/workflows/update_docs.yml
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      680 2021-12-09 10:01:31.000000 rfactor-0.1.1/.gitignore
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     1259 2021-12-09 10:01:31.000000 rfactor-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      206 2021-12-09 10:01:31.000000 rfactor-0.1.1/AUTHORS.rst
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      992 2021-12-09 10:32:59.000000 rfactor-0.1.1/CHANGELOG.rst
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     7454 2021-12-09 10:01:31.000000 rfactor-0.1.1/LICENSE
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     4250 2021-12-09 11:02:20.000000 rfactor-0.1.1/PKG-INFO
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     3575 2021-12-09 10:34:01.000000 rfactor-0.1.1/README.md
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     3044 2021-12-09 10:32:55.000000 rfactor-0.1.1/README.rst
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/docs/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     1154 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/Makefile
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/docs/_static/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)       18 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/_static/.gitignore
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/docs/_static/png/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     9358 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/_static/png/DepartementOmgeving_logo.png
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     6044 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/_static/png/KULeuven_logo.png
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    10193 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/_static/png/VMM_logo.png
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     4564 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/_static/png/fluves_logo.png
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    19251 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/_static/png/matlab_comp.png
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    17687 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/_static/png/python_matlab_comp.png
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)       41 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/authors.rst
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)       43 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/changelog.rst
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     2217 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/codelegacy.rst
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)       62 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/conduct.rst
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    10125 2021-12-09 10:32:55.000000 rfactor-0.1.1/docs/conf.py
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     6535 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/contributing.rst
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    10873 2021-12-09 10:32:55.000000 rfactor-0.1.1/docs/get-started.rst
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      634 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/index.rst
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     2020 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/installation.rst
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)       63 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/license.rst
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      760 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/make.bat
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/docs/notebooks/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    45807 2021-12-09 10:01:31.000000 rfactor-0.1.1/docs/notebooks/202106_check_erosivity_implementation.ipynb
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)   388502 2021-12-09 10:32:55.000000 rfactor-0.1.1/docs/notebooks/analysis_flanders.ipynb
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/docs/notebooks/data/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      484 2021-12-09 10:32:55.000000 rfactor-0.1.1/docs/notebooks/data/README.md
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000) 13925190 2021-12-09 10:01:36.000000 rfactor-0.1.1/docs/notebooks/data/erosivity_belgium.csv
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    28488 2021-12-09 10:32:55.000000 rfactor-0.1.1/docs/notebooks/data/files.csv
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     1878 2021-12-09 10:32:55.000000 rfactor-0.1.1/docs/notebooks/data/stations.csv
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     4444 2021-12-09 10:32:55.000000 rfactor-0.1.1/docs/rfactor.rst
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      164 2021-12-09 10:01:31.000000 rfactor-0.1.1/environment.yml
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      365 2021-12-09 10:01:31.000000 rfactor-0.1.1/pyproject.toml
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     1678 2021-12-09 11:02:20.000000 rfactor-0.1.1/setup.cfg
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      704 2021-12-09 10:01:31.000000 rfactor-0.1.1/setup.py
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/src/
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/src/rfactor/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      863 2021-12-09 10:01:31.000000 rfactor-0.1.1/src/rfactor/__init__.py
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/src/rfactor/matlab/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     7657 2021-12-09 10:01:31.000000 rfactor-0.1.1/src/rfactor/matlab/core.m
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     1021 2021-12-09 10:01:31.000000 rfactor-0.1.1/src/rfactor/matlab/main.m
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    11179 2021-12-09 10:01:31.000000 rfactor-0.1.1/src/rfactor/process.py
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    10325 2021-12-09 10:32:55.000000 rfactor-0.1.1/src/rfactor/rfactor.py
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/src/rfactor.egg-info/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     4250 2021-12-09 11:02:20.000000 rfactor-0.1.1/src/rfactor.egg-info/PKG-INFO
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     2079 2021-12-09 11:02:20.000000 rfactor-0.1.1/src/rfactor.egg-info/SOURCES.txt
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)        1 2021-12-09 11:02:20.000000 rfactor-0.1.1/src/rfactor.egg-info/dependency_links.txt
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)        1 2021-12-09 10:03:31.000000 rfactor-0.1.1/src/rfactor.egg-info/not-zip-safe
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)      291 2021-12-09 11:02:20.000000 rfactor-0.1.1/src/rfactor.egg-info/requires.txt
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)        8 2021-12-09 11:02:20.000000 rfactor-0.1.1/src/rfactor.egg-info/top_level.txt
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/tests/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 10:01:31.000000 rfactor-0.1.1/tests/__init__.py
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     4940 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/conftest.py
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/tests/data/
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/tests/data/test_erosivitydata/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)   151489 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/data/test_erosivitydata/test_data_maximum_intensity.csv
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)   155331 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/data/test_erosivitydata/test_data_maximum_intensity_matlab_clone.csv
-drwxr-xr-x   0 stijnvh   (1000) stijnvh   (1000)        0 2021-12-09 11:02:20.000000 rfactor-0.1.1/tests/data/test_rainfalldata/
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    34308 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/data/test_rainfalldata/P01_001_2018.txt
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    44176 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/data/test_rainfalldata/P01_003_2020.txt
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    51574 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/data/test_rainfalldata/P01_010_2012.txt
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    44269 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/data/test_rainfalldata/P01_010_2016.txt
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    36259 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/data/test_rainfalldata/P05_038_2018.txt
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    41072 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/data/test_rainfalldata/P05_039_2017.txt
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    55233 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/data/test_rainfalldata/P08_018_2012.txt
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    40488 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/data/test_rainfalldata/P09_032_2020.txt
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    43992 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/data/test_rainfalldata/P11_007_2008.txt
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)    79781 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/data/test_rainfalldata/P11_024_2012.txt
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     8696 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/test_process.py
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     9307 2021-12-09 10:32:55.000000 rfactor-0.1.1/tests/test_rfactor.py
--rw-r--r--   0 stijnvh   (1000) stijnvh   (1000)     2636 2021-12-09 10:01:31.000000 rfactor-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-12 13:19:37.000000 rfactor-0.1.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-12 13:19:37.000000 rfactor-0.1.2/.drone.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-12 13:19:37.000000 rfactor-0.1.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:01.000000 rfactor-0.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-12 13:19:37.000000 rfactor-0.1.2/.github/CODE_OF_CONDUCT.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:01.000000 rfactor-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-12 13:19:37.000000 rfactor-0.1.2/.github/ISSUE_TEMPLATE/documentation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-12 13:19:37.000000 rfactor-0.1.2/.github/workflows/binder.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-12 13:19:37.000000 rfactor-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 13:19:37.000000 rfactor-0.1.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-12 13:19:37.000000 rfactor-0.1.2/.github/workflows/update_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-12 13:19:37.000000 rfactor-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-12 13:19:37.000000 rfactor-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-12 13:19:37.000000 rfactor-0.1.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-12 13:19:37.000000 rfactor-0.1.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-12 13:19:37.000000 rfactor-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-12 13:22:02.000000 rfactor-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-12 13:19:37.000000 rfactor-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-12 13:19:37.000000 rfactor-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/docs/_static/png/
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/_static/png/DepartementOmgeving_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/_static/png/KULeuven_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/_static/png/VMM_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/_static/png/fluves_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/_static/png/matlab_comp.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/_static/png/python_matlab_comp.png
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/codelegacy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/get-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    45807 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/notebooks/202106_check_erosivity_implementation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   608406 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/notebooks/analysis_flanders.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/docs/notebooks/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/notebooks/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/notebooks/data/erosivity_belgium.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    28488 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/notebooks/data/files.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/notebooks/data/stations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-06-12 13:19:37.000000 rfactor-0.1.2/docs/rfactor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-12 13:19:37.000000 rfactor-0.1.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-12 13:19:37.000000 rfactor-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-12 13:22:02.000000 rfactor-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-12 13:19:37.000000 rfactor-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:01.000000 rfactor-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/src/rfactor/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-12 13:19:37.000000 rfactor-0.1.2/src/rfactor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/src/rfactor/matlab/
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-12 13:19:37.000000 rfactor-0.1.2/src/rfactor/matlab/core.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-12 13:19:37.000000 rfactor-0.1.2/src/rfactor/matlab/main.m
+-rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-06-12 13:19:37.000000 rfactor-0.1.2/src/rfactor/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-06-12 13:19:37.000000 rfactor-0.1.2/src/rfactor/rfactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-12 13:19:37.000000 rfactor-0.1.2/src/rfactor/valid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/src/rfactor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-12 13:22:01.000000 rfactor-0.1.2/src/rfactor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-12 13:22:01.000000 rfactor-0.1.2/src/rfactor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:22:01.000000 rfactor-0.1.2/src/rfactor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:19:45.000000 rfactor-0.1.2/src/rfactor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-12 13:22:01.000000 rfactor-0.1.2/src/rfactor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 13:22:01.000000 rfactor-0.1.2/src/rfactor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:01.000000 rfactor-0.1.2/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/tests/data/test_erosivitydata/
+-rw-r--r--   0 runner    (1001) docker     (123)   151489 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/data/test_erosivitydata/test_data_maximum_intensity.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   155331 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/data/test_erosivitydata/test_data_maximum_intensity_matlab_clone.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/tests/data/test_rainfalldata/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/data/test_rainfalldata/P01_001_2018.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/data/test_rainfalldata/P01_003_2020.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/data/test_rainfalldata/P01_010_2012.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/data/test_rainfalldata/P01_010_2016.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/data/test_rainfalldata/P05_038_2018.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/data/test_rainfalldata/P05_039_2017.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/data/test_rainfalldata/P08_018_2012.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/data/test_rainfalldata/P09_032_2020.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/data/test_rainfalldata/P11_007_2008.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/data/test_rainfalldata/P11_024_2012.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:22:02.000000 rfactor-0.1.2/tests/data/test_rainfalldata_vmm_format/
+-rw-r--r--   0 runner    (1001) docker     (123)   327096 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/data/test_rainfalldata_vmm_format/P01_010.CSV
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/test_rfactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-12 13:19:37.000000 rfactor-0.1.2/tests/test_valid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-12 13:19:37.000000 rfactor-0.1.2/tox.ini
```

### Comparing `rfactor-0.1.1/.coveragerc` & `rfactor-0.1.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/.drone.yml` & `rfactor-0.1.2/.drone.yml`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/.github/CODE_OF_CONDUCT.rst` & `rfactor-0.1.2/.github/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/.github/workflows/binder.yml` & `rfactor-0.1.2/.github/workflows/binder.yml`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/.github/workflows/ci.yml` & `rfactor-0.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/.github/workflows/deploy.yml` & `rfactor-0.1.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/.github/workflows/update_docs.yml` & `rfactor-0.1.2/.github/workflows/update_docs.yml`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/.gitignore` & `rfactor-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/.pre-commit-config.yaml` & `rfactor-0.1.2/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 exclude: '^docs/conf.py'
 
 repos:
-- repo: git://github.com/pre-commit/pre-commit-hooks
+- repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.0.1
   hooks:
   - id: trailing-whitespace
   - id: check-added-large-files
   - id: check-ast
   - id: check-json
   - id: check-merge-conflict
@@ -15,26 +15,26 @@
   - id: debug-statements
   - id: end-of-file-fixer
   - id: requirements-txt-fixer
   - id: mixed-line-ending
     args: ['--fix=auto']  # replace 'auto' with 'lf' to enforce Linux/Mac line endings or 'crlf' for Windows
 
 - repo: https://github.com/pycqa/isort
-  rev: 5.9.1
+  rev: 5.11.5
   hooks:
   - id: isort
 
 - repo: https://github.com/psf/black
-  rev: 21.6b0
+  rev: 22.3.0
   hooks:
   - id: black
     language_version: python3
 
-- repo: https://gitlab.com/pycqa/flake8
-  rev: 3.9.2
+- repo: https://github.com/pycqa/flake8
+  rev: 5.0.4
   hooks:
   - id: flake8
   ## You can add flake8 plugins via `additional_dependencies`:
   #  additional_dependencies: [flake8-bugbear]
 
 # Strip the output of jupyter notebooks
 - repo: https://github.com/kynan/nbstripout
```

### Comparing `rfactor-0.1.1/LICENSE` & `rfactor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/PKG-INFO` & `rfactor-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfactor
-Version: 0.1.1
+Version: 0.1.2
 Summary: Scripts to compute and analyse the RUSLE R-factor.
 Home-page: https://github.com/cn-ws/rfactor
 Author: Sacha Gobeyn
 Author-email: sacha@fluves.com
 License: LGPL-3
 Project-URL: Documentation, https://cn-ws.github.io/rfactor/
 Project-URL: Source, https://github.com/cn-ws/rfactor
@@ -51,32 +51,42 @@
 > used for the core computations. Since version 0.1.0, a faster Python
 > implementation is provided. Using the version 0.0.x will provide other
 > results compared to version \>0.1.0, as explained in the [package documentation](https://cn-ws.github.io/rfactor/).
 
 Get started
 -----------
 This package makes use of `Python` (and a limited number of dependencies
-such as Pandas and Numpy). Make sure to check out the installation instructions, and follow the example in
+such as Pandas and Numpy). To install:
+
+```
+pip install rfactor
+```
+
+Make sure to check out the installation instructions and follow the example in
 the _Get started section_ of the [package documentation](https://cn-ws.github.io/rfactor/).
 
 Rainfall and erosivity data
 ---------------------------
 
 Any 10 minute ezqolurion input rainfall should work, but input rainfall data for the initial project
 were provided by the Flemish Environment Agency (VMM) and the Royal Meteorological Institute (RMI).
-Teh data from the Flemish Environment Agency (VMM) are available via
+The data from the Flemish Environment Agency (VMM) are available via
 [waterinfo](https://www.waterinfo.be). The input rainfall data from the
 Royal Meteorological Institute (RMI) are not shared in this project.
 Please contact the RMI if you would like to obtain the a copy of the RMI
 rainfall input data.
 
 The erosivity data calculated with the rainfall input data are provided
 by the partners of this project, and are used as test data for analysing
 the R-factor for Flanders.
 
+Code
+----
+The open-source code can be found on [GitHub](https://github.com/cn-ws/rfactor).
+
 Documentation
 -------------
 
 The documentation can be found on the [R-factor documentation
 page](https://cn-ws.github.io/rfactor/index.html).
 
 License
@@ -104,9 +114,7 @@
 ![image](docs/_static/png/fluves_logo.png)
 
 Note
 ----
 
 This project has been set up using PyScaffold 3.2.3. For details and
 usage information on PyScaffold see <https://pyscaffold.org/>.
-
-
```

### Comparing `rfactor-0.1.1/README.md` & `rfactor-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,32 +31,42 @@
 > used for the core computations. Since version 0.1.0, a faster Python
 > implementation is provided. Using the version 0.0.x will provide other
 > results compared to version \>0.1.0, as explained in the [package documentation](https://cn-ws.github.io/rfactor/).
 
 Get started
 -----------
 This package makes use of `Python` (and a limited number of dependencies
-such as Pandas and Numpy). Make sure to check out the installation instructions, and follow the example in
+such as Pandas and Numpy). To install:
+
+```
+pip install rfactor
+```
+
+Make sure to check out the installation instructions and follow the example in
 the _Get started section_ of the [package documentation](https://cn-ws.github.io/rfactor/).
 
 Rainfall and erosivity data
 ---------------------------
 
 Any 10 minute ezqolurion input rainfall should work, but input rainfall data for the initial project
 were provided by the Flemish Environment Agency (VMM) and the Royal Meteorological Institute (RMI).
-Teh data from the Flemish Environment Agency (VMM) are available via
+The data from the Flemish Environment Agency (VMM) are available via
 [waterinfo](https://www.waterinfo.be). The input rainfall data from the
 Royal Meteorological Institute (RMI) are not shared in this project.
 Please contact the RMI if you would like to obtain the a copy of the RMI
 rainfall input data.
 
 The erosivity data calculated with the rainfall input data are provided
 by the partners of this project, and are used as test data for analysing
 the R-factor for Flanders.
 
+Code
+----
+The open-source code can be found on [GitHub](https://github.com/cn-ws/rfactor).
+
 Documentation
 -------------
 
 The documentation can be found on the [R-factor documentation
 page](https://cn-ws.github.io/rfactor/index.html).
 
 License
```

### Comparing `rfactor-0.1.1/README.rst` & `rfactor-0.1.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -21,18 +21,21 @@
 This code is developed as a function of an analysis of rainfall
 erosivity in Flanders. The results found in the example notebooks
 are also found in `this report <https://www.friscris.be/nl/publications/herziening-van-de-neerslagerosiviteitsfactor-r-voor-de-vlaamse-erosiemodellering(9d4e2953-6c93-48d0-a1c2-d66d03c749aa).html>`_).
 
 Get started
 -----------
 This package makes use of ``Python`` (and a limited number of
-dependencies such as Pandas and Numpy). The installation
-(see :ref:`here <installation>`) is managed by making use of
-`Miniconda <https://docs.conda.io/en/latest/miniconda.html>`_. Make sure
-tocheck out the installation instructions, and follow the example in the
+dependencies such as Pandas and Numpy). To install the package:
+
+::
+
+   pip install rfactor
+
+For more information, check out the :ref:`installation instructions <installation>` and follow the example in the
 :ref:`Get started <getstarted>` page.
 
 Data & application to Flanders
 ------------------------------
 Input rainfall data are provided by the Flemish Environment Agency (VMM),
 which are also available via `waterinfo <https://www.waterinfo.be>`_. The
 input rainfall data from the Royal Meteorological Institute
@@ -44,14 +47,19 @@
 for Flanders.
 
 Documentation
 -------------
 The documentation can be found on the
 `R-factor documentation page <https://cn-ws.github.io/rfactor/index.html>`_.
 
+Code
+----
+The open-source code can be found on
+`GitHub <https://github.com/cn-ws/rfactor/>`_.
+
 License
 -------
 This project is licensed under GNU Lesser Public License v3.0, see
 :ref:`here <license>` for more information.
 
 Contact
 -------
```

### Comparing `rfactor-0.1.1/docs/Makefile` & `rfactor-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/_static/png/DepartementOmgeving_logo.png` & `rfactor-0.1.2/docs/_static/png/DepartementOmgeving_logo.png`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/_static/png/KULeuven_logo.png` & `rfactor-0.1.2/docs/_static/png/KULeuven_logo.png`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/_static/png/VMM_logo.png` & `rfactor-0.1.2/docs/_static/png/VMM_logo.png`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/_static/png/fluves_logo.png` & `rfactor-0.1.2/docs/_static/png/fluves_logo.png`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/_static/png/matlab_comp.png` & `rfactor-0.1.2/docs/_static/png/matlab_comp.png`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/_static/png/python_matlab_comp.png` & `rfactor-0.1.2/docs/_static/png/python_matlab_comp.png`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/codelegacy.rst` & `rfactor-0.1.2/docs/codelegacy.rst`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/conf.py` & `rfactor-0.1.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,11 +290,11 @@
     "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
     "setuptools": ("https://setuptools.readthedocs.io/en/stable/", None),
     "pyscaffold": ("https://pyscaffold.org/en/stable", None),
 }
 
 print(f"loading configurations for {project} {version} ...", file=sys.stderr)
 
-html_context = {
-    "source_url_prefix": "https://github.com/cn-ws/rfactor/tree/master/docs/",
-    "display_vcs_links": 1
-}
+# html_context = {
+#    "source_url_prefix": "https://github.com/cn-ws/rfactor/tree/master/docs/",
+#    "display_vcs_links": 1
+#}
```

### Comparing `rfactor-0.1.1/docs/contributing.rst` & `rfactor-0.1.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/index.rst` & `rfactor-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/installation.rst` & `rfactor-0.1.2/docs/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,24 @@
 
 .. note::
 
     Matlab or Octave were previously used to run the core rfactor code.
     See :ref:`codelegacy` for more information on the conversion towards a
     Python environment.
 
+Latest release
+--------------
+
+The rfactor package is available on `PyPI <https://pypi.org/project/rfactor/>`_. Make sure to setup an environment (either virtualenv, conda,….) first with ``pip`` installed. To install the rfactor package, run:
+
+::
+
+    pip install rfactor
+
+
 .. _installfromsource:
 
 Install from source
 -------------------
 
 To install from source, ``git clone`` the repository somewhere on your local
 machine and install the code from source.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rfactor-0.1.1/docs/make.bat` & `rfactor-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/notebooks/202106_check_erosivity_implementation.ipynb` & `rfactor-0.1.2/docs/notebooks/202106_check_erosivity_implementation.ipynb`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/notebooks/data/files.csv` & `rfactor-0.1.2/docs/notebooks/data/files.csv`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/notebooks/data/stations.csv` & `rfactor-0.1.2/docs/notebooks/data/stations.csv`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/docs/rfactor.rst` & `rfactor-0.1.2/docs/rfactor.rst`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 
 with
  - :math:`o`: the number of increments for a particular rain event,
  - :math:`e_r`: the rain energy per unit depth,
    (:math:`\frac{\text{J}}{\text{m}^{2}.\text{mm}}`), and
  - :math:`\Delta V_r`: the rain depth (mm).
 
+Note these equations assume that events are predefined. Typically, the end of
+and event is defined by a period of no rainfall. For Flanders, six hours is
+used as time period, and in addition, only events with a volume of 1.27 mm
+are retained in the calculations.
+
 Energy per unit depth of rain
 -----------------------------
 
 There are number of ways to compute the rain energy per unit depth
 :math:`e_r`, depending on the area for which the R-factor is computed. For an
 application for Flanders/Belgium, the rain energy per unit is defined by
 (Salles et al., 1999, 2002, Verstraeten et al., 2006):
```

### Comparing `rfactor-0.1.1/setup.cfg` & `rfactor-0.1.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,20 @@
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
-	importlib-metadata; python_version<"3.8"
+	importlib-metadata>=1.1.0,<4.3; python_version<"3.8"
 	pandas
 	numpy
 	matplotlib
 	tqdm
 	python-dotenv
-	jupyter
 	joblib
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
@@ -42,14 +41,15 @@
 develop = 
 	pytest
 	pytest-cov
 	pytest-xdist
 	sphinx
 	sphinx_rtd_theme
 	nbsphinx
+	jupyter
 	pre-commit
 	black
 	flake8
 	pytest-datafiles
 	tox
 	sphinx-copybutton
 	interrogate
```

### Comparing `rfactor-0.1.1/setup.py` & `rfactor-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/src/rfactor/__init__.py` & `rfactor-0.1.2/src/rfactor/__init__.py`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/src/rfactor/matlab/core.m` & `rfactor-0.1.2/src/rfactor/matlab/core.m`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/src/rfactor/matlab/main.m` & `rfactor-0.1.2/src/rfactor/matlab/main.m`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/src/rfactor/process.py` & `rfactor-0.1.2/src/rfactor/rfactor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,335 +1,322 @@
-import re
-from pathlib import Path
+import multiprocessing as mp
+import warnings
+from functools import partial
 
 import numpy as np
 import pandas as pd
-from tqdm import tqdm
+from joblib import Parallel, delayed
 
+TIME_BETWEEN_EVENTS = "6 hours"
+MIN_CUMUL_EVENT = 1.27
 
-def _days_since_start_year(series):
-    """Translate datetime series to days since start of the year
 
-    Parameters
-    ----------
-    series : pd.Series
-        Series with Datetime values. All datetime values should be of the same year.
+class RFactorInputError(Exception):
+    """Raise when input data are not conform the rfactor required input format."""
 
-    Returns
-    -------
-    days_since_start : pd.Series
-        Days since the start of the year as a float value.
 
-    Notes
-    Support function to provide integration with original Matlab implementation. Output
-    is different from Pandas datetime attribute `dayofyear` as it includes time of the
-    day as decimal value.
-    """
-    current_year = series.dt.year.unique()
-    if not len(current_year) == 1:
-        raise Exception("Input data should all be in the same year.")
+class RFactorKeyError(Exception):
+    """Raise when input data missing required column names."""
 
-    days_since_start = (
-        (series - pd.Timestamp(f"{current_year[0]}-01-01")).dt.total_seconds()
-        / 60.0
-        / 1440.0
-    )
-    return days_since_start
 
+class RFactorTypeError(Exception):
+    """Raise when input data data type of a data column is wrong."""
 
-def _extract_metadata_from_file_path(file_path):
-    """Get metadata from file name
 
-    Expects to be 'STATION_NAME_YYYY.txt' as format with ``STATION_NAME`` the
-    measurement station and the ``YYYY`` as the year of the measurement.
+def rain_energy_per_unit_depth(rain):
+    """Calculate rain energy per unit depth according to Salles/Verstraeten.
 
     Parameters
     ----------
-    file_path : pathlib.Path
-        File path of the file to extract station/year from
+    rain : numpy.ndarray
+        Rain (mm)
 
     Returns
     -------
-    station: str
-    year : str
-    """
-    if not re.fullmatch(".*_[0-9]{4}$", file_path.stem):
-        raise ValueError(
-            "Input file_path_format should " "match with 'STATION_NAME_YYYY.txt'"
-        )
-    station = "_".join(file_path.stem.split("_")[:-1])
-    year = file_path.stem.split("_")[-1]
-    return station, year
-
-
-def _check_path(file_path):
-    """Provide user feedback on file_path type."""
-    if not isinstance(file_path, Path):
-        if isinstance(file_path, str):
-            raise TypeError(
-                f"`file_path` should be a `pathlib.Path` object, use "
-                f"`Path({file_path})` to convert string file_path to valid `Path`."
-            )
-        else:
-            raise TypeError("`file_path` should be a pathlib.Path object")
-
-
-def load_rain_file(file_path):
-    """Load (legacy Matlab) file format of rainfall data of a single station/year.
-
-    The input files are defined by text files (extension: ``.txt``) that hold
-    non-zero rainfall timeseries. The data are split per station and per year with
-    a specific datafile tag (file name format: ``SOURCE_STATION_YEAR.txt``). The data
-    should not contain headers, with the first column defined as 'minutes since the
-    start of the year' and the second as the rainfall depth during the t last minutes
-    (t is the temporal resolution of the timeseries).
+    energy : float
+        Energy per unit depth.
 
-    Parameters
-    ----------
-    file_path : pathlib.Path
-        File path with rainfall data according to defined format.
-
-    Returns
-    -------
-    rain : pd.DataFrame
-        DataFrame with rainfall time series. Contains the following columns:
+    Notes
+    -----
+    The rain energy per unit depth :math:`e_r` (:math:`\\text{J}.\\text{mm}^{-1}.
+    \\text{m}^{-2}`) for an application for Flanders/Belgium is defined
+    by [1]_ [2]_ [3]_:
 
-        - *minutes_since* (int): Minutes since the start of the year
-        - *rain_mm* (float): Rain in mm
-        - *datetime* (pd.Timestamp): Time stamp
-        - *station* (str): station name
-        - *year* (int): year of the measurement
-        - *tag* (str): tag identifier, formatted as ``STATION_YEAR``
+    .. math::
 
-    Example
-    -------
-    1. Example of a rainfall file:
+        e_r = 11.12i_r^{0.31}
 
-    ::
+    with
 
-       9390 1.00 \n
-       9470 0.20 \n
-       9480 0.50 \n
-       10770 0.10 \n
-       ...  ...
+     - :math:`i_r` the rain intensity for every 10-min
+       increment (mm :math:`\\text{h}^{-1}` ).
 
+    References
+    ----------
+    .. [1] Salles, C., Poesen, J., Pissart, A., 1999, Rain erosivity indices and drop
+        size distribution for central Belgium. Presented at the General Assembly of
+        the European Geophysical Society, The Hague, The Netherlands, p. 280.
+
+    .. [2] Salles, C., Poesen, J., Sempere-Torres, D., 2002. Kinetic energy of rain and
+        its functional relationship with intensity. Journal of Hydrology 257, 256–270.
+        https://doi.org/10.1016/S0022-1694(01)00555-8
+
+    .. [3]  Verstraeten, G., Poesen, J., Demarée, G., Salles, C., 2006, Long-term
+        (105 years) variability in rain erosivity as derived from 10-min rainfall
+        depth data for Ukkel (Brussels, Belgium): Implications for assessing soil
+        erosion rates. Journal Geophysysical Research, 111, D22109.
+        https://doi.org/10.1029/2006JD007169
     """
-    _check_path(file_path)
-    if file_path.is_dir():
-        raise ValueError(
-            "`file_path` need to be the path " "to a file instead of a directory"
-        )
+    rain_energy = 0.1112 * ((rain * 6.0) ** 0.31) * rain
+    return rain_energy.sum()
 
-    station, year = _extract_metadata_from_file_path(file_path)
-    rain = pd.read_csv(
-        file_path, delimiter=" ", header=None, names=["minutes_since", "rain_mm"]
-    )
-    rain["datetime"] = pd.Timestamp(f"{year}-01-01") + pd.to_timedelta(
-        pd.to_numeric(rain["minutes_since"]), unit="min"
-    )
-    rain["station"] = station
-    rain["year"] = rain["datetime"].dt.year
-    rain["tag"] = rain["station"].astype(str) + "_" + rain["year"].astype(str)
-    return rain
 
+def maximum_intensity_matlab_clone(df):
+    """Maximum rain intensity for 30-min interval (Matlab clone).
 
-def load_rain_folder(folder_path):
-    """Load all (legacy Matlab format) files of rainfall data in a folder
+    The implementation is a direct Python-translation of the original Matlab
+    implementation by Verstraeten.
 
     Parameters
     ----------
-    folder_path : pathlib.Path
-        Folder path with rainfall data according to legacy Matlab format,
-        see :func:`rfactor.process.load_rain_file`.
+    df : pandas.DataFrame
+        DataFrame with rainfall time series. Needs to contain the following columns:
+
+        - *datetime* (pandas.Timestamp): Time stamp
+        - *rain_mm* (float): Rain in mm
+        - *event_rain_cum* (float): Cumulative rain in mm
 
     Returns
     -------
-    rain : pd.DataFrame
-        DataFrame with rainfall time series. Contains the following columns:
-
-        - *minutes_since* (int): Minutes since the start of the year
-        - *rain_mm* (float): Rain in mm
-        - *datetime* (pd.Timestamp): Time stamp
-        - *station* (str): station name
-        - *year* (int): year of the measurement
-        - *tag* (str): tag identifier, formatted as ``STATION_YEAR``
+    maxprecip_30min : float
+        Maximal 30-minute intensity during event (in mm/h).
     """
-    _check_path(folder_path)
-    if folder_path.is_file():
-        raise ValueError(
-            "`folder_path` need to be the path " "to a directory instead of a file"
+    if np.isnan(df["rain_mm"]).any():
+        raise Exception(
+            "Matlab intensity method does not support Nan values in rain" "time series."
         )
 
-    lst_df = []
+    current_year = df["datetime"].dt.year.unique()
+    if not len(current_year) == 1:
+        raise RFactorInputError("Data should all be in the same year.")
+
+    df["minutes_since"] = (
+        df["datetime"] - pd.Timestamp(f"{current_year[0]}-01-01")
+    ).dt.total_seconds().values / 60
+
+    timestamps = df["minutes_since"].values
+    rain = df["rain_mm"].values
+    rain_cum = df["event_rain_cum"].values
 
-    files = list(folder_path.glob("*.txt"))
-    for file_path in tqdm(files, total=len(files)):
-        lst_df.append(load_rain_file(file_path))
+    maxprecip_30min = 0.0
 
-    all_rain = pd.concat(lst_df)
-    all_rain = all_rain.sort_values(["station", "minutes_since"])
-    all_rain.index = range(len(all_rain))
-    return all_rain
+    if timestamps[-1] - timestamps[0] <= 30:
+        maxprecip_30min = rain[0] * 2  # *2 to mimick matlab
 
+    for idx in range(len(df) - 1):
+        eind_30min = timestamps[idx] + 20
+        begin_rain = rain_cum[idx] - rain[idx]
 
-def write_erosivity_data(df, folder_path):
-    """Write output erosivity to (legacy Matlab format) in folder.
+        eind_rain = np.interp(eind_30min, timestamps, rain_cum)
+        precip_30min = eind_rain - begin_rain
 
-    Written data are split-up for each year and station
-    (file name format: ``SOURCE_STATION_YEAR.txt``) and does not contain any headers.
-    The columns (no header!) in the written text files represent the following:
+        if precip_30min > maxprecip_30min:
+            maxprecip_30min = precip_30min
 
-    - *days_since* (float): Days since the start of the year.
-    - *erosivity_cum* (float): Cumulative erosivity over events.
-    - *all_event_rain_cum* (float): Cumulative rain over events.
+    return maxprecip_30min * 2
+
+
+def maximum_intensity(df):
+    """Maximum rain intensity for 30-min interval (Pandas rolling) expressed as mm/hour
+
+    The implementation uses a rolling window of the chosen interval to derive the
+    maximal intensity.
 
     Parameters
     ----------
     df : pandas.DataFrame
-        DataFrame with rfactor/erosivity time series. Can contain multiple columns,
-        but should have at least the following:
+        DataFrame with rainfall time series. Needs to contain the following columns:
 
-        - *datetime* (pandas.Timestamp): Time stamp
-        - *station* (str): Station identifier
-        - *erosivity_cum* (float): Cumulative erosivity over events
-        - *all_event_rain_cum* (float): Cumulative rain over events
-
-    folder_path : pathlib.Path
-        Folder path to save data according to legacy Matlab format,
-        see :func:`rfactor.process.load_rain_file`.
+        - *datetime* (pandas.Timestamp): Timestamp
+        - *rain_mm* (float): Rain in mm
 
+    Returns
+    -------
+    maxprecip_30min : float
+        Maximal 30-minute intensity during event (in mm/h).
     """
-    _check_path(folder_path)
-
-    folder_path.mkdir(exist_ok=True, parents=True)
-
-    for (station, year), df_group in df.groupby(["station", df["datetime"].dt.year]):
-        df_group["days_since"] = _days_since_start_year(df_group["datetime"])
-        formats = {
-            "days_since": "{:.3f}",
-            "erosivity_cum": "{:.2f}",
-            "all_event_rain_cum": "{:.1f}",
-        }
-        for column, fformat in formats.items():
-            df_group[column] = df_group[column].map(lambda x: fformat.format(x))
-        df_group[["days_since", "erosivity_cum", "all_event_rain_cum"]].to_csv(
-            folder_path / f"{station}_{year}.csv", header=None, index=None, sep=" "
-        )
+    # formula requires mm/hr, intensity is derived on half an hour
+    return df.rolling("30min", on="datetime")["rain_mm"].sum().max() * 2
 
 
-def get_rfactor_station_year(erosivity, stations=None, years=None):
-    """Get R-factor at end of every year for each station from cumulative erosivity.
+def _compute_erosivity(
+    rain,
+    intensity_method,
+    event_split=TIME_BETWEEN_EVENTS,
+    event_threshold=MIN_CUMUL_EVENT,
+):
+    """Calculate erosivity according to Verstraeten G. for a single year/station combi
 
     Parameters
     ----------
-    erosivity: pandas.DataFrame
-        See :func:`rfactor.rfactor.compute_erosivity`
-    stations: list
-        List of stations to extract R for.
-    years: list
-        List of years to extract R for.
+    rain : pd.DataFrame
+        DataFrame with rainfall time series. Need to contain the following columns:
+
+        - *datetime* (pd.Timestamp): Time stamp
+        - *rain_mm* (float): Rain in mm
+    intensity_method : Callable
+        Function to derive the maximal rain intensity (over 30min)
+    event_split : str
+        Time interval to split into individual rain events
+    event_threshold : float
+        Minimal cumulative rain of an event to take into account for erosivity
+        derivationevent_rain_cum
 
     Returns
     -------
-    erosivity: pandas.DataFrame
-        Updated with:
+    events : pd.DataFrame
+        DataFrame with erosivity output for each event.
 
-        - *year* (int): year
-        - *station* (str): station
-        - *erosivity_cum* (float): cumulative erosivity at
-          end of *year* and at *station*.
+        - *datetime* (pd.Timestamp): Time stamp
+        - *event_rain_cum* (float): Cumulative rain for each event
+        - *max_30min_intensity* (float): Maximal 30min intensity for each event
+        - *event_energy* (float): Rain energy per unit depth for each event
+        - *erosivity* (float): Erosivity for each event
+        - *all_events_cum* (float): Cumulative rain over all events together
+        - *erosivity_cum* (float): Cumulative erosivity over all events together
 
     """
+    if len(rain["datetime"].dt.year.unique()) != 1:  # data of a single year
+        raise RFactorInputError("DataFrame should contain data of a single year.")
+
+    # mark start of each rain event
+    rain = rain[rain["rain_mm"] > 0.0]  # Only keep measurements with rain
+    rain = rain.assign(event_start=False)
+    rain.loc[rain["datetime"].diff() >= event_split, "event_start"] = True
+    rain.loc[rain.index[0], "event_start"] = True
+
+    # add an event identifier
+    rain = rain.assign(event_idx=rain["event_start"].cumsum())
+
+    # add cumulative rain for each event
+    rain = rain.assign(event_rain_cum=rain.groupby("event_idx")["rain_mm"].cumsum())
+
+    # add rain energy for each event
+    rain = rain.assign(
+        event_energy=rain.groupby("event_idx")["rain_mm"].transform(
+            rain_energy_per_unit_depth
+        )
+    )
+
+    # calculate the maximal rain intensity in 30minutes interval
+    max_intensity_event = (
+        rain.groupby("event_idx")[["datetime", "rain_mm", "event_rain_cum"]]
+        .apply(intensity_method)
+        .rename("max_30min_intensity")
+        .reset_index()
+    )
+    rain = pd.merge(rain, max_intensity_event, how="left")
+
+    # derive event summary
+    columns = ["datetime", "event_rain_cum", "max_30min_intensity", "event_energy"]
+    rain_events = rain.groupby("event_idx")[columns].agg(
+        {
+            "datetime": "first",
+            "event_rain_cum": "last",
+            "max_30min_intensity": "last",
+            "event_energy": "last",
+        }
+    )
+
+    # calculate the erosivity
+    rain_events = rain_events.assign(
+        erosivity=rain_events["event_energy"] * rain_events["max_30min_intensity"]
+    )
 
-    if stations is not None:
-        unexisting_stations = set(stations).difference(
-            set(erosivity["station"].unique())
+    # cumulative rain over all events
+    rain_events = rain_events.assign(
+        all_event_rain_cum=(
+            rain_events["event_rain_cum"].shift(1, fill_value=0.0).cumsum()
         )
-        if unexisting_stations:
-            raise KeyError(
-                f"Station name(s): {unexisting_stations} not part of data set."
-            )
-        erosivity = erosivity.loc[erosivity["station"].isin(stations)]
-    if years is not None:
-        unexisting_years = set(years).difference(set(erosivity["year"].unique()))
-        if unexisting_years:
-            raise KeyError(f"Year(s): {unexisting_years} not part of data set.")
-        erosivity = erosivity.loc[erosivity["year"].isin(years)]
-
-    erosivity = erosivity.groupby(["year", "station"]).aggregate("erosivity_cum").last()
-    erosivity = erosivity.reset_index().sort_values(["station", "year"])
-    erosivity.index = range(len(erosivity))
-    return erosivity
+    )
+
+    # remove events below threshold
+    events = rain_events[round(rain_events["event_rain_cum"], 2) > event_threshold]
+
+    # add cumulative erosivity
+    events = events.assign(erosivity_cum=events["erosivity"].cumsum())
+
+    return events
 
 
-def compute_rainfall_statistics(df_rainfall, df_station_metadata=None):
-    """Compute general statistics for rainfall timeseries.
+def _apply_rfactor(name, group, intensity_method):
+    """Wrapper helper function for parallel execution of erosivity on groups"""
+    df = _compute_erosivity(group, intensity_method)
+    df[["station", "year"]] = name
+    return df
 
-    Statistics (number of records, min, max, median and years data) are
-    computed for each measurement station
+
+def compute_erosivity(rain, intensity_method=maximum_intensity):
+    """Calculate erosivity according to Verstraeten G. for each year/station combination
 
     Parameters
     ----------
-    df_rainfall: pandas.DataFrame
-        See :func:`rfactor.process.load_rain_file`
-    df_station_metadata: pandas.DataFrame
-        Dataframe holding station metadata. This dataframe has one mandatory
-        column:
-
-        - *station* (str): Name or code of the measurement station
-        - *x* (float): X-coordinate of measurement station.
-        - *y* (float): Y-coordinate of measurement station.
+    rain : pandas.DataFrame
+        DataFrame with rainfall time series. Need to contain the following columns:
+
+        - *datetime* (pandas.Timestamp): Time stamp
+        - *rain_mm* (float): Rain in mm
+        - *station* (str): Measurement station identifier
+
+    intensity_method : Callable, default maximum_intensity
+        Function to derive the maximal rain intensity (over 30min).
 
     Returns
     -------
-    df_statistics: pandas.DataFrame
-        Apart from the ``station``, ``x``, ``y`` when ``df_station_metadata`` is
-        provided, the following columns are returned:
-
-        - *year* (list): List of the years fror which data is available for the station.
-        - *records* (int): Total number of records for the station.
-        - *min* (float): Minimal measured value for the station.
-        - *median* (float): Median measured value for the station.
-        - *max* (float): Maximal measured value for the station.
+    all_erosivity: pandas.DataFrame
+        See :func:`rfactor.rfactor._compute_erosivity`, added with
 
+        - *tag* (str): unique tag for year, station-couple.
     """
-    df_rainfall = df_rainfall.sort_values(by="year")
-    df_statistics = (
-        df_rainfall[["year", "station", "rain_mm"]]
-        .groupby("station")
-        .aggregate(
-            {
-                "year": lambda x: sorted(set(x)),
-                "rain_mm": [np.min, np.max, np.median, "count"],
-            }
+    if not {"station", "rain_mm", "datetime"}.issubset(rain.columns):
+        raise RFactorKeyError(
+            "DataFrame should contain 'datetime', 'rain_mm' and 'station' columns."
         )
-    ).reset_index()
-    df_statistics.columns = df_statistics.columns.map("".join)
-    rename_cols = {
-        "year<lambda>": "year",
-        "rain_mmamin": "min",
-        "rain_mmamax": "max",
-        "rain_mmmedian": "median",
-        "rain_mmcount": "records",
-    }
-    df_statistics = df_statistics.rename(columns=rename_cols)
-
-    if df_station_metadata is not None:
-        df_statistics = df_statistics.merge(
-            df_station_metadata, on="station", how="left"
+    if not pd.core.dtypes.common.is_datetime64_any_dtype(rain["datetime"]):
+        raise RFactorTypeError(
+            "The 'datetime' column needs to be of a datetime data type."
         )
-        df_statistics = df_statistics[
-            [
-                "year",
-                "station",
-                "x",
-                "y",
-                "records",
-                "min",
-                "median",
-                "max",
-            ]
-        ]
-    else:
-        df_statistics = df_statistics[["year", "records", "min", "median", "max"]]
+    if not pd.core.dtypes.common.is_string_dtype(rain["station"]):
+        raise RFactorTypeError(
+            "The 'station' column needs to be of a str/object data type."
+        )
+    if not pd.core.dtypes.common.is_float_dtype(rain["rain_mm"]):
+        raise RFactorTypeError("The 'rain_mm' column needs to be of a float type.")
+
+    if ((rain["rain_mm"] == 0).sum() > 0) or (rain["rain_mm"].isnull().sum() > 0):
+        msg = (
+            "Can only accept non-zero/non-NULL timeseries. Removing zero and/or "
+            "NULL-values detected in input 'rain_mm' column."
+        )
+        warnings.warn(msg)
+
+    rain = rain.assign(year=rain["datetime"].dt.year.astype(np.int64))
+
+    if "tag" not in rain.columns:
+        rain = rain.assign(
+            tag=rain["station"].astype(str) + "_" + rain["year"].astype(str)
+        )
+
+    fun_with_method = partial(_apply_rfactor, intensity_method=intensity_method)
+    grouped = rain.groupby(["station", "year"])
+    results = Parallel(n_jobs=mp.cpu_count() - 1)(
+        delayed(fun_with_method)(name, group) for name, group in grouped
+    )
+    all_erosivity = pd.concat(results)
+
+    # couple tag
+    all_erosivity = all_erosivity.merge(
+        rain[["station", "year", "tag"]].drop_duplicates(), on=["station", "year"]
+    )
+    all_erosivity.index = all_erosivity["datetime"]
 
-    return df_statistics
+    return all_erosivity
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rfactor-0.1.1/src/rfactor.egg-info/PKG-INFO` & `rfactor-0.1.2/src/rfactor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfactor
-Version: 0.1.1
+Version: 0.1.2
 Summary: Scripts to compute and analyse the RUSLE R-factor.
 Home-page: https://github.com/cn-ws/rfactor
 Author: Sacha Gobeyn
 Author-email: sacha@fluves.com
 License: LGPL-3
 Project-URL: Documentation, https://cn-ws.github.io/rfactor/
 Project-URL: Source, https://github.com/cn-ws/rfactor
@@ -51,32 +51,42 @@
 > used for the core computations. Since version 0.1.0, a faster Python
 > implementation is provided. Using the version 0.0.x will provide other
 > results compared to version \>0.1.0, as explained in the [package documentation](https://cn-ws.github.io/rfactor/).
 
 Get started
 -----------
 This package makes use of `Python` (and a limited number of dependencies
-such as Pandas and Numpy). Make sure to check out the installation instructions, and follow the example in
+such as Pandas and Numpy). To install:
+
+```
+pip install rfactor
+```
+
+Make sure to check out the installation instructions and follow the example in
 the _Get started section_ of the [package documentation](https://cn-ws.github.io/rfactor/).
 
 Rainfall and erosivity data
 ---------------------------
 
 Any 10 minute ezqolurion input rainfall should work, but input rainfall data for the initial project
 were provided by the Flemish Environment Agency (VMM) and the Royal Meteorological Institute (RMI).
-Teh data from the Flemish Environment Agency (VMM) are available via
+The data from the Flemish Environment Agency (VMM) are available via
 [waterinfo](https://www.waterinfo.be). The input rainfall data from the
 Royal Meteorological Institute (RMI) are not shared in this project.
 Please contact the RMI if you would like to obtain the a copy of the RMI
 rainfall input data.
 
 The erosivity data calculated with the rainfall input data are provided
 by the partners of this project, and are used as test data for analysing
 the R-factor for Flanders.
 
+Code
+----
+The open-source code can be found on [GitHub](https://github.com/cn-ws/rfactor).
+
 Documentation
 -------------
 
 The documentation can be found on the [R-factor documentation
 page](https://cn-ws.github.io/rfactor/index.html).
 
 License
@@ -104,9 +114,7 @@
 ![image](docs/_static/png/fluves_logo.png)
 
 Note
 ----
 
 This project has been set up using PyScaffold 3.2.3. For details and
 usage information on PyScaffold see <https://pyscaffold.org/>.
-
-
```

### Comparing `rfactor-0.1.1/src/rfactor.egg-info/SOURCES.txt` & `rfactor-0.1.2/src/rfactor.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -44,31 +44,34 @@
 docs/notebooks/data/README.md
 docs/notebooks/data/erosivity_belgium.csv
 docs/notebooks/data/files.csv
 docs/notebooks/data/stations.csv
 src/rfactor/__init__.py
 src/rfactor/process.py
 src/rfactor/rfactor.py
+src/rfactor/valid.py
 src/rfactor.egg-info/PKG-INFO
 src/rfactor.egg-info/SOURCES.txt
 src/rfactor.egg-info/dependency_links.txt
 src/rfactor.egg-info/not-zip-safe
 src/rfactor.egg-info/requires.txt
 src/rfactor.egg-info/top_level.txt
 src/rfactor/matlab/core.m
 src/rfactor/matlab/main.m
 tests/__init__.py
 tests/conftest.py
 tests/test_process.py
 tests/test_rfactor.py
+tests/test_valid.py
 tests/data/test_erosivitydata/test_data_maximum_intensity.csv
 tests/data/test_erosivitydata/test_data_maximum_intensity_matlab_clone.csv
 tests/data/test_rainfalldata/P01_001_2018.txt
 tests/data/test_rainfalldata/P01_003_2020.txt
 tests/data/test_rainfalldata/P01_010_2012.txt
 tests/data/test_rainfalldata/P01_010_2016.txt
 tests/data/test_rainfalldata/P05_038_2018.txt
 tests/data/test_rainfalldata/P05_039_2017.txt
 tests/data/test_rainfalldata/P08_018_2012.txt
 tests/data/test_rainfalldata/P09_032_2020.txt
 tests/data/test_rainfalldata/P11_007_2008.txt
-tests/data/test_rainfalldata/P11_024_2012.txt
+tests/data/test_rainfalldata/P11_024_2012.txt
+tests/data/test_rainfalldata_vmm_format/P01_010.CSV
```

### Comparing `rfactor-0.1.1/tests/conftest.py` & `rfactor-0.1.2/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import os
 import textwrap
 from pathlib import Path
 
 import pandas as pd
 import pytest
 
-from rfactor.process import load_rain_file, load_rain_folder
+from rfactor.process import (
+    load_rain_file,
+    load_rain_file_matlab_legacy,
+    load_rain_folder,
+)
 
 CURRENT_DIR = Path(os.path.dirname(__file__))
 
 
 @pytest.fixture()
 def rain_benchmark_closure():
     """Rain data used for benchmark reference case"""
 
     def rain_benchmark_year(station, year):
         """Get benchmark data for given year and station"""
         rain = load_rain_file(
-            CURRENT_DIR / "data" / "test_rainfalldata" / f"{station}_{year}.txt"
+            CURRENT_DIR / "data" / "test_rainfalldata" / f"{station}_{year}.txt",
+            load_rain_file_matlab_legacy,
         )
         return rain
 
     return rain_benchmark_year
 
 
 @pytest.fixture()
@@ -68,14 +73,20 @@
         """
     with open(example_rain_path, "w") as rain:
         rain.write(textwrap.dedent(example_rain_data))
     return example_rain_path
 
 
 @pytest.fixture()
+def rain_data_file_csv_vmm():
+    "Example rainfall CSV data file"
+    return CURRENT_DIR / "data" / "test_rainfalldata_vmm_format" / "P01_010.CSV"
+
+
+@pytest.fixture()
 def rain_data_folder(tmp_path):
     """Example rainfall data file"""
     example_rain_path = tmp_path / "rain"
     example_rain_path.mkdir()
 
     # create example data files for multiple years
     for idx, year in enumerate([2020, 2021]):
@@ -88,14 +99,31 @@
         with open(rain_file, "w") as rain:
             rain.write(textwrap.dedent(example_rain_data))
 
     return example_rain_path
 
 
 @pytest.fixture()
+def data_folder_non_existing(tmp_path):
+    """Example rainfall data file"""
+    example_rain_path_non_existing = tmp_path / "non-existing"
+
+    return example_rain_path_non_existing
+
+
+@pytest.fixture()
+def data_folder_empty(tmp_path):
+    """Example rainfall data file"""
+    example_rain_path_empty = tmp_path / "empty"
+    example_rain_path_empty.mkdir()
+
+    return example_rain_path_empty
+
+
+@pytest.fixture()
 def dummy_rain():
     """Dummy rainfall data according to required input data."""
     rain = [
         0.27,
         0.02,
         0.48,
         0.22,
```

### Comparing `rfactor-0.1.1/tests/data/test_erosivitydata/test_data_maximum_intensity.csv` & `rfactor-0.1.2/tests/data/test_erosivitydata/test_data_maximum_intensity.csv`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/tests/data/test_erosivitydata/test_data_maximum_intensity_matlab_clone.csv` & `rfactor-0.1.2/tests/data/test_erosivitydata/test_data_maximum_intensity_matlab_clone.csv`

 * *Files identical despite different names*

### Comparing `rfactor-0.1.1/tests/test_process.py` & `rfactor-0.1.2/tests/test_process.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 import pandas as pd
 import pytest
 
 from rfactor.process import (
     _check_path,
     _days_since_start_year,
     _extract_metadata_from_file_path,
+    compute_diagnostics,
     compute_rainfall_statistics,
     get_rfactor_station_year,
     load_rain_file,
+    load_rain_file_csv_vmm,
+    load_rain_file_matlab_legacy,
     load_rain_folder,
     write_erosivity_data,
 )
 
 
 def test_days_since_last_year_float():
     """Moment of the day is translated as decimal number."""
@@ -76,86 +79,125 @@
     with pytest.raises(TypeError) as excinfo:
         _check_path(np.array([1, 2]))
     assert " should be a pathlib.Path" in str(excinfo.value)
 
 
 def test_load_rain_file(rain_data_file):
     """Valid rainfall data should be parsed to rain DataFrame"""
-    rainfall_data = load_rain_file(rain_data_file)
+    rainfall_data = load_rain_file(rain_data_file, load_rain_file_matlab_legacy)
     assert isinstance(rainfall_data, pd.DataFrame)
+
     assert list(rainfall_data.columns) == [
-        "minutes_since",
-        "rain_mm",
         "datetime",
         "station",
+        "rain_mm",
         "year",
         "tag",
     ]
     assert list(rainfall_data["station"].unique()) == ["station_name"]
     assert list(rainfall_data.iloc[0].values) == [
-        1,
-        1.0,
         pd.to_datetime("2021-01-01 00:01:00"),
         "station_name",
+        1.0,
         2021,
         "station_name_2021",
     ]
     assert list(rainfall_data.iloc[-1].values) == [
-        525599,
-        10.00,
         pd.to_datetime("2021-12-31 23:59:00"),
         "station_name",
+        10.00,
         2021,
         "station_name_2021",
     ]
 
 
+def test_compute_diagnostics(rain_data_file_csv_vmm):
+    """Test compute diagnostics funf or vmm input file"""
+    rain_data = load_rain_file(rain_data_file_csv_vmm, load_rain_file_csv_vmm)
+    diagnostics = compute_diagnostics(rain_data)
+
+    assert set(diagnostics.columns) == {
+        "station",
+        "year",
+        "coverage",
+        1,
+        2,
+        3,
+        4,
+        5,
+        6,
+        7,
+        8,
+        9,
+        10,
+        11,
+        12,
+    }
+    assert diagnostics["coverage"].iloc[0] == pytest.approx(0.972928)
+    assert (
+        diagnostics[[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]].iloc[0].to_list()
+        == [0] * 2 + [1] * 10
+    )
+
+
 def test_load_rain_file_with_folder(rain_data_folder):
     """When input is a file, should return ValueError to user"""
+
     with pytest.raises(ValueError) as excinfo:
-        load_rain_file(rain_data_folder)
+        load_rain_file(rain_data_folder, load_rain_file_matlab_legacy)
     assert "a file instead of a directory" in str(excinfo.value)
 
 
-def test_load_rain_folder(rain_data_folder):
+def test_load_rain_folder(
+    rain_data_folder, data_folder_non_existing, data_folder_empty
+):
     """Rainfall data should be parsed to rain DataFrame
     when loading multiple files adding a year and tag column"""
-    rainfall_data = load_rain_folder(rain_data_folder)
+    rainfall_data = load_rain_folder(rain_data_folder, load_rain_file_matlab_legacy)
     assert isinstance(rainfall_data, pd.DataFrame)
     assert list(rainfall_data.columns) == [
-        "minutes_since",
-        "rain_mm",
         "datetime",
         "station",
+        "rain_mm",
         "year",
         "tag",
     ]
     assert list(rainfall_data["station"].unique()) == ["station_0", "station_1"]
     assert list(rainfall_data.iloc[0].values) == [
-        1,
-        1.0,
         pd.to_datetime("2020-01-01 00:01:00"),
         "station_0",
+        1.0,
         2020,
         "station_0_2020",
     ]
     assert list(rainfall_data.iloc[-1].values) == [
-        525599,
-        10.00,
         pd.to_datetime("2021-12-31 23:59:00"),
         "station_1",
+        10.00,
         2021,
         "station_1_2021",
     ]
+    with pytest.raises(FileNotFoundError) as excinfo:
+        load_rain_folder(data_folder_non_existing, load_rain_file_matlab_legacy)
+    assert f"Input folder '{data_folder_non_existing}' does not exists." in str(
+        excinfo.value
+    )
+
+    with pytest.raises(FileNotFoundError) as excinfo:
+        load_rain_folder(data_folder_empty, load_rain_file_matlab_legacy)
+    assert (
+        f"Input folder '{data_folder_empty}' does not contain any 'txt'-files."
+        in str(excinfo.value)
+    )
 
 
 def test_load_rain_folder_with_file(rain_data_file):
     """When input is a file, should return ValueError to user"""
     with pytest.raises(ValueError) as excinfo:
-        load_rain_folder(rain_data_file)
+        load_rain_folder(rain_data_file, load_rain_file_matlab_legacy)
     assert "a directory instead of a file" in str(excinfo.value)
 
 
 def test_write_erosivity(dummy_erosivity, tmpdir):
     """Check written legacy matlab format files output"""
     erosivity = dummy_erosivity
 
@@ -227,21 +269,21 @@
     with pytest.raises(KeyError) as excinfo:
         get_rfactor_station_year(dummy_erosivity, years=years_of_interest)
     assert "1991" in str(excinfo.value)
 
 
 def test_rainfall_statistics(rain_data_folder):
     """"""
-    rainfall_data = load_rain_folder(rain_data_folder)
+    rainfall_data = load_rain_folder(rain_data_folder, load_rain_file_matlab_legacy)
     rf_stats = compute_rainfall_statistics(rainfall_data)
     assert set(rf_stats.columns) == set(["year", "records", "min", "median", "max"])
     assert isinstance(rf_stats["year"][0], list)
     assert rf_stats["records"].dtype == np.int64
 
 
 def test_rainfall_statistics_with_metadata(rain_data_folder, station_metadata):
     """Extend rain stats with metadata"""
-    rainfall_data = load_rain_folder(rain_data_folder)
+    rainfall_data = load_rain_folder(rain_data_folder, load_rain_file_matlab_legacy)
     rf_stats = compute_rainfall_statistics(rainfall_data, station_metadata)
     assert set(rf_stats.columns) == set(
         ["year", "station", "x", "y", "records", "min", "median", "max"]
     )
```

### Comparing `rfactor-0.1.1/tests/test_rfactor.py` & `rfactor-0.1.2/tests/test_rfactor.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,28 @@
         }
     )
     with pytest.raises(RFactorInputError) as excinfo:
         _compute_erosivity(df, maximum_intensity)
     assert "contain data of a single year." in str(excinfo.value)
 
 
+def test_compute_0_or_NULL_rain_mm_warning(dummy_rain, recwarn):
+    """Test if 0 and NUll in 'rain_mm' column throws warning"""
+    df = dummy_rain.copy()
+    df.loc[[0, 1, 2], "rain_mm"] = [0, np.nan, 0]
+    compute_erosivity(df, maximum_intensity)
+    # test warning
+    w = recwarn.pop(UserWarning)
+    assert (
+        str(w.message)
+        == "Can only accept non-zero/non-NULL timeseries. Removing zero and/or "
+        "NULL-values detected in input 'rain_mm' column."
+    )
+
+
 def test_apply_rfactor(rain_benchmark_closure):
     """apply_rfactor adds the station/year data to dataframe"""
     station, year = "P01_001", 2018
     rain = rain_benchmark_closure(station, year)
     erosivity_support_func = _compute_erosivity(rain, maximum_intensity)
     erosivity_apply_rfactor = _apply_rfactor((station, year), rain, maximum_intensity)
```

### Comparing `rfactor-0.1.1/tox.ini` & `rfactor-0.1.2/tox.ini`

 * *Files identical despite different names*

