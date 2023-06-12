# Comparing `tmp/hyswap-0.0.0a0.tar.gz` & `tmp/hyswap-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyswap-0.0.0a0.tar", last modified: Wed Jun  7 19:49:11 2023, max compression
+gzip compressed data, was "hyswap-0.0.1.tar", last modified: Mon Jun 12 12:25:06 2023, max compression
```

## Comparing `hyswap-0.0.0a0.tar` & `hyswap-0.0.1.tar`

### file list

```diff
@@ -1,54 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:49:11.841919 hyswap-0.0.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:49:11.837919 hyswap-0.0.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:49:11.837919 hyswap-0.0.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/DISCLAIMER.md
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-07 19:49:11.841919 hyswap-0.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/code.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:49:11.837919 hyswap-0.0.0a0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:49:11.837919 hyswap-0.0.0a0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/docs/source/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:49:11.837919 hyswap-0.0.0a0/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/docs/source/examples/cumulative_hydrograph_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/docs/source/examples/flow_duration_curve_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/docs/source/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/docs/source/examples/raster_hydrograph_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/docs/source/examples/streamflow_duration_hydrograph_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:49:11.841919 hyswap-0.0.0a0/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)    28371 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/docs/source/reference/hyswap.png
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/docs/source/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:49:11.841919 hyswap-0.0.0a0/hyswap/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/hyswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-07 19:49:11.000000 hyswap-0.0.0a0/hyswap/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/hyswap/cumulative.py
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/hyswap/exceedance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/hyswap/percentiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/hyswap/rasterhydrograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/hyswap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:49:11.841919 hyswap-0.0.0a0/hyswap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-07 19:49:11.000000 hyswap-0.0.0a0/hyswap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-07 19:49:11.000000 hyswap-0.0.0a0/hyswap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:49:11.000000 hyswap-0.0.0a0/hyswap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 19:49:11.000000 hyswap-0.0.0a0/hyswap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 19:49:11.000000 hyswap-0.0.0a0/hyswap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:49:11.841919 hyswap-0.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:49:11.841919 hyswap-0.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/tests/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/tests/test_exceedance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/tests/test_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/tests/test_rasterhydrograph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-06-07 19:48:37.000000 hyswap-0.0.0a0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.385591 hyswap-0.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-12 12:24:31.000000 hyswap-0.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-12 12:24:31.000000 hyswap-0.0.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-12 12:24:31.000000 hyswap-0.0.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-12 12:24:31.000000 hyswap-0.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-12 12:24:31.000000 hyswap-0.0.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-12 12:24:31.000000 hyswap-0.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-12 12:24:31.000000 hyswap-0.0.1/DISCLAIMER.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-12 12:24:31.000000 hyswap-0.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-12 12:25:06.385591 hyswap-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-12 12:24:31.000000 hyswap-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-12 12:24:31.000000 hyswap-0.0.1/code.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/examples/cumulative_hydrograph_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/examples/flow_duration_curve_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/examples/raster_hydrograph_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/examples/streamflow_duration_hydrograph_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/docs/source/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/meta/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/meta/disclaimer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/meta/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.381591 hyswap-0.0.1/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)    28371 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/reference/hyswap.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-12 12:24:31.000000 hyswap-0.0.1/docs/source/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.385591 hyswap-0.0.1/hyswap/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 12:25:06.000000 hyswap-0.0.1/hyswap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/exceedance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/rasterhydrograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-06-12 12:24:31.000000 hyswap-0.0.1/hyswap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.385591 hyswap-0.0.1/hyswap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-12 12:25:06.000000 hyswap-0.0.1/hyswap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-12 12:25:06.000000 hyswap-0.0.1/hyswap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:25:06.000000 hyswap-0.0.1/hyswap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 12:25:06.000000 hyswap-0.0.1/hyswap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 12:25:06.000000 hyswap-0.0.1/hyswap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-12 12:24:31.000000 hyswap-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-12 12:24:31.000000 hyswap-0.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 12:24:31.000000 hyswap-0.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:25:06.385591 hyswap-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:24:31.000000 hyswap-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:25:06.385591 hyswap-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-12 12:24:31.000000 hyswap-0.0.1/tests/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-12 12:24:31.000000 hyswap-0.0.1/tests/test_exceedance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-12 12:24:31.000000 hyswap-0.0.1/tests/test_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-12 12:24:31.000000 hyswap-0.0.1/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-06-12 12:24:31.000000 hyswap-0.0.1/tests/test_rasterhydrograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-06-12 12:24:31.000000 hyswap-0.0.1/tests/test_utils.py
```

### Comparing `hyswap-0.0.0a0/.github/workflows/build.yml` & `hyswap-0.0.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/.github/workflows/docs.yml` & `hyswap-0.0.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/.github/workflows/pypi.yml` & `hyswap-0.0.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/.gitignore` & `hyswap-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/.gitlab-ci.yml` & `hyswap-0.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/CONTRIBUTING.md` & `hyswap-0.0.1/CONTRIBUTING.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,17 @@
       - [Style](#style)
       - [Doc-strings](#doc-strings)
   - [Documentation](#documentation)
     - [Contributing to the Documentation](#contributing-to-the-documentation)
   - [Feedback and Feature Requests](#feedback-and-feature-requests)
     - [Submitting Feedback](#submitting-feedback)
     - [Feature Requests](#feature-requests)
+  - [Merge Workflow (USGS Maintainers)](#merge-workflow-usgs-maintainers)
+    - [Contributions on GitLab](#contributions-on-gitlab)
+    - [Contributions on GitHub](#contributions-on-github)
   - [Acknowledgements](#acknowledgements)
 
 ---
 
 ## Bugs
 
 ### Reporting Bugs
@@ -146,9 +149,34 @@
 Please be sure to:
 * Explain in detail how it would work, possibly with pseudo-code or an example use-case
 * Keep the scope of the proposed feature as narrow as possible
 * Make clear whether you would like to implement this feature, you need help devising the implementation, or you are unable to implement the feature yourself but would like it as a user
 
 ---
 
+## Merge Workflow (USGS Maintainers)
+
+This code repository exists (and is publicly available) on both the USGS GitLab platform (code.usgs.gov) and within the DOI-USGS organization on GitHub (github.com/DOI-USGS).
+The canonical 'source' repository is on GitLab, all commits on all branches are automatically mirrored from the GitLab repository to the GitHub repository.
+To maintain this mirroring and keep the two repositories *exactly* the same (i.e., identical commit histories), there is a specific workflow that must be followed when merging contributions to the project.
+
+Whether contributions are made via GitLab or GitHub, they should follow the code contribution guidelines outlined above.
+Below, the specific steps that should be taken to merge or integrate these contributions into the `hyswap` project are outlined.
+
+### Contributions on GitLab
+When contributions are proposed on GitLab via merge requests, they can be discussed, altered, and ultimately merged on that platform.
+There is no special action that needs to be taken on behalf of the code maintainers and developers in this case.
+
+### Contributions on GitHub
+When contributions are proposed on GitHub via pull requests, the review and discussion of the changes can take place within the pull request as usual.
+However, **the pull request cannot be merged on GitHub**, as this throws off the automatic mirroring which goes from GitLab to GitHub.
+Once a pull request has been reviewed and "approved" on GitHub, a USGS code maintainer or developer (someone with push access to the GitLab repository) has to take action to **push the proposed code to GitLab**.
+This process involves the maintainer having a local clone of the `hyswap` project with remote connections to both the GitLab and GitHub repositories.
+Locally, the maintainer has to checkout the proposed code from the approved pull request on GitHub.
+Then they can push those changes to the *GitLab* repository by specifying the remote repository and "main" branch on GitLab.
+Once the changes are pushed to GitLab, they will be automatically mirrored back to GitHub.
+In this process, the GitHub pull request will get closed, and the code commits will be credited to the appropriate authors on GitHub too, all while maintaining the mirror and keeping the GitHub and GitLab repositories identical.
+
+---
+
 ## Acknowledgements
 This document was adapted from the `cookiecutter` project's [CONTRIBUTING file](https://github.com/audreyr/cookiecutter/blob/master/CONTRIBUTING.rst) and the `dataretrieval` project's [CONTRIBUTING file](https://github.com/DOI-USGS/dataretrieval-python/blob/master/CONTRIBUTING.md).
```

### Comparing `hyswap-0.0.0a0/DISCLAIMER.md` & `hyswap-0.0.1/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/LICENSE.md` & `hyswap-0.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/PKG-INFO` & `hyswap-0.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyswap
-Version: 0.0.0a0
+Version: 0.0.1
 Summary: Analysis of surface water data.
 Author-email: USGS <comptools@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United States because it contains materials that originally came from the United States Geological Survey, an agency of the United States Department of Interior.
         For more information, see the official USGS copyright policy at https://www.usgs.gov/information-policies-and-instructions/copyrights-and-credits.
@@ -33,51 +33,70 @@
 Project-URL: repository, https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap.git
 Keywords: USGS,water data,analysis
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# hyswap
+# hyswap - HYdrologic Surface Water Analysis Package
 
 [![USGS-category-image](https://img.shields.io/badge/USGS-Core-green.svg)](https://owi.usgs.gov/R/packages.html#core)
 [![pipeline-status-image](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/badges/main/pipeline.svg)](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/-/commits/main)
 [![coverage-report-image](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/badges/main/coverage.svg)](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/-/commits/main)
+[![PyPI version](https://badge.fury.io/py/hyswap.svg)](https://badge.fury.io/py/hyswap)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyswap)
+
+## Overview
+
+`hyswap` (HYdrologic Surface Water Analysis Package), is a Python package which provides a set of functions for manipulating and visualizing USGS water data.
+Specifically, a number of functions for calculating statistics (e.g., exceedance probabilities, daily historic percentiles) and generating related plots (e.g., flow duration curves, streamflow duration hydrographs) are available.
+These methods are provided in a modular fashion as individual functions, and are designed to give the user flexibility in implementation.
 
 ### Project Documentation
 
-`hyswap` documentation is available at: [Link](https://rconnect.usgs.gov/hyswap-docs/html/)
+For more information, visit the `hyswap` [documentation](https://doi-usgs.github.io/hyswap/).
 
 ## Installation
 
-### User Installation
+### User Installation via `pip`
 
-User installation is possible from source right now.
-First you will need to clone the repository.
+One-liner to install `hyswap` via `pip`:
+
+```bash
+pip install hyswap
+```
+
+*Note:* `hyswap` has 4 dependencies right now, `numpy`, `pandas`, `scipy`, and `matplotlib`, these will be installed automatically when installing the package via `pip`.
+
+### User Installation From Source
+
+To install `hyswap` from source, first you will need to clone the repository.
 Next, from the root of the repository, run the following commands:
 
 ```bash
 pip install -r requirements.txt
 pip install .
 ```
 
 ### Developer Installation
 
-Developer installation is possible from source right now.
+Developer installation should be performed from source.
 First you will need to clone the repository.
 Next, from the root of the repository, run the following commands:
 
 ```bash
 pip install -r requirements.txt
 pip install -r requirements-dev.txt
 pip install -e .
 ```
 
 ### Testing and Building Documentation Locally
 
+To test the code and building and test the documentation locally, you must have cloned the source repository, follow the instructions above for a "developer installation" first.
+
 To test the package locally, run the following command from the root of the repository:
 
 ```bash
 pytest
 ```
 
 To build the documentation locally, run the following commands from the root of the repository:
```

### Comparing `hyswap-0.0.0a0/code.json` & `hyswap-0.0.1/code.json`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/docs/Makefile` & `hyswap-0.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/docs/source/conf.py` & `hyswap-0.0.1/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,16 @@
 # doctest
 doctest_global_setup = '''
 import hyswap
 from hyswap import exceedance
 from hyswap import rasterhydrograph
 from hyswap import utils
 from hyswap import percentiles
+from hyswap import cumulative
+from hyswap import plots
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import dataretrieval
 '''
 
 # mpl plots - metadata for the documentation plots
@@ -127,10 +129,15 @@
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 # -- Options for linkcheck -------------------------------------------
 
 # Links to not "check" because they are problematic for the link checker
-# linkcheck_ignore = [
-#     r'https://google.com'
-# ]
+linkcheck_ignore = [
+    r'https://doi.org/10.3133/wsp1542A'
+]
+
+linkcheck_exclude_documents = [
+    r'meta/disclaimer*',
+    r'meta/contributing*'
+]
```

### Comparing `hyswap-0.0.0a0/docs/source/reference/hyswap.png` & `hyswap-0.0.1/docs/source/reference/hyswap.png`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/docs/source/reference/index.rst` & `hyswap-0.0.1/docs/source/reference/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -37,7 +37,21 @@
 
 Percentile Calculation Functions
 --------------------------------
 
 .. automodule:: hyswap.percentiles
     :members:
     :special-members:
+
+Cumulative Calculation Functions
+--------------------------------
+
+.. automodule:: hyswap.cumulative
+    :members:
+    :special-members:
+
+Plotting Functions
+------------------
+
+.. automodule:: hyswap.plots
+    :members:
+    :special-members:
```

### Comparing `hyswap-0.0.0a0/hyswap/cumulative.py` & `hyswap-0.0.1/hyswap/cumulative.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,22 +43,16 @@
     .. doctest::
 
         >>> df = pd.DataFrame({
         ...     "date": pd.date_range("2000-01-01", "2000-12-31"),
         ...     "data": np.arange(366)})
         >>> results = cumulative.calculate_daily_cumulative_values(
         ...     df, "data", date_column_name="date")
-        >>> results.head()
-                    year  doy  cumulative
-        date
-        2000-01-01  2000    1           0
-        2000-01-02  2000    2           1
-        2000-01-03  2000    3           3
-        2000-01-04  2000    4           6
-        2000-01-05  2000    5          10
+        >>> results.columns.tolist()
+        ['index_year', 'index_doy', 'cumulative']
     """
     # set date index, add day/year columns with function
     df = define_year_doy_columns(df, date_column_name=date_column_name,
                                  year_type=year_type, clip_leap_day=True)
     # get unique years in the data
     years = df['index_year'].unique()
     # make a dataframe to hold cumulative values for each year
```

### Comparing `hyswap-0.0.0a0/hyswap/exceedance.py` & `hyswap-0.0.1/hyswap/exceedance.py`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/hyswap/percentiles.py` & `hyswap-0.0.1/hyswap/percentiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,16 +125,16 @@
         ...     df, "00060_Mean")
         >>> len(results.index)  # 366 days in a leap year
         366
         >>> len(results.columns)  # 8 default percentiles
         8
     """
     # define year and day of year columns and convert date column to datetime
-    # if necessary - copy input df so it is not modified by the function
-    df = define_year_doy_columns(df.copy(), date_column_name=date_column_name,
+    # if necessary
+    df = define_year_doy_columns(df, date_column_name=date_column_name,
                                  year_type=year_type, clip_leap_day=True)
     # based on date, get min and max day of year available
     min_day = np.nanmax((1, df.index.dayofyear.min()))
     max_day = np.nanmin((366, df.index.dayofyear.max() + 1))
     # make temporal index
     t_idx = np.arange(min_day, max_day)
     # initialize a DataFrame to hold percentiles by day of year
@@ -148,15 +148,33 @@
         meta = calculate_metadata(data)
 
         # only calculate data if there are at least min_years of data
         if meta['n_years'] >= min_years:
             # calculate percentiles for the day of year and add to DataFrame
             percentiles_by_day.loc[t_idx == doy, :] = \
                 calculate_fixed_percentile_thresholds(
-                data, percentiles=percentiles, method=method, **kwargs)
+                    data, percentiles=percentiles, method=method, **kwargs)
         else:
             # if there are not at least 10 years of data,
             # set percentiles to NaN
             percentiles_by_day.loc[t_idx == doy, :] = np.nan
 
+    # replace index with multi-index of doy_index and month-day values
+    # month_day values
+    month_day = pd.to_datetime(
+        percentiles_by_day.index, format='%j').strftime('%m-%d')
+    # doy_index values
+    doy_index = percentiles_by_day.index.values
+    if year_type == 'water':
+        doy_index = doy_index - 273
+        doy_index[doy_index < 1] += 365
+    elif year_type == 'climate':
+        doy_index = doy_index - 90
+        doy_index[doy_index < 1] += 365
+    percentiles_by_day.index = pd.MultiIndex.from_arrays(
+        [doy_index, month_day], names=['doy', 'month-day'])
+
+    # sort percentiles by index
+    percentiles_by_day.sort_index(inplace=True)
+
     # return percentiles by day of year
     return percentiles_by_day
```

### Comparing `hyswap-0.0.0a0/hyswap/rasterhydrograph.py` & `hyswap-0.0.1/hyswap/rasterhydrograph.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,42 +81,54 @@
         365
     """
     # check inputs, set date to index, define year/doy columns
     df = _check_inputs(df, data_column_name, date_column_name,
                        data_type, year_type, begin_year, end_year)
 
     # calculate the date range
-    date_range = _calculate_date_range(df, begin_year, end_year)
+    date_range = _calculate_date_range(df, year_type, begin_year, end_year)
 
     # format date_range as YYYY-MM-DD
     date_range = date_range.strftime('%Y-%m-%d')
 
     # set data type
     data_type = _set_data_type(data_type)
 
     # make output data frame
     # calculation of rolling mean is done on the data column
     df_out = rolling_average(df, data_column_name, data_type, **kwargs)
 
     # convert date index to YYYY-MM-DD format
     df_out.index = df_out.index.strftime('%Y-%m-%d')
 
-    # fill in missing dates as nan values to complete the years
-    df_out = df_out.reindex(index=date_range)
+    # expand data frame to include all dates in date_range
+    df_out = df_out.reindex(date_range)
 
     # convert date index to datetime format
     df_out.index = pd.to_datetime(df_out.index)
 
-    # adjust for leap years by removing NaN rows
-    df_out = df_out.dropna(axis=0, how='all')
+    # re-define year and doy columns
+    df_out = define_year_doy_columns(df_out, year_type=year_type,
+                                     clip_leap_day=True)
+
+    # sort by date
+    df_out = df_out.sort_index()
+
+    # define future columns as doy_month-day
+    fut_col = [str(df_out['index_doy'][i]) + '-' +
+               str(df_out['index_month_day'][i])
+               for i in range(len(df_out['index_doy'].unique()))]
 
     # set index to year and day of year columns
     df_out = df_out.pivot(index='index_year', columns='index_doy',
                           values=data_column_name)
 
+    # rename columns to be index_doy, index_month_day
+    df_out.columns = fut_col
+
     # reverse order of the index so year order matches legacy Water Watch
     df_out = df_out.iloc[::-1]
 
     # remove all NaN columns and rows
     df_out = df_out.dropna(axis=1, how='all')
     df_out = df_out.dropna(axis=0, how='all')
 
@@ -212,43 +224,54 @@
     # define year and doy columns and set index as date col if needed
     df = define_year_doy_columns(df, date_column_name, year_type,
                                  clip_leap_day=True)
 
     return df
 
 
-def _calculate_date_range(df, begin_year, end_year):
+def _calculate_date_range(df, year_type, begin_year, end_year):
     """Private function to calculate the date range and set the index.
 
     Parameters
     ----------
     df : pandas.DataFrame
         The data to format. Must have a date column or the index must be the
         date values.
+    year_type : str
+        The type of year to use. Must be one of 'calendar', 'water', or
+        'climate'.
     begin_year : int, None
         The first year to include in the data. If None, the first year in
         the data will be used.
     end_year : int, None
         The last year to include in the data. If None, the last year in the
         data will be used.
 
     Returns
     -------
     date_range : pandas.DatetimeIndex
         The date range.
     """
-    # set begin year
+    # set begin/end year if not provided
     if begin_year is None:
-        begin_year = df['index_year'].min()
-    begin_date = df.loc[df['index_year'] == begin_year].index.min()
-
-    # set end year
+        begin_year = df.index.year.min()
     if end_year is None:
-        end_year = df['index_year'].max()
-    end_date = df.loc[df['index_year'] == end_year].index.max()
+        end_year = df.index.year.max()
+    # calendar year from Jan 1 to Dec 31
+    if year_type == 'calendar':
+        begin_date = pd.to_datetime(str(begin_year) + '-01-01')
+        end_date = pd.to_datetime(str(end_year) + '-12-31')
+    # water year from Oct 1 to Sep 30
+    elif year_type == 'water':
+        begin_date = pd.to_datetime(str(begin_year-1) + '-10-01')
+        end_date = pd.to_datetime(str(end_year) + '-09-30')
+    # climate year from Apr 1 to Mar 31
+    elif year_type == 'climate':
+        begin_date = pd.to_datetime(str(begin_year-1) + '-04-01')
+        end_date = pd.to_datetime(str(end_year) + '-03-31')
 
     # set date range
     date_range = pd.date_range(begin_date, end_date)
 
     return date_range
```

### Comparing `hyswap-0.0.0a0/hyswap/utils.py` & `hyswap-0.0.1/hyswap/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility functions for hyswap."""
+import pandas as pd
 
 
 def filter_approved_data(data, filter_column=None):
     """Filter a dataframe to only return approved "A" (or "A, e") data.
 
     Parameters
     ----------
@@ -215,15 +216,15 @@
     meta["n_lows"] = len(data.loc[data <= 0.01])
 
     return meta
 
 
 def define_year_doy_columns(df, date_column_name=None, year_type='calendar',
                             clip_leap_day=False):
-    """Function to add year and day of year columns to a DataFrame.
+    """Function to add year, day of year, and month-day columns to a DataFrame.
 
     Parameters
     ----------
     df : pandas.DataFrame
         DataFrame containing data to filter. Expects datetime information to be
         available in the index or in a column named `date_column_name`.
 
@@ -243,16 +244,16 @@
 
     clip_leap_day : bool, optional
         If True, February 29 is removed from the DataFrame. Default is False.
 
     Returns
     -------
     df : pandas.DataFrame
-        DataFrame with year and day of year columns added. Also makes the
-        date_column_name the index of the DataFrame.
+        DataFrame with year, day of year, and month-day columns added. Also
+        makes the date_column_name the index of the DataFrame.
     """
     # set the df index
     if date_column_name is not None:
         df = df.set_index(date_column_name)
     # check that year_type is valid
     if year_type not in ['calendar', 'water', 'climate']:
         raise ValueError(
@@ -283,14 +284,16 @@
         # adjust Apr 1 to be day 1 of climate year for leap and non-leap years
         df.loc[df.index.is_leap_year & (df.index.month >= 4),
                'index_doy'] -= 91
         df.loc[~df.index.is_leap_year & (df.index.month >= 4),
                'index_doy'] -= 90
         # adjust Jan 1 to be day 276 of climate year for all years
         df.loc[df.index.month < 4, 'index_doy'] += 275
+    # add month and day columns
+    df['index_month_day'] = df.index.strftime('%m-%d')
     # clip leap year and adjustment
     if clip_leap_day:
         df = leap_year_adjustment(df, year_type=year_type)
     # sort the df by year and day of year
     df = df.sort_values(['index_year', 'index_doy'])
     return df
 
@@ -331,7 +334,99 @@
                (df.index.month > 2) &
                (df.index.month < 10), 'index_doy'] -= 1
     elif year_type == 'climate':
         df.loc[df.index.is_leap_year &
                (df.index.month > 2) &
                (df.index.month < 4), 'index_doy'] -= 1
     return df
+
+
+def munge_nwis_stats(df, source_pct_col=None, target_pct_col=None,
+                     year_type='calendar'):
+    """Function to munge and reformat NWIS statistics data.
+
+    This is a utility function that exists to help munge NWIS percentile data
+    served via the NWIS statistics web service. This function is intended to
+    be used on Python dataretrieval dataframe returns for the nwis.get_stats()
+    function for "daily" data, a single site, and a single parameter code.
+
+    df : pandas.DataFrame
+        DataFrame containing NWIS statistics data retrieved from the statistics
+        web service. Assumed to come in as a dataframe retrieved with a
+        package like dataretrieval or similar.
+    source_pct_col : list, optional
+        List of column names to use as the source percentiles. If None, the
+        values are assumed to correspond to the 0, 5, 10, 25, 75, 90, 95,
+        and 100 percentiles in the NWIS statistics service return.
+    target_pct_col : list, optional
+        List of column names to use as the target percentiles. If None, then
+        integer values are used as the column names corresponding to the
+        default source values.
+    year_type : str, optional
+        The type of year to use. Must be one of 'calendar', 'water', or
+        'climate'. Default is 'calendar' which starts the year on January 1
+        and ends on December 31. 'water' starts the year on October 1 and
+        ends on September 30 of the following year which is the "water year".
+        For example, October 1, 2010 to September 30, 2011 is "water year
+        2011". 'climate' years begin on April 1 and end on March 31 of the
+        following year, they are numbered by the ending year. For example,
+        April 1, 2010 to March 31, 2011 is "climate year 2011".
+
+    Returns
+    -------
+    df_slim : pandas.DataFrame
+        DataFrame containing munged and reformatted NWIS statistics data.
+        Reformatting is for use with the hyswap package plotting function for
+        duration hydrographs with statistical information in background of
+        the plot.
+
+    Examples
+    --------
+    Get some NWIS statistics data.
+
+    .. doctest::
+
+        >>> df, md = dataretrieval.nwis.get_stats(
+        ...     "03586500", parameterCd="00060", statReportType="daily")
+
+    Then apply the function to munge the data.
+
+    .. doctest::
+
+        >>> df = utils.munge_nwis_stats(df)
+        >>> df.shape
+        (366, 8)
+    """
+    # set defaults
+    if source_pct_col is None:
+        source_pct_col = ['min_va', 'p05_va', 'p10_va', 'p25_va',
+                          'p75_va', 'p90_va', 'p95_va', 'max_va']
+    if target_pct_col is None:
+        target_pct_col = [0, 5, 10, 25, 75, 90, 95, 100]
+    # check lengths of lists for column names
+    if len(source_pct_col) != len(target_pct_col):
+        raise ValueError('source_pct_col and target_pct_col must be the same '
+                         'length')
+    # rename date columns
+    df.rename(columns={'month_nu': 'month', 'day_nu': 'day', 'end_yr': 'year'},
+              inplace=True)
+    # make end year 2020 for leap year
+    df['year'] = 2020
+    # construct date column
+    df['date'] = pd.to_datetime(df[['day', 'month', 'year']])
+    # set doy_index and month-day as multi-index
+    month_day = df['date'].dt.strftime('%m-%d')
+    doy_index = df['date'].dt.dayofyear
+    if year_type == 'water':
+        doy_index = doy_index - 273
+        doy_index[doy_index < 1] += 365
+    elif year_type == 'climate':
+        doy_index = doy_index - 90
+        doy_index[doy_index < 1] += 365
+    df.index = pd.MultiIndex.from_arrays(
+        [doy_index, month_day], names=['doy', 'month-day'])
+    # slim down to just the columns used for the plot
+    df_slim = df[source_pct_col]
+    # rename columns
+    df_slim.columns = target_pct_col
+    # return the dataframe
+    return df_slim
```

### Comparing `hyswap-0.0.0a0/hyswap.egg-info/PKG-INFO` & `hyswap-0.0.1/hyswap.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyswap
-Version: 0.0.0a0
+Version: 0.0.1
 Summary: Analysis of surface water data.
 Author-email: USGS <comptools@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United States because it contains materials that originally came from the United States Geological Survey, an agency of the United States Department of Interior.
         For more information, see the official USGS copyright policy at https://www.usgs.gov/information-policies-and-instructions/copyrights-and-credits.
@@ -33,51 +33,70 @@
 Project-URL: repository, https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap.git
 Keywords: USGS,water data,analysis
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# hyswap
+# hyswap - HYdrologic Surface Water Analysis Package
 
 [![USGS-category-image](https://img.shields.io/badge/USGS-Core-green.svg)](https://owi.usgs.gov/R/packages.html#core)
 [![pipeline-status-image](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/badges/main/pipeline.svg)](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/-/commits/main)
 [![coverage-report-image](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/badges/main/coverage.svg)](https://code.usgs.gov/water/computational-tools/surface-water-work/hyswap/-/commits/main)
+[![PyPI version](https://badge.fury.io/py/hyswap.svg)](https://badge.fury.io/py/hyswap)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyswap)
+
+## Overview
+
+`hyswap` (HYdrologic Surface Water Analysis Package), is a Python package which provides a set of functions for manipulating and visualizing USGS water data.
+Specifically, a number of functions for calculating statistics (e.g., exceedance probabilities, daily historic percentiles) and generating related plots (e.g., flow duration curves, streamflow duration hydrographs) are available.
+These methods are provided in a modular fashion as individual functions, and are designed to give the user flexibility in implementation.
 
 ### Project Documentation
 
-`hyswap` documentation is available at: [Link](https://rconnect.usgs.gov/hyswap-docs/html/)
+For more information, visit the `hyswap` [documentation](https://doi-usgs.github.io/hyswap/).
 
 ## Installation
 
-### User Installation
+### User Installation via `pip`
 
-User installation is possible from source right now.
-First you will need to clone the repository.
+One-liner to install `hyswap` via `pip`:
+
+```bash
+pip install hyswap
+```
+
+*Note:* `hyswap` has 4 dependencies right now, `numpy`, `pandas`, `scipy`, and `matplotlib`, these will be installed automatically when installing the package via `pip`.
+
+### User Installation From Source
+
+To install `hyswap` from source, first you will need to clone the repository.
 Next, from the root of the repository, run the following commands:
 
 ```bash
 pip install -r requirements.txt
 pip install .
 ```
 
 ### Developer Installation
 
-Developer installation is possible from source right now.
+Developer installation should be performed from source.
 First you will need to clone the repository.
 Next, from the root of the repository, run the following commands:
 
 ```bash
 pip install -r requirements.txt
 pip install -r requirements-dev.txt
 pip install -e .
 ```
 
 ### Testing and Building Documentation Locally
 
+To test the code and building and test the documentation locally, you must have cloned the source repository, follow the instructions above for a "developer installation" first.
+
 To test the package locally, run the following command from the root of the repository:
 
 ```bash
 pytest
 ```
 
 To build the documentation locally, run the following commands from the root of the repository:
```

### Comparing `hyswap-0.0.0a0/hyswap.egg-info/SOURCES.txt` & `hyswap-0.0.1/hyswap.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -17,26 +17,31 @@
 docs/source/conf.py
 docs/source/index.rst
 docs/source/examples/cumulative_hydrograph_examples.rst
 docs/source/examples/flow_duration_curve_examples.rst
 docs/source/examples/index.rst
 docs/source/examples/raster_hydrograph_examples.rst
 docs/source/examples/streamflow_duration_hydrograph_examples.rst
+docs/source/meta/contributing.rst
+docs/source/meta/disclaimer.rst
+docs/source/meta/installation.rst
 docs/source/reference/hyswap.png
 docs/source/reference/index.rst
 hyswap/__init__.py
 hyswap/_version.py
 hyswap/cumulative.py
 hyswap/exceedance.py
 hyswap/percentiles.py
+hyswap/plots.py
 hyswap/rasterhydrograph.py
 hyswap/utils.py
 hyswap.egg-info/PKG-INFO
 hyswap.egg-info/SOURCES.txt
 hyswap.egg-info/dependency_links.txt
 hyswap.egg-info/requires.txt
 hyswap.egg-info/top_level.txt
 tests/test_cumulative.py
 tests/test_exceedance.py
 tests/test_percentiles.py
+tests/test_plots.py
 tests/test_rasterhydrograph.py
 tests/test_utils.py
```

### Comparing `hyswap-0.0.0a0/pyproject.toml` & `hyswap-0.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/tests/test_cumulative.py` & `hyswap-0.0.1/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/tests/test_exceedance.py` & `hyswap-0.0.1/tests/test_exceedance.py`

 * *Files identical despite different names*

### Comparing `hyswap-0.0.0a0/tests/test_percentiles.py` & `hyswap-0.0.1/tests/test_percentiles.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,47 +33,53 @@
         'data': np.arange(101),
         'date': pd.date_range('2019-01-01', '2019-04-11')})
     # test the function
     percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
         df, 'data', date_column_name='date')
     assert percentiles_.shape == (101, 8)
     assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
-    assert percentiles_.index.tolist() == list(range(1, 102))
+    assert percentiles_.index.get_level_values(1).tolist()[0] == '01-01'
+    assert percentiles_.index.get_level_values(0).tolist()[0] == 1
     # test the function with no date column and dates in the index
     df = df.set_index('date')
     percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
         df, 'data')
     assert percentiles_.shape == (101, 8)
     assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
-    assert percentiles_.index.tolist() == list(range(1, 102))
+    assert percentiles_.index.get_level_values(1).tolist()[0] == '01-01'
+    assert percentiles_.index.get_level_values(0).tolist()[0] == 1
     # test the function with a different set of percentiles
     percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
         df, 'data', percentiles=np.array((0, 10, 50, 90, 100)))
     assert percentiles_.shape == (101, 5)
     assert percentiles_.columns.tolist() == [0, 10, 50, 90, 100]
-    assert percentiles_.index.tolist() == list(range(1, 102))
+    assert percentiles_.index.get_level_values(1).tolist()[0] == '01-01'
+    assert percentiles_.index.get_level_values(0).tolist()[0] == 1
     # all percentiles should be NaN because demo dataset is 1 year only
     assert percentiles_.isna().all().all()
     # test the function with a different year type
     percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
         df, 'data', year_type='water')
     assert percentiles_.shape == (101, 8)
     assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
-    assert percentiles_.index.tolist()[0] == 1
-    assert percentiles_.index.tolist()[-1] == 101
+    assert percentiles_.index.get_level_values(1).tolist()[0] == '01-01'
+    assert percentiles_.index.get_level_values(0).tolist()[0] == 93
+    assert percentiles_.index.get_level_values(1).tolist()[-1] == '04-11'
+    assert percentiles_.index.get_level_values(0).tolist()[-1] == 193
     # all percentiles should be NaN because demo dataset is 1 year only
     assert percentiles_.isna().all().all()
     # test the function with a different year type and a different set of
     # percentiles
     percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
         df, 'data', year_type='climate',
         percentiles=np.array((0, 10, 50, 90, 100)))
     assert percentiles_.shape == (101, 5)
     assert percentiles_.columns.tolist() == [0, 10, 50, 90, 100]
-    assert percentiles_.index.tolist()[0] == 1
+    assert percentiles_.index.get_level_values(1).tolist()[0] == '04-01'
+    assert percentiles_.index.get_level_values(0).tolist()[0] == 1
     # all percentiles should be NaN because demo dataset is 1 year only
     assert percentiles_.isna().all().all()
     # make a bigger dummy dataset so values are not NaN
     df = pd.DataFrame({
         'data': np.random.random(
             len(pd.date_range('2000-01-01', '2020-12-31'))),
         'date': pd.date_range('2000-01-01', '2020-12-31')})
@@ -87,21 +93,25 @@
             len(pd.date_range('2000-01-01', '2001-12-31'))),
         'date': pd.date_range('2000-01-01', '2001-12-31')})
     # test the function
     percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
         df, 'data', date_column_name='date', year_type='water')
     assert percentiles_.shape == (365, 8)
     assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
-    assert percentiles_.index.tolist()[0] == 1
-    assert percentiles_.index.tolist()[-1] == 365
+    assert percentiles_.index.get_level_values(1).tolist()[0] == '10-01'
+    assert percentiles_.index.get_level_values(0).tolist()[0] == 1
+    assert percentiles_.index.get_level_values(1).tolist()[-1] == '09-30'
+    assert percentiles_.index.get_level_values(0).tolist()[-1] == 365
     # test a longer dummy set that exceeds 1 year
     df = pd.DataFrame({
         'data': np.random.random(
             len(pd.date_range('2001-01-01', '2002-12-31'))),
         'date': pd.date_range('2001-01-01', '2002-12-31')})
     # test the function
     percentiles_ = percentiles.calculate_variable_percentile_thresholds_by_day(
         df, 'data', date_column_name='date', year_type='water')
     assert percentiles_.shape == (365, 8)
     assert percentiles_.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
-    assert percentiles_.index.tolist()[0] == 1
-    assert percentiles_.index.tolist()[-1] == 365
+    assert percentiles_.index.get_level_values(1).tolist()[0] == '10-01'
+    assert percentiles_.index.get_level_values(0).tolist()[0] == 1
+    assert percentiles_.index.get_level_values(1).tolist()[-1] == '09-30'
+    assert percentiles_.index.get_level_values(0).tolist()[-1] == 365
```

### Comparing `hyswap-0.0.0a0/tests/test_rasterhydrograph.py` & `hyswap-0.0.1/tests/test_rasterhydrograph.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,23 +22,25 @@
          'index_year': dummy_dates.year.tolist(),
          'month': dummy_dates.month.tolist(),
          'day': dummy_dates.day.tolist(),
          'index_doy': dummy_dates.dayofyear.tolist()}
         )
     df.set_index('date', inplace=True)
     # test the function with default values
-    date_range = rasterhydrograph._calculate_date_range(df, None, None)
+    date_range = rasterhydrograph._calculate_date_range(df, 'calendar',
+                                                        None, None)
     assert date_range[0].year == 2018
-    assert date_range[0].month == 6
+    assert date_range[0].month == 1
     assert date_range[0].day == 1
     assert date_range[-1].year == 2022
-    assert date_range[-1].month == 1
+    assert date_range[-1].month == 12
     assert date_range[-1].day == 31
     # test the function specifying start and end years
-    date_range = rasterhydrograph._calculate_date_range(df, 2019, 2020)
+    date_range = rasterhydrograph._calculate_date_range(df, 'calendar',
+                                                        2019, 2020)
     assert date_range[0].year == 2019
     assert date_range[0].month == 1
     assert date_range[0].day == 1
     assert date_range[-1].year == 2020
     assert date_range[-1].month == 12
     assert date_range[-1].day == 31
 
@@ -143,89 +145,89 @@
     )
     df_date = df.set_index('date')
     # test the function with a dataframe and a date column
     df_out = rasterhydrograph.format_data(df, 'value', 'date')
     assert len(df_out.index) == 5
     assert len(df_out.columns) == 365
     # assert day 1 of 2018 has no data, is NaN
-    assert np.isnan(df_out.loc[2018].loc[1])
+    assert np.isnan(df_out.loc[2018][0])
     # assert day 350 of 2022 has no data, is NaN
-    assert np.isnan(df_out.loc[2022].loc[350])
+    assert np.isnan(df_out.loc[2022][349])
     # test the function with a dataframe and a date index
     df_out = rasterhydrograph.format_data(df_date, 'value')
     assert len(df_out.index) == 5
     assert len(df_out.columns) == 365
     # assert day 1 of 2018 has no data, is NaN
-    assert np.isnan(df_out.loc[2018].loc[1])
+    assert np.isnan(df_out.loc[2018][0])
     # assert day 350 of 2022 has no data, is NaN
-    assert np.isnan(df_out.loc[2022].loc[350])
+    assert np.isnan(df_out.loc[2022][349])
     # test the function with a dataframe and a date index and beginning year
     df_out = rasterhydrograph.format_data(df_date, 'value', begin_year=2019)
     assert len(df_out.index) == 4
     assert len(df_out.columns) == 365
     # assert day 1 of 2019 has data, is not NaN
-    assert ~np.isnan(df_out.loc[2019].loc[1])
+    assert ~np.isnan(df_out.loc[2019][0])
     # assert day 350 of 2022 has no data, is NaN
-    assert np.isnan(df_out.loc[2022].loc[350])
+    assert np.isnan(df_out.loc[2022][349])
     # test the function with a dataframe and a date index and ending year
     df_out = rasterhydrograph.format_data(df_date, 'value', end_year=2021)
     assert len(df_out.index) == 4
     assert len(df_out.columns) == 365
     # assert day 1 of 2018 has no data, is NaN
-    assert np.isnan(df_out.loc[2018].loc[1])
+    assert np.isnan(df_out.loc[2018][0])
     # assert day 350 of 2021 has data, is not NaN
-    assert ~np.isnan(df_out.loc[2021].loc[350])
+    assert ~np.isnan(df_out.loc[2021][349])
     # test the function with a dataframe and a date index and a different
     # data averaging scheme
     df_7out = rasterhydrograph.format_data(df_date, 'value',
                                            data_type='7-day')
     assert len(df_7out.index) == 5
     assert len(df_7out.columns) == 365
     # assert day 1 of 2018 has no data, is NaN
-    assert np.isnan(df_7out.loc[2018].loc[1])
+    assert np.isnan(df_7out.loc[2018][0])
     # assert day 350 of 2022 has no data, is NaN
-    assert np.isnan(df_7out.loc[2022].loc[350])
+    assert np.isnan(df_7out.loc[2022][349])
     # check that there are non-NaN values in the data frame
     assert ~np.isnan(df_7out.values).all()
     # test the function with a dataframe and a date index and a water year
     df_out_water = rasterhydrograph.format_data(df_date, 'value',
                                                 year_type='water')
     assert len(df_out_water.index) == 5
     assert len(df_out_water.columns) == 365
     # check that there are non-NaN values in the data frame
     assert ~np.isnan(df_out_water.values).all()
     # check that day 1 of year 2019 is 10/1/2018
-    assert df_out_water.loc[2019].loc[1] == df_out.loc[2018].loc[274]
+    assert df_out_water.loc[2019][0] == df_out.loc[2018][273]
     # check that the last day of year 2020 is 9/30/2020
-    assert df_out_water.loc[2020].loc[365] == df_out.loc[2020].loc[273]
+    assert df_out_water.loc[2020][364] == df_out.loc[2020][272]
     # test the function with a dataframe and a date index and a different
     # data averaging scheme and a water year
     df_7out_water = rasterhydrograph.format_data(df_date, 'value',
                                                  data_type='7-day',
                                                  year_type='water')
     assert len(df_7out_water.index) == 5
     assert len(df_7out_water.columns) == 365
     # check that there are non-NaN values in the data frame
     assert ~np.isnan(df_7out_water.values).all()
     # check that day 1 of year 2019 is 10/1/2018
-    assert df_7out_water.loc[2019].loc[1] == df_7out.loc[2018].loc[274]
+    assert df_7out_water.loc[2019][0] == df_7out.loc[2018][273]
     # check that the last day of year 2020 is 9/30/2020
-    assert df_7out_water.loc[2020].loc[365] == df_7out.loc[2020].loc[273]
+    assert df_7out_water.loc[2020][364] == df_7out.loc[2020][272]
     # test the function with a dataframe and a date index and in a
     # climate year
     df_out_climate = rasterhydrograph.format_data(df_date, 'value',
                                                   year_type='climate')
     assert len(df_out_climate.index) == 4
     assert len(df_out_climate.columns) == 365
     # check that there are non-NaN values in the data frame
     assert ~np.isnan(df_out_climate.values).all()
     # check that day 1 of year 2020 is 4/1/2019
-    assert df_out_climate.loc[2020].loc[1] == df_out.loc[2019].loc[91]
+    assert df_out_climate.loc[2020][0] == df_out.loc[2019][90]
     # check that the last day of year 2021 is 3/31/2021
-    assert df_out_climate.loc[2021].loc[365] == df_out.loc[2021].loc[90]
+    assert df_out_climate.loc[2021][364] == df_out.loc[2021][89]
     # test the function with a dataframe and a date index and a different
     # data averaging scheme via kwargs and a climate year
     df_7out_climate = rasterhydrograph.format_data(df_date, 'value',
                                                    data_type='7-day',
                                                    year_type='climate',
                                                    center=True)
     assert len(df_7out_climate.index) == 4
```

### Comparing `hyswap-0.0.0a0/tests/test_utils.py` & `hyswap-0.0.1/tests/test_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -197,7 +197,54 @@
                                        year_type='climate',
                                        clip_leap_day=True)
     assert df.index.year.unique().tolist() == [2020]
     assert df['index_year'].unique().tolist() == [2020, 2021]
     assert df['index_doy'].tolist() == list(range(276, 366)) + \
         list(range(1, 276))
     assert len(df['index_doy']) == 365
+
+
+def test_munge_nwis_stats():
+    """Test the munge_nwis_stats function."""
+    # make a dataframe
+    df = pd.DataFrame({
+        'month_nu': [1, 2, 3, 4],
+        'day_nu': [1, 2, 3, 4],
+        'end_yr': [2019, 2019, 2019, 2019],
+        'min_va': [1, 2, 3, 4],
+        'max_va': [5, 6, 7, 8],
+        'mean_va': [9, 10, 11, 12],
+        'p05_va': [13, 14, 15, 16],
+        'p10_va': [17, 18, 19, 20],
+        'p25_va': [21, 22, 23, 24],
+        'p50_va': [25, 26, 27, 28],
+        'p75_va': [29, 30, 31, 32],
+        'p90_va': [33, 34, 35, 36],
+        'p95_va': [37, 38, 39, 40],
+    })
+    # apply the function
+    df_slim = utils.munge_nwis_stats(df)
+    # check the output
+    assert df_slim.shape == (4, 8)
+    assert len(df.columns) > len(df_slim.columns)
+    assert 0 in df_slim.columns
+    assert df_slim.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
+    # function w/ additional parameters
+    df_slim = utils.munge_nwis_stats(df, ['min_va', 'max_va'], [0, 100])
+    assert df_slim.shape == (4, 2)
+    assert df_slim.columns.tolist() == [0, 100]
+    assert len(df.columns) > len(df_slim.columns)
+    # raise error if column lists are of different lengths
+    with pytest.raises(ValueError):
+        utils.munge_nwis_stats(df, ['min_va', 'max_va'], [0, 100, 200])
+    # specify year type
+    df_slim = utils.munge_nwis_stats(df, year_type='water')
+    assert df_slim.shape == (4, 8)
+    assert len(df.columns) > len(df_slim.columns)
+    assert 0 in df_slim.columns
+    assert df_slim.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
+    # check with climate year
+    df_slim = utils.munge_nwis_stats(df, year_type='climate')
+    assert df_slim.shape == (4, 8)
+    assert len(df.columns) > len(df_slim.columns)
+    assert 0 in df_slim.columns
+    assert df_slim.columns.tolist() == [0, 5, 10, 25, 75, 90, 95, 100]
```

