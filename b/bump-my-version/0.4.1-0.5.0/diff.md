# Comparing `tmp/bump-my-version-0.4.1.tar.gz` & `tmp/bump-my-version-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bump-my-version-0.4.1.tar", last modified: Fri Jun  9 11:43:57 2023, max compression
+gzip compressed data, was "bump-my-version-0.5.0.tar", last modified: Mon Jun 12 14:03:04 2023, max compression
```

## Comparing `bump-my-version-0.4.1.tar` & `bump-my-version-0.5.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.863182 bump-my-version-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-09 11:43:57.863182 bump-my-version-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.859182 bump-my-version-0.4.1/bump_my_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-09 11:43:57.000000 bump-my-version-0.4.1/bump_my_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-09 11:43:57.000000 bump-my-version-0.4.1/bump_my_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:43:57.000000 bump-my-version-0.4.1/bump_my_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 11:43:57.000000 bump-my-version-0.4.1/bump_my_version.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-09 11:43:57.000000 bump-my-version-0.4.1/bump_my_version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 11:43:57.000000 bump-my-version-0.4.1/bump_my_version.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.859182 bump-my-version-0.4.1/bumpversion/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/bumpversion/version_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 11:43:57.863182 bump-my-version-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.859182 bump-my-version-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.859182 bump-my-version-0.4.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/basic_cfg.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/basic_cfg.toml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/basic_cfg_expected.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.863182 bump-my-version-0.4.1/tests/fixtures/glob/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.863182 bump-my-version-0.4.1/tests/fixtures/glob/directory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/glob/directory/file3.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/glob/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/glob/file2.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/glob/not-text.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:43:57.863182 bump-my-version-0.4.1/tests/fixtures/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/interpolation/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/interpolation/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/fixtures/interpolation/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-09 11:43:35.000000 bump-my-version-0.4.1/tests/test_version_part.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.417677 bump-my-version-0.5.0/bump_my_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-06-12 14:03:04.000000 bump-my-version-0.5.0/bump_my_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-12 14:03:04.000000 bump-my-version-0.5.0/bump_my_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:03:04.000000 bump-my-version-0.5.0/bump_my_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 14:03:04.000000 bump-my-version-0.5.0/bump_my_version.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-12 14:03:04.000000 bump-my-version-0.5.0/bump_my_version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 14:03:04.000000 bump-my-version-0.5.0/bump_my_version.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/bumpversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/version_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/basic_cfg.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/basic_cfg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/basic_cfg_expected.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/tests/fixtures/glob/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/tests/fixtures/glob/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/glob/directory/file3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/glob/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/glob/file2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/glob/not-text.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/tests/fixtures/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/interpolation/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/interpolation/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/interpolation/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_version_part.py
```

### Comparing `bump-my-version-0.4.1/CHANGELOG.md` & `bump-my-version-0.5.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,45 @@
 # Changelog
 
+## 0.5.0 (2023-06-12)
+[Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.4.1...0.5.0)
+
+### Fixes
+
+- Fixed ruff complaints about subprocess. [c429c68](https://github.com/callowayproject/bump-my-version/commit/c429c682515455558095836cb108a93fa23aa67f)
+    
+- Fixed issue with formatting. [da7544f](https://github.com/callowayproject/bump-my-version/commit/da7544f18780d5f289381d33a87b331c3eaf4d6b)
+    
+  There is an underlying edge case where the deriving previous environment variables with multple ways of formatting version numbers will fail.
+### New
+
+- Add test to reproduce issue #14. [d78ff46](https://github.com/callowayproject/bump-my-version/commit/d78ff46d65ce75b7651e5697eef59dbcb71c935e)
+    
+- Added documentation for replacing strings in different files. [893ec03](https://github.com/callowayproject/bump-my-version/commit/893ec03f6ceaf2a050c31f10006aa63c0411af4e)
+    
+  Fixes #6
+### Other
+
+- Made `VERSION_PART` optional. [f236b7d](https://github.com/callowayproject/bump-my-version/commit/f236b7de94d9f58e493c617848e3eb02e85a24c7)
+    
+  - Fixes #16
+  - `VERSION_PART` is detected from the arguments based on the configuration
+### Updates
+
+- Updated docs indicated VERSION_PART is optional. [22edeac](https://github.com/callowayproject/bump-my-version/commit/22edeac9018e75f79d7167fbfc6ca56cda4d3b07)
+    
+- Updated tests for bad version parts. [23be62d](https://github.com/callowayproject/bump-my-version/commit/23be62deed9fb7d51a8bbc195433d1a4ce74c11f)
+    
+- Changed exception type raised when bad version part is detected. [1e3ebc5](https://github.com/callowayproject/bump-my-version/commit/1e3ebc5b144294771b7bfe812299af4f92ae212a)
+    
+  - ValueError -> click.BadArgumentUsage
+- Updated readme. [7780265](https://github.com/callowayproject/bump-my-version/commit/7780265b97ce49492fef73ca3ac8a1cce27a2fad)
+    
+  Fixes #7
+
 ## 0.4.1 (2023-06-09)
 [Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.4.0...0.4.1)
 
 ### Fixes
 
 - Fixes release.yaml. [01870d5](https://github.com/callowayproject/bump-my-version/commit/01870d5878b5f0a6e601863c4b9c25572db6cbb0)
```

### Comparing `bump-my-version-0.4.1/CODE_OF_CONDUCT.md` & `bump-my-version-0.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/CONTRIBUTING.md` & `bump-my-version-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/LICENSE` & `bump-my-version-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/PKG-INFO` & `bump-my-version-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.4.1
+Version: 0.5.0
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -84,30 +84,16 @@
 * supports Python 3.8+ and PyPy3. Python 3.7 should work but isn't actively tested.
 
 ## Future Direction
 
 - Make it easier to get the current version
 - Switch having both the version part and files to change as arguments on the command line.
 - Make the version part argument _truly_ optional when `--new-version` is specified
-- Allow for multiple tags, including one that moves for having a `v2` that always points to the latest version of version 2.
-- https://github.com/c4urself/bump2version/issues/253 Have an "always increment" configuration
+- Allow for multiple tags, including one that moves for having a `v2` that always points to the latest version of version 2. [For example](https://github.com/actions/toolkit/blob/master/docs/action-versioning.md#recommendations)
 - Better UI with [Rich](https://rich.readthedocs.io/en/stable/index.html)
-- https://github.com/c4urself/bump2version/issues/267 Ignore-missing error in files flag
-- https://github.com/c4urself/bump2version/issues/233 How are relative configured file paths resolved?
-- https://github.com/c4urself/bump2version/issues/225 Properly resolve configuration file through parent directories when in a git or mercurial repo
-
-**Documentation opportunities**
-
-- https://github.com/c4urself/bump2version/issues/252 
-- https://github.com/c4urself/bump2version/issues/247
-- https://github.com/c4urself/bump2version/issues/243
-- https://github.com/c4urself/bump2version/issues/240
-- https://github.com/c4urself/bump2version/issues/239
-- Add dates to releases in changelog
-- https://github.com/c4urself/bump2version/issues/200 Add CalVer examples
 
 ## Installation
 
 You can download and install the latest version of this software from the Python package index (PyPI) as follows:
 
 ```console
 pip install --upgrade bump-my-version
```

### Comparing `bump-my-version-0.4.1/README.md` & `bump-my-version-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -29,30 +29,16 @@
 * supports Python 3.8+ and PyPy3. Python 3.7 should work but isn't actively tested.
 
 ## Future Direction
 
 - Make it easier to get the current version
 - Switch having both the version part and files to change as arguments on the command line.
 - Make the version part argument _truly_ optional when `--new-version` is specified
-- Allow for multiple tags, including one that moves for having a `v2` that always points to the latest version of version 2.
-- https://github.com/c4urself/bump2version/issues/253 Have an "always increment" configuration
+- Allow for multiple tags, including one that moves for having a `v2` that always points to the latest version of version 2. [For example](https://github.com/actions/toolkit/blob/master/docs/action-versioning.md#recommendations)
 - Better UI with [Rich](https://rich.readthedocs.io/en/stable/index.html)
-- https://github.com/c4urself/bump2version/issues/267 Ignore-missing error in files flag
-- https://github.com/c4urself/bump2version/issues/233 How are relative configured file paths resolved?
-- https://github.com/c4urself/bump2version/issues/225 Properly resolve configuration file through parent directories when in a git or mercurial repo
-
-**Documentation opportunities**
-
-- https://github.com/c4urself/bump2version/issues/252 
-- https://github.com/c4urself/bump2version/issues/247
-- https://github.com/c4urself/bump2version/issues/243
-- https://github.com/c4urself/bump2version/issues/240
-- https://github.com/c4urself/bump2version/issues/239
-- Add dates to releases in changelog
-- https://github.com/c4urself/bump2version/issues/200 Add CalVer examples
 
 ## Installation
 
 You can download and install the latest version of this software from the Python package index (PyPI) as follows:
 
 ```console
 pip install --upgrade bump-my-version
```

### Comparing `bump-my-version-0.4.1/bump_my_version.egg-info/PKG-INFO` & `bump-my-version-0.5.0/bump_my_version.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.4.1
+Version: 0.5.0
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -84,30 +84,16 @@
 * supports Python 3.8+ and PyPy3. Python 3.7 should work but isn't actively tested.
 
 ## Future Direction
 
 - Make it easier to get the current version
 - Switch having both the version part and files to change as arguments on the command line.
 - Make the version part argument _truly_ optional when `--new-version` is specified
-- Allow for multiple tags, including one that moves for having a `v2` that always points to the latest version of version 2.
-- https://github.com/c4urself/bump2version/issues/253 Have an "always increment" configuration
+- Allow for multiple tags, including one that moves for having a `v2` that always points to the latest version of version 2. [For example](https://github.com/actions/toolkit/blob/master/docs/action-versioning.md#recommendations)
 - Better UI with [Rich](https://rich.readthedocs.io/en/stable/index.html)
-- https://github.com/c4urself/bump2version/issues/267 Ignore-missing error in files flag
-- https://github.com/c4urself/bump2version/issues/233 How are relative configured file paths resolved?
-- https://github.com/c4urself/bump2version/issues/225 Properly resolve configuration file through parent directories when in a git or mercurial repo
-
-**Documentation opportunities**
-
-- https://github.com/c4urself/bump2version/issues/252 
-- https://github.com/c4urself/bump2version/issues/247
-- https://github.com/c4urself/bump2version/issues/243
-- https://github.com/c4urself/bump2version/issues/240
-- https://github.com/c4urself/bump2version/issues/239
-- Add dates to releases in changelog
-- https://github.com/c4urself/bump2version/issues/200 Add CalVer examples
 
 ## Installation
 
 You can download and install the latest version of this software from the Python package index (PyPI) as follows:
 
 ```console
 pip install --upgrade bump-my-version
```

### Comparing `bump-my-version-0.4.1/bump_my_version.egg-info/SOURCES.txt` & `bump-my-version-0.5.0/bump_my_version.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/bumpversion/aliases.py` & `bump-my-version-0.5.0/bumpversion/aliases.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/bumpversion/autocast.py` & `bump-my-version-0.5.0/bumpversion/autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/bumpversion/bump.py` & `bump-my-version-0.5.0/bumpversion/bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/bumpversion/cli.py` & `bump-my-version-0.5.0/bumpversion/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 #     """Version bump your Python project."""
 #     if ctx.invoked_subcommand is None:
 #         ctx.invoke(bump)
 
 
 @click.command(context_settings={"ignore_unknown_options": True})
 @click.version_option(version=__version__)
-@click.argument("version_part")
-@click.argument("files", nargs=-1, type=click.Path())
+@click.argument("args", nargs=-1, type=str)
 @click.option(
     "--config-file",
     metavar="FILE",
     required=False,
     envvar="BUMPVERSION_CONFIG_FILE",
     type=click.Path(exists=True),
     help="Config file to read most of the variables from.",
@@ -161,16 +160,16 @@
 @click.option(
     "--list",
     "show_list",
     is_flag=True,
     help="List machine readable information",
 )
 def cli(
-    version_part: str,
-    files: list,
+    # version_part: str,
+    args: list,
     config_file: Optional[str],
     verbose: int,
     allow_dirty: Optional[bool],
     current_version: Optional[str],
     new_version: Optional[str],
     parse: Optional[str],
     serialize: Optional[List[str]],
@@ -186,14 +185,16 @@
     message: Optional[str],
     commit_args: Optional[str],
     show_list: bool,
 ) -> None:
     """
     Change the version.
 
+    ARGS may contain any of the following:
+
     VERSION_PART is the part of the version to increase, e.g. `minor` .
     Valid values include those given in the `--serialize` / `--parse` option.
 
     FILES are additional file(s) to modify.
     If you want to rewrite only files specified on the command line, use with the
     `--no-configured-files` option.
     """
@@ -215,14 +216,22 @@
         tag_message=tag_message,
         message=message,
         commit_args=commit_args,
     )
 
     found_config_file = find_config_file(config_file)
     config = get_configuration(found_config_file, **overrides)
+    if args:
+        if args[0] not in config.parts.keys():
+            raise click.BadArgumentUsage(f"Unknown version part: {args[0]}")
+        version_part = args[0]
+        files = args[1:]
+    else:
+        version_part = None
+        files = args
 
     if show_list:
         log_list(config, version_part, new_version)
         return
 
     config.allow_dirty = allow_dirty if allow_dirty is not None else config.allow_dirty
     if not config.allow_dirty and config.scm_info.tool:
@@ -236,14 +245,16 @@
 
     do_bump(version_part, new_version, config, found_config_file, dry_run)
 
 
 def log_list(config: Config, version_part: Optional[str], new_version: Optional[str]) -> None:
     """Output configuration with new version."""
     ctx = get_context(config)
-    version = config.version_config.parse(config.current_version)
-    next_version = get_next_version(version, config, version_part, new_version)
-    next_version_str = config.version_config.serialize(next_version, ctx)
+    if version_part:
+        version = config.version_config.parse(config.current_version)
+        next_version = get_next_version(version, config, version_part, new_version)
+        next_version_str = config.version_config.serialize(next_version, ctx)
+
+        click.echo(f"new_version={next_version_str}")
 
-    click.echo(f"new_version={next_version_str}")
     for key, value in config.dict(exclude={"scm_info", "parts"}).items():
         click.echo(f"{key}={value}")
```

### Comparing `bump-my-version-0.4.1/bumpversion/config.py` & `bump-my-version-0.5.0/bumpversion/config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/bumpversion/exceptions.py` & `bump-my-version-0.5.0/bumpversion/exceptions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/bumpversion/files.py` & `bump-my-version-0.5.0/bumpversion/files.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/bumpversion/functions.py` & `bump-my-version-0.5.0/bumpversion/functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/bumpversion/logging.py` & `bump-my-version-0.5.0/bumpversion/logging.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/bumpversion/scm.py` & `bump-my-version-0.5.0/bumpversion/scm.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,27 +44,28 @@
 
         env = os.environ.copy()
         env["HGENCODING"] = "utf-8"
         env["BUMPVERSION_CURRENT_VERSION"] = current_version
         env["BUMPVERSION_NEW_VERSION"] = new_version
 
         try:
-            subprocess.run([*cls._COMMIT_COMMAND, f.name, *extra_args], env=env, capture_output=True, check=True)
+            cmd = [*cls._COMMIT_COMMAND, f.name, *extra_args]
+            subprocess.run(cmd, env=env, capture_output=True, check=True)  # noqa: S603
         except subprocess.CalledProcessError as exc:  # pragma: no-coverage
             err_msg = f"Failed to run {exc.cmd}: return code {exc.returncode}, output: {exc.output}"
             logger.exception(err_msg)
             raise exc
         finally:
             os.unlink(f.name)
 
     @classmethod
     def is_usable(cls) -> bool:
         """Is the VCS implementation usable."""
         try:
-            result = subprocess.run(cls._TEST_USABLE_COMMAND, check=True, capture_output=True)
+            result = subprocess.run(cls._TEST_USABLE_COMMAND, check=True, capture_output=True)  # noqa: S603
             return result.returncode == 0
         except (FileNotFoundError, PermissionError, NotADirectoryError, subprocess.CalledProcessError):
             return False
 
     @classmethod
     def assert_nondirty(cls) -> None:
         """Assert that the working directory is not dirty."""
@@ -85,15 +86,15 @@
         """Create a tag of the new_version in VCS."""
         raise NotImplementedError
 
     @classmethod
     def get_all_tags(cls) -> List[str]:
         """Return all tags in VCS."""
         try:
-            result = subprocess.run(cls._ALL_TAGS_COMMAND, text=True, check=True, capture_output=True)
+            result = subprocess.run(cls._ALL_TAGS_COMMAND, text=True, check=True, capture_output=True)  # noqa: S603
             return result.stdout.splitlines()
         except (FileNotFoundError, PermissionError, NotADirectoryError, subprocess.CalledProcessError):
             return []
 
     @classmethod
     def commit_to_scm(
         cls,
@@ -185,28 +186,28 @@
     _ALL_TAGS_COMMAND = ["git", "tag", "--list"]
 
     @classmethod
     def assert_nondirty(cls) -> None:
         """Assert that the working directory is not dirty."""
         lines = [
             line.strip()
-            for line in subprocess.check_output(["git", "status", "--porcelain"]).splitlines()
+            for line in subprocess.check_output(["git", "status", "--porcelain"]).splitlines()  # noqa: S603, S607
             if not line.strip().startswith(b"??")
         ]
 
         if lines:
             joined_lines = b"\n".join(lines).decode()
             raise DirtyWorkingDirectoryError(f"Git working directory is not clean:\n\n{joined_lines}")
 
     @classmethod
     def latest_tag_info(cls, tag_pattern: str) -> SCMInfo:
         """Return information about the latest tag."""
         try:
             # git-describe doesn't update the git-index, so we do that
-            subprocess.run(["git", "update-index", "--refresh", "-q"], capture_output=True)
+            subprocess.run(["git", "update-index", "--refresh", "-q"], capture_output=True)  # noqa: S603, S607
         except subprocess.CalledProcessError as e:
             logger.debug("Error when running git update-index: %s", e.stderr)
             return SCMInfo(tool=cls)
 
         try:
             # get info about the latest tag in git
             # TODO: This only works if the tag name is prefixed with `v`.
@@ -216,15 +217,15 @@
                 "describe",
                 "--dirty",
                 "--tags",
                 "--long",
                 "--abbrev=40",
                 f"--match={tag_pattern}",
             ]
-            result = subprocess.run(git_cmd, text=True, check=True, capture_output=True)
+            result = subprocess.run(git_cmd, text=True, check=True, capture_output=True)  # noqa: S603
             describe_out = result.stdout.strip().split("-")
         except subprocess.CalledProcessError as e:
             logger.debug("Error when running git describe: %s", e.stderr)
             return SCMInfo(tool=cls)
 
         info = SCMInfo(tool=cls)
 
@@ -239,15 +240,15 @@
         info.current_version = "-".join(describe_out).lstrip("v")
 
         return info
 
     @classmethod
     def add_path(cls, path: Union[str, Path]) -> None:
         """Add a path to the VCS."""
-        subprocess.check_output(["git", "add", "--update", str(path)])
+        subprocess.check_output(["git", "add", "--update", str(path)])  # noqa: S603, S607
 
     @classmethod
     def tag(cls, name: str, sign: bool = False, message: Optional[str] = None) -> None:
         """
         Create a tag of the new_version in VCS.
 
         If only name is given, bumpversion uses a lightweight tag.
@@ -259,15 +260,15 @@
             message: A optional message to annotate the tag.
         """
         command = ["git", "tag", name]
         if sign:
             command += ["--sign"]
         if message:
             command += ["--message", message]
-        subprocess.check_output(command)
+        subprocess.check_output(command)  # noqa: S603
 
 
 class Mercurial(SourceCodeManager):
     """Mercurial implementation."""
 
     _TEST_USABLE_COMMAND = ["hg", "root"]
     _COMMIT_COMMAND = ["hg", "commit", "--logfile"]
@@ -275,31 +276,31 @@
 
     @classmethod
     def latest_tag_info(cls, tag_pattern: str) -> SCMInfo:
         """Return information about the latest tag."""
         current_version = None
         re_pattern = tag_pattern.replace("*", ".*")
         result = subprocess.run(
-            ["hg", "log", "-r", f"tag('re:{re_pattern}')", "--template", "{latesttag}\n"],
+            ["hg", "log", "-r", f"tag('re:{re_pattern}')", "--template", "{latesttag}\n"],  # noqa: S603, S607
             text=True,
             check=True,
             capture_output=True,
         )
         result.check_returncode()
         if result.stdout:
             current_version = result.stdout.splitlines(keepends=False)[0].lstrip("v")
-        is_dirty = len(subprocess.check_output(["hg", "status", "-mard"])) != 0
+        is_dirty = len(subprocess.check_output(["hg", "status", "-mard"])) != 0  # noqa: S603, S607
         return SCMInfo(tool=cls, current_version=current_version, dirty=is_dirty)
 
     @classmethod
     def assert_nondirty(cls) -> None:
         """Assert that the working directory is clean."""
         lines = [
             line.strip()
-            for line in subprocess.check_output(["hg", "status", "-mard"]).splitlines()
+            for line in subprocess.check_output(["hg", "status", "-mard"]).splitlines()  # noqa: S603, S607
             if not line.strip().startswith(b"??")
         ]
 
         if lines:
             joined_lines = b"\n".join(lines).decode()
             raise DirtyWorkingDirectoryError(f"Mercurial working directory is not clean:\n{joined_lines}")
 
@@ -325,15 +326,15 @@
             SignedTagsError: If ``sign`` is ``True``
         """
         command = ["hg", "tag", name]
         if sign:
             raise SignedTagsError("Mercurial does not support signed tags.")
         if message:
             command += ["--message", message]
-        subprocess.check_output(command)
+        subprocess.check_output(command)  # noqa: S603
 
 
 def get_scm_info(tag_pattern: str) -> SCMInfo:
     """Return a dict with the latest source code management info."""
     if Git.is_usable():
         return Git.latest_tag_info(tag_pattern)
     elif Mercurial.is_usable():
```

### Comparing `bump-my-version-0.4.1/bumpversion/utils.py` & `bump-my-version-0.5.0/bumpversion/utils.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/bumpversion/version_part.py` & `bump-my-version-0.5.0/bumpversion/version_part.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/pyproject.toml` & `bump-my-version-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 [tool.ruff.isort]
 order-by-type = true
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.bumpversion]
-current_version = "0.4.1"
+current_version = "0.5.0"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "{new_version}"
 allow_dirty = true
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<dev>dev\\d+))?"
 serialize = [
```

### Comparing `bump-my-version-0.4.1/tests/conftest.py` & `bump-my-version-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/tests/fixtures/basic_cfg.cfg` & `bump-my-version-0.5.0/tests/fixtures/basic_cfg.cfg`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/tests/fixtures/basic_cfg.toml` & `bump-my-version-0.5.0/tests/fixtures/basic_cfg.toml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/tests/fixtures/basic_cfg_expected.json` & `bump-my-version-0.5.0/tests/fixtures/basic_cfg_expected.json`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/tests/test_autocast.py` & `bump-my-version-0.5.0/tests/test_autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/tests/test_bump.py` & `bump-my-version-0.5.0/tests/test_bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/tests/test_cli.py` & `bump-my-version-0.5.0/tests/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -97,23 +97,23 @@
                 "XXX{spam};{blob};{slurp}",
                 "--search",
                 "my-search",
                 "--replace",
                 "my-replace",
                 "--no-commit",
                 "--no-tag",
-                "patch",
+                "slurp",
                 "do-this-file.txt",
             ],
         )
 
     # Assert
     assert result.exit_code == 0
     assert mocked_do_bump.call_count == 1
-    assert mocked_do_bump.call_args[0][0] == "patch"
+    assert mocked_do_bump.call_args[0][0] == "slurp"
     assert mocked_do_bump.call_args[0][1] == "1.2.0"
     the_config = mocked_do_bump.call_args[0][2]
     assert the_config.current_version == "1.1.0"
     assert the_config.allow_dirty
     assert the_config.parse == r"XXX(?P<spam>\d+);(?P<blob>\d+);(?P<slurp>\d+)"
     assert the_config.serialize == ["XXX{spam};{blob};{slurp}"]
     assert the_config.search == "my-search"
@@ -149,16 +149,16 @@
         result: Result = runner.invoke(cli.cli, ["patch", "--current-version", "1.1.1", "--no-allow-dirty", "dirty2"])
 
     # Assert
     assert result.exit_code != 0
     assert "working directory is not clean" in result.output
 
 
-def test_listing_outputs_correctly_and_stops(tmp_path: Path, fixtures_path: Path):
-    """The --list option should list the configuration and nothing else."""
+def test_listing_with_version_part(tmp_path: Path, fixtures_path: Path):
+    """The --list option should list the configuration with new_version.."""
     # Arrange
     config_path = tmp_path / "pyproject.toml"
     toml_path = fixtures_path / "basic_cfg.toml"
     shutil.copy(toml_path, config_path)
     runner: CliRunner = CliRunner()
 
     with inside_dir(tmp_path):
@@ -189,14 +189,53 @@
         "'bumpversion/__init__.py', 'glob': None, 'parse': None, 'serialize': None, "
         "'search': None, 'replace': None}, {'filename': 'CHANGELOG.md', 'glob': None, "
         "'parse': None, 'serialize': None, 'search': '**unreleased**', 'replace': "
         "'**unreleased**\\n**v{new_version}**'}]",
     }
 
 
+def test_listing_without_version_part(tmp_path: Path, fixtures_path: Path):
+    """The --list option should list the configuration without new_version."""
+    # Arrange
+    config_path = tmp_path / "pyproject.toml"
+    toml_path = fixtures_path / "basic_cfg.toml"
+    shutil.copy(toml_path, config_path)
+    runner: CliRunner = CliRunner()
+
+    with inside_dir(tmp_path):
+        result: Result = runner.invoke(cli.cli, ["--list"])
+
+    if result.exit_code != 0:
+        print(result.output)
+        print(result.exception)
+
+    assert result.exit_code == 0
+    assert set(result.output.splitlines(keepends=False)) == {
+        "current_version=1.0.0",
+        "parse=(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\-(?P<release>[a-z]+))?",
+        "serialize=['{major}.{minor}.{patch}-{release}', '{major}.{minor}.{patch}']",
+        "search={current_version}",
+        "replace={new_version}",
+        "tag=True",
+        "sign_tags=False",
+        "tag_name=v{new_version}",
+        "tag_message=Bump version: {current_version} → {new_version}",
+        "allow_dirty=False",
+        "commit=True",
+        "message=Bump version: {current_version} → {new_version}",
+        "commit_args=None",
+        "files=[{'filename': 'setup.py', 'glob': None, 'parse': None, 'serialize': "
+        "None, 'search': None, 'replace': None}, {'filename': "
+        "'bumpversion/__init__.py', 'glob': None, 'parse': None, 'serialize': None, "
+        "'search': None, 'replace': None}, {'filename': 'CHANGELOG.md', 'glob': None, "
+        "'parse': None, 'serialize': None, 'search': '**unreleased**', 'replace': "
+        "'**unreleased**\\n**v{new_version}**'}]",
+    }
+
+
 def test_non_scm_operations_if_scm_not_installed(tmp_path: Path, monkeypatch):
     """Everything works except SCM commands if the SCM is unusable."""
     # Arrange
     monkeypatch.setenv("PATH", "")
 
     with inside_dir(tmp_path):
         version_path = tmp_path / "VERSION"
@@ -205,7 +244,36 @@
         runner: CliRunner = CliRunner()
 
         # Act
         runner.invoke(cli.cli, ["major", "--current-version", "31.0.3", "VERSION"])
 
     # Assert
     assert version_path.read_text() == "32.0.0"
+
+
+@pytest.mark.parametrize(
+    ["version_part"],
+    [
+        param("charlie", id="bad_version_part"),
+        param("", id="missing_version_part"),
+    ],
+)
+def test_detects_bad_or_missing_version_part(version_part: str, tmp_path: Path, monkeypatch):
+    """It properly detects bad or missing version part."""
+    # Arrange
+    monkeypatch.setenv("PATH", "")
+
+    with inside_dir(tmp_path):
+        version_path = tmp_path / "VERSION"
+        version_path.write_text("31.0.3")
+
+        runner: CliRunner = CliRunner()
+        args = ["--current-version", "31.0.3"]
+        if version_part:
+            args.append(version_part)
+        args.append("VERSION")
+        # Act
+        result = runner.invoke(cli.cli, args)
+
+    # Assert
+    assert result.exception is not None
+    assert "Unknown version part:" in result.stdout
```

### Comparing `bump-my-version-0.4.1/tests/test_config.py` & `bump-my-version-0.5.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/tests/test_files.py` & `bump-my-version-0.5.0/tests/test_files.py`

 * *Files 14% similar despite different names*

```diff
@@ -149,14 +149,84 @@
 
     assert full_vers_path.read_text() == "2.0.1"
     assert maj_vers_path.read_text() == "2"
     assert readme_path.read_text() == "MyAwesomeSoftware(TM) v2.0"
     assert build_num_path.read_text() == "2.0.1+jane+38945"
 
 
+def test_issue_14(tmp_path: Path):
+    full_vers_path = tmp_path / "FULL_VERSION.txt"
+    full_vers_path.write_text("3.1.0-rc+build.1031")
+    assembly_path = tmp_path / "AssemblyInfo.cs"
+    assembly_path.write_text(
+        '[assembly: AssemblyFileVersion("3.1.0-rc+build.1031")]\n' '[assembly: AssemblyVersion("3.1.1031.0")]'
+    )
+    csv_path = tmp_path / "Version.csv"
+    csv_path.write_text("1;3;1;0;rc;build.1031")
+
+    overrides = {
+        "current_version": "3.1.0-rc+build.1031",
+        "parse": r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(-(?P<release>[0-9A-Za-z]+))?(\+build\.(?P<build>.[0-9A-Za-z]+))?",
+        "serialize": ["{major}.{minor}.{patch}-{release}+build.{build}", "{major}.{minor}.{patch}+build.{build}"],
+        "commit": True,
+        "message": "Bump version: {current_version} -> {new_version}",
+        "tag": False,
+        "tag_name": "{new_version}",
+        "tag_message": "Version {new_version}",
+        "allow_dirty": True,
+        "files": [
+            {
+                "filename": str(full_vers_path),
+            },
+            {
+                "filename": str(assembly_path),
+                "search": '[assembly: AssemblyFileVersion("{current_version}")]',
+                "replace": '[assembly: AssemblyFileVersion("{new_version}")]',
+            },
+            {
+                "filename": str(assembly_path),
+                "parse": r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<build>\d+)\.(?P<patch>\d+)",
+                "serialize": ["{major}.{minor}.{build}.{patch}"],
+                "search": '[assembly: AssemblyVersion("{current_version}")]',
+                "replace": '[assembly: AssemblyVersion("{new_version}")]',
+            },
+            {
+                "filename": str(csv_path),
+                "parse": r"(?P<major>\d+);(?P<minor>\d+);(?P<patch>\d+);(?P<release>[0-9A-Za-z]+)?;(build\.(?P<build>.[0-9A-Za-z]+))?",
+                "serialize": [
+                    "{major};{minor};{patch};{release};build.{build}",
+                    "{major};{minor};{patch};;build.{build}",
+                ],
+                "search": "1;{current_version}",
+                "replace": "1;{new_version}",
+            },
+        ],
+        "parts": {
+            "release": {"values": ["beta", "rc", "final"], "optional_value": "final"},
+            "build": {
+                "first_value": 1000,
+                "independent": True,
+            },
+        },
+    }
+    conf, version_config, current_version = get_config_data(overrides)
+    major_version = current_version.bump("patch", version_config.order)
+
+    ctx = get_context(conf)
+
+    for file_cfg in conf.files:
+        cfg_file = files.ConfiguredFile(file_cfg, version_config)
+        cfg_file.replace_version(current_version, major_version, ctx)
+
+    assert full_vers_path.read_text() == "3.1.1-beta+build.1031"
+    expected = '[assembly: AssemblyFileVersion("3.1.1-beta+build.1031")]\n[assembly: AssemblyVersion("3.1.1031.1")]'
+    assert assembly_path.read_text() == expected
+    assert csv_path.read_text() == "1;3;1;1;beta;build.1031"
+
+
 def test_search_replace_to_avoid_updating_unconcerned_lines(tmp_path: Path):
     req_path = tmp_path / "requirements.txt"
     req_path.write_text("Django>=1.5.6,<1.6\nMyProject==1.5.6")
 
     changelog_path = tmp_path / "CHANGELOG.md"
     changelog_path.write_text(
         dedent(
```

### Comparing `bump-my-version-0.4.1/tests/test_functions.py` & `bump-my-version-0.5.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/tests/test_scm.py` & `bump-my-version-0.5.0/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.4.1/tests/test_version_part.py` & `bump-my-version-0.5.0/tests/test_version_part.py`

 * *Files identical despite different names*

