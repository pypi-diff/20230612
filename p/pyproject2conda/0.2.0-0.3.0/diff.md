# Comparing `tmp/pyproject2conda-0.2.0.tar.gz` & `tmp/pyproject2conda-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject2conda-0.2.0.tar", last modified: Fri Jun  9 14:08:47 2023, max compression
+gzip compressed data, was "pyproject2conda-0.3.0.tar", last modified: Mon Jun 12 15:45:39 2023, max compression
```

## Comparing `pyproject2conda-0.2.0.tar` & `pyproject2conda-0.3.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.302221 pyproject2conda-0.2.0/
--rw-r--r--   0 wpk      (42033)    36681     1380 2023-06-05 16:53:12.000000 pyproject2conda-0.2.0/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681      540 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/.editorconfig
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.237643 pyproject2conda-0.2.0/.github/
--rw-r--r--   0 wpk      (42033)    36681      367 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033)    36681     1360 2023-06-07 14:22:48.000000 pyproject2conda-0.2.0/.gitignore
--rw-r--r--   0 wpk      (42033)    36681      161 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033)    36681     3582 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681       20 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033)    36681      465 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/.recipe-append.yaml
--rw-r--r--   0 wpk      (42033)    36681      122 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681      178 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033)    36681     9748 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      258 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681    11647 2023-06-09 14:08:00.000000 pyproject2conda-0.2.0/Makefile
--rw-r--r--   0 wpk      (42033)    36681    16062 2023-06-09 14:08:47.301422 pyproject2conda-0.2.0/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681    13269 2023-06-09 14:08:00.000000 pyproject2conda-0.2.0/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.238282 pyproject2conda-0.2.0/changelog.d/
--rw-r--r--   0 wpk      (42033)    36681       64 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.239162 pyproject2conda-0.2.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.241114 pyproject2conda-0.2.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033)    36681      213 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033)    36681      774 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033)    36681      269 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/changelog.d/templates/new_fragment.md.j2
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.248235 pyproject2conda-0.2.0/docs/
--rw-r--r--   0 wpk      (42033)    36681     1401 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/Makefile
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.222678 pyproject2conda-0.2.0/docs/_static/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.248739 pyproject2conda-0.2.0/docs/_static/css/
--rw-r--r--   0 wpk      (42033)    36681     2937 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.250835 pyproject2conda-0.2.0/docs/_static/js/
--rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033)    36681      706 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.256856 pyproject2conda-0.2.0/docs/_templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.261140 pyproject2conda-0.2.0/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033)    36681      289 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      249 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033)    36681      405 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033)    36681      424 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      374 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.263679 pyproject2conda-0.2.0/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033)    36681      106 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033)    36681     1119 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033)    36681     1418 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033)    36681     1186 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033)    36681     1212 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033)    36681     1177 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033)    36681     1071 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033)    36681     1179 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033)    36681       69 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/authors.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/changelog.md
--rw-r--r--   0 wpk      (42033)    36681    14781 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/conf.py
--rw-r--r--   0 wpk      (42033)    36681       74 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.265127 pyproject2conda-0.2.0/docs/examples/
--rw-r--r--   0 wpk      (42033)    36681      536 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/docs/examples/example-usage.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.265775 pyproject2conda-0.2.0/docs/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033)    36681      241 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/index.md
--rw-r--r--   0 wpk      (42033)    36681      936 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/docs/installation.md
--rw-r--r--   0 wpk      (42033)    36681       40 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/license.md
--rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/make.bat
--rw-r--r--   0 wpk      (42033)    36681      169 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.266542 pyproject2conda-0.2.0/docs/reference/
--rw-r--r--   0 wpk      (42033)    36681      143 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/reference/index.md
--rw-r--r--   0 wpk      (42033)    36681        0 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.278245 pyproject2conda-0.2.0/environment/
--rw-r--r--   0 wpk      (42033)    36681      943 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      260 2023-06-07 14:20:27.000000 pyproject2conda-0.2.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      108 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       79 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      574 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      377 2023-06-07 14:20:28.000000 pyproject2conda-0.2.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       53 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      153 2023-06-07 14:20:29.000000 pyproject2conda-0.2.0/environment/lint.yaml
--rw-r--r--   0 wpk      (42033)    36681       25 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      144 2023-06-07 14:20:29.000000 pyproject2conda-0.2.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      299 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/environment/tools.yaml
--rw-r--r--   0 wpk      (42033)    36681      148 2023-06-07 14:20:17.000000 pyproject2conda-0.2.0/environment.yaml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.279565 pyproject2conda-0.2.0/examples/
--rw-r--r--   0 wpk      (42033)    36681      222 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/examples/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.280511 pyproject2conda-0.2.0/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033)    36681     6304 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/pyproject.toml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.287460 pyproject2conda-0.2.0/scripts/
--rw-r--r--   0 wpk      (42033)    36681      846 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033)    36681      312 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033)    36681     1099 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033)    36681      266 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/lint.mk
--rw-r--r--   0 wpk      (42033)    36681      598 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/recipe-append.sh
--rw-r--r--   0 wpk      (42033)    36681       91 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033)    36681      489 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033)    36681       38 2023-06-09 14:08:47.302406 pyproject2conda-0.2.0/setup.cfg
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.226108 pyproject2conda-0.2.0/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.290284 pyproject2conda-0.2.0/src/pyproject2conda/
--rw-r--r--   0 wpk      (42033)    36681      648 2023-06-07 15:56:44.000000 pyproject2conda-0.2.0/src/pyproject2conda/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     6563 2023-06-09 14:08:00.000000 pyproject2conda-0.2.0/src/pyproject2conda/cli.py
--rw-r--r--   0 wpk      (42033)    36681    15006 2023-06-09 14:08:00.000000 pyproject2conda-0.2.0/src/pyproject2conda/parser.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.296674 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/
--rw-r--r--   0 wpk      (42033)    36681    16062 2023-06-09 14:08:47.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     2413 2023-06-09 14:08:47.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-06-09 14:08:47.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033)    36681       60 2023-06-09 14:08:47.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/entry_points.txt
--rw-r--r--   0 wpk      (42033)    36681      109 2023-06-09 14:08:47.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033)    36681       16 2023-06-09 14:08:47.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-06-05 17:19:50.000000 pyproject2conda-0.2.0/src/pyproject2conda.egg-info/zip-safe
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-09 14:08:47.300387 pyproject2conda-0.2.0/tests/
--rw-r--r--   0 wpk      (42033)    36681       45 2023-06-05 16:53:11.000000 pyproject2conda-0.2.0/tests/__init__.py
--rw-r--r--   0 wpk      (42033)    36681      611 2023-06-07 02:50:51.000000 pyproject2conda-0.2.0/tests/test-pyproject.toml
--rw-r--r--   0 wpk      (42033)    36681     6093 2023-06-09 14:08:00.000000 pyproject2conda-0.2.0/tests/test_cli.py
--rw-r--r--   0 wpk      (42033)    36681     3738 2023-06-07 18:24:18.000000 pyproject2conda-0.2.0/tests/test_parser.py
--rw-r--r--   0 wpk      (42033)    36681     4101 2023-06-07 18:24:18.000000 pyproject2conda-0.2.0/tox.ini
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.064900 pyproject2conda-0.3.0/
+-rw-r--r--   0 wpk      (42033)    36681     1380 2023-06-05 16:53:12.000000 pyproject2conda-0.3.0/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681      567 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/.editorconfig
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.012272 pyproject2conda-0.3.0/.github/
+-rw-r--r--   0 wpk      (42033)    36681      367 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033)    36681     1360 2023-06-07 14:22:48.000000 pyproject2conda-0.3.0/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033)    36681     3582 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033)    36681      494 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033)    36681      122 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681      178 2023-06-07 15:56:44.000000 pyproject2conda-0.3.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033)    36681     9748 2023-06-07 15:56:44.000000 pyproject2conda-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681     1645 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      258 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681    11647 2023-06-09 14:08:00.000000 pyproject2conda-0.3.0/Makefile
+-rw-r--r--   0 wpk      (42033)    36681    20665 2023-06-12 15:45:39.063949 pyproject2conda-0.3.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681    17872 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.012968 pyproject2conda-0.3.0/changelog.d/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.013664 pyproject2conda-0.3.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.014649 pyproject2conda-0.3.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033)    36681      213 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      774 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      269 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.021095 pyproject2conda-0.3.0/docs/
+-rw-r--r--   0 wpk      (42033)    36681     1401 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.000041 pyproject2conda-0.3.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.021620 pyproject2conda-0.3.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033)    36681     2937 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.022867 pyproject2conda-0.3.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033)    36681      706 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.027683 pyproject2conda-0.3.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.031192 pyproject2conda-0.3.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033)    36681      289 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      249 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033)    36681      405 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033)    36681      424 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      374 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.033672 pyproject2conda-0.3.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033)    36681      106 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033)    36681     1119 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033)    36681     1418 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033)    36681     1186 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681     1212 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033)    36681     1177 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033)    36681     1071 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033)    36681     1179 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681       69 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033)    36681    14781 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033)    36681       74 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.035082 pyproject2conda-0.3.0/docs/examples/
+-rw-r--r--   0 wpk      (42033)    36681      536 2023-06-07 15:56:44.000000 pyproject2conda-0.3.0/docs/examples/example-usage.md
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.035816 pyproject2conda-0.3.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/examples/usage/demo.ipynb
+-rw-r--r--   0 wpk      (42033)    36681      241 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/index.md
+-rw-r--r--   0 wpk      (42033)    36681      936 2023-06-07 15:56:44.000000 pyproject2conda-0.3.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033)    36681       40 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/license.md
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033)    36681      169 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.036544 pyproject2conda-0.3.0/docs/reference/
+-rw-r--r--   0 wpk      (42033)    36681      143 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.044443 pyproject2conda-0.3.0/environment/
+-rw-r--r--   0 wpk      (42033)    36681      943 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      260 2023-06-07 14:20:27.000000 pyproject2conda-0.3.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      108 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681       83 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      574 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      377 2023-06-07 14:20:28.000000 pyproject2conda-0.3.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033)    36681       53 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      153 2023-06-07 14:20:29.000000 pyproject2conda-0.3.0/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033)    36681       25 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      144 2023-06-07 14:20:29.000000 pyproject2conda-0.3.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      299 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033)    36681      148 2023-06-07 14:20:17.000000 pyproject2conda-0.3.0/environment.yaml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.045236 pyproject2conda-0.3.0/examples/
+-rw-r--r--   0 wpk      (42033)    36681      222 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/examples/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.046003 pyproject2conda-0.3.0/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/examples/usage/demo.ipynb
+-rw-r--r--   0 wpk      (42033)    36681     6291 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/pyproject.toml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.051437 pyproject2conda-0.3.0/scripts/
+-rw-r--r--   0 wpk      (42033)    36681      865 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033)    36681      312 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033)    36681     1099 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033)    36681      266 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033)    36681      598 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/scripts/recipe-append.sh
+-rw-r--r--   0 wpk      (42033)    36681       91 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033)    36681      489 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033)    36681       38 2023-06-12 15:45:39.065249 pyproject2conda-0.3.0/setup.cfg
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.003063 pyproject2conda-0.3.0/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.053811 pyproject2conda-0.3.0/src/pyproject2conda/
+-rw-r--r--   0 wpk      (42033)    36681      622 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/src/pyproject2conda/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     7544 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/src/pyproject2conda/cli.py
+-rw-r--r--   0 wpk      (42033)    36681    16931 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/src/pyproject2conda/parser.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.059524 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681    20665 2023-06-12 15:45:38.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     2413 2023-06-12 15:45:38.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-06-12 15:45:38.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033)    36681       60 2023-06-12 15:45:38.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/entry_points.txt
+-rw-r--r--   0 wpk      (42033)    36681      109 2023-06-12 15:45:38.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033)    36681       16 2023-06-12 15:45:38.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-06-05 17:19:50.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.062707 pyproject2conda-0.3.0/tests/
+-rw-r--r--   0 wpk      (42033)    36681       45 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/tests/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681      744 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/tests/test-pyproject.toml
+-rw-r--r--   0 wpk      (42033)    36681     6147 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/tests/test_cli.py
+-rw-r--r--   0 wpk      (42033)    36681     4486 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/tests/test_parser.py
+-rw-r--r--   0 wpk      (42033)    36681     4101 2023-06-07 18:24:18.000000 pyproject2conda-0.3.0/tox.ini
```

### Comparing `pyproject2conda-0.2.0/.cruft.json` & `pyproject2conda-0.3.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/.editorconfig` & `pyproject2conda-0.3.0/.editorconfig`

 * *Files 21% similar despite different names*

```diff
@@ -38,7 +38,11 @@
 trim_trailing_whitespace = false
 
 
 [*.md]
 indent_size = 2
 max_line_length = 80
 trim_trailing_whitespace = false
+
+
+[*.toml]
+indent_size = 4
```

### Comparing `pyproject2conda-0.2.0/.gitignore` & `pyproject2conda-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/.pre-commit-config.yaml` & `pyproject2conda-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/CONTRIBUTING.md` & `pyproject2conda-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/LICENSE` & `pyproject2conda-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/Makefile` & `pyproject2conda-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/PKG-INFO` & `pyproject2conda-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: pyproject2conda
-Version: 0.2.0
-Summary: A script to convert a Python project declared on a pyproject.toml to a conda environment.
-Author-email: "William P. Krekelberg" <wpk@nist.gov>
-License: NIST-PD
-Project-URL: homepage, https://github.com/wpk-nist-gov/pyproject2conda
-Project-URL: documentation, https://pages.nist.gov/pyproject2conda/
-Keywords: pyproject2conda
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: Public Domain
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 <!-- markdownlint-disable MD041 -->
 
 [![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
@@ -92,58 +68,97 @@
 conda install -c wpk-nist pyproject2conda
 ```
 
 ## Example usage
 
 ### Basic usage
 
+<!-- [[[cog
+import subprocess
+import shlex
+
+def run_command(cmd, wrapper="bash", include_cmd=True):
+    args = shlex.split(cmd)
+    output = subprocess.check_output(args)
+
+    total = output.decode()
+    if include_cmd:
+        total = f"$ {cmd}\n{total}"
+
+    if wrapper:
+        total = f"\n```{wrapper}\n"  + total + "```\n"
+
+    print(total)
+
+def cat_lines(path="tests/test-pyproject.toml", begin=0, end=8, begin_dot=True, end_dot=True):
+    with open(path, 'r') as f:
+        lines = [line.rstrip() for line in f]
+
+    output = '\n'.join(lines[slice(begin, end)])
+
+    if begin_dot:
+        output = "# ...\n" +  output
+
+    if end_dot:
+        output = output + "\n# ..."
+
+    output = "\n```toml\n" + output + "\n```\n"
+    print(output)
+]]] -->
+<!-- [[[end]]] -->
+
 Consider the `toml` file [test-pyproject.toml](./tests/test-pyproject.toml).
 
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog cat_lines(begin=0, end=8, begin_dot=False)]]] -->
+
 ```toml
 [project]
 name = "hello"
 requires-python = ">=3.8,<3.11"
 dependencies = [
-  "athing", # p2c: -p # a comment
-  "bthing", # p2c: -s bthing-conda
-  "cthing", # p2c: -c conda-forge
-
+    "athing", # p2c: -p # a comment
+    "bthing", # p2c: -s "bthing-conda"
+    "cthing; python_version < '3.10'", # p2c: -c conda-forge
 ]
 # ...
-
 ```
 
+<!-- [[[end]]] -->
+<!-- prettier-ignore-end -->
+
 Note the comment lines `# p2c:...`. These are special tokens that
 `pyproject2conda` will analyze. The basic options are:
 
-```bash
-Arguments:   Additional (conda) packages
-
--p --pip     Pip install pyproject package on this line.
--s --skip    Skip pyproject package on this line.
--c --channel Add channel to pyproject package on this line
-```
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog run_command("""python -c "from pyproject2conda.parser import _default_parser; _default_parser().parse_args(['--help'])" """, include_cmd=False)]]] -->
 
-So, if we run the following, we get:
+```bash
+usage: -c [-h] [-c CHANNEL] [-p] [-s] [package ...]
 
-<!-- [[[cog
-import subprocess
-import shlex
+Parser searches for comments '# p2c: [OPTIONS]
 
-def run_command(cmd, wrapper="bash"):
-    args = shlex.split(cmd)
-    output = subprocess.check_output(args)
-    total = f"$ {cmd}\n{output.decode()}"
+positional arguments:
+  package
 
-    if wrapper:
-        total = f"\n```{wrapper}\n"  + total + "```\n"
+options:
+  -h, --help            show this help message and exit
+  -c CHANNEL, --channel CHANNEL
+                        Channel to add to the pyproject requirement
+  -p, --pip             If specified, install dependency on pyproject
+                        dependency (on this line) with pip
+  -s, --skip            If specified skip pyproject dependency on this line
+```
 
-    print(total)
-]]] -->
 <!-- [[[end]]] -->
+<!-- prettier-ignore-end -->
+
+So, if we run the following, we get:
 
 <!-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml")]]] -->
 
 ```bash
 $ pyproject2conda yaml -f tests/test-pyproject.toml
 channels:
@@ -154,71 +169,108 @@
   - pip
   - pip:
       - athing
 ```
 
 <!-- [[[end]]] -->
 
-Note that other comments can be mixed in. This also works with extras. For
-example, with the following:
+Note that other comments can be mixed in.
 
-Also, by default, the python version is not included in the resulting conda
-output. To include the specification from pyproject.toml, use `-p/--python`
-option:
+By default, the python version is not included in the resulting conda output. To
+include the specification from pyproject.toml, use `-p/--python` option:
 
 <!-- markdownlint-disable-next-line MD013 -->
-<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -p")]]] -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml --python-include")]]] -->
 
 ```bash
-$ pyproject2conda yaml -f tests/test-pyproject.toml -p
+$ pyproject2conda yaml -f tests/test-pyproject.toml --python-include
 channels:
   - conda-forge
 dependencies:
   - python>=3.8,<3.11
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
 ```
 
 <!-- [[[end]]] -->
 
-To specify a value of python, pass a value with:
+To specify a specific value of python in the output, pass a value with:
 
 <!-- markdownlint-disable-next-line MD013 -->
-<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -p python=3.9")]]] -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml --python-include python=3.9")]]] -->
 
 ```bash
-$ pyproject2conda yaml -f tests/test-pyproject.toml -p python=3.9
+$ pyproject2conda yaml -f tests/test-pyproject.toml --python-include python=3.9
 channels:
   - conda-forge
 dependencies:
   - python=3.9
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
 ```
 
 <!-- [[[end]]] -->
 
+Note that this is for including python in the resulting environment file.
+
+You can also constrain packages by the python version using the standard
+pyproject.toml syntax `"...; python_version < 'some-version-number'"`. For is
+parsed for for both the pip packages and conda packages:
+
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml --python-version 3.10")]]] -->
+
+```bash
+$ pyproject2conda yaml -f tests/test-pyproject.toml --python-version 3.10
+channels:
+  - conda-forge
+dependencies:
+  - bthing-conda
+  - pip
+  - pip:
+      - athing
+```
+
+<!-- [[[end]]] -->
+
+### Installing extras
+
+Given the extra dependency:
+
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable MD013 -->
+<!-- [[[cog cat_lines(begin=9, end=21)]]] -->
+
 ```toml
 # ...
 [project.optional-dependencies]
 test = [
-  "pandas",
-  "pytest", # p2c: -c conda-forge
+    "pandas",
+    "pytest", # p2c: -c conda-forge
 
 ]
+dev-extras = [
+    # p2c: -s "additional-thing; python_version < '3.9'" # this is an additional conda package
+    ## p2c: -s "another-thing" # this will be skipped because of ## before p2c.
+    "matplotlib", # p2c: -s conda-matplotlib
+]
+dev = ["hello[test]", "hello[dev-extras]"]
 # ...
-
 ```
 
+<!-- [[[end]]] -->
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
 and running the the following gives:
 
 <!-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -e test")]]] -->
 
 ```bash
 $ pyproject2conda yaml -f tests/test-pyproject.toml -e test
@@ -234,28 +286,14 @@
       - athing
 ```
 
 <!-- [[[end]]] -->
 
 `pyproject2conda` also works with self referenced dependencies:
 
-```toml
-# ...
-[project.optional-dependencies]
-# ...
-dev-extras = [
-  # p2c: -s additional-thing # this is an additional conda package
-  "matplotlib", # p2c: -s conda-matplotlib
-
-]
-dev = ["hello[test]", "hello[dev-extras]"]
-# ...
-
-```
-
 <!-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -e dev")]]] -->
 
 ```bash
 $ pyproject2conda yaml -f tests/test-pyproject.toml -e dev
 channels:
   - conda-forge
@@ -269,24 +307,27 @@
   - pip
   - pip:
       - athing
 ```
 
 <!-- [[[end]]] -->
 
+This also shows that `p2c` comments without dependencies are also parsed. To
+comment out such lines, make sure `p2c` is preceded by `##`.
+
 ### Usage within python
 
 `pyproject2conda` can also be used within python:
 
 ```pycon
 >>> from pyproject2conda import PyProject2Conda
 >>> p = PyProject2Conda.from_path("./tests/test-pyproject.toml")
 
 # Basic environment
->>> print(p.to_conda_yaml(python="get").strip())
+>>> print(p.to_conda_yaml(python_include="get").strip())
 channels:
   - conda-forge
 dependencies:
   - python>=3.8,<3.11
   - bthing-conda
   - conda-forge::cthing
   - pip
@@ -309,37 +350,52 @@
 ```
 
 ### Configuration
 
 `pyproject2conda` can be configured with a `[tool.pyproject2conda]` section in
 `pyproject.toml`. To specify conda channels use:
 
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog cat_lines(begin=22, end=24)]]] -->
+
 ```toml
-# Why channel conda-forge appeared above
+# ...
 [tool.pyproject2conda]
-channels = ["conda-forge"]
-
+channels = ['conda-forge']
+# ...
 ```
 
+<!-- [[[end]]] -->
+<!-- prettier-ignore-end -->
+
 Note that specifying channels at the comand line overrides
 
 You can also specify `isolated-dependencies`. These are dependencies for things
 that should not include package dependencies (things like build dependencies).
 For example:
 
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog cat_lines(begin=25, end=None)]]] -->
+
 ```toml
+# ...
 [tool.pyproject2conda.isolated-dependencies]
 dist-pypi = [
-  "setuptools",
-  "build", # p2c: -p
+    "setuptools",
+    "build", # p2c: -p
 
 ]
-
+# ...
 ```
 
+<!-- [[[end]]] -->
+<!-- prettier-ignore-end -->
+
 These can be accessed using either of the following:
 
 <!-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -i dist-pypi")]]] -->
 
 ```bash
 $ pyproject2conda yaml -f tests/test-pyproject.toml -i dist-pypi
@@ -370,14 +426,15 @@
   - pip:
       - build
 
 ```
 
 ### CLI options
 
+<!-- prettier-ignore-start -->
 <!-- [[[cog run_command("pyproject2conda --help")]]] -->
 
 ```bash
 $ pyproject2conda --help
 Usage: pyproject2conda [OPTIONS] COMMAND [ARGS]...
 
 Options:
@@ -414,28 +471,36 @@
 ```bash
 $ pyproject2conda yaml --help
 Usage: pyproject2conda yaml [OPTIONS]
 
   Create yaml file from dependencies and optional-dependencies.
 
 Options:
-  -e, --extra TEXT     Extra depenedencies. Can specify multiple times for
-                       multiple extras.
-  -i, --isolated TEXT  Isolated dependencies (under
-                       [tool.pyproject2conda.isolated-dependencies]).  Can
-                       specify multiple times.
-  -c, --channel TEXT   conda channel.  Can specify. Overrides
-                       [tool.pyproject2conda.channels]
-  -f, --file PATH      input pyproject.toml file
-  -n, --name TEXT      Name of conda env
-  -o, --output PATH    File to output results
-  -p, --python TEXT    if flag passed without options, include python spec
-                       from pyproject.toml in output.  If value passed, use
-                       this value of python in the output
-  --help               Show this message and exit.
+  -e, --extra TEXT       Extra depenedencies. Can specify multiple times for
+                         multiple extras.
+  -i, --isolated TEXT    Isolated dependencies (under
+                         [tool.pyproject2conda.isolated-dependencies]).  Can
+                         specify multiple times.
+  -c, --channel TEXT     conda channel.  Can specify. Overrides
+                         [tool.pyproject2conda.channels]
+  -f, --file PATH        input pyproject.toml file
+  -n, --name TEXT        Name of conda env
+  -o, --output PATH      File to output results
+  --python-include TEXT  If flag passed without options, include python spec
+                         from pyproject.toml in yaml output.  If value passed,
+                         use this value (exactly) in the output. So, for
+                         example, pass `--python-include "python=3.8"`
+  --python-version TEXT  Python version to check `python_verion <=>
+                         {python_version}` lines against.  That is, this
+                         version is used to limit packages in resulting
+                         output. For example, if have a line like
+                         `a-package; python_version < '3.9'`, Using `--python-
+                         version 3.10` will not include `a-package`, while
+                         `--python-version 3.8` will include `a-package`.
+  --help                 Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
 
 <!-- [[[cog run_command("pyproject2conda requirements --help")]]] -->
 
 ```bash
@@ -466,29 +531,37 @@
   Create requirement files for conda and pip.
 
   These can be install with, for example,
 
   conda install --file {path_conda} pip install -r {path_pip}
 
 Options:
-  -e, --extra TEXT     Extra depenedencies. Can specify multiple times for
-                       multiple extras.
-  -i, --isolated TEXT  Isolated dependencies (under
-                       [tool.pyproject2conda.isolated-dependencies]).  Can
-                       specify multiple times.
-  -p, --python TEXT    if flag passed without options, include python spec
-                       from pyproject.toml in output.  If value passed, use
-                       this value of python in the output
-  -c, --channel TEXT   conda channel.  Can specify. Overrides
-                       [tool.pyproject2conda.channels]
-  -f, --file PATH      input pyproject.toml file
-  --prefix TEXT        set conda-output=prefix + 'conda.txt', pip-
-                       output=prefix + 'pip.txt'
+  -e, --extra TEXT       Extra depenedencies. Can specify multiple times for
+                         multiple extras.
+  -i, --isolated TEXT    Isolated dependencies (under
+                         [tool.pyproject2conda.isolated-dependencies]).  Can
+                         specify multiple times.
+  --python-include TEXT  If flag passed without options, include python spec
+                         from pyproject.toml in yaml output.  If value passed,
+                         use this value (exactly) in the output. So, for
+                         example, pass `--python-include "python=3.8"`
+  --python-version TEXT  Python version to check `python_verion <=>
+                         {python_version}` lines against.  That is, this
+                         version is used to limit packages in resulting
+                         output. For example, if have a line like
+                         `a-package; python_version < '3.9'`, Using `--python-
+                         version 3.10` will not include `a-package`, while
+                         `--python-version 3.8` will include `a-package`.
+  -c, --channel TEXT     conda channel.  Can specify. Overrides
+                         [tool.pyproject2conda.channels]
+  -f, --file PATH        input pyproject.toml file
+  --prefix TEXT          set conda-output=prefix + 'conda.txt', pip-
+                         output=prefix + 'pip.txt'
   --prepend-channel
-  --help               Show this message and exit.
+  --help                 Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
 
 <!-- [[[cog run_command("pyproject2conda json --help")]]] -->
 
 ```bash
@@ -497,30 +570,39 @@
 
   Create json representation.
 
   Keys are: "dependencies": conda dependencies. "pip": pip dependencies.
   "channels": conda channels.
 
 Options:
-  -e, --extra TEXT     Extra depenedencies. Can specify multiple times for
-                       multiple extras.
-  -i, --isolated TEXT  Isolated dependencies (under
-                       [tool.pyproject2conda.isolated-dependencies]).  Can
-                       specify multiple times.
-  -p, --python TEXT    if flag passed without options, include python spec
-                       from pyproject.toml in output.  If value passed, use
-                       this value of python in the output
-  -c, --channel TEXT   conda channel.  Can specify. Overrides
-                       [tool.pyproject2conda.channels]
-  -f, --file PATH      input pyproject.toml file
-  -o, --output PATH    File to output results
-  --help               Show this message and exit.
+  -e, --extra TEXT       Extra depenedencies. Can specify multiple times for
+                         multiple extras.
+  -i, --isolated TEXT    Isolated dependencies (under
+                         [tool.pyproject2conda.isolated-dependencies]).  Can
+                         specify multiple times.
+  --python-include TEXT  If flag passed without options, include python spec
+                         from pyproject.toml in yaml output.  If value passed,
+                         use this value (exactly) in the output. So, for
+                         example, pass `--python-include "python=3.8"`
+  --python-version TEXT  Python version to check `python_verion <=>
+                         {python_version}` lines against.  That is, this
+                         version is used to limit packages in resulting
+                         output. For example, if have a line like
+                         `a-package; python_version < '3.9'`, Using `--python-
+                         version 3.10` will not include `a-package`, while
+                         `--python-version 3.8` will include `a-package`.
+  -c, --channel TEXT     conda channel.  Can specify. Overrides
+                         [tool.pyproject2conda.channels]
+  -f, --file PATH        input pyproject.toml file
+  -o, --output PATH      File to output results
+  --help                 Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
+<!-- prettier-ignore-end -->
 
 <!-- end-docs -->
 
 <!-- ## Documentation -->
 
 <!-- See the [documentation][docs-link] for a look at -->
 <!-- `pyproject2conda` in action. -->
@@ -540,43 +622,7 @@
 ## Credits
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
 Project template forked from
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
-
-# Changelog
-
-Changelog for `pyproject2conda`
-
-## Unreleased
-
-See the fragment files in
-[changelog.d](https://github.com/wpk-nist-gov/pyproject2conda)
-
-<!-- scriv-insert-here -->
-
-This software was developed by employees of the National Institute of Standards
-and Technology (NIST), an agency of the Federal Government. Pursuant to title 17
-United States Code Section 105, works of NIST employees are not subject to
-copyright protection in the United States and are considered to be in the public
-domain. Permission to freely use, copy, modify, and distribute this software and
-its documentation without fee is hereby granted, provided that this notice and
-disclaimer of warranty appears in all copies.
-
-THE SOFTWARE IS PROVIDED 'AS IS' WITHOUT ANY WARRANTY OF ANY KIND, EITHER
-EXPRESSED, IMPLIED, OR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTY
-THAT THE SOFTWARE WILL CONFORM TO SPECIFICATIONS, ANY IMPLIED WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND FREEDOM FROM
-INFRINGEMENT, AND ANY WARRANTY THAT THE DOCUMENTATION WILL CONFORM TO THE
-SOFTWARE, OR ANY WARRANTY THAT THE SOFTWARE WILL BE ERROR FREE. IN NO EVENT
-SHALL NIST BE LIABLE FOR ANY DAMAGES, INCLUDING, BUT NOT LIMITED TO, DIRECT,
-INDIRECT, SPECIAL OR CONSEQUENTIAL DAMAGES, ARISING OUT OF, RESULTING FROM, OR
-IN ANY WAY CONNECTED WITH THIS SOFTWARE, WHETHER OR NOT BASED UPON WARRANTY,
-CONTRACT, TORT, OR OTHERWISE, WHETHER OR NOT INJURY WAS SUSTAINED BY PERSONS OR
-PROPERTY OR OTHERWISE, AND WHETHER OR NOT LOSS WAS SUSTAINED FROM, OR AROSE OUT
-OF THE RESULTS OF, OR USE OF, THE SOFTWARE OR SERVICES PROVIDED HEREUNDER.
-
-Distributions of NIST software should also include copyright and licensing
-statements of any third-party software that are legally bundled with the code in
-compliance with the conditions of those licenses.
```

### Comparing `pyproject2conda-0.2.0/changelog.d/templates/auto-changelog/template.jinja2` & `pyproject2conda-0.3.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/Makefile` & `pyproject2conda-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/_static/css/nist-combined.css` & `pyproject2conda-0.3.0/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/_static/js/leave_notice.js` & `pyproject2conda-0.3.0/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/_static/js/nist-header-footer.js` & `pyproject2conda-0.3.0/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/_templates/autosummary/class.rst` & `pyproject2conda-0.3.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/_templates/autosummary/module.rst` & `pyproject2conda-0.3.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/_templates/class-individual-pages.rst` & `pyproject2conda-0.3.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/_templates/class-single-page.rst` & `pyproject2conda-0.3.0/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/_templates/custom-module-template.rst` & `pyproject2conda-0.3.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/_templates/module-custom-imported.rst` & `pyproject2conda-0.3.0/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/_templates/module-custom.rst` & `pyproject2conda-0.3.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/_templates/module-single.rst` & `pyproject2conda-0.3.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/_templates/module-template.rst` & `pyproject2conda-0.3.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/conf.py` & `pyproject2conda-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/examples/example-usage.md` & `pyproject2conda-0.3.0/docs/examples/example-usage.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/examples/usage/demo.ipynb` & `pyproject2conda-0.3.0/docs/examples/usage/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/installation.md` & `pyproject2conda-0.3.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/docs/make.bat` & `pyproject2conda-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/environment/dev-extras.yaml` & `pyproject2conda-0.3.0/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/environment/docs-extras.yaml` & `pyproject2conda-0.3.0/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/examples/usage/demo.ipynb` & `pyproject2conda-0.3.0/examples/usage/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/pyproject.toml` & `pyproject2conda-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -26,27 +26,25 @@
 requires-python = ">=3.8"
 dependencies = [
     "tomli",
     "ruamel.yaml",
     "tomlkit",
     "rich-click",
     "click-default-group",
-    # "typing-extensions; python<3.10",
+    # "typing-extensions; python_version<'3.10'",
 
 ] # additional packages
 
 [project.urls]
 homepage = "https://github.com/wpk-nist-gov/pyproject2conda"
 documentation = "https://pages.nist.gov/pyproject2conda/"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "pytest-xdist", "pytest-sugar"]
 
-# dev = []
-# docs = []
 [project.scripts]
 pyproject2conda = "pyproject2conda.cli:app"
 
 ## grayskull still messes some things up, but use scripts/recipe-append.sh for this
 [tool.setuptools]
 zip-safe = true # if using mypy, must be False
 include-package-data = true
```

### Comparing `pyproject2conda-0.2.0/scripts/dist-conda.mk` & `pyproject2conda-0.3.0/scripts/dist-conda.mk`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 clean-build:
 	rm -rf build
 
 # by default, only use a few sections
 grayskull_args ?= --maintainers wpk-nist-gov --sections package source build requirements
 grayskull: clean-recipe
+	-mkdir dist-conda
 	grayskull pypi $(sdist_path) $(grayskull_args) -o dist-conda
 
 # append the rest
 recipe_base_path ?= dist-conda/$(project_name)/meta.yaml
 recipe_append_path ?= .recipe-append.yaml
 recipe-append:
 	bash scripts/recipe-append.sh $(recipe_base_path) $(recipe_append_path)
```

### Comparing `pyproject2conda-0.2.0/scripts/docs-examples-symlinks.sh` & `pyproject2conda-0.3.0/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/scripts/recipe-append.sh` & `pyproject2conda-0.3.0/scripts/recipe-append.sh`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/src/pyproject2conda/__init__.py` & `pyproject2conda-0.3.0/src/pyproject2conda/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from .parser import PyProject2Conda
 
 # updated versioning scheme
 try:
     from importlib.metadata import version as _version
 except ImportError:
-    from importlib_metadata import version as _version  # type: ignore[no-redef]
+    from importlib_metadata import version as _version
 
 try:
     __version__ = _version("pyproject2conda")
 except Exception:
     # Local copy or not installed with setuptools.
     # Disable minimum version checks on downstream libraries.
     __version__ = "999"
```

### Comparing `pyproject2conda-0.2.0/src/pyproject2conda/cli.py` & `pyproject2conda-0.3.0/src/pyproject2conda/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -49,22 +49,36 @@
     default=None,
     help="File to output results",
 )
 
 VERBOSE_CLI = click.option("-v", "--verbose", "verbose", is_flag=True, default=False)
 
 
-PYTHON_CLI = click.option(
-    "-p",
-    "--python",
-    "python",
+PYTHON_INCLUDE_CLI = click.option(
+    "--python-include",
+    "python_include",
     is_flag=False,
     flag_value="get",
     default=None,
-    help="if flag passed without options, include python spec from pyproject.toml in output.  If value passed, use this value of python in the output",
+    help="""
+    If flag passed without options, include python spec from pyproject.toml in yaml output.  If value passed, use this value (exactly) in the output.
+    So, for example, pass `--python-include "python=3.8"`
+    """,
+)
+
+PYTHON_VERSION_CLI = click.option(
+    "--python-version",
+    "python_version",
+    type=str,
+    default=None,
+    help="""
+    Python version to check `python_verion <=> {python_version}` lines against.  That is, this version is used to limit packages in resulting output.
+    For example, if have a line like   `a-package; python_version < '3.9'`,
+    Using `--python-version 3.10` will not include `a-package`, while `--python-version 3.8` will include `a-package`.
+    """,
 )
 
 
 class AliasedGroup(click.Group):
     """Provide aliasing for commands"""
 
     def get_command(self, ctx, cmd_name):
@@ -104,37 +118,40 @@
 @app.command()
 @EXTRAS_CLI
 @ISOLATED_CLI
 @CHANNEL_CLI
 @PYPROJECT_CLI
 @NAME_CLI
 @OUTPUT_CLI
-@PYTHON_CLI
+@PYTHON_INCLUDE_CLI
+@PYTHON_VERSION_CLI
 def yaml(
     extras,
     isolated,
     channels,
     filename,
     name,
     output,
-    python,
+    python_include,
+    python_version,
 ):
     """Create yaml file from dependencies and optional-dependencies."""
 
     if not channels:
         channels = None
 
     d = PyProject2Conda.from_path(filename)
     s = d.to_conda_yaml(
         extras=extras,
         isolated=isolated,
         channels=channels,
         name=name,
         stream=output,
-        python=python,
+        python_include=python_include,
+        python_version=python_version,
     )
     if not output:
         click.echo(s, nl=False)
 
 
 @app.command()
 @EXTRAS_CLI
@@ -158,15 +175,16 @@
     if not output:
         click.echo(s, nl=False)
 
 
 @app.command()
 @EXTRAS_CLI
 @ISOLATED_CLI
-@PYTHON_CLI
+@PYTHON_INCLUDE_CLI
+@PYTHON_VERSION_CLI
 @CHANNEL_CLI
 @PYPROJECT_CLI
 @click.option(
     "--prefix",
     "prefix",
     type=str,
     default=None,
@@ -178,15 +196,16 @@
     default=False,
 )
 @click.argument("path_conda", type=str, required=False)
 @click.argument("path_pip", type=str, required=False)
 def conda_requirements(
     extras,
     isolated,
-    python,
+    python_include,
+    python_version,
     channels,
     filename,
     prefix,
     prepend_channel,
     # paths,
     path_conda,
     path_pip,
@@ -211,37 +230,40 @@
         path_pip = prefix + "pip.txt"
 
     d = PyProject2Conda.from_path(filename)
 
     deps, reqs = d.to_conda_requirements(
         extras=extras,
         isolated=isolated,
-        python=python,
+        python_include=python_include,
+        python_version=python_version,
         channels=channels,
         prepend_channel=prepend_channel,
         stream_conda=path_conda,
         stream_pip=path_pip,
     )
 
     if not path_conda:
         s = f"#conda requirements\n{deps}\n#pip requirements\n{reqs}"
         click.echo(s, nl=False)
 
 
 @app.command("json")
 @EXTRAS_CLI
 @ISOLATED_CLI
-@PYTHON_CLI
+@PYTHON_INCLUDE_CLI
+@PYTHON_VERSION_CLI
 @CHANNEL_CLI
 @PYPROJECT_CLI
 @OUTPUT_CLI
 def to_json(
     extras,
     isolated,
-    python,
+    python_include,
+    python_version,
     channels,
     filename,
     output,
 ):
     """
     Create json representation.
 
@@ -252,31 +274,35 @@
     """
 
     import json
 
     d = PyProject2Conda.from_path(filename)
 
     result = d.to_conda_lists(
-        extras=extras, isolated=isolated, channels=channels, python=python
+        extras=extras,
+        isolated=isolated,
+        channels=channels,
+        python_include=python_include,
+        python_version=python_version,
     )
 
     if output:
         with open(output, "w") as f:
             json.dump(result, f)
     else:
         click.echo(json.dumps(result))  # , indent=2))
 
 
 # @app.command("yaml-conda-req")
 # @EXTRAS_CLI
-# @PYTHON_CLI
+# @PYTHON_INCLUDE_CLI
 # @PYPROJECT_CLI
 # def conda_requirements(
 #         extras,
-#         python,
+#         python_include,
 #         filename,
 
 # ):
 #     d = PyProject2Conda.from_path(filename)
 
 #     output = d.to_conda_lists(extras=extras)
 #     click.echo(f"{output}")
@@ -284,30 +310,30 @@
 
 # @app.command()
 # @ISOLATED_CLI
 # @CHANNEL_CLI
 # @PYPROJECT_CLI
 # @NAME_CLI
 # @OUTPUT_CLI
-# @PYTHON_CLI
+# @PYTHON_INCLUDE_CLI
 # def isolated(
 #     isolated,
 #     channel,
 #     filename,
 #     name,
 #     output,
-#     python,
+#     python_include,
 # ):
 #     """Create yaml file from [tool.pyproject2conda.isolated-dependencies]"""
 
 #     if not channel:
 #         channel = None
 #     d = PyProject2Conda.from_path(filename)
 #     s = d.to_conda_yaml(
-#         isolated=isolated, channels=channel, name=name, python=python, stream=output
+#         isolated=isolated, channels=channel, name=name, python_include=python_include, stream=output
 #     )
 #     if not output:
 #         click.echo(s, nl=False)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pyproject2conda-0.2.0/src/pyproject2conda/parser.py` & `pyproject2conda-0.3.0/src/pyproject2conda/parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,36 +5,37 @@
 Main parser to turn pyproject.toml -> environment.yaml
 """
 from __future__ import annotations
 
 import argparse
 import re
 import shlex
+from functools import lru_cache
 from pathlib import Path
-from typing import Any, Mapping, Optional, Sequence, TypeVar, Union
+from typing import Any, Generator, Mapping, Optional, Sequence, TypeVar, Union, cast
 
 import tomlkit
+from packaging.specifiers import SpecifierSet
+from packaging.version import Version
 from ruamel.yaml import YAML
 
 # -- typing ----------------------------------------------------------------------------
 
 Tstr_opt = Optional[str]
 Tstr_seq_opt = Optional[Union[str, Sequence[str]]]
 
 
 # --- Default parser -------------------------------------------------------------------
 
-_DEFAULTS = {}
 
-
-def _default_parser():
-    if "parser" in _DEFAULTS:
-        return _DEFAULTS["parser"]
-
-    parser = argparse.ArgumentParser()
+@lru_cache
+def _default_parser() -> argparse.ArgumentParser:
+    parser = argparse.ArgumentParser(
+        description="Parser searches for comments '# p2c: [OPTIONS]"
+    )
 
     parser.add_argument(
         "-c",
         "--channel",
         type=str,
         help="Channel to add to the pyproject requirement",
     )
@@ -46,17 +47,16 @@
     )
     parser.add_argument(
         "-s",
         "--skip",
         action="store_true",
         help="If specified skip pyproject dependency on this line",
     )
-    parser.add_argument("package", nargs="*")
 
-    _DEFAULTS["parser"] = parser
+    parser.add_argument("package", nargs="*")
 
     return parser
 
 
 # taken from https://github.com/conda/conda-lock/blob/main/conda_lock/common.py
 def get_in(
     keys: Sequence[Any], nested_dict: Mapping[Any, Any], default: Any = None
@@ -97,15 +97,15 @@
         output = ""
 
     return output
 
 
 def _iter_value_comment_pairs(
     array: tomlkit.items.Array,
-) -> list[tuple(Tstr_opt, Tstr_opt)]:
+) -> Generator[tuple[Tstr_opt, Tstr_opt], None, None]:
     """Extract value and comments from array"""
     for v in array._value:
         if v.value is not None and not isinstance(v.value, tomlkit.items.Null):
             value = str(v.value)  # .as_string()
         else:
             value = None
         if v.comment:
@@ -116,15 +116,15 @@
             continue
         yield (value, comment)
 
 
 def _matches_package_name(
     dep: Tstr_opt,
     package_name: str,
-) -> list[str]:
+) -> list[str] | None:
     """
     Check if `dep` matches pattern {package_name}[extra,..]
 
     If it does, return extras, else return None
     """
 
     if not dep:
@@ -142,15 +142,15 @@
 
 def get_value_comment_pairs(
     package_name: str,
     deps: tomlkit.items.Array,
     extras: Tstr_seq_opt = None,
     opts: tomlkit.items.Table | None = None,
     include_root: bool = True,
-) -> list[tuple(Tstr_opt, Tstr_opt)]:
+) -> list[tuple[Tstr_opt, Tstr_opt]]:
     """Recursively build dependency, comment pairs from deps and extras."""
     if include_root:
         out = list(_iter_value_comment_pairs(deps))
     else:
         out = []
 
     if extras is None:
@@ -158,15 +158,17 @@
     else:
         assert opts is not None
 
     if isinstance(extras, str):
         extras = [extras]
 
     for extra in extras:
-        for value, comment in _iter_value_comment_pairs(opts[extra]):
+        for value, comment in _iter_value_comment_pairs(
+            cast(tomlkit.items.Array, opts[extra])
+        ):
             if new_extras := _matches_package_name(value, package_name):
                 out.extend(
                     get_value_comment_pairs(
                         package_name=package_name,
                         extras=new_extras,
                         deps=deps,
                         opts=opts,
@@ -175,152 +177,188 @@
                 )
             else:
                 out.append((value, comment))
 
     return out
 
 
+def _pyproject_to_value_comment_pairs(
+    data: tomlkit.toml_document.TOMLDocument,
+    extras: Tstr_seq_opt = None,
+    isolated: Tstr_seq_opt = None,
+    unique: bool = True,
+):
+    package_name = cast(str, get_in(["project", "name"], data))
+
+    deps = cast(tomlkit.items.Array, get_in(["project", "dependencies"], data))
+
+    if isolated:
+        value_comment_list = get_value_comment_pairs(
+            package_name=package_name,
+            extras=isolated,
+            deps=deps,
+            opts=get_in(["tool", "pyproject2conda", "isolated-dependencies"], data),
+            include_root=False,
+        )
+    else:
+        value_comment_list = get_value_comment_pairs(
+            package_name=package_name,
+            extras=extras,
+            deps=deps,
+            opts=get_in(["project", "optional-dependencies"], data),
+        )
+
+    if unique:
+        value_comment_list = _unique_list(value_comment_list)
+
+    return value_comment_list
+
+
 def _match_p2c_comment(comment: Tstr_opt) -> Tstr_opt:
     if not comment or not (match := re.match(r".*?#\s*p2c:\s*([^\#]*)", comment)):
         return None
+    elif re.match(r".*?##\s*p2c:", comment):
+        # This checks for double ##.  If found, ignore line
+        return None
     else:
         return match.group(1).strip()
 
 
-def _parse_p2c(match: Tstr_opt) -> Tstr_opt:
+def _parse_p2c(match: Tstr_opt) -> dict[str, Any] | None:
     """Parse match from _match_p2c_comment"""
 
     if match:
         return vars(_default_parser().parse_args(shlex.split(match)))
     else:
         return None
 
 
-def parse_p2c_comment(comment: Tstr_opt) -> Tstr_opt:
+def parse_p2c_comment(comment: Tstr_opt) -> dict[str, Any] | None:
     if match := _match_p2c_comment(comment):
         return _parse_p2c(match)
     else:
         return None
 
 
+def _limit_deps_by_python_version(
+    deps: list[str], python_version: Tstr_opt = None
+) -> list[str]:
+    if python_version:
+        version = Version(python_version)
+    else:
+        version = None
+
+    matcher = re.compile(
+        r"(?P<dep>.*?);\s*python_version\s*(?P<token>[<=>~]*)\s*[\'|\"](?P<version>.*?)[\'|\"]"
+    )
+
+    output = []
+    for dep in deps:
+        if match := matcher.match(dep):
+            if not version or version in SpecifierSet(
+                match["token"] + match["version"]
+            ):
+                output.append(match["dep"])
+        else:
+            output.append(dep)
+    return output
+
+
 def value_comment_pairs_to_conda(
-    value_comment_list: list[tuple(Tstr_opt, Tstr_opt)]
+    value_comment_list: list[tuple[Tstr_opt, Tstr_opt]],
 ) -> dict[str, Any]:
     """Convert raw value/comment pairs to install lines"""
 
-    conda_deps = []
-    pip_deps = []
+    conda_deps: list[Tstr_opt] = []
+    pip_deps: list[Tstr_opt] = []
 
     def _check_value(value):
         if not value:
             raise ValueError("trying to add value that does not exist")
 
     for value, comment in value_comment_list:
         if comment and (parsed := parse_p2c_comment(comment)):
             if parsed["pip"]:
                 _check_value(value)
                 pip_deps.append(value)
             elif not parsed["skip"]:
                 _check_value(value)
 
                 if parsed["channel"]:
-                    v = "{}::{}".format(parsed["channel"], value)
+                    conda_deps.append("{}::{}".format(parsed["channel"], value))
                 else:
-                    v = value
-                conda_deps.append(v)
+                    conda_deps.append(value)
 
             conda_deps.extend(parsed["package"])
         elif value:
             conda_deps.append(value)
 
     return {"dependencies": conda_deps, "pip": pip_deps}
 
 
-def _pyproject_to_value_comment_pairs(
-    data: tomlkit.toml_document.TOMLDocument,
-    extras: Tstr_seq_opt = None,
-    isolated: Tstr_seq_opt = None,
-    unique: bool = True,
-):
-    project = data["project"]
-    package_name = project["name"]
-
-    deps = project["dependencies"]
-
-    if isolated:
-        value_comment_list = get_value_comment_pairs(
-            package_name=package_name,
-            extras=isolated,
-            deps=deps,
-            opts=get_in(["tool", "pyproject2conda", "isolated-dependencies"], data),
-            include_root=False,
-        )
-    else:
-        value_comment_list = get_value_comment_pairs(
-            package_name=package_name,
-            extras=extras,
-            deps=deps,
-            opts=get_in(["project", "optional-dependencies"], data),
-        )
-
-    if unique:
-        value_comment_list = _unique_list(value_comment_list)
-
-    return value_comment_list
-
-
 def pyproject_to_conda_lists(
-    data: str | Path | tomlkit.toml_document.TOMLDocument,
+    data: tomlkit.toml_document.TOMLDocument,
     extras: Tstr_seq_opt = None,
     isolated: Tstr_seq_opt = None,
     channels: Tstr_seq_opt = None,
-    python: Tstr_opt = None,
-):
-    if python == "get":
-        python = "python" + get_in(["project", "requires-python"], data).unwrap()
+    python_include: Tstr_opt = None,
+    python_version: Tstr_opt = None,
+) -> dict[str, Any]:
+    if python_include == "get":
+        python_include = (
+            "python" + get_in(["project", "requires-python"], data).unwrap()
+        )
 
     if channels is None:
-        channels = get_in(["tool", "pyproject2conda", "channels"], data, None)
-        if channels:
-            channels = channels.unwrap()
+        channels_doc = get_in(["tool", "pyproject2conda", "channels"], data, None)
+        if channels_doc:
+            channels = channels_doc.unwrap()
     if isinstance(channels, str):
         channels = [channels]
 
     value_comment_list = _pyproject_to_value_comment_pairs(
         data=data,
         extras=extras,
         isolated=isolated,
     )
 
-    output = value_comment_pairs_to_conda(value_comment_list)
-
-    if python:
-        output["dependencies"].insert(0, python)
+    output = value_comment_pairs_to_conda(
+        value_comment_list,
+    )
 
+    if python_include:
+        output["dependencies"].insert(0, python_include)
     if channels:
         output["channels"] = channels
 
+    # limit python version/remove python_verions <=> part
+    output["dependencies"] = _limit_deps_by_python_version(
+        output["dependencies"], python_version
+    )
+
     return output
 
 
 def pyproject_to_conda(
-    data: str | Path | tomlkit.toml_document.TOMLDocument,
+    data: tomlkit.toml_document.TOMLDocument,
     extras: Tstr_seq_opt = None,
     isolated: Tstr_seq_opt = None,
     channels: Tstr_seq_opt = None,
     name: Tstr_opt = None,
-    python: Tstr_opt = None,
+    python_include: Tstr_opt = None,
     stream: str | Path | None = None,
+    python_version: Tstr_opt = None,
 ):
     output = pyproject_to_conda_lists(
         data=data,
         extras=extras,
         isolated=isolated,
         channels=channels,
-        python=python,
+        python_include=python_include,
+        python_version=python_version,
     )
     return _output_to_yaml(**output, name=name, stream=stream)
 
 
 def _yaml_to_string(yaml, data, add_final_eol=False) -> str:
     import io
 
@@ -338,15 +376,15 @@
 def _output_to_yaml(
     dependencies: list[str] | None,
     channels: list[str] | None = None,
     pip: list[str] | None = None,
     name: Tstr_opt = None,
     stream: str | Path | None = None,
 ):
-    data = {}
+    data: dict[str, Any] = {}
 
     if name:
         data["name"] = name
 
     if channels:
         data["channels"] = channels
 
@@ -379,57 +417,61 @@
     """Wrapper class to transform pyproject.toml -> environment.yaml"""
 
     def __init__(
         self,
         data: tomlkit.toml_document.TOMLDocument,
         name: Tstr_opt = None,
         channels: Tstr_seq_opt = None,
-        python: Tstr_opt = None,
+        python_include: Tstr_opt = None,
     ) -> None:
         self.data = data
         self.name = name
         self.channels = channels
-        self.python = python
+        self.python_include = python_include
 
     def to_conda_yaml(
         self,
         extras: Tstr_seq_opt = None,
         isolated: Tstr_seq_opt = None,
         name: Tstr_opt = None,
         channels: Tstr_seq_opt = None,
-        python: Tstr_opt = None,
+        python_include: Tstr_opt = None,
         stream: str | Path | None = None,
+        python_version: Tstr_opt = None,
     ):
         self._check_extras_isolated(extras, isolated)
 
         return pyproject_to_conda(
             data=self.data,
             extras=extras,
             isolated=isolated,
             name=name or self.name,
             channels=channels or self.channels,
-            python=python or self.python,
+            python_include=python_include or self.python_include,
             stream=stream,
+            python_version=python_version,
         )
 
     def to_conda_lists(
         self,
         extras: Tstr_seq_opt = None,
         isolated: Tstr_seq_opt = None,
         channels: Tstr_seq_opt = None,
-        python: Tstr_opt = None,
+        python_include: Tstr_opt = None,
+        python_version: Tstr_opt = None,
     ) -> dict[str, Any]:
         self._check_extras_isolated(extras, isolated)
 
         return pyproject_to_conda_lists(
             data=self.data,
             extras=extras,
             isolated=isolated,
             channels=channels or self.channels,
-            python=python or self.python,
+            python_include=python_include or self.python_include,
+            python_version=python_version,
         )
 
     def to_requirement_list(
         self,
         extras: Tstr_seq_opt = None,
         isolated: Tstr_seq_opt = None,
     ) -> list[str]:
@@ -461,24 +503,26 @@
             return s
 
     def to_conda_requirements(
         self,
         extras: Tstr_opt = None,
         isolated: Tstr_seq_opt = None,
         channels: Tstr_seq_opt = None,
-        python: Tstr_opt = None,
+        python_include: Tstr_opt = None,
+        python_version: Tstr_opt = None,
         prepend_channel: bool = False,
         stream_conda: str | Path | None = None,
         stream_pip: str | Path | None = None,
     ):
         output = self.to_conda_lists(
             extras=extras,
             isolated=isolated,
             channels=channels,
-            python=python,
+            python_include=python_include,
+            python_version=python_version,
         )
 
         deps = output.get("dependencies", None)
         reqs = output.get("pip", None)
 
         channels = output.get("channels", None)
         if channels and prepend_channel:
@@ -533,35 +577,39 @@
 
     @classmethod
     def from_string(
         cls: type[T],
         toml_string: str,
         name: Tstr_opt = None,
         channels: Tstr_seq_opt = None,
-        python: Tstr_opt = None,
+        python_include: Tstr_opt = None,
     ) -> T:
         data = tomlkit.parse(toml_string)
-        return cls(data=data, name=name, channels=channels, python=python)
+        return cls(
+            data=data, name=name, channels=channels, python_include=python_include
+        )
 
     @classmethod
     def from_path(
         cls: type[T],
         path: str | Path,
         name: Tstr_opt = None,
         channels: Tstr_seq_opt = None,
-        python: Tstr_opt = None,
+        python_include: Tstr_opt = None,
     ) -> T:
         path = Path(path)
 
         if not path.exists():
             raise ValueError(f"{path} does not exist")
 
         with open(path, "rb") as f:
             data = tomlkit.load(f)
-        return cls(data=data, name=name, channels=channels, python=python)
+        return cls(
+            data=data, name=name, channels=channels, python_include=python_include
+        )
 
 
 def _list_to_stream(values, stream=None):
     value = "\n".join(values)
     if isinstance(stream, (str, Path)):
         with open(stream, "w") as f:
             f.write(value)
```

### Comparing `pyproject2conda-0.2.0/src/pyproject2conda.egg-info/PKG-INFO` & `pyproject2conda-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject2conda
-Version: 0.2.0
+Version: 0.3.0
 Summary: A script to convert a Python project declared on a pyproject.toml to a conda environment.
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/wpk-nist-gov/pyproject2conda
 Project-URL: documentation, https://pages.nist.gov/pyproject2conda/
 Keywords: pyproject2conda
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -92,58 +92,97 @@
 conda install -c wpk-nist pyproject2conda
 ```
 
 ## Example usage
 
 ### Basic usage
 
+<!-- [[[cog
+import subprocess
+import shlex
+
+def run_command(cmd, wrapper="bash", include_cmd=True):
+    args = shlex.split(cmd)
+    output = subprocess.check_output(args)
+
+    total = output.decode()
+    if include_cmd:
+        total = f"$ {cmd}\n{total}"
+
+    if wrapper:
+        total = f"\n```{wrapper}\n"  + total + "```\n"
+
+    print(total)
+
+def cat_lines(path="tests/test-pyproject.toml", begin=0, end=8, begin_dot=True, end_dot=True):
+    with open(path, 'r') as f:
+        lines = [line.rstrip() for line in f]
+
+    output = '\n'.join(lines[slice(begin, end)])
+
+    if begin_dot:
+        output = "# ...\n" +  output
+
+    if end_dot:
+        output = output + "\n# ..."
+
+    output = "\n```toml\n" + output + "\n```\n"
+    print(output)
+]]] -->
+<!-- [[[end]]] -->
+
 Consider the `toml` file [test-pyproject.toml](./tests/test-pyproject.toml).
 
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog cat_lines(begin=0, end=8, begin_dot=False)]]] -->
+
 ```toml
 [project]
 name = "hello"
 requires-python = ">=3.8,<3.11"
 dependencies = [
-  "athing", # p2c: -p # a comment
-  "bthing", # p2c: -s bthing-conda
-  "cthing", # p2c: -c conda-forge
-
+    "athing", # p2c: -p # a comment
+    "bthing", # p2c: -s "bthing-conda"
+    "cthing; python_version < '3.10'", # p2c: -c conda-forge
 ]
 # ...
-
 ```
 
+<!-- [[[end]]] -->
+<!-- prettier-ignore-end -->
+
 Note the comment lines `# p2c:...`. These are special tokens that
 `pyproject2conda` will analyze. The basic options are:
 
-```bash
-Arguments:   Additional (conda) packages
-
--p --pip     Pip install pyproject package on this line.
--s --skip    Skip pyproject package on this line.
--c --channel Add channel to pyproject package on this line
-```
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog run_command("""python -c "from pyproject2conda.parser import _default_parser; _default_parser().parse_args(['--help'])" """, include_cmd=False)]]] -->
 
-So, if we run the following, we get:
+```bash
+usage: -c [-h] [-c CHANNEL] [-p] [-s] [package ...]
 
-<!-- [[[cog
-import subprocess
-import shlex
+Parser searches for comments '# p2c: [OPTIONS]
 
-def run_command(cmd, wrapper="bash"):
-    args = shlex.split(cmd)
-    output = subprocess.check_output(args)
-    total = f"$ {cmd}\n{output.decode()}"
+positional arguments:
+  package
 
-    if wrapper:
-        total = f"\n```{wrapper}\n"  + total + "```\n"
+options:
+  -h, --help            show this help message and exit
+  -c CHANNEL, --channel CHANNEL
+                        Channel to add to the pyproject requirement
+  -p, --pip             If specified, install dependency on pyproject
+                        dependency (on this line) with pip
+  -s, --skip            If specified skip pyproject dependency on this line
+```
 
-    print(total)
-]]] -->
 <!-- [[[end]]] -->
+<!-- prettier-ignore-end -->
+
+So, if we run the following, we get:
 
 <!-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml")]]] -->
 
 ```bash
 $ pyproject2conda yaml -f tests/test-pyproject.toml
 channels:
@@ -154,71 +193,108 @@
   - pip
   - pip:
       - athing
 ```
 
 <!-- [[[end]]] -->
 
-Note that other comments can be mixed in. This also works with extras. For
-example, with the following:
+Note that other comments can be mixed in.
 
-Also, by default, the python version is not included in the resulting conda
-output. To include the specification from pyproject.toml, use `-p/--python`
-option:
+By default, the python version is not included in the resulting conda output. To
+include the specification from pyproject.toml, use `-p/--python` option:
 
 <!-- markdownlint-disable-next-line MD013 -->
-<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -p")]]] -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml --python-include")]]] -->
 
 ```bash
-$ pyproject2conda yaml -f tests/test-pyproject.toml -p
+$ pyproject2conda yaml -f tests/test-pyproject.toml --python-include
 channels:
   - conda-forge
 dependencies:
   - python>=3.8,<3.11
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
 ```
 
 <!-- [[[end]]] -->
 
-To specify a value of python, pass a value with:
+To specify a specific value of python in the output, pass a value with:
 
 <!-- markdownlint-disable-next-line MD013 -->
-<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -p python=3.9")]]] -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml --python-include python=3.9")]]] -->
 
 ```bash
-$ pyproject2conda yaml -f tests/test-pyproject.toml -p python=3.9
+$ pyproject2conda yaml -f tests/test-pyproject.toml --python-include python=3.9
 channels:
   - conda-forge
 dependencies:
   - python=3.9
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
 ```
 
 <!-- [[[end]]] -->
 
+Note that this is for including python in the resulting environment file.
+
+You can also constrain packages by the python version using the standard
+pyproject.toml syntax `"...; python_version < 'some-version-number'"`. For is
+parsed for for both the pip packages and conda packages:
+
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml --python-version 3.10")]]] -->
+
+```bash
+$ pyproject2conda yaml -f tests/test-pyproject.toml --python-version 3.10
+channels:
+  - conda-forge
+dependencies:
+  - bthing-conda
+  - pip
+  - pip:
+      - athing
+```
+
+<!-- [[[end]]] -->
+
+### Installing extras
+
+Given the extra dependency:
+
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable MD013 -->
+<!-- [[[cog cat_lines(begin=9, end=21)]]] -->
+
 ```toml
 # ...
 [project.optional-dependencies]
 test = [
-  "pandas",
-  "pytest", # p2c: -c conda-forge
+    "pandas",
+    "pytest", # p2c: -c conda-forge
 
 ]
+dev-extras = [
+    # p2c: -s "additional-thing; python_version < '3.9'" # this is an additional conda package
+    ## p2c: -s "another-thing" # this will be skipped because of ## before p2c.
+    "matplotlib", # p2c: -s conda-matplotlib
+]
+dev = ["hello[test]", "hello[dev-extras]"]
 # ...
-
 ```
 
+<!-- [[[end]]] -->
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
 and running the the following gives:
 
 <!-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -e test")]]] -->
 
 ```bash
 $ pyproject2conda yaml -f tests/test-pyproject.toml -e test
@@ -234,28 +310,14 @@
       - athing
 ```
 
 <!-- [[[end]]] -->
 
 `pyproject2conda` also works with self referenced dependencies:
 
-```toml
-# ...
-[project.optional-dependencies]
-# ...
-dev-extras = [
-  # p2c: -s additional-thing # this is an additional conda package
-  "matplotlib", # p2c: -s conda-matplotlib
-
-]
-dev = ["hello[test]", "hello[dev-extras]"]
-# ...
-
-```
-
 <!-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -e dev")]]] -->
 
 ```bash
 $ pyproject2conda yaml -f tests/test-pyproject.toml -e dev
 channels:
   - conda-forge
@@ -269,24 +331,27 @@
   - pip
   - pip:
       - athing
 ```
 
 <!-- [[[end]]] -->
 
+This also shows that `p2c` comments without dependencies are also parsed. To
+comment out such lines, make sure `p2c` is preceded by `##`.
+
 ### Usage within python
 
 `pyproject2conda` can also be used within python:
 
 ```pycon
 >>> from pyproject2conda import PyProject2Conda
 >>> p = PyProject2Conda.from_path("./tests/test-pyproject.toml")
 
 # Basic environment
->>> print(p.to_conda_yaml(python="get").strip())
+>>> print(p.to_conda_yaml(python_include="get").strip())
 channels:
   - conda-forge
 dependencies:
   - python>=3.8,<3.11
   - bthing-conda
   - conda-forge::cthing
   - pip
@@ -309,37 +374,52 @@
 ```
 
 ### Configuration
 
 `pyproject2conda` can be configured with a `[tool.pyproject2conda]` section in
 `pyproject.toml`. To specify conda channels use:
 
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog cat_lines(begin=22, end=24)]]] -->
+
 ```toml
-# Why channel conda-forge appeared above
+# ...
 [tool.pyproject2conda]
-channels = ["conda-forge"]
-
+channels = ['conda-forge']
+# ...
 ```
 
+<!-- [[[end]]] -->
+<!-- prettier-ignore-end -->
+
 Note that specifying channels at the comand line overrides
 
 You can also specify `isolated-dependencies`. These are dependencies for things
 that should not include package dependencies (things like build dependencies).
 For example:
 
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog cat_lines(begin=25, end=None)]]] -->
+
 ```toml
+# ...
 [tool.pyproject2conda.isolated-dependencies]
 dist-pypi = [
-  "setuptools",
-  "build", # p2c: -p
+    "setuptools",
+    "build", # p2c: -p
 
 ]
-
+# ...
 ```
 
+<!-- [[[end]]] -->
+<!-- prettier-ignore-end -->
+
 These can be accessed using either of the following:
 
 <!-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml -i dist-pypi")]]] -->
 
 ```bash
 $ pyproject2conda yaml -f tests/test-pyproject.toml -i dist-pypi
@@ -370,14 +450,15 @@
   - pip:
       - build
 
 ```
 
 ### CLI options
 
+<!-- prettier-ignore-start -->
 <!-- [[[cog run_command("pyproject2conda --help")]]] -->
 
 ```bash
 $ pyproject2conda --help
 Usage: pyproject2conda [OPTIONS] COMMAND [ARGS]...
 
 Options:
@@ -414,28 +495,36 @@
 ```bash
 $ pyproject2conda yaml --help
 Usage: pyproject2conda yaml [OPTIONS]
 
   Create yaml file from dependencies and optional-dependencies.
 
 Options:
-  -e, --extra TEXT     Extra depenedencies. Can specify multiple times for
-                       multiple extras.
-  -i, --isolated TEXT  Isolated dependencies (under
-                       [tool.pyproject2conda.isolated-dependencies]).  Can
-                       specify multiple times.
-  -c, --channel TEXT   conda channel.  Can specify. Overrides
-                       [tool.pyproject2conda.channels]
-  -f, --file PATH      input pyproject.toml file
-  -n, --name TEXT      Name of conda env
-  -o, --output PATH    File to output results
-  -p, --python TEXT    if flag passed without options, include python spec
-                       from pyproject.toml in output.  If value passed, use
-                       this value of python in the output
-  --help               Show this message and exit.
+  -e, --extra TEXT       Extra depenedencies. Can specify multiple times for
+                         multiple extras.
+  -i, --isolated TEXT    Isolated dependencies (under
+                         [tool.pyproject2conda.isolated-dependencies]).  Can
+                         specify multiple times.
+  -c, --channel TEXT     conda channel.  Can specify. Overrides
+                         [tool.pyproject2conda.channels]
+  -f, --file PATH        input pyproject.toml file
+  -n, --name TEXT        Name of conda env
+  -o, --output PATH      File to output results
+  --python-include TEXT  If flag passed without options, include python spec
+                         from pyproject.toml in yaml output.  If value passed,
+                         use this value (exactly) in the output. So, for
+                         example, pass `--python-include "python=3.8"`
+  --python-version TEXT  Python version to check `python_verion <=>
+                         {python_version}` lines against.  That is, this
+                         version is used to limit packages in resulting
+                         output. For example, if have a line like
+                         `a-package; python_version < '3.9'`, Using `--python-
+                         version 3.10` will not include `a-package`, while
+                         `--python-version 3.8` will include `a-package`.
+  --help                 Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
 
 <!-- [[[cog run_command("pyproject2conda requirements --help")]]] -->
 
 ```bash
@@ -466,29 +555,37 @@
   Create requirement files for conda and pip.
 
   These can be install with, for example,
 
   conda install --file {path_conda} pip install -r {path_pip}
 
 Options:
-  -e, --extra TEXT     Extra depenedencies. Can specify multiple times for
-                       multiple extras.
-  -i, --isolated TEXT  Isolated dependencies (under
-                       [tool.pyproject2conda.isolated-dependencies]).  Can
-                       specify multiple times.
-  -p, --python TEXT    if flag passed without options, include python spec
-                       from pyproject.toml in output.  If value passed, use
-                       this value of python in the output
-  -c, --channel TEXT   conda channel.  Can specify. Overrides
-                       [tool.pyproject2conda.channels]
-  -f, --file PATH      input pyproject.toml file
-  --prefix TEXT        set conda-output=prefix + 'conda.txt', pip-
-                       output=prefix + 'pip.txt'
+  -e, --extra TEXT       Extra depenedencies. Can specify multiple times for
+                         multiple extras.
+  -i, --isolated TEXT    Isolated dependencies (under
+                         [tool.pyproject2conda.isolated-dependencies]).  Can
+                         specify multiple times.
+  --python-include TEXT  If flag passed without options, include python spec
+                         from pyproject.toml in yaml output.  If value passed,
+                         use this value (exactly) in the output. So, for
+                         example, pass `--python-include "python=3.8"`
+  --python-version TEXT  Python version to check `python_verion <=>
+                         {python_version}` lines against.  That is, this
+                         version is used to limit packages in resulting
+                         output. For example, if have a line like
+                         `a-package; python_version < '3.9'`, Using `--python-
+                         version 3.10` will not include `a-package`, while
+                         `--python-version 3.8` will include `a-package`.
+  -c, --channel TEXT     conda channel.  Can specify. Overrides
+                         [tool.pyproject2conda.channels]
+  -f, --file PATH        input pyproject.toml file
+  --prefix TEXT          set conda-output=prefix + 'conda.txt', pip-
+                         output=prefix + 'pip.txt'
   --prepend-channel
-  --help               Show this message and exit.
+  --help                 Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
 
 <!-- [[[cog run_command("pyproject2conda json --help")]]] -->
 
 ```bash
@@ -497,30 +594,39 @@
 
   Create json representation.
 
   Keys are: "dependencies": conda dependencies. "pip": pip dependencies.
   "channels": conda channels.
 
 Options:
-  -e, --extra TEXT     Extra depenedencies. Can specify multiple times for
-                       multiple extras.
-  -i, --isolated TEXT  Isolated dependencies (under
-                       [tool.pyproject2conda.isolated-dependencies]).  Can
-                       specify multiple times.
-  -p, --python TEXT    if flag passed without options, include python spec
-                       from pyproject.toml in output.  If value passed, use
-                       this value of python in the output
-  -c, --channel TEXT   conda channel.  Can specify. Overrides
-                       [tool.pyproject2conda.channels]
-  -f, --file PATH      input pyproject.toml file
-  -o, --output PATH    File to output results
-  --help               Show this message and exit.
+  -e, --extra TEXT       Extra depenedencies. Can specify multiple times for
+                         multiple extras.
+  -i, --isolated TEXT    Isolated dependencies (under
+                         [tool.pyproject2conda.isolated-dependencies]).  Can
+                         specify multiple times.
+  --python-include TEXT  If flag passed without options, include python spec
+                         from pyproject.toml in yaml output.  If value passed,
+                         use this value (exactly) in the output. So, for
+                         example, pass `--python-include "python=3.8"`
+  --python-version TEXT  Python version to check `python_verion <=>
+                         {python_version}` lines against.  That is, this
+                         version is used to limit packages in resulting
+                         output. For example, if have a line like
+                         `a-package; python_version < '3.9'`, Using `--python-
+                         version 3.10` will not include `a-package`, while
+                         `--python-version 3.8` will include `a-package`.
+  -c, --channel TEXT     conda channel.  Can specify. Overrides
+                         [tool.pyproject2conda.channels]
+  -f, --file PATH        input pyproject.toml file
+  -o, --output PATH      File to output results
+  --help                 Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
+<!-- prettier-ignore-end -->
 
 <!-- end-docs -->
 
 <!-- ## Documentation -->
 
 <!-- See the [documentation][docs-link] for a look at -->
 <!-- `pyproject2conda` in action. -->
```

### Comparing `pyproject2conda-0.2.0/src/pyproject2conda.egg-info/SOURCES.txt` & `pyproject2conda-0.3.0/src/pyproject2conda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.2.0/tests/test-pyproject.toml` & `pyproject2conda-0.3.0/tests/test-pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [project]
 name = "hello"
 requires-python = ">=3.8,<3.11"
 dependencies = [
     "athing", # p2c: -p # a comment
-    "bthing", # p2c: -s bthing-conda
-    "cthing", # p2c: -c conda-forge
+    "bthing", # p2c: -s "bthing-conda"
+    "cthing; python_version < '3.10'", # p2c: -c conda-forge
 
 ]
 
 [project.optional-dependencies]
 test = [
     "pandas",
     "pytest", # p2c: -c conda-forge
 
 ]
 dev-extras = [
-    # p2c: -s additional-thing # this is an additional conda package
+    # p2c: -s "additional-thing; python_version < '3.9'" # this is an additional conda package
+    ## p2c: -s "another-thing" # this will be skipped because of ## before p2c.
     "matplotlib", # p2c: -s conda-matplotlib
 
 ]
 dev = ["hello[test]", "hello[dev-extras]"]
 
 [tool.pyproject2conda]
 channels = ['conda-forge']
```

### Comparing `pyproject2conda-0.2.0/tests/test_cli.py` & `pyproject2conda-0.3.0/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
     """
 
-    for opt in ["-p", "--python"]:
+    for opt in ["--python-include"]:
         result = do_run(runner, "yaml", opt)
         check_result(result, expected)
 
     # -p python=3.8
     expected = """\
 channels:
   - conda-forge
@@ -72,15 +72,15 @@
   - python=3.8
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
     """
-    for opt in ["-p", "--python"]:
+    for opt in ["--python-include"]:
         result = do_run(runner, "yaml", opt, "python=3.8")
         check_result(result, expected)
 
     # dev
     expected = """\
 channels:
   - conda-forge
@@ -169,24 +169,24 @@
 
 def test_requirements():
     runner = CliRunner()
 
     expected = """\
 athing
 bthing
-cthing
+cthing; python_version < '3.10'
     """
 
     result = do_run(runner, "requirements")
     check_result(result, expected)
 
     expected = """\
 athing
 bthing
-cthing
+cthing; python_version < '3.10'
 pandas
 pytest
 matplotlib
     """
 
     result = do_run(runner, "requirements", "-e", "dev")
     check_result(result, expected)
```

### Comparing `pyproject2conda-0.2.0/tests/test_parser.py` & `pyproject2conda-0.3.0/tests/test_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,20 +11,37 @@
         "# p2c: -c -d # some other thing",
         "# some other thing # p2c: -c -d # another thing",
     ]:
         match = parser._match_p2c_comment(comment)
 
         assert match == expected
 
+    # check for skip
+    for comment in [
+        "##p2c: -c -d",
+        "## p2c: -c -d",
+        "  ##p2c: -c -d",
+        "## p2c: -c -d # some other thing",
+        "# some other thing ## p2c: -c -d # another thing",
+    ]:
+        match = parser._match_p2c_comment(comment)
+
+        assert match is None
+
 
 def test_parse_p2c():
     def get_expected(pip=False, skip=False, channel=None, package=None):
         if package is None:
             package = []
-        return {"pip": pip, "skip": skip, "channel": channel, "package": package}
+        return {
+            "pip": pip,
+            "skip": skip,
+            "channel": channel,
+            "package": package,
+        }
 
     assert parser._parse_p2c("--pip") == get_expected(pip=True)
     assert parser._parse_p2c("-p") == get_expected(pip=True)
 
     assert parser._parse_p2c("--skip") == get_expected(skip=True)
     assert parser._parse_p2c("-s") == get_expected(skip=True)
 
@@ -36,27 +53,29 @@
         package=["athing>=0.3,<0.2"]
     )
 
     assert parser._parse_p2c("athing>=0.3,<0.2 bthing ") == get_expected(
         package=["athing>=0.3,<0.2", "bthing"]
     )
 
+    assert parser._parse_p2c("'athing >= 0.3, <0.2' bthing ") == get_expected(
+        package=["athing >= 0.3, <0.2", "bthing"]
+    )
 
-def test_complete():
-    from tomlkit import parse
 
+def test_complete():
     toml = dedent(
         """\
     [project]
     name = "hello"
     requires-python = ">=3.8,<3.11"
     dependencies = [
     "athing", # p2c: -p # a comment
     "bthing", # p2c: -s bthing-conda
-    "cthing", # p2c: -c conda-forge
+    "cthing; python_version<'3.10'", # p2c: -c conda-forge
     ]
 
     [project.optional-dependencies]
     test = [
     "pandas",
     "pytest", # p2c: -c conda-forge
     ]
@@ -78,61 +97,68 @@
     "build", # p2c: -p
     ]
     """
     )
 
     d = parser.PyProject2Conda.from_string(toml)
 
-    out = d.to_conda_yaml()
-
     expected = """\
 channels:
   - conda-forge
 dependencies:
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
     """
 
-    assert dedent(expected) == out
+    assert dedent(expected) == d.to_conda_yaml()
 
     # test -p option
-    out = d.to_conda_yaml(python="get")
-
     expected = """\
 channels:
   - conda-forge
 dependencies:
   - python>=3.8,<3.11
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
     """
-
-    assert dedent(expected) == out
-
-    out = d.to_conda_yaml(python="python=3.9")
+    assert dedent(expected) == d.to_conda_yaml(python_include="get")
 
     expected = """\
 channels:
   - conda-forge
 dependencies:
   - python=3.9
   - bthing-conda
   - conda-forge::cthing
   - pip
   - pip:
       - athing
     """
+    assert dedent(expected) == d.to_conda_yaml(python_include="python=3.9")
 
-    assert dedent(expected) == out
+    # test passing python_version
+    expected = """\
+channels:
+  - conda-forge
+dependencies:
+  - python=3.10
+  - bthing-conda
+  - pip
+  - pip:
+      - athing
+    """
+    assert dedent(expected) == d.to_conda_yaml(
+        python_include="python=3.10", python_version="3.10"
+    )
 
     out = d.to_conda_yaml(channels="hello")
 
     expected = """\
 channels:
   - hello
 dependencies:
```

### Comparing `pyproject2conda-0.2.0/tox.ini` & `pyproject2conda-0.3.0/tox.ini`

 * *Files identical despite different names*

