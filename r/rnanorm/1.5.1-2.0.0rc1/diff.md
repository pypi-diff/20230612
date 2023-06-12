# Comparing `tmp/rnanorm-1.5.1.tar.gz` & `tmp/rnanorm-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnanorm-1.5.1.tar", last modified: Tue May 24 11:37:29 2022, max compression
+gzip compressed data, was "rnanorm-2.0.0rc1.tar", last modified: Mon Jun 12 08:22:10 2023, max compression
```

## Comparing `rnanorm-1.5.1.tar` & `rnanorm-2.0.0rc1.tar`

### file list

```diff
@@ -1,7 +1,59 @@
--rw-r--r--   0        0        0     2794 2022-05-24 11:36:53.921111 rnanorm-1.5.1/README.rst
--rw-r--r--   0        0        0     1417 2022-05-24 11:36:53.921111 rnanorm-1.5.1/pyproject.toml
--rw-r--r--   0        0        0       71 2022-05-24 11:36:53.921111 rnanorm-1.5.1/src/rnanorm/__init__.py
--rw-r--r--   0        0        0     6049 2022-05-24 11:36:53.921111 rnanorm-1.5.1/src/rnanorm/__main__.py
--rw-r--r--   0        0        0     2854 2022-05-24 11:36:53.921111 rnanorm-1.5.1/src/rnanorm/annotation.py
--rw-r--r--   0        0        0     5593 2022-05-24 11:36:53.921111 rnanorm-1.5.1/src/rnanorm/normalization.py
--rw-r--r--   0        0        0      218 1970-01-01 00:00:00.000000 rnanorm-1.5.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.215154 rnanorm-2.0.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.207154 rnanorm-2.0.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.211154 rnanorm-2.0.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-12 08:22:10.215154 rnanorm-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.211154 rnanorm-2.0.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/docs/guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/docs/ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-12 08:22:10.215154 rnanorm-2.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.211154 rnanorm-2.0.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.211154 rnanorm-2.0.0rc1/src/rnanorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.211154 rnanorm-2.0.0rc1/src/rnanorm/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    74590 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/files/gencode.v26.annotation.chr21.gtf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    23755 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/files/gtex_lung.first30.chr21.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/files/prepare_gtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.215154 rnanorm-2.0.0rc1/src/rnanorm/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/methods/between_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/methods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/methods/within_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.211154 rnanorm-2.0.0rc1/src/rnanorm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-12 08:22:10.000000 rnanorm-2.0.0rc1/src/rnanorm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-12 08:22:10.000000 rnanorm-2.0.0rc1/src/rnanorm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:22:10.000000 rnanorm-2.0.0rc1/src/rnanorm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-12 08:22:10.000000 rnanorm-2.0.0rc1/src/rnanorm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-12 08:22:10.000000 rnanorm-2.0.0rc1/src/rnanorm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 08:22:10.000000 rnanorm-2.0.0rc1/src/rnanorm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.215154 rnanorm-2.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.215154 rnanorm-2.0.0rc1/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/files/gtex.lung.30.chr21.tmm_factors_edgeR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/files/gtex.lung.30.chr21.uq_factors_edgeR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_cpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_cuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_fpkm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_library_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_tmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_tpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_uq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tox.ini
```

### Comparing `rnanorm-1.5.1/pyproject.toml` & `rnanorm-2.0.0rc1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,85 @@
 [build-system]
-requires = ["flit_core >=2,<3"]
-build-backend = "flit_core.buildapi"
-
-[tool.black]
-target-version = ["py38"]
-line-length = 119
-
-[tool.flit.metadata]
-module = "rnanorm"
-author = "Genialis, Inc."
-author-email = "miha@genialis.com"
-home-page="https://github.com/genialis/rnaseq-normalization/"
-description-file = "README.rst"
-requires-python=">=3.6, <3.11"
 requires = [
-    "numpy",
-    "pandas",
-    "scipy",
-    "pybedtools",
+    "setuptools >= 64.0.0",
+    "setuptools_scm >= 6.4.0",
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "rnanorm"
+description = "Common RNAseq normalization methods"
+authors = [
+    {name = "Genialis, Inc."},
+    {email = "dev-team@genialis.com"},
+]
+dynamic = ["version"]
+readme = "README.rst"
+license = {text = "Proprietary"}
+requires-python = ">=3.8, <3.11"
+keywords = [
+    "bio",
+    "bioinformatics",
+    "data science",
+    "machine learning",
+    "artificial intelligence",
+    "python",
+    "genialis",
 ]
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 4 - Beta",
+    "Environment :: Console",
     "Intended Audience :: Developers",
-    "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
-    "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
+dependencies = [
+    "click",
+    "numpy >= 1.0.0",
+    "pandas >= 1.0.0",
+    "scikit-learn >= 1.0.0",
+    "pandera",
+]
 
-[tool.flit.metadata.requires-extra]
-linters = [
-    "black",
-    "pydocstyle",
-    "isort",
-    "flake8",
+[project.optional-dependencies]
+docs = [
+    "sphinx>=5.1.1",
+    "sphinx-autodoc-typehints>=1.19.2",
+]
+package = [
+    "build>=0.8.0",
+    "check-manifest>=0.48",
+    "twine>=4.0.1",  # Required by tox -e packaging
 ]
 test = [
+    "black",
+    "flake8",
+    "isort",
+    "mypy",
+    "pydocstyle[toml]",
     "pytest",
+    "pytest-cov",
 ]
 
-[tool.flit.scripts]
-rnanorm = "rnanorm.__main__:main"
+[project.urls]
+repository = "https://github.com/genialis/RNAnorm"
+
+[project.scripts]
+rnanorm = "rnanorm.cli:main"
+
+[tool.setuptools_scm]
+
+[tool.black]
+target-version = ["py38", "py39", "py310"]
+line-length = 99
 
 [tool.isort]
-line_length = 119
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
+profile = "black"
+
+[tool.pydocstyle]
+add-select = "D404"
+add-ignore = "D202"
```

