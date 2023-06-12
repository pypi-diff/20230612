# Comparing `tmp/mappr-0.3.4.tar.gz` & `tmp/mappr-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mappr-0.3.4.tar", max compression
+gzip compressed data, was "mappr-0.3.5.tar", max compression
```

## Comparing `mappr-0.3.4.tar` & `mappr-0.3.5.tar`

### file list

```diff
@@ -1,30 +1,72 @@
--rw-r--r--   0        0        0        0 2022-08-01 15:08:17.000000 mappr-0.3.4/.venv/lib/python3.7/site-packages/_pytest/py.typed
--rw-r--r--   0        0        0        0 2022-08-01 15:08:05.000000 mappr-0.3.4/.venv/lib/python3.7/site-packages/attr/py.typed
--rw-r--r--   0        0        0        0 2022-08-01 15:07:59.000000 mappr-0.3.4/.venv/lib/python3.7/site-packages/importlib_metadata/py.typed
--rw-r--r--   0        0        0        0 2022-08-01 15:08:04.000000 mappr-0.3.4/.venv/lib/python3.7/site-packages/iniconfig/py.typed
--rw-r--r--   0        0        0       64 2022-08-01 15:08:25.000000 mappr-0.3.4/.venv/lib/python3.7/site-packages/mypy/py.typed
--rw-r--r--   0        0        0        0 2022-08-01 15:08:06.000000 mappr-0.3.4/.venv/lib/python3.7/site-packages/packaging/py.typed
--rw-r--r--   0        0        0        0 2022-08-01 15:08:08.000000 mappr-0.3.4/.venv/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
--rw-r--r--   0        0        0        0 2022-08-01 15:08:08.000000 mappr-0.3.4/.venv/lib/python3.7/site-packages/py/py.typed
--rw-r--r--   0        0        0        0 2022-08-01 15:08:24.000000 mappr-0.3.4/.venv/lib/python3.7/site-packages/pydantic/py.typed
--rw-r--r--   0        0        0        0 2022-08-01 15:08:18.000000 mappr-0.3.4/.venv/lib/python3.7/site-packages/pytest/py.typed
--rw-r--r--   0        0        0        0 2022-08-01 15:08:18.000000 mappr-0.3.4/.venv/lib/python3.7/site-packages/sphinx/py.typed
--rw-r--r--   0        0        0      239 2022-08-01 15:51:26.256982 mappr-0.3.4/AUTHORS
--rw-r--r--   0        0        0    11357 2022-08-01 15:51:26.256982 mappr-0.3.4/LICENSE
--rw-r--r--   0        0        0     3847 2022-08-01 15:51:26.256982 mappr-0.3.4/README.rst
--rw-r--r--   0        0        0     4241 2022-08-01 15:51:26.256982 mappr-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      785 2022-08-01 15:51:26.256982 mappr-0.3.4/src/mappr/__init__.py
--rw-r--r--   0        0        0     1759 2022-08-01 15:51:26.256982 mappr-0.3.4/src/mappr/conversion.py
--rw-r--r--   0        0        0      105 2022-08-01 15:51:26.256982 mappr-0.3.4/src/mappr/enums.py
--rw-r--r--   0        0        0      661 2022-08-01 15:51:26.256982 mappr-0.3.4/src/mappr/exc.py
--rw-r--r--   0        0        0      269 2022-08-01 15:51:26.256982 mappr-0.3.4/src/mappr/integrations/__init__.py
--rw-r--r--   0        0        0      358 2022-08-01 15:51:26.256982 mappr-0.3.4/src/mappr/integrations/pydantic.py
--rw-r--r--   0        0        0      270 2022-08-01 15:51:26.256982 mappr-0.3.4/src/mappr/integrations/sqlalchemy.py
--rw-r--r--   0        0        0     1146 2022-08-01 15:51:26.256982 mappr-0.3.4/src/mappr/iterators.py
--rw-r--r--   0        0        0     3276 2022-08-01 15:51:26.256982 mappr-0.3.4/src/mappr/mappers.py
--rw-r--r--   0        0        0        0 2022-08-01 15:51:26.256982 mappr-0.3.4/src/mappr/py.typed
--rw-r--r--   0        0        0     2742 2022-08-01 15:51:26.256982 mappr-0.3.4/src/mappr/registry.py
--rw-r--r--   0        0        0      185 2022-08-01 15:51:26.256982 mappr-0.3.4/src/mappr/testing.py
--rw-r--r--   0        0        0     1000 2022-08-01 15:51:26.256982 mappr-0.3.4/src/mappr/types.py
--rw-r--r--   0        0        0      598 2022-08-01 15:51:33.322399 mappr-0.3.4/setup.py
--rw-r--r--   0        0        0      565 2022-08-01 15:51:33.322650 mappr-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/_pytest/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/attr/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/attrs/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/certifi/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/charset_normalizer/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/idna/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/iniconfig/py.typed
+-rw-r--r--   0        0        0       26 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/isort/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/jinja2/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/markupsafe/py.typed
+-rw-r--r--   0        0        0       64 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/mypy/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/packaging/py.typed
+-rw-r--r--   0        0        0      286 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/pip/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/platformdirs/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/py/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/pyparsing/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/pytest/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/soupsieve/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/sphinx/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/termcolor/py.typed
+-rw-r--r--   0        0        0       26 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/tomli/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/tomlkit/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/.venv/lib/python3.8/site-packages/unidecode/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:54.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/_pytest/py.typed
+-rw-r--r--   0        0        0       59 2023-06-12 02:43:47.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/babel/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:38.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/certifi/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:39.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/charset_normalizer/py.typed
+-rw-r--r--   0        0        0       72 2023-06-12 02:43:53.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/coverage/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:45.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/exceptiongroup/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:38.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/idna/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:46.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/importlib_metadata/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:43.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/iniconfig/py.typed
+-rw-r--r--   0        0        0       26 2023-06-12 02:43:59.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:59.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/isort/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:46.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/jinja2/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:38.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/markupsafe/py.typed
+-rw-r--r--   0        0        0       64 2023-06-12 02:44:00.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/mypy/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:46.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/packaging/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/peltak_changelog/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/peltak_todos/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:59.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/pydantic/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:54.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/pytest/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:45.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/soupsieve/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:54.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/sphinx/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:58.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:52.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/termcolor/py.typed
+-rw-r--r--   0        0        0       26 2023-06-12 02:43:44.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/tomli/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:52.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/tomlkit/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 02:43:46.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/unidecode/py.typed
+-rw-r--r--   0        0        0       93 2023-06-12 02:43:38.000000 mappr-0.3.5/.venv/lib/python3.8/site-packages/urllib3/py.typed
+-rw-r--r--   0        0        0      239 2023-06-12 02:47:46.093393 mappr-0.3.5/AUTHORS
+-rw-r--r--   0        0        0    11357 2023-06-12 02:47:46.093393 mappr-0.3.5/LICENSE
+-rw-r--r--   0        0        0     3847 2023-06-12 02:47:46.093393 mappr-0.3.5/README.rst
+-rw-r--r--   0        0        0     3652 2023-06-12 02:47:46.097393 mappr-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      708 2023-06-12 02:47:46.097393 mappr-0.3.5/src/mappr/__init__.py
+-rw-r--r--   0        0        0     1759 2023-06-12 02:47:46.097393 mappr-0.3.5/src/mappr/conversion.py
+-rw-r--r--   0        0        0      105 2023-06-12 02:47:46.097393 mappr-0.3.5/src/mappr/enums.py
+-rw-r--r--   0        0        0      661 2023-06-12 02:47:46.097393 mappr-0.3.5/src/mappr/exc.py
+-rw-r--r--   0        0        0      267 2023-06-12 02:47:46.097393 mappr-0.3.5/src/mappr/integrations/__init__.py
+-rw-r--r--   0        0        0      358 2023-06-12 02:47:46.097393 mappr-0.3.5/src/mappr/integrations/pydantic.py
+-rw-r--r--   0        0        0      270 2023-06-12 02:47:46.097393 mappr-0.3.5/src/mappr/integrations/sqlalchemy.py
+-rw-r--r--   0        0        0     1146 2023-06-12 02:47:46.097393 mappr-0.3.5/src/mappr/iterators.py
+-rw-r--r--   0        0        0     3276 2023-06-12 02:47:46.097393 mappr-0.3.5/src/mappr/mappers.py
+-rw-r--r--   0        0        0        0 2023-06-12 02:47:46.097393 mappr-0.3.5/src/mappr/py.typed
+-rw-r--r--   0        0        0     2742 2023-06-12 02:47:46.097393 mappr-0.3.5/src/mappr/registry.py
+-rw-r--r--   0        0        0      185 2023-06-12 02:47:46.097393 mappr-0.3.5/src/mappr/testing.py
+-rw-r--r--   0        0        0     1002 2023-06-12 02:47:46.097393 mappr-0.3.5/src/mappr/types.py
+-rw-r--r--   0        0        0      731 2023-06-12 02:47:52.610911 mappr-0.3.5/setup.py
+-rw-r--r--   0        0        0      563 2023-06-12 02:47:52.611179 mappr-0.3.5/PKG-INFO
```

### Comparing `mappr-0.3.4/LICENSE` & `mappr-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mappr-0.3.4/README.rst` & `mappr-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `mappr-0.3.4/pyproject.toml` & `mappr-0.3.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,45 @@
+[tool]
 [tool.poetry]
 name = "mappr"
-version = "0.3.4"
+version = "0.3.5"
 description = ""
 authors = ["Mateusz Klos <novopl@gmail.com>"]
 repository = "https://github.com/novopl/mappr"
 homepage = "https://novopl.github.io/mappr"
 documentation = "https://novopl.github.io/mappr"
 license = "Proprietary"
 packages = [
     { include = "mappr", from = "src" },
 ]
 include = ["LICENSE", "AUTHORS", "README.rst", "**/py.typed"]
 exclude = ["tests/**", "ops/**", ".venv/**"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = ">=3.8.1,<4.0"
+peltak-changelog = "^0.0.4"
+peltak-todos = "^0.0.10"
 
 [tool.poetry.dev-dependencies]
-coverage = "~=5.3"
-mypy = ">=0.790"
-peltak = "~=0.27.1"
-psutil = "~=5.7.3"
-pycodestyle = "~=2.6.0"
-pylint = "~=2.6.0"
-pytest = "~=6.1.2"
-pytest-cov = "~=2.10.1"
-pytest-sugar = "~=0.9.4"
+codecov = "^2.1.13"
+coverage = "^7.2.7"
+flake8 = "^6.0.0"
+mypy = "^1.3.0"
+peltak = "^0.30.0"
+pycodestyle = "^2.10.0"
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
+pytest-sugar = "^0.9.7"
 pydantic = "^1.7.3"
-sphinx-material = "^0.0.32"
-flake8 = "^3.8.4"
-Sphinx = "^3.4.3"
-sphinx-autodoc-typehints = "^1.11.1"
-codecov = "^2.1.11"
 SQLAlchemy = "^1.3.22"
+Sphinx = "^7.0.1"
+sphinx-autodoc-typehints = "^1.23.4"
+sphinx-material = "^0.0.35"
+isort = "^5.12.0"
 
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-
-##################
-#     PYTEST     #
-##################
-
-
-[tool.pytest.ini_options]
-addopts = "--durations=3"
-doctest_optionflags = "NORMALIZE_WHITESPACE IGNORE_EXCEPTION_DETAIL ELLIPSIS"
-
-[tool.coverage.run]
-branch = true
-source = ["src"]
-
-[tool.coverage.report]
-exclude_lines = ["nocov"]
-
-
-##################
-#     PYLINT     #
-##################
-
-[tool.pylint.MASTER]
-jobs = 1
-ignore = 'migrations'
-ignore-patterns = []
-
-[tool.pylint.REPORTS]
-output-format = 'colorized'
-reports = 'no'
-
-[tool.pylint.'MESSAGES CONTROL']
-disable = 'all'
-enable = [
-    # 'missing-docstring',
-    'redefined-builtin',
-    'wrong-import-order',
-]
-
-
-##################
-#     PELTAK     #
-##################
 
 [tool.peltak]
 pelconf_version = "0"
 commands = [
   "peltak.extra.changelog",
   "peltak.extra.git",
   "peltak.extra.gitflow",
@@ -190,7 +145,16 @@
 about = "Create PR for the current release branch"
 command = """
 gh pr create \
     --repo novopl/mappr \
     --title "Release: v$(peltak version --porcelain)" \
     --body "$(peltak changelog)"
 """
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+##################
+#     PELTAK     #
+##################
+
```

### Comparing `mappr-0.3.4/src/mappr/conversion.py` & `mappr-0.3.5/src/mappr/conversion.py`

 * *Files identical despite different names*

### Comparing `mappr-0.3.4/src/mappr/exc.py` & `mappr-0.3.5/src/mappr/exc.py`

 * *Files identical despite different names*

### Comparing `mappr-0.3.4/src/mappr/iterators.py` & `mappr-0.3.5/src/mappr/iterators.py`

 * *Files identical despite different names*

### Comparing `mappr-0.3.4/src/mappr/mappers.py` & `mappr-0.3.5/src/mappr/mappers.py`

 * *Files identical despite different names*

### Comparing `mappr-0.3.4/src/mappr/registry.py` & `mappr-0.3.5/src/mappr/registry.py`

 * *Files identical despite different names*

### Comparing `mappr-0.3.4/src/mappr/types.py` & `mappr-0.3.5/src/mappr/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import dataclasses
 from typing import Any, Callable, Dict, Iterator, Type
+
 from .enums import Strategy
 
+
 ConverterFn = Callable[[Any], Any]
 MappingFn = Callable[[Any], Any]
 FieldMapping = Dict[str, MappingFn]
 FieldIterator = Iterator[str]
 TestFn = Callable[[Type], bool]
```

### Comparing `mappr-0.3.4/PKG-INFO` & `mappr-0.3.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mappr
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Home-page: https://novopl.github.io/mappr
 License: Proprietary
 Author: Mateusz Klos
 Author-email: novopl@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: peltak-changelog (>=0.0.4,<0.0.5)
+Requires-Dist: peltak-todos (>=0.0.10,<0.0.11)
 Project-URL: Documentation, https://novopl.github.io/mappr
 Project-URL: Repository, https://github.com/novopl/mappr
```

