# Comparing `tmp/piptools_sync-1.0.3.tar.gz` & `tmp/piptools_sync-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piptools_sync-1.0.3.tar", last modified: Fri Apr 21 13:48:26 2023, max compression
+gzip compressed data, was "piptools_sync-1.0.4.tar", last modified: Mon Jun 12 11:18:24 2023, max compression
```

## Comparing `piptools_sync-1.0.3.tar` & `piptools_sync-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 13:48:26.528265 piptools_sync-1.0.3/
--rw-rw-rw-   0        0        0      157 2023-04-18 15:26:46.000000 piptools_sync-1.0.3/AUTHORS.md
--rw-rw-rw-   0        0        0     3830 2023-04-21 13:48:16.000000 piptools_sync-1.0.3/CHANGELOG.md
--rw-rw-rw-   0        0        0     1074 2022-08-23 11:11:28.000000 piptools_sync-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      194 2022-08-23 11:11:28.000000 piptools_sync-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    13543 2023-04-21 13:48:26.533795 piptools_sync-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    12567 2023-04-21 13:48:16.000000 piptools_sync-1.0.3/README.md
--rw-rw-rw-   0        0        0     2241 2022-10-07 21:51:55.000000 piptools_sync-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1693 2023-04-21 13:48:26.533795 piptools_sync-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      108 2023-04-21 12:31:49.000000 piptools_sync-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:48:26.433761 piptools_sync-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 13:48:26.497008 piptools_sync-1.0.3/src/piptools_sync/
--rw-rw-rw-   0        0        0     1706 2023-04-21 13:48:16.000000 piptools_sync-1.0.3/src/piptools_sync/__init__.py
--rw-rw-rw-   0        0        0      167 2023-04-07 17:19:25.000000 piptools_sync-1.0.3/src/piptools_sync/config.toml
--rw-rw-rw-   0        0        0     7645 2023-04-08 11:56:30.000000 piptools_sync-1.0.3/src/piptools_sync/mapping.json
--rw-rw-rw-   0        0        0    17398 2023-04-21 12:31:49.000000 piptools_sync-1.0.3/src/piptools_sync/piptools_sync.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:48:26.497008 piptools_sync-1.0.3/src/piptools_sync.egg-info/
--rw-rw-rw-   0        0        0    13543 2023-04-21 13:48:26.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13231 2023-04-18 15:26:46.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/PKG-INFO.rum-bak
--rw-rw-rw-   0        0        0      838 2023-04-21 13:48:26.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 13:48:26.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-21 13:48:26.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2023-04-21 13:48:26.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-21 13:48:26.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 13:48:26.528265 piptools_sync-1.0.3/tests/
--rw-rw-rw-   0        0        0      583 2022-09-04 19:08:21.000000 piptools_sync-1.0.3/tests/test__utility_find_file_path.py
--rw-rw-rw-   0        0        0      541 2022-08-26 17:02:45.000000 piptools_sync-1.0.3/tests/test__utility_remove_vee.py
--rw-rw-rw-   0        0        0      529 2022-08-28 18:06:52.000000 piptools_sync-1.0.3/tests/test_find_requirements_file.py
--rw-rw-rw-   0        0        0      348 2022-08-27 18:08:46.000000 piptools_sync-1.0.3/tests/test_find_yaml_config_file.py
--rw-rw-rw-   0        0        0      555 2022-09-20 15:51:26.000000 piptools_sync-1.0.3/tests/test_generate_db.py
--rw-rw-rw-   0        0        0      411 2022-08-28 17:54:33.000000 piptools_sync-1.0.3/tests/test_get_installed_version.py
--rw-rw-rw-   0        0        0      358 2022-08-26 17:04:02.000000 piptools_sync-1.0.3/tests/test_get_precommit_repos.py
--rw-rw-rw-   0        0        0      575 2022-08-28 17:54:33.000000 piptools_sync-1.0.3/tests/test_get_requirement_versions.py
--rw-rw-rw-   0        0        0      693 2022-08-28 15:02:33.000000 piptools_sync-1.0.3/tests/test_update_yaml.py
--rw-rw-rw-   0        0        0      465 2022-08-28 14:26:16.000000 piptools_sync-1.0.3/tests/test_yaml_to_dict.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:18:24.885353 piptools_sync-1.0.4/
+-rw-rw-rw-   0        0        0      172 2023-06-12 10:17:11.000000 piptools_sync-1.0.4/AUTHORS.md
+-rw-rw-rw-   0        0        0     4459 2023-06-12 11:18:12.000000 piptools_sync-1.0.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1074 2022-08-23 11:11:28.000000 piptools_sync-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-06-12 10:14:46.000000 piptools_sync-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    13972 2023-06-12 11:18:24.885353 piptools_sync-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12504 2023-06-12 11:18:12.000000 piptools_sync-1.0.4/README.md
+-rw-rw-rw-   0        0        0     2316 2023-06-12 11:03:35.000000 piptools_sync-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0     2185 2023-06-12 11:18:24.885353 piptools_sync-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      108 2023-04-21 12:31:49.000000 piptools_sync-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:18:24.787986 piptools_sync-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 11:18:24.834879 piptools_sync-1.0.4/src/piptools_sync/
+-rw-rw-rw-   0        0        0     1674 2023-06-12 11:18:12.000000 piptools_sync-1.0.4/src/piptools_sync/__init__.py
+-rw-rw-rw-   0        0        0      167 2023-04-07 17:19:25.000000 piptools_sync-1.0.4/src/piptools_sync/config.toml
+-rw-rw-rw-   0        0        0     7645 2023-04-08 11:56:30.000000 piptools_sync-1.0.4/src/piptools_sync/mapping.json
+-rw-rw-rw-   0        0        0    17700 2023-06-12 11:16:01.000000 piptools_sync-1.0.4/src/piptools_sync/piptools_sync.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:18:24.854056 piptools_sync-1.0.4/src/piptools_sync.egg-info/
+-rw-rw-rw-   0        0        0    13972 2023-06-12 11:18:24.000000 piptools_sync-1.0.4/src/piptools_sync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13231 2023-04-18 15:26:46.000000 piptools_sync-1.0.4/src/piptools_sync.egg-info/PKG-INFO.rum-bak
+-rw-rw-rw-   0        0        0      838 2023-06-12 11:18:24.000000 piptools_sync-1.0.4/src/piptools_sync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 11:18:24.000000 piptools_sync-1.0.4/src/piptools_sync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-12 11:18:24.000000 piptools_sync-1.0.4/src/piptools_sync.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      101 2023-06-12 11:18:24.000000 piptools_sync-1.0.4/src/piptools_sync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-12 11:18:24.000000 piptools_sync-1.0.4/src/piptools_sync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 11:18:24.885353 piptools_sync-1.0.4/tests/
+-rw-rw-rw-   0        0        0      583 2022-09-04 19:08:21.000000 piptools_sync-1.0.4/tests/test__utility_find_file_path.py
+-rw-rw-rw-   0        0        0      541 2022-08-26 17:02:45.000000 piptools_sync-1.0.4/tests/test__utility_remove_vee.py
+-rw-rw-rw-   0        0        0      529 2022-08-28 18:06:52.000000 piptools_sync-1.0.4/tests/test_find_requirements_file.py
+-rw-rw-rw-   0        0        0      348 2022-08-27 18:08:46.000000 piptools_sync-1.0.4/tests/test_find_yaml_config_file.py
+-rw-rw-rw-   0        0        0      555 2022-09-20 15:51:26.000000 piptools_sync-1.0.4/tests/test_generate_db.py
+-rw-rw-rw-   0        0        0      411 2022-08-28 17:54:33.000000 piptools_sync-1.0.4/tests/test_get_installed_version.py
+-rw-rw-rw-   0        0        0      358 2022-08-26 17:04:02.000000 piptools_sync-1.0.4/tests/test_get_precommit_repos.py
+-rw-rw-rw-   0        0        0      575 2022-08-28 17:54:33.000000 piptools_sync-1.0.4/tests/test_get_requirement_versions.py
+-rw-rw-rw-   0        0        0      693 2022-08-28 15:02:33.000000 piptools_sync-1.0.4/tests/test_update_yaml.py
+-rw-rw-rw-   0        0        0      465 2022-08-28 14:26:16.000000 piptools_sync-1.0.4/tests/test_yaml_to_dict.py
```

### Comparing `piptools_sync-1.0.3/CHANGELOG.md` & `piptools_sync-1.0.4/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.0.4 (2023-06-12)
+### Fix
+* Correct use of importlib traversables ([`210cfa5`](https://github.com/Stephen-RA-King/piptools-sync/commit/210cfa5851cf88e971506eeda98a30d5edc12050))
+
+### Documentation
+* Reorder & remove some badges ([`9480988`](https://github.com/Stephen-RA-King/piptools-sync/commit/9480988bfa7de3a8e1bc4035804c964f751a9c2f))
+* Minor updates ([`d02e30a`](https://github.com/Stephen-RA-King/piptools-sync/commit/d02e30af50be1fa5c5f4bffc4aa405fefc77bd24))
+* Add update github support files ([`11aa75e`](https://github.com/Stephen-RA-King/piptools-sync/commit/11aa75e49c96adeb38d626c892c590441f54bc17))
+
 ## v1.0.3 (2023-04-21)
 ### Fix
 * Shebang for version 3 env ([`b1442d8`](https://github.com/Stephen-RA-King/piptools-sync/commit/b1442d88028386ffacdba39dfe5ae04c30ac534d))
 
 ### Documentation
 * Update email link ([`cf67f5f`](https://github.com/Stephen-RA-King/piptools-sync/commit/cf67f5f16c366f0567c4d90667b77cb4ffe9ad34))
 * Update author email ([`9cfd29f`](https://github.com/Stephen-RA-King/piptools-sync/commit/9cfd29fd3e845b16e55b6a0c8eb4f9963ee6bd18))
```

### Comparing `piptools_sync-1.0.3/LICENSE` & `piptools_sync-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.3/PKG-INFO` & `piptools_sync-1.0.4/src/piptools_sync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 Metadata-Version: 2.1
-Name: piptools_sync
-Version: 1.0.3
+Name: piptools-sync
+Version: 1.0.4
 Summary: A piptools pre-commit version sync utility
 Home-page: https://github.com/Stephen-RA-King/piptools-sync
 Download-URL: https://github.com/Stephen-RA-King/piptools_sync/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
 License: MIT
-Keywords: utility
+Project-URL: documentation, https://piptools-sync.readthedocs.io/en/latest/
+Project-URL: Release Notes, https://github.com/Stephen-RA-King/piptools_sync/releases
+Project-URL: Source Code, https://github.com/Stephen-RA-King/piptools_sync/
+Project-URL: Issue Tracker, https://github.com/Stephen-RA-King/piptools_sync/issues
+Keywords: pre-commit-hooks,version-sync,pip-tools,pre-commit,dependency-manager
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Piptools-sync
 
 ---
 
 _**A pre-commit plugin to align pre-commit repository versions with those derived by pip-tools.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
-[![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
-[![pre-commit.ci][pre-commit.ci-image]][pre-commit.ci-url]
-[![CodeFactor][codefactor-image]][codefactor-url]
-[![Codeclimate][codeclimate-image]][codeclimate-url]
 [![CodeQl][codeql-image]][codeql-url]
+[![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
-[![pre-commit][pre-commit-image]][pre-commit-url]
+[![CodeFactor][codefactor-image]][codefactor-url]
+[![Codeclimate][codeclimate-image]][codeclimate-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
@@ -71,30 +75,30 @@
 With further investigation I noticed that pip-tools had pinned flake8 to an earlier version to what pre-commit was caching.
 
 In short - pip-tools does a spectacularly good job pinning your dependencies and the dependencies of these dependencies. It has one job to do and it does it perfectly.
 The pre-commit autoupdate command just updates the "rev" for the "repo" in the .pre-commit-config.yaml file to the latest version available and ignores the dependencies.
 
 The following example displays the way flake8 and a few plugins are configured by the two tools :
 
-- pip-tools (via requirements.txt)
+-   pip-tools (via requirements.txt)
 
 ```shell
 flake8==4.0.1
     # via ...
 flake8-bugbear==22.8.23
     # via ...
 flake8-comprehensions==3.10.0
     # via ...
 flake8-eradicate==1.3.0
     # via ...
 flake8-simplify==0.19.3
     # via ...
 ```
 
-- pre-commit (via .pre-commit-config.yaml)
+-   pre-commit (via .pre-commit-config.yaml)
 
 ```shell
   - repo: https://github.com/pycqa/flake8
     rev 5.0.4
     hooks:
       - id: flake8
         additional_dependencies:
@@ -201,28 +205,28 @@
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://piptools-sync.readthedocs.io/en/latest/?)
 
-- [**Example Usage**](https://piptools-sync.readthedocs.io/en/latest/example.html)
-- [**Credits**](https://piptools-sync.readthedocs.io/en/latest/example.html)
-- [**Changelog**](https://piptools-sync.readthedocs.io/en/latest/changelog.html)
-- [**API Reference**](https://piptools-sync.readthedocs.io/en/latest/autoapi/index.html)
+-   [**Example Usage**](https://piptools-sync.readthedocs.io/en/latest/example.html)
+-   [**Credits**](https://piptools-sync.readthedocs.io/en/latest/example.html)
+-   [**Changelog**](https://piptools-sync.readthedocs.io/en/latest/changelog.html)
+-   [**API Reference**](https://piptools-sync.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**](https://github.com/Stephen-RA-King/piptools-sync/wiki)
 
 ## Future Enhancements
 
 ---
 
-- Move some global variables into a separate settings file (toml).
-- Settings configurable from the command line (and therefore configurable from the pre-commit.yaml file).
-- Improve web request performance with asyncio / aiohttp libraries.
+-   Move some global variables into a separate settings file (toml).
+-   Settings configurable from the command line (and therefore configurable from the pre-commit.yaml file).
+-   Improve web request performance with asyncio / aiohttp libraries.
 
 ## Meta
 
 ---
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
```

### Comparing `piptools_sync-1.0.3/README.md` & `piptools_sync-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,21 @@
 
 _**A pre-commit plugin to align pre-commit repository versions with those derived by pip-tools.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
-[![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
-[![pre-commit.ci][pre-commit.ci-image]][pre-commit.ci-url]
-[![CodeFactor][codefactor-image]][codefactor-url]
-[![Codeclimate][codeclimate-image]][codeclimate-url]
 [![CodeQl][codeql-image]][codeql-url]
+[![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
-[![pre-commit][pre-commit-image]][pre-commit-url]
+[![CodeFactor][codefactor-image]][codefactor-url]
+[![Codeclimate][codeclimate-image]][codeclimate-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
@@ -45,30 +43,30 @@
 With further investigation I noticed that pip-tools had pinned flake8 to an earlier version to what pre-commit was caching.
 
 In short - pip-tools does a spectacularly good job pinning your dependencies and the dependencies of these dependencies. It has one job to do and it does it perfectly.
 The pre-commit autoupdate command just updates the "rev" for the "repo" in the .pre-commit-config.yaml file to the latest version available and ignores the dependencies.
 
 The following example displays the way flake8 and a few plugins are configured by the two tools :
 
-- pip-tools (via requirements.txt)
+-   pip-tools (via requirements.txt)
 
 ```shell
 flake8==4.0.1
     # via ...
 flake8-bugbear==22.8.23
     # via ...
 flake8-comprehensions==3.10.0
     # via ...
 flake8-eradicate==1.3.0
     # via ...
 flake8-simplify==0.19.3
     # via ...
 ```
 
-- pre-commit (via .pre-commit-config.yaml)
+-   pre-commit (via .pre-commit-config.yaml)
 
 ```shell
   - repo: https://github.com/pycqa/flake8
     rev 5.0.4
     hooks:
       - id: flake8
         additional_dependencies:
@@ -175,28 +173,28 @@
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://piptools-sync.readthedocs.io/en/latest/?)
 
-- [**Example Usage**](https://piptools-sync.readthedocs.io/en/latest/example.html)
-- [**Credits**](https://piptools-sync.readthedocs.io/en/latest/example.html)
-- [**Changelog**](https://piptools-sync.readthedocs.io/en/latest/changelog.html)
-- [**API Reference**](https://piptools-sync.readthedocs.io/en/latest/autoapi/index.html)
+-   [**Example Usage**](https://piptools-sync.readthedocs.io/en/latest/example.html)
+-   [**Credits**](https://piptools-sync.readthedocs.io/en/latest/example.html)
+-   [**Changelog**](https://piptools-sync.readthedocs.io/en/latest/changelog.html)
+-   [**API Reference**](https://piptools-sync.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**](https://github.com/Stephen-RA-King/piptools-sync/wiki)
 
 ## Future Enhancements
 
 ---
 
-- Move some global variables into a separate settings file (toml).
-- Settings configurable from the command line (and therefore configurable from the pre-commit.yaml file).
-- Improve web request performance with asyncio / aiohttp libraries.
+-   Move some global variables into a separate settings file (toml).
+-   Settings configurable from the command line (and therefore configurable from the pre-commit.yaml file).
+-   Improve web request performance with asyncio / aiohttp libraries.
 
 ## Meta
 
 ---
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
```

### Comparing `piptools_sync-1.0.3/pyproject.toml` & `piptools_sync-1.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 ]
 build-backend = "setuptools.build_meta"
 
 [tool]
 [tool.black]
 line-length = 88
 
-[tool.pytest.ini_options]
-# https://docs.pytest.org/en/6.2.x/reference.html?highlight=minversion#configuration-options
-minversion = "6.0"
-testpaths = [
-    "tests",
+[tool.cruft]
+skip = [
+    "tests/",
+    "src/",
+    "*/header.png",
+    ".pypirc",
+    "CHANGELOG.md",
+    "setup.cfg"
 ]
 
 [tool.isort]
 import_heading_stdlib = "Core Library modules"
 import_heading_thirdparty = "Third party modules"
 import_heading_firstparty = "First party modules"
 import_heading_localfolder = "Local modules"
@@ -48,16 +51,22 @@
 warn_unused_ignores = true
 strict_optional = true
 warn_redundant_casts = true
 warn_unused_configs = true
 disallow_untyped_calls = false
 disallow_incomplete_defs = true
 follow_imports = "skip"
-html_report = "mypy-report"
+html_report = "reports/mypy"
+cache_dir = 'cache/.mypy_cache'
 mypy_path = "typeshed/pyi:typeshed/imports"
+exclude = [
+    '^tests/[\w]*.py$',
+    '^tools/[\w]*.py$',
+    '^tasks.py$'
+]
 
 [tool.semantic_release]
 version_variable = [
     "src/piptools_sync/__init__.py:__version__",
     "README.md:rev:",
     "docs/conf.py:version",
 ]
```

### Comparing `piptools_sync-1.0.3/setup.cfg` & `piptools_sync-1.0.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -17,90 +17,121 @@
 00000100: 7369 6f6e 2073 796e 6320 7574 696c 6974  sion sync utilit
 00000110: 790d 0a6c 6f6e 675f 6465 7363 7269 7074  y..long_descript
 00000120: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
 00000130: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
 00000140: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
 00000150: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
 00000160: 646f 776e 0d0a 6b65 7977 6f72 6473 203d  down..keywords =
-00000170: 2075 7469 6c69 7479 2c0d 0a70 6c61 7466   utility,..platf
-00000180: 6f72 6d73 203d 2041 6e79 0d0a 7572 6c20  orms = Any..url 
-00000190: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-000001a0: 2e63 6f6d 2f53 7465 7068 656e 2d52 412d  .com/Stephen-RA-
-000001b0: 4b69 6e67 2f70 6970 746f 6f6c 732d 7379  King/piptools-sy
-000001c0: 6e63 0d0a 646f 776e 6c6f 6164 5f75 726c  nc..download_url
-000001d0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-000001e0: 622e 636f 6d2f 5374 6570 6865 6e2d 5241  b.com/Stephen-RA
-000001f0: 2d4b 696e 672f 7069 7074 6f6f 6c73 5f73  -King/piptools_s
-00000200: 796e 632f 6172 6368 6976 652f 7265 6673  ync/archive/refs
-00000210: 2f68 6561 6473 2f6d 6169 6e2e 7a69 700d  /heads/main.zip.
-00000220: 0a6c 6963 656e 7365 203d 204d 4954 0d0a  .license = MIT..
-00000230: 6c69 6365 6e73 655f 6669 6c65 203d 204c  license_file = L
-00000240: 4943 454e 5345 0d0a 636c 6173 7369 6669  ICENSE..classifi
-00000250: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
-00000260: 6d65 6e74 2053 7461 7475 7320 3a3a 2035  ment Status :: 5
-00000270: 202d 2050 726f 6475 6374 696f 6e2f 5374   - Production/St
-00000280: 6162 6c65 0d0a 0945 6e76 6972 6f6e 6d65  able...Environme
-00000290: 6e74 203a 3a20 436f 6e73 6f6c 650d 0a09  nt :: Console...
-000002a0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-000002b0: 6520 3a3a 2044 6576 656c 6f70 6572 730d  e :: Developers.
-000002c0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-000002d0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-000002e0: 6465 6e74 0d0a 094e 6174 7572 616c 204c  dent...Natural L
-000002f0: 616e 6775 6167 6520 3a3a 2045 6e67 6c69  anguage :: Engli
-00000300: 7368 0d0a 0950 726f 6772 616d 6d69 6e67  sh...Programming
-00000310: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000320: 686f 6e20 3a3a 2033 0d0a 0950 726f 6772  hon :: 3...Progr
-00000330: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000340: 3a3a 2050 7974 686f 6e20 3a3a 2033 203a  :: Python :: 3 :
-00000350: 3a20 4f6e 6c79 0d0a 0950 726f 6772 616d  : Only...Program
-00000360: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000370: 2050 7974 686f 6e20 3a3a 2033 2e39 0d0a   Python :: 3.9..
-00000380: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000390: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000003a0: 3a3a 2033 2e31 300d 0a0d 0a5b 6f70 7469  :: 3.10....[opti
-000003b0: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
-000003c0: 7220 3d20 0d0a 093d 7372 630d 0a70 6163  r = ...=src..pac
-000003d0: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
-000003e0: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
-000003f0: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
-00000400: 6461 7461 203d 2054 7275 650d 0a70 7974  data = True..pyt
-00000410: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-00000420: 3d33 2e38 0d0a 696e 7374 616c 6c5f 7265  =3.8..install_re
-00000430: 7175 6972 6573 203d 200d 0a09 6169 6f68  quires = ...aioh
-00000440: 7474 700d 0a09 636c 6963 6b0d 0a09 6769  ttp...click...gi
-00000450: 7470 7974 686f 6e0d 0a09 7079 7961 6d6c  tpython...pyyaml
-00000460: 0d0a 0972 6571 7565 7374 730d 0a09 746f  ...requests...to
-00000470: 6d6c 0d0a 0974 7164 6d0d 0a0d 0a5b 6f70  ml...tqdm....[op
-00000480: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000490: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-000004a0: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  c....[options.pa
-000004b0: 636b 6167 655f 6461 7461 5d0d 0a70 6970  ckage_data]..pip
-000004c0: 746f 6f6c 735f 7379 6e63 203d 200d 0a09  tools_sync = ...
-000004d0: 636f 6e66 6967 2e74 6f6d 6c0d 0a09 6d61  config.toml...ma
-000004e0: 7070 696e 672e 6a73 6f6e 0d0a 0d0a 5b6f  pping.json....[o
-000004f0: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
-00000500: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
-00000510: 7269 7074 7320 3d20 0d0a 0970 6970 746f  ripts = ...pipto
-00000520: 6f6c 735f 7379 6e63 203d 2070 6970 746f  ols_sync = pipto
-00000530: 6f6c 735f 7379 6e63 2e70 6970 746f 6f6c  ols_sync.piptool
-00000540: 735f 7379 6e63 3a6d 6169 6e0d 0a0d 0a5b  s_sync:main....[
-00000550: 666c 616b 6538 5d0d 0a64 6f63 7374 7269  flake8]..docstri
-00000560: 6e67 2d63 6f6e 7665 6e74 696f 6e20 3d20  ng-convention = 
-00000570: 6e75 6d70 790d 0a6d 6178 2d63 6f6d 706c  numpy..max-compl
-00000580: 6578 6974 7920 3d20 3138 0d0a 6d61 782d  exity = 18..max-
-00000590: 6c69 6e65 2d6c 656e 6774 6820 3d20 3838  line-length = 88
-000005a0: 0d0a 7365 6c65 6374 203d 2042 2c20 4239  ..select = B, B9
-000005b0: 2c20 432c 2044 2c20 452c 2046 2c20 4e2c  , C, D, E, F, N,
-000005c0: 2057 0d0a 6578 636c 7564 6520 3d20 7465   W..exclude = te
-000005d0: 7374 732f 2a2c 2e74 6f78 2f2a 2c2e 6e6f  sts/*,.tox/*,.no
-000005e0: 782f 2a2c 646f 6373 2f2a 2c2e 6769 742f  x/*,docs/*,.git/
-000005f0: 2a2c 2e67 6974 6875 622f 2a0d 0a69 676e  *,.github/*..ign
-00000600: 6f72 6520 3d20 0d0a 0945 3230 332c 0d0a  ore = ...E203,..
-00000610: 0957 3530 332c 0d0a 7065 722d 6669 6c65  .W503,..per-file
-00000620: 2d69 676e 6f72 6573 203d 200d 0a09 5f5f  -ignores = ...__
-00000630: 696e 6974 5f5f 2e70 793a 4634 3031 0d0a  init__.py:F401..
-00000640: 0970 6174 686d 6167 6963 2e70 793a 4634  .pathmagic.py:F4
-00000650: 3031 0d0a 0974 6573 745f 7069 7074 6f6f  01...test_piptoo
-00000660: 6c73 5f73 796e 632e 7079 3a46 3430 310d  ls_sync.py:F401.
-00000670: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000680: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000690: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000170: 2070 7265 2d63 6f6d 6d69 742d 686f 6f6b   pre-commit-hook
+00000180: 732c 7665 7273 696f 6e2d 7379 6e63 2c70  s,version-sync,p
+00000190: 6970 2d74 6f6f 6c73 2c70 7265 2d63 6f6d  ip-tools,pre-com
+000001a0: 6d69 742c 6465 7065 6e64 656e 6379 2d6d  mit,dependency-m
+000001b0: 616e 6167 6572 0d0a 706c 6174 666f 726d  anager..platform
+000001c0: 7320 3d20 416e 790d 0a75 726c 203d 2068  s = Any..url = h
+000001d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001e0: 6d2f 5374 6570 6865 6e2d 5241 2d4b 696e  m/Stephen-RA-Kin
+000001f0: 672f 7069 7074 6f6f 6c73 2d73 796e 630d  g/piptools-sync.
+00000200: 0a64 6f77 6e6c 6f61 645f 7572 6c20 3d20  .download_url = 
+00000210: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000220: 6f6d 2f53 7465 7068 656e 2d52 412d 4b69  om/Stephen-RA-Ki
+00000230: 6e67 2f70 6970 746f 6f6c 735f 7379 6e63  ng/piptools_sync
+00000240: 2f61 7263 6869 7665 2f72 6566 732f 6865  /archive/refs/he
+00000250: 6164 732f 6d61 696e 2e7a 6970 0d0a 6c69  ads/main.zip..li
+00000260: 6365 6e73 6520 3d20 4d49 540d 0a6c 6963  cense = MIT..lic
+00000270: 656e 7365 5f66 696c 6573 203d 204c 4943  ense_files = LIC
+00000280: 454e 5345 0d0a 7072 6f6a 6563 745f 7572  ENSE..project_ur
+00000290: 6c73 203d 200d 0a09 646f 6375 6d65 6e74  ls = ...document
+000002a0: 6174 696f 6e20 3d20 6874 7470 733a 2f2f  ation = https://
+000002b0: 7069 7074 6f6f 6c73 2d73 796e 632e 7265  piptools-sync.re
+000002c0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+000002d0: 6c61 7465 7374 2f0d 0a09 5265 6c65 6173  latest/...Releas
+000002e0: 6520 4e6f 7465 7320 3d20 6874 7470 733a  e Notes = https:
+000002f0: 2f2f 6769 7468 7562 2e63 6f6d 2f53 7465  //github.com/Ste
+00000300: 7068 656e 2d52 412d 4b69 6e67 2f70 6970  phen-RA-King/pip
+00000310: 746f 6f6c 735f 7379 6e63 2f72 656c 6561  tools_sync/relea
+00000320: 7365 730d 0a09 536f 7572 6365 2043 6f64  ses...Source Cod
+00000330: 6520 3d20 6874 7470 733a 2f2f 6769 7468  e = https://gith
+00000340: 7562 2e63 6f6d 2f53 7465 7068 656e 2d52  ub.com/Stephen-R
+00000350: 412d 4b69 6e67 2f70 6970 746f 6f6c 735f  A-King/piptools_
+00000360: 7379 6e63 2f0d 0a09 4973 7375 6520 5472  sync/...Issue Tr
+00000370: 6163 6b65 7220 3d20 6874 7470 733a 2f2f  acker = https://
+00000380: 6769 7468 7562 2e63 6f6d 2f53 7465 7068  github.com/Steph
+00000390: 656e 2d52 412d 4b69 6e67 2f70 6970 746f  en-RA-King/pipto
+000003a0: 6f6c 735f 7379 6e63 2f69 7373 7565 730d  ols_sync/issues.
+000003b0: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+000003c0: 0a09 4465 7665 6c6f 706d 656e 7420 5374  ..Development St
+000003d0: 6174 7573 203a 3a20 3520 2d20 5072 6f64  atus :: 5 - Prod
+000003e0: 7563 7469 6f6e 2f53 7461 626c 650d 0a09  uction/Stable...
+000003f0: 456e 7669 726f 6e6d 656e 7420 3a3a 2043  Environment :: C
+00000400: 6f6e 736f 6c65 0d0a 0949 6e74 656e 6465  onsole...Intende
+00000410: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
+00000420: 7665 6c6f 7065 7273 0d0a 094c 6963 656e  velopers...Licen
+00000430: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000440: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000450: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
+00000460: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+00000470: 656e 6465 6e74 0d0a 094e 6174 7572 616c  endent...Natural
+00000480: 204c 616e 6775 6167 6520 3a3a 2045 6e67   Language :: Eng
+00000490: 6c69 7368 0d0a 0950 726f 6772 616d 6d69  lish...Programmi
+000004a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000004b0: 7974 686f 6e20 3a3a 2033 0d0a 0950 726f  ython :: 3...Pro
+000004c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000004d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000004e0: 203a 3a20 4f6e 6c79 0d0a 0950 726f 6772   :: Only...Progr
+000004f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000500: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
+00000510: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000520: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000530: 6e20 3a3a 2033 2e31 300d 0a09 5072 6f67  n :: 3.10...Prog
+00000540: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000550: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000560: 3131 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  11....[options].
+00000570: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
+00000580: 0a09 3d73 7263 0d0a 7061 636b 6167 6573  ..=src..packages
+00000590: 203d 2066 696e 643a 0d0a 696e 636c 7564   = find:..includ
+000005a0: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
+000005b0: 2054 7275 650d 0a70 7974 686f 6e5f 7265   True..python_re
+000005c0: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
+000005d0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+000005e0: 203d 200d 0a09 6169 6f68 7474 703e 3d33   = ...aiohttp>=3
+000005f0: 2e38 2e34 0d0a 0963 6c69 636b 3e3d 382e  .8.4...click>=8.
+00000600: 312e 330d 0a09 6769 7470 7974 686f 6e3e  1.3...gitpython>
+00000610: 3d33 2e31 2e33 310d 0a09 7079 7961 6d6c  =3.1.31...pyyaml
+00000620: 3e3d 362e 300d 0a09 7265 7175 6573 7473  >=6.0...requests
+00000630: 3e3d 322e 3238 2e32 0d0a 0974 6f6d 6c3e  >=2.28.2...toml>
+00000640: 3d30 2e31 302e 320d 0a09 7471 646d 3e3d  =0.10.2...tqdm>=
+00000650: 342e 3634 2e31 0d0a 0d0a 5b6f 7074 696f  4.64.1....[optio
+00000660: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+00000670: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
+00000680: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000690: 6765 5f64 6174 615d 0d0a 7069 7074 6f6f  ge_data]..piptoo
+000006a0: 6c73 5f73 796e 6320 3d20 0d0a 0963 6f6e  ls_sync = ...con
+000006b0: 6669 672e 746f 6d6c 0d0a 096d 6170 7069  fig.toml...mappi
+000006c0: 6e67 2e6a 736f 6e0d 0a0d 0a5b 6f70 7469  ng.json....[opti
+000006d0: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
+000006e0: 5d0d 0a63 6f6e 736f 6c65 5f73 6372 6970  ]..console_scrip
+000006f0: 7473 203d 200d 0a09 7069 7074 6f6f 6c73  ts = ...piptools
+00000700: 5f73 796e 6320 3d20 7069 7074 6f6f 6c73  _sync = piptools
+00000710: 5f73 796e 632e 7069 7074 6f6f 6c73 5f73  _sync.piptools_s
+00000720: 796e 633a 6d61 696e 0d0a 0d0a 5b66 6c61  ync:main....[fla
+00000730: 6b65 385d 0d0a 646f 6373 7472 696e 672d  ke8]..docstring-
+00000740: 636f 6e76 656e 7469 6f6e 203d 206e 756d  convention = num
+00000750: 7079 0d0a 6d61 782d 636f 6d70 6c65 7869  py..max-complexi
+00000760: 7479 203d 2031 380d 0a6d 6178 2d6c 696e  ty = 18..max-lin
+00000770: 652d 6c65 6e67 7468 203d 2038 380d 0a73  e-length = 88..s
+00000780: 656c 6563 7420 3d20 422c 2042 392c 2043  elect = B, B9, C
+00000790: 2c20 442c 2045 2c20 462c 204e 2c20 570d  , D, E, F, N, W.
+000007a0: 0a65 7863 6c75 6465 203d 2074 6573 7473  .exclude = tests
+000007b0: 2f2a 2c2e 746f 782f 2a2c 2e6e 6f78 2f2a  /*,.tox/*,.nox/*
+000007c0: 2c64 6f63 732f 2a2c 2e67 6974 2f2a 2c2e  ,docs/*,.git/*,.
+000007d0: 6769 7468 7562 2f2a 0d0a 6967 6e6f 7265  github/*..ignore
+000007e0: 203d 200d 0a09 4532 3033 2c0d 0a09 5735   = ...E203,...W5
+000007f0: 3033 2c0d 0a09 4239 3037 2c0d 0a09 4431  03,...B907,...D1
+00000800: 3033 0d0a 7065 722d 6669 6c65 2d69 676e  03..per-file-ign
+00000810: 6f72 6573 203d 200d 0a09 5f5f 696e 6974  ores = ...__init
+00000820: 5f5f 2e70 793a 4634 3031 0d0a 0970 6174  __.py:F401...pat
+00000830: 686d 6167 6963 2e70 793a 4634 3031 0d0a  hmagic.py:F401..
+00000840: 0974 6573 745f 7069 7074 6f6f 6c73 5f73  .test_piptools_s
+00000850: 796e 632e 7079 3a46 3430 310d 0a0d 0a5b  ync.py:F401....[
+00000860: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000870: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000880: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `piptools_sync-1.0.3/src/piptools_sync/__init__.py` & `piptools_sync-1.0.4/src/piptools_sync/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # Core Library modules
 import logging.config
 from importlib.resources import as_file, files
 from pathlib import Path
 
 # Third party modules
 import git
-import toml  # type: ignore
-import yaml  # type: ignore
+import toml
+import yaml
 
 __title__ = "piptools-sync"
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 __author__ = "Stephen R A King"
 __description__ = "A piptools pre-commit version sync utility"
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022 Stephen R A King"
```

### Comparing `piptools_sync-1.0.3/src/piptools_sync/mapping.json` & `piptools_sync-1.0.4/src/piptools_sync/mapping.json`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.3/src/piptools_sync/piptools_sync.py` & `piptools_sync-1.0.4/src/piptools_sync/piptools_sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python3
-"""A pre-commit utility plugin to verify requirement versions determined by
-pip-tools are utilized by pre-commit
-"""
+"""A pre-commit plugin to sync versions from pip-tools to pre-commit."""
 
 # Core Library modules
 import json
 import os
 import time
 from importlib.metadata import PackageNotFoundError, version as ver
+from importlib.resources import as_file
 from pathlib import Path
 from typing import Any, Union
 
 # Third party modules
-import requests  # type:ignore
-import yaml  # type:ignore
+import requests
+import yaml
 from tqdm import tqdm
 
 # Local modules
 from . import MAPPING_FILE, ROOT_DIR, logger, toml_config
 
 PRECOMMIT_CONFIG_FILE = ".pre-commit-config.yaml"
 PRECOMMIT_REPOS_URL = "https://pre-commit.com/all-hooks.json"
@@ -30,15 +29,15 @@
     "https://github.com/pre-commit/mirrors-mypy": "mypy",
     "https://github.com/pre-commit/mirrors-yapf": "yapf",
     "https://github.com/FalconSocial/pre-commit-mirrors-pep257": "pep257",
 }
 
 
 def load_settings() -> None:
-    """Get the configuration settings from the toml file"""
+    """Get the configuration settings from the toml file."""
     debug_config = [(bool(toml_config["APP"]["DEBUG"]))]  # noqa
     if not debug_config:
         logger.disabled = True
 
 
 def _utility_find_file_path(partial_path: str) -> Union[Path, int]:
     """Given a partial file path, find the absolute file path for the file.
@@ -189,25 +188,28 @@
         raise SystemExit(e) from None
 
 
 def get_latest_pypi_repo_version(name: str) -> Union[str, int]:
     """Given a repository name , find the latest version utilizing PyPI API.
 
     Parameters
+    ----------
     name : str
         Supplied project name. This is not the URL.
 
     Returns
+    -------
     version : str
         The latest repository version.
 
     0 :
         Indicates the repository was not found.
 
     Raises
+    ------
     SystemExit:
         if requests.get() operations fails for any reason.
     """
     logger.debug("starting **** get_precommit_repos ****")
     int_url = "https://pypi.org/pypi/<project>/json"
     dst_url = int_url.replace("<project>", name)
     headers = {"Accept": "application/json"}
@@ -222,33 +224,35 @@
             logger.debug("%s - for %s", version, name)
             return version
     except requests.exceptions.RequestException as e:
         raise SystemExit(e) from None
 
 
 def generate_db(force: int = 0) -> dict[str, str]:
-    """Generate a mapping from pre-commit repo to PyPI repo
+    """Generate a mapping from pre-commit repo to PyPI repo.
 
     Generates a dictionary data structure:
     key : pre-commit URL
     value : PyPi project name
     e.g. {"https://github.com/pre-commit/pre-commit-hooks": "pre-commit-hooks",}
 
     Parameters
+    ----------
     force : int
         When set to 1 will force the generation of a new mapping
 
     Returns
+    -------
     mapping : dict
         the mapping dictionary
     """
     logger.debug("starting **** generate_db ****")
 
     def generate_file() -> dict:
-        """Create the mapping dictionary is it does not exist or is out of date"""
+        """Create the mapping dictionary is it does not exist or is out of date."""
         mapping_db = {}
         pyrepos = get_precommit_repos()
         logger.debug("List of precommit repositories: %s", pyrepos)
         for repo in tqdm(pyrepos):
             inta_repo, *_ = repo
             inta_repo = inta_repo.lower()
             mapping_db[inta_repo] = ""
@@ -257,40 +261,41 @@
                 mapping_db[inta_repo] = MANUAL_MAPPING[inta_repo]
             else:
                 *_, project = inta_repo.split("/")
                 result = get_latest_pypi_repo_version(project)
                 if result != 0:
                     logger.debug("project found on PyPI...mapping value to key")
                     mapping_db[inta_repo] = project
-        with open(MAPPING_FILE, "w") as outfile:
+        with MAPPING_FILE.open("w") as outfile:
             json.dump(mapping_db, outfile)
         return mapping_db
 
-    if not MAPPING_FILE.exists() or force == 1 or MAPPING_FILE.stat().st_size < 5:
-        logger.debug("Generating new mapping")
-        mapping = generate_file()
-    elif int(time.time() - os.path.getmtime(MAPPING_FILE)) > REGEN_PERIOD:
-        logger.debug("mapping expired... Generating a new mapping")
-        mapping = generate_file()
-    else:
-        logger.debug("Reusing mapping")
-        with open(MAPPING_FILE) as infile:  # type: ignore
-            mapping = json.load(infile)
-
+    with as_file(MAPPING_FILE) as mapping_file:
+        if not mapping_file.exists() or force == 1 or mapping_file.stat().st_size < 5:
+            logger.debug("Generating new mapping")
+            mapping = generate_file()
+        elif int(time.time() - os.path.getmtime(mapping_file)) > REGEN_PERIOD:
+            logger.debug("mapping expired... Generating a new mapping")
+            mapping = generate_file()
+        else:
+            logger.debug("Reusing mapping")
+            mapping = json.loads(MAPPING_FILE.read_text(encoding="utf-8"))
     return mapping
 
 
 def find_yaml_config_file() -> Path:
     """Find the '.pre-commit-config.yaml' config file in the project directory.
 
     Returns
+    -------
     pc_file : Path
         Path object for the configuration file.
 
-    Raise
+    Raises
+    ------
     FileNotFoundError :
         If the config file cannot be found.
     """
     logger.debug("starting **** find_yaml_config_file ****")
     file_list_text = list(ROOT_DIR.iterdir())
     file_list_path = [Path(i) for i in file_list_text]
     for filepath in file_list_path:
@@ -306,37 +311,42 @@
 
     yaml data structure in python is {"repos": [ { }, { }, { } ] }
     so to get an individual repo & rev:
     1st repo - data["repos"][0]["repo"]
     1st rev - data["repos"][0]["rev"]
 
     Parameters
+    ----------
     yaml_file : Path
         Pathlib.Path object to configuration file.
 
     Returns
+    -------
     repos : dict
         Dictionary object mapping repository name to version.
     """
     logger.debug("starting **** yaml_to_dict ****")
     with open(yaml_file) as f:
         yaml_contents = yaml.safe_load(f)
     repos = {}
     for _, repo in enumerate(yaml_contents["repos"]):
+        if repo["repo"] in ("local", "meta"):
+            continue
         version = repo["rev"]
         version = _utility_remove_vee(version)
         repos[repo["repo"].strip().lower()] = version.strip()
     logger.debug("%s", repos)
     return repos
 
 
 def update_yaml(yaml_file: Path, repo: str, version: str) -> None:
-    """update a repo in the '.pre-commit-config.yaml' file with the given version.
+    """Update a repo in the '.pre-commit-config.yaml' file with the given version.
 
     Parameters
+    ----------
     yaml_file : Path
         pathlib.Path object to the pre-commit config file.
     repo : str
         The URL string of the Repository to update.
     version : str
         String representation of the version to apply.
     """
@@ -361,14 +371,15 @@
 def find_requirements_file() -> Any:
     """Find the first piptools generated file in the pip requirements tree.
 
     Given the root requirements file find and verify the final layered
     requirements file is a pip-tools generated file.
 
     Returns
+    -------
     result : Path
         The pathlib.Path object to the derived requirement file.
     """
     logger.debug("starting **** find_requirements_file function ****")
     logger.debug("root requirement: %s", ROOT_REQUIREMENT)
 
     def next_file(req_file: Path) -> Any:
@@ -407,18 +418,20 @@
 def get_installed_version(package: str) -> Union[str, None]:
     """Return installed package version given the package name.
 
     This is the package version installed by pip and not the version in the
     requirements file or the pre-commit-config.yaml file
 
     Parameters
+    ----------
     package : str
         The name of the installed package.
 
     Returns
+    -------
     installed_version : str
         version of the package installed by pip.
 
     None :
         if the package is not found
     """
     logger.debug("starting **** get_installed_version function ****")
@@ -431,20 +444,22 @@
         return None
 
 
 def get_requirement_versions(req_file: Path, req_list: list) -> dict:
     """Get the repo version from the requirements file.
 
     Parameters
+    ----------
     req_file : Path
         pathlib.Path object for the derived requirements file.
     req_list : list
         A list comprising packages that need versions.
 
     Returns
+    -------
     req_version_list : dict
         A Dictionary comprising key: package name, Value: the version
         e.g. {'click': '8.1.3'}
     """
     logger.debug("starting **** get_requirement_versions function ****")
     req_version_list = {}
     with open(req_file) as f:
```

### Comparing `piptools_sync-1.0.3/src/piptools_sync.egg-info/PKG-INFO` & `piptools_sync-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 Metadata-Version: 2.1
-Name: piptools-sync
-Version: 1.0.3
+Name: piptools_sync
+Version: 1.0.4
 Summary: A piptools pre-commit version sync utility
 Home-page: https://github.com/Stephen-RA-King/piptools-sync
 Download-URL: https://github.com/Stephen-RA-King/piptools_sync/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
 License: MIT
-Keywords: utility
+Project-URL: documentation, https://piptools-sync.readthedocs.io/en/latest/
+Project-URL: Release Notes, https://github.com/Stephen-RA-King/piptools_sync/releases
+Project-URL: Source Code, https://github.com/Stephen-RA-King/piptools_sync/
+Project-URL: Issue Tracker, https://github.com/Stephen-RA-King/piptools_sync/issues
+Keywords: pre-commit-hooks,version-sync,pip-tools,pre-commit,dependency-manager
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Piptools-sync
 
 ---
 
 _**A pre-commit plugin to align pre-commit repository versions with those derived by pip-tools.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
-[![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
-[![pre-commit.ci][pre-commit.ci-image]][pre-commit.ci-url]
-[![CodeFactor][codefactor-image]][codefactor-url]
-[![Codeclimate][codeclimate-image]][codeclimate-url]
 [![CodeQl][codeql-image]][codeql-url]
+[![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
-[![pre-commit][pre-commit-image]][pre-commit-url]
+[![CodeFactor][codefactor-image]][codefactor-url]
+[![Codeclimate][codeclimate-image]][codeclimate-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
@@ -71,30 +75,30 @@
 With further investigation I noticed that pip-tools had pinned flake8 to an earlier version to what pre-commit was caching.
 
 In short - pip-tools does a spectacularly good job pinning your dependencies and the dependencies of these dependencies. It has one job to do and it does it perfectly.
 The pre-commit autoupdate command just updates the "rev" for the "repo" in the .pre-commit-config.yaml file to the latest version available and ignores the dependencies.
 
 The following example displays the way flake8 and a few plugins are configured by the two tools :
 
-- pip-tools (via requirements.txt)
+-   pip-tools (via requirements.txt)
 
 ```shell
 flake8==4.0.1
     # via ...
 flake8-bugbear==22.8.23
     # via ...
 flake8-comprehensions==3.10.0
     # via ...
 flake8-eradicate==1.3.0
     # via ...
 flake8-simplify==0.19.3
     # via ...
 ```
 
-- pre-commit (via .pre-commit-config.yaml)
+-   pre-commit (via .pre-commit-config.yaml)
 
 ```shell
   - repo: https://github.com/pycqa/flake8
     rev 5.0.4
     hooks:
       - id: flake8
         additional_dependencies:
@@ -201,28 +205,28 @@
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://piptools-sync.readthedocs.io/en/latest/?)
 
-- [**Example Usage**](https://piptools-sync.readthedocs.io/en/latest/example.html)
-- [**Credits**](https://piptools-sync.readthedocs.io/en/latest/example.html)
-- [**Changelog**](https://piptools-sync.readthedocs.io/en/latest/changelog.html)
-- [**API Reference**](https://piptools-sync.readthedocs.io/en/latest/autoapi/index.html)
+-   [**Example Usage**](https://piptools-sync.readthedocs.io/en/latest/example.html)
+-   [**Credits**](https://piptools-sync.readthedocs.io/en/latest/example.html)
+-   [**Changelog**](https://piptools-sync.readthedocs.io/en/latest/changelog.html)
+-   [**API Reference**](https://piptools-sync.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**](https://github.com/Stephen-RA-King/piptools-sync/wiki)
 
 ## Future Enhancements
 
 ---
 
-- Move some global variables into a separate settings file (toml).
-- Settings configurable from the command line (and therefore configurable from the pre-commit.yaml file).
-- Improve web request performance with asyncio / aiohttp libraries.
+-   Move some global variables into a separate settings file (toml).
+-   Settings configurable from the command line (and therefore configurable from the pre-commit.yaml file).
+-   Improve web request performance with asyncio / aiohttp libraries.
 
 ## Meta
 
 ---
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
```

### Comparing `piptools_sync-1.0.3/src/piptools_sync.egg-info/PKG-INFO.rum-bak` & `piptools_sync-1.0.4/src/piptools_sync.egg-info/PKG-INFO.rum-bak`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.3/src/piptools_sync.egg-info/SOURCES.txt` & `piptools_sync-1.0.4/src/piptools_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.3/tests/test__utility_find_file_path.py` & `piptools_sync-1.0.4/tests/test__utility_find_file_path.py`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.3/tests/test__utility_remove_vee.py` & `piptools_sync-1.0.4/tests/test__utility_remove_vee.py`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.3/tests/test_find_requirements_file.py` & `piptools_sync-1.0.4/tests/test_find_requirements_file.py`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.3/tests/test_generate_db.py` & `piptools_sync-1.0.4/tests/test_generate_db.py`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.3/tests/test_get_requirement_versions.py` & `piptools_sync-1.0.4/tests/test_get_requirement_versions.py`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.3/tests/test_update_yaml.py` & `piptools_sync-1.0.4/tests/test_update_yaml.py`

 * *Files identical despite different names*

