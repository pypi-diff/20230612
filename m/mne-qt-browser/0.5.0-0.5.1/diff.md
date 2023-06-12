# Comparing `tmp/mne-qt-browser-0.5.0.tar.gz` & `tmp/mne-qt-browser-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mne-qt-browser-0.5.0.tar", last modified: Thu Apr  6 01:43:30 2023, max compression
+gzip compressed data, was "mne-qt-browser-0.5.1.tar", last modified: Mon Jun 12 19:08:56 2023, max compression
```

## Comparing `mne-qt-browser-0.5.0.tar` & `mne-qt-browser-0.5.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:43:30.812919 mne-qt-browser-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:43:30.804919 mne-qt-browser-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:43:30.804919 mne-qt-browser-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:43:30.804919 mne-qt-browser-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/.github/workflows/qt_viz_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-06 01:43:30.812919 mne-qt-browser-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:43:30.804919 mne-qt-browser-0.5.0/mne_qt_browser/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/_fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)   183910 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/_pg_figure.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-06 01:43:30.000000 mne-qt-browser-0.5.0/mne_qt_browser/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/figure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:43:30.808919 mne-qt-browser-0.5.0/mne_qt_browser/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:43:30.808919 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:43:30.808919 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/annotations.svg
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/fullscreen.svg
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/help.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/less_channels.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/less_time.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/more_channels.svg
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/more_time.svg
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/overview_bar.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/settings.svg
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/ssp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/zoom_in.svg
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/zoom_out.svg
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/index.theme
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:43:30.808919 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:43:30.812919 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/annotations.svg
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/fullscreen.svg
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/help.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/less_channels.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/less_time.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/more_channels.svg
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/more_time.svg
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/overview_bar.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/settings.svg
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/ssp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/zoom_in.svg
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/zoom_out.svg
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/icons/light/index.theme
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:43:30.812919 mne-qt-browser-0.5.0/mne_qt_browser/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/tests/test_pg_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/mne_qt_browser/tests/test_speed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:43:30.808919 mne-qt-browser-0.5.0/mne_qt_browser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-06 01:43:30.000000 mne-qt-browser-0.5.0/mne_qt_browser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-06 01:43:30.000000 mne-qt-browser-0.5.0/mne_qt_browser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 01:43:30.000000 mne-qt-browser-0.5.0/mne_qt_browser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-06 01:43:30.000000 mne-qt-browser-0.5.0/mne_qt_browser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-06 01:43:30.000000 mne-qt-browser-0.5.0/mne_qt_browser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)   770491 2023-04-06 01:43:12.000000 mne-qt-browser-0.5.0/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 01:43:30.812919 mne-qt-browser-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:08:56.877947 mne-qt-browser-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:08:56.869947 mne-qt-browser-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:08:56.869947 mne-qt-browser-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:08:56.869947 mne-qt-browser-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/.github/workflows/qt_viz_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-12 19:08:56.877947 mne-qt-browser-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:08:56.873947 mne-qt-browser-0.5.1/mne_qt_browser/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/_pg_figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 19:08:56.000000 mne-qt-browser-0.5.1/mne_qt_browser/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/figure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:08:56.873947 mne-qt-browser-0.5.1/mne_qt_browser/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:08:56.873947 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:08:56.873947 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/annotations.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/fullscreen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/help.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/less_channels.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/less_time.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/more_channels.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/more_time.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/overview_bar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/ssp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/zoom_in.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/zoom_out.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/index.theme
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:08:56.873947 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:08:56.877947 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/annotations.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/fullscreen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/help.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/less_channels.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/less_time.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/more_channels.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/more_time.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/overview_bar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/ssp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/zoom_in.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/zoom_out.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/icons/light/index.theme
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:08:56.877947 mne-qt-browser-0.5.1/mne_qt_browser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/tests/test_pg_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/mne_qt_browser/tests/test_speed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:08:56.873947 mne-qt-browser-0.5.1/mne_qt_browser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-12 19:08:56.000000 mne-qt-browser-0.5.1/mne_qt_browser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-12 19:08:56.000000 mne-qt-browser-0.5.1/mne_qt_browser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:08:56.000000 mne-qt-browser-0.5.1/mne_qt_browser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-12 19:08:56.000000 mne-qt-browser-0.5.1/mne_qt_browser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 19:08:56.000000 mne-qt-browser-0.5.1/mne_qt_browser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)   770491 2023-06-12 19:08:36.000000 mne-qt-browser-0.5.1/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:08:56.877947 mne-qt-browser-0.5.1/setup.cfg
```

### Comparing `mne-qt-browser-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `mne-qt-browser-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `mne-qt-browser-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/.github/pull_request_template.md` & `mne-qt-browser-0.5.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/.github/workflows/qt_viz_tests.yml` & `mne-qt-browser-0.5.1/.github/workflows/qt_viz_tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   group: ${{ github.workflow }}-${{ github.event.number }}-${{ github.event.type }}
   cancel-in-progress: true
 on:
     pull_request:
     push:
       branches: [main]
     schedule:
-      - cron: "0 4 * * *"
+      - cron: "0 4 * * 1"  # At 04:00 on Monday
 
 jobs:
   style:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
@@ -25,15 +25,15 @@
       - name: Lint with ruff
         run: ruff .
   pytest:
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu, windows, macos]
-        mne: [main, maint/1.3]
+        mne: [main, maint/1.4]
         opengl: ['opengl']
         python: ['3.11']
         name: [matrix]
         include:
           - os: ubuntu
             mne: main
             opengl: 'opengl'
@@ -41,20 +41,20 @@
             name: old 3.8
           - os: ubuntu
             mne: main
             opengl: ''
             python: '3.9'
             name: no opengl
           - os: ubuntu
-            mne: maint/1.3
+            mne: maint/1.4
             opengl: ''
             python: '3.9'
             name: no opengl
           - os: ubuntu
-            mne: maint/1.0
+            mne: maint/1.3
             opengl: 'opengl'
             python: '3.9'
             name: old
     name: pytest ${{ matrix.name }} / ${{ matrix.os }} / MNE ${{ matrix.mne }}
     runs-on: ${{ matrix.os }}-latest
     env:
       MNE_LOGGING_LEVEL: 'warning'
@@ -101,15 +101,15 @@
           qt: true
       - run: glxinfo | grep enderer
         name: Check OpenGL
         working-directory: ../mne-python
         if: runner.os == 'Linux' && contains(matrix.opengl, 'opengl')
       - name: Show system information
         run: mne sys_info
-      - run: pytest -m pgtest --cov=mne_qt_browser --cov-report=xml ../mne-python/mne/viz ../mne-python/mne/report
+      - run: pytest -m pgtest --cov=mne_qt_browser --cov-report=xml ../mne-python/mne/report ../mne-python/mne/viz
         name: Run MNE-Tests
       - run: pytest --error-for-skips mne_qt_browser/tests/test_pg_specific.py
         name: Run pyqtgraph-specific tests
       # These are slow on macOS, so skip them
       - run: pytest mne_qt_browser/tests/test_speed.py
         name: Run benchmarks
         if: runner.os != 'macOS'
@@ -160,16 +160,17 @@
       - name: Install dependencies
         run: |  # use MNE main to ensure test files are available
           set -e
           python -m pip install --upgrade pip
           git clone -b ${MNE_BRANCH} --single-branch --branch main https://github.com/mne-tools/mne-python.git ../mne-python
           python -m pip install -qe ../mne-python
           # Avoid a problematic version of PySide6
+          # https://wiki.qt.io/Qt_for_Python_Development_Notes#1._Juni_2023
           if [[ "$QT_LIB" == "PySide6" ]]; then
-            QT_LIB_INSTALL="PySide6!=6.5"
+            QT_LIB_INSTALL="PySide6!=6.5.1"
           else
             QT_LIB_INSTALL="$QT_LIB"
           fi
           if [[ "${{ matrix.opengl }}" == "opengl" ]]; then
             PIP_OPTION="[opengl,tests]"
           else
             PIP_OPTION="[tests]"
@@ -192,15 +193,15 @@
       - name: Start Qt on its own
         run: LD_DEBUG=libs python -c "from ${QT_LIB}.QtWidgets import QApplication, QWidget; app = QApplication([]); import matplotlib; matplotlib.use('QtAgg'); import matplotlib.pyplot as plt; plt.figure()"
       - name: Check Qt
         run: |
           mne sys_info -pd
           echo ${QT_LIB}:
           mne sys_info -pd | grep "^.*qtpy.*${QT_LIB}=.*$"
-      - run: pytest -m pgtest --cov=mne_qt_browser --cov-report=xml ../mne-python/mne/viz ../mne-python/mne/report
+      - run: pytest -m pgtest --cov=mne_qt_browser --cov-report=xml ../mne-python/mne/report ../mne-python/mne/viz
         name: Run MNE-Tests
       - run: pytest --error-for-skips mne_qt_browser/tests/test_pg_specific.py
         name: Run pyqtgraph-specific tests
       # For some reason this dies on Linux PySide2. We can live without this
       # case given our primary target moving forward is Qt6+
       - run: pytest mne_qt_browser/tests/test_speed.py
         name: Run benchmarks
```

### Comparing `mne-qt-browser-0.5.0/.github/workflows/release.yml` & `mne-qt-browser-0.5.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/.gitignore` & `mne-qt-browser-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/CONTRIBUTING.md` & `mne-qt-browser-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/LICENSE` & `mne-qt-browser-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/PKG-INFO` & `mne-qt-browser-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mne-qt-browser
-Version: 0.5.0
+Version: 0.5.1
 Summary: A new backend based on pyqtgraph for the 2D-Data-Browser in MNE-Python
 Author-email: Martin Schulz <dev@earthman-music.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2021-2022, authors of mne-qt-browser
         All rights reserved.
```

### Comparing `mne-qt-browser-0.5.0/README.md` & `mne-qt-browser-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/codecov.yml` & `mne-qt-browser-0.5.1/codecov.yml`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/_fixes.py` & `mne-qt-browser-0.5.1/mne_qt_browser/_fixes.py`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/_pg_figure.py` & `mne-qt-browser-0.5.1/mne_qt_browser/_pg_figure.py`

 * *Files 0% similar despite different names*

```diff
@@ -6438,5058 +6438,5092 @@
 00019250: 6564 5f72 656d 6f76 655f 6463 203d 2073  ed_remove_dc = s
 00019260: 656c 662e 6d6e 652e 7265 6d6f 7665 5f64  elf.mne.remove_d
 00019270: 630a 2020 2020 2020 2020 7365 6c66 2e6d  c.        self.m
 00019280: 6e65 2e72 656d 6f76 655f 6463 203d 2046  ne.remove_dc = F
 00019290: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
 000192a0: 6120 3d20 6272 6f77 7365 722e 5f70 726f  a = browser._pro
 000192b0: 6365 7373 5f64 6174 6128 6461 7461 2c20  cess_data(data, 
-000192c0: 302c 206c 656e 2864 6174 6129 2c20 7069  0, len(data), pi
-000192d0: 636b 732c 2073 656c 6629 0a20 2020 2020  cks, self).     
-000192e0: 2020 2073 656c 662e 6d6e 652e 7265 6d6f     self.mne.remo
-000192f0: 7665 5f64 6320 3d20 7374 6173 6865 645f  ve_dc = stashed_
-00019300: 7265 6d6f 7665 5f64 630a 0a20 2020 2020  remove_dc..     
-00019310: 2020 2073 656c 662e 6d6e 652e 676c 6f62     self.mne.glob
-00019320: 616c 5f64 6174 6120 3d20 6461 7461 0a20  al_data = data. 
-00019330: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-00019340: 676c 6f62 616c 5f74 696d 6573 203d 2074  global_times = t
-00019350: 696d 6573 0a0a 2020 2020 2020 2020 2320  imes..        # 
-00019360: 4361 6c63 756c 6174 6520 5a2d 5363 6f72  Calculate Z-Scor
-00019370: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
-00019380: 7072 6f63 6573 7354 6578 742e 656d 6974  processText.emit
-00019390: 2827 4361 6c63 756c 6174 696e 6720 5a2d  ('Calculating Z-
-000193a0: 5363 6f72 6573 2e2e 2e27 290a 2020 2020  Scores...').    
-000193b0: 2020 2020 6272 6f77 7365 722e 5f67 6574      browser._get
-000193c0: 5f7a 7363 6f72 6528 6461 7461 290a 2020  _zscore(data).  
-000193d0: 2020 2020 2020 6465 6c20 6272 6f77 7365        del browse
-000193e0: 720a 0a20 2020 2020 2020 2073 656c 662e  r..        self.
-000193f0: 6c6f 6164 696e 6746 696e 6973 6865 642e  loadingFinished.
-00019400: 656d 6974 2829 0a0a 2020 2020 6465 6620  emit()..    def 
-00019410: 636c 6561 6e28 7365 6c66 293a 2020 2320  clean(self):  # 
-00019420: 6e6f 7161 3a20 4431 3032 0a20 2020 2020  noqa: D102.     
-00019430: 2020 2069 6620 7365 6c66 2e69 7352 756e     if self.isRun
-00019440: 6e69 6e67 2829 3a0a 2020 2020 2020 2020  ning():.        
-00019450: 2020 2020 7761 6974 5f74 696d 6520 3d20      wait_time = 
-00019460: 3130 2020 2320 6d61 782e 2077 6169 7469  10  # max. waiti
-00019470: 6e67 2074 696d 6520 696e 2073 6563 6f6e  ng time in secon
-00019480: 6473 0a20 2020 2020 2020 2020 2020 206c  ds.            l
-00019490: 6f67 6765 722e 696e 666f 2827 5761 6974  ogger.info('Wait
-000194a0: 696e 6720 666f 7220 4c6f 6164 696e 672d  ing for Loading-
-000194b0: 5468 7265 6164 2074 6f20 6669 6e69 7368  Thread to finish
-000194c0: 2e2e 2e20 270a 2020 2020 2020 2020 2020  ... '.          
-000194d0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-000194e0: 286d 6178 2e20 7b77 6169 745f 7469 6d65  (max. {wait_time
-000194f0: 7d20 7365 6329 2729 0a20 2020 2020 2020  } sec)').       
-00019500: 2020 2020 2073 656c 662e 7761 6974 2869       self.wait(i
-00019510: 6e74 2877 6169 745f 7469 6d65 202a 2031  nt(wait_time * 1
-00019520: 6533 2929 0a20 2020 2020 2020 205f 6469  e3)).        _di
-00019530: 7363 6f6e 6e65 6374 2873 656c 662e 6c6f  sconnect(self.lo
-00019540: 6164 5072 6f67 7265 7373 290a 2020 2020  adProgress).    
-00019550: 2020 2020 5f64 6973 636f 6e6e 6563 7428      _disconnect(
-00019560: 7365 6c66 2e70 726f 6365 7373 5465 7874  self.processText
-00019570: 290a 2020 2020 2020 2020 5f64 6973 636f  ).        _disco
-00019580: 6e6e 6563 7428 7365 6c66 2e6c 6f61 6469  nnect(self.loadi
-00019590: 6e67 4669 6e69 7368 6564 290a 2020 2020  ngFinished).    
-000195a0: 2020 2020 6465 6c20 7365 6c66 2e6d 6e65      del self.mne
-000195b0: 0a20 2020 2020 2020 2064 656c 2073 656c  .        del sel
-000195c0: 662e 7765 616b 6272 6f77 7365 720a 0a0a  f.weakbrowser...
-000195d0: 636c 6173 7320 5f50 474d 6574 6143 6c61  class _PGMetaCla
-000195e0: 7373 2874 7970 6528 514d 6169 6e57 696e  ss(type(QMainWin
-000195f0: 646f 7729 2c20 7479 7065 2842 726f 7773  dow), type(Brows
-00019600: 6572 4261 7365 2929 3a0a 2020 2020 2222  erBase)):.    ""
-00019610: 2243 6c61 7373 2069 7320 6e65 6365 7373  "Class is necess
-00019620: 6172 7920 746f 2070 7265 7665 6e74 2061  ary to prevent a
-00019630: 206d 6574 6163 6c61 7373 2063 6f6e 666c   metaclass confl
-00019640: 6963 742e 0a0a 2020 2020 5468 6520 636f  ict...    The co
-00019650: 6e66 6c69 6374 2061 7269 7365 7320 6475  nflict arises du
-00019660: 6520 746f 2074 6865 2064 6966 6665 7265  e to the differe
-00019670: 6e74 2074 7970 6573 206f 6620 514d 6169  nt types of QMai
-00019680: 6e57 696e 646f 7720 616e 640a 2020 2020  nWindow and.    
-00019690: 4272 6f77 7365 7242 6173 652e 0a20 2020  BrowserBase..   
-000196a0: 2022 2222 0a0a 2020 2020 7061 7373 0a0a   """..    pass..
-000196b0: 0a23 2054 686f 7365 2061 7265 2074 6865  .# Those are the
-000196c0: 2073 6574 7469 6e67 7320 7768 6963 6820   settings which 
-000196d0: 6172 6520 7374 6f72 6564 206f 6e20 6561  are stored on ea
-000196e0: 6368 2064 6576 6963 650a 2320 6465 7065  ch device.# depe
-000196f0: 6e64 696e 6720 6f6e 2069 7473 206f 7065  nding on its ope
-00019700: 7261 7469 6e67 2073 7973 7465 6d20 7769  rating system wi
-00019710: 7468 2051 5365 7474 696e 6773 2e0a 0a71  th QSettings...q
-00019720: 7365 7474 696e 6773 5f70 6172 616d 7320  settings_params 
-00019730: 3d20 7b0a 2020 2020 2320 416e 7469 616c  = {.    # Antial
-00019740: 6961 7369 6e67 2028 776f 726b 7320 7769  iasing (works wi
-00019750: 7468 2f77 6974 686f 7574 204f 7065 6e47  th/without OpenG
-00019760: 4c2c 2069 6e74 6567 6572 2062 6563 6175  L, integer becau
-00019770: 7365 2051 5365 7474 696e 6773 0a20 2020  se QSettings.   
-00019780: 2023 2063 616e 2774 2068 616e 646c 6520   # can't handle 
-00019790: 626f 6f6c 6561 6e73 290a 2020 2020 2761  booleans).    'a
-000197a0: 6e74 6961 6c69 6173 696e 6727 3a20 4661  ntialiasing': Fa
-000197b0: 6c73 652c 0a20 2020 2023 2053 7465 7073  lse,.    # Steps
-000197c0: 2070 6572 2076 6965 7720 2872 656c 6174   per view (relat
-000197d0: 6976 6520 746f 2074 696d 6529 0a20 2020  ive to time).   
-000197e0: 2027 7363 726f 6c6c 5f73 656e 7369 7469   'scroll_sensiti
-000197f0: 7669 7479 273a 2031 3030 2c0a 2020 2020  vity': 100,.    
-00019800: 2320 446f 776e 7361 6d70 6c69 6e67 2d46  # Downsampling-F
-00019810: 6163 746f 7220 286f 7220 2761 7574 6f27  actor (or 'auto'
-00019820: 2c20 7365 6520 5365 7474 696e 6773 4469  , see SettingsDi
-00019830: 616c 6f67 2066 6f72 2064 6574 6169 6c73  alog for details
-00019840: 290a 2020 2020 2764 6f77 6e73 616d 706c  ).    'downsampl
-00019850: 696e 6727 3a20 312c 0a20 2020 2023 2044  ing': 1,.    # D
-00019860: 6f77 6e73 616d 706c 696e 672d 4d65 7468  ownsampling-Meth
-00019870: 6f64 2028 7365 7420 5365 7474 696e 6773  od (set Settings
-00019880: 4469 616c 6f67 2066 6f72 2064 6574 6169  Dialog for detai
-00019890: 6c73 290a 2020 2020 2764 735f 6d65 7468  ls).    'ds_meth
-000198a0: 6f64 273a 2027 7065 616b 270a 7d0a 0a0a  od': 'peak'.}...
-000198b0: 6465 6620 5f73 6372 6565 6e5f 6765 6f6d  def _screen_geom
-000198c0: 6574 7279 2877 6964 6765 7429 3a0a 2020  etry(widget):.  
-000198d0: 2020 7472 793a 0a20 2020 2020 2020 2023    try:.        #
-000198e0: 2051 7420 352e 3134 2b0a 2020 2020 2020   Qt 5.14+.      
-000198f0: 2020 7265 7475 726e 2077 6964 6765 742e    return widget.
-00019900: 7363 7265 656e 2829 2e67 656f 6d65 7472  screen().geometr
-00019910: 7928 290a 2020 2020 6578 6365 7074 2041  y().    except A
-00019920: 7474 7269 6275 7465 4572 726f 723a 0a20  ttributeError:. 
-00019930: 2020 2020 2020 2023 2054 6f70 2063 656e         # Top cen
-00019940: 7465 7220 6f66 2074 6865 2077 6964 6765  ter of the widge
-00019950: 740a 2020 2020 2020 2020 7363 7265 656e  t.        screen
-00019960: 203d 2051 4775 6941 7070 6c69 6361 7469   = QGuiApplicati
-00019970: 6f6e 2e73 6372 6565 6e41 7428 0a20 2020  on.screenAt(.   
-00019980: 2020 2020 2020 2020 2077 6964 6765 742e           widget.
-00019990: 6d61 7054 6f47 6c6f 6261 6c28 5150 6f69  mapToGlobal(QPoi
-000199a0: 6e74 2877 6964 6765 742e 7769 6474 6828  nt(widget.width(
-000199b0: 2920 2f2f 2032 2c20 3029 2929 0a20 2020  ) // 2, 0))).   
-000199c0: 2020 2020 2069 6620 7363 7265 656e 2069       if screen i
-000199d0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-000199e0: 2020 2020 7363 7265 656e 203d 2051 4775      screen = QGu
-000199f0: 6941 7070 6c69 6361 7469 6f6e 2e70 7269  iApplication.pri
-00019a00: 6d61 7279 5363 7265 656e 2829 0a20 2020  maryScreen().   
-00019a10: 2020 2020 2067 656f 6d65 7472 7920 3d20       geometry = 
-00019a20: 7363 7265 656e 2e67 656f 6d65 7472 7928  screen.geometry(
-00019a30: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00019a40: 6e20 6765 6f6d 6574 7279 0a0a 0a64 6566  n geometry...def
-00019a50: 205f 6d65 7468 7061 7274 6961 6c28 6d65   _methpartial(me
-00019a60: 7468 2c20 2a2a 6b77 6172 6773 293a 0a20  th, **kwargs):. 
-00019a70: 2020 2022 2222 5573 6520 5765 616b 4d65     """Use WeakMe
-00019a80: 7468 6f64 2074 6f20 6372 6561 7465 2061  thod to create a
-00019a90: 2070 6172 7469 616c 206d 6574 686f 642e   partial method.
-00019aa0: 2222 220a 2020 2020 6d65 7468 203d 2077  """.    meth = w
-00019ab0: 6561 6b72 6566 2e57 6561 6b4d 6574 686f  eakref.WeakMetho
-00019ac0: 6428 6d65 7468 290a 0a20 2020 2064 6566  d(meth)..    def
-00019ad0: 2063 616c 6c28 2a61 7267 735f 2c20 2a2a   call(*args_, **
-00019ae0: 6b77 6172 6773 5f29 3a0a 2020 2020 2020  kwargs_):.      
-00019af0: 2020 6d65 7468 5f20 3d20 6d65 7468 2829    meth_ = meth()
-00019b00: 0a20 2020 2020 2020 2069 6620 6d65 7468  .        if meth
-00019b10: 5f20 6973 206e 6f74 204e 6f6e 653a 0a20  _ is not None:. 
-00019b20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00019b30: 6e20 6d65 7468 5f28 2a61 7267 735f 2c20  n meth_(*args_, 
-00019b40: 2a2a 6b77 6172 6773 2c20 2a2a 6b77 6172  **kwargs, **kwar
-00019b50: 6773 5f29 0a0a 2020 2020 7265 7475 726e  gs_)..    return
-00019b60: 2063 616c 6c0a 0a0a 6465 6620 5f64 6973   call...def _dis
-00019b70: 636f 6e6e 6563 7428 7369 672c 202a 2c20  connect(sig, *, 
-00019b80: 616c 6c6f 775f 6572 726f 723d 4661 6c73  allow_error=Fals
-00019b90: 6529 3a0a 2020 2020 7472 793a 0a20 2020  e):.    try:.   
-00019ba0: 2020 2020 2073 6967 2e64 6973 636f 6e6e       sig.disconn
-00019bb0: 6563 7428 290a 2020 2020 6578 6365 7074  ect().    except
-00019bc0: 2028 5479 7065 4572 726f 722c 2052 756e   (TypeError, Run
-00019bd0: 7469 6d65 4572 726f 7229 3a20 2023 2069  timeError):  # i
-00019be0: 6620 7468 6572 6520 6172 6520 6e6f 2063  f there are no c
-00019bf0: 6f6e 6e65 6374 696f 6e73 2c20 6967 6e6f  onnections, igno
-00019c00: 7265 2069 740a 2020 2020 2020 2020 6966  re it.        if
-00019c10: 206e 6f74 2061 6c6c 6f77 5f65 7272 6f72   not allow_error
-00019c20: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00019c30: 6973 650a 0a0a 636c 6173 7320 4d4e 4551  ise...class MNEQ
-00019c40: 7442 726f 7773 6572 2842 726f 7773 6572  tBrowser(Browser
-00019c50: 4261 7365 2c20 514d 6169 6e57 696e 646f  Base, QMainWindo
-00019c60: 772c 206d 6574 6163 6c61 7373 3d5f 5047  w, metaclass=_PG
-00019c70: 4d65 7461 436c 6173 7329 3a0a 2020 2020  MetaClass):.    
-00019c80: 2222 2241 2050 7951 7447 7261 7068 2d62  """A PyQtGraph-b
-00019c90: 6163 6b65 6e64 2066 6f72 2032 4420 6461  ackend for 2D da
-00019ca0: 7461 2062 726f 7773 696e 672e 2222 220a  ta browsing.""".
-00019cb0: 0a20 2020 2067 6f74 436c 6f73 6564 203d  .    gotClosed =
-00019cc0: 2053 6967 6e61 6c28 290a 0a20 2020 2040   Signal()..    @
-00019cd0: 5f73 6166 655f 7370 6c61 7368 0a20 2020  _safe_splash.   
-00019ce0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00019cf0: 6c66 2c20 2a2a 6b77 6172 6773 293a 0a20  lf, **kwargs):. 
-00019d00: 2020 2020 2020 2073 656c 662e 6261 636b         self.back
-00019d10: 656e 645f 6e61 6d65 203d 2027 7079 7174  end_name = 'pyqt
-00019d20: 6772 6170 6827 0a20 2020 2020 2020 2073  graph'.        s
-00019d30: 656c 662e 5f63 6c6f 7365 6420 3d20 4661  elf._closed = Fa
-00019d40: 6c73 650a 0a20 2020 2020 2020 2042 726f  lse..        Bro
-00019d50: 7773 6572 4261 7365 2e5f 5f69 6e69 745f  wserBase.__init_
-00019d60: 5f28 7365 6c66 2c20 2a2a 6b77 6172 6773  _(self, **kwargs
-00019d70: 290a 2020 2020 2020 2020 514d 6169 6e57  ).        QMainW
-00019d80: 696e 646f 772e 5f5f 696e 6974 5f5f 2873  indow.__init__(s
-00019d90: 656c 6629 0a0a 2020 2020 2020 2020 2320  elf)..        # 
-00019da0: 4164 6420 746f 206c 6973 7420 746f 206b  Add to list to k
-00019db0: 6565 7020 6120 7265 6665 7265 6e63 6520  eep a reference 
-00019dc0: 616e 6420 6176 6f69 6420 7072 656d 6174  and avoid premat
-00019dd0: 7572 650a 2020 2020 2020 2020 2320 6761  ure.        # ga
-00019de0: 7262 6167 652d 636f 6c6c 6563 7469 6f6e  rbage-collection
-00019df0: 2e0a 2020 2020 2020 2020 5f62 726f 7773  ..        _brows
-00019e00: 6572 5f69 6e73 7461 6e63 6573 2e61 7070  er_instances.app
-00019e10: 656e 6428 7365 6c66 290a 0a20 2020 2020  end(self)..     
-00019e20: 2020 2023 2053 6574 2074 6865 2062 726f     # Set the bro
-00019e30: 7773 6572 2073 7479 6c65 0a20 2020 2020  wser style.     
-00019e40: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00019e50: 2020 2020 6672 6f6d 206d 6e65 2e76 697a      from mne.viz
-00019e60: 2e62 6163 6b65 6e64 732e 5f75 7469 6c73  .backends._utils
-00019e70: 2069 6d70 6f72 7420 5f71 745f 6765 745f   import _qt_get_
-00019e80: 7374 796c 6573 6865 6574 0a20 2020 2020  stylesheet.     
-00019e90: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00019ea0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-00019eb0: 2073 7479 6c65 7368 6565 7420 3d20 4e6f   stylesheet = No
-00019ec0: 6e65 0a20 2020 2020 2020 2065 6c73 653a  ne.        else:
-00019ed0: 0a20 2020 2020 2020 2020 2020 2073 7479  .            sty
-00019ee0: 6c65 7368 6565 7420 3d20 5f71 745f 6765  lesheet = _qt_ge
-00019ef0: 745f 7374 796c 6573 6865 6574 2867 6574  t_stylesheet(get
-00019f00: 6174 7472 2873 656c 662e 6d6e 652c 2027  attr(self.mne, '
-00019f10: 7468 656d 6527 2c20 2761 7574 6f27 2929  theme', 'auto'))
-00019f20: 0a20 2020 2020 2020 2069 6620 7374 796c  .        if styl
-00019f30: 6573 6865 6574 2069 7320 6e6f 7420 4e6f  esheet is not No
-00019f40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00019f50: 7365 6c66 2e73 6574 5374 796c 6553 6865  self.setStyleShe
-00019f60: 6574 2873 7479 6c65 7368 6565 7429 0a0a  et(stylesheet)..
-00019f70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00019f80: 6d6e 652e 7769 6e64 6f77 5f74 6974 6c65  mne.window_title
-00019f90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00019fa0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00019fb0: 6574 5769 6e64 6f77 5469 746c 6528 7365  etWindowTitle(se
-00019fc0: 6c66 2e6d 6e65 2e77 696e 646f 775f 7469  lf.mne.window_ti
-00019fd0: 746c 6529 0a20 2020 2020 2020 2051 4170  tle).        QAp
-00019fe0: 706c 6963 6174 696f 6e2e 7072 6f63 6573  plication.proces
-00019ff0: 7345 7665 6e74 7328 2920 2023 206e 6565  sEvents()  # nee
-0001a000: 6473 2074 6f20 6861 7070 656e 2066 6f72  ds to happen for
-0001a010: 2074 6865 2074 6865 6d65 2074 6f20 6265   the theme to be
-0001a020: 2073 6574 0a0a 2020 2020 2020 2020 2320   set..        # 
-0001a030: 4869 4450 4920 7374 7566 660a 2020 2020  HiDPI stuff.    
-0001a040: 2020 2020 7365 6c66 2e5f 7069 7865 6c5f      self._pixel_
-0001a050: 7261 7469 6f20 3d20 7365 6c66 2e64 6576  ratio = self.dev
-0001a060: 6963 6550 6978 656c 5261 7469 6f28 290a  icePixelRatio().
-0001a070: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0001a080: 6562 7567 2866 2744 6573 6b74 6f70 2070  ebug(f'Desktop p
-0001a090: 6978 656c 2072 6174 696f 3a20 7b73 656c  ixel ratio: {sel
-0001a0a0: 662e 5f70 6978 656c 5f72 6174 696f 3a30  f._pixel_ratio:0
-0001a0b0: 2e33 667d 2729 0a20 2020 2020 2020 2073  .3f}').        s
-0001a0c0: 656c 662e 6d6e 652e 6d6b 5065 6e20 3d20  elf.mne.mkPen = 
-0001a0d0: 5f6d 6574 6870 6172 7469 616c 2873 656c  _methpartial(sel
-0001a0e0: 662e 5f68 6964 7069 5f6d 6b50 656e 290a  f._hidpi_mkPen).
-0001a0f0: 0a20 2020 2020 2020 2062 6763 6f6c 6f72  .        bgcolor
-0001a100: 203d 2073 656c 662e 7061 6c65 7474 6528   = self.palette(
-0001a110: 292e 636f 6c6f 7228 7365 6c66 2e62 6163  ).color(self.bac
-0001a120: 6b67 726f 756e 6452 6f6c 6528 2929 2e67  kgroundRole()).g
-0001a130: 6574 5267 6246 2829 5b3a 335d 0a20 2020  etRgbF()[:3].   
-0001a140: 2020 2020 2073 656c 662e 6d6e 652e 6461       self.mne.da
-0001a150: 726b 203d 2063 7370 6163 655f 636f 6e76  rk = cspace_conv
-0001a160: 6572 7428 6267 636f 6c6f 722c 2027 7352  ert(bgcolor, 'sR
-0001a170: 4742 3127 2c20 2743 4945 4c61 6227 295b  GB1', 'CIELab')[
-0001a180: 305d 203c 2035 300a 0a20 2020 2020 2020  0] < 50..       
-0001a190: 2023 2075 7064 6174 6520 6963 6f6e 2074   # update icon t
-0001a1a0: 6865 6d65 0a20 2020 2020 2020 205f 7174  heme.        _qt
-0001a1b0: 5f69 6e69 745f 6963 6f6e 7328 290a 2020  _init_icons().  
-0001a1c0: 2020 2020 2020 6966 2073 656c 662e 6d6e        if self.mn
-0001a1d0: 652e 6461 726b 3a0a 2020 2020 2020 2020  e.dark:.        
-0001a1e0: 2020 2020 5149 636f 6e2e 7365 7454 6865      QIcon.setThe
-0001a1f0: 6d65 4e61 6d65 2827 6461 726b 2729 0a20  meName('dark'). 
-0001a200: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001a210: 2020 2020 2020 2020 2051 4963 6f6e 2e73           QIcon.s
-0001a220: 6574 5468 656d 654e 616d 6528 276c 6967  etThemeName('lig
-0001a230: 6874 2729 0a0a 2020 2020 2020 2020 2320  ht')..        # 
-0001a240: 636f 6e74 726f 6c20 7261 6973 696e 6720  control raising 
-0001a250: 7769 7468 205f 7174 5f72 6169 7365 5f77  with _qt_raise_w
-0001a260: 696e 646f 770a 2020 2020 2020 2020 7365  indow.        se
-0001a270: 6c66 2e73 6574 4174 7472 6962 7574 6528  lf.setAttribute(
-0001a280: 5174 2e57 415f 5368 6f77 5769 7468 6f75  Qt.WA_ShowWithou
-0001a290: 7441 6374 6976 6174 696e 672c 2054 7275  tActivating, Tru
-0001a2a0: 6529 0a0a 2020 2020 2020 2020 2320 496e  e)..        # In
-0001a2b0: 6974 6961 6c69 7a65 2061 7474 7269 6275  itialize attribu
-0001a2c0: 7465 7320 7768 6963 6820 6172 6520 6f6e  tes which are on
-0001a2d0: 6c79 2075 7365 6420 6279 2070 7971 7467  ly used by pyqtg
-0001a2e0: 7261 7068 2c20 6e6f 7420 6279 0a20 2020  raph, not by.   
-0001a2f0: 2020 2020 2023 206d 6174 706c 6f74 6c69       # matplotli
-0001a300: 6220 616e 6420 6164 6420 7468 656d 2074  b and add them t
-0001a310: 6f20 4d4e 4542 726f 7773 6550 6172 616d  o MNEBrowseParam
-0001a320: 732e 0a0a 2020 2020 2020 2020 2320 4578  s...        # Ex
-0001a330: 6163 746c 7920 6f6e 6520 4d65 7373 6167  actly one Messag
-0001a340: 6542 6f78 2066 6f72 206d 6573 7361 6765  eBox for message
-0001a350: 7320 746f 2066 6163 696c 6974 6174 6520  s to facilitate 
-0001a360: 7465 7374 696e 672f 6465 6275 6767 696e  testing/debuggin
-0001a370: 670a 2020 2020 2020 2020 7365 6c66 2e6d  g.        self.m
-0001a380: 7367 5f62 6f78 203d 2051 4d65 7373 6167  sg_box = QMessag
-0001a390: 6542 6f78 2873 656c 6629 0a20 2020 2020  eBox(self).     
-0001a3a0: 2020 2023 204d 6573 7361 6765 426f 7820     # MessageBox 
-0001a3b0: 6d6f 6461 6c69 7479 206e 6565 6473 2074  modality needs t
-0001a3c0: 6f20 6265 2061 6461 7074 6564 2066 6f72  o be adapted for
-0001a3d0: 2074 6573 7473 0a20 2020 2020 2020 2023   tests.        #
-0001a3e0: 2028 6f74 6865 7277 6973 6520 7465 7374   (otherwise test
-0001a3f0: 2065 7865 6375 7469 6f6e 2062 6c6f 636b   execution block
-0001a400: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-0001a410: 7465 7374 5f6d 6f64 6520 3d20 4661 6c73  test_mode = Fals
-0001a420: 650a 2020 2020 2020 2020 2320 4120 5365  e.        # A Se
-0001a430: 7474 696e 6773 2d44 6961 6c6f 670a 2020  ttings-Dialog.  
-0001a440: 2020 2020 2020 7365 6c66 2e6d 6e65 2e66        self.mne.f
-0001a450: 6967 5f73 6574 7469 6e67 7320 3d20 4e6f  ig_settings = No
-0001a460: 6e65 0a20 2020 2020 2020 2023 2053 746f  ne.        # Sto
-0001a470: 7265 7320 6465 6369 6d61 7465 6420 6461  res decimated da
-0001a480: 7461 0a20 2020 2020 2020 2073 656c 662e  ta.        self.
-0001a490: 6d6e 652e 6465 6369 6d5f 6461 7461 203d  mne.decim_data =
-0001a4a0: 204e 6f6e 650a 2020 2020 2020 2020 2320   None.        # 
-0001a4b0: 5374 6f72 6573 2079 706f 7320 666f 7220  Stores ypos for 
-0001a4c0: 7365 6c65 6374 696f 6e2d 6d6f 6465 0a20  selection-mode. 
-0001a4d0: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-0001a4e0: 7365 6c65 6374 696f 6e5f 7970 6f73 5f64  selection_ypos_d
-0001a4f0: 6963 7420 3d20 6469 6374 2829 0a20 2020  ict = dict().   
-0001a500: 2020 2020 2023 2050 6172 616d 6574 6572       # Parameter
-0001a510: 7320 666f 7220 7072 6563 6f6d 7075 7469  s for precomputi
-0001a520: 6e67 0a20 2020 2020 2020 2073 656c 662e  ng.        self.
-0001a530: 6d6e 652e 656e 6162 6c65 5f70 7265 636f  mne.enable_preco
-0001a540: 6d70 7574 6520 3d20 4661 6c73 650a 2020  mpute = False.  
-0001a550: 2020 2020 2020 7365 6c66 2e6d 6e65 2e64        self.mne.d
-0001a560: 6174 615f 7072 6563 6f6d 7075 7465 6420  ata_precomputed 
-0001a570: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-0001a580: 7365 6c66 2e5f 7265 7275 6e5f 6c6f 6164  self._rerun_load
-0001a590: 5f74 6872 6561 6420 3d20 4661 6c73 650a  _thread = False.
-0001a5a0: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
-0001a5b0: 2e7a 7363 6f72 655f 7267 6261 203d 204e  .zscore_rgba = N
-0001a5c0: 6f6e 650a 2020 2020 2020 2020 2320 436f  one.        # Co
-0001a5d0: 6e74 6169 6e65 7220 666f 7220 7472 6163  ntainer for trac
-0001a5e0: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
-0001a5f0: 6d6e 652e 7472 6163 6573 203d 206c 6973  mne.traces = lis
-0001a600: 7428 290a 2020 2020 2020 2020 2320 5363  t().        # Sc
-0001a610: 616c 652d 4661 6374 6f72 0a20 2020 2020  ale-Factor.     
-0001a620: 2020 2073 656c 662e 6d6e 652e 7363 616c     self.mne.scal
-0001a630: 655f 6661 6374 6f72 203d 2031 0a20 2020  e_factor = 1.   
-0001a640: 2020 2020 2023 2053 746f 7265 7320 6368       # Stores ch
-0001a650: 616e 6e65 6c2d 7479 7065 7320 666f 7220  annel-types for 
-0001a660: 6275 7474 6572 666c 792d 6d6f 6465 0a20  butterfly-mode. 
-0001a670: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-0001a680: 6275 7474 6572 666c 795f 7479 7065 5f6f  butterfly_type_o
-0001a690: 7264 6572 203d 205b 7470 2066 6f72 2074  rder = [tp for t
-0001a6a0: 7020 696e 0a20 2020 2020 2020 2020 2020  p in.           
+000192c0: 302c 2064 6174 612e 7368 6170 655b 2d31  0, data.shape[-1
+000192d0: 5d2c 2070 6963 6b73 2c20 7365 6c66 290a  ], picks, self).
+000192e0: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
+000192f0: 2e72 656d 6f76 655f 6463 203d 2073 7461  .remove_dc = sta
+00019300: 7368 6564 5f72 656d 6f76 655f 6463 0a0a  shed_remove_dc..
+00019310: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
+00019320: 2e67 6c6f 6261 6c5f 6461 7461 203d 2064  .global_data = d
+00019330: 6174 610a 2020 2020 2020 2020 7365 6c66  ata.        self
+00019340: 2e6d 6e65 2e67 6c6f 6261 6c5f 7469 6d65  .mne.global_time
+00019350: 7320 3d20 7469 6d65 730a 0a20 2020 2020  s = times..     
+00019360: 2020 2023 2043 616c 6375 6c61 7465 205a     # Calculate Z
+00019370: 2d53 636f 7265 730a 2020 2020 2020 2020  -Scores.        
+00019380: 7365 6c66 2e70 726f 6365 7373 5465 7874  self.processText
+00019390: 2e65 6d69 7428 2743 616c 6375 6c61 7469  .emit('Calculati
+000193a0: 6e67 205a 2d53 636f 7265 732e 2e2e 2729  ng Z-Scores...')
+000193b0: 0a20 2020 2020 2020 2062 726f 7773 6572  .        browser
+000193c0: 2e5f 6765 745f 7a73 636f 7265 2864 6174  ._get_zscore(dat
+000193d0: 6129 0a20 2020 2020 2020 2064 656c 2062  a).        del b
+000193e0: 726f 7773 6572 0a0a 2020 2020 2020 2020  rowser..        
+000193f0: 7365 6c66 2e6c 6f61 6469 6e67 4669 6e69  self.loadingFini
+00019400: 7368 6564 2e65 6d69 7428 290a 0a20 2020  shed.emit()..   
+00019410: 2064 6566 2063 6c65 616e 2873 656c 6629   def clean(self)
+00019420: 3a20 2023 206e 6f71 613a 2044 3130 320a  :  # noqa: D102.
+00019430: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00019440: 6973 5275 6e6e 696e 6728 293a 0a20 2020  isRunning():.   
+00019450: 2020 2020 2020 2020 2077 6169 745f 7469           wait_ti
+00019460: 6d65 203d 2031 3020 2023 206d 6178 2e20  me = 10  # max. 
+00019470: 7761 6974 696e 6720 7469 6d65 2069 6e20  waiting time in 
+00019480: 7365 636f 6e64 730a 2020 2020 2020 2020  seconds.        
+00019490: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+000194a0: 2757 6169 7469 6e67 2066 6f72 204c 6f61  'Waiting for Loa
+000194b0: 6469 6e67 2d54 6872 6561 6420 746f 2066  ding-Thread to f
+000194c0: 696e 6973 682e 2e2e 2027 0a20 2020 2020  inish... '.     
+000194d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194e0: 2020 2066 2728 6d61 782e 207b 7761 6974     f'(max. {wait
+000194f0: 5f74 696d 657d 2073 6563 2927 290a 2020  _time} sec)').  
+00019500: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
+00019510: 6169 7428 696e 7428 7761 6974 5f74 696d  ait(int(wait_tim
+00019520: 6520 2a20 3165 3329 290a 2020 2020 2020  e * 1e3)).      
+00019530: 2020 5f64 6973 636f 6e6e 6563 7428 7365    _disconnect(se
+00019540: 6c66 2e6c 6f61 6450 726f 6772 6573 7329  lf.loadProgress)
+00019550: 0a20 2020 2020 2020 205f 6469 7363 6f6e  .        _discon
+00019560: 6e65 6374 2873 656c 662e 7072 6f63 6573  nect(self.proces
+00019570: 7354 6578 7429 0a20 2020 2020 2020 205f  sText).        _
+00019580: 6469 7363 6f6e 6e65 6374 2873 656c 662e  disconnect(self.
+00019590: 6c6f 6164 696e 6746 696e 6973 6865 6429  loadingFinished)
+000195a0: 0a20 2020 2020 2020 2064 656c 2073 656c  .        del sel
+000195b0: 662e 6d6e 650a 2020 2020 2020 2020 6465  f.mne.        de
+000195c0: 6c20 7365 6c66 2e77 6561 6b62 726f 7773  l self.weakbrows
+000195d0: 6572 0a0a 0a63 6c61 7373 205f 5047 4d65  er...class _PGMe
+000195e0: 7461 436c 6173 7328 7479 7065 2851 4d61  taClass(type(QMa
+000195f0: 696e 5769 6e64 6f77 292c 2074 7970 6528  inWindow), type(
+00019600: 4272 6f77 7365 7242 6173 6529 293a 0a20  BrowserBase)):. 
+00019610: 2020 2022 2222 436c 6173 7320 6973 206e     """Class is n
+00019620: 6563 6573 7361 7279 2074 6f20 7072 6576  ecessary to prev
+00019630: 656e 7420 6120 6d65 7461 636c 6173 7320  ent a metaclass 
+00019640: 636f 6e66 6c69 6374 2e0a 0a20 2020 2054  conflict...    T
+00019650: 6865 2063 6f6e 666c 6963 7420 6172 6973  he conflict aris
+00019660: 6573 2064 7565 2074 6f20 7468 6520 6469  es due to the di
+00019670: 6666 6572 656e 7420 7479 7065 7320 6f66  fferent types of
+00019680: 2051 4d61 696e 5769 6e64 6f77 2061 6e64   QMainWindow and
+00019690: 0a20 2020 2042 726f 7773 6572 4261 7365  .    BrowserBase
+000196a0: 2e0a 2020 2020 2222 220a 0a20 2020 2070  ..    """..    p
+000196b0: 6173 730a 0a0a 2320 5468 6f73 6520 6172  ass...# Those ar
+000196c0: 6520 7468 6520 7365 7474 696e 6773 2077  e the settings w
+000196d0: 6869 6368 2061 7265 2073 746f 7265 6420  hich are stored 
+000196e0: 6f6e 2065 6163 6820 6465 7669 6365 0a23  on each device.#
+000196f0: 2064 6570 656e 6469 6e67 206f 6e20 6974   depending on it
+00019700: 7320 6f70 6572 6174 696e 6720 7379 7374  s operating syst
+00019710: 656d 2077 6974 6820 5153 6574 7469 6e67  em with QSetting
+00019720: 732e 0a0a 7173 6574 7469 6e67 735f 7061  s...qsettings_pa
+00019730: 7261 6d73 203d 207b 0a20 2020 2023 2041  rams = {.    # A
+00019740: 6e74 6961 6c69 6173 696e 6720 2877 6f72  ntialiasing (wor
+00019750: 6b73 2077 6974 682f 7769 7468 6f75 7420  ks with/without 
+00019760: 4f70 656e 474c 2c20 696e 7465 6765 7220  OpenGL, integer 
+00019770: 6265 6361 7573 6520 5153 6574 7469 6e67  because QSetting
+00019780: 730a 2020 2020 2320 6361 6e27 7420 6861  s.    # can't ha
+00019790: 6e64 6c65 2062 6f6f 6c65 616e 7329 0a20  ndle booleans). 
+000197a0: 2020 2027 616e 7469 616c 6961 7369 6e67     'antialiasing
+000197b0: 273a 2046 616c 7365 2c0a 2020 2020 2320  ': False,.    # 
+000197c0: 5374 6570 7320 7065 7220 7669 6577 2028  Steps per view (
+000197d0: 7265 6c61 7469 7665 2074 6f20 7469 6d65  relative to time
+000197e0: 290a 2020 2020 2773 6372 6f6c 6c5f 7365  ).    'scroll_se
+000197f0: 6e73 6974 6976 6974 7927 3a20 3130 302c  nsitivity': 100,
+00019800: 0a20 2020 2023 2044 6f77 6e73 616d 706c  .    # Downsampl
+00019810: 696e 672d 4661 6374 6f72 2028 6f72 2027  ing-Factor (or '
+00019820: 6175 746f 272c 2073 6565 2053 6574 7469  auto', see Setti
+00019830: 6e67 7344 6961 6c6f 6720 666f 7220 6465  ngsDialog for de
+00019840: 7461 696c 7329 0a20 2020 2027 646f 776e  tails).    'down
+00019850: 7361 6d70 6c69 6e67 273a 2031 2c0a 2020  sampling': 1,.  
+00019860: 2020 2320 446f 776e 7361 6d70 6c69 6e67    # Downsampling
+00019870: 2d4d 6574 686f 6420 2873 6574 2053 6574  -Method (set Set
+00019880: 7469 6e67 7344 6961 6c6f 6720 666f 7220  tingsDialog for 
+00019890: 6465 7461 696c 7329 0a20 2020 2027 6473  details).    'ds
+000198a0: 5f6d 6574 686f 6427 3a20 2770 6561 6b27  _method': 'peak'
+000198b0: 0a7d 0a0a 0a64 6566 205f 7363 7265 656e  .}...def _screen
+000198c0: 5f67 656f 6d65 7472 7928 7769 6467 6574  _geometry(widget
+000198d0: 293a 0a20 2020 2074 7279 3a0a 2020 2020  ):.    try:.    
+000198e0: 2020 2020 2320 5174 2035 2e31 342b 0a20      # Qt 5.14+. 
+000198f0: 2020 2020 2020 2072 6574 7572 6e20 7769         return wi
+00019900: 6467 6574 2e73 6372 6565 6e28 292e 6765  dget.screen().ge
+00019910: 6f6d 6574 7279 2829 0a20 2020 2065 7863  ometry().    exc
+00019920: 6570 7420 4174 7472 6962 7574 6545 7272  ept AttributeErr
+00019930: 6f72 3a0a 2020 2020 2020 2020 2320 546f  or:.        # To
+00019940: 7020 6365 6e74 6572 206f 6620 7468 6520  p center of the 
+00019950: 7769 6467 6574 0a20 2020 2020 2020 2073  widget.        s
+00019960: 6372 6565 6e20 3d20 5147 7569 4170 706c  creen = QGuiAppl
+00019970: 6963 6174 696f 6e2e 7363 7265 656e 4174  ication.screenAt
+00019980: 280a 2020 2020 2020 2020 2020 2020 7769  (.            wi
+00019990: 6467 6574 2e6d 6170 546f 476c 6f62 616c  dget.mapToGlobal
+000199a0: 2851 506f 696e 7428 7769 6467 6574 2e77  (QPoint(widget.w
+000199b0: 6964 7468 2829 202f 2f20 322c 2030 2929  idth() // 2, 0))
+000199c0: 290a 2020 2020 2020 2020 6966 2073 6372  ).        if scr
+000199d0: 6565 6e20 6973 204e 6f6e 653a 0a20 2020  een is None:.   
+000199e0: 2020 2020 2020 2020 2073 6372 6565 6e20           screen 
+000199f0: 3d20 5147 7569 4170 706c 6963 6174 696f  = QGuiApplicatio
+00019a00: 6e2e 7072 696d 6172 7953 6372 6565 6e28  n.primaryScreen(
+00019a10: 290a 2020 2020 2020 2020 6765 6f6d 6574  ).        geomet
+00019a20: 7279 203d 2073 6372 6565 6e2e 6765 6f6d  ry = screen.geom
+00019a30: 6574 7279 2829 0a0a 2020 2020 2020 2020  etry()..        
+00019a40: 7265 7475 726e 2067 656f 6d65 7472 790a  return geometry.
+00019a50: 0a0a 6465 6620 5f6d 6574 6870 6172 7469  ..def _methparti
+00019a60: 616c 286d 6574 682c 202a 2a6b 7761 7267  al(meth, **kwarg
+00019a70: 7329 3a0a 2020 2020 2222 2255 7365 2057  s):.    """Use W
+00019a80: 6561 6b4d 6574 686f 6420 746f 2063 7265  eakMethod to cre
+00019a90: 6174 6520 6120 7061 7274 6961 6c20 6d65  ate a partial me
+00019aa0: 7468 6f64 2e22 2222 0a20 2020 206d 6574  thod.""".    met
+00019ab0: 6820 3d20 7765 616b 7265 662e 5765 616b  h = weakref.Weak
+00019ac0: 4d65 7468 6f64 286d 6574 6829 0a0a 2020  Method(meth)..  
+00019ad0: 2020 6465 6620 6361 6c6c 282a 6172 6773    def call(*args
+00019ae0: 5f2c 202a 2a6b 7761 7267 735f 293a 0a20  _, **kwargs_):. 
+00019af0: 2020 2020 2020 206d 6574 685f 203d 206d         meth_ = m
+00019b00: 6574 6828 290a 2020 2020 2020 2020 6966  eth().        if
+00019b10: 206d 6574 685f 2069 7320 6e6f 7420 4e6f   meth_ is not No
+00019b20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00019b30: 7265 7475 726e 206d 6574 685f 282a 6172  return meth_(*ar
+00019b40: 6773 5f2c 202a 2a6b 7761 7267 732c 202a  gs_, **kwargs, *
+00019b50: 2a6b 7761 7267 735f 290a 0a20 2020 2072  *kwargs_)..    r
+00019b60: 6574 7572 6e20 6361 6c6c 0a0a 0a64 6566  eturn call...def
+00019b70: 205f 6469 7363 6f6e 6e65 6374 2873 6967   _disconnect(sig
+00019b80: 2c20 2a2c 2061 6c6c 6f77 5f65 7272 6f72  , *, allow_error
+00019b90: 3d46 616c 7365 293a 0a20 2020 2074 7279  =False):.    try
+00019ba0: 3a0a 2020 2020 2020 2020 7369 672e 6469  :.        sig.di
+00019bb0: 7363 6f6e 6e65 6374 2829 0a20 2020 2065  sconnect().    e
+00019bc0: 7863 6570 7420 2854 7970 6545 7272 6f72  xcept (TypeError
+00019bd0: 2c20 5275 6e74 696d 6545 7272 6f72 293a  , RuntimeError):
+00019be0: 2020 2320 6966 2074 6865 7265 2061 7265    # if there are
+00019bf0: 206e 6f20 636f 6e6e 6563 7469 6f6e 732c   no connections,
+00019c00: 2069 676e 6f72 6520 6974 0a20 2020 2020   ignore it.     
+00019c10: 2020 2069 6620 6e6f 7420 616c 6c6f 775f     if not allow_
+00019c20: 6572 726f 723a 0a20 2020 2020 2020 2020  error:.         
+00019c30: 2020 2072 6169 7365 0a0a 0a63 6c61 7373     raise...class
+00019c40: 204d 4e45 5174 4272 6f77 7365 7228 4272   MNEQtBrowser(Br
+00019c50: 6f77 7365 7242 6173 652c 2051 4d61 696e  owserBase, QMain
+00019c60: 5769 6e64 6f77 2c20 6d65 7461 636c 6173  Window, metaclas
+00019c70: 733d 5f50 474d 6574 6143 6c61 7373 293a  s=_PGMetaClass):
+00019c80: 0a20 2020 2022 2222 4120 5079 5174 4772  .    """A PyQtGr
+00019c90: 6170 682d 6261 636b 656e 6420 666f 7220  aph-backend for 
+00019ca0: 3244 2064 6174 6120 6272 6f77 7369 6e67  2D data browsing
+00019cb0: 2e22 2222 0a0a 2020 2020 676f 7443 6c6f  ."""..    gotClo
+00019cc0: 7365 6420 3d20 5369 676e 616c 2829 0a0a  sed = Signal()..
+00019cd0: 2020 2020 405f 7361 6665 5f73 706c 6173      @_safe_splas
+00019ce0: 680a 2020 2020 6465 6620 5f5f 696e 6974  h.    def __init
+00019cf0: 5f5f 2873 656c 662c 202a 2a6b 7761 7267  __(self, **kwarg
+00019d00: 7329 3a0a 2020 2020 2020 2020 7365 6c66  s):.        self
+00019d10: 2e62 6163 6b65 6e64 5f6e 616d 6520 3d20  .backend_name = 
+00019d20: 2770 7971 7467 7261 7068 270a 2020 2020  'pyqtgraph'.    
+00019d30: 2020 2020 7365 6c66 2e5f 636c 6f73 6564      self._closed
+00019d40: 203d 2046 616c 7365 0a0a 2020 2020 2020   = False..      
+00019d50: 2020 4272 6f77 7365 7242 6173 652e 5f5f    BrowserBase.__
+00019d60: 696e 6974 5f5f 2873 656c 662c 202a 2a6b  init__(self, **k
+00019d70: 7761 7267 7329 0a20 2020 2020 2020 2051  wargs).        Q
+00019d80: 4d61 696e 5769 6e64 6f77 2e5f 5f69 6e69  MainWindow.__ini
+00019d90: 745f 5f28 7365 6c66 290a 0a20 2020 2020  t__(self)..     
+00019da0: 2020 2023 2041 6464 2074 6f20 6c69 7374     # Add to list
+00019db0: 2074 6f20 6b65 6570 2061 2072 6566 6572   to keep a refer
+00019dc0: 656e 6365 2061 6e64 2061 766f 6964 2070  ence and avoid p
+00019dd0: 7265 6d61 7475 7265 0a20 2020 2020 2020  remature.       
+00019de0: 2023 2067 6172 6261 6765 2d63 6f6c 6c65   # garbage-colle
+00019df0: 6374 696f 6e2e 0a20 2020 2020 2020 205f  ction..        _
+00019e00: 6272 6f77 7365 725f 696e 7374 616e 6365  browser_instance
+00019e10: 732e 6170 7065 6e64 2873 656c 6629 0a0a  s.append(self)..
+00019e20: 2020 2020 2020 2020 2320 5365 7420 7468          # Set th
+00019e30: 6520 6272 6f77 7365 7220 7374 796c 650a  e browser style.
+00019e40: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00019e50: 2020 2020 2020 2020 2066 726f 6d20 6d6e           from mn
+00019e60: 652e 7669 7a2e 6261 636b 656e 6473 2e5f  e.viz.backends._
+00019e70: 7574 696c 7320 696d 706f 7274 205f 7174  utils import _qt
+00019e80: 5f67 6574 5f73 7479 6c65 7368 6565 740a  _get_stylesheet.
+00019e90: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00019ea0: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
+00019eb0: 2020 2020 2020 7374 796c 6573 6865 6574        stylesheet
+00019ec0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00019ed0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00019ee0: 2020 7374 796c 6573 6865 6574 203d 205f    stylesheet = _
+00019ef0: 7174 5f67 6574 5f73 7479 6c65 7368 6565  qt_get_styleshee
+00019f00: 7428 6765 7461 7474 7228 7365 6c66 2e6d  t(getattr(self.m
+00019f10: 6e65 2c20 2774 6865 6d65 272c 2027 6175  ne, 'theme', 'au
+00019f20: 746f 2729 290a 2020 2020 2020 2020 6966  to')).        if
+00019f30: 2073 7479 6c65 7368 6565 7420 6973 206e   stylesheet is n
+00019f40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00019f50: 2020 2020 2073 656c 662e 7365 7453 7479       self.setSty
+00019f60: 6c65 5368 6565 7428 7374 796c 6573 6865  leSheet(styleshe
+00019f70: 6574 290a 0a20 2020 2020 2020 2069 6620  et)..        if 
+00019f80: 7365 6c66 2e6d 6e65 2e77 696e 646f 775f  self.mne.window_
+00019f90: 7469 746c 6520 6973 206e 6f74 204e 6f6e  title is not Non
+00019fa0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00019fb0: 656c 662e 7365 7457 696e 646f 7754 6974  elf.setWindowTit
+00019fc0: 6c65 2873 656c 662e 6d6e 652e 7769 6e64  le(self.mne.wind
+00019fd0: 6f77 5f74 6974 6c65 290a 2020 2020 2020  ow_title).      
+00019fe0: 2020 5141 7070 6c69 6361 7469 6f6e 2e70    QApplication.p
+00019ff0: 726f 6365 7373 4576 656e 7473 2829 2020  rocessEvents()  
+0001a000: 2320 6e65 6564 7320 746f 2068 6170 7065  # needs to happe
+0001a010: 6e20 666f 7220 7468 6520 7468 656d 6520  n for the theme 
+0001a020: 746f 2062 6520 7365 740a 0a20 2020 2020  to be set..     
+0001a030: 2020 2023 2048 6944 5049 2073 7475 6666     # HiDPI stuff
+0001a040: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
+0001a050: 6978 656c 5f72 6174 696f 203d 2073 656c  ixel_ratio = sel
+0001a060: 662e 6465 7669 6365 5069 7865 6c52 6174  f.devicePixelRat
+0001a070: 696f 2829 0a20 2020 2020 2020 206c 6f67  io().        log
+0001a080: 6765 722e 6465 6275 6728 6627 4465 736b  ger.debug(f'Desk
+0001a090: 746f 7020 7069 7865 6c20 7261 7469 6f3a  top pixel ratio:
+0001a0a0: 207b 7365 6c66 2e5f 7069 7865 6c5f 7261   {self._pixel_ra
+0001a0b0: 7469 6f3a 302e 3366 7d27 290a 2020 2020  tio:0.3f}').    
+0001a0c0: 2020 2020 7365 6c66 2e6d 6e65 2e6d 6b50      self.mne.mkP
+0001a0d0: 656e 203d 205f 6d65 7468 7061 7274 6961  en = _methpartia
+0001a0e0: 6c28 7365 6c66 2e5f 6869 6470 695f 6d6b  l(self._hidpi_mk
+0001a0f0: 5065 6e29 0a0a 2020 2020 2020 2020 6267  Pen)..        bg
+0001a100: 636f 6c6f 7220 3d20 7365 6c66 2e70 616c  color = self.pal
+0001a110: 6574 7465 2829 2e63 6f6c 6f72 2873 656c  ette().color(sel
+0001a120: 662e 6261 636b 6772 6f75 6e64 526f 6c65  f.backgroundRole
+0001a130: 2829 292e 6765 7452 6762 4628 295b 3a33  ()).getRgbF()[:3
+0001a140: 5d0a 2020 2020 2020 2020 7365 6c66 2e6d  ].        self.m
+0001a150: 6e65 2e64 6172 6b20 3d20 6373 7061 6365  ne.dark = cspace
+0001a160: 5f63 6f6e 7665 7274 2862 6763 6f6c 6f72  _convert(bgcolor
+0001a170: 2c20 2773 5247 4231 272c 2027 4349 454c  , 'sRGB1', 'CIEL
+0001a180: 6162 2729 5b30 5d20 3c20 3530 0a0a 2020  ab')[0] < 50..  
+0001a190: 2020 2020 2020 2320 7570 6461 7465 2069        # update i
+0001a1a0: 636f 6e20 7468 656d 650a 2020 2020 2020  con theme.      
+0001a1b0: 2020 5f71 745f 696e 6974 5f69 636f 6e73    _qt_init_icons
+0001a1c0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0001a1d0: 6c66 2e6d 6e65 2e64 6172 6b3a 0a20 2020  lf.mne.dark:.   
+0001a1e0: 2020 2020 2020 2020 2051 4963 6f6e 2e73           QIcon.s
+0001a1f0: 6574 5468 656d 654e 616d 6528 2764 6172  etThemeName('dar
+0001a200: 6b27 290a 2020 2020 2020 2020 656c 7365  k').        else
+0001a210: 3a0a 2020 2020 2020 2020 2020 2020 5149  :.            QI
+0001a220: 636f 6e2e 7365 7454 6865 6d65 4e61 6d65  con.setThemeName
+0001a230: 2827 6c69 6768 7427 290a 0a20 2020 2020  ('light')..     
+0001a240: 2020 2023 2063 6f6e 7472 6f6c 2072 6169     # control rai
+0001a250: 7369 6e67 2077 6974 6820 5f71 745f 7261  sing with _qt_ra
+0001a260: 6973 655f 7769 6e64 6f77 0a20 2020 2020  ise_window.     
+0001a270: 2020 2073 656c 662e 7365 7441 7474 7269     self.setAttri
+0001a280: 6275 7465 2851 742e 5741 5f53 686f 7757  bute(Qt.WA_ShowW
+0001a290: 6974 686f 7574 4163 7469 7661 7469 6e67  ithoutActivating
+0001a2a0: 2c20 5472 7565 290a 0a20 2020 2020 2020  , True)..       
+0001a2b0: 2023 2049 6e69 7469 616c 697a 6520 6174   # Initialize at
+0001a2c0: 7472 6962 7574 6573 2077 6869 6368 2061  tributes which a
+0001a2d0: 7265 206f 6e6c 7920 7573 6564 2062 7920  re only used by 
+0001a2e0: 7079 7174 6772 6170 682c 206e 6f74 2062  pyqtgraph, not b
+0001a2f0: 790a 2020 2020 2020 2020 2320 6d61 7470  y.        # matp
+0001a300: 6c6f 746c 6962 2061 6e64 2061 6464 2074  lotlib and add t
+0001a310: 6865 6d20 746f 204d 4e45 4272 6f77 7365  hem to MNEBrowse
+0001a320: 5061 7261 6d73 2e0a 0a20 2020 2020 2020  Params...       
+0001a330: 2023 2045 7861 6374 6c79 206f 6e65 204d   # Exactly one M
+0001a340: 6573 7361 6765 426f 7820 666f 7220 6d65  essageBox for me
+0001a350: 7373 6167 6573 2074 6f20 6661 6369 6c69  ssages to facili
+0001a360: 7461 7465 2074 6573 7469 6e67 2f64 6562  tate testing/deb
+0001a370: 7567 6769 6e67 0a20 2020 2020 2020 2073  ugging.        s
+0001a380: 656c 662e 6d73 675f 626f 7820 3d20 514d  elf.msg_box = QM
+0001a390: 6573 7361 6765 426f 7828 7365 6c66 290a  essageBox(self).
+0001a3a0: 2020 2020 2020 2020 2320 4d65 7373 6167          # Messag
+0001a3b0: 6542 6f78 206d 6f64 616c 6974 7920 6e65  eBox modality ne
+0001a3c0: 6564 7320 746f 2062 6520 6164 6170 7465  eds to be adapte
+0001a3d0: 6420 666f 7220 7465 7374 730a 2020 2020  d for tests.    
+0001a3e0: 2020 2020 2320 286f 7468 6572 7769 7365      # (otherwise
+0001a3f0: 2074 6573 7420 6578 6563 7574 696f 6e20   test execution 
+0001a400: 626c 6f63 6b73 290a 2020 2020 2020 2020  blocks).        
+0001a410: 7365 6c66 2e74 6573 745f 6d6f 6465 203d  self.test_mode =
+0001a420: 2046 616c 7365 0a20 2020 2020 2020 2023   False.        #
+0001a430: 2041 2053 6574 7469 6e67 732d 4469 616c   A Settings-Dial
+0001a440: 6f67 0a20 2020 2020 2020 2073 656c 662e  og.        self.
+0001a450: 6d6e 652e 6669 675f 7365 7474 696e 6773  mne.fig_settings
+0001a460: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0001a470: 2320 5374 6f72 6573 2064 6563 696d 6174  # Stores decimat
+0001a480: 6564 2064 6174 610a 2020 2020 2020 2020  ed data.        
+0001a490: 7365 6c66 2e6d 6e65 2e64 6563 696d 5f64  self.mne.decim_d
+0001a4a0: 6174 6120 3d20 4e6f 6e65 0a20 2020 2020  ata = None.     
+0001a4b0: 2020 2023 2053 746f 7265 7320 7970 6f73     # Stores ypos
+0001a4c0: 2066 6f72 2073 656c 6563 7469 6f6e 2d6d   for selection-m
+0001a4d0: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
+0001a4e0: 2e6d 6e65 2e73 656c 6563 7469 6f6e 5f79  .mne.selection_y
+0001a4f0: 706f 735f 6469 6374 203d 2064 6963 7428  pos_dict = dict(
+0001a500: 290a 2020 2020 2020 2020 2320 5061 7261  ).        # Para
+0001a510: 6d65 7465 7273 2066 6f72 2070 7265 636f  meters for preco
+0001a520: 6d70 7574 696e 670a 2020 2020 2020 2020  mputing.        
+0001a530: 7365 6c66 2e6d 6e65 2e65 6e61 626c 655f  self.mne.enable_
+0001a540: 7072 6563 6f6d 7075 7465 203d 2046 616c  precompute = Fal
+0001a550: 7365 0a20 2020 2020 2020 2073 656c 662e  se.        self.
+0001a560: 6d6e 652e 6461 7461 5f70 7265 636f 6d70  mne.data_precomp
+0001a570: 7574 6564 203d 2046 616c 7365 0a20 2020  uted = False.   
+0001a580: 2020 2020 2073 656c 662e 5f72 6572 756e       self._rerun
+0001a590: 5f6c 6f61 645f 7468 7265 6164 203d 2046  _load_thread = F
+0001a5a0: 616c 7365 0a20 2020 2020 2020 2073 656c  alse.        sel
+0001a5b0: 662e 6d6e 652e 7a73 636f 7265 5f72 6762  f.mne.zscore_rgb
+0001a5c0: 6120 3d20 4e6f 6e65 0a20 2020 2020 2020  a = None.       
+0001a5d0: 2023 2043 6f6e 7461 696e 6572 2066 6f72   # Container for
+0001a5e0: 2074 7261 6365 730a 2020 2020 2020 2020   traces.        
+0001a5f0: 7365 6c66 2e6d 6e65 2e74 7261 6365 7320  self.mne.traces 
+0001a600: 3d20 6c69 7374 2829 0a20 2020 2020 2020  = list().       
+0001a610: 2023 2053 6361 6c65 2d46 6163 746f 720a   # Scale-Factor.
+0001a620: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
+0001a630: 2e73 6361 6c65 5f66 6163 746f 7220 3d20  .scale_factor = 
+0001a640: 310a 2020 2020 2020 2020 2320 5374 6f72  1.        # Stor
+0001a650: 6573 2063 6861 6e6e 656c 2d74 7970 6573  es channel-types
+0001a660: 2066 6f72 2062 7574 7465 7266 6c79 2d6d   for butterfly-m
+0001a670: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
+0001a680: 2e6d 6e65 2e62 7574 7465 7266 6c79 5f74  .mne.butterfly_t
+0001a690: 7970 655f 6f72 6465 7220 3d20 5b74 7020  ype_order = [tp 
+0001a6a0: 666f 7220 7470 2069 6e0a 2020 2020 2020  for tp in.      
 0001a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6c0: 2020 2020 2020 2020 2020 2020 2020 4441                DA
-0001a6d0: 5441 5f43 485f 5459 5045 535f 4f52 4445  TA_CH_TYPES_ORDE
-0001a6e0: 520a 2020 2020 2020 2020 2020 2020 2020  R.              
+0001a6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6d0: 2020 2044 4154 415f 4348 5f54 5950 4553     DATA_CH_TYPES
+0001a6e0: 5f4f 5244 4552 0a20 2020 2020 2020 2020  _ORDER.         
 0001a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a700: 2020 2020 2020 2020 2020 2069 6620 7470             if tp
-0001a710: 2069 6e20 7365 6c66 2e6d 6e65 2e63 685f   in self.mne.ch_
-0001a720: 7479 7065 735d 0a20 2020 2020 2020 2069  types].        i
-0001a730: 6620 7365 6c66 2e6d 6e65 2e69 735f 6570  f self.mne.is_ep
-0001a740: 6f63 6873 3a0a 2020 2020 2020 2020 2020  ochs:.          
-0001a750: 2020 2320 5374 6f72 6573 2070 6172 616d    # Stores param
-0001a760: 6574 6572 7320 666f 7220 6570 6f63 6873  eters for epochs
-0001a770: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001a780: 662e 6d6e 652e 6570 6f63 685f 6475 7220  f.mne.epoch_dur 
-0001a790: 3d20 6e70 2e64 6966 6628 7365 6c66 2e6d  = np.diff(self.m
-0001a7a0: 6e65 2e62 6f75 6e64 6172 795f 7469 6d65  ne.boundary_time
-0001a7b0: 735b 3a32 5d29 5b30 5d0a 2020 2020 2020  s[:2])[0].      
-0001a7c0: 2020 2020 2020 6570 6f63 685f 6964 7820        epoch_idx 
-0001a7d0: 3d20 6e70 2e73 6561 7263 6873 6f72 7465  = np.searchsorte
-0001a7e0: 6428 7365 6c66 2e6d 6e65 2e6d 6964 706f  d(self.mne.midpo
-0001a7f0: 696e 7473 2c0a 2020 2020 2020 2020 2020  ints,.          
+0001a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a710: 6966 2074 7020 696e 2073 656c 662e 6d6e  if tp in self.mn
+0001a720: 652e 6368 5f74 7970 6573 5d0a 2020 2020  e.ch_types].    
+0001a730: 2020 2020 6966 2073 656c 662e 6d6e 652e      if self.mne.
+0001a740: 6973 5f65 706f 6368 733a 0a20 2020 2020  is_epochs:.     
+0001a750: 2020 2020 2020 2023 2053 746f 7265 7320         # Stores 
+0001a760: 7061 7261 6d65 7465 7273 2066 6f72 2065  parameters for e
+0001a770: 706f 6368 730a 2020 2020 2020 2020 2020  pochs.          
+0001a780: 2020 7365 6c66 2e6d 6e65 2e65 706f 6368    self.mne.epoch
+0001a790: 5f64 7572 203d 206e 702e 6469 6666 2873  _dur = np.diff(s
+0001a7a0: 656c 662e 6d6e 652e 626f 756e 6461 7279  elf.mne.boundary
+0001a7b0: 5f74 696d 6573 5b3a 325d 295b 305d 0a20  _times[:2])[0]. 
+0001a7c0: 2020 2020 2020 2020 2020 2065 706f 6368             epoch
+0001a7d0: 5f69 6478 203d 206e 702e 7365 6172 6368  _idx = np.search
+0001a7e0: 736f 7274 6564 2873 656c 662e 6d6e 652e  sorted(self.mne.
+0001a7f0: 6d69 6470 6f69 6e74 732c 0a20 2020 2020  midpoints,.     
 0001a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a810: 2020 2020 2020 2020 2020 2020 2020 2873                (s
-0001a820: 656c 662e 6d6e 652e 745f 7374 6172 742c  elf.mne.t_start,
-0001a830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a820: 2020 2028 7365 6c66 2e6d 6e65 2e74 5f73     (self.mne.t_s
+0001a830: 7461 7274 2c0a 2020 2020 2020 2020 2020  tart,.          
 0001a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a850: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0001a860: 6e65 2e74 5f73 7461 7274 202b 2073 656c  ne.t_start + sel
-0001a870: 662e 6d6e 652e 6475 7261 7469 6f6e 2929  f.mne.duration))
-0001a880: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001a890: 662e 6d6e 652e 6570 6f63 685f 6964 7820  f.mne.epoch_idx 
-0001a8a0: 3d20 6e70 2e61 7261 6e67 6528 6570 6f63  = np.arange(epoc
-0001a8b0: 685f 6964 785b 305d 2c20 6570 6f63 685f  h_idx[0], epoch_
-0001a8c0: 6964 785b 315d 290a 0a20 2020 2020 2020  idx[1])..       
-0001a8d0: 2023 204c 6f61 6420 6672 6f6d 2051 5365   # Load from QSe
-0001a8e0: 7474 696e 6773 2069 6620 6176 6169 6c61  ttings if availa
-0001a8f0: 626c 650a 2020 2020 2020 2020 666f 7220  ble.        for 
-0001a900: 7170 6172 616d 2069 6e20 7173 6574 7469  qparam in qsetti
-0001a910: 6e67 735f 7061 7261 6d73 3a0a 2020 2020  ngs_params:.    
-0001a920: 2020 2020 2020 2020 6465 6661 756c 7420          default 
-0001a930: 3d20 7173 6574 7469 6e67 735f 7061 7261  = qsettings_para
-0001a940: 6d73 5b71 7061 7261 6d5d 0a20 2020 2020  ms[qparam].     
-0001a950: 2020 2020 2020 2071 7661 6c75 6520 3d20         qvalue = 
-0001a960: 5153 6574 7469 6e67 7328 292e 7661 6c75  QSettings().valu
-0001a970: 6528 7170 6172 616d 2c20 6465 6661 756c  e(qparam, defaul
-0001a980: 7456 616c 7565 3d64 6566 6175 6c74 290a  tValue=default).
-0001a990: 2020 2020 2020 2020 2020 2020 2320 5153              # QS
-0001a9a0: 6574 7469 6e67 7320 6d61 7920 616c 7465  ettings may alte
-0001a9b0: 7220 7479 7065 7320 6465 7065 6e64 696e  r types dependin
-0001a9c0: 6720 6f6e 204f 530a 2020 2020 2020 2020  g on OS.        
-0001a9d0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-0001a9e0: 7461 6e63 6528 7176 616c 7565 2c20 7479  tance(qvalue, ty
-0001a9f0: 7065 2864 6566 6175 6c74 2929 3a0a 2020  pe(default)):.  
-0001aa00: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0001aa10: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0001aa20: 2020 2020 2020 2071 7661 6c75 6520 3d20         qvalue = 
-0001aa30: 6c69 7465 7261 6c5f 6576 616c 2871 7661  literal_eval(qva
-0001aa40: 6c75 6529 0a20 2020 2020 2020 2020 2020  lue).           
-0001aa50: 2020 2020 2065 7863 6570 7420 2853 796e       except (Syn
-0001aa60: 7461 7845 7272 6f72 2c20 5661 6c75 6545  taxError, ValueE
-0001aa70: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
-0001aa80: 2020 2020 2020 2020 2020 2069 6620 7176             if qv
-0001aa90: 616c 7565 2069 6e20 5b27 7472 7565 272c  alue in ['true',
-0001aaa0: 2027 6661 6c73 6527 5d3a 0a20 2020 2020   'false']:.     
+0001a850: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001a860: 656c 662e 6d6e 652e 745f 7374 6172 7420  elf.mne.t_start 
+0001a870: 2b20 7365 6c66 2e6d 6e65 2e64 7572 6174  + self.mne.durat
+0001a880: 696f 6e29 290a 2020 2020 2020 2020 2020  ion)).          
+0001a890: 2020 7365 6c66 2e6d 6e65 2e65 706f 6368    self.mne.epoch
+0001a8a0: 5f69 6478 203d 206e 702e 6172 616e 6765  _idx = np.arange
+0001a8b0: 2865 706f 6368 5f69 6478 5b30 5d2c 2065  (epoch_idx[0], e
+0001a8c0: 706f 6368 5f69 6478 5b31 5d29 0a0a 2020  poch_idx[1])..  
+0001a8d0: 2020 2020 2020 2320 4c6f 6164 2066 726f        # Load fro
+0001a8e0: 6d20 5153 6574 7469 6e67 7320 6966 2061  m QSettings if a
+0001a8f0: 7661 696c 6162 6c65 0a20 2020 2020 2020  vailable.       
+0001a900: 2066 6f72 2071 7061 7261 6d20 696e 2071   for qparam in q
+0001a910: 7365 7474 696e 6773 5f70 6172 616d 733a  settings_params:
+0001a920: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
+0001a930: 6175 6c74 203d 2071 7365 7474 696e 6773  ault = qsettings
+0001a940: 5f70 6172 616d 735b 7170 6172 616d 5d0a  _params[qparam].
+0001a950: 2020 2020 2020 2020 2020 2020 7176 616c              qval
+0001a960: 7565 203d 2051 5365 7474 696e 6773 2829  ue = QSettings()
+0001a970: 2e76 616c 7565 2871 7061 7261 6d2c 2064  .value(qparam, d
+0001a980: 6566 6175 6c74 5661 6c75 653d 6465 6661  efaultValue=defa
+0001a990: 756c 7429 0a20 2020 2020 2020 2020 2020  ult).           
+0001a9a0: 2023 2051 5365 7474 696e 6773 206d 6179   # QSettings may
+0001a9b0: 2061 6c74 6572 2074 7970 6573 2064 6570   alter types dep
+0001a9c0: 656e 6469 6e67 206f 6e20 4f53 0a20 2020  ending on OS.   
+0001a9d0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0001a9e0: 6973 696e 7374 616e 6365 2871 7661 6c75  isinstance(qvalu
+0001a9f0: 652c 2074 7970 6528 6465 6661 756c 7429  e, type(default)
+0001aa00: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001aa10: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001aa20: 2020 2020 2020 2020 2020 2020 7176 616c              qval
+0001aa30: 7565 203d 206c 6974 6572 616c 5f65 7661  ue = literal_eva
+0001aa40: 6c28 7176 616c 7565 290a 2020 2020 2020  l(qvalue).      
+0001aa50: 2020 2020 2020 2020 2020 6578 6365 7074            except
+0001aa60: 2028 5379 6e74 6178 4572 726f 722c 2056   (SyntaxError, V
+0001aa70: 616c 7565 4572 726f 7229 3a0a 2020 2020  alueError):.    
+0001aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aa90: 6966 2071 7661 6c75 6520 696e 205b 2774  if qvalue in ['t
+0001aaa0: 7275 6527 2c20 2766 616c 7365 275d 3a0a  rue', 'false']:.
 0001aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aac0: 2020 2071 7661 6c75 6520 3d20 626f 6f6c     qvalue = bool
-0001aad0: 2871 7661 6c75 6529 0a20 2020 2020 2020  (qvalue).       
-0001aae0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0001aaf0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001ab00: 2020 2020 2020 2020 2020 2071 7661 6c75             qvalu
-0001ab10: 6520 3d20 6465 6661 756c 740a 2020 2020  e = default.    
-0001ab20: 2020 2020 2020 2020 7365 7461 7474 7228          setattr(
-0001ab30: 7365 6c66 2e6d 6e65 2c20 7170 6172 616d  self.mne, qparam
-0001ab40: 2c20 7176 616c 7565 290a 0a20 2020 2020  , qvalue)..     
-0001ab50: 2020 2023 2049 6e69 7469 616c 697a 6520     # Initialize 
-0001ab60: 6368 616e 6e65 6c2d 636f 6c6f 7273 2066  channel-colors f
-0001ab70: 6f72 2066 6173 7465 7220 696e 6465 7869  or faster indexi
-0001ab80: 6e67 206c 6174 6572 0a20 2020 2020 2020  ng later.       
-0001ab90: 2073 656c 662e 6d6e 652e 6368 5f63 6f6c   self.mne.ch_col
-0001aba0: 6f72 5f72 6566 203d 2064 6963 7428 290a  or_ref = dict().
-0001abb0: 2020 2020 2020 2020 666f 7220 6964 782c          for idx,
-0001abc0: 2063 685f 6e61 6d65 2069 6e20 656e 756d   ch_name in enum
-0001abd0: 6572 6174 6528 7365 6c66 2e6d 6e65 2e63  erate(self.mne.c
-0001abe0: 685f 6e61 6d65 7329 3a0a 2020 2020 2020  h_names):.      
-0001abf0: 2020 2020 2020 6368 5f74 7970 6520 3d20        ch_type = 
-0001ac00: 7365 6c66 2e6d 6e65 2e63 685f 7479 7065  self.mne.ch_type
-0001ac10: 735b 6964 785d 0a20 2020 2020 2020 2020  s[idx].         
-0001ac20: 2020 2073 656c 662e 6d6e 652e 6368 5f63     self.mne.ch_c
-0001ac30: 6f6c 6f72 5f72 6566 5b63 685f 6e61 6d65  olor_ref[ch_name
-0001ac40: 5d20 3d20 7365 6c66 2e6d 6e65 2e63 685f  ] = self.mne.ch_
-0001ac50: 636f 6c6f 725f 6469 6374 5b63 685f 7479  color_dict[ch_ty
-0001ac60: 7065 5d0a 0a20 2020 2020 2020 2023 2049  pe]..        # I
-0001ac70: 6e69 7469 616c 697a 6520 6570 6f63 6820  nitialize epoch 
-0001ac80: 636f 6c6f 7273 2066 6f72 2066 6173 7465  colors for faste
-0001ac90: 7220 696e 6465 7869 6e67 206c 6174 6572  r indexing later
-0001aca0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0001acb0: 2e6d 6e65 2e69 735f 6570 6f63 6873 3a0a  .mne.is_epochs:.
-0001acc0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0001acd0: 656c 662e 6d6e 652e 6570 6f63 685f 636f  elf.mne.epoch_co
-0001ace0: 6c6f 7273 2069 7320 4e6f 6e65 3a0a 2020  lors is None:.  
-0001acf0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001ad00: 6c66 2e6d 6e65 2e65 706f 6368 5f63 6f6c  lf.mne.epoch_col
-0001ad10: 6f72 5f72 6566 203d 205c 0a20 2020 2020  or_ref = \.     
-0001ad20: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0001ad30: 702e 7265 7065 6174 285b 746f 5f72 6762  p.repeat([to_rgb
-0001ad40: 615f 6172 7261 7928 6329 2066 6f72 2063  a_array(c) for c
-0001ad50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001aac0: 2020 2020 2020 2020 7176 616c 7565 203d          qvalue =
+0001aad0: 2062 6f6f 6c28 7176 616c 7565 290a 2020   bool(qvalue).  
+0001aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aaf0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001ab00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab10: 7176 616c 7565 203d 2064 6566 6175 6c74  qvalue = default
+0001ab20: 0a20 2020 2020 2020 2020 2020 2073 6574  .            set
+0001ab30: 6174 7472 2873 656c 662e 6d6e 652c 2071  attr(self.mne, q
+0001ab40: 7061 7261 6d2c 2071 7661 6c75 6529 0a0a  param, qvalue)..
+0001ab50: 2020 2020 2020 2020 2320 496e 6974 6961          # Initia
+0001ab60: 6c69 7a65 2063 6861 6e6e 656c 2d63 6f6c  lize channel-col
+0001ab70: 6f72 7320 666f 7220 6661 7374 6572 2069  ors for faster i
+0001ab80: 6e64 6578 696e 6720 6c61 7465 720a 2020  ndexing later.  
+0001ab90: 2020 2020 2020 7365 6c66 2e6d 6e65 2e63        self.mne.c
+0001aba0: 685f 636f 6c6f 725f 7265 6620 3d20 6469  h_color_ref = di
+0001abb0: 6374 2829 0a20 2020 2020 2020 2066 6f72  ct().        for
+0001abc0: 2069 6478 2c20 6368 5f6e 616d 6520 696e   idx, ch_name in
+0001abd0: 2065 6e75 6d65 7261 7465 2873 656c 662e   enumerate(self.
+0001abe0: 6d6e 652e 6368 5f6e 616d 6573 293a 0a20  mne.ch_names):. 
+0001abf0: 2020 2020 2020 2020 2020 2063 685f 7479             ch_ty
+0001ac00: 7065 203d 2073 656c 662e 6d6e 652e 6368  pe = self.mne.ch
+0001ac10: 5f74 7970 6573 5b69 6478 5d0a 2020 2020  _types[idx].    
+0001ac20: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
+0001ac30: 2e63 685f 636f 6c6f 725f 7265 665b 6368  .ch_color_ref[ch
+0001ac40: 5f6e 616d 655d 203d 2073 656c 662e 6d6e  _name] = self.mn
+0001ac50: 652e 6368 5f63 6f6c 6f72 5f64 6963 745b  e.ch_color_dict[
+0001ac60: 6368 5f74 7970 655d 0a0a 2020 2020 2020  ch_type]..      
+0001ac70: 2020 2320 496e 6974 6961 6c69 7a65 2065    # Initialize e
+0001ac80: 706f 6368 2063 6f6c 6f72 7320 666f 7220  poch colors for 
+0001ac90: 6661 7374 6572 2069 6e64 6578 696e 6720  faster indexing 
+0001aca0: 6c61 7465 720a 2020 2020 2020 2020 6966  later.        if
+0001acb0: 2073 656c 662e 6d6e 652e 6973 5f65 706f   self.mne.is_epo
+0001acc0: 6368 733a 0a20 2020 2020 2020 2020 2020  chs:.           
+0001acd0: 2069 6620 7365 6c66 2e6d 6e65 2e65 706f   if self.mne.epo
+0001ace0: 6368 5f63 6f6c 6f72 7320 6973 204e 6f6e  ch_colors is Non
+0001acf0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001ad00: 2020 2073 656c 662e 6d6e 652e 6570 6f63     self.mne.epoc
+0001ad10: 685f 636f 6c6f 725f 7265 6620 3d20 5c0a  h_color_ref = \.
+0001ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad30: 2020 2020 6e70 2e72 6570 6561 7428 5b74      np.repeat([t
+0001ad40: 6f5f 7267 6261 5f61 7272 6179 2863 2920  o_rgba_array(c) 
+0001ad50: 666f 7220 630a 2020 2020 2020 2020 2020  for c.          
 0001ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad70: 696e 2073 656c 662e 6d6e 652e 6368 5f63  in self.mne.ch_c
-0001ad80: 6f6c 6f72 5f72 6566 2e76 616c 7565 7328  olor_ref.values(
-0001ad90: 295d 2c0a 2020 2020 2020 2020 2020 2020  )],.            
+0001ad70: 2020 2020 2069 6e20 7365 6c66 2e6d 6e65       in self.mne
+0001ad80: 2e63 685f 636f 6c6f 725f 7265 662e 7661  .ch_color_ref.va
+0001ad90: 6c75 6573 2829 5d2c 0a20 2020 2020 2020  lues()],.       
 0001ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001adb0: 2020 6c65 6e28 7365 6c66 2e6d 6e65 2e69    len(self.mne.i
-0001adc0: 6e73 7429 2c20 6178 6973 3d31 290a 2020  nst), axis=1).  
-0001add0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0001ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001adf0: 7365 6c66 2e6d 6e65 2e65 706f 6368 5f63  self.mne.epoch_c
-0001ae00: 6f6c 6f72 5f72 6566 203d 206e 702e 656d  olor_ref = np.em
-0001ae10: 7074 7928 286c 656e 2873 656c 662e 6d6e  pty((len(self.mn
-0001ae20: 652e 6368 5f6e 616d 6573 292c 0a20 2020  e.ch_names),.   
-0001ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001adb0: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
+0001adc0: 6d6e 652e 696e 7374 292c 2061 7869 733d  mne.inst), axis=
+0001add0: 3129 0a20 2020 2020 2020 2020 2020 2065  1).            e
+0001ade0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0001adf0: 2020 2020 2073 656c 662e 6d6e 652e 6570       self.mne.ep
+0001ae00: 6f63 685f 636f 6c6f 725f 7265 6620 3d20  och_color_ref = 
+0001ae10: 6e70 2e65 6d70 7479 2828 6c65 6e28 7365  np.empty((len(se
+0001ae20: 6c66 2e6d 6e65 2e63 685f 6e61 6d65 7329  lf.mne.ch_names)
+0001ae30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 0001ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae60: 2020 6c65 6e28 7365 6c66 2e6d 6e65 2e69    len(self.mne.i
-0001ae70: 6e73 7429 2c20 3429 290a 2020 2020 2020  nst), 4)).      
-0001ae80: 2020 2020 2020 2020 2020 666f 7220 6570            for ep
-0001ae90: 6f5f 6964 782c 2065 706f 2069 6e20 656e  o_idx, epo in en
-0001aea0: 756d 6572 6174 6528 7365 6c66 2e6d 6e65  umerate(self.mne
-0001aeb0: 2e65 706f 6368 5f63 6f6c 6f72 7329 3a0a  .epoch_colors):.
-0001aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aed0: 2020 2020 666f 7220 6368 5f69 6478 2c20      for ch_idx, 
-0001aee0: 636f 6c6f 7220 696e 2065 6e75 6d65 7261  color in enumera
-0001aef0: 7465 2865 706f 293a 0a20 2020 2020 2020  te(epo):.       
+0001ae60: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
+0001ae70: 6d6e 652e 696e 7374 292c 2034 2929 0a20  mne.inst), 4)). 
+0001ae80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001ae90: 6f72 2065 706f 5f69 6478 2c20 6570 6f20  or epo_idx, epo 
+0001aea0: 696e 2065 6e75 6d65 7261 7465 2873 656c  in enumerate(sel
+0001aeb0: 662e 6d6e 652e 6570 6f63 685f 636f 6c6f  f.mne.epoch_colo
+0001aec0: 7273 293a 0a20 2020 2020 2020 2020 2020  rs):.           
+0001aed0: 2020 2020 2020 2020 2066 6f72 2063 685f           for ch_
+0001aee0: 6964 782c 2063 6f6c 6f72 2069 6e20 656e  idx, color in en
+0001aef0: 756d 6572 6174 6528 6570 6f29 3a0a 2020  umerate(epo):.  
 0001af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af10: 2073 656c 662e 6d6e 652e 6570 6f63 685f   self.mne.epoch_
-0001af20: 636f 6c6f 725f 7265 665b 6368 5f69 6478  color_ref[ch_idx
-0001af30: 2c20 6570 6f5f 6964 785d 203d 205c 0a20  , epo_idx] = \. 
-0001af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af50: 2020 2020 2020 2020 2020 2074 6f5f 7267             to_rg
-0001af60: 6261 5f61 7272 6179 2863 6f6c 6f72 290a  ba_array(color).
-0001af70: 0a20 2020 2020 2020 2020 2020 2023 204d  .            # M
-0001af80: 6172 6b20 6261 6420 6570 6f63 6873 0a20  ark bad epochs. 
-0001af90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001afa0: 6d6e 652e 6570 6f63 685f 636f 6c6f 725f  mne.epoch_color_
-0001afb0: 7265 665b 3a2c 2073 656c 662e 6d6e 652e  ref[:, self.mne.
-0001afc0: 6261 645f 6570 6f63 6873 5d20 3d20 5c0a  bad_epochs] = \.
-0001afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afe0: 746f 5f72 6762 615f 6172 7261 7928 7365  to_rgba_array(se
-0001aff0: 6c66 2e6d 6e65 2e65 706f 6368 5f63 6f6c  lf.mne.epoch_col
-0001b000: 6f72 5f62 6164 290a 0a20 2020 2020 2020  or_bad)..       
-0001b010: 2020 2020 2023 204d 6172 6b20 6261 6420       # Mark bad 
-0001b020: 6368 616e 6e65 6c73 0a20 2020 2020 2020  channels.       
-0001b030: 2020 2020 2062 6164 5f69 6478 7320 3d20       bad_idxs = 
-0001b040: 6e70 2e69 6e31 6428 7365 6c66 2e6d 6e65  np.in1d(self.mne
-0001b050: 2e63 685f 6e61 6d65 732c 2073 656c 662e  .ch_names, self.
-0001b060: 6d6e 652e 696e 666f 5b27 6261 6473 275d  mne.info['bads']
-0001b070: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0001b080: 6c66 2e6d 6e65 2e65 706f 6368 5f63 6f6c  lf.mne.epoch_col
-0001b090: 6f72 5f72 6566 5b62 6164 5f69 6478 732c  or_ref[bad_idxs,
-0001b0a0: 203a 5d20 3d20 5c0a 2020 2020 2020 2020   :] = \.        
-0001b0b0: 2020 2020 2020 2020 746f 5f72 6762 615f          to_rgba_
-0001b0c0: 6172 7261 7928 7365 6c66 2e6d 6e65 2e63  array(self.mne.c
-0001b0d0: 685f 636f 6c6f 725f 6261 6429 0a0a 2020  h_color_bad)..  
-0001b0e0: 2020 2020 2020 2320 4164 6420 4c6f 6164        # Add Load
-0001b0f0: 2d50 726f 6772 6573 7362 6172 2066 6f72  -Progressbar for
-0001b100: 206c 6f61 6469 6e67 2069 6e20 6120 7468   loading in a th
-0001b110: 7265 6164 0a20 2020 2020 2020 2073 656c  read.        sel
-0001b120: 662e 6d6e 652e 6c6f 6164 5f70 726f 675f  f.mne.load_prog_
-0001b130: 6c61 6265 6c20 3d20 514c 6162 656c 2827  label = QLabel('
-0001b140: 4c6f 6164 696e 672e 2e2e 2729 0a20 2020  Loading...').   
-0001b150: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-0001b160: 4261 7228 292e 6164 6457 6964 6765 7428  Bar().addWidget(
-0001b170: 7365 6c66 2e6d 6e65 2e6c 6f61 645f 7072  self.mne.load_pr
-0001b180: 6f67 5f6c 6162 656c 290a 2020 2020 2020  og_label).      
-0001b190: 2020 7365 6c66 2e6d 6e65 2e6c 6f61 645f    self.mne.load_
-0001b1a0: 7072 6f67 5f6c 6162 656c 2e68 6964 6528  prog_label.hide(
-0001b1b0: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
-0001b1c0: 6e65 2e6c 6f61 645f 7072 6f67 7265 7373  ne.load_progress
-0001b1d0: 6261 7220 3d20 5150 726f 6772 6573 7342  bar = QProgressB
-0001b1e0: 6172 2829 0a20 2020 2020 2020 2023 2053  ar().        # S
-0001b1f0: 6574 2074 6f20 6e5f 6368 756e 6b73 206f  et to n_chunks o
-0001b200: 6620 4c6f 6164 5275 6e6e 6572 0a20 2020  f LoadRunner.   
-0001b210: 2020 2020 2073 656c 662e 6d6e 652e 6c6f       self.mne.lo
-0001b220: 6164 5f70 726f 6772 6573 7362 6172 2e73  ad_progressbar.s
-0001b230: 6574 4d61 7869 6d75 6d28 3130 290a 2020  etMaximum(10).  
-0001b240: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0001b250: 7342 6172 2829 2e61 6464 5769 6467 6574  sBar().addWidget
-0001b260: 2873 656c 662e 6d6e 652e 6c6f 6164 5f70  (self.mne.load_p
-0001b270: 726f 6772 6573 7362 6172 2c20 7374 7265  rogressbar, stre
-0001b280: 7463 683d 3129 0a20 2020 2020 2020 2073  tch=1).        s
-0001b290: 656c 662e 6d6e 652e 6c6f 6164 5f70 726f  elf.mne.load_pro
-0001b2a0: 6772 6573 7362 6172 2e68 6964 6528 290a  gressbar.hide().
-0001b2b0: 0a20 2020 2020 2020 2023 2041 2051 5468  .        # A QTh
-0001b2c0: 7265 6164 2066 6f72 2070 7265 6c6f 6164  read for preload
-0001b2d0: 696e 670a 2020 2020 2020 2020 7365 6c66  ing.        self
-0001b2e0: 2e6c 6f61 645f 7468 7265 6164 203d 204c  .load_thread = L
-0001b2f0: 6f61 6454 6872 6561 6428 7365 6c66 290a  oadThread(self).
-0001b300: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
-0001b310: 6520 6365 6e74 7261 6c57 6964 6765 7420  e centralWidget 
-0001b320: 616e 6420 6c61 796f 7574 0a20 2020 2020  and layout.     
-0001b330: 2020 2077 6964 6765 7420 3d20 5157 6964     widget = QWid
-0001b340: 6765 7428 290a 2020 2020 2020 2020 6c61  get().        la
-0001b350: 796f 7574 203d 2051 4772 6964 4c61 796f  yout = QGridLayo
-0001b360: 7574 2829 0a0a 2020 2020 2020 2020 2320  ut()..        # 
-0001b370: 496e 6974 6961 6c69 7a65 2041 7869 732d  Initialize Axis-
-0001b380: 4974 656d 730a 2020 2020 2020 2020 7365  Items.        se
-0001b390: 6c66 2e6d 6e65 2e74 696d 655f 6178 6973  lf.mne.time_axis
-0001b3a0: 203d 2054 696d 6541 7869 7328 7365 6c66   = TimeAxis(self
-0001b3b0: 2e6d 6e65 290a 2020 2020 2020 2020 6966  .mne).        if
-0001b3c0: 2073 656c 662e 6d6e 652e 6973 5f65 706f   self.mne.is_epo
-0001b3d0: 6368 733a 0a20 2020 2020 2020 2020 2020  chs:.           
-0001b3e0: 2073 656c 662e 6d6e 652e 7469 6d65 5f61   self.mne.time_a
-0001b3f0: 7869 732e 7365 744c 6162 656c 2874 6578  xis.setLabel(tex
-0001b400: 743d 2745 706f 6368 2049 6e64 6578 272c  t='Epoch Index',
-0001b410: 2075 6e69 7473 3d4e 6f6e 6529 0a20 2020   units=None).   
-0001b420: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0001b430: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-0001b440: 7469 6d65 5f61 7869 732e 7365 744c 6162  time_axis.setLab
-0001b450: 656c 2874 6578 743d 2754 696d 6527 2c20  el(text='Time', 
-0001b460: 756e 6974 733d 2773 2729 0a0a 2020 2020  units='s')..    
-0001b470: 2020 2020 7365 6c66 2e6d 6e65 2e63 6861      self.mne.cha
-0001b480: 6e6e 656c 5f61 7869 7320 3d20 4368 616e  nnel_axis = Chan
-0001b490: 6e65 6c41 7869 7328 7365 6c66 290a 2020  nelAxis(self).  
-0001b4a0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e76        self.mne.v
-0001b4b0: 6965 7762 6f78 203d 2052 6177 5669 6577  iewbox = RawView
-0001b4c0: 426f 7828 7365 6c66 290a 0a20 2020 2020  Box(self)..     
-0001b4d0: 2020 2023 2053 7461 7274 2070 7265 636f     # Start preco
-0001b4e0: 6d70 7574 696e 6720 6966 2065 6e61 626c  mputing if enabl
-0001b4f0: 6564 0a20 2020 2020 2020 2073 656c 662e  ed.        self.
-0001b500: 5f69 6e69 745f 7072 6563 6f6d 7075 7465  _init_precompute
-0001b510: 2829 0a0a 2020 2020 2020 2020 2320 5061  ()..        # Pa
-0001b520: 7261 6d65 7465 7273 2066 6f72 206f 7665  rameters for ove
-0001b530: 7276 6965 7762 6172 0a20 2020 2020 2020  rviewbar.       
-0001b540: 2073 656c 662e 6d6e 652e 6f76 6572 7669   self.mne.overvi
-0001b550: 6577 5f6d 6f64 6520 3d20 6765 7461 7474  ew_mode = getatt
-0001b560: 7228 7365 6c66 2e6d 6e65 2c20 276f 7665  r(self.mne, 'ove
-0001b570: 7276 6965 775f 6d6f 6465 272c 2027 6368  rview_mode', 'ch
-0001b580: 616e 6e65 6c73 2729 0a20 2020 2020 2020  annels').       
-0001b590: 206f 7665 7276 6965 775f 6974 656d 7320   overview_items 
-0001b5a0: 3d20 6469 6374 280a 2020 2020 2020 2020  = dict(.        
-0001b5b0: 2020 2020 656d 7074 793d 2745 6d70 7479      empty='Empty
-0001b5c0: 272c 0a20 2020 2020 2020 2020 2020 2063  ',.            c
-0001b5d0: 6861 6e6e 656c 733d 2743 6861 6e6e 656c  hannels='Channel
-0001b5e0: 7327 2c0a 2020 2020 2020 2020 290a 2020  s',.        ).  
-0001b5f0: 2020 2020 2020 6966 2073 656c 662e 6d6e        if self.mn
-0001b600: 652e 656e 6162 6c65 5f70 7265 636f 6d70  e.enable_precomp
-0001b610: 7574 653a 0a20 2020 2020 2020 2020 2020  ute:.           
-0001b620: 206f 7665 7276 6965 775f 6974 656d 735b   overview_items[
-0001b630: 277a 7363 6f72 6527 5d20 3d20 275a 2d53  'zscore'] = 'Z-S
-0001b640: 636f 7265 270a 2020 2020 2020 2020 656c  core'.        el
-0001b650: 6966 2073 656c 662e 6d6e 652e 6f76 6572  if self.mne.over
-0001b660: 7669 6577 5f6d 6f64 6520 3d3d 2027 7a73  view_mode == 'zs
-0001b670: 636f 7265 273a 0a20 2020 2020 2020 2020  core':.         
-0001b680: 2020 2077 6172 6e28 2743 616e 6e6f 7420     warn('Cannot 
-0001b690: 7573 6520 7a2d 7363 6f72 6520 6d6f 6465  use z-score mode
-0001b6a0: 2077 6974 686f 7574 2070 7265 636f 6d70   without precomp
-0001b6b0: 7574 6174 696f 6e2c 2073 6574 7469 6e67  utation, setting
-0001b6c0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-0001b6d0: 2020 2020 276f 7665 7276 6965 775f 6d6f      'overview_mo
-0001b6e0: 6465 3d22 6368 616e 6e65 6c73 2227 290a  de="channels"').
-0001b6f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001b700: 2e6d 6e65 2e6f 7665 7276 6965 775f 6d6f  .mne.overview_mo
-0001b710: 6465 203d 2027 6368 616e 6e65 6c73 270a  de = 'channels'.
-0001b720: 2020 2020 2020 2020 5f63 6865 636b 5f6f          _check_o
-0001b730: 7074 696f 6e28 0a20 2020 2020 2020 2020  ption(.         
-0001b740: 2020 2027 6f76 6572 7669 6577 5f6d 6f64     'overview_mod
-0001b750: 6527 2c20 7365 6c66 2e6d 6e65 2e6f 7665  e', self.mne.ove
-0001b760: 7276 6965 775f 6d6f 6465 2c0a 2020 2020  rview_mode,.    
-0001b770: 2020 2020 2020 2020 6c69 7374 286f 7665          list(ove
-0001b780: 7276 6965 775f 6974 656d 7329 202b 205b  rview_items) + [
-0001b790: 2768 6964 6465 6e27 5d29 0a20 2020 2020  'hidden']).     
-0001b7a0: 2020 2068 6964 655f 6f76 6572 7669 6577     hide_overview
-0001b7b0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-0001b7c0: 2069 6620 7365 6c66 2e6d 6e65 2e6f 7665   if self.mne.ove
-0001b7d0: 7276 6965 775f 6d6f 6465 203d 3d20 2768  rview_mode == 'h
-0001b7e0: 6964 6465 6e27 3a0a 2020 2020 2020 2020  idden':.        
-0001b7f0: 2020 2020 6869 6465 5f6f 7665 7276 6965      hide_overvie
-0001b800: 7720 3d20 5472 7565 0a20 2020 2020 2020  w = True.       
-0001b810: 2020 2020 2073 656c 662e 6d6e 652e 6f76       self.mne.ov
-0001b820: 6572 7669 6577 5f6d 6f64 6520 3d20 2763  erview_mode = 'c
-0001b830: 6861 6e6e 656c 7327 0a0a 2020 2020 2020  hannels'..      
-0001b840: 2020 2320 496e 6974 6961 6c69 7a65 2064    # Initialize d
-0001b850: 6174 6120 286e 6565 6465 6420 696e 2044  ata (needed in D
-0001b860: 6174 6154 7261 6365 2e75 7064 6174 655f  ataTrace.update_
-0001b870: 6461 7461 292e 0a20 2020 2020 2020 2073  data)..        s
-0001b880: 656c 662e 5f75 7064 6174 655f 6461 7461  elf._update_data
-0001b890: 2829 0a0a 2020 2020 2020 2020 2320 496e  ()..        # In
-0001b8a0: 6974 6961 6c69 7a65 2054 7261 6365 2d50  itialize Trace-P
-0001b8b0: 6c6f 740a 2020 2020 2020 2020 7365 6c66  lot.        self
-0001b8c0: 2e6d 6e65 2e70 6c74 203d 2050 6c6f 7449  .mne.plt = PlotI
-0001b8d0: 7465 6d28 7669 6577 426f 783d 7365 6c66  tem(viewBox=self
-0001b8e0: 2e6d 6e65 2e76 6965 7762 6f78 2c0a 2020  .mne.viewbox,.  
-0001b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b900: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-0001b910: 6973 4974 656d 733d 7b27 626f 7474 6f6d  isItems={'bottom
-0001b920: 273a 2073 656c 662e 6d6e 652e 7469 6d65  ': self.mne.time
-0001b930: 5f61 7869 732c 0a20 2020 2020 2020 2020  _axis,.         
+0001af10: 2020 2020 2020 7365 6c66 2e6d 6e65 2e65        self.mne.e
+0001af20: 706f 6368 5f63 6f6c 6f72 5f72 6566 5b63  poch_color_ref[c
+0001af30: 685f 6964 782c 2065 706f 5f69 6478 5d20  h_idx, epo_idx] 
+0001af40: 3d20 5c0a 2020 2020 2020 2020 2020 2020  = \.            
+0001af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af60: 746f 5f72 6762 615f 6172 7261 7928 636f  to_rgba_array(co
+0001af70: 6c6f 7229 0a0a 2020 2020 2020 2020 2020  lor)..          
+0001af80: 2020 2320 4d61 726b 2062 6164 2065 706f    # Mark bad epo
+0001af90: 6368 730a 2020 2020 2020 2020 2020 2020  chs.            
+0001afa0: 7365 6c66 2e6d 6e65 2e65 706f 6368 5f63  self.mne.epoch_c
+0001afb0: 6f6c 6f72 5f72 6566 5b3a 2c20 7365 6c66  olor_ref[:, self
+0001afc0: 2e6d 6e65 2e62 6164 5f65 706f 6368 735d  .mne.bad_epochs]
+0001afd0: 203d 205c 0a20 2020 2020 2020 2020 2020   = \.           
+0001afe0: 2020 2020 2074 6f5f 7267 6261 5f61 7272       to_rgba_arr
+0001aff0: 6179 2873 656c 662e 6d6e 652e 6570 6f63  ay(self.mne.epoc
+0001b000: 685f 636f 6c6f 725f 6261 6429 0a0a 2020  h_color_bad)..  
+0001b010: 2020 2020 2020 2020 2020 2320 4d61 726b            # Mark
+0001b020: 2062 6164 2063 6861 6e6e 656c 730a 2020   bad channels.  
+0001b030: 2020 2020 2020 2020 2020 6261 645f 6964            bad_id
+0001b040: 7873 203d 206e 702e 696e 3164 2873 656c  xs = np.in1d(sel
+0001b050: 662e 6d6e 652e 6368 5f6e 616d 6573 2c20  f.mne.ch_names, 
+0001b060: 7365 6c66 2e6d 6e65 2e69 6e66 6f5b 2762  self.mne.info['b
+0001b070: 6164 7327 5d29 0a20 2020 2020 2020 2020  ads']).         
+0001b080: 2020 2073 656c 662e 6d6e 652e 6570 6f63     self.mne.epoc
+0001b090: 685f 636f 6c6f 725f 7265 665b 6261 645f  h_color_ref[bad_
+0001b0a0: 6964 7873 2c20 3a5d 203d 205c 0a20 2020  idxs, :] = \.   
+0001b0b0: 2020 2020 2020 2020 2020 2020 2074 6f5f               to_
+0001b0c0: 7267 6261 5f61 7272 6179 2873 656c 662e  rgba_array(self.
+0001b0d0: 6d6e 652e 6368 5f63 6f6c 6f72 5f62 6164  mne.ch_color_bad
+0001b0e0: 290a 0a20 2020 2020 2020 2023 2041 6464  )..        # Add
+0001b0f0: 204c 6f61 642d 5072 6f67 7265 7373 6261   Load-Progressba
+0001b100: 7220 666f 7220 6c6f 6164 696e 6720 696e  r for loading in
+0001b110: 2061 2074 6872 6561 640a 2020 2020 2020   a thread.      
+0001b120: 2020 7365 6c66 2e6d 6e65 2e6c 6f61 645f    self.mne.load_
+0001b130: 7072 6f67 5f6c 6162 656c 203d 2051 4c61  prog_label = QLa
+0001b140: 6265 6c28 274c 6f61 6469 6e67 2e2e 2e27  bel('Loading...'
+0001b150: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0001b160: 7461 7475 7342 6172 2829 2e61 6464 5769  tatusBar().addWi
+0001b170: 6467 6574 2873 656c 662e 6d6e 652e 6c6f  dget(self.mne.lo
+0001b180: 6164 5f70 726f 675f 6c61 6265 6c29 0a20  ad_prog_label). 
+0001b190: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
+0001b1a0: 6c6f 6164 5f70 726f 675f 6c61 6265 6c2e  load_prog_label.
+0001b1b0: 6869 6465 2829 0a20 2020 2020 2020 2073  hide().        s
+0001b1c0: 656c 662e 6d6e 652e 6c6f 6164 5f70 726f  elf.mne.load_pro
+0001b1d0: 6772 6573 7362 6172 203d 2051 5072 6f67  gressbar = QProg
+0001b1e0: 7265 7373 4261 7228 290a 2020 2020 2020  ressBar().      
+0001b1f0: 2020 2320 5365 7420 746f 206e 5f63 6875    # Set to n_chu
+0001b200: 6e6b 7320 6f66 204c 6f61 6452 756e 6e65  nks of LoadRunne
+0001b210: 720a 2020 2020 2020 2020 7365 6c66 2e6d  r.        self.m
+0001b220: 6e65 2e6c 6f61 645f 7072 6f67 7265 7373  ne.load_progress
+0001b230: 6261 722e 7365 744d 6178 696d 756d 2831  bar.setMaximum(1
+0001b240: 3029 0a20 2020 2020 2020 2073 656c 662e  0).        self.
+0001b250: 7374 6174 7573 4261 7228 292e 6164 6457  statusBar().addW
+0001b260: 6964 6765 7428 7365 6c66 2e6d 6e65 2e6c  idget(self.mne.l
+0001b270: 6f61 645f 7072 6f67 7265 7373 6261 722c  oad_progressbar,
+0001b280: 2073 7472 6574 6368 3d31 290a 2020 2020   stretch=1).    
+0001b290: 2020 2020 7365 6c66 2e6d 6e65 2e6c 6f61      self.mne.loa
+0001b2a0: 645f 7072 6f67 7265 7373 6261 722e 6869  d_progressbar.hi
+0001b2b0: 6465 2829 0a0a 2020 2020 2020 2020 2320  de()..        # 
+0001b2c0: 4120 5154 6872 6561 6420 666f 7220 7072  A QThread for pr
+0001b2d0: 656c 6f61 6469 6e67 0a20 2020 2020 2020  eloading.       
+0001b2e0: 2073 656c 662e 6c6f 6164 5f74 6872 6561   self.load_threa
+0001b2f0: 6420 3d20 4c6f 6164 5468 7265 6164 2873  d = LoadThread(s
+0001b300: 656c 6629 0a0a 2020 2020 2020 2020 2320  elf)..        # 
+0001b310: 4372 6561 7465 2063 656e 7472 616c 5769  Create centralWi
+0001b320: 6467 6574 2061 6e64 206c 6179 6f75 740a  dget and layout.
+0001b330: 2020 2020 2020 2020 7769 6467 6574 203d          widget =
+0001b340: 2051 5769 6467 6574 2829 0a20 2020 2020   QWidget().     
+0001b350: 2020 206c 6179 6f75 7420 3d20 5147 7269     layout = QGri
+0001b360: 644c 6179 6f75 7428 290a 0a20 2020 2020  dLayout()..     
+0001b370: 2020 2023 2049 6e69 7469 616c 697a 6520     # Initialize 
+0001b380: 4178 6973 2d49 7465 6d73 0a20 2020 2020  Axis-Items.     
+0001b390: 2020 2073 656c 662e 6d6e 652e 7469 6d65     self.mne.time
+0001b3a0: 5f61 7869 7320 3d20 5469 6d65 4178 6973  _axis = TimeAxis
+0001b3b0: 2873 656c 662e 6d6e 6529 0a20 2020 2020  (self.mne).     
+0001b3c0: 2020 2069 6620 7365 6c66 2e6d 6e65 2e69     if self.mne.i
+0001b3d0: 735f 6570 6f63 6873 3a0a 2020 2020 2020  s_epochs:.      
+0001b3e0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e74        self.mne.t
+0001b3f0: 696d 655f 6178 6973 2e73 6574 4c61 6265  ime_axis.setLabe
+0001b400: 6c28 7465 7874 3d27 4570 6f63 6820 496e  l(text='Epoch In
+0001b410: 6465 7827 2c20 756e 6974 733d 4e6f 6e65  dex', units=None
+0001b420: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0001b430: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001b440: 2e6d 6e65 2e74 696d 655f 6178 6973 2e73  .mne.time_axis.s
+0001b450: 6574 4c61 6265 6c28 7465 7874 3d27 5469  etLabel(text='Ti
+0001b460: 6d65 272c 2075 6e69 7473 3d27 7327 290a  me', units='s').
+0001b470: 0a20 2020 2020 2020 2073 656c 662e 6d6e  .        self.mn
+0001b480: 652e 6368 616e 6e65 6c5f 6178 6973 203d  e.channel_axis =
+0001b490: 2043 6861 6e6e 656c 4178 6973 2873 656c   ChannelAxis(sel
+0001b4a0: 6629 0a20 2020 2020 2020 2073 656c 662e  f).        self.
+0001b4b0: 6d6e 652e 7669 6577 626f 7820 3d20 5261  mne.viewbox = Ra
+0001b4c0: 7756 6965 7742 6f78 2873 656c 6629 0a0a  wViewBox(self)..
+0001b4d0: 2020 2020 2020 2020 2320 5374 6172 7420          # Start 
+0001b4e0: 7072 6563 6f6d 7075 7469 6e67 2069 6620  precomputing if 
+0001b4f0: 656e 6162 6c65 640a 2020 2020 2020 2020  enabled.        
+0001b500: 7365 6c66 2e5f 696e 6974 5f70 7265 636f  self._init_preco
+0001b510: 6d70 7574 6528 290a 0a20 2020 2020 2020  mpute()..       
+0001b520: 2023 2050 6172 616d 6574 6572 7320 666f   # Parameters fo
+0001b530: 7220 6f76 6572 7669 6577 6261 720a 2020  r overviewbar.  
+0001b540: 2020 2020 2020 7365 6c66 2e6d 6e65 2e6f        self.mne.o
+0001b550: 7665 7276 6965 775f 6d6f 6465 203d 2067  verview_mode = g
+0001b560: 6574 6174 7472 2873 656c 662e 6d6e 652c  etattr(self.mne,
+0001b570: 2027 6f76 6572 7669 6577 5f6d 6f64 6527   'overview_mode'
+0001b580: 2c20 2763 6861 6e6e 656c 7327 290a 2020  , 'channels').  
+0001b590: 2020 2020 2020 6f76 6572 7669 6577 5f69        overview_i
+0001b5a0: 7465 6d73 203d 2064 6963 7428 0a20 2020  tems = dict(.   
+0001b5b0: 2020 2020 2020 2020 2065 6d70 7479 3d27           empty='
+0001b5c0: 456d 7074 7927 2c0a 2020 2020 2020 2020  Empty',.        
+0001b5d0: 2020 2020 6368 616e 6e65 6c73 3d27 4368      channels='Ch
+0001b5e0: 616e 6e65 6c73 272c 0a20 2020 2020 2020  annels',.       
+0001b5f0: 2029 0a20 2020 2020 2020 2069 6620 7365   ).        if se
+0001b600: 6c66 2e6d 6e65 2e65 6e61 626c 655f 7072  lf.mne.enable_pr
+0001b610: 6563 6f6d 7075 7465 3a0a 2020 2020 2020  ecompute:.      
+0001b620: 2020 2020 2020 6f76 6572 7669 6577 5f69        overview_i
+0001b630: 7465 6d73 5b27 7a73 636f 7265 275d 203d  tems['zscore'] =
+0001b640: 2027 5a2d 5363 6f72 6527 0a20 2020 2020   'Z-Score'.     
+0001b650: 2020 2065 6c69 6620 7365 6c66 2e6d 6e65     elif self.mne
+0001b660: 2e6f 7665 7276 6965 775f 6d6f 6465 203d  .overview_mode =
+0001b670: 3d20 277a 7363 6f72 6527 3a0a 2020 2020  = 'zscore':.    
+0001b680: 2020 2020 2020 2020 7761 726e 2827 4361          warn('Ca
+0001b690: 6e6e 6f74 2075 7365 207a 2d73 636f 7265  nnot use z-score
+0001b6a0: 206d 6f64 6520 7769 7468 6f75 7420 7072   mode without pr
+0001b6b0: 6563 6f6d 7075 7461 7469 6f6e 2c20 7365  ecomputation, se
+0001b6c0: 7474 696e 6720 270a 2020 2020 2020 2020  tting '.        
+0001b6d0: 2020 2020 2020 2020 2027 6f76 6572 7669           'overvi
+0001b6e0: 6577 5f6d 6f64 653d 2263 6861 6e6e 656c  ew_mode="channel
+0001b6f0: 7322 2729 0a20 2020 2020 2020 2020 2020  s"').           
+0001b700: 2073 656c 662e 6d6e 652e 6f76 6572 7669   self.mne.overvi
+0001b710: 6577 5f6d 6f64 6520 3d20 2763 6861 6e6e  ew_mode = 'chann
+0001b720: 656c 7327 0a20 2020 2020 2020 205f 6368  els'.        _ch
+0001b730: 6563 6b5f 6f70 7469 6f6e 280a 2020 2020  eck_option(.    
+0001b740: 2020 2020 2020 2020 276f 7665 7276 6965          'overvie
+0001b750: 775f 6d6f 6465 272c 2073 656c 662e 6d6e  w_mode', self.mn
+0001b760: 652e 6f76 6572 7669 6577 5f6d 6f64 652c  e.overview_mode,
+0001b770: 0a20 2020 2020 2020 2020 2020 206c 6973  .            lis
+0001b780: 7428 6f76 6572 7669 6577 5f69 7465 6d73  t(overview_items
+0001b790: 2920 2b20 5b27 6869 6464 656e 275d 290a  ) + ['hidden']).
+0001b7a0: 2020 2020 2020 2020 6869 6465 5f6f 7665          hide_ove
+0001b7b0: 7276 6965 7720 3d20 4661 6c73 650a 2020  rview = False.  
+0001b7c0: 2020 2020 2020 6966 2073 656c 662e 6d6e        if self.mn
+0001b7d0: 652e 6f76 6572 7669 6577 5f6d 6f64 6520  e.overview_mode 
+0001b7e0: 3d3d 2027 6869 6464 656e 273a 0a20 2020  == 'hidden':.   
+0001b7f0: 2020 2020 2020 2020 2068 6964 655f 6f76           hide_ov
+0001b800: 6572 7669 6577 203d 2054 7275 650a 2020  erview = True.  
+0001b810: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+0001b820: 6e65 2e6f 7665 7276 6965 775f 6d6f 6465  ne.overview_mode
+0001b830: 203d 2027 6368 616e 6e65 6c73 270a 0a20   = 'channels'.. 
+0001b840: 2020 2020 2020 2023 2049 6e69 7469 616c         # Initial
+0001b850: 697a 6520 6461 7461 2028 6e65 6564 6564  ize data (needed
+0001b860: 2069 6e20 4461 7461 5472 6163 652e 7570   in DataTrace.up
+0001b870: 6461 7465 5f64 6174 6129 2e0a 2020 2020  date_data)..    
+0001b880: 2020 2020 7365 6c66 2e5f 7570 6461 7465      self._update
+0001b890: 5f64 6174 6128 290a 0a20 2020 2020 2020  _data()..       
+0001b8a0: 2023 2049 6e69 7469 616c 697a 6520 5472   # Initialize Tr
+0001b8b0: 6163 652d 506c 6f74 0a20 2020 2020 2020  ace-Plot.       
+0001b8c0: 2073 656c 662e 6d6e 652e 706c 7420 3d20   self.mne.plt = 
+0001b8d0: 506c 6f74 4974 656d 2876 6965 7742 6f78  PlotItem(viewBox
+0001b8e0: 3d73 656c 662e 6d6e 652e 7669 6577 626f  =self.mne.viewbo
+0001b8f0: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
+0001b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b910: 2020 2061 7869 7349 7465 6d73 3d7b 2762     axisItems={'b
+0001b920: 6f74 746f 6d27 3a20 7365 6c66 2e6d 6e65  ottom': self.mne
+0001b930: 2e74 696d 655f 6178 6973 2c0a 2020 2020  .time_axis,.    
 0001b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001b950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b960: 2020 276c 6566 7427 3a20 7365 6c66 2e6d    'left': self.m
-0001b970: 6e65 2e63 6861 6e6e 656c 5f61 7869 737d  ne.channel_axis}
-0001b980: 290a 2020 2020 2020 2020 2320 4869 6465  ).        # Hide
-0001b990: 2041 7574 6f52 616e 6765 2d42 7574 746f   AutoRange-Butto
-0001b9a0: 6e0a 2020 2020 2020 2020 7365 6c66 2e6d  n.        self.m
-0001b9b0: 6e65 2e70 6c74 2e68 6964 6542 7574 746f  ne.plt.hideButto
-0001b9c0: 6e73 2829 0a20 2020 2020 2020 2023 2043  ns().        # C
-0001b9d0: 6f6e 6669 6775 7265 2058 592d 5261 6e67  onfigure XY-Rang
-0001b9e0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0001b9f0: 662e 6d6e 652e 6973 5f65 706f 6368 733a  f.mne.is_epochs:
-0001ba00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001ba10: 662e 6d6e 652e 786d 6178 203d 206c 656e  f.mne.xmax = len
-0001ba20: 2873 656c 662e 6d6e 652e 696e 7374 2e74  (self.mne.inst.t
-0001ba30: 696d 6573 2920 2a20 6c65 6e28 7365 6c66  imes) * len(self
-0001ba40: 2e6d 6e65 2e69 6e73 7429 205c 0a20 2020  .mne.inst) \.   
-0001ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ba60: 2020 2020 2020 2020 202f 2073 656c 662e           / self.
-0001ba70: 6d6e 652e 696e 666f 5b27 7366 7265 7127  mne.info['sfreq'
-0001ba80: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-0001ba90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001baa0: 2e6d 6e65 2e78 6d61 7820 3d20 7365 6c66  .mne.xmax = self
-0001bab0: 2e6d 6e65 2e69 6e73 742e 7469 6d65 735b  .mne.inst.times[
-0001bac0: 2d31 5d0a 2020 2020 2020 2020 2320 4164  -1].        # Ad
-0001bad0: 6420 6f6e 6520 656d 7074 7920 6c69 6e65  d one empty line
-0001bae0: 2061 7320 7061 6464 696e 6720 6174 2074   as padding at t
-0001baf0: 6f70 2028 793d 3029 2e0a 2020 2020 2020  op (y=0)..      
-0001bb00: 2020 2320 4e65 6761 7469 7665 2059 2d41    # Negative Y-A
-0001bb10: 7869 7320 746f 2064 6973 706c 6179 2063  xis to display c
-0001bb20: 6861 6e6e 656c 7320 6672 6f6d 2074 6f70  hannels from top
-0001bb30: 2e0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-0001bb40: 6e65 2e79 6d61 7820 3d20 6c65 6e28 7365  ne.ymax = len(se
-0001bb50: 6c66 2e6d 6e65 2e63 685f 6f72 6465 7229  lf.mne.ch_order)
-0001bb60: 202b 2031 0a20 2020 2020 2020 2073 656c   + 1.        sel
-0001bb70: 662e 6d6e 652e 706c 742e 7365 744c 696d  f.mne.plt.setLim
-0001bb80: 6974 7328 784d 696e 3d30 2c20 784d 6178  its(xMin=0, xMax
-0001bb90: 3d73 656c 662e 6d6e 652e 786d 6178 2c0a  =self.mne.xmax,.
-0001bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bbb0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-0001bbc0: 4d69 6e3d 302c 2079 4d61 783d 7365 6c66  Min=0, yMax=self
-0001bbd0: 2e6d 6e65 2e79 6d61 7829 0a20 2020 2020  .mne.ymax).     
-0001bbe0: 2020 2023 2043 6f6e 6e65 6374 2053 6967     # Connect Sig
-0001bbf0: 6e61 6c73 2066 726f 6d20 506c 6f74 4974  nals from PlotIt
-0001bc00: 656d 0a20 2020 2020 2020 2073 656c 662e  em.        self.
-0001bc10: 6d6e 652e 706c 742e 7369 6758 5261 6e67  mne.plt.sigXRang
-0001bc20: 6543 6861 6e67 6564 2e63 6f6e 6e65 6374  eChanged.connect
-0001bc30: 2873 656c 662e 5f78 7261 6e67 655f 6368  (self._xrange_ch
-0001bc40: 616e 6765 6429 0a20 2020 2020 2020 2073  anged).        s
-0001bc50: 656c 662e 6d6e 652e 706c 742e 7369 6759  elf.mne.plt.sigY
-0001bc60: 5261 6e67 6543 6861 6e67 6564 2e63 6f6e  RangeChanged.con
-0001bc70: 6e65 6374 2873 656c 662e 5f79 7261 6e67  nect(self._yrang
-0001bc80: 655f 6368 616e 6765 6429 0a0a 2020 2020  e_changed)..    
-0001bc90: 2020 2020 2320 4164 6420 7472 6163 6573      # Add traces
-0001bca0: 0a20 2020 2020 2020 2066 6f72 2063 685f  .        for ch_
-0001bcb0: 6964 7820 696e 2073 656c 662e 6d6e 652e  idx in self.mne.
-0001bcc0: 7069 636b 733a 0a20 2020 2020 2020 2020  picks:.         
-0001bcd0: 2020 2044 6174 6154 7261 6365 2873 656c     DataTrace(sel
-0001bce0: 662c 2063 685f 6964 7829 0a0a 2020 2020  f, ch_idx)..    
-0001bcf0: 2020 2020 2320 496e 6974 6961 6c69 7a65      # Initialize
-0001bd00: 2045 706f 6368 7320 4772 6964 0a20 2020   Epochs Grid.   
-0001bd10: 2020 2020 2069 6620 7365 6c66 2e6d 6e65       if self.mne
-0001bd20: 2e69 735f 6570 6f63 6873 3a0a 2020 2020  .is_epochs:.    
-0001bd30: 2020 2020 2020 2020 6772 6964 5f70 656e          grid_pen
-0001bd40: 203d 2073 656c 662e 6d6e 652e 6d6b 5065   = self.mne.mkPe
-0001bd50: 6e28 636f 6c6f 723d 276b 272c 2077 6964  n(color='k', wid
-0001bd60: 7468 3d32 2c20 7374 796c 653d 5174 2e44  th=2, style=Qt.D
-0001bd70: 6173 684c 696e 6529 0a20 2020 2020 2020  ashLine).       
-0001bd80: 2020 2020 2066 6f72 2078 5f67 7269 6420       for x_grid 
-0001bd90: 696e 2073 656c 662e 6d6e 652e 626f 756e  in self.mne.boun
-0001bda0: 6461 7279 5f74 696d 6573 5b31 3a2d 315d  dary_times[1:-1]
-0001bdb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001bdc0: 2020 6772 6964 5f6c 696e 6520 3d20 496e    grid_line = In
-0001bdd0: 6669 6e69 7465 4c69 6e65 2870 6f73 3d78  finiteLine(pos=x
-0001bde0: 5f67 7269 642c 0a20 2020 2020 2020 2020  _grid,.         
+0001b960: 2020 2020 2020 2027 6c65 6674 273a 2073         'left': s
+0001b970: 656c 662e 6d6e 652e 6368 616e 6e65 6c5f  elf.mne.channel_
+0001b980: 6178 6973 7d29 0a20 2020 2020 2020 2023  axis}).        #
+0001b990: 2048 6964 6520 4175 746f 5261 6e67 652d   Hide AutoRange-
+0001b9a0: 4275 7474 6f6e 0a20 2020 2020 2020 2073  Button.        s
+0001b9b0: 656c 662e 6d6e 652e 706c 742e 6869 6465  elf.mne.plt.hide
+0001b9c0: 4275 7474 6f6e 7328 290a 2020 2020 2020  Buttons().      
+0001b9d0: 2020 2320 436f 6e66 6967 7572 6520 5859    # Configure XY
+0001b9e0: 2d52 616e 6765 0a20 2020 2020 2020 2069  -Range.        i
+0001b9f0: 6620 7365 6c66 2e6d 6e65 2e69 735f 6570  f self.mne.is_ep
+0001ba00: 6f63 6873 3a0a 2020 2020 2020 2020 2020  ochs:.          
+0001ba10: 2020 7365 6c66 2e6d 6e65 2e78 6d61 7820    self.mne.xmax 
+0001ba20: 3d20 6c65 6e28 7365 6c66 2e6d 6e65 2e69  = len(self.mne.i
+0001ba30: 6e73 742e 7469 6d65 7329 202a 206c 656e  nst.times) * len
+0001ba40: 2873 656c 662e 6d6e 652e 696e 7374 2920  (self.mne.inst) 
+0001ba50: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
+0001ba60: 2020 2020 2020 2020 2020 2020 2020 2f20                / 
+0001ba70: 7365 6c66 2e6d 6e65 2e69 6e66 6f5b 2773  self.mne.info['s
+0001ba80: 6672 6571 275d 0a20 2020 2020 2020 2065  freq'].        e
+0001ba90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0001baa0: 2073 656c 662e 6d6e 652e 786d 6178 203d   self.mne.xmax =
+0001bab0: 2073 656c 662e 6d6e 652e 696e 7374 2e74   self.mne.inst.t
+0001bac0: 696d 6573 5b2d 315d 0a20 2020 2020 2020  imes[-1].       
+0001bad0: 2023 2041 6464 206f 6e65 2065 6d70 7479   # Add one empty
+0001bae0: 206c 696e 6520 6173 2070 6164 6469 6e67   line as padding
+0001baf0: 2061 7420 746f 7020 2879 3d30 292e 0a20   at top (y=0).. 
+0001bb00: 2020 2020 2020 2023 204e 6567 6174 6976         # Negativ
+0001bb10: 6520 592d 4178 6973 2074 6f20 6469 7370  e Y-Axis to disp
+0001bb20: 6c61 7920 6368 616e 6e65 6c73 2066 726f  lay channels fro
+0001bb30: 6d20 746f 702e 0a20 2020 2020 2020 2073  m top..        s
+0001bb40: 656c 662e 6d6e 652e 796d 6178 203d 206c  elf.mne.ymax = l
+0001bb50: 656e 2873 656c 662e 6d6e 652e 6368 5f6f  en(self.mne.ch_o
+0001bb60: 7264 6572 2920 2b20 310a 2020 2020 2020  rder) + 1.      
+0001bb70: 2020 7365 6c66 2e6d 6e65 2e70 6c74 2e73    self.mne.plt.s
+0001bb80: 6574 4c69 6d69 7473 2878 4d69 6e3d 302c  etLimits(xMin=0,
+0001bb90: 2078 4d61 783d 7365 6c66 2e6d 6e65 2e78   xMax=self.mne.x
+0001bba0: 6d61 782c 0a20 2020 2020 2020 2020 2020  max,.           
+0001bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bbc0: 2020 2020 794d 696e 3d30 2c20 794d 6178      yMin=0, yMax
+0001bbd0: 3d73 656c 662e 6d6e 652e 796d 6178 290a  =self.mne.ymax).
+0001bbe0: 2020 2020 2020 2020 2320 436f 6e6e 6563          # Connec
+0001bbf0: 7420 5369 676e 616c 7320 6672 6f6d 2050  t Signals from P
+0001bc00: 6c6f 7449 7465 6d0a 2020 2020 2020 2020  lotItem.        
+0001bc10: 7365 6c66 2e6d 6e65 2e70 6c74 2e73 6967  self.mne.plt.sig
+0001bc20: 5852 616e 6765 4368 616e 6765 642e 636f  XRangeChanged.co
+0001bc30: 6e6e 6563 7428 7365 6c66 2e5f 7872 616e  nnect(self._xran
+0001bc40: 6765 5f63 6861 6e67 6564 290a 2020 2020  ge_changed).    
+0001bc50: 2020 2020 7365 6c66 2e6d 6e65 2e70 6c74      self.mne.plt
+0001bc60: 2e73 6967 5952 616e 6765 4368 616e 6765  .sigYRangeChange
+0001bc70: 642e 636f 6e6e 6563 7428 7365 6c66 2e5f  d.connect(self._
+0001bc80: 7972 616e 6765 5f63 6861 6e67 6564 290a  yrange_changed).
+0001bc90: 0a20 2020 2020 2020 2023 2041 6464 2074  .        # Add t
+0001bca0: 7261 6365 730a 2020 2020 2020 2020 666f  races.        fo
+0001bcb0: 7220 6368 5f69 6478 2069 6e20 7365 6c66  r ch_idx in self
+0001bcc0: 2e6d 6e65 2e70 6963 6b73 3a0a 2020 2020  .mne.picks:.    
+0001bcd0: 2020 2020 2020 2020 4461 7461 5472 6163          DataTrac
+0001bce0: 6528 7365 6c66 2c20 6368 5f69 6478 290a  e(self, ch_idx).
+0001bcf0: 0a20 2020 2020 2020 2023 2049 6e69 7469  .        # Initi
+0001bd00: 616c 697a 6520 4570 6f63 6873 2047 7269  alize Epochs Gri
+0001bd10: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+0001bd20: 662e 6d6e 652e 6973 5f65 706f 6368 733a  f.mne.is_epochs:
+0001bd30: 0a20 2020 2020 2020 2020 2020 2067 7269  .            gri
+0001bd40: 645f 7065 6e20 3d20 7365 6c66 2e6d 6e65  d_pen = self.mne
+0001bd50: 2e6d 6b50 656e 2863 6f6c 6f72 3d27 6b27  .mkPen(color='k'
+0001bd60: 2c20 7769 6474 683d 322c 2073 7479 6c65  , width=2, style
+0001bd70: 3d51 742e 4461 7368 4c69 6e65 290a 2020  =Qt.DashLine).  
+0001bd80: 2020 2020 2020 2020 2020 666f 7220 785f            for x_
+0001bd90: 6772 6964 2069 6e20 7365 6c66 2e6d 6e65  grid in self.mne
+0001bda0: 2e62 6f75 6e64 6172 795f 7469 6d65 735b  .boundary_times[
+0001bdb0: 313a 2d31 5d3a 0a20 2020 2020 2020 2020  1:-1]:.         
+0001bdc0: 2020 2020 2020 2067 7269 645f 6c69 6e65         grid_line
+0001bdd0: 203d 2049 6e66 696e 6974 654c 696e 6528   = InfiniteLine(
+0001bde0: 706f 733d 785f 6772 6964 2c0a 2020 2020  pos=x_grid,.    
 0001bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be10: 7065 6e3d 6772 6964 5f70 656e 2c0a 2020  pen=grid_pen,.  
-0001be20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be10: 2020 2020 2070 656e 3d67 7269 645f 7065       pen=grid_pe
+0001be20: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
 0001be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be40: 2020 2020 2020 206d 6f76 6162 6c65 3d46         movable=F
-0001be50: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-0001be60: 2020 2020 2020 7365 6c66 2e6d 6e65 2e70        self.mne.p
-0001be70: 6c74 2e61 6464 4974 656d 2867 7269 645f  lt.addItem(grid_
-0001be80: 6c69 6e65 290a 0a20 2020 2020 2020 2023  line)..        #
-0001be90: 2041 6464 2065 7665 6e74 730a 2020 2020   Add events.    
-0001bea0: 2020 2020 6966 2067 6574 6174 7472 2873      if getattr(s
-0001beb0: 656c 662e 6d6e 652c 2027 6576 656e 745f  elf.mne, 'event_
-0001bec0: 6e75 6d73 272c 204e 6f6e 6529 2069 7320  nums', None) is 
-0001bed0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0001bee0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e65        self.mne.e
-0001bef0: 7665 6e74 735f 7669 7369 626c 6520 3d20  vents_visible = 
-0001bf00: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0001bf10: 2066 6f72 2065 765f 7469 6d65 2c20 6576   for ev_time, ev
-0001bf20: 5f69 6420 696e 207a 6970 2873 656c 662e  _id in zip(self.
-0001bf30: 6d6e 652e 6576 656e 745f 7469 6d65 732c  mne.event_times,
-0001bf40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001be40: 2020 2020 2020 2020 2020 2020 6d6f 7661              mova
+0001be50: 626c 653d 4661 6c73 6529 0a20 2020 2020  ble=False).     
+0001be60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001be70: 6d6e 652e 706c 742e 6164 6449 7465 6d28  mne.plt.addItem(
+0001be80: 6772 6964 5f6c 696e 6529 0a0a 2020 2020  grid_line)..    
+0001be90: 2020 2020 2320 4164 6420 6576 656e 7473      # Add events
+0001bea0: 0a20 2020 2020 2020 2069 6620 6765 7461  .        if geta
+0001beb0: 7474 7228 7365 6c66 2e6d 6e65 2c20 2765  ttr(self.mne, 'e
+0001bec0: 7665 6e74 5f6e 756d 7327 2c20 4e6f 6e65  vent_nums', None
+0001bed0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0001bee0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001bef0: 6d6e 652e 6576 656e 7473 5f76 6973 6962  mne.events_visib
+0001bf00: 6c65 203d 2054 7275 650a 2020 2020 2020  le = True.      
+0001bf10: 2020 2020 2020 666f 7220 6576 5f74 696d        for ev_tim
+0001bf20: 652c 2065 765f 6964 2069 6e20 7a69 7028  e, ev_id in zip(
+0001bf30: 7365 6c66 2e6d 6e65 2e65 7665 6e74 5f74  self.mne.event_t
+0001bf40: 696d 6573 2c0a 2020 2020 2020 2020 2020  imes,.          
 0001bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf60: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-0001bf70: 6576 656e 745f 6e75 6d73 293a 0a20 2020  event_nums):.   
-0001bf80: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-0001bf90: 6f72 203d 2073 656c 662e 6d6e 652e 6576  or = self.mne.ev
-0001bfa0: 656e 745f 636f 6c6f 725f 6469 6374 5b65  ent_color_dict[e
-0001bfb0: 765f 6964 5d0a 2020 2020 2020 2020 2020  v_id].          
-0001bfc0: 2020 2020 2020 6c61 6265 6c20 3d20 7365        label = se
-0001bfd0: 6c66 2e6d 6e65 2e65 7665 6e74 5f69 645f  lf.mne.event_id_
-0001bfe0: 7265 762e 6765 7428 6576 5f69 642c 2065  rev.get(ev_id, e
-0001bff0: 765f 6964 290a 2020 2020 2020 2020 2020  v_id).          
-0001c000: 2020 2020 2020 6576 656e 745f 6c69 6e65        event_line
-0001c010: 203d 2045 7665 6e74 4c69 6e65 2873 656c   = EventLine(sel
-0001c020: 662e 6d6e 652c 2065 765f 7469 6d65 2c20  f.mne, ev_time, 
-0001c030: 6c61 6265 6c2c 2063 6f6c 6f72 290a 2020  label, color).  
-0001c040: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001c050: 6c66 2e6d 6e65 2e65 7665 6e74 5f6c 696e  lf.mne.event_lin
-0001c060: 6573 2e61 7070 656e 6428 6576 656e 745f  es.append(event_
-0001c070: 6c69 6e65 290a 2020 2020 2020 2020 656c  line).        el
-0001c080: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001c090: 7365 6c66 2e6d 6e65 2e65 7665 6e74 735f  self.mne.events_
-0001c0a0: 7669 7369 626c 6520 3d20 4661 6c73 650a  visible = False.
-0001c0b0: 0a20 2020 2020 2020 2023 2041 6464 2053  .        # Add S
-0001c0c0: 6361 6c65 2d42 6172 730a 2020 2020 2020  cale-Bars.      
-0001c0d0: 2020 7365 6c66 2e5f 6164 645f 7363 616c    self._add_scal
-0001c0e0: 6562 6172 7328 290a 0a20 2020 2020 2020  ebars()..       
-0001c0f0: 2023 2043 6865 636b 2066 6f72 204f 7065   # Check for Ope
-0001c100: 6e47 4c0a 2020 2020 2020 2020 2320 4966  nGL.        # If
-0001c110: 2061 2075 7365 7220 646f 6573 6e27 7420   a user doesn't 
-0001c120: 7370 6563 6966 7920 7768 6574 6865 7220  specify whether 
-0001c130: 6f72 206e 6f74 2074 6f20 7573 6520 6974  or not to use it
-0001c140: 3a0a 2020 2020 2020 2020 2320 312e 2049  :.        # 1. I
-0001c150: 6620 6f6e 206d 6163 4f53 2c20 656e 6162  f on macOS, enab
-0001c160: 6c65 2069 7420 6279 2064 6566 6175 6c74  le it by default
-0001c170: 2074 6f20 6176 6f69 6420 7365 6766 6175   to avoid segfau
-0001c180: 6c74 0a20 2020 2020 2020 2023 2032 2e20  lt.        # 2. 
-0001c190: 4f74 6865 7277 6973 652c 2064 6973 6162  Otherwise, disab
-0001c1a0: 6c65 2069 7420 2870 6572 666f 726d 616e  le it (performan
-0001c1b0: 6365 2064 6966 6665 7265 6e63 6573 2073  ce differences s
-0001c1c0: 6565 6d20 6d69 6e69 6d61 6c2c 2061 6e64  eem minimal, and
-0001c1d0: 0a20 2020 2020 2020 2023 2020 2020 5079  .        #    Py
-0001c1e0: 4f70 656e 474c 2069 7320 616e 206f 7074  OpenGL is an opt
-0001c1f0: 696f 6e61 6c20 7265 7175 6972 656d 656e  ional requiremen
-0001c200: 7429 0a20 2020 2020 2020 206f 7065 6e67  t).        openg
-0001c210: 6c5f 6b65 7920 3d20 274d 4e45 5f42 524f  l_key = 'MNE_BRO
-0001c220: 5753 4552 5f55 5345 5f4f 5045 4e47 4c27  WSER_USE_OPENGL'
-0001c230: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0001c240: 2e6d 6e65 2e75 7365 5f6f 7065 6e67 6c20  .mne.use_opengl 
-0001c250: 6973 204e 6f6e 653a 2020 2320 6465 6661  is None:  # defa
-0001c260: 756c 743a 206f 7074 2d69 6e0a 2020 2020  ult: opt-in.    
-0001c270: 2020 2020 2020 2020 2320 4f70 656e 474c          # OpenGL
-0001c280: 206e 6565 6473 2074 6f20 6265 2065 6e61   needs to be ena
-0001c290: 626c 6564 206f 6e20 6d61 634f 530a 2020  bled on macOS.  
-0001c2a0: 2020 2020 2020 2020 2020 2320 2868 7474            # (htt
-0001c2b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0001c2c0: 6d6e 652d 746f 6f6c 732f 6d6e 652d 7174  mne-tools/mne-qt
-0001c2d0: 2d62 726f 7773 6572 2f69 7373 7565 732f  -browser/issues/
-0001c2e0: 3533 290a 2020 2020 2020 2020 2020 2020  53).            
-0001c2f0: 6465 6661 756c 7420 3d20 2774 7275 6527  default = 'true'
-0001c300: 2069 6620 706c 6174 666f 726d 2e73 7973   if platform.sys
-0001c310: 7465 6d28 2920 3d3d 2027 4461 7277 696e  tem() == 'Darwin
-0001c320: 2720 656c 7365 2027 270a 2020 2020 2020  ' else ''.      
-0001c330: 2020 2020 2020 636f 6e66 6967 5f76 616c        config_val
-0001c340: 203d 2067 6574 5f63 6f6e 6669 6728 6f70   = get_config(op
-0001c350: 656e 676c 5f6b 6579 2c20 6465 6661 756c  engl_key, defaul
-0001c360: 7429 2e6c 6f77 6572 2829 0a20 2020 2020  t).lower().     
-0001c370: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-0001c380: 7573 655f 6f70 656e 676c 203d 2028 636f  use_opengl = (co
-0001c390: 6e66 6967 5f76 616c 203d 3d20 2774 7275  nfig_val == 'tru
-0001c3a0: 6527 290a 0a20 2020 2020 2020 2069 6620  e')..        if 
-0001c3b0: 7365 6c66 2e6d 6e65 2e75 7365 5f6f 7065  self.mne.use_ope
-0001c3c0: 6e67 6c3a 0a20 2020 2020 2020 2020 2020  ngl:.           
-0001c3d0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0001c3e0: 2020 2020 2020 696d 706f 7274 204f 7065        import Ope
-0001c3f0: 6e47 4c0a 2020 2020 2020 2020 2020 2020  nGL.            
-0001c400: 6578 6365 7074 2028 4d6f 6475 6c65 4e6f  except (ModuleNo
-0001c410: 7446 6f75 6e64 4572 726f 722c 2049 6d70  tFoundError, Imp
-0001c420: 6f72 7445 7272 6f72 2920 6173 2065 7863  ortError) as exc
-0001c430: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001c440: 2020 2320 4f6e 206d 6163 4f53 2c20 6966    # On macOS, if
-0001c450: 2075 7365 5f6f 7065 6e67 6c20 6973 2054   use_opengl is T
-0001c460: 7275 6520 7765 2072 6169 7365 2061 6e20  rue we raise an 
-0001c470: 6572 726f 7220 6265 6361 7573 650a 2020  error because.  
-0001c480: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0001c490: 6974 2063 616e 206c 6561 6420 746f 2073  it can lead to s
-0001c4a0: 6567 6661 756c 7473 2e20 4966 2061 2075  egfaults. If a u
-0001c4b0: 7365 7220 7265 616c 6c79 206b 6e6f 7773  ser really knows
-0001c4c0: 2077 6861 7420 7468 6579 0a20 2020 2020   what they.     
-0001c4d0: 2020 2020 2020 2020 2020 2023 2061 7265             # are
-0001c4e0: 2064 6f69 6e67 2c20 7468 6579 2063 616e   doing, they can
-0001c4f0: 2070 6173 7320 7573 655f 6f70 656e 676c   pass use_opengl
-0001c500: 3d46 616c 7365 2028 6f72 2073 6574 0a20  =False (or set. 
-0001c510: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001c520: 204d 4e45 5f42 524f 5753 4552 5f55 5345   MNE_BROWSER_USE
-0001c530: 5f4f 5045 4e47 4c3d 6661 6c73 6529 0a20  _OPENGL=false). 
-0001c540: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001c550: 6620 706c 6174 666f 726d 2e73 7973 7465  f platform.syste
-0001c560: 6d28 2920 3d3d 2027 4461 7277 696e 273a  m() == 'Darwin':
-0001c570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c580: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
-0001c590: 6d65 4572 726f 7228 0a20 2020 2020 2020  meError(.       
+0001bf60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001bf70: 2e6d 6e65 2e65 7665 6e74 5f6e 756d 7329  .mne.event_nums)
+0001bf80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001bf90: 2020 636f 6c6f 7220 3d20 7365 6c66 2e6d    color = self.m
+0001bfa0: 6e65 2e65 7665 6e74 5f63 6f6c 6f72 5f64  ne.event_color_d
+0001bfb0: 6963 745b 6576 5f69 645d 0a20 2020 2020  ict[ev_id].     
+0001bfc0: 2020 2020 2020 2020 2020 206c 6162 656c             label
+0001bfd0: 203d 2073 656c 662e 6d6e 652e 6576 656e   = self.mne.even
+0001bfe0: 745f 6964 5f72 6576 2e67 6574 2865 765f  t_id_rev.get(ev_
+0001bff0: 6964 2c20 6576 5f69 6429 0a20 2020 2020  id, ev_id).     
+0001c000: 2020 2020 2020 2020 2020 2065 7665 6e74             event
+0001c010: 5f6c 696e 6520 3d20 4576 656e 744c 696e  _line = EventLin
+0001c020: 6528 7365 6c66 2e6d 6e65 2c20 6576 5f74  e(self.mne, ev_t
+0001c030: 696d 652c 206c 6162 656c 2c20 636f 6c6f  ime, label, colo
+0001c040: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+0001c050: 2020 2073 656c 662e 6d6e 652e 6576 656e     self.mne.even
+0001c060: 745f 6c69 6e65 732e 6170 7065 6e64 2865  t_lines.append(e
+0001c070: 7665 6e74 5f6c 696e 6529 0a20 2020 2020  vent_line).     
+0001c080: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001c090: 2020 2020 2073 656c 662e 6d6e 652e 6576       self.mne.ev
+0001c0a0: 656e 7473 5f76 6973 6962 6c65 203d 2046  ents_visible = F
+0001c0b0: 616c 7365 0a0a 2020 2020 2020 2020 2320  alse..        # 
+0001c0c0: 4164 6420 5363 616c 652d 4261 7273 0a20  Add Scale-Bars. 
+0001c0d0: 2020 2020 2020 2073 656c 662e 5f61 6464         self._add
+0001c0e0: 5f73 6361 6c65 6261 7273 2829 0a0a 2020  _scalebars()..  
+0001c0f0: 2020 2020 2020 2320 4368 6563 6b20 666f        # Check fo
+0001c100: 7220 4f70 656e 474c 0a20 2020 2020 2020  r OpenGL.       
+0001c110: 2023 2049 6620 6120 7573 6572 2064 6f65   # If a user doe
+0001c120: 736e 2774 2073 7065 6369 6679 2077 6865  sn't specify whe
+0001c130: 7468 6572 206f 7220 6e6f 7420 746f 2075  ther or not to u
+0001c140: 7365 2069 743a 0a20 2020 2020 2020 2023  se it:.        #
+0001c150: 2031 2e20 4966 206f 6e20 6d61 634f 532c   1. If on macOS,
+0001c160: 2065 6e61 626c 6520 6974 2062 7920 6465   enable it by de
+0001c170: 6661 756c 7420 746f 2061 766f 6964 2073  fault to avoid s
+0001c180: 6567 6661 756c 740a 2020 2020 2020 2020  egfault.        
+0001c190: 2320 322e 204f 7468 6572 7769 7365 2c20  # 2. Otherwise, 
+0001c1a0: 6469 7361 626c 6520 6974 2028 7065 7266  disable it (perf
+0001c1b0: 6f72 6d61 6e63 6520 6469 6666 6572 656e  ormance differen
+0001c1c0: 6365 7320 7365 656d 206d 696e 696d 616c  ces seem minimal
+0001c1d0: 2c20 616e 640a 2020 2020 2020 2020 2320  , and.        # 
+0001c1e0: 2020 2050 794f 7065 6e47 4c20 6973 2061     PyOpenGL is a
+0001c1f0: 6e20 6f70 7469 6f6e 616c 2072 6571 7569  n optional requi
+0001c200: 7265 6d65 6e74 290a 2020 2020 2020 2020  rement).        
+0001c210: 6f70 656e 676c 5f6b 6579 203d 2027 4d4e  opengl_key = 'MN
+0001c220: 455f 4252 4f57 5345 525f 5553 455f 4f50  E_BROWSER_USE_OP
+0001c230: 454e 474c 270a 2020 2020 2020 2020 6966  ENGL'.        if
+0001c240: 2073 656c 662e 6d6e 652e 7573 655f 6f70   self.mne.use_op
+0001c250: 656e 676c 2069 7320 4e6f 6e65 3a20 2023  engl is None:  #
+0001c260: 2064 6566 6175 6c74 3a20 6f70 742d 696e   default: opt-in
+0001c270: 0a20 2020 2020 2020 2020 2020 2023 204f  .            # O
+0001c280: 7065 6e47 4c20 6e65 6564 7320 746f 2062  penGL needs to b
+0001c290: 6520 656e 6162 6c65 6420 6f6e 206d 6163  e enabled on mac
+0001c2a0: 4f53 0a20 2020 2020 2020 2020 2020 2023  OS.            #
+0001c2b0: 2028 6874 7470 733a 2f2f 6769 7468 7562   (https://github
+0001c2c0: 2e63 6f6d 2f6d 6e65 2d74 6f6f 6c73 2f6d  .com/mne-tools/m
+0001c2d0: 6e65 2d71 742d 6272 6f77 7365 722f 6973  ne-qt-browser/is
+0001c2e0: 7375 6573 2f35 3329 0a20 2020 2020 2020  sues/53).       
+0001c2f0: 2020 2020 2064 6566 6175 6c74 203d 2027       default = '
+0001c300: 7472 7565 2720 6966 2070 6c61 7466 6f72  true' if platfor
+0001c310: 6d2e 7379 7374 656d 2829 203d 3d20 2744  m.system() == 'D
+0001c320: 6172 7769 6e27 2065 6c73 6520 2727 0a20  arwin' else ''. 
+0001c330: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+0001c340: 675f 7661 6c20 3d20 6765 745f 636f 6e66  g_val = get_conf
+0001c350: 6967 286f 7065 6e67 6c5f 6b65 792c 2064  ig(opengl_key, d
+0001c360: 6566 6175 6c74 292e 6c6f 7765 7228 290a  efault).lower().
+0001c370: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001c380: 2e6d 6e65 2e75 7365 5f6f 7065 6e67 6c20  .mne.use_opengl 
+0001c390: 3d20 2863 6f6e 6669 675f 7661 6c20 3d3d  = (config_val ==
+0001c3a0: 2027 7472 7565 2729 0a0a 2020 2020 2020   'true')..      
+0001c3b0: 2020 6966 2073 656c 662e 6d6e 652e 7573    if self.mne.us
+0001c3c0: 655f 6f70 656e 676c 3a0a 2020 2020 2020  e_opengl:.      
+0001c3d0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0001c3e0: 2020 2020 2020 2020 2020 2069 6d70 6f72             impor
+0001c3f0: 7420 4f70 656e 474c 0a20 2020 2020 2020  t OpenGL.       
+0001c400: 2020 2020 2065 7863 6570 7420 284d 6f64       except (Mod
+0001c410: 756c 654e 6f74 466f 756e 6445 7272 6f72  uleNotFoundError
+0001c420: 2c20 496d 706f 7274 4572 726f 7229 2061  , ImportError) a
+0001c430: 7320 6578 633a 0a20 2020 2020 2020 2020  s exc:.         
+0001c440: 2020 2020 2020 2023 204f 6e20 6d61 634f         # On macO
+0001c450: 532c 2069 6620 7573 655f 6f70 656e 676c  S, if use_opengl
+0001c460: 2069 7320 5472 7565 2077 6520 7261 6973   is True we rais
+0001c470: 6520 616e 2065 7272 6f72 2062 6563 6175  e an error becau
+0001c480: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+0001c490: 2020 2023 2069 7420 6361 6e20 6c65 6164     # it can lead
+0001c4a0: 2074 6f20 7365 6766 6175 6c74 732e 2049   to segfaults. I
+0001c4b0: 6620 6120 7573 6572 2072 6561 6c6c 7920  f a user really 
+0001c4c0: 6b6e 6f77 7320 7768 6174 2074 6865 790a  knows what they.
+0001c4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c4e0: 2320 6172 6520 646f 696e 672c 2074 6865  # are doing, the
+0001c4f0: 7920 6361 6e20 7061 7373 2075 7365 5f6f  y can pass use_o
+0001c500: 7065 6e67 6c3d 4661 6c73 6520 286f 7220  pengl=False (or 
+0001c510: 7365 740a 2020 2020 2020 2020 2020 2020  set.            
+0001c520: 2020 2020 2320 4d4e 455f 4252 4f57 5345      # MNE_BROWSE
+0001c530: 525f 5553 455f 4f50 454e 474c 3d66 616c  R_USE_OPENGL=fal
+0001c540: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+0001c550: 2020 2020 6966 2070 6c61 7466 6f72 6d2e      if platform.
+0001c560: 7379 7374 656d 2829 203d 3d20 2744 6172  system() == 'Dar
+0001c570: 7769 6e27 3a0a 2020 2020 2020 2020 2020  win':.          
+0001c580: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0001c590: 5275 6e74 696d 6545 7272 6f72 280a 2020  RuntimeError(.  
 0001c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c5b0: 2027 506c 6f74 7469 6e67 206f 6e20 6d61   'Plotting on ma
-0001c5c0: 634f 5320 7769 7468 6f75 7420 4f70 656e  cOS without Open
-0001c5d0: 474c 206d 6179 2062 6520 756e 7374 6162  GL may be unstab
-0001c5e0: 6c65 2120 270a 2020 2020 2020 2020 2020  le! '.          
-0001c5f0: 2020 2020 2020 2020 2020 2020 2020 2757                'W
-0001c600: 6520 7265 636f 6d6d 656e 6420 696e 7374  e recommend inst
-0001c610: 616c 6c69 6e67 2050 794f 7065 6e47 4c2c  alling PyOpenGL,
-0001c620: 2062 7574 2069 7420 636f 756c 6420 6e6f   but it could no
-0001c630: 7420 270a 2020 2020 2020 2020 2020 2020  t '.            
-0001c640: 2020 2020 2020 2020 2020 2020 6627 6265              f'be
-0001c650: 2069 6d70 6f72 7465 642c 2067 6f74 3a5c   imported, got:\
-0001c660: 6e7b 6578 637d 5c6e 5c6e 270a 2020 2020  n{exc}\n\n'.    
-0001c670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c680: 2020 2020 2749 6620 796f 7520 7761 6e74      'If you want
-0001c690: 2074 6f20 7472 7920 706c 6f74 7469 6e67   to try plotting
-0001c6a0: 2077 6974 686f 7574 204f 7065 6e47 4c2c   without OpenGL,
-0001c6b0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-0001c6c0: 2020 2020 2020 2020 2020 2027 796f 7520             'you 
-0001c6d0: 6361 6e20 7061 7373 2075 7365 5f6f 7065  can pass use_ope
-0001c6e0: 6e67 6c3d 4661 6c73 6520 2875 7365 2061  ngl=False (use a
-0001c6f0: 7420 796f 7572 206f 776e 2027 0a20 2020  t your own '.   
-0001c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c710: 2020 2020 2027 7269 736b 2129 2e20 4966       'risk!). If
-0001c720: 2079 6f75 206b 6e6f 7720 6e6f 6e2d 4f70   you know non-Op
-0001c730: 656e 474c 2070 6c6f 7474 696e 6720 6973  enGL plotting is
-0001c740: 2073 7461 626c 6520 270a 2020 2020 2020   stable '.      
+0001c5b0: 2020 2020 2020 2750 6c6f 7474 696e 6720        'Plotting 
+0001c5c0: 6f6e 206d 6163 4f53 2077 6974 686f 7574  on macOS without
+0001c5d0: 204f 7065 6e47 4c20 6d61 7920 6265 2075   OpenGL may be u
+0001c5e0: 6e73 7461 626c 6521 2027 0a20 2020 2020  nstable! '.     
+0001c5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c600: 2020 2027 5765 2072 6563 6f6d 6d65 6e64     'We recommend
+0001c610: 2069 6e73 7461 6c6c 696e 6720 5079 4f70   installing PyOp
+0001c620: 656e 474c 2c20 6275 7420 6974 2063 6f75  enGL, but it cou
+0001c630: 6c64 206e 6f74 2027 0a20 2020 2020 2020  ld not '.       
+0001c640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c650: 2066 2762 6520 696d 706f 7274 6564 2c20   f'be imported, 
+0001c660: 676f 743a 5c6e 7b65 7863 7d5c 6e5c 6e27  got:\n{exc}\n\n'
+0001c670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c680: 2020 2020 2020 2020 2027 4966 2079 6f75           'If you
+0001c690: 2077 616e 7420 746f 2074 7279 2070 6c6f   want to try plo
+0001c6a0: 7474 696e 6720 7769 7468 6f75 7420 4f70  tting without Op
+0001c6b0: 656e 474c 2c20 270a 2020 2020 2020 2020  enGL, '.        
+0001c6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c6d0: 2779 6f75 2063 616e 2070 6173 7320 7573  'you can pass us
+0001c6e0: 655f 6f70 656e 676c 3d46 616c 7365 2028  e_opengl=False (
+0001c6f0: 7573 6520 6174 2079 6f75 7220 6f77 6e20  use at your own 
+0001c700: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0001c710: 2020 2020 2020 2020 2020 2772 6973 6b21            'risk!
+0001c720: 292e 2049 6620 796f 7520 6b6e 6f77 206e  ). If you know n
+0001c730: 6f6e 2d4f 7065 6e47 4c20 706c 6f74 7469  on-OpenGL plotti
+0001c740: 6e67 2069 7320 7374 6162 6c65 2027 0a20  ng is stable '. 
 0001c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c760: 2020 276f 6e20 796f 7572 2073 7973 7465    'on your syste
-0001c770: 6d2c 2079 6f75 2063 616e 2061 6c73 6f20  m, you can also 
-0001c780: 7365 7420 7468 6520 636f 6e66 6967 2076  set the config v
-0001c790: 616c 7565 2027 0a20 2020 2020 2020 2020  alue '.         
-0001c7a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001c7b0: 277b 6f70 656e 676c 5f6b 6579 7d3d 6661  '{opengl_key}=fa
-0001c7c0: 6c73 6520 746f 2070 6572 6d61 6e65 6e74  lse to permanent
-0001c7d0: 6c79 2063 6861 6e67 6520 270a 2020 2020  ly change '.    
-0001c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c7f0: 2020 2020 2774 6865 2064 6566 6175 6c74      'the default
-0001c800: 2062 6568 6176 696f 7220 6f6e 2079 6f75   behavior on you
-0001c810: 7220 7379 7374 656d 2e27 2920 6672 6f6d  r system.') from
-0001c820: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0001c830: 2020 2020 2020 2320 6f74 6865 7277 6973        # otherwis
-0001c840: 652c 2065 6d69 7420 6120 7761 726e 696e  e, emit a warnin
-0001c850: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-0001c860: 2020 7761 726e 2827 5079 4f70 656e 474c    warn('PyOpenGL
-0001c870: 2077 6173 206e 6f74 2066 6f75 6e64 2061   was not found a
-0001c880: 6e64 204f 7065 6e47 4c20 6361 6e6e 6f74  nd OpenGL cannot
-0001c890: 2062 6520 7573 6564 2e20 270a 2020 2020   be used. '.    
-0001c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8b0: 2027 436f 6e73 6964 6572 2069 6e73 7461   'Consider insta
-0001c8c0: 6c6c 696e 6720 7079 6f70 656e 676c 2077  lling pyopengl w
-0001c8d0: 6974 6820 7069 7020 6f72 2063 6f6e 6461  ith pip or conda
-0001c8e0: 206f 7220 7365 7420 270a 2020 2020 2020   or set '.      
-0001c8f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0001c900: 2275 7365 5f6f 7065 6e67 6c3d 4661 6c73  "use_opengl=Fals
-0001c910: 6522 2074 6f20 6176 6f69 6420 7468 6973  e" to avoid this
-0001c920: 2077 6172 6e69 6e67 2e27 290a 2020 2020   warning.').    
-0001c930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001c940: 2e6d 6e65 2e75 7365 5f6f 7065 6e67 6c20  .mne.use_opengl 
-0001c950: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-0001c960: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001c970: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0001c980: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
-0001c990: 2020 2020 2020 2020 2020 2066 2755 7369             f'Usi
-0001c9a0: 6e67 2070 796f 7065 6e67 6c20 7769 7468  ng pyopengl with
-0001c9b0: 2076 6572 7369 6f6e 207b 4f70 656e 474c   version {OpenGL
-0001c9c0: 2e5f 5f76 6572 7369 6f6e 5f5f 7d27 290a  .__version__}').
-0001c9d0: 2020 2020 2020 2020 2320 496e 6974 6961          # Initia
-0001c9e0: 6c69 7a65 2042 726f 7773 6572 5669 6577  lize BrowserView
-0001c9f0: 2028 696e 6865 7269 7473 2051 4772 6170   (inherits QGrap
-0001ca00: 6869 6373 5669 6577 290a 2020 2020 2020  hicsView).      
-0001ca10: 2020 7365 6c66 2e6d 6e65 2e76 6965 7720    self.mne.view 
-0001ca20: 3d20 4272 6f77 7365 7256 6965 7728 7365  = BrowserView(se
-0001ca30: 6c66 2e6d 6e65 2e70 6c74 2c0a 2020 2020  lf.mne.plt,.    
-0001ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c760: 2020 2020 2020 2027 6f6e 2079 6f75 7220         'on your 
+0001c770: 7379 7374 656d 2c20 796f 7520 6361 6e20  system, you can 
+0001c780: 616c 736f 2073 6574 2074 6865 2063 6f6e  also set the con
+0001c790: 6669 6720 7661 6c75 6520 270a 2020 2020  fig value '.    
+0001c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c7b0: 2020 2020 6627 7b6f 7065 6e67 6c5f 6b65      f'{opengl_ke
+0001c7c0: 797d 3d66 616c 7365 2074 6f20 7065 726d  y}=false to perm
+0001c7d0: 616e 656e 746c 7920 6368 616e 6765 2027  anently change '
+0001c7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c7f0: 2020 2020 2020 2020 2027 7468 6520 6465           'the de
+0001c800: 6661 756c 7420 6265 6861 7669 6f72 206f  fault behavior o
+0001c810: 6e20 796f 7572 2073 7973 7465 6d2e 2729  n your system.')
+0001c820: 2066 726f 6d20 4e6f 6e65 0a20 2020 2020   from None.     
+0001c830: 2020 2020 2020 2020 2020 2023 206f 7468             # oth
+0001c840: 6572 7769 7365 2c20 656d 6974 2061 2077  erwise, emit a w
+0001c850: 6172 6e69 6e67 0a20 2020 2020 2020 2020  arning.         
+0001c860: 2020 2020 2020 2077 6172 6e28 2750 794f         warn('PyO
+0001c870: 7065 6e47 4c20 7761 7320 6e6f 7420 666f  penGL was not fo
+0001c880: 756e 6420 616e 6420 4f70 656e 474c 2063  und and OpenGL c
+0001c890: 616e 6e6f 7420 6265 2075 7365 642e 2027  annot be used. '
+0001c8a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c8b0: 2020 2020 2020 2743 6f6e 7369 6465 7220        'Consider 
+0001c8c0: 696e 7374 616c 6c69 6e67 2070 796f 7065  installing pyope
+0001c8d0: 6e67 6c20 7769 7468 2070 6970 206f 7220  ngl with pip or 
+0001c8e0: 636f 6e64 6120 6f72 2073 6574 2027 0a20  conda or set '. 
+0001c8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c900: 2020 2020 2722 7573 655f 6f70 656e 676c      '"use_opengl
+0001c910: 3d46 616c 7365 2220 746f 2061 766f 6964  =False" to avoid
+0001c920: 2074 6869 7320 7761 726e 696e 672e 2729   this warning.')
+0001c930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c940: 2073 656c 662e 6d6e 652e 7573 655f 6f70   self.mne.use_op
+0001c950: 656e 676c 203d 2046 616c 7365 0a20 2020  engl = False.   
+0001c960: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0001c970: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0001c980: 6f67 6765 722e 696e 666f 280a 2020 2020  ogger.info(.    
+0001c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c9a0: 6627 5573 696e 6720 7079 6f70 656e 676c  f'Using pyopengl
+0001c9b0: 2077 6974 6820 7665 7273 696f 6e20 7b4f   with version {O
+0001c9c0: 7065 6e47 4c2e 5f5f 7665 7273 696f 6e5f  penGL.__version_
+0001c9d0: 5f7d 2729 0a20 2020 2020 2020 2023 2049  _}').        # I
+0001c9e0: 6e69 7469 616c 697a 6520 4272 6f77 7365  nitialize Browse
+0001c9f0: 7256 6965 7720 2869 6e68 6572 6974 7320  rView (inherits 
+0001ca00: 5147 7261 7068 6963 7356 6965 7729 0a20  QGraphicsView). 
+0001ca10: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
+0001ca20: 7669 6577 203d 2042 726f 7773 6572 5669  view = BrowserVi
+0001ca30: 6577 2873 656c 662e 6d6e 652e 706c 742c  ew(self.mne.plt,
+0001ca40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0001ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ca60: 7573 654f 7065 6e47 4c3d 7365 6c66 2e6d  useOpenGL=self.m
-0001ca70: 6e65 2e75 7365 5f6f 7065 6e67 6c2c 0a20  ne.use_opengl,. 
-0001ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca60: 2020 2020 2075 7365 4f70 656e 474c 3d73       useOpenGL=s
+0001ca70: 656c 662e 6d6e 652e 7573 655f 6f70 656e  elf.mne.use_open
+0001ca80: 676c 2c0a 2020 2020 2020 2020 2020 2020  gl,.            
 0001ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001caa0: 2020 2062 6163 6b67 726f 756e 643d 2777     background='w
-0001cab0: 2729 0a20 2020 2020 2020 2062 6763 6f6c  ').        bgcol
-0001cac0: 6f72 203d 2067 6574 6174 7472 2873 656c  or = getattr(sel
-0001cad0: 662e 6d6e 652c 2027 6267 636f 6c6f 7227  f.mne, 'bgcolor'
-0001cae0: 2c20 2777 2729 0a20 2020 2020 2020 2073  , 'w').        s
-0001caf0: 656c 662e 6d6e 652e 7669 6577 2e73 6574  elf.mne.view.set
-0001cb00: 4261 636b 6772 6f75 6e64 285f 6765 745f  Background(_get_
-0001cb10: 636f 6c6f 7228 6267 636f 6c6f 722c 2073  color(bgcolor, s
-0001cb20: 656c 662e 6d6e 652e 6461 726b 2929 0a20  elf.mne.dark)). 
-0001cb30: 2020 2020 2020 206c 6179 6f75 742e 6164         layout.ad
-0001cb40: 6457 6964 6765 7428 7365 6c66 2e6d 6e65  dWidget(self.mne
-0001cb50: 2e76 6965 772c 2030 2c20 3029 0a0a 2020  .view, 0, 0)..  
-0001cb60: 2020 2020 2020 2320 496e 6974 6961 6c69        # Initiali
-0001cb70: 7a65 2053 6372 6f6c 6c2d 4261 7273 0a20  ze Scroll-Bars. 
-0001cb80: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-0001cb90: 6178 5f68 7363 726f 6c6c 203d 2054 696d  ax_hscroll = Tim
-0001cba0: 6553 6372 6f6c 6c42 6172 2873 656c 662e  eScrollBar(self.
-0001cbb0: 6d6e 6529 0a20 2020 2020 2020 206c 6179  mne).        lay
-0001cbc0: 6f75 742e 6164 6457 6964 6765 7428 7365  out.addWidget(se
-0001cbd0: 6c66 2e6d 6e65 2e61 785f 6873 6372 6f6c  lf.mne.ax_hscrol
-0001cbe0: 6c2c 2031 2c20 302c 2031 2c20 3229 0a0a  l, 1, 0, 1, 2)..
-0001cbf0: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
-0001cc00: 2e61 785f 7673 6372 6f6c 6c20 3d20 4368  .ax_vscroll = Ch
-0001cc10: 616e 6e65 6c53 6372 6f6c 6c42 6172 2873  annelScrollBar(s
-0001cc20: 656c 662e 6d6e 6529 0a20 2020 2020 2020  elf.mne).       
-0001cc30: 206c 6179 6f75 742e 6164 6457 6964 6765   layout.addWidge
-0001cc40: 7428 7365 6c66 2e6d 6e65 2e61 785f 7673  t(self.mne.ax_vs
-0001cc50: 6372 6f6c 6c2c 2030 2c20 3129 0a0a 2020  croll, 0, 1)..  
-0001cc60: 2020 2020 2020 2320 496e 6974 6961 6c69        # Initiali
-0001cc70: 7a65 2056 4c69 6e65 0a20 2020 2020 2020  ze VLine.       
-0001cc80: 2073 656c 662e 6d6e 652e 766c 696e 6520   self.mne.vline 
-0001cc90: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-0001cca0: 656c 662e 6d6e 652e 766c 696e 655f 7669  elf.mne.vline_vi
-0001ccb0: 7369 626c 6520 3d20 4661 6c73 650a 0a20  sible = False.. 
-0001ccc0: 2020 2020 2020 2023 2049 6e69 7469 616c         # Initial
-0001ccd0: 697a 6520 6372 6f73 7368 6169 7220 2861  ize crosshair (a
-0001cce0: 7320 696e 2070 7971 7467 7261 7068 2065  s in pyqtgraph e
-0001ccf0: 7861 6d70 6c65 290a 2020 2020 2020 2020  xample).        
-0001cd00: 7365 6c66 2e6d 6e65 2e63 726f 7373 6861  self.mne.crossha
-0001cd10: 6972 5f65 6e61 626c 6564 203d 2046 616c  ir_enabled = Fal
-0001cd20: 7365 0a20 2020 2020 2020 2073 656c 662e  se.        self.
-0001cd30: 6d6e 652e 6372 6f73 7368 6169 725f 6820  mne.crosshair_h 
-0001cd40: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-0001cd50: 656c 662e 6d6e 652e 6372 6f73 7368 6169  elf.mne.crosshai
-0001cd60: 7220 3d20 4e6f 6e65 0a20 2020 2020 2020  r = None.       
-0001cd70: 2073 656c 662e 6d6e 652e 7669 6577 2e73   self.mne.view.s
-0001cd80: 6967 5363 656e 654d 6f75 7365 4d6f 7665  igSceneMouseMove
-0001cd90: 642e 636f 6e6e 6563 7428 7365 6c66 2e5f  d.connect(self._
-0001cda0: 6d6f 7573 655f 6d6f 7665 6429 0a0a 2020  mouse_moved)..  
-0001cdb0: 2020 2020 2020 2320 496e 6974 6961 6c69        # Initiali
-0001cdc0: 7a65 2041 6e6e 6f74 6174 696f 6e2d 5769  ze Annotation-Wi
-0001cdd0: 6467 6574 730a 2020 2020 2020 2020 7365  dgets.        se
-0001cde0: 6c66 2e6d 6e65 2e61 6e6e 6f74 6174 696f  lf.mne.annotatio
-0001cdf0: 6e5f 6d6f 6465 203d 2046 616c 7365 0a20  n_mode = False. 
-0001ce00: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0001ce10: 6c66 2e6d 6e65 2e69 735f 6570 6f63 6873  lf.mne.is_epochs
-0001ce20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0001ce30: 6c66 2e5f 696e 6974 5f61 6e6e 6f74 5f6d  lf._init_annot_m
-0001ce40: 6f64 6528 290a 0a20 2020 2020 2020 2023  ode()..        #
-0001ce50: 204f 7665 7276 6965 7742 6172 0a20 2020   OverviewBar.   
-0001ce60: 2020 2020 2073 656c 662e 6d6e 652e 6f76       self.mne.ov
-0001ce70: 6572 7669 6577 5f62 6172 203d 204f 7665  erview_bar = Ove
-0001ce80: 7276 6965 7742 6172 2873 656c 6629 0a20  rviewBar(self). 
-0001ce90: 2020 2020 2020 206c 6179 6f75 742e 6164         layout.ad
-0001cea0: 6457 6964 6765 7428 7365 6c66 2e6d 6e65  dWidget(self.mne
-0001ceb0: 2e6f 7665 7276 6965 775f 6261 722c 2032  .overview_bar, 2
-0001cec0: 2c20 302c 2031 2c20 3229 0a0a 2020 2020  , 0, 1, 2)..    
-0001ced0: 2020 2020 7769 6467 6574 2e73 6574 4c61      widget.setLa
-0001cee0: 796f 7574 286c 6179 6f75 7429 0a20 2020  yout(layout).   
-0001cef0: 2020 2020 2073 656c 662e 7365 7443 656e       self.setCen
-0001cf00: 7472 616c 5769 6467 6574 2877 6964 6765  tralWidget(widge
-0001cf10: 7429 0a0a 2020 2020 2020 2020 2320 496e  t)..        # In
-0001cf20: 6974 6961 6c69 7a65 2053 656c 6563 7469  itialize Selecti
-0001cf30: 6f6e 2d44 6961 6c6f 670a 2020 2020 2020  on-Dialog.      
-0001cf40: 2020 6966 2067 6574 6174 7472 2873 656c    if getattr(sel
-0001cf50: 662e 6d6e 652c 2027 6772 6f75 705f 6279  f.mne, 'group_by
-0001cf60: 272c 204e 6f6e 6529 2069 6e20 5b27 706f  ', None) in ['po
-0001cf70: 7369 7469 6f6e 272c 2027 7365 6c65 6374  sition', 'select
-0001cf80: 696f 6e27 5d3a 0a20 2020 2020 2020 2020  ion']:.         
-0001cf90: 2020 2073 656c 662e 5f63 7265 6174 655f     self._create_
-0001cfa0: 7365 6c65 6374 696f 6e5f 6669 6728 290a  selection_fig().
-0001cfb0: 0a20 2020 2020 2020 2023 2049 6e69 7469  .        # Initi
-0001cfc0: 616c 697a 6520 5072 6f6a 6563 746f 7273  alize Projectors
-0001cfd0: 2d44 6961 6c6f 6720 6966 2073 686f 775f  -Dialog if show_
-0001cfe0: 6f70 7469 6f6e 733d 5472 7565 0a20 2020  options=True.   
-0001cff0: 2020 2020 2069 6620 6765 7461 7474 7228       if getattr(
-0001d000: 7365 6c66 2e6d 6e65 2c20 2773 686f 775f  self.mne, 'show_
-0001d010: 6f70 7469 6f6e 7327 2c20 4661 6c73 6529  options', False)
-0001d020: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0001d030: 6c66 2e5f 746f 6767 6c65 5f70 726f 6a5f  lf._toggle_proj_
-0001d040: 6669 6728 290a 0a20 2020 2020 2020 2023  fig()..        #
-0001d050: 2049 6e69 7469 616c 697a 6520 546f 6f6c   Initialize Tool
-0001d060: 6261 720a 2020 2020 2020 2020 7365 6c66  bar.        self
-0001d070: 2e6d 6e65 2e74 6f6f 6c62 6172 203d 2073  .mne.toolbar = s
-0001d080: 656c 662e 6164 6454 6f6f 6c42 6172 2827  elf.addToolBar('
-0001d090: 546f 6f6c 7327 290a 2020 2020 2020 2020  Tools').        
-0001d0a0: 2320 746f 6f6c 5f62 7574 746f 6e5f 7374  # tool_button_st
-0001d0b0: 796c 6520 3d20 5174 2e54 6f6f 6c42 7574  yle = Qt.ToolBut
-0001d0c0: 746f 6e54 6578 7442 6573 6964 6549 636f  tonTextBesideIco
-0001d0d0: 6e0a 2020 2020 2020 2020 746f 6f6c 5f62  n.        tool_b
-0001d0e0: 7574 746f 6e5f 7374 796c 6520 3d20 5174  utton_style = Qt
-0001d0f0: 2e54 6f6f 6c42 7574 746f 6e49 636f 6e4f  .ToolButtonIconO
-0001d100: 6e6c 790a 2020 2020 2020 2020 7365 6c66  nly.        self
-0001d110: 2e6d 6e65 2e74 6f6f 6c62 6172 2e73 6574  .mne.toolbar.set
-0001d120: 546f 6f6c 4275 7474 6f6e 5374 796c 6528  ToolButtonStyle(
-0001d130: 746f 6f6c 5f62 7574 746f 6e5f 7374 796c  tool_button_styl
-0001d140: 6529 0a0a 2020 2020 2020 2020 6164 6563  e)..        adec
-0001d150: 725f 7469 6d65 203d 2051 4163 7469 6f6e  r_time = QAction
-0001d160: 280a 2020 2020 2020 2020 2020 2020 5149  (.            QI
-0001d170: 636f 6e2e 6672 6f6d 5468 656d 6528 226c  con.fromTheme("l
-0001d180: 6573 735f 7469 6d65 2229 2c20 272d 2054  ess_time"), '- T
-0001d190: 696d 6527 2c20 7061 7265 6e74 3d73 656c  ime', parent=sel
-0001d1a0: 6629 0a20 2020 2020 2020 2061 6465 6372  f).        adecr
-0001d1b0: 5f74 696d 652e 7472 6967 6765 7265 642e  _time.triggered.
-0001d1c0: 636f 6e6e 6563 7428 0a20 2020 2020 2020  connect(.       
-0001d1d0: 2020 2020 205f 6d65 7468 7061 7274 6961       _methpartia
-0001d1e0: 6c28 7365 6c66 2e63 6861 6e67 655f 6475  l(self.change_du
-0001d1f0: 7261 7469 6f6e 2c20 7374 6570 3d2d 302e  ration, step=-0.
-0001d200: 3229 290a 2020 2020 2020 2020 7365 6c66  2)).        self
-0001d210: 2e6d 6e65 2e74 6f6f 6c62 6172 2e61 6464  .mne.toolbar.add
-0001d220: 4163 7469 6f6e 2861 6465 6372 5f74 696d  Action(adecr_tim
-0001d230: 6529 0a20 2020 2020 2020 2061 696e 6372  e).        aincr
-0001d240: 5f74 696d 6520 3d20 5141 6374 696f 6e28  _time = QAction(
-0001d250: 0a20 2020 2020 2020 2020 2020 2051 4963  .            QIc
-0001d260: 6f6e 2e66 726f 6d54 6865 6d65 2822 6d6f  on.fromTheme("mo
-0001d270: 7265 5f74 696d 6522 292c 2027 2b20 5469  re_time"), '+ Ti
-0001d280: 6d65 272c 2070 6172 656e 743d 7365 6c66  me', parent=self
-0001d290: 290a 2020 2020 2020 2020 6169 6e63 725f  ).        aincr_
-0001d2a0: 7469 6d65 2e74 7269 6767 6572 6564 2e63  time.triggered.c
-0001d2b0: 6f6e 6e65 6374 280a 2020 2020 2020 2020  onnect(.        
-0001d2c0: 2020 2020 5f6d 6574 6870 6172 7469 616c      _methpartial
-0001d2d0: 2873 656c 662e 6368 616e 6765 5f64 7572  (self.change_dur
-0001d2e0: 6174 696f 6e2c 2073 7465 703d 302e 3235  ation, step=0.25
-0001d2f0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0001d300: 6d6e 652e 746f 6f6c 6261 722e 6164 6441  mne.toolbar.addA
-0001d310: 6374 696f 6e28 6169 6e63 725f 7469 6d65  ction(aincr_time
-0001d320: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
-0001d330: 6e65 2e74 6f6f 6c62 6172 2e61 6464 5365  ne.toolbar.addSe
-0001d340: 7061 7261 746f 7228 290a 0a20 2020 2020  parator()..     
-0001d350: 2020 2061 6465 6372 5f6e 6368 616e 203d     adecr_nchan =
-0001d360: 2051 4163 7469 6f6e 280a 2020 2020 2020   QAction(.      
-0001d370: 2020 2020 2020 5149 636f 6e2e 6672 6f6d        QIcon.from
-0001d380: 5468 656d 6528 226c 6573 735f 6368 616e  Theme("less_chan
-0001d390: 6e65 6c73 2229 2c20 272d 2043 6861 6e6e  nels"), '- Chann
-0001d3a0: 656c 7327 2c20 7061 7265 6e74 3d73 656c  els', parent=sel
-0001d3b0: 6629 0a20 2020 2020 2020 2061 6465 6372  f).        adecr
-0001d3c0: 5f6e 6368 616e 2e74 7269 6767 6572 6564  _nchan.triggered
-0001d3d0: 2e63 6f6e 6e65 6374 280a 2020 2020 2020  .connect(.      
-0001d3e0: 2020 2020 2020 5f6d 6574 6870 6172 7469        _methparti
-0001d3f0: 616c 2873 656c 662e 6368 616e 6765 5f6e  al(self.change_n
-0001d400: 6368 616e 2c20 7374 6570 3d2d 3130 2929  chan, step=-10))
-0001d410: 0a20 2020 2020 2020 2073 656c 662e 6d6e  .        self.mn
-0001d420: 652e 746f 6f6c 6261 722e 6164 6441 6374  e.toolbar.addAct
-0001d430: 696f 6e28 6164 6563 725f 6e63 6861 6e29  ion(adecr_nchan)
-0001d440: 0a20 2020 2020 2020 2061 696e 6372 5f6e  .        aincr_n
-0001d450: 6368 616e 203d 2051 4163 7469 6f6e 280a  chan = QAction(.
-0001d460: 2020 2020 2020 2020 2020 2020 5149 636f              QIco
-0001d470: 6e2e 6672 6f6d 5468 656d 6528 226d 6f72  n.fromTheme("mor
-0001d480: 655f 6368 616e 6e65 6c73 2229 2c20 272b  e_channels"), '+
-0001d490: 2043 6861 6e6e 656c 7327 2c20 7061 7265   Channels', pare
-0001d4a0: 6e74 3d73 656c 6629 0a20 2020 2020 2020  nt=self).       
-0001d4b0: 2061 696e 6372 5f6e 6368 616e 2e74 7269   aincr_nchan.tri
-0001d4c0: 6767 6572 6564 2e63 6f6e 6e65 6374 280a  ggered.connect(.
-0001d4d0: 2020 2020 2020 2020 2020 2020 5f6d 6574              _met
-0001d4e0: 6870 6172 7469 616c 2873 656c 662e 6368  hpartial(self.ch
-0001d4f0: 616e 6765 5f6e 6368 616e 2c20 7374 6570  ange_nchan, step
-0001d500: 3d31 3029 290a 2020 2020 2020 2020 7365  =10)).        se
-0001d510: 6c66 2e6d 6e65 2e74 6f6f 6c62 6172 2e61  lf.mne.toolbar.a
-0001d520: 6464 4163 7469 6f6e 2861 696e 6372 5f6e  ddAction(aincr_n
-0001d530: 6368 616e 290a 2020 2020 2020 2020 7365  chan).        se
-0001d540: 6c66 2e6d 6e65 2e74 6f6f 6c62 6172 2e61  lf.mne.toolbar.a
-0001d550: 6464 5365 7061 7261 746f 7228 290a 0a20  ddSeparator().. 
-0001d560: 2020 2020 2020 2061 6465 6372 5f6e 6368         adecr_nch
-0001d570: 616e 203d 2051 4163 7469 6f6e 280a 2020  an = QAction(.  
-0001d580: 2020 2020 2020 2020 2020 5149 636f 6e2e            QIcon.
-0001d590: 6672 6f6d 5468 656d 6528 227a 6f6f 6d5f  fromTheme("zoom_
-0001d5a0: 6f75 7422 292c 2027 5a6f 6f6d 206f 7574  out"), 'Zoom out
-0001d5b0: 272c 2070 6172 656e 743d 7365 6c66 290a  ', parent=self).
-0001d5c0: 2020 2020 2020 2020 6164 6563 725f 6e63          adecr_nc
-0001d5d0: 6861 6e2e 7472 6967 6765 7265 642e 636f  han.triggered.co
-0001d5e0: 6e6e 6563 7428 0a20 2020 2020 2020 2020  nnect(.         
-0001d5f0: 2020 205f 6d65 7468 7061 7274 6961 6c28     _methpartial(
-0001d600: 7365 6c66 2e73 6361 6c65 5f61 6c6c 2c20  self.scale_all, 
-0001d610: 7374 6570 3d34 202f 2035 2929 0a20 2020  step=4 / 5)).   
-0001d620: 2020 2020 2073 656c 662e 6d6e 652e 746f       self.mne.to
-0001d630: 6f6c 6261 722e 6164 6441 6374 696f 6e28  olbar.addAction(
-0001d640: 6164 6563 725f 6e63 6861 6e29 0a20 2020  adecr_nchan).   
-0001d650: 2020 2020 2061 696e 6372 5f6e 6368 616e       aincr_nchan
-0001d660: 203d 2051 4163 7469 6f6e 280a 2020 2020   = QAction(.    
-0001d670: 2020 2020 2020 2020 5149 636f 6e2e 6672          QIcon.fr
-0001d680: 6f6d 5468 656d 6528 227a 6f6f 6d5f 696e  omTheme("zoom_in
-0001d690: 2229 2c20 275a 6f6f 6d20 696e 272c 2070  "), 'Zoom in', p
-0001d6a0: 6172 656e 743d 7365 6c66 290a 2020 2020  arent=self).    
-0001d6b0: 2020 2020 6169 6e63 725f 6e63 6861 6e2e      aincr_nchan.
-0001d6c0: 7472 6967 6765 7265 642e 636f 6e6e 6563  triggered.connec
-0001d6d0: 7428 0a20 2020 2020 2020 2020 2020 205f  t(.            _
-0001d6e0: 6d65 7468 7061 7274 6961 6c28 7365 6c66  methpartial(self
-0001d6f0: 2e73 6361 6c65 5f61 6c6c 2c20 7374 6570  .scale_all, step
-0001d700: 3d35 202f 2034 2929 0a20 2020 2020 2020  =5 / 4)).       
-0001d710: 2073 656c 662e 6d6e 652e 746f 6f6c 6261   self.mne.toolba
-0001d720: 722e 6164 6441 6374 696f 6e28 6169 6e63  r.addAction(ainc
-0001d730: 725f 6e63 6861 6e29 0a20 2020 2020 2020  r_nchan).       
-0001d740: 2073 656c 662e 6d6e 652e 746f 6f6c 6261   self.mne.toolba
-0001d750: 722e 6164 6453 6570 6172 6174 6f72 2829  r.addSeparator()
-0001d760: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-0001d770: 2073 656c 662e 6d6e 652e 6973 5f65 706f   self.mne.is_epo
-0001d780: 6368 733a 0a20 2020 2020 2020 2020 2020  chs:.           
-0001d790: 2061 746f 6767 6c65 5f61 6e6e 6f74 203d   atoggle_annot =
-0001d7a0: 2051 4163 7469 6f6e 280a 2020 2020 2020   QAction(.      
-0001d7b0: 2020 2020 2020 2020 2020 5149 636f 6e2e            QIcon.
-0001d7c0: 6672 6f6d 5468 656d 6528 2261 6e6e 6f74  fromTheme("annot
-0001d7d0: 6174 696f 6e73 2229 2c20 2741 6e6e 6f74  ations"), 'Annot
-0001d7e0: 6174 696f 6e73 272c 2070 6172 656e 743d  ations', parent=
-0001d7f0: 7365 6c66 290a 2020 2020 2020 2020 2020  self).          
-0001d800: 2020 6174 6f67 676c 655f 616e 6e6f 742e    atoggle_annot.
-0001d810: 7472 6967 6765 7265 642e 636f 6e6e 6563  triggered.connec
-0001d820: 7428 7365 6c66 2e5f 746f 6767 6c65 5f61  t(self._toggle_a
-0001d830: 6e6e 6f74 6174 696f 6e5f 6669 6729 0a20  nnotation_fig). 
-0001d840: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001d850: 6d6e 652e 746f 6f6c 6261 722e 6164 6441  mne.toolbar.addA
-0001d860: 6374 696f 6e28 6174 6f67 676c 655f 616e  ction(atoggle_an
-0001d870: 6e6f 7429 0a0a 2020 2020 2020 2020 6174  not)..        at
-0001d880: 6f67 676c 655f 7072 6f6a 203d 2051 4163  oggle_proj = QAc
-0001d890: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-0001d8a0: 2020 5149 636f 6e2e 6672 6f6d 5468 656d    QIcon.fromThem
-0001d8b0: 6528 2273 7370 2229 2c20 2753 5350 272c  e("ssp"), 'SSP',
-0001d8c0: 2070 6172 656e 743d 7365 6c66 290a 2020   parent=self).  
-0001d8d0: 2020 2020 2020 6174 6f67 676c 655f 7072        atoggle_pr
-0001d8e0: 6f6a 2e74 7269 6767 6572 6564 2e63 6f6e  oj.triggered.con
-0001d8f0: 6e65 6374 2873 656c 662e 5f74 6f67 676c  nect(self._toggl
-0001d900: 655f 7072 6f6a 5f66 6967 290a 2020 2020  e_proj_fig).    
-0001d910: 2020 2020 7365 6c66 2e6d 6e65 2e74 6f6f      self.mne.too
-0001d920: 6c62 6172 2e61 6464 4163 7469 6f6e 2861  lbar.addAction(a
-0001d930: 746f 6767 6c65 5f70 726f 6a29 0a0a 2020  toggle_proj)..  
-0001d940: 2020 2020 2020 6275 7474 6f6e 203d 2051        button = Q
-0001d950: 546f 6f6c 4275 7474 6f6e 2873 656c 662e  ToolButton(self.
-0001d960: 6d6e 652e 746f 6f6c 6261 7229 0a20 2020  mne.toolbar).   
-0001d970: 2020 2020 2062 7574 746f 6e2e 7365 7454       button.setT
-0001d980: 6f6f 6c54 6970 280a 2020 2020 2020 2020  oolTip(.        
-0001d990: 2020 2020 273c 6832 3e4f 7665 7276 6965      '<h2>Overvie
-0001d9a0: 772d 4d6f 6465 733c 2f68 323e 270a 2020  w-Modes</h2>'.  
-0001d9b0: 2020 2020 2020 2020 2020 273c 756c 3e27            '<ul>'
-0001d9c0: 0a20 2020 2020 2020 2020 2020 2027 3c6c  .            '<l
-0001d9d0: 693e 656d 7074 793a 3c62 723e 270a 2020  i>empty:<br>'.  
-0001d9e0: 2020 2020 2020 2020 2020 2744 6973 706c            'Displ
-0001d9f0: 6179 206e 6f20 6261 636b 6772 6f75 6e64  ay no background
-0001da00: 2e3c 2f6c 693e 270a 2020 2020 2020 2020  .</li>'.        
-0001da10: 2020 2020 273c 6c69 3e63 6861 6e6e 656c      '<li>channel
-0001da20: 733a 3c62 723e 270a 2020 2020 2020 2020  s:<br>'.        
-0001da30: 2020 2020 2744 6973 706c 6179 2065 6163      'Display eac
-0001da40: 6820 6368 616e 6e65 6c20 7769 7468 2069  h channel with i
-0001da50: 7473 2063 6861 6e6e 656c 2d74 7970 6520  ts channel-type 
-0001da60: 636f 6c6f 722e 3c2f 6c69 3e27 0a20 2020  color.</li>'.   
-0001da70: 2020 2020 2020 2020 2027 3c6c 693e 7a73           '<li>zs
-0001da80: 636f 7265 3a3c 6272 3e27 0a20 2020 2020  core:<br>'.     
-0001da90: 2020 2020 2020 2027 4469 7370 6c61 7920         'Display 
-0001daa0: 7468 6520 7a73 636f 7265 2066 6f72 2074  the zscore for t
-0001dab0: 6865 2064 6174 6120 6672 6f6d 2065 6163  he data from eac
-0001dac0: 6820 6368 616e 6e65 6c20 6163 726f 7373  h channel across
-0001dad0: 2074 696d 652e 2027 0a20 2020 2020 2020   time. '.       
-0001dae0: 2020 2020 2027 5265 6420 696e 6469 6361       'Red indica
-0001daf0: 7465 7320 6869 6768 207a 7363 6f72 6573  tes high zscores
-0001db00: 2c20 626c 7565 2069 6e64 6963 6174 6573  , blue indicates
-0001db10: 206c 6f77 207a 7363 6f72 6573 2c20 270a   low zscores, '.
-0001db20: 2020 2020 2020 2020 2020 2020 2761 6e64              'and
-0001db30: 2074 6865 2062 6f75 6e64 6172 6965 7320   the boundaries 
-0001db40: 6f66 2074 6865 2063 6f6c 6f72 2067 7261  of the color gra
-0001db50: 6469 656e 7420 6172 6520 6465 6669 6e65  dient are define
-0001db60: 6420 6279 2074 6865 2027 0a20 2020 2020  d by the '.     
-0001db70: 2020 2020 2020 2027 6d69 6e69 6d75 6d2f         'minimum/
-0001db80: 6d61 7869 6d75 6d20 7a73 636f 7265 2e27  maximum zscore.'
-0001db90: 0a20 2020 2020 2020 2020 2020 2027 5468  .            'Th
-0001dba0: 6973 206f 6e6c 7920 776f 726b 7320 6966  is only works if
-0001dbb0: 2070 7265 636f 6d70 7574 6520 6973 2073   precompute is s
-0001dbc0: 6574 2074 6f20 2254 7275 6522 2c20 6f72  et to "True", or
-0001dbd0: 2069 6620 6974 2069 7320 270a 2020 2020   if it is '.    
-0001dbe0: 2020 2020 2020 2020 2765 6e61 626c 6564          'enabled
-0001dbf0: 2077 6974 6820 2261 7574 6f22 2061 6e64   with "auto" and
-0001dc00: 2065 6e6f 7567 6820 6672 6565 2052 414d   enough free RAM
-0001dc10: 2069 7320 6176 6169 6c61 626c 652e 3c2f   is available.</
-0001dc20: 6c69 3e27 0a20 2020 2020 2020 2020 2020  li>'.           
-0001dc30: 2029 0a20 2020 2020 2020 2062 7574 746f   ).        butto
-0001dc40: 6e2e 7365 7454 6578 7428 274f 7665 7276  n.setText('Overv
-0001dc50: 6965 7720 4261 7227 290a 2020 2020 2020  iew Bar').      
-0001dc60: 2020 6275 7474 6f6e 2e73 6574 4963 6f6e    button.setIcon
-0001dc70: 2851 4963 6f6e 2e66 726f 6d54 6865 6d65  (QIcon.fromTheme
-0001dc80: 2827 6f76 6572 7669 6577 5f62 6172 2729  ('overview_bar')
-0001dc90: 290a 2020 2020 2020 2020 6275 7474 6f6e  ).        button
-0001dca0: 2e73 6574 546f 6f6c 4275 7474 6f6e 5374  .setToolButtonSt
-0001dcb0: 796c 6528 746f 6f6c 5f62 7574 746f 6e5f  yle(tool_button_
-0001dcc0: 7374 796c 6529 0a20 2020 2020 2020 206d  style).        m
-0001dcd0: 656e 7520 3d20 7365 6c66 2e6d 6e65 2e6f  enu = self.mne.o
-0001dce0: 7665 7276 6965 775f 6d65 6e75 203d 2051  verview_menu = Q
-0001dcf0: 4d65 6e75 2862 7574 746f 6e29 0a20 2020  Menu(button).   
-0001dd00: 2020 2020 2067 726f 7570 203d 2051 4163       group = QAc
-0001dd10: 7469 6f6e 4772 6f75 7028 6d65 6e75 290a  tionGroup(menu).
-0001dd20: 2020 2020 2020 2020 666f 7220 6b65 792c          for key,
-0001dd30: 2074 6578 7420 696e 206f 7665 7276 6965   text in overvie
-0001dd40: 775f 6974 656d 732e 6974 656d 7328 293a  w_items.items():
-0001dd50: 0a20 2020 2020 2020 2020 2020 2072 6164  .            rad
-0001dd60: 696f 203d 2051 5261 6469 6f42 7574 746f  io = QRadioButto
-0001dd70: 6e28 6d65 6e75 290a 2020 2020 2020 2020  n(menu).        
-0001dd80: 2020 2020 7261 6469 6f2e 7365 7454 6578      radio.setTex
-0001dd90: 7428 7465 7874 290a 2020 2020 2020 2020  t(text).        
-0001dda0: 2020 2020 6966 206b 6579 203d 3d20 7365      if key == se
-0001ddb0: 6c66 2e6d 6e65 2e6f 7665 7276 6965 775f  lf.mne.overview_
-0001ddc0: 6d6f 6465 3a0a 2020 2020 2020 2020 2020  mode:.          
-0001ddd0: 2020 2020 2020 7261 6469 6f2e 7365 7443        radio.setC
-0001dde0: 6865 636b 6564 2854 7275 6529 0a20 2020  hecked(True).   
-0001ddf0: 2020 2020 2020 2020 2061 6374 696f 6e20           action 
-0001de00: 3d20 5157 6964 6765 7441 6374 696f 6e28  = QWidgetAction(
-0001de10: 6d65 6e75 290a 2020 2020 2020 2020 2020  menu).          
-0001de20: 2020 6163 7469 6f6e 2e73 6574 4465 6661    action.setDefa
-0001de30: 756c 7457 6964 6765 7428 7261 6469 6f29  ultWidget(radio)
-0001de40: 0a20 2020 2020 2020 2020 2020 206d 656e  .            men
-0001de50: 752e 6164 6441 6374 696f 6e28 6163 7469  u.addAction(acti
-0001de60: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
-0001de70: 6772 6f75 702e 6164 6441 6374 696f 6e28  group.addAction(
-0001de80: 6163 7469 6f6e 290a 2020 2020 2020 2020  action).        
-0001de90: 2020 2020 7261 6469 6f2e 636c 6963 6b65      radio.clicke
-0001dea0: 642e 636f 6e6e 6563 7428 0a20 2020 2020  d.connect(.     
-0001deb0: 2020 2020 2020 2020 2020 205f 6d65 7468             _meth
-0001dec0: 7061 7274 6961 6c28 0a20 2020 2020 2020  partial(.       
-0001ded0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001dee0: 662e 5f6f 7665 7276 6965 775f 7261 6469  f._overview_radi
-0001def0: 6f5f 636c 6963 6b65 642c 206d 656e 753d  o_clicked, menu=
-0001df00: 6d65 6e75 2c20 6e65 775f 6d6f 6465 3d6b  menu, new_mode=k
-0001df10: 6579 2929 0a20 2020 2020 2020 206d 656e  ey)).        men
-0001df20: 752e 6164 6453 6570 6172 6174 6f72 2829  u.addSeparator()
-0001df30: 0a20 2020 2020 2020 2076 6973 6962 6c65  .        visible
-0001df40: 203d 2051 4163 7469 6f6e 2827 5669 7369   = QAction('Visi
-0001df50: 626c 6527 2c20 7061 7265 6e74 3d6d 656e  ble', parent=men
-0001df60: 7529 0a20 2020 2020 2020 206d 656e 752e  u).        menu.
-0001df70: 6164 6441 6374 696f 6e28 7669 7369 626c  addAction(visibl
-0001df80: 6529 0a20 2020 2020 2020 2076 6973 6962  e).        visib
-0001df90: 6c65 2e73 6574 4368 6563 6b61 626c 6528  le.setCheckable(
-0001dfa0: 5472 7565 290a 2020 2020 2020 2020 7669  True).        vi
-0001dfb0: 7369 626c 652e 7365 7443 6865 636b 6564  sible.setChecked
-0001dfc0: 2854 7275 6529 0a20 2020 2020 2020 2073  (True).        s
-0001dfd0: 656c 662e 6d6e 652e 6f76 6572 7669 6577  elf.mne.overview
-0001dfe0: 5f62 6172 2e73 6574 5669 7369 626c 6528  _bar.setVisible(
-0001dff0: 5472 7565 290a 2020 2020 2020 2020 7669  True).        vi
-0001e000: 7369 626c 652e 7472 6967 6765 7265 642e  sible.triggered.
-0001e010: 636f 6e6e 6563 7428 7365 6c66 2e5f 746f  connect(self._to
-0001e020: 6767 6c65 5f6f 7665 7276 6965 775f 6261  ggle_overview_ba
-0001e030: 7229 0a20 2020 2020 2020 2069 6620 6869  r).        if hi
-0001e040: 6465 5f6f 7665 7276 6965 773a 0a20 2020  de_overview:.   
-0001e050: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
-0001e060: 646f 6573 6e27 7420 776f 726b 2062 6563  doesn't work bec
-0001e070: 6175 7365 2069 7420 6861 736e 2774 2062  ause it hasn't b
-0001e080: 6565 6e20 7368 6f77 6e20 7965 743a 0a20  een shown yet:. 
-0001e090: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
-0001e0a0: 662e 5f74 6f67 676c 655f 6f76 6572 7669  f._toggle_overvi
-0001e0b0: 6577 5f62 6172 2829 0a20 2020 2020 2020  ew_bar().       
-0001e0c0: 2020 2020 2076 6973 6962 6c65 2e73 6574       visible.set
-0001e0d0: 4368 6563 6b65 6428 4661 6c73 6529 0a20  Checked(False). 
-0001e0e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001e0f0: 6d6e 652e 6f76 6572 7669 6577 5f62 6172  mne.overview_bar
-0001e100: 2e73 6574 5669 7369 626c 6528 4661 6c73  .setVisible(Fals
-0001e110: 6529 0a20 2020 2020 2020 2062 7574 746f  e).        butto
-0001e120: 6e2e 7365 744d 656e 7528 7365 6c66 2e6d  n.setMenu(self.m
-0001e130: 6e65 2e6f 7665 7276 6965 775f 6d65 6e75  ne.overview_menu
-0001e140: 290a 2020 2020 2020 2020 6275 7474 6f6e  ).        button
-0001e150: 2e73 6574 506f 7075 704d 6f64 6528 5154  .setPopupMode(QT
-0001e160: 6f6f 6c42 7574 746f 6e2e 496e 7374 616e  oolButton.Instan
-0001e170: 7450 6f70 7570 290a 2020 2020 2020 2020  tPopup).        
-0001e180: 7365 6c66 2e6d 6e65 2e74 6f6f 6c62 6172  self.mne.toolbar
-0001e190: 2e61 6464 5769 6467 6574 2862 7574 746f  .addWidget(butto
-0001e1a0: 6e29 0a0a 2020 2020 2020 2020 7365 6c66  n)..        self
-0001e1b0: 2e6d 6e65 2e74 6f6f 6c62 6172 2e61 6464  .mne.toolbar.add
-0001e1c0: 5365 7061 7261 746f 7228 290a 0a20 2020  Separator()..   
-0001e1d0: 2020 2020 2061 7365 7474 696e 6773 203d       asettings =
-0001e1e0: 2051 4163 7469 6f6e 2851 4963 6f6e 2e66   QAction(QIcon.f
-0001e1f0: 726f 6d54 6865 6d65 2822 7365 7474 696e  romTheme("settin
-0001e200: 6773 2229 2c20 2753 6574 7469 6e67 7327  gs"), 'Settings'
-0001e210: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001e220: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0001e230: 7265 6e74 3d73 656c 6629 0a20 2020 2020  rent=self).     
-0001e240: 2020 2061 7365 7474 696e 6773 2e74 7269     asettings.tri
-0001e250: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
-0001e260: 656c 662e 5f74 6f67 676c 655f 7365 7474  elf._toggle_sett
-0001e270: 696e 6773 5f66 6967 290a 2020 2020 2020  ings_fig).      
-0001e280: 2020 7365 6c66 2e6d 6e65 2e74 6f6f 6c62    self.mne.toolb
-0001e290: 6172 2e61 6464 4163 7469 6f6e 2861 7365  ar.addAction(ase
-0001e2a0: 7474 696e 6773 290a 0a20 2020 2020 2020  ttings)..       
-0001e2b0: 2061 6865 6c70 203d 2051 4163 7469 6f6e   ahelp = QAction
-0001e2c0: 2851 4963 6f6e 2e66 726f 6d54 6865 6d65  (QIcon.fromTheme
-0001e2d0: 2822 6865 6c70 2229 2c20 2748 656c 7027  ("help"), 'Help'
-0001e2e0: 2c20 7061 7265 6e74 3d73 656c 6629 0a20  , parent=self). 
-0001e2f0: 2020 2020 2020 2061 6865 6c70 2e74 7269         ahelp.tri
-0001e300: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
-0001e310: 656c 662e 5f74 6f67 676c 655f 6865 6c70  elf._toggle_help
-0001e320: 5f66 6967 290a 2020 2020 2020 2020 7365  _fig).        se
-0001e330: 6c66 2e6d 6e65 2e74 6f6f 6c62 6172 2e61  lf.mne.toolbar.a
-0001e340: 6464 4163 7469 6f6e 2861 6865 6c70 290a  ddAction(ahelp).
-0001e350: 0a20 2020 2020 2020 2023 2053 6574 2053  .        # Set S
-0001e360: 7461 7274 2d52 616e 6765 2028 6166 7465  tart-Range (afte
-0001e370: 7220 616c 6c20 6e65 6365 7373 6172 7920  r all necessary 
-0001e380: 656c 656d 656e 7473 2061 7265 2069 6e69  elements are ini
-0001e390: 7469 616c 697a 6564 290a 2020 2020 2020  tialized).      
-0001e3a0: 2020 7365 6c66 2e6d 6e65 2e70 6c74 2e73    self.mne.plt.s
-0001e3b0: 6574 5852 616e 6765 2873 656c 662e 6d6e  etXRange(self.mn
-0001e3c0: 652e 745f 7374 6172 742c 0a20 2020 2020  e.t_start,.     
+0001caa0: 2020 2020 2020 2020 6261 636b 6772 6f75          backgrou
+0001cab0: 6e64 3d27 7727 290a 2020 2020 2020 2020  nd='w').        
+0001cac0: 6267 636f 6c6f 7220 3d20 6765 7461 7474  bgcolor = getatt
+0001cad0: 7228 7365 6c66 2e6d 6e65 2c20 2762 6763  r(self.mne, 'bgc
+0001cae0: 6f6c 6f72 272c 2027 7727 290a 2020 2020  olor', 'w').    
+0001caf0: 2020 2020 7365 6c66 2e6d 6e65 2e76 6965      self.mne.vie
+0001cb00: 772e 7365 7442 6163 6b67 726f 756e 6428  w.setBackground(
+0001cb10: 5f67 6574 5f63 6f6c 6f72 2862 6763 6f6c  _get_color(bgcol
+0001cb20: 6f72 2c20 7365 6c66 2e6d 6e65 2e64 6172  or, self.mne.dar
+0001cb30: 6b29 290a 2020 2020 2020 2020 6c61 796f  k)).        layo
+0001cb40: 7574 2e61 6464 5769 6467 6574 2873 656c  ut.addWidget(sel
+0001cb50: 662e 6d6e 652e 7669 6577 2c20 302c 2030  f.mne.view, 0, 0
+0001cb60: 290a 0a20 2020 2020 2020 2023 2049 6e69  )..        # Ini
+0001cb70: 7469 616c 697a 6520 5363 726f 6c6c 2d42  tialize Scroll-B
+0001cb80: 6172 730a 2020 2020 2020 2020 7365 6c66  ars.        self
+0001cb90: 2e6d 6e65 2e61 785f 6873 6372 6f6c 6c20  .mne.ax_hscroll 
+0001cba0: 3d20 5469 6d65 5363 726f 6c6c 4261 7228  = TimeScrollBar(
+0001cbb0: 7365 6c66 2e6d 6e65 290a 2020 2020 2020  self.mne).      
+0001cbc0: 2020 6c61 796f 7574 2e61 6464 5769 6467    layout.addWidg
+0001cbd0: 6574 2873 656c 662e 6d6e 652e 6178 5f68  et(self.mne.ax_h
+0001cbe0: 7363 726f 6c6c 2c20 312c 2030 2c20 312c  scroll, 1, 0, 1,
+0001cbf0: 2032 290a 0a20 2020 2020 2020 2073 656c   2)..        sel
+0001cc00: 662e 6d6e 652e 6178 5f76 7363 726f 6c6c  f.mne.ax_vscroll
+0001cc10: 203d 2043 6861 6e6e 656c 5363 726f 6c6c   = ChannelScroll
+0001cc20: 4261 7228 7365 6c66 2e6d 6e65 290a 2020  Bar(self.mne).  
+0001cc30: 2020 2020 2020 6c61 796f 7574 2e61 6464        layout.add
+0001cc40: 5769 6467 6574 2873 656c 662e 6d6e 652e  Widget(self.mne.
+0001cc50: 6178 5f76 7363 726f 6c6c 2c20 302c 2031  ax_vscroll, 0, 1
+0001cc60: 290a 0a20 2020 2020 2020 2023 2049 6e69  )..        # Ini
+0001cc70: 7469 616c 697a 6520 564c 696e 650a 2020  tialize VLine.  
+0001cc80: 2020 2020 2020 7365 6c66 2e6d 6e65 2e76        self.mne.v
+0001cc90: 6c69 6e65 203d 204e 6f6e 650a 2020 2020  line = None.    
+0001cca0: 2020 2020 7365 6c66 2e6d 6e65 2e76 6c69      self.mne.vli
+0001ccb0: 6e65 5f76 6973 6962 6c65 203d 2046 616c  ne_visible = Fal
+0001ccc0: 7365 0a0a 2020 2020 2020 2020 2320 496e  se..        # In
+0001ccd0: 6974 6961 6c69 7a65 2063 726f 7373 6861  itialize crossha
+0001cce0: 6972 2028 6173 2069 6e20 7079 7174 6772  ir (as in pyqtgr
+0001ccf0: 6170 6820 6578 616d 706c 6529 0a20 2020  aph example).   
+0001cd00: 2020 2020 2073 656c 662e 6d6e 652e 6372       self.mne.cr
+0001cd10: 6f73 7368 6169 725f 656e 6162 6c65 6420  osshair_enabled 
+0001cd20: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+0001cd30: 7365 6c66 2e6d 6e65 2e63 726f 7373 6861  self.mne.crossha
+0001cd40: 6972 5f68 203d 204e 6f6e 650a 2020 2020  ir_h = None.    
+0001cd50: 2020 2020 7365 6c66 2e6d 6e65 2e63 726f      self.mne.cro
+0001cd60: 7373 6861 6972 203d 204e 6f6e 650a 2020  sshair = None.  
+0001cd70: 2020 2020 2020 7365 6c66 2e6d 6e65 2e76        self.mne.v
+0001cd80: 6965 772e 7369 6753 6365 6e65 4d6f 7573  iew.sigSceneMous
+0001cd90: 654d 6f76 6564 2e63 6f6e 6e65 6374 2873  eMoved.connect(s
+0001cda0: 656c 662e 5f6d 6f75 7365 5f6d 6f76 6564  elf._mouse_moved
+0001cdb0: 290a 0a20 2020 2020 2020 2023 2049 6e69  )..        # Ini
+0001cdc0: 7469 616c 697a 6520 416e 6e6f 7461 7469  tialize Annotati
+0001cdd0: 6f6e 2d57 6964 6765 7473 0a20 2020 2020  on-Widgets.     
+0001cde0: 2020 2073 656c 662e 6d6e 652e 616e 6e6f     self.mne.anno
+0001cdf0: 7461 7469 6f6e 5f6d 6f64 6520 3d20 4661  tation_mode = Fa
+0001ce00: 6c73 650a 2020 2020 2020 2020 6966 206e  lse.        if n
+0001ce10: 6f74 2073 656c 662e 6d6e 652e 6973 5f65  ot self.mne.is_e
+0001ce20: 706f 6368 733a 0a20 2020 2020 2020 2020  pochs:.         
+0001ce30: 2020 2073 656c 662e 5f69 6e69 745f 616e     self._init_an
+0001ce40: 6e6f 745f 6d6f 6465 2829 0a0a 2020 2020  not_mode()..    
+0001ce50: 2020 2020 2320 4f76 6572 7669 6577 4261      # OverviewBa
+0001ce60: 720a 2020 2020 2020 2020 7365 6c66 2e6d  r.        self.m
+0001ce70: 6e65 2e6f 7665 7276 6965 775f 6261 7220  ne.overview_bar 
+0001ce80: 3d20 4f76 6572 7669 6577 4261 7228 7365  = OverviewBar(se
+0001ce90: 6c66 290a 2020 2020 2020 2020 6c61 796f  lf).        layo
+0001cea0: 7574 2e61 6464 5769 6467 6574 2873 656c  ut.addWidget(sel
+0001ceb0: 662e 6d6e 652e 6f76 6572 7669 6577 5f62  f.mne.overview_b
+0001cec0: 6172 2c20 322c 2030 2c20 312c 2032 290a  ar, 2, 0, 1, 2).
+0001ced0: 0a20 2020 2020 2020 2077 6964 6765 742e  .        widget.
+0001cee0: 7365 744c 6179 6f75 7428 6c61 796f 7574  setLayout(layout
+0001cef0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0001cf00: 6574 4365 6e74 7261 6c57 6964 6765 7428  etCentralWidget(
+0001cf10: 7769 6467 6574 290a 0a20 2020 2020 2020  widget)..       
+0001cf20: 2023 2049 6e69 7469 616c 697a 6520 5365   # Initialize Se
+0001cf30: 6c65 6374 696f 6e2d 4469 616c 6f67 0a20  lection-Dialog. 
+0001cf40: 2020 2020 2020 2069 6620 6765 7461 7474         if getatt
+0001cf50: 7228 7365 6c66 2e6d 6e65 2c20 2767 726f  r(self.mne, 'gro
+0001cf60: 7570 5f62 7927 2c20 4e6f 6e65 2920 696e  up_by', None) in
+0001cf70: 205b 2770 6f73 6974 696f 6e27 2c20 2773   ['position', 's
+0001cf80: 656c 6563 7469 6f6e 275d 3a0a 2020 2020  election']:.    
+0001cf90: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
+0001cfa0: 6561 7465 5f73 656c 6563 7469 6f6e 5f66  eate_selection_f
+0001cfb0: 6967 2829 0a0a 2020 2020 2020 2020 2320  ig()..        # 
+0001cfc0: 496e 6974 6961 6c69 7a65 2050 726f 6a65  Initialize Proje
+0001cfd0: 6374 6f72 732d 4469 616c 6f67 2069 6620  ctors-Dialog if 
+0001cfe0: 7368 6f77 5f6f 7074 696f 6e73 3d54 7275  show_options=Tru
+0001cff0: 650a 2020 2020 2020 2020 6966 2067 6574  e.        if get
+0001d000: 6174 7472 2873 656c 662e 6d6e 652c 2027  attr(self.mne, '
+0001d010: 7368 6f77 5f6f 7074 696f 6e73 272c 2046  show_options', F
+0001d020: 616c 7365 293a 0a20 2020 2020 2020 2020  alse):.         
+0001d030: 2020 2073 656c 662e 5f74 6f67 676c 655f     self._toggle_
+0001d040: 7072 6f6a 5f66 6967 2829 0a0a 2020 2020  proj_fig()..    
+0001d050: 2020 2020 2320 496e 6974 6961 6c69 7a65      # Initialize
+0001d060: 2054 6f6f 6c62 6172 0a20 2020 2020 2020   Toolbar.       
+0001d070: 2073 656c 662e 6d6e 652e 746f 6f6c 6261   self.mne.toolba
+0001d080: 7220 3d20 7365 6c66 2e61 6464 546f 6f6c  r = self.addTool
+0001d090: 4261 7228 2754 6f6f 6c73 2729 0a20 2020  Bar('Tools').   
+0001d0a0: 2020 2020 2023 2074 6f6f 6c5f 6275 7474       # tool_butt
+0001d0b0: 6f6e 5f73 7479 6c65 203d 2051 742e 546f  on_style = Qt.To
+0001d0c0: 6f6c 4275 7474 6f6e 5465 7874 4265 7369  olButtonTextBesi
+0001d0d0: 6465 4963 6f6e 0a20 2020 2020 2020 2074  deIcon.        t
+0001d0e0: 6f6f 6c5f 6275 7474 6f6e 5f73 7479 6c65  ool_button_style
+0001d0f0: 203d 2051 742e 546f 6f6c 4275 7474 6f6e   = Qt.ToolButton
+0001d100: 4963 6f6e 4f6e 6c79 0a20 2020 2020 2020  IconOnly.       
+0001d110: 2073 656c 662e 6d6e 652e 746f 6f6c 6261   self.mne.toolba
+0001d120: 722e 7365 7454 6f6f 6c42 7574 746f 6e53  r.setToolButtonS
+0001d130: 7479 6c65 2874 6f6f 6c5f 6275 7474 6f6e  tyle(tool_button
+0001d140: 5f73 7479 6c65 290a 0a20 2020 2020 2020  _style)..       
+0001d150: 2061 6465 6372 5f74 696d 6520 3d20 5141   adecr_time = QA
+0001d160: 6374 696f 6e28 0a20 2020 2020 2020 2020  ction(.         
+0001d170: 2020 2051 4963 6f6e 2e66 726f 6d54 6865     QIcon.fromThe
+0001d180: 6d65 2822 6c65 7373 5f74 696d 6522 292c  me("less_time"),
+0001d190: 2027 2d20 5469 6d65 272c 2070 6172 656e   '- Time', paren
+0001d1a0: 743d 7365 6c66 290a 2020 2020 2020 2020  t=self).        
+0001d1b0: 6164 6563 725f 7469 6d65 2e74 7269 6767  adecr_time.trigg
+0001d1c0: 6572 6564 2e63 6f6e 6e65 6374 280a 2020  ered.connect(.  
+0001d1d0: 2020 2020 2020 2020 2020 5f6d 6574 6870            _methp
+0001d1e0: 6172 7469 616c 2873 656c 662e 6368 616e  artial(self.chan
+0001d1f0: 6765 5f64 7572 6174 696f 6e2c 2073 7465  ge_duration, ste
+0001d200: 703d 2d30 2e32 2929 0a20 2020 2020 2020  p=-0.2)).       
+0001d210: 2073 656c 662e 6d6e 652e 746f 6f6c 6261   self.mne.toolba
+0001d220: 722e 6164 6441 6374 696f 6e28 6164 6563  r.addAction(adec
+0001d230: 725f 7469 6d65 290a 2020 2020 2020 2020  r_time).        
+0001d240: 6169 6e63 725f 7469 6d65 203d 2051 4163  aincr_time = QAc
+0001d250: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+0001d260: 2020 5149 636f 6e2e 6672 6f6d 5468 656d    QIcon.fromThem
+0001d270: 6528 226d 6f72 655f 7469 6d65 2229 2c20  e("more_time"), 
+0001d280: 272b 2054 696d 6527 2c20 7061 7265 6e74  '+ Time', parent
+0001d290: 3d73 656c 6629 0a20 2020 2020 2020 2061  =self).        a
+0001d2a0: 696e 6372 5f74 696d 652e 7472 6967 6765  incr_time.trigge
+0001d2b0: 7265 642e 636f 6e6e 6563 7428 0a20 2020  red.connect(.   
+0001d2c0: 2020 2020 2020 2020 205f 6d65 7468 7061           _methpa
+0001d2d0: 7274 6961 6c28 7365 6c66 2e63 6861 6e67  rtial(self.chang
+0001d2e0: 655f 6475 7261 7469 6f6e 2c20 7374 6570  e_duration, step
+0001d2f0: 3d30 2e32 3529 290a 2020 2020 2020 2020  =0.25)).        
+0001d300: 7365 6c66 2e6d 6e65 2e74 6f6f 6c62 6172  self.mne.toolbar
+0001d310: 2e61 6464 4163 7469 6f6e 2861 696e 6372  .addAction(aincr
+0001d320: 5f74 696d 6529 0a20 2020 2020 2020 2073  _time).        s
+0001d330: 656c 662e 6d6e 652e 746f 6f6c 6261 722e  elf.mne.toolbar.
+0001d340: 6164 6453 6570 6172 6174 6f72 2829 0a0a  addSeparator()..
+0001d350: 2020 2020 2020 2020 6164 6563 725f 6e63          adecr_nc
+0001d360: 6861 6e20 3d20 5141 6374 696f 6e28 0a20  han = QAction(. 
+0001d370: 2020 2020 2020 2020 2020 2051 4963 6f6e             QIcon
+0001d380: 2e66 726f 6d54 6865 6d65 2822 6c65 7373  .fromTheme("less
+0001d390: 5f63 6861 6e6e 656c 7322 292c 2027 2d20  _channels"), '- 
+0001d3a0: 4368 616e 6e65 6c73 272c 2070 6172 656e  Channels', paren
+0001d3b0: 743d 7365 6c66 290a 2020 2020 2020 2020  t=self).        
+0001d3c0: 6164 6563 725f 6e63 6861 6e2e 7472 6967  adecr_nchan.trig
+0001d3d0: 6765 7265 642e 636f 6e6e 6563 7428 0a20  gered.connect(. 
+0001d3e0: 2020 2020 2020 2020 2020 205f 6d65 7468             _meth
+0001d3f0: 7061 7274 6961 6c28 7365 6c66 2e63 6861  partial(self.cha
+0001d400: 6e67 655f 6e63 6861 6e2c 2073 7465 703d  nge_nchan, step=
+0001d410: 2d31 3029 290a 2020 2020 2020 2020 7365  -10)).        se
+0001d420: 6c66 2e6d 6e65 2e74 6f6f 6c62 6172 2e61  lf.mne.toolbar.a
+0001d430: 6464 4163 7469 6f6e 2861 6465 6372 5f6e  ddAction(adecr_n
+0001d440: 6368 616e 290a 2020 2020 2020 2020 6169  chan).        ai
+0001d450: 6e63 725f 6e63 6861 6e20 3d20 5141 6374  ncr_nchan = QAct
+0001d460: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+0001d470: 2051 4963 6f6e 2e66 726f 6d54 6865 6d65   QIcon.fromTheme
+0001d480: 2822 6d6f 7265 5f63 6861 6e6e 656c 7322  ("more_channels"
+0001d490: 292c 2027 2b20 4368 616e 6e65 6c73 272c  ), '+ Channels',
+0001d4a0: 2070 6172 656e 743d 7365 6c66 290a 2020   parent=self).  
+0001d4b0: 2020 2020 2020 6169 6e63 725f 6e63 6861        aincr_ncha
+0001d4c0: 6e2e 7472 6967 6765 7265 642e 636f 6e6e  n.triggered.conn
+0001d4d0: 6563 7428 0a20 2020 2020 2020 2020 2020  ect(.           
+0001d4e0: 205f 6d65 7468 7061 7274 6961 6c28 7365   _methpartial(se
+0001d4f0: 6c66 2e63 6861 6e67 655f 6e63 6861 6e2c  lf.change_nchan,
+0001d500: 2073 7465 703d 3130 2929 0a20 2020 2020   step=10)).     
+0001d510: 2020 2073 656c 662e 6d6e 652e 746f 6f6c     self.mne.tool
+0001d520: 6261 722e 6164 6441 6374 696f 6e28 6169  bar.addAction(ai
+0001d530: 6e63 725f 6e63 6861 6e29 0a20 2020 2020  ncr_nchan).     
+0001d540: 2020 2073 656c 662e 6d6e 652e 746f 6f6c     self.mne.tool
+0001d550: 6261 722e 6164 6453 6570 6172 6174 6f72  bar.addSeparator
+0001d560: 2829 0a0a 2020 2020 2020 2020 6164 6563  ()..        adec
+0001d570: 725f 6e63 6861 6e20 3d20 5141 6374 696f  r_nchan = QActio
+0001d580: 6e28 0a20 2020 2020 2020 2020 2020 2051  n(.            Q
+0001d590: 4963 6f6e 2e66 726f 6d54 6865 6d65 2822  Icon.fromTheme("
+0001d5a0: 7a6f 6f6d 5f6f 7574 2229 2c20 275a 6f6f  zoom_out"), 'Zoo
+0001d5b0: 6d20 6f75 7427 2c20 7061 7265 6e74 3d73  m out', parent=s
+0001d5c0: 656c 6629 0a20 2020 2020 2020 2061 6465  elf).        ade
+0001d5d0: 6372 5f6e 6368 616e 2e74 7269 6767 6572  cr_nchan.trigger
+0001d5e0: 6564 2e63 6f6e 6e65 6374 280a 2020 2020  ed.connect(.    
+0001d5f0: 2020 2020 2020 2020 5f6d 6574 6870 6172          _methpar
+0001d600: 7469 616c 2873 656c 662e 7363 616c 655f  tial(self.scale_
+0001d610: 616c 6c2c 2073 7465 703d 3420 2f20 3529  all, step=4 / 5)
+0001d620: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
+0001d630: 6e65 2e74 6f6f 6c62 6172 2e61 6464 4163  ne.toolbar.addAc
+0001d640: 7469 6f6e 2861 6465 6372 5f6e 6368 616e  tion(adecr_nchan
+0001d650: 290a 2020 2020 2020 2020 6169 6e63 725f  ).        aincr_
+0001d660: 6e63 6861 6e20 3d20 5141 6374 696f 6e28  nchan = QAction(
+0001d670: 0a20 2020 2020 2020 2020 2020 2051 4963  .            QIc
+0001d680: 6f6e 2e66 726f 6d54 6865 6d65 2822 7a6f  on.fromTheme("zo
+0001d690: 6f6d 5f69 6e22 292c 2027 5a6f 6f6d 2069  om_in"), 'Zoom i
+0001d6a0: 6e27 2c20 7061 7265 6e74 3d73 656c 6629  n', parent=self)
+0001d6b0: 0a20 2020 2020 2020 2061 696e 6372 5f6e  .        aincr_n
+0001d6c0: 6368 616e 2e74 7269 6767 6572 6564 2e63  chan.triggered.c
+0001d6d0: 6f6e 6e65 6374 280a 2020 2020 2020 2020  onnect(.        
+0001d6e0: 2020 2020 5f6d 6574 6870 6172 7469 616c      _methpartial
+0001d6f0: 2873 656c 662e 7363 616c 655f 616c 6c2c  (self.scale_all,
+0001d700: 2073 7465 703d 3520 2f20 3429 290a 2020   step=5 / 4)).  
+0001d710: 2020 2020 2020 7365 6c66 2e6d 6e65 2e74        self.mne.t
+0001d720: 6f6f 6c62 6172 2e61 6464 4163 7469 6f6e  oolbar.addAction
+0001d730: 2861 696e 6372 5f6e 6368 616e 290a 2020  (aincr_nchan).  
+0001d740: 2020 2020 2020 7365 6c66 2e6d 6e65 2e74        self.mne.t
+0001d750: 6f6f 6c62 6172 2e61 6464 5365 7061 7261  oolbar.addSepara
+0001d760: 746f 7228 290a 0a20 2020 2020 2020 2069  tor()..        i
+0001d770: 6620 6e6f 7420 7365 6c66 2e6d 6e65 2e69  f not self.mne.i
+0001d780: 735f 6570 6f63 6873 3a0a 2020 2020 2020  s_epochs:.      
+0001d790: 2020 2020 2020 6174 6f67 676c 655f 616e        atoggle_an
+0001d7a0: 6e6f 7420 3d20 5141 6374 696f 6e28 0a20  not = QAction(. 
+0001d7b0: 2020 2020 2020 2020 2020 2020 2020 2051                 Q
+0001d7c0: 4963 6f6e 2e66 726f 6d54 6865 6d65 2822  Icon.fromTheme("
+0001d7d0: 616e 6e6f 7461 7469 6f6e 7322 292c 2027  annotations"), '
+0001d7e0: 416e 6e6f 7461 7469 6f6e 7327 2c20 7061  Annotations', pa
+0001d7f0: 7265 6e74 3d73 656c 6629 0a20 2020 2020  rent=self).     
+0001d800: 2020 2020 2020 2061 746f 6767 6c65 5f61         atoggle_a
+0001d810: 6e6e 6f74 2e74 7269 6767 6572 6564 2e63  nnot.triggered.c
+0001d820: 6f6e 6e65 6374 2873 656c 662e 5f74 6f67  onnect(self._tog
+0001d830: 676c 655f 616e 6e6f 7461 7469 6f6e 5f66  gle_annotation_f
+0001d840: 6967 290a 2020 2020 2020 2020 2020 2020  ig).            
+0001d850: 7365 6c66 2e6d 6e65 2e74 6f6f 6c62 6172  self.mne.toolbar
+0001d860: 2e61 6464 4163 7469 6f6e 2861 746f 6767  .addAction(atogg
+0001d870: 6c65 5f61 6e6e 6f74 290a 0a20 2020 2020  le_annot)..     
+0001d880: 2020 2061 746f 6767 6c65 5f70 726f 6a20     atoggle_proj 
+0001d890: 3d20 5141 6374 696f 6e28 0a20 2020 2020  = QAction(.     
+0001d8a0: 2020 2020 2020 2051 4963 6f6e 2e66 726f         QIcon.fro
+0001d8b0: 6d54 6865 6d65 2822 7373 7022 292c 2027  mTheme("ssp"), '
+0001d8c0: 5353 5027 2c20 7061 7265 6e74 3d73 656c  SSP', parent=sel
+0001d8d0: 6629 0a20 2020 2020 2020 2061 746f 6767  f).        atogg
+0001d8e0: 6c65 5f70 726f 6a2e 7472 6967 6765 7265  le_proj.triggere
+0001d8f0: 642e 636f 6e6e 6563 7428 7365 6c66 2e5f  d.connect(self._
+0001d900: 746f 6767 6c65 5f70 726f 6a5f 6669 6729  toggle_proj_fig)
+0001d910: 0a20 2020 2020 2020 2073 656c 662e 6d6e  .        self.mn
+0001d920: 652e 746f 6f6c 6261 722e 6164 6441 6374  e.toolbar.addAct
+0001d930: 696f 6e28 6174 6f67 676c 655f 7072 6f6a  ion(atoggle_proj
+0001d940: 290a 0a20 2020 2020 2020 2062 7574 746f  )..        butto
+0001d950: 6e20 3d20 5154 6f6f 6c42 7574 746f 6e28  n = QToolButton(
+0001d960: 7365 6c66 2e6d 6e65 2e74 6f6f 6c62 6172  self.mne.toolbar
+0001d970: 290a 2020 2020 2020 2020 6275 7474 6f6e  ).        button
+0001d980: 2e73 6574 546f 6f6c 5469 7028 0a20 2020  .setToolTip(.   
+0001d990: 2020 2020 2020 2020 2027 3c68 323e 4f76           '<h2>Ov
+0001d9a0: 6572 7669 6577 2d4d 6f64 6573 3c2f 6832  erview-Modes</h2
+0001d9b0: 3e27 0a20 2020 2020 2020 2020 2020 2027  >'.            '
+0001d9c0: 3c75 6c3e 270a 2020 2020 2020 2020 2020  <ul>'.          
+0001d9d0: 2020 273c 6c69 3e65 6d70 7479 3a3c 6272    '<li>empty:<br
+0001d9e0: 3e27 0a20 2020 2020 2020 2020 2020 2027  >'.            '
+0001d9f0: 4469 7370 6c61 7920 6e6f 2062 6163 6b67  Display no backg
+0001da00: 726f 756e 642e 3c2f 6c69 3e27 0a20 2020  round.</li>'.   
+0001da10: 2020 2020 2020 2020 2027 3c6c 693e 6368           '<li>ch
+0001da20: 616e 6e65 6c73 3a3c 6272 3e27 0a20 2020  annels:<br>'.   
+0001da30: 2020 2020 2020 2020 2027 4469 7370 6c61           'Displa
+0001da40: 7920 6561 6368 2063 6861 6e6e 656c 2077  y each channel w
+0001da50: 6974 6820 6974 7320 6368 616e 6e65 6c2d  ith its channel-
+0001da60: 7479 7065 2063 6f6c 6f72 2e3c 2f6c 693e  type color.</li>
+0001da70: 270a 2020 2020 2020 2020 2020 2020 273c  '.            '<
+0001da80: 6c69 3e7a 7363 6f72 653a 3c62 723e 270a  li>zscore:<br>'.
+0001da90: 2020 2020 2020 2020 2020 2020 2744 6973              'Dis
+0001daa0: 706c 6179 2074 6865 207a 7363 6f72 6520  play the zscore 
+0001dab0: 666f 7220 7468 6520 6461 7461 2066 726f  for the data fro
+0001dac0: 6d20 6561 6368 2063 6861 6e6e 656c 2061  m each channel a
+0001dad0: 6372 6f73 7320 7469 6d65 2e20 270a 2020  cross time. '.  
+0001dae0: 2020 2020 2020 2020 2020 2752 6564 2069            'Red i
+0001daf0: 6e64 6963 6174 6573 2068 6967 6820 7a73  ndicates high zs
+0001db00: 636f 7265 732c 2062 6c75 6520 696e 6469  cores, blue indi
+0001db10: 6361 7465 7320 6c6f 7720 7a73 636f 7265  cates low zscore
+0001db20: 732c 2027 0a20 2020 2020 2020 2020 2020  s, '.           
+0001db30: 2027 616e 6420 7468 6520 626f 756e 6461   'and the bounda
+0001db40: 7269 6573 206f 6620 7468 6520 636f 6c6f  ries of the colo
+0001db50: 7220 6772 6164 6965 6e74 2061 7265 2064  r gradient are d
+0001db60: 6566 696e 6564 2062 7920 7468 6520 270a  efined by the '.
+0001db70: 2020 2020 2020 2020 2020 2020 276d 696e              'min
+0001db80: 696d 756d 2f6d 6178 696d 756d 207a 7363  imum/maximum zsc
+0001db90: 6f72 652e 270a 2020 2020 2020 2020 2020  ore.'.          
+0001dba0: 2020 2754 6869 7320 6f6e 6c79 2077 6f72    'This only wor
+0001dbb0: 6b73 2069 6620 7072 6563 6f6d 7075 7465  ks if precompute
+0001dbc0: 2069 7320 7365 7420 746f 2022 5472 7565   is set to "True
+0001dbd0: 222c 206f 7220 6966 2069 7420 6973 2027  ", or if it is '
+0001dbe0: 0a20 2020 2020 2020 2020 2020 2027 656e  .            'en
+0001dbf0: 6162 6c65 6420 7769 7468 2022 6175 746f  abled with "auto
+0001dc00: 2220 616e 6420 656e 6f75 6768 2066 7265  " and enough fre
+0001dc10: 6520 5241 4d20 6973 2061 7661 696c 6162  e RAM is availab
+0001dc20: 6c65 2e3c 2f6c 693e 270a 2020 2020 2020  le.</li>'.      
+0001dc30: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001dc40: 6275 7474 6f6e 2e73 6574 5465 7874 2827  button.setText('
+0001dc50: 4f76 6572 7669 6577 2042 6172 2729 0a20  Overview Bar'). 
+0001dc60: 2020 2020 2020 2062 7574 746f 6e2e 7365         button.se
+0001dc70: 7449 636f 6e28 5149 636f 6e2e 6672 6f6d  tIcon(QIcon.from
+0001dc80: 5468 656d 6528 276f 7665 7276 6965 775f  Theme('overview_
+0001dc90: 6261 7227 2929 0a20 2020 2020 2020 2062  bar')).        b
+0001dca0: 7574 746f 6e2e 7365 7454 6f6f 6c42 7574  utton.setToolBut
+0001dcb0: 746f 6e53 7479 6c65 2874 6f6f 6c5f 6275  tonStyle(tool_bu
+0001dcc0: 7474 6f6e 5f73 7479 6c65 290a 2020 2020  tton_style).    
+0001dcd0: 2020 2020 6d65 6e75 203d 2073 656c 662e      menu = self.
+0001dce0: 6d6e 652e 6f76 6572 7669 6577 5f6d 656e  mne.overview_men
+0001dcf0: 7520 3d20 514d 656e 7528 6275 7474 6f6e  u = QMenu(button
+0001dd00: 290a 2020 2020 2020 2020 6772 6f75 7020  ).        group 
+0001dd10: 3d20 5141 6374 696f 6e47 726f 7570 286d  = QActionGroup(m
+0001dd20: 656e 7529 0a20 2020 2020 2020 2066 6f72  enu).        for
+0001dd30: 206b 6579 2c20 7465 7874 2069 6e20 6f76   key, text in ov
+0001dd40: 6572 7669 6577 5f69 7465 6d73 2e69 7465  erview_items.ite
+0001dd50: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+0001dd60: 2020 7261 6469 6f20 3d20 5152 6164 696f    radio = QRadio
+0001dd70: 4275 7474 6f6e 286d 656e 7529 0a20 2020  Button(menu).   
+0001dd80: 2020 2020 2020 2020 2072 6164 696f 2e73           radio.s
+0001dd90: 6574 5465 7874 2874 6578 7429 0a20 2020  etText(text).   
+0001dda0: 2020 2020 2020 2020 2069 6620 6b65 7920           if key 
+0001ddb0: 3d3d 2073 656c 662e 6d6e 652e 6f76 6572  == self.mne.over
+0001ddc0: 7669 6577 5f6d 6f64 653a 0a20 2020 2020  view_mode:.     
+0001ddd0: 2020 2020 2020 2020 2020 2072 6164 696f             radio
+0001dde0: 2e73 6574 4368 6563 6b65 6428 5472 7565  .setChecked(True
+0001ddf0: 290a 2020 2020 2020 2020 2020 2020 6163  ).            ac
+0001de00: 7469 6f6e 203d 2051 5769 6467 6574 4163  tion = QWidgetAc
+0001de10: 7469 6f6e 286d 656e 7529 0a20 2020 2020  tion(menu).     
+0001de20: 2020 2020 2020 2061 6374 696f 6e2e 7365         action.se
+0001de30: 7444 6566 6175 6c74 5769 6467 6574 2872  tDefaultWidget(r
+0001de40: 6164 696f 290a 2020 2020 2020 2020 2020  adio).          
+0001de50: 2020 6d65 6e75 2e61 6464 4163 7469 6f6e    menu.addAction
+0001de60: 2861 6374 696f 6e29 0a20 2020 2020 2020  (action).       
+0001de70: 2020 2020 2067 726f 7570 2e61 6464 4163       group.addAc
+0001de80: 7469 6f6e 2861 6374 696f 6e29 0a20 2020  tion(action).   
+0001de90: 2020 2020 2020 2020 2072 6164 696f 2e63           radio.c
+0001dea0: 6c69 636b 6564 2e63 6f6e 6e65 6374 280a  licked.connect(.
+0001deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dec0: 5f6d 6574 6870 6172 7469 616c 280a 2020  _methpartial(.  
+0001ded0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dee0: 2020 7365 6c66 2e5f 6f76 6572 7669 6577    self._overview
+0001def0: 5f72 6164 696f 5f63 6c69 636b 6564 2c20  _radio_clicked, 
+0001df00: 6d65 6e75 3d6d 656e 752c 206e 6577 5f6d  menu=menu, new_m
+0001df10: 6f64 653d 6b65 7929 290a 2020 2020 2020  ode=key)).      
+0001df20: 2020 6d65 6e75 2e61 6464 5365 7061 7261    menu.addSepara
+0001df30: 746f 7228 290a 2020 2020 2020 2020 7669  tor().        vi
+0001df40: 7369 626c 6520 3d20 5141 6374 696f 6e28  sible = QAction(
+0001df50: 2756 6973 6962 6c65 272c 2070 6172 656e  'Visible', paren
+0001df60: 743d 6d65 6e75 290a 2020 2020 2020 2020  t=menu).        
+0001df70: 6d65 6e75 2e61 6464 4163 7469 6f6e 2876  menu.addAction(v
+0001df80: 6973 6962 6c65 290a 2020 2020 2020 2020  isible).        
+0001df90: 7669 7369 626c 652e 7365 7443 6865 636b  visible.setCheck
+0001dfa0: 6162 6c65 2854 7275 6529 0a20 2020 2020  able(True).     
+0001dfb0: 2020 2076 6973 6962 6c65 2e73 6574 4368     visible.setCh
+0001dfc0: 6563 6b65 6428 5472 7565 290a 2020 2020  ecked(True).    
+0001dfd0: 2020 2020 7365 6c66 2e6d 6e65 2e6f 7665      self.mne.ove
+0001dfe0: 7276 6965 775f 6261 722e 7365 7456 6973  rview_bar.setVis
+0001dff0: 6962 6c65 2854 7275 6529 0a20 2020 2020  ible(True).     
+0001e000: 2020 2076 6973 6962 6c65 2e74 7269 6767     visible.trigg
+0001e010: 6572 6564 2e63 6f6e 6e65 6374 2873 656c  ered.connect(sel
+0001e020: 662e 5f74 6f67 676c 655f 6f76 6572 7669  f._toggle_overvi
+0001e030: 6577 5f62 6172 290a 2020 2020 2020 2020  ew_bar).        
+0001e040: 6966 2068 6964 655f 6f76 6572 7669 6577  if hide_overview
+0001e050: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0001e060: 5468 6973 2064 6f65 736e 2774 2077 6f72  This doesn't wor
+0001e070: 6b20 6265 6361 7573 6520 6974 2068 6173  k because it has
+0001e080: 6e27 7420 6265 656e 2073 686f 776e 2079  n't been shown y
+0001e090: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
+0001e0a0: 2320 7365 6c66 2e5f 746f 6767 6c65 5f6f  # self._toggle_o
+0001e0b0: 7665 7276 6965 775f 6261 7228 290a 2020  verview_bar().  
+0001e0c0: 2020 2020 2020 2020 2020 7669 7369 626c            visibl
+0001e0d0: 652e 7365 7443 6865 636b 6564 2846 616c  e.setChecked(Fal
+0001e0e0: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+0001e0f0: 7365 6c66 2e6d 6e65 2e6f 7665 7276 6965  self.mne.overvie
+0001e100: 775f 6261 722e 7365 7456 6973 6962 6c65  w_bar.setVisible
+0001e110: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+0001e120: 6275 7474 6f6e 2e73 6574 4d65 6e75 2873  button.setMenu(s
+0001e130: 656c 662e 6d6e 652e 6f76 6572 7669 6577  elf.mne.overview
+0001e140: 5f6d 656e 7529 0a20 2020 2020 2020 2062  _menu).        b
+0001e150: 7574 746f 6e2e 7365 7450 6f70 7570 4d6f  utton.setPopupMo
+0001e160: 6465 2851 546f 6f6c 4275 7474 6f6e 2e49  de(QToolButton.I
+0001e170: 6e73 7461 6e74 506f 7075 7029 0a20 2020  nstantPopup).   
+0001e180: 2020 2020 2073 656c 662e 6d6e 652e 746f       self.mne.to
+0001e190: 6f6c 6261 722e 6164 6457 6964 6765 7428  olbar.addWidget(
+0001e1a0: 6275 7474 6f6e 290a 0a20 2020 2020 2020  button)..       
+0001e1b0: 2073 656c 662e 6d6e 652e 746f 6f6c 6261   self.mne.toolba
+0001e1c0: 722e 6164 6453 6570 6172 6174 6f72 2829  r.addSeparator()
+0001e1d0: 0a0a 2020 2020 2020 2020 6173 6574 7469  ..        asetti
+0001e1e0: 6e67 7320 3d20 5141 6374 696f 6e28 5149  ngs = QAction(QI
+0001e1f0: 636f 6e2e 6672 6f6d 5468 656d 6528 2273  con.fromTheme("s
+0001e200: 6574 7469 6e67 7322 292c 2027 5365 7474  ettings"), 'Sett
+0001e210: 696e 6773 272c 0a20 2020 2020 2020 2020  ings',.         
+0001e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e230: 2020 2070 6172 656e 743d 7365 6c66 290a     parent=self).
+0001e240: 2020 2020 2020 2020 6173 6574 7469 6e67          asetting
+0001e250: 732e 7472 6967 6765 7265 642e 636f 6e6e  s.triggered.conn
+0001e260: 6563 7428 7365 6c66 2e5f 746f 6767 6c65  ect(self._toggle
+0001e270: 5f73 6574 7469 6e67 735f 6669 6729 0a20  _settings_fig). 
+0001e280: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
+0001e290: 746f 6f6c 6261 722e 6164 6441 6374 696f  toolbar.addActio
+0001e2a0: 6e28 6173 6574 7469 6e67 7329 0a0a 2020  n(asettings)..  
+0001e2b0: 2020 2020 2020 6168 656c 7020 3d20 5141        ahelp = QA
+0001e2c0: 6374 696f 6e28 5149 636f 6e2e 6672 6f6d  ction(QIcon.from
+0001e2d0: 5468 656d 6528 2268 656c 7022 292c 2027  Theme("help"), '
+0001e2e0: 4865 6c70 272c 2070 6172 656e 743d 7365  Help', parent=se
+0001e2f0: 6c66 290a 2020 2020 2020 2020 6168 656c  lf).        ahel
+0001e300: 702e 7472 6967 6765 7265 642e 636f 6e6e  p.triggered.conn
+0001e310: 6563 7428 7365 6c66 2e5f 746f 6767 6c65  ect(self._toggle
+0001e320: 5f68 656c 705f 6669 6729 0a20 2020 2020  _help_fig).     
+0001e330: 2020 2073 656c 662e 6d6e 652e 746f 6f6c     self.mne.tool
+0001e340: 6261 722e 6164 6441 6374 696f 6e28 6168  bar.addAction(ah
+0001e350: 656c 7029 0a0a 2020 2020 2020 2020 2320  elp)..        # 
+0001e360: 5365 7420 5374 6172 742d 5261 6e67 6520  Set Start-Range 
+0001e370: 2861 6674 6572 2061 6c6c 206e 6563 6573  (after all neces
+0001e380: 7361 7279 2065 6c65 6d65 6e74 7320 6172  sary elements ar
+0001e390: 6520 696e 6974 6961 6c69 7a65 6429 0a20  e initialized). 
+0001e3a0: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
+0001e3b0: 706c 742e 7365 7458 5261 6e67 6528 7365  plt.setXRange(se
+0001e3c0: 6c66 2e6d 6e65 2e74 5f73 7461 7274 2c0a  lf.mne.t_start,.
 0001e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e3e0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0001e3f0: 6e65 2e74 5f73 7461 7274 202b 2073 656c  ne.t_start + sel
-0001e400: 662e 6d6e 652e 6475 7261 7469 6f6e 2c0a  f.mne.duration,.
-0001e410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e420: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001e430: 6164 6469 6e67 3d30 290a 2020 2020 2020  adding=0).      
-0001e440: 2020 6966 2073 656c 662e 6d6e 652e 6275    if self.mne.bu
-0001e450: 7474 6572 666c 793a 0a20 2020 2020 2020  tterfly:.       
-0001e460: 2020 2020 2073 656c 662e 5f73 6574 5f62       self._set_b
-0001e470: 7574 7465 7266 6c79 2854 7275 6529 0a20  utterfly(True). 
-0001e480: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001e490: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
-0001e4a0: 652e 706c 742e 7365 7459 5261 6e67 6528  e.plt.setYRange(
-0001e4b0: 302c 2073 656c 662e 6d6e 652e 6e5f 6368  0, self.mne.n_ch
-0001e4c0: 616e 6e65 6c73 202b 2031 2c20 7061 6464  annels + 1, padd
-0001e4d0: 696e 673d 3029 0a0a 2020 2020 2020 2020  ing=0)..        
-0001e4e0: 2320 5365 7420 5369 7a65 0a20 2020 2020  # Set Size.     
-0001e4f0: 2020 2077 6964 7468 203d 2069 6e74 2873     width = int(s
-0001e500: 656c 662e 6d6e 652e 6669 6773 697a 655b  elf.mne.figsize[
-0001e510: 305d 202a 2073 656c 662e 6c6f 6769 6361  0] * self.logica
-0001e520: 6c44 7069 5828 2929 0a20 2020 2020 2020  lDpiX()).       
-0001e530: 2068 6569 6768 7420 3d20 696e 7428 7365   height = int(se
-0001e540: 6c66 2e6d 6e65 2e66 6967 7369 7a65 5b31  lf.mne.figsize[1
-0001e550: 5d20 2a20 7365 6c66 2e6c 6f67 6963 616c  ] * self.logical
-0001e560: 4470 6959 2829 290a 2020 2020 2020 2020  DpiY()).        
-0001e570: 7365 6c66 2e72 6573 697a 6528 7769 6474  self.resize(widt
-0001e580: 682c 2068 6569 6768 7429 0a0a 2020 2020  h, height)..    
-0001e590: 2020 2020 2320 496e 6974 6961 6c69 7a65      # Initialize
-0001e5a0: 204b 6579 626f 6172 642d 5368 6f72 7463   Keyboard-Shortc
-0001e5b0: 7574 730a 2020 2020 2020 2020 6973 5f6d  uts.        is_m
-0001e5c0: 6163 203d 2070 6c61 7466 6f72 6d2e 7379  ac = platform.sy
-0001e5d0: 7374 656d 2829 203d 3d20 2744 6172 7769  stem() == 'Darwi
-0001e5e0: 6e27 0a20 2020 2020 2020 2064 7572 5f6b  n'.        dur_k
-0001e5f0: 6579 7320 3d20 2827 666e 202b 20e2 8690  eys = ('fn + ...
-0001e600: 272c 2027 666e 202b 20e2 8692 2729 2069  ', 'fn + ...') i
-0001e610: 6620 6973 5f6d 6163 2065 6c73 6520 2827  f is_mac else ('
-0001e620: 486f 6d65 272c 2027 456e 6427 290a 2020  Home', 'End').  
-0001e630: 2020 2020 2020 6368 5f6b 6579 7320 3d20        ch_keys = 
-0001e640: 2827 666e 202b 20e2 8691 272c 2027 666e  ('fn + ...', 'fn
-0001e650: 202b 20e2 8693 2729 2069 6620 6973 5f6d   + ...') if is_m
-0001e660: 6163 2065 6c73 6520 2827 5061 6765 2075  ac else ('Page u
-0001e670: 7027 2c20 2750 6167 6520 646f 776e 2729  p', 'Page down')
-0001e680: 0a20 2020 2020 2020 2068 7363 726f 6c6c  .        hscroll
-0001e690: 5f74 7970 6520 3d20 2731 2065 706f 6368  _type = '1 epoch
-0001e6a0: 2720 6966 2073 656c 662e 6d6e 652e 6973  ' if self.mne.is
-0001e6b0: 5f65 706f 6368 7320 656c 7365 2027 c2bc  _epochs else '..
-0001e6c0: 2070 6167 6527 0a0a 2020 2020 2020 2020   page'..        
-0001e6d0: 7365 6c66 2e6d 6e65 2e6b 6579 626f 6172  self.mne.keyboar
-0001e6e0: 645f 7368 6f72 7463 7574 7320 3d20 7b0a  d_shortcuts = {.
-0001e6f0: 2020 2020 2020 2020 2020 2020 276c 6566              'lef
-0001e700: 7427 3a20 7b0a 2020 2020 2020 2020 2020  t': {.          
-0001e710: 2020 2020 2020 2761 6c69 6173 273a 2027        'alias': '
-0001e720: e286 9027 2c0a 2020 2020 2020 2020 2020  ...',.          
-0001e730: 2020 2020 2020 2771 745f 6b65 7927 3a20        'qt_key': 
-0001e740: 5174 2e4b 6579 5f4c 6566 742c 0a20 2020  Qt.Key_Left,.   
-0001e750: 2020 2020 2020 2020 2020 2020 2027 6d6f               'mo
-0001e760: 6469 6669 6572 273a 205b 4e6f 6e65 2c20  difier': [None, 
-0001e770: 2753 6869 6674 275d 2c0a 2020 2020 2020  'Shift'],.      
-0001e780: 2020 2020 2020 2020 2020 2773 6c6f 7427            'slot'
-0001e790: 3a20 5b73 656c 662e 6873 6372 6f6c 6c5d  : [self.hscroll]
-0001e7a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001e7b0: 2020 2770 6172 616d 6574 6572 273a 205b    'parameter': [
-0001e7c0: 2d34 302c 2027 2d66 756c 6c27 5d2c 0a20  -40, '-full'],. 
-0001e7d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0001e7e0: 6465 7363 7269 7074 696f 6e27 3a20 5b66  description': [f
-0001e7f0: 2753 6372 6f6c 6c20 6c65 6674 2028 7b68  'Scroll left ({h
-0001e800: 7363 726f 6c6c 5f74 7970 657d 2927 2c0a  scroll_type})',.
-0001e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e3e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001e3f0: 656c 662e 6d6e 652e 745f 7374 6172 7420  elf.mne.t_start 
+0001e400: 2b20 7365 6c66 2e6d 6e65 2e64 7572 6174  + self.mne.durat
+0001e410: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+0001e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e430: 2020 2020 7061 6464 696e 673d 3029 0a20      padding=0). 
+0001e440: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+0001e450: 6e65 2e62 7574 7465 7266 6c79 3a0a 2020  ne.butterfly:.  
+0001e460: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0001e470: 7365 745f 6275 7474 6572 666c 7928 5472  set_butterfly(Tr
+0001e480: 7565 290a 2020 2020 2020 2020 656c 7365  ue).        else
+0001e490: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0001e4a0: 6c66 2e6d 6e65 2e70 6c74 2e73 6574 5952  lf.mne.plt.setYR
+0001e4b0: 616e 6765 2830 2c20 7365 6c66 2e6d 6e65  ange(0, self.mne
+0001e4c0: 2e6e 5f63 6861 6e6e 656c 7320 2b20 312c  .n_channels + 1,
+0001e4d0: 2070 6164 6469 6e67 3d30 290a 0a20 2020   padding=0)..   
+0001e4e0: 2020 2020 2023 2053 6574 2053 697a 650a       # Set Size.
+0001e4f0: 2020 2020 2020 2020 7769 6474 6820 3d20          width = 
+0001e500: 696e 7428 7365 6c66 2e6d 6e65 2e66 6967  int(self.mne.fig
+0001e510: 7369 7a65 5b30 5d20 2a20 7365 6c66 2e6c  size[0] * self.l
+0001e520: 6f67 6963 616c 4470 6958 2829 290a 2020  ogicalDpiX()).  
+0001e530: 2020 2020 2020 6865 6967 6874 203d 2069        height = i
+0001e540: 6e74 2873 656c 662e 6d6e 652e 6669 6773  nt(self.mne.figs
+0001e550: 697a 655b 315d 202a 2073 656c 662e 6c6f  ize[1] * self.lo
+0001e560: 6769 6361 6c44 7069 5928 2929 0a20 2020  gicalDpiY()).   
+0001e570: 2020 2020 2073 656c 662e 7265 7369 7a65       self.resize
+0001e580: 2877 6964 7468 2c20 6865 6967 6874 290a  (width, height).
+0001e590: 0a20 2020 2020 2020 2023 2049 6e69 7469  .        # Initi
+0001e5a0: 616c 697a 6520 4b65 7962 6f61 7264 2d53  alize Keyboard-S
+0001e5b0: 686f 7274 6375 7473 0a20 2020 2020 2020  hortcuts.       
+0001e5c0: 2069 735f 6d61 6320 3d20 706c 6174 666f   is_mac = platfo
+0001e5d0: 726d 2e73 7973 7465 6d28 2920 3d3d 2027  rm.system() == '
+0001e5e0: 4461 7277 696e 270a 2020 2020 2020 2020  Darwin'.        
+0001e5f0: 6475 725f 6b65 7973 203d 2028 2766 6e20  dur_keys = ('fn 
+0001e600: 2b20 e286 9027 2c20 2766 6e20 2b20 e286  + ...', 'fn + ..
+0001e610: 9227 2920 6966 2069 735f 6d61 6320 656c  .') if is_mac el
+0001e620: 7365 2028 2748 6f6d 6527 2c20 2745 6e64  se ('Home', 'End
+0001e630: 2729 0a20 2020 2020 2020 2063 685f 6b65  ').        ch_ke
+0001e640: 7973 203d 2028 2766 6e20 2b20 e286 9127  ys = ('fn + ...'
+0001e650: 2c20 2766 6e20 2b20 e286 9327 2920 6966  , 'fn + ...') if
+0001e660: 2069 735f 6d61 6320 656c 7365 2028 2750   is_mac else ('P
+0001e670: 6167 6520 7570 272c 2027 5061 6765 2064  age up', 'Page d
+0001e680: 6f77 6e27 290a 2020 2020 2020 2020 6873  own').        hs
+0001e690: 6372 6f6c 6c5f 7479 7065 203d 2027 3120  croll_type = '1 
+0001e6a0: 6570 6f63 6827 2069 6620 7365 6c66 2e6d  epoch' if self.m
+0001e6b0: 6e65 2e69 735f 6570 6f63 6873 2065 6c73  ne.is_epochs els
+0001e6c0: 6520 27c2 bc20 7061 6765 270a 0a20 2020  e '.. page'..   
+0001e6d0: 2020 2020 2073 656c 662e 6d6e 652e 6b65       self.mne.ke
+0001e6e0: 7962 6f61 7264 5f73 686f 7274 6375 7473  yboard_shortcuts
+0001e6f0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+0001e700: 2027 6c65 6674 273a 207b 0a20 2020 2020   'left': {.     
+0001e710: 2020 2020 2020 2020 2020 2027 616c 6961             'alia
+0001e720: 7327 3a20 27e2 8690 272c 0a20 2020 2020  s': '...',.     
+0001e730: 2020 2020 2020 2020 2020 2027 7174 5f6b             'qt_k
+0001e740: 6579 273a 2051 742e 4b65 795f 4c65 6674  ey': Qt.Key_Left
+0001e750: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001e760: 2020 276d 6f64 6966 6965 7227 3a20 5b4e    'modifier': [N
+0001e770: 6f6e 652c 2027 5368 6966 7427 5d2c 0a20  one, 'Shift'],. 
+0001e780: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001e790: 736c 6f74 273a 205b 7365 6c66 2e68 7363  slot': [self.hsc
+0001e7a0: 726f 6c6c 5d2c 0a20 2020 2020 2020 2020  roll],.         
+0001e7b0: 2020 2020 2020 2027 7061 7261 6d65 7465         'paramete
+0001e7c0: 7227 3a20 5b27 6c65 6674 272c 2027 2d66  r': ['left', '-f
+0001e7d0: 756c 6c27 5d2c 0a20 2020 2020 2020 2020  ull'],.         
+0001e7e0: 2020 2020 2020 2027 6465 7363 7269 7074         'descript
+0001e7f0: 696f 6e27 3a20 5b66 2753 6372 6f6c 6c20  ion': [f'Scroll 
+0001e800: 6c65 6674 2028 7b68 7363 726f 6c6c 5f74  left ({hscroll_t
+0001e810: 7970 657d 2927 2c0a 2020 2020 2020 2020  ype})',.        
 0001e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e830: 2753 6372 6f6c 6c20 6c65 6674 2028 6675  'Scroll left (fu
-0001e840: 6c6c 2070 6167 6529 275d 0a20 2020 2020  ll page)'].     
-0001e850: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-0001e860: 2020 2020 2020 2772 6967 6874 273a 207b        'right': {
-0001e870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e880: 2027 616c 6961 7327 3a20 27e2 8692 272c   'alias': '...',
-0001e890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e8a0: 2027 7174 5f6b 6579 273a 2051 742e 4b65   'qt_key': Qt.Ke
-0001e8b0: 795f 5269 6768 742c 0a20 2020 2020 2020  y_Right,.       
-0001e8c0: 2020 2020 2020 2020 2027 6d6f 6469 6669           'modifi
-0001e8d0: 6572 273a 205b 4e6f 6e65 2c20 2753 6869  er': [None, 'Shi
-0001e8e0: 6674 275d 2c0a 2020 2020 2020 2020 2020  ft'],.          
-0001e8f0: 2020 2020 2020 2773 6c6f 7427 3a20 5b73        'slot': [s
-0001e900: 656c 662e 6873 6372 6f6c 6c5d 2c0a 2020  elf.hscroll],.  
-0001e910: 2020 2020 2020 2020 2020 2020 2020 2770                'p
-0001e920: 6172 616d 6574 6572 273a 205b 3430 2c20  arameter': [40, 
-0001e930: 272b 6675 6c6c 275d 2c0a 2020 2020 2020  '+full'],.      
-0001e940: 2020 2020 2020 2020 2020 2764 6573 6372            'descr
-0001e950: 6970 7469 6f6e 273a 205b 6627 5363 726f  iption': [f'Scro
-0001e960: 6c6c 2072 6967 6874 2028 7b68 7363 726f  ll right ({hscro
-0001e970: 6c6c 5f74 7970 657d 2927 2c0a 2020 2020  ll_type})',.    
-0001e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e990: 2020 2020 2020 2020 2020 2020 2753 6372              'Scr
-0001e9a0: 6f6c 6c20 7269 6768 7420 2866 756c 6c20  oll right (full 
-0001e9b0: 7061 6765 2927 5d0a 2020 2020 2020 2020  page)'].        
-0001e9c0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-0001e9d0: 2020 2027 7570 273a 207b 0a20 2020 2020     'up': {.     
-0001e9e0: 2020 2020 2020 2020 2020 2027 616c 6961             'alia
-0001e9f0: 7327 3a20 27e2 8691 272c 0a20 2020 2020  s': '...',.     
-0001ea00: 2020 2020 2020 2020 2020 2027 7174 5f6b             'qt_k
-0001ea10: 6579 273a 2051 742e 4b65 795f 5570 2c0a  ey': Qt.Key_Up,.
-0001ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea30: 2773 6c6f 7427 3a20 5b73 656c 662e 7673  'slot': [self.vs
-0001ea40: 6372 6f6c 6c5d 2c0a 2020 2020 2020 2020  croll],.        
-0001ea50: 2020 2020 2020 2020 2770 6172 616d 6574          'paramet
-0001ea60: 6572 273a 205b 272d 6675 6c6c 275d 2c0a  er': ['-full'],.
-0001ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea80: 2764 6573 6372 6970 7469 6f6e 273a 205b  'description': [
-0001ea90: 2753 6372 6f6c 6c20 7570 2028 6675 6c6c  'Scroll up (full
-0001eaa0: 2070 6167 6529 275d 0a20 2020 2020 2020   page)'].       
-0001eab0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-0001eac0: 2020 2020 2764 6f77 6e27 3a20 7b0a 2020      'down': {.  
-0001ead0: 2020 2020 2020 2020 2020 2020 2020 2761                'a
-0001eae0: 6c69 6173 273a 2027 e286 9327 2c0a 2020  lias': '...',.  
-0001eaf0: 2020 2020 2020 2020 2020 2020 2020 2771                'q
-0001eb00: 745f 6b65 7927 3a20 5174 2e4b 6579 5f44  t_key': Qt.Key_D
-0001eb10: 6f77 6e2c 0a20 2020 2020 2020 2020 2020  own,.           
-0001eb20: 2020 2020 2027 736c 6f74 273a 205b 7365       'slot': [se
-0001eb30: 6c66 2e76 7363 726f 6c6c 5d2c 0a20 2020  lf.vscroll],.   
-0001eb40: 2020 2020 2020 2020 2020 2020 2027 7061               'pa
-0001eb50: 7261 6d65 7465 7227 3a20 5b27 2b66 756c  rameter': ['+ful
-0001eb60: 6c27 5d2c 0a20 2020 2020 2020 2020 2020  l'],.           
-0001eb70: 2020 2020 2027 6465 7363 7269 7074 696f       'descriptio
-0001eb80: 6e27 3a20 5b27 5363 726f 6c6c 2064 6f77  n': ['Scroll dow
-0001eb90: 6e20 2866 756c 6c20 7061 6765 2927 5d0a  n (full page)'].
-0001eba0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-0001ebb0: 2020 2020 2020 2020 2020 2027 686f 6d65             'home
-0001ebc0: 273a 207b 0a20 2020 2020 2020 2020 2020  ': {.           
-0001ebd0: 2020 2020 2027 616c 6961 7327 3a20 6475       'alias': du
-0001ebe0: 725f 6b65 7973 5b30 5d2c 0a20 2020 2020  r_keys[0],.     
-0001ebf0: 2020 2020 2020 2020 2020 2027 7174 5f6b             'qt_k
-0001ec00: 6579 273a 2051 742e 4b65 795f 486f 6d65  ey': Qt.Key_Home
-0001ec10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001ec20: 2020 276b 7727 3a20 2773 7465 7027 2c0a    'kw': 'step',.
-0001ec30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ec40: 2773 6c6f 7427 3a20 5b73 656c 662e 6368  'slot': [self.ch
-0001ec50: 616e 6765 5f64 7572 6174 696f 6e5d 2c0a  ange_duration],.
-0001ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ec70: 2770 6172 616d 6574 6572 273a 205b 2d30  'parameter': [-0
-0001ec80: 2e32 5d2c 0a20 2020 2020 2020 2020 2020  .2],.           
-0001ec90: 2020 2020 2027 6465 7363 7269 7074 696f       'descriptio
-0001eca0: 6e27 3a20 5b66 2744 6563 7265 6173 6520  n': [f'Decrease 
-0001ecb0: 6475 7261 7469 6f6e 2028 7b68 7363 726f  duration ({hscro
-0001ecc0: 6c6c 5f74 7970 657d 2927 5d0a 2020 2020  ll_type})'].    
-0001ecd0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-0001ece0: 2020 2020 2020 2027 656e 6427 3a20 7b0a         'end': {.
-0001ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ed00: 2761 6c69 6173 273a 2064 7572 5f6b 6579  'alias': dur_key
-0001ed10: 735b 315d 2c0a 2020 2020 2020 2020 2020  s[1],.          
-0001ed20: 2020 2020 2020 2771 745f 6b65 7927 3a20        'qt_key': 
-0001ed30: 5174 2e4b 6579 5f45 6e64 2c0a 2020 2020  Qt.Key_End,.    
-0001ed40: 2020 2020 2020 2020 2020 2020 276b 7727              'kw'
-0001ed50: 3a20 2773 7465 7027 2c0a 2020 2020 2020  : 'step',.      
-0001ed60: 2020 2020 2020 2020 2020 2773 6c6f 7427            'slot'
-0001ed70: 3a20 5b73 656c 662e 6368 616e 6765 5f64  : [self.change_d
-0001ed80: 7572 6174 696f 6e5d 2c0a 2020 2020 2020  uration],.      
-0001ed90: 2020 2020 2020 2020 2020 2770 6172 616d            'param
-0001eda0: 6574 6572 273a 205b 302e 3235 5d2c 0a20  eter': [0.25],. 
-0001edb0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0001edc0: 6465 7363 7269 7074 696f 6e27 3a20 5b66  description': [f
-0001edd0: 2749 6e63 7265 6173 6520 6475 7261 7469  'Increase durati
-0001ede0: 6f6e 2028 7b68 7363 726f 6c6c 5f74 7970  on ({hscroll_typ
-0001edf0: 657d 2927 5d0a 2020 2020 2020 2020 2020  e})'].          
-0001ee00: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-0001ee10: 2027 7061 6765 646f 776e 273a 207b 0a20   'pagedown': {. 
-0001ee20: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0001ee30: 616c 6961 7327 3a20 6368 5f6b 6579 735b  alias': ch_keys[
-0001ee40: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
-0001ee50: 2020 2020 2771 745f 6b65 7927 3a20 5174      'qt_key': Qt
-0001ee60: 2e4b 6579 5f50 6167 6544 6f77 6e2c 0a20  .Key_PageDown,. 
-0001ee70: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0001ee80: 6d6f 6469 6669 6572 273a 205b 4e6f 6e65  modifier': [None
-0001ee90: 2c20 2753 6869 6674 275d 2c0a 2020 2020  , 'Shift'],.    
-0001eea0: 2020 2020 2020 2020 2020 2020 276b 7727              'kw'
-0001eeb0: 3a20 2773 7465 7027 2c0a 2020 2020 2020  : 'step',.      
-0001eec0: 2020 2020 2020 2020 2020 2773 6c6f 7427            'slot'
-0001eed0: 3a20 5b73 656c 662e 6368 616e 6765 5f6e  : [self.change_n
-0001eee0: 6368 616e 5d2c 0a20 2020 2020 2020 2020  chan],.         
-0001eef0: 2020 2020 2020 2027 7061 7261 6d65 7465         'paramete
-0001ef00: 7227 3a20 5b2d 312c 202d 3130 5d2c 0a20  r': [-1, -10],. 
-0001ef10: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0001ef20: 6465 7363 7269 7074 696f 6e27 3a20 5b27  description': ['
-0001ef30: 4465 6372 6561 7365 2073 686f 776e 2063  Decrease shown c
-0001ef40: 6861 6e6e 656c 7320 2831 2927 2c0a 2020  hannels (1)',.  
-0001ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef60: 2020 2020 2020 2020 2020 2020 2020 2744                'D
-0001ef70: 6563 7265 6173 6520 7368 6f77 6e20 6368  ecrease shown ch
-0001ef80: 616e 6e65 6c73 2028 3130 2927 5d0a 2020  annels (10)'].  
-0001ef90: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-0001efa0: 2020 2020 2020 2020 2027 7061 6765 7570           'pageup
-0001efb0: 273a 207b 0a20 2020 2020 2020 2020 2020  ': {.           
-0001efc0: 2020 2020 2027 616c 6961 7327 3a20 6368       'alias': ch
-0001efd0: 5f6b 6579 735b 315d 2c0a 2020 2020 2020  _keys[1],.      
-0001efe0: 2020 2020 2020 2020 2020 2771 745f 6b65            'qt_ke
-0001eff0: 7927 3a20 5174 2e4b 6579 5f50 6167 6555  y': Qt.Key_PageU
-0001f000: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
-0001f010: 2020 2027 6d6f 6469 6669 6572 273a 205b     'modifier': [
-0001f020: 4e6f 6e65 2c20 2753 6869 6674 275d 2c0a  None, 'Shift'],.
-0001f030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f040: 276b 7727 3a20 2773 7465 7027 2c0a 2020  'kw': 'step',.  
-0001f050: 2020 2020 2020 2020 2020 2020 2020 2773                's
-0001f060: 6c6f 7427 3a20 5b73 656c 662e 6368 616e  lot': [self.chan
-0001f070: 6765 5f6e 6368 616e 5d2c 0a20 2020 2020  ge_nchan],.     
-0001f080: 2020 2020 2020 2020 2020 2027 7061 7261             'para
-0001f090: 6d65 7465 7227 3a20 5b31 2c20 3130 5d2c  meter': [1, 10],
-0001f0a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f0b0: 2027 6465 7363 7269 7074 696f 6e27 3a20   'description': 
-0001f0c0: 5b27 496e 6372 6561 7365 2073 686f 776e  ['Increase shown
-0001f0d0: 2063 6861 6e6e 656c 7320 2831 2927 2c0a   channels (1)',.
-0001f0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e830: 2020 2020 2020 2020 2753 6372 6f6c 6c20          'Scroll 
+0001e840: 6c65 6674 2028 6675 6c6c 2070 6167 6529  left (full page)
+0001e850: 275d 0a20 2020 2020 2020 2020 2020 207d  '].            }
+0001e860: 2c0a 2020 2020 2020 2020 2020 2020 2772  ,.            'r
+0001e870: 6967 6874 273a 207b 0a20 2020 2020 2020  ight': {.       
+0001e880: 2020 2020 2020 2020 2027 616c 6961 7327           'alias'
+0001e890: 3a20 27e2 8692 272c 0a20 2020 2020 2020  : '...',.       
+0001e8a0: 2020 2020 2020 2020 2027 7174 5f6b 6579           'qt_key
+0001e8b0: 273a 2051 742e 4b65 795f 5269 6768 742c  ': Qt.Key_Right,
+0001e8c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e8d0: 2027 6d6f 6469 6669 6572 273a 205b 4e6f   'modifier': [No
+0001e8e0: 6e65 2c20 2753 6869 6674 275d 2c0a 2020  ne, 'Shift'],.  
+0001e8f0: 2020 2020 2020 2020 2020 2020 2020 2773                's
+0001e900: 6c6f 7427 3a20 5b73 656c 662e 6873 6372  lot': [self.hscr
+0001e910: 6f6c 6c5d 2c0a 2020 2020 2020 2020 2020  oll],.          
+0001e920: 2020 2020 2020 2770 6172 616d 6574 6572        'parameter
+0001e930: 273a 205b 2772 6967 6874 272c 2027 2b66  ': ['right', '+f
+0001e940: 756c 6c27 5d2c 0a20 2020 2020 2020 2020  ull'],.         
+0001e950: 2020 2020 2020 2027 6465 7363 7269 7074         'descript
+0001e960: 696f 6e27 3a20 5b66 2753 6372 6f6c 6c20  ion': [f'Scroll 
+0001e970: 7269 6768 7420 287b 6873 6372 6f6c 6c5f  right ({hscroll_
+0001e980: 7479 7065 7d29 272c 0a20 2020 2020 2020  type})',.       
+0001e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e9a0: 2020 2020 2020 2020 2027 5363 726f 6c6c           'Scroll
+0001e9b0: 2072 6967 6874 2028 6675 6c6c 2070 6167   right (full pag
+0001e9c0: 6529 275d 0a20 2020 2020 2020 2020 2020  e)'].           
+0001e9d0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+0001e9e0: 2775 7027 3a20 7b0a 2020 2020 2020 2020  'up': {.        
+0001e9f0: 2020 2020 2020 2020 2761 6c69 6173 273a          'alias':
+0001ea00: 2027 e286 9127 2c0a 2020 2020 2020 2020   '...',.        
+0001ea10: 2020 2020 2020 2020 2771 745f 6b65 7927          'qt_key'
+0001ea20: 3a20 5174 2e4b 6579 5f55 702c 0a20 2020  : Qt.Key_Up,.   
+0001ea30: 2020 2020 2020 2020 2020 2020 2027 736c               'sl
+0001ea40: 6f74 273a 205b 7365 6c66 2e76 7363 726f  ot': [self.vscro
+0001ea50: 6c6c 5d2c 0a20 2020 2020 2020 2020 2020  ll],.           
+0001ea60: 2020 2020 2027 7061 7261 6d65 7465 7227       'parameter'
+0001ea70: 3a20 5b27 2d66 756c 6c27 5d2c 0a20 2020  : ['-full'],.   
+0001ea80: 2020 2020 2020 2020 2020 2020 2027 6465               'de
+0001ea90: 7363 7269 7074 696f 6e27 3a20 5b27 5363  scription': ['Sc
+0001eaa0: 726f 6c6c 2075 7020 2866 756c 6c20 7061  roll up (full pa
+0001eab0: 6765 2927 5d0a 2020 2020 2020 2020 2020  ge)'].          
+0001eac0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+0001ead0: 2027 646f 776e 273a 207b 0a20 2020 2020   'down': {.     
+0001eae0: 2020 2020 2020 2020 2020 2027 616c 6961             'alia
+0001eaf0: 7327 3a20 27e2 8693 272c 0a20 2020 2020  s': '...',.     
+0001eb00: 2020 2020 2020 2020 2020 2027 7174 5f6b             'qt_k
+0001eb10: 6579 273a 2051 742e 4b65 795f 446f 776e  ey': Qt.Key_Down
+0001eb20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001eb30: 2020 2773 6c6f 7427 3a20 5b73 656c 662e    'slot': [self.
+0001eb40: 7673 6372 6f6c 6c5d 2c0a 2020 2020 2020  vscroll],.      
+0001eb50: 2020 2020 2020 2020 2020 2770 6172 616d            'param
+0001eb60: 6574 6572 273a 205b 272b 6675 6c6c 275d  eter': ['+full']
+0001eb70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001eb80: 2020 2764 6573 6372 6970 7469 6f6e 273a    'description':
+0001eb90: 205b 2753 6372 6f6c 6c20 646f 776e 2028   ['Scroll down (
+0001eba0: 6675 6c6c 2070 6167 6529 275d 0a20 2020  full page)'].   
+0001ebb0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+0001ebc0: 2020 2020 2020 2020 2768 6f6d 6527 3a20          'home': 
+0001ebd0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+0001ebe0: 2020 2761 6c69 6173 273a 2064 7572 5f6b    'alias': dur_k
+0001ebf0: 6579 735b 305d 2c0a 2020 2020 2020 2020  eys[0],.        
+0001ec00: 2020 2020 2020 2020 2771 745f 6b65 7927          'qt_key'
+0001ec10: 3a20 5174 2e4b 6579 5f48 6f6d 652c 0a20  : Qt.Key_Home,. 
+0001ec20: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001ec30: 6b77 273a 2027 7374 6570 272c 0a20 2020  kw': 'step',.   
+0001ec40: 2020 2020 2020 2020 2020 2020 2027 736c               'sl
+0001ec50: 6f74 273a 205b 7365 6c66 2e63 6861 6e67  ot': [self.chang
+0001ec60: 655f 6475 7261 7469 6f6e 5d2c 0a20 2020  e_duration],.   
+0001ec70: 2020 2020 2020 2020 2020 2020 2027 7061               'pa
+0001ec80: 7261 6d65 7465 7227 3a20 5b2d 302e 325d  rameter': [-0.2]
+0001ec90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001eca0: 2020 2764 6573 6372 6970 7469 6f6e 273a    'description':
+0001ecb0: 205b 6627 4465 6372 6561 7365 2064 7572   [f'Decrease dur
+0001ecc0: 6174 696f 6e20 287b 6873 6372 6f6c 6c5f  ation ({hscroll_
+0001ecd0: 7479 7065 7d29 275d 0a20 2020 2020 2020  type})'].       
+0001ece0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+0001ecf0: 2020 2020 2765 6e64 273a 207b 0a20 2020      'end': {.   
+0001ed00: 2020 2020 2020 2020 2020 2020 2027 616c               'al
+0001ed10: 6961 7327 3a20 6475 725f 6b65 7973 5b31  ias': dur_keys[1
+0001ed20: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0001ed30: 2020 2027 7174 5f6b 6579 273a 2051 742e     'qt_key': Qt.
+0001ed40: 4b65 795f 456e 642c 0a20 2020 2020 2020  Key_End,.       
+0001ed50: 2020 2020 2020 2020 2027 6b77 273a 2027           'kw': '
+0001ed60: 7374 6570 272c 0a20 2020 2020 2020 2020  step',.         
+0001ed70: 2020 2020 2020 2027 736c 6f74 273a 205b         'slot': [
+0001ed80: 7365 6c66 2e63 6861 6e67 655f 6475 7261  self.change_dura
+0001ed90: 7469 6f6e 5d2c 0a20 2020 2020 2020 2020  tion],.         
+0001eda0: 2020 2020 2020 2027 7061 7261 6d65 7465         'paramete
+0001edb0: 7227 3a20 5b30 2e32 355d 2c0a 2020 2020  r': [0.25],.    
+0001edc0: 2020 2020 2020 2020 2020 2020 2764 6573              'des
+0001edd0: 6372 6970 7469 6f6e 273a 205b 6627 496e  cription': [f'In
+0001ede0: 6372 6561 7365 2064 7572 6174 696f 6e20  crease duration 
+0001edf0: 287b 6873 6372 6f6c 6c5f 7479 7065 7d29  ({hscroll_type})
+0001ee00: 275d 0a20 2020 2020 2020 2020 2020 207d  '].            }
+0001ee10: 2c0a 2020 2020 2020 2020 2020 2020 2770  ,.            'p
+0001ee20: 6167 6564 6f77 6e27 3a20 7b0a 2020 2020  agedown': {.    
+0001ee30: 2020 2020 2020 2020 2020 2020 2761 6c69              'ali
+0001ee40: 6173 273a 2063 685f 6b65 7973 5b30 5d2c  as': ch_keys[0],
+0001ee50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ee60: 2027 7174 5f6b 6579 273a 2051 742e 4b65   'qt_key': Qt.Ke
+0001ee70: 795f 5061 6765 446f 776e 2c0a 2020 2020  y_PageDown,.    
+0001ee80: 2020 2020 2020 2020 2020 2020 276d 6f64              'mod
+0001ee90: 6966 6965 7227 3a20 5b4e 6f6e 652c 2027  ifier': [None, '
+0001eea0: 5368 6966 7427 5d2c 0a20 2020 2020 2020  Shift'],.       
+0001eeb0: 2020 2020 2020 2020 2027 6b77 273a 2027           'kw': '
+0001eec0: 7374 6570 272c 0a20 2020 2020 2020 2020  step',.         
+0001eed0: 2020 2020 2020 2027 736c 6f74 273a 205b         'slot': [
+0001eee0: 7365 6c66 2e63 6861 6e67 655f 6e63 6861  self.change_ncha
+0001eef0: 6e5d 2c0a 2020 2020 2020 2020 2020 2020  n],.            
+0001ef00: 2020 2020 2770 6172 616d 6574 6572 273a      'parameter':
+0001ef10: 205b 2d31 2c20 2d31 305d 2c0a 2020 2020   [-1, -10],.    
+0001ef20: 2020 2020 2020 2020 2020 2020 2764 6573              'des
+0001ef30: 6372 6970 7469 6f6e 273a 205b 2744 6563  cription': ['Dec
+0001ef40: 7265 6173 6520 7368 6f77 6e20 6368 616e  rease shown chan
+0001ef50: 6e65 6c73 2028 3129 272c 0a20 2020 2020  nels (1)',.     
+0001ef60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ef70: 2020 2020 2020 2020 2020 2027 4465 6372             'Decr
+0001ef80: 6561 7365 2073 686f 776e 2063 6861 6e6e  ease shown chann
+0001ef90: 656c 7320 2831 3029 275d 0a20 2020 2020  els (10)'].     
+0001efa0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+0001efb0: 2020 2020 2020 2770 6167 6575 7027 3a20        'pageup': 
+0001efc0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+0001efd0: 2020 2761 6c69 6173 273a 2063 685f 6b65    'alias': ch_ke
+0001efe0: 7973 5b31 5d2c 0a20 2020 2020 2020 2020  ys[1],.         
+0001eff0: 2020 2020 2020 2027 7174 5f6b 6579 273a         'qt_key':
+0001f000: 2051 742e 4b65 795f 5061 6765 5570 2c0a   Qt.Key_PageUp,.
+0001f010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f020: 276d 6f64 6966 6965 7227 3a20 5b4e 6f6e  'modifier': [Non
+0001f030: 652c 2027 5368 6966 7427 5d2c 0a20 2020  e, 'Shift'],.   
+0001f040: 2020 2020 2020 2020 2020 2020 2027 6b77               'kw
+0001f050: 273a 2027 7374 6570 272c 0a20 2020 2020  ': 'step',.     
+0001f060: 2020 2020 2020 2020 2020 2027 736c 6f74             'slot
+0001f070: 273a 205b 7365 6c66 2e63 6861 6e67 655f  ': [self.change_
+0001f080: 6e63 6861 6e5d 2c0a 2020 2020 2020 2020  nchan],.        
+0001f090: 2020 2020 2020 2020 2770 6172 616d 6574          'paramet
+0001f0a0: 6572 273a 205b 312c 2031 305d 2c0a 2020  er': [1, 10],.  
+0001f0b0: 2020 2020 2020 2020 2020 2020 2020 2764                'd
+0001f0c0: 6573 6372 6970 7469 6f6e 273a 205b 2749  escription': ['I
+0001f0d0: 6e63 7265 6173 6520 7368 6f77 6e20 6368  ncrease shown ch
+0001f0e0: 616e 6e65 6c73 2028 3129 272c 0a20 2020  annels (1)',.   
 0001f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f100: 2749 6e63 7265 6173 6520 7368 6f77 6e20  'Increase shown 
-0001f110: 6368 616e 6e65 6c73 2028 3130 2927 5d0a  channels (10)'].
-0001f120: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-0001f130: 2020 2020 2020 2020 2020 2027 2d27 3a20             '-': 
-0001f140: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-0001f150: 2020 2771 745f 6b65 7927 3a20 5174 2e4b    'qt_key': Qt.K
-0001f160: 6579 5f4d 696e 7573 2c0a 2020 2020 2020  ey_Minus,.      
-0001f170: 2020 2020 2020 2020 2020 2773 6c6f 7427            'slot'
-0001f180: 3a20 5b73 656c 662e 7363 616c 655f 616c  : [self.scale_al
-0001f190: 6c5d 2c0a 2020 2020 2020 2020 2020 2020  l],.            
-0001f1a0: 2020 2020 276b 7727 3a20 2773 7465 7027      'kw': 'step'
-0001f1b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001f1c0: 2020 2770 6172 616d 6574 6572 273a 205b    'parameter': [
-0001f1d0: 3420 2f20 355d 2c0a 2020 2020 2020 2020  4 / 5],.        
-0001f1e0: 2020 2020 2020 2020 2764 6573 6372 6970          'descrip
-0001f1f0: 7469 6f6e 273a 205b 2744 6563 7265 6173  tion': ['Decreas
-0001f200: 6520 5363 616c 6527 5d0a 2020 2020 2020  e Scale'].      
-0001f210: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-0001f220: 2020 2020 2027 2b27 3a20 7b0a 2020 2020       '+': {.    
-0001f230: 2020 2020 2020 2020 2020 2020 2771 745f              'qt_
-0001f240: 6b65 7927 3a20 5174 2e4b 6579 5f50 6c75  key': Qt.Key_Plu
-0001f250: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0001f260: 2020 2027 736c 6f74 273a 205b 7365 6c66     'slot': [self
-0001f270: 2e73 6361 6c65 5f61 6c6c 5d2c 0a20 2020  .scale_all],.   
-0001f280: 2020 2020 2020 2020 2020 2020 2027 6b77               'kw
-0001f290: 273a 2027 7374 6570 272c 0a20 2020 2020  ': 'step',.     
-0001f2a0: 2020 2020 2020 2020 2020 2027 7061 7261             'para
-0001f2b0: 6d65 7465 7227 3a20 5b35 202f 2034 5d2c  meter': [5 / 4],
-0001f2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f2d0: 2027 6465 7363 7269 7074 696f 6e27 3a20   'description': 
-0001f2e0: 5b27 496e 6372 6561 7365 2053 6361 6c65  ['Increase Scale
-0001f2f0: 275d 0a20 2020 2020 2020 2020 2020 207d  '].            }
-0001f300: 2c0a 2020 2020 2020 2020 2020 2020 273d  ,.            '=
-0001f310: 273a 207b 0a20 2020 2020 2020 2020 2020  ': {.           
-0001f320: 2020 2020 2027 7174 5f6b 6579 273a 2051       'qt_key': Q
-0001f330: 742e 4b65 795f 4571 7561 6c2c 0a20 2020  t.Key_Equal,.   
-0001f340: 2020 2020 2020 2020 2020 2020 2027 736c               'sl
-0001f350: 6f74 273a 205b 7365 6c66 2e73 6361 6c65  ot': [self.scale
-0001f360: 5f61 6c6c 5d2c 0a20 2020 2020 2020 2020  _all],.         
-0001f370: 2020 2020 2020 2027 6b77 273a 2027 7374         'kw': 'st
-0001f380: 6570 272c 0a20 2020 2020 2020 2020 2020  ep',.           
-0001f390: 2020 2020 2027 7061 7261 6d65 7465 7227       'parameter'
-0001f3a0: 3a20 5b35 202f 2034 5d2c 0a20 2020 2020  : [5 / 4],.     
-0001f3b0: 2020 2020 2020 2020 2020 2027 6465 7363             'desc
-0001f3c0: 7269 7074 696f 6e27 3a20 5b27 496e 6372  ription': ['Incr
-0001f3d0: 6561 7365 2053 6361 6c65 275d 0a20 2020  ease Scale'].   
-0001f3e0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-0001f3f0: 2020 2020 2020 2020 2761 273a 207b 0a20          'a': {. 
-0001f400: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0001f410: 7174 5f6b 6579 273a 2051 742e 4b65 795f  qt_key': Qt.Key_
-0001f420: 412c 0a20 2020 2020 2020 2020 2020 2020  A,.             
-0001f430: 2020 2027 736c 6f74 273a 205b 7365 6c66     'slot': [self
-0001f440: 2e5f 746f 6767 6c65 5f61 6e6e 6f74 6174  ._toggle_annotat
-0001f450: 696f 6e5f 6669 672c 0a20 2020 2020 2020  ion_fig,.       
-0001f460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f470: 2020 7365 6c66 2e5f 746f 6767 6c65 5f61    self._toggle_a
-0001f480: 6e6e 6f74 6174 696f 6e73 5d2c 0a20 2020  nnotations],.   
-0001f490: 2020 2020 2020 2020 2020 2020 2027 6d6f               'mo
-0001f4a0: 6469 6669 6572 273a 205b 4e6f 6e65 2c20  difier': [None, 
-0001f4b0: 2753 6869 6674 275d 2c0a 2020 2020 2020  'Shift'],.      
-0001f4c0: 2020 2020 2020 2020 2020 2764 6573 6372            'descr
-0001f4d0: 6970 7469 6f6e 273a 205b 2754 6f67 676c  iption': ['Toggl
-0001f4e0: 6520 416e 6e6f 7461 7469 6f6e 2d54 6f6f  e Annotation-Too
-0001f4f0: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
-0001f500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f510: 2020 2020 2754 6f67 676c 6520 416e 6e6f      'Toggle Anno
-0001f520: 7461 7469 6f6e 7320 7669 7369 626c 6527  tations visible'
-0001f530: 5d0a 2020 2020 2020 2020 2020 2020 7d2c  ].            },
-0001f540: 0a20 2020 2020 2020 2020 2020 2027 6227  .            'b'
-0001f550: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-0001f560: 2020 2020 2771 745f 6b65 7927 3a20 5174      'qt_key': Qt
-0001f570: 2e4b 6579 5f42 2c0a 2020 2020 2020 2020  .Key_B,.        
-0001f580: 2020 2020 2020 2020 2773 6c6f 7427 3a20          'slot': 
-0001f590: 5b73 656c 662e 5f74 6f67 676c 655f 6275  [self._toggle_bu
-0001f5a0: 7474 6572 666c 795d 2c0a 2020 2020 2020  tterfly],.      
-0001f5b0: 2020 2020 2020 2020 2020 2764 6573 6372            'descr
-0001f5c0: 6970 7469 6f6e 273a 205b 2754 6f67 676c  iption': ['Toggl
-0001f5d0: 6520 4275 7474 6572 666c 7927 5d0a 2020  e Butterfly'].  
-0001f5e0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-0001f5f0: 2020 2020 2020 2020 2027 6427 3a20 7b0a           'd': {.
-0001f600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f610: 2771 745f 6b65 7927 3a20 5174 2e4b 6579  'qt_key': Qt.Key
-0001f620: 5f44 2c0a 2020 2020 2020 2020 2020 2020  _D,.            
-0001f630: 2020 2020 2773 6c6f 7427 3a20 5b73 656c      'slot': [sel
-0001f640: 662e 5f74 6f67 676c 655f 6463 5d2c 0a20  f._toggle_dc],. 
-0001f650: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0001f660: 6465 7363 7269 7074 696f 6e27 3a20 5b27  description': ['
-0001f670: 546f 6767 6c65 2044 432d 436f 7272 6563  Toggle DC-Correc
-0001f680: 7469 6f6e 275d 0a20 2020 2020 2020 2020  tion'].         
-0001f690: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-0001f6a0: 2020 2765 273a 207b 0a20 2020 2020 2020    'e': {.       
-0001f6b0: 2020 2020 2020 2020 2027 7174 5f6b 6579           'qt_key
-0001f6c0: 273a 2051 742e 4b65 795f 452c 0a20 2020  ': Qt.Key_E,.   
-0001f6d0: 2020 2020 2020 2020 2020 2020 2027 736c               'sl
-0001f6e0: 6f74 273a 205b 7365 6c66 2e5f 746f 6767  ot': [self._togg
-0001f6f0: 6c65 5f65 7665 6e74 735d 2c0a 2020 2020  le_events],.    
-0001f700: 2020 2020 2020 2020 2020 2020 2764 6573              'des
-0001f710: 6372 6970 7469 6f6e 273a 205b 2754 6f67  cription': ['Tog
-0001f720: 676c 6520 4576 656e 7473 2076 6973 6962  gle Events visib
-0001f730: 6c65 275d 0a20 2020 2020 2020 2020 2020  le'].           
-0001f740: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-0001f750: 2768 273a 207b 0a20 2020 2020 2020 2020  'h': {.         
-0001f760: 2020 2020 2020 2027 7174 5f6b 6579 273a         'qt_key':
-0001f770: 2051 742e 4b65 795f 482c 0a20 2020 2020   Qt.Key_H,.     
-0001f780: 2020 2020 2020 2020 2020 2027 736c 6f74             'slot
-0001f790: 273a 205b 7365 6c66 2e5f 746f 6767 6c65  ': [self._toggle
-0001f7a0: 5f65 706f 6368 5f68 6973 746f 6772 616d  _epoch_histogram
-0001f7b0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0001f7c0: 2020 2027 6465 7363 7269 7074 696f 6e27     'description'
-0001f7d0: 3a20 5b27 546f 6767 6c65 2045 706f 6368  : ['Toggle Epoch
-0001f7e0: 2d48 6973 746f 6772 616d 275d 0a20 2020  -Histogram'].   
-0001f7f0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-0001f800: 2020 2020 2020 2020 276a 273a 207b 0a20          'j': {. 
-0001f810: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0001f820: 7174 5f6b 6579 273a 2051 742e 4b65 795f  qt_key': Qt.Key_
-0001f830: 4a2c 0a20 2020 2020 2020 2020 2020 2020  J,.             
-0001f840: 2020 2027 736c 6f74 273a 205b 7365 6c66     'slot': [self
-0001f850: 2e5f 746f 6767 6c65 5f70 726f 6a5f 6669  ._toggle_proj_fi
-0001f860: 672c 0a20 2020 2020 2020 2020 2020 2020  g,.             
-0001f870: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001f880: 2e5f 746f 6767 6c65 5f61 6c6c 5f70 726f  ._toggle_all_pro
-0001f890: 6a73 5d2c 0a20 2020 2020 2020 2020 2020  js],.           
-0001f8a0: 2020 2020 2027 6d6f 6469 6669 6572 273a       'modifier':
-0001f8b0: 205b 4e6f 6e65 2c20 2753 6869 6674 275d   [None, 'Shift']
-0001f8c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001f8d0: 2020 2764 6573 6372 6970 7469 6f6e 273a    'description':
-0001f8e0: 205b 2754 6f67 676c 6520 5072 6f6a 6563   ['Toggle Projec
-0001f8f0: 7469 6f6e 2046 6967 7572 6527 2c0a 2020  tion Figure',.  
-0001f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f910: 2020 2020 2020 2020 2020 2020 2020 2754                'T
-0001f920: 6f67 676c 6520 616c 6c20 7072 6f6a 6563  oggle all projec
-0001f930: 7469 6f6e 7327 5d0a 2020 2020 2020 2020  tions'].        
-0001f940: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-0001f950: 2020 2027 6c27 3a20 7b0a 2020 2020 2020     'l': {.      
-0001f960: 2020 2020 2020 2020 2020 2771 745f 6b65            'qt_ke
-0001f970: 7927 3a20 5174 2e4b 6579 5f4c 2c0a 2020  y': Qt.Key_L,.  
-0001f980: 2020 2020 2020 2020 2020 2020 2020 2773                's
-0001f990: 6c6f 7427 3a20 5b73 656c 662e 5f74 6f67  lot': [self._tog
-0001f9a0: 676c 655f 616e 7469 616c 6961 7369 6e67  gle_antialiasing
-0001f9b0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0001f9c0: 2020 2027 6465 7363 7269 7074 696f 6e27     'description'
-0001f9d0: 3a20 5b27 546f 6767 6c65 2041 6e74 6961  : ['Toggle Antia
-0001f9e0: 6c69 6173 696e 6727 5d0a 2020 2020 2020  liasing'].      
-0001f9f0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-0001fa00: 2020 2020 2027 6f27 3a20 7b0a 2020 2020       'o': {.    
-0001fa10: 2020 2020 2020 2020 2020 2020 2771 745f              'qt_
-0001fa20: 6b65 7927 3a20 5174 2e4b 6579 5f4f 2c0a  key': Qt.Key_O,.
-0001fa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fa40: 2773 6c6f 7427 3a20 5b73 656c 662e 5f74  'slot': [self._t
-0001fa50: 6f67 676c 655f 6f76 6572 7669 6577 5f62  oggle_overview_b
-0001fa60: 6172 5d2c 0a20 2020 2020 2020 2020 2020  ar],.           
-0001fa70: 2020 2020 2027 6465 7363 7269 7074 696f       'descriptio
-0001fa80: 6e27 3a20 5b27 546f 6767 6c65 204f 7665  n': ['Toggle Ove
-0001fa90: 7276 6965 772d 4261 7227 5d0a 2020 2020  rview-Bar'].    
-0001faa0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-0001fab0: 2020 2020 2020 2027 7427 3a20 7b0a 2020         't': {.  
-0001fac0: 2020 2020 2020 2020 2020 2020 2020 2771                'q
-0001fad0: 745f 6b65 7927 3a20 5174 2e4b 6579 5f54  t_key': Qt.Key_T
-0001fae0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001faf0: 2020 2773 6c6f 7427 3a20 5b73 656c 662e    'slot': [self.
-0001fb00: 5f74 6f67 676c 655f 7469 6d65 5f66 6f72  _toggle_time_for
-0001fb10: 6d61 745d 2c0a 2020 2020 2020 2020 2020  mat],.          
-0001fb20: 2020 2020 2020 2764 6573 6372 6970 7469        'descripti
-0001fb30: 6f6e 273a 205b 2754 6f67 676c 6520 5469  on': ['Toggle Ti
-0001fb40: 6d65 2d46 6f72 6d61 7427 5d0a 2020 2020  me-Format'].    
-0001fb50: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-0001fb60: 2020 2020 2020 2027 7327 3a20 7b0a 2020         's': {.  
-0001fb70: 2020 2020 2020 2020 2020 2020 2020 2771                'q
-0001fb80: 745f 6b65 7927 3a20 5174 2e4b 6579 5f53  t_key': Qt.Key_S
-0001fb90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001fba0: 2020 2773 6c6f 7427 3a20 5b73 656c 662e    'slot': [self.
-0001fbb0: 5f74 6f67 676c 655f 7363 616c 6562 6172  _toggle_scalebar
-0001fbc0: 735d 2c0a 2020 2020 2020 2020 2020 2020  s],.            
-0001fbd0: 2020 2020 2764 6573 6372 6970 7469 6f6e      'description
-0001fbe0: 273a 205b 2754 6f67 676c 6520 5363 616c  ': ['Toggle Scal
-0001fbf0: 6562 6172 7327 5d0a 2020 2020 2020 2020  ebars'].        
-0001fc00: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-0001fc10: 2020 2027 7727 3a20 7b0a 2020 2020 2020     'w': {.      
-0001fc20: 2020 2020 2020 2020 2020 2771 745f 6b65            'qt_ke
-0001fc30: 7927 3a20 5174 2e4b 6579 5f57 2c0a 2020  y': Qt.Key_W,.  
-0001fc40: 2020 2020 2020 2020 2020 2020 2020 2773                's
-0001fc50: 6c6f 7427 3a20 5b73 656c 662e 5f74 6f67  lot': [self._tog
-0001fc60: 676c 655f 7768 6974 656e 696e 675d 2c0a  gle_whitening],.
-0001fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fc80: 2764 6573 6372 6970 7469 6f6e 273a 205b  'description': [
-0001fc90: 2754 6f67 676c 6520 5768 6974 656e 696e  'Toggle Whitenin
-0001fca0: 6727 5d0a 2020 2020 2020 2020 2020 2020  g'].            
-0001fcb0: 7d2c 0a20 2020 2020 2020 2020 2020 2027  },.            '
-0001fcc0: 7827 3a20 7b0a 2020 2020 2020 2020 2020  x': {.          
-0001fcd0: 2020 2020 2020 2771 745f 6b65 7927 3a20        'qt_key': 
-0001fce0: 5174 2e4b 6579 5f58 2c0a 2020 2020 2020  Qt.Key_X,.      
-0001fcf0: 2020 2020 2020 2020 2020 2773 6c6f 7427            'slot'
-0001fd00: 3a20 5b73 656c 662e 5f74 6f67 676c 655f  : [self._toggle_
-0001fd10: 6372 6f73 7368 6169 725d 2c0a 2020 2020  crosshair],.    
-0001fd20: 2020 2020 2020 2020 2020 2020 2764 6573              'des
-0001fd30: 6372 6970 7469 6f6e 273a 205b 2754 6f67  cription': ['Tog
-0001fd40: 676c 6520 4372 6f73 7368 6169 7227 5d0a  gle Crosshair'].
-0001fd50: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-0001fd60: 2020 2020 2020 2020 2020 2027 7a27 3a20             'z': 
-0001fd70: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-0001fd80: 2020 2771 745f 6b65 7927 3a20 5174 2e4b    'qt_key': Qt.K
-0001fd90: 6579 5f5a 2c0a 2020 2020 2020 2020 2020  ey_Z,.          
-0001fda0: 2020 2020 2020 2773 6c6f 7427 3a20 5b73        'slot': [s
-0001fdb0: 656c 662e 5f74 6f67 676c 655f 7a65 6e6d  elf._toggle_zenm
-0001fdc0: 6f64 655d 2c0a 2020 2020 2020 2020 2020  ode],.          
-0001fdd0: 2020 2020 2020 2764 6573 6372 6970 7469        'descripti
-0001fde0: 6f6e 273a 205b 2754 6f67 676c 6520 5a65  on': ['Toggle Ze
-0001fdf0: 6e2d 4d6f 6465 275d 0a20 2020 2020 2020  n-Mode'].       
-0001fe00: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-0001fe10: 2020 2020 273f 273a 207b 0a20 2020 2020      '?': {.     
-0001fe20: 2020 2020 2020 2020 2020 2027 7174 5f6b             'qt_k
-0001fe30: 6579 273a 2051 742e 4b65 795f 5175 6573  ey': Qt.Key_Ques
-0001fe40: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
-0001fe50: 2020 2020 2020 2773 6c6f 7427 3a20 5b73        'slot': [s
-0001fe60: 656c 662e 5f74 6f67 676c 655f 6865 6c70  elf._toggle_help
-0001fe70: 5f66 6967 5d2c 0a20 2020 2020 2020 2020  _fig],.         
-0001fe80: 2020 2020 2020 2027 6465 7363 7269 7074         'descript
-0001fe90: 696f 6e27 3a20 5b27 5368 6f77 2048 656c  ion': ['Show Hel
-0001fea0: 7027 5d0a 2020 2020 2020 2020 2020 2020  p'].            
-0001feb0: 7d2c 0a20 2020 2020 2020 2020 2020 2027  },.            '
-0001fec0: 6631 3127 3a20 7b0a 2020 2020 2020 2020  f11': {.        
-0001fed0: 2020 2020 2020 2020 2771 745f 6b65 7927          'qt_key'
-0001fee0: 3a20 5174 2e4b 6579 5f46 3131 2c0a 2020  : Qt.Key_F11,.  
-0001fef0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-0001ff00: 6c6f 7427 3a20 5b73 656c 662e 5f74 6f67  lot': [self._tog
-0001ff10: 676c 655f 6675 6c6c 7363 7265 656e 5d2c  gle_fullscreen],
-0001ff20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ff30: 2027 6465 7363 7269 7074 696f 6e27 3a20   'description': 
-0001ff40: 5b27 546f 6767 6c65 2046 756c 6c2d 5363  ['Toggle Full-Sc
-0001ff50: 7265 656e 275d 0a20 2020 2020 2020 2020  reen'].         
-0001ff60: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-0001ff70: 2020 2765 7363 6170 6527 3a20 7b0a 2020    'escape': {.  
-0001ff80: 2020 2020 2020 2020 2020 2020 2020 2771                'q
-0001ff90: 745f 6b65 7927 3a20 5174 2e4b 6579 5f45  t_key': Qt.Key_E
-0001ffa0: 7363 6170 652c 0a20 2020 2020 2020 2020  scape,.         
-0001ffb0: 2020 2020 2020 2027 736c 6f74 273a 205b         'slot': [
-0001ffc0: 7365 6c66 2e5f 6368 6563 6b5f 636c 6f73  self._check_clos
-0001ffd0: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
-0001ffe0: 2020 2020 2764 6573 6372 6970 7469 6f6e      'description
-0001fff0: 273a 205b 2743 6c6f 7365 275d 0a20 2020  ': ['Close'].   
-00020000: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00020010: 2020 2020 2020 2020 2320 4a75 7374 2066          # Just f
-00020020: 6f72 2074 6573 7469 6e67 0a20 2020 2020  or testing.     
-00020030: 2020 2020 2020 2027 656e 7465 7227 3a20         'enter': 
-00020040: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00020050: 2020 2771 745f 6b65 7927 3a20 5174 2e4b    'qt_key': Qt.K
-00020060: 6579 5f45 6e74 6572 0a20 2020 2020 2020  ey_Enter.       
-00020070: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00020080: 2020 2020 2720 273a 207b 0a20 2020 2020      ' ': {.     
-00020090: 2020 2020 2020 2020 2020 2027 7174 5f6b             'qt_k
-000200a0: 6579 273a 2051 742e 4b65 795f 5370 6163  ey': Qt.Key_Spac
-000200b0: 650a 2020 2020 2020 2020 2020 2020 7d0a  e.            }.
-000200c0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000200d0: 2020 6966 2073 656c 662e 6d6e 652e 6973    if self.mne.is
-000200e0: 5f65 706f 6368 733a 0a20 2020 2020 2020  _epochs:.       
-000200f0: 2020 2020 2023 2044 6973 6162 6c65 2074       # Disable t
-00020100: 696d 6520 666f 726d 6174 2074 6f67 676c  ime format toggl
-00020110: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00020120: 6465 6c20 7365 6c66 2e6d 6e65 2e6b 6579  del self.mne.key
-00020130: 626f 6172 645f 7368 6f72 7463 7574 735b  board_shortcuts[
-00020140: 2774 275d 0a0a 2020 2020 6465 6620 5f68  't']..    def _h
-00020150: 6964 7069 5f6d 6b50 656e 2873 656c 662c  idpi_mkPen(self,
-00020160: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-00020170: 293a 0a20 2020 2020 2020 206b 7761 7267  ):.        kwarg
-00020180: 735b 2777 6964 7468 275d 203d 2073 656c  s['width'] = sel
-00020190: 662e 5f70 6978 656c 5f72 6174 696f 202a  f._pixel_ratio *
-000201a0: 206b 7761 7267 732e 6765 7428 2777 6964   kwargs.get('wid
-000201b0: 7468 272c 2031 2e29 0a20 2020 2020 2020  th', 1.).       
-000201c0: 2072 6574 7572 6e20 6d6b 5065 6e28 2a61   return mkPen(*a
-000201d0: 7267 732c 202a 2a6b 7761 7267 7329 0a0a  rgs, **kwargs)..
-000201e0: 2020 2020 6465 6620 5f75 7064 6174 655f      def _update_
-000201f0: 7961 7869 735f 6c61 6265 6c73 2873 656c  yaxis_labels(sel
-00020200: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00020210: 2e6d 6e65 2e63 6861 6e6e 656c 5f61 7869  .mne.channel_axi
-00020220: 732e 7265 7061 696e 7428 290a 0a20 2020  s.repaint()..   
-00020230: 2064 6566 205f 6164 645f 7363 616c 6562   def _add_scaleb
-00020240: 6172 7328 7365 6c66 293a 0a20 2020 2020  ars(self):.     
-00020250: 2020 2022 2222 4164 6420 7363 616c 6562     """Add scaleb
-00020260: 6172 7320 666f 7220 616c 6c20 6368 616e  ars for all chan
-00020270: 6e65 6c2d 7479 7065 732e 0a0a 2020 2020  nel-types...    
-00020280: 2020 2020 2873 6365 6e65 2068 616e 646c      (scene handl
-00020290: 6573 2073 686f 7769 6e67 2074 6865 6d20  es showing them 
-000202a0: 696e 2077 6865 6e20 696e 2076 6965 770a  in when in view.
-000202b0: 2020 2020 2020 2020 7261 6e67 6529 0a20          range). 
-000202c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000202d0: 2020 2073 656c 662e 6d6e 652e 7363 616c     self.mne.scal
-000202e0: 6562 6172 732e 636c 6561 7228 290a 2020  ebars.clear().  
-000202f0: 2020 2020 2020 2320 546f 206b 6565 7020        # To keep 
-00020300: 6f72 6465 7220 286e 702e 756e 6971 7565  order (np.unique
-00020310: 2073 6f72 7473 290a 2020 2020 2020 2020   sorts).        
-00020320: 6f72 6465 7265 645f 7479 7065 7320 3d20  ordered_types = 
-00020330: 7365 6c66 2e6d 6e65 2e63 685f 7479 7065  self.mne.ch_type
-00020340: 735b 7365 6c66 2e6d 6e65 2e63 685f 6f72  s[self.mne.ch_or
-00020350: 6465 725d 0a20 2020 2020 2020 2075 6e69  der].        uni
-00020360: 7175 655f 7479 7065 5f69 6478 7320 3d20  que_type_idxs = 
-00020370: 6e70 2e75 6e69 7175 6528 6f72 6465 7265  np.unique(ordere
-00020380: 645f 7479 7065 732c 0a20 2020 2020 2020  d_types,.       
-00020390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000203a0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000203b0: 7475 726e 5f69 6e64 6578 3d54 7275 6529  turn_index=True)
-000203c0: 5b31 5d0a 2020 2020 2020 2020 6368 5f74  [1].        ch_t
-000203d0: 7970 6573 5f6f 7264 6572 6564 203d 205b  ypes_ordered = [
-000203e0: 6f72 6465 7265 645f 7479 7065 735b 6964  ordered_types[id
-000203f0: 785d 2066 6f72 2069 6478 0a20 2020 2020  x] for idx.     
-00020400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020410: 2020 2020 2020 2069 6e20 736f 7274 6564         in sorted
-00020420: 2875 6e69 7175 655f 7479 7065 5f69 6478  (unique_type_idx
-00020430: 7329 5d0a 2020 2020 2020 2020 666f 7220  s)].        for 
-00020440: 6368 5f74 7970 6520 696e 205b 6374 2066  ch_type in [ct f
-00020450: 6f72 2063 7420 696e 2063 685f 7479 7065  or ct in ch_type
-00020460: 735f 6f72 6465 7265 640a 2020 2020 2020  s_ordered.      
-00020470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020480: 2020 6966 2063 7420 213d 2027 7374 696d    if ct != 'stim
-00020490: 2720 616e 640a 2020 2020 2020 2020 2020  ' and.          
-000204a0: 2020 2020 2020 2020 2020 2020 2020 6374                ct
-000204b0: 2069 6e20 7365 6c66 2e6d 6e65 2e73 6361   in self.mne.sca
-000204c0: 6c69 6e67 7320 616e 640a 2020 2020 2020  lings and.      
-000204d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000204e0: 2020 6374 2069 6e20 6765 7461 7474 7228    ct in getattr(
-000204f0: 7365 6c66 2e6d 6e65 2c20 2775 6e69 7473  self.mne, 'units
-00020500: 272c 207b 7d29 2061 6e64 0a20 2020 2020  ', {}) and.     
-00020510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020520: 2020 2063 7420 696e 2067 6574 6174 7472     ct in getattr
-00020530: 2873 656c 662e 6d6e 652c 2027 756e 6974  (self.mne, 'unit
-00020540: 5f73 6361 6c69 6e67 7327 2c20 7b7d 295d  _scalings', {})]
-00020550: 3a0a 2020 2020 2020 2020 2020 2020 7363  :.            sc
-00020560: 616c 655f 6261 7220 3d20 5363 616c 6542  ale_bar = ScaleB
-00020570: 6172 2873 656c 662e 6d6e 652c 2063 685f  ar(self.mne, ch_
-00020580: 7479 7065 290a 2020 2020 2020 2020 2020  type).          
-00020590: 2020 7365 6c66 2e6d 6e65 2e73 6361 6c65    self.mne.scale
-000205a0: 6261 7273 5b63 685f 7479 7065 5d20 3d20  bars[ch_type] = 
-000205b0: 7363 616c 655f 6261 720a 2020 2020 2020  scale_bar.      
-000205c0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e70        self.mne.p
-000205d0: 6c74 2e61 6464 4974 656d 2873 6361 6c65  lt.addItem(scale
-000205e0: 5f62 6172 290a 0a20 2020 2020 2020 2020  _bar)..         
-000205f0: 2020 2073 6361 6c65 5f62 6172 5f74 6578     scale_bar_tex
-00020600: 7420 3d20 5363 616c 6542 6172 5465 7874  t = ScaleBarText
-00020610: 2873 656c 662e 6d6e 652c 2063 685f 7479  (self.mne, ch_ty
-00020620: 7065 290a 2020 2020 2020 2020 2020 2020  pe).            
-00020630: 7365 6c66 2e6d 6e65 2e73 6361 6c65 6261  self.mne.scaleba
-00020640: 725f 7465 7874 735b 6368 5f74 7970 655d  r_texts[ch_type]
-00020650: 203d 2073 6361 6c65 5f62 6172 5f74 6578   = scale_bar_tex
-00020660: 740a 2020 2020 2020 2020 2020 2020 7365  t.            se
-00020670: 6c66 2e6d 6e65 2e70 6c74 2e61 6464 4974  lf.mne.plt.addIt
-00020680: 656d 2873 6361 6c65 5f62 6172 5f74 6578  em(scale_bar_tex
-00020690: 7429 0a0a 2020 2020 2020 2020 7365 6c66  t)..        self
-000206a0: 2e5f 7365 745f 7363 616c 6562 6172 735f  ._set_scalebars_
-000206b0: 7669 7369 626c 6528 7365 6c66 2e6d 6e65  visible(self.mne
-000206c0: 2e73 6361 6c65 6261 7273 5f76 6973 6962  .scalebars_visib
-000206d0: 6c65 290a 0a20 2020 2064 6566 205f 7570  le)..    def _up
-000206e0: 6461 7465 5f73 6361 6c65 6261 725f 785f  date_scalebar_x_
-000206f0: 706f 7369 7469 6f6e 7328 7365 6c66 293a  positions(self):
-00020700: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00020710: 2e6d 6e65 2e73 6361 6c65 6261 7273 5f76  .mne.scalebars_v
-00020720: 6973 6962 6c65 3a0a 2020 2020 2020 2020  isible:.        
-00020730: 2020 2020 666f 7220 7363 616c 6562 6172      for scalebar
-00020740: 2069 6e20 7365 6c66 2e6d 6e65 2e73 6361   in self.mne.sca
-00020750: 6c65 6261 7273 2e76 616c 7565 7328 293a  lebars.values():
-00020760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020770: 2073 6361 6c65 6261 722e 7570 6461 7465   scalebar.update
-00020780: 5f78 5f70 6f73 6974 696f 6e28 290a 0a20  _x_position().. 
-00020790: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-000207a0: 6361 6c65 6261 725f 7465 7874 2069 6e20  calebar_text in 
-000207b0: 7365 6c66 2e6d 6e65 2e73 6361 6c65 6261  self.mne.scaleba
-000207c0: 725f 7465 7874 732e 7661 6c75 6573 2829  r_texts.values()
-000207d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000207e0: 2020 7363 616c 6562 6172 5f74 6578 742e    scalebar_text.
-000207f0: 7570 6461 7465 5f78 5f70 6f73 6974 696f  update_x_positio
-00020800: 6e28 290a 0a20 2020 2064 6566 205f 7570  n()..    def _up
-00020810: 6461 7465 5f73 6361 6c65 6261 725f 795f  date_scalebar_y_
-00020820: 706f 7369 7469 6f6e 7328 7365 6c66 293a  positions(self):
-00020830: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00020840: 2e6d 6e65 2e73 6361 6c65 6261 7273 5f76  .mne.scalebars_v
-00020850: 6973 6962 6c65 3a0a 2020 2020 2020 2020  isible:.        
-00020860: 2020 2020 666f 7220 7363 616c 6562 6172      for scalebar
-00020870: 2069 6e20 7365 6c66 2e6d 6e65 2e73 6361   in self.mne.sca
-00020880: 6c65 6261 7273 2e76 616c 7565 7328 293a  lebars.values():
-00020890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000208a0: 2073 6361 6c65 6261 722e 7570 6461 7465   scalebar.update
-000208b0: 5f79 5f70 6f73 6974 696f 6e28 290a 0a20  _y_position().. 
-000208c0: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-000208d0: 6361 6c65 6261 725f 7465 7874 2069 6e20  calebar_text in 
-000208e0: 7365 6c66 2e6d 6e65 2e73 6361 6c65 6261  self.mne.scaleba
-000208f0: 725f 7465 7874 732e 7661 6c75 6573 2829  r_texts.values()
-00020900: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00020910: 2020 7363 616c 6562 6172 5f74 6578 742e    scalebar_text.
-00020920: 7570 6461 7465 5f79 5f70 6f73 6974 696f  update_y_positio
-00020930: 6e28 290a 0a20 2020 2064 6566 205f 7570  n()..    def _up
-00020940: 6461 7465 5f73 6361 6c65 6261 725f 7661  date_scalebar_va
-00020950: 6c75 6573 2873 656c 6629 3a0a 2020 2020  lues(self):.    
-00020960: 2020 2020 666f 7220 7363 616c 6562 6172      for scalebar
-00020970: 5f74 6578 7420 696e 2073 656c 662e 6d6e  _text in self.mn
-00020980: 652e 7363 616c 6562 6172 5f74 6578 7473  e.scalebar_texts
-00020990: 2e76 616c 7565 7328 293a 0a20 2020 2020  .values():.     
-000209a0: 2020 2020 2020 2073 6361 6c65 6261 725f         scalebar_
-000209b0: 7465 7874 2e75 7064 6174 655f 7661 6c75  text.update_valu
-000209c0: 6528 290a 0a20 2020 2064 6566 205f 7365  e()..    def _se
-000209d0: 745f 7363 616c 6562 6172 735f 7669 7369  t_scalebars_visi
-000209e0: 626c 6528 7365 6c66 2c20 7669 7369 626c  ble(self, visibl
-000209f0: 6529 3a0a 2020 2020 2020 2020 666f 7220  e):.        for 
-00020a00: 7363 616c 6562 6172 2069 6e20 7365 6c66  scalebar in self
-00020a10: 2e6d 6e65 2e73 6361 6c65 6261 7273 2e76  .mne.scalebars.v
-00020a20: 616c 7565 7328 293a 0a20 2020 2020 2020  alues():.       
-00020a30: 2020 2020 2073 6361 6c65 6261 722e 7365       scalebar.se
-00020a40: 7456 6973 6962 6c65 2876 6973 6962 6c65  tVisible(visible
-00020a50: 290a 0a20 2020 2020 2020 2066 6f72 2073  )..        for s
-00020a60: 6361 6c65 6261 725f 7465 7874 2069 6e20  calebar_text in 
-00020a70: 7365 6c66 2e6d 6e65 2e73 6361 6c65 6261  self.mne.scaleba
-00020a80: 725f 7465 7874 732e 7661 6c75 6573 2829  r_texts.values()
-00020a90: 3a0a 2020 2020 2020 2020 2020 2020 7363  :.            sc
-00020aa0: 616c 6562 6172 5f74 6578 742e 7365 7456  alebar_text.setV
-00020ab0: 6973 6962 6c65 2876 6973 6962 6c65 290a  isible(visible).
-00020ac0: 0a20 2020 2020 2020 2073 656c 662e 5f75  .        self._u
-00020ad0: 7064 6174 655f 7363 616c 6562 6172 5f79  pdate_scalebar_y
-00020ae0: 5f70 6f73 6974 696f 6e73 2829 0a0a 2020  _positions()..  
-00020af0: 2020 6465 6620 5f74 6f67 676c 655f 7363    def _toggle_sc
-00020b00: 616c 6562 6172 7328 7365 6c66 293a 0a20  alebars(self):. 
-00020b10: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-00020b20: 7363 616c 6562 6172 735f 7669 7369 626c  scalebars_visibl
-00020b30: 6520 3d20 6e6f 7420 7365 6c66 2e6d 6e65  e = not self.mne
-00020b40: 2e73 6361 6c65 6261 7273 5f76 6973 6962  .scalebars_visib
-00020b50: 6c65 0a20 2020 2020 2020 2073 656c 662e  le.        self.
-00020b60: 5f73 6574 5f73 6361 6c65 6261 7273 5f76  _set_scalebars_v
-00020b70: 6973 6962 6c65 2873 656c 662e 6d6e 652e  isible(self.mne.
-00020b80: 7363 616c 6562 6172 735f 7669 7369 626c  scalebars_visibl
-00020b90: 6529 0a0a 2020 2020 6465 6620 5f6f 7665  e)..    def _ove
-00020ba0: 7276 6965 775f 6d6f 6465 5f63 6861 6e67  rview_mode_chang
-00020bb0: 6564 2873 656c 662c 206e 6577 5f6d 6f64  ed(self, new_mod
-00020bc0: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-00020bd0: 2e6d 6e65 2e6f 7665 7276 6965 775f 6d6f  .mne.overview_mo
-00020be0: 6465 203d 206e 6577 5f6d 6f64 650a 2020  de = new_mode.  
-00020bf0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e6f        self.mne.o
-00020c00: 7665 7276 6965 775f 6261 722e 7365 745f  verview_bar.set_
-00020c10: 6261 636b 6772 6f75 6e64 2829 0a20 2020  background().   
-00020c20: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00020c30: 2e6d 6e65 2e6f 7665 7276 6965 775f 6261  .mne.overview_ba
-00020c40: 722e 6973 5669 7369 626c 6528 293a 0a20  r.isVisible():. 
-00020c50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00020c60: 5f74 6f67 676c 655f 6f76 6572 7669 6577  _toggle_overview
-00020c70: 5f62 6172 2829 0a0a 2020 2020 6465 6620  _bar()..    def 
-00020c80: 5f6f 7665 7276 6965 775f 7261 6469 6f5f  _overview_radio_
-00020c90: 636c 6963 6b65 6428 7365 6c66 2c20 6368  clicked(self, ch
-00020ca0: 6563 6b65 642c 202a 2c20 6d65 6e75 2c20  ecked, *, menu, 
-00020cb0: 6e65 775f 6d6f 6465 293a 0a20 2020 2020  new_mode):.     
-00020cc0: 2020 206d 656e 752e 636c 6f73 6528 290a     menu.close().
-00020cd0: 2020 2020 2020 2020 7365 6c66 2e5f 6f76          self._ov
-00020ce0: 6572 7669 6577 5f6d 6f64 655f 6368 616e  erview_mode_chan
-00020cf0: 6765 6428 6e65 775f 6d6f 6465 3d6e 6577  ged(new_mode=new
-00020d00: 5f6d 6f64 6529 0a0a 2020 2020 6465 6620  _mode)..    def 
-00020d10: 7363 616c 655f 616c 6c28 7365 6c66 2c20  scale_all(self, 
-00020d20: 6368 6563 6b65 643d 4661 6c73 652c 202a  checked=False, *
-00020d30: 2c20 7374 6570 293a 0a20 2020 2020 2020  , step):.       
-00020d40: 2022 2222 5363 616c 6520 616c 6c20 7472   """Scale all tr
-00020d50: 6163 6573 2062 7920 6d75 6c74 6970 6c79  aces by multiply
-00020d60: 696e 6720 7769 7468 2073 7465 702e 2222  ing with step.""
-00020d70: 220a 2020 2020 2020 2020 7365 6c66 2e6d  ".        self.m
-00020d80: 6e65 2e73 6361 6c65 5f66 6163 746f 7220  ne.scale_factor 
-00020d90: 2a3d 2073 7465 700a 0a20 2020 2020 2020  *= step..       
-00020da0: 2023 2052 6561 7070 6c79 2063 6c69 7070   # Reapply clipp
-00020db0: 696e 6720 6966 206e 6563 6573 7361 7279  ing if necessary
-00020dc0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00020dd0: 2e6d 6e65 2e63 6c69 7070 696e 6720 6973  .mne.clipping is
-00020de0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00020df0: 2020 2020 2020 2073 656c 662e 5f75 7064         self._upd
-00020e00: 6174 655f 6461 7461 2829 0a0a 2020 2020  ate_data()..    
-00020e10: 2020 2020 2320 5363 616c 6520 5472 6163      # Scale Trac
-00020e20: 6573 2028 6279 2073 6361 6c69 6e67 2074  es (by scaling t
-00020e30: 6865 2049 7465 6d2c 206e 6f74 2074 6865  he Item, not the
-00020e40: 2064 6174 6129 0a20 2020 2020 2020 2066   data).        f
-00020e50: 6f72 206c 696e 6520 696e 2073 656c 662e  or line in self.
-00020e60: 6d6e 652e 7472 6163 6573 3a0a 2020 2020  mne.traces:.    
-00020e70: 2020 2020 2020 2020 6c69 6e65 2e75 7064          line.upd
-00020e80: 6174 655f 7363 616c 6528 290a 0a20 2020  ate_scale()..   
-00020e90: 2020 2020 2023 2055 7064 6174 6520 5363       # Update Sc
-00020ea0: 616c 6562 6172 730a 2020 2020 2020 2020  alebars.        
-00020eb0: 7365 6c66 2e5f 7570 6461 7465 5f73 6361  self._update_sca
-00020ec0: 6c65 6261 725f 7661 6c75 6573 2829 0a0a  lebar_values()..
-00020ed0: 2020 2020 6465 6620 6873 6372 6f6c 6c28      def hscroll(
-00020ee0: 7365 6c66 2c20 7374 6570 293a 0a20 2020  self, step):.   
-00020ef0: 2020 2020 2022 2222 5363 726f 6c6c 2068       """Scroll h
-00020f00: 6f72 697a 6f6e 7461 6c6c 7920 6279 2073  orizontally by s
-00020f10: 7465 702e 2222 220a 2020 2020 2020 2020  tep.""".        
-00020f20: 6966 2073 7465 7020 3d3d 2027 2b66 756c  if step == '+ful
-00020f30: 6c27 3a0a 2020 2020 2020 2020 2020 2020  l':.            
-00020f40: 7265 6c5f 7374 6570 203d 2073 656c 662e  rel_step = self.
-00020f50: 6d6e 652e 6475 7261 7469 6f6e 0a20 2020  mne.duration.   
-00020f60: 2020 2020 2065 6c69 6620 7374 6570 203d       elif step =
-00020f70: 3d20 272d 6675 6c6c 273a 0a20 2020 2020  = '-full':.     
-00020f80: 2020 2020 2020 2072 656c 5f73 7465 7020         rel_step 
-00020f90: 3d20 2d20 7365 6c66 2e6d 6e65 2e64 7572  = - self.mne.dur
-00020fa0: 6174 696f 6e0a 2020 2020 2020 2020 656c  ation.        el
-00020fb0: 6966 2073 656c 662e 6d6e 652e 6973 5f65  if self.mne.is_e
-00020fc0: 706f 6368 733a 0a20 2020 2020 2020 2020  pochs:.         
-00020fd0: 2020 2064 6972 6563 7469 6f6e 203d 2031     direction = 1
-00020fe0: 2069 6620 7374 6570 203e 2030 2065 6c73   if step > 0 els
-00020ff0: 6520 2d31 0a20 2020 2020 2020 2020 2020  e -1.           
-00021000: 2072 656c 5f73 7465 7020 3d20 6469 7265   rel_step = dire
-00021010: 6374 696f 6e20 2a20 7365 6c66 2e6d 6e65  ction * self.mne
-00021020: 2e64 7572 6174 696f 6e20 2f20 7365 6c66  .duration / self
-00021030: 2e6d 6e65 2e6e 5f65 706f 6368 730a 2020  .mne.n_epochs.  
-00021040: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00021050: 2020 2020 2020 2020 7265 6c5f 7374 6570          rel_step
-00021060: 203d 2073 7465 7020 2a20 7365 6c66 2e6d   = step * self.m
-00021070: 6e65 2e64 7572 6174 696f 6e20 2f20 7365  ne.duration / se
-00021080: 6c66 2e6d 6e65 2e73 6372 6f6c 6c5f 7365  lf.mne.scroll_se
-00021090: 6e73 6974 6976 6974 790a 2020 2020 2020  nsitivity.      
-000210a0: 2020 2320 4765 7420 6375 7272 656e 7420    # Get current 
-000210b0: 7261 6e67 6520 616e 6420 6164 6420 7374  range and add st
-000210c0: 6570 2074 6f20 6974 0a20 2020 2020 2020  ep to it.       
-000210d0: 2078 6d69 6e2c 2078 6d61 7820 3d20 5b69   xmin, xmax = [i
-000210e0: 202b 2072 656c 5f73 7465 7020 666f 7220   + rel_step for 
-000210f0: 6920 696e 2073 656c 662e 6d6e 652e 7669  i in self.mne.vi
-00021100: 6577 626f 782e 7669 6577 5261 6e67 6528  ewbox.viewRange(
-00021110: 295b 305d 5d0a 0a20 2020 2020 2020 2069  )[0]]..        i
-00021120: 6620 786d 696e 203c 2030 3a0a 2020 2020  f xmin < 0:.    
-00021130: 2020 2020 2020 2020 786d 696e 203d 2030          xmin = 0
-00021140: 0a20 2020 2020 2020 2020 2020 2078 6d61  .            xma
-00021150: 7820 3d20 786d 696e 202b 2073 656c 662e  x = xmin + self.
-00021160: 6d6e 652e 6475 7261 7469 6f6e 0a20 2020  mne.duration.   
-00021170: 2020 2020 2065 6c69 6620 786d 6178 203e       elif xmax >
-00021180: 2073 656c 662e 6d6e 652e 786d 6178 3a0a   self.mne.xmax:.
-00021190: 2020 2020 2020 2020 2020 2020 786d 6178              xmax
-000211a0: 203d 2073 656c 662e 6d6e 652e 786d 6178   = self.mne.xmax
-000211b0: 0a20 2020 2020 2020 2020 2020 2078 6d69  .            xmi
-000211c0: 6e20 3d20 786d 6178 202d 2073 656c 662e  n = xmax - self.
-000211d0: 6d6e 652e 6475 7261 7469 6f6e 0a0a 2020  mne.duration..  
-000211e0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e70        self.mne.p
-000211f0: 6c74 2e73 6574 5852 616e 6765 2878 6d69  lt.setXRange(xmi
-00021200: 6e2c 2078 6d61 782c 2070 6164 6469 6e67  n, xmax, padding
-00021210: 3d30 290a 0a20 2020 2064 6566 2076 7363  =0)..    def vsc
-00021220: 726f 6c6c 2873 656c 662c 2073 7465 7029  roll(self, step)
-00021230: 3a0a 2020 2020 2020 2020 2222 2253 6372  :.        """Scr
-00021240: 6f6c 6c20 7665 7274 6963 616c 6c79 2062  oll vertically b
-00021250: 7920 7374 6570 2e22 2222 0a20 2020 2020  y step.""".     
-00021260: 2020 2069 6620 7365 6c66 2e6d 6e65 2e66     if self.mne.f
-00021270: 6967 5f73 656c 6563 7469 6f6e 2069 7320  ig_selection is 
-00021280: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00021290: 2020 2020 2020 6966 2073 7465 7020 3d3d        if step ==
-000212a0: 2027 2b66 756c 6c27 3a0a 2020 2020 2020   '+full':.      
-000212b0: 2020 2020 2020 2020 2020 7374 6570 203d            step =
-000212c0: 2031 0a20 2020 2020 2020 2020 2020 2065   1.            e
-000212d0: 6c69 6620 7374 6570 203d 3d20 272d 6675  lif step == '-fu
-000212e0: 6c6c 273a 0a20 2020 2020 2020 2020 2020  ll':.           
-000212f0: 2020 2020 2073 7465 7020 3d20 2d31 0a20       step = -1. 
-00021300: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00021310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021320: 2073 7465 7020 3d20 696e 7428 7374 6570   step = int(step
-00021330: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00021340: 6c66 2e6d 6e65 2e66 6967 5f73 656c 6563  lf.mne.fig_selec
-00021350: 7469 6f6e 2e5f 7363 726f 6c6c 5f73 656c  tion._scroll_sel
-00021360: 6563 7469 6f6e 2873 7465 7029 0a20 2020  ection(step).   
-00021370: 2020 2020 2065 6c69 6620 7365 6c66 2e6d       elif self.m
-00021380: 6e65 2e62 7574 7465 7266 6c79 3a0a 2020  ne.butterfly:.  
-00021390: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000213a0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000213b0: 2020 2020 2020 2020 2020 2023 2047 6574             # Get
-000213c0: 2063 7572 7265 6e74 2072 616e 6765 2061   current range a
-000213d0: 6e64 2061 6464 2073 7465 7020 746f 2069  nd add step to i
-000213e0: 740a 2020 2020 2020 2020 2020 2020 6966  t.            if
-000213f0: 2073 7465 7020 3d3d 2027 2b66 756c 6c27   step == '+full'
-00021400: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00021410: 2020 7374 6570 203d 2073 656c 662e 6d6e    step = self.mn
-00021420: 652e 6e5f 6368 616e 6e65 6c73 0a20 2020  e.n_channels.   
-00021430: 2020 2020 2020 2020 2065 6c69 6620 7374           elif st
-00021440: 6570 203d 3d20 272d 6675 6c6c 273a 0a20  ep == '-full':. 
-00021450: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00021460: 7465 7020 3d20 2d20 7365 6c66 2e6d 6e65  tep = - self.mne
-00021470: 2e6e 5f63 6861 6e6e 656c 730a 2020 2020  .n_channels.    
-00021480: 2020 2020 2020 2020 796d 696e 2c20 796d          ymin, ym
-00021490: 6178 203d 205b 6920 2b20 7374 6570 2066  ax = [i + step f
-000214a0: 6f72 2069 2069 6e20 7365 6c66 2e6d 6e65  or i in self.mne
-000214b0: 2e76 6965 7762 6f78 2e76 6965 7752 616e  .viewbox.viewRan
-000214c0: 6765 2829 5b31 5d5d 0a0a 2020 2020 2020  ge()[1]]..      
-000214d0: 2020 2020 2020 6966 2079 6d69 6e20 3c20        if ymin < 
-000214e0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-000214f0: 2020 2079 6d69 6e20 3d20 300a 2020 2020     ymin = 0.    
-00021500: 2020 2020 2020 2020 2020 2020 796d 6178              ymax
-00021510: 203d 2073 656c 662e 6d6e 652e 6e5f 6368   = self.mne.n_ch
-00021520: 616e 6e65 6c73 202b 2031 0a20 2020 2020  annels + 1.     
-00021530: 2020 2020 2020 2065 6c69 6620 796d 6178         elif ymax
-00021540: 203e 2073 656c 662e 6d6e 652e 796d 6178   > self.mne.ymax
-00021550: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00021560: 2020 796d 6178 203d 2073 656c 662e 6d6e    ymax = self.mn
-00021570: 652e 796d 6178 0a20 2020 2020 2020 2020  e.ymax.         
-00021580: 2020 2020 2020 2079 6d69 6e20 3d20 796d         ymin = ym
-00021590: 6178 202d 2073 656c 662e 6d6e 652e 6e5f  ax - self.mne.n_
-000215a0: 6368 616e 6e65 6c73 202d 2031 0a0a 2020  channels - 1..  
-000215b0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-000215c0: 6e65 2e70 6c74 2e73 6574 5952 616e 6765  ne.plt.setYRange
-000215d0: 2879 6d69 6e2c 2079 6d61 782c 2070 6164  (ymin, ymax, pad
-000215e0: 6469 6e67 3d30 290a 0a20 2020 2064 6566  ding=0)..    def
-000215f0: 2063 6861 6e67 655f 6475 7261 7469 6f6e   change_duration
-00021600: 2873 656c 662c 2063 6865 636b 6564 3d46  (self, checked=F
-00021610: 616c 7365 2c20 2a2c 2073 7465 7029 3a0a  alse, *, step):.
-00021620: 2020 2020 2020 2020 2222 2243 6861 6e67          """Chang
-00021630: 6520 6475 7261 7469 6f6e 2062 7920 7374  e duration by st
-00021640: 6570 2e22 2222 0a20 2020 2020 2020 2078  ep.""".        x
-00021650: 6d69 6e2c 2078 6d61 7820 3d20 7365 6c66  min, xmax = self
-00021660: 2e6d 6e65 2e76 6965 7762 6f78 2e76 6965  .mne.viewbox.vie
-00021670: 7752 616e 6765 2829 5b30 5d0a 0a20 2020  wRange()[0]..   
-00021680: 2020 2020 2069 6620 7365 6c66 2e6d 6e65       if self.mne
-00021690: 2e69 735f 6570 6f63 6873 3a0a 2020 2020  .is_epochs:.    
-000216a0: 2020 2020 2020 2020 2320 7573 6520 7468          # use th
-000216b0: 6520 6c65 6e67 7468 206f 6620 6f6e 6520  e length of one 
-000216c0: 6570 6f63 6820 6173 2064 7572 6174 696f  epoch as duratio
-000216d0: 6e20 6368 616e 6765 0a20 2020 2020 2020  n change.       
-000216e0: 2020 2020 206d 696e 5f64 7572 203d 206c       min_dur = l
-000216f0: 656e 2873 656c 662e 6d6e 652e 696e 7374  en(self.mne.inst
-00021700: 2e74 696d 6573 2920 2f20 7365 6c66 2e6d  .times) / self.m
-00021710: 6e65 2e69 6e66 6f5b 2773 6672 6571 275d  ne.info['sfreq']
-00021720: 0a20 2020 2020 2020 2020 2020 2073 7465  .            ste
-00021730: 705f 6469 7220 3d20 2831 2069 6620 7374  p_dir = (1 if st
-00021740: 6570 203e 2030 2065 6c73 6520 2d31 290a  ep > 0 else -1).
-00021750: 2020 2020 2020 2020 2020 2020 7265 6c5f              rel_
-00021760: 7374 6570 203d 206d 696e 5f64 7572 202a  step = min_dur *
-00021770: 2073 7465 705f 6469 720a 2020 2020 2020   step_dir.      
-00021780: 2020 2020 2020 7365 6c66 2e6d 6e65 2e6e        self.mne.n
-00021790: 5f65 706f 6368 7320 3d20 6e70 2e63 6c69  _epochs = np.cli
-000217a0: 7028 7365 6c66 2e6d 6e65 2e6e 5f65 706f  p(self.mne.n_epo
-000217b0: 6368 7320 2b20 7374 6570 5f64 6972 2c0a  chs + step_dir,.
-000217c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000217d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000217e0: 2020 2020 2020 2020 312c 206c 656e 2873          1, len(s
-000217f0: 656c 662e 6d6e 652e 696e 7374 2929 0a20  elf.mne.inst)). 
-00021800: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00021810: 2020 2020 2020 2020 2023 206e 6576 6572           # never
-00021820: 2073 686f 7720 6665 7765 7220 7468 616e   show fewer than
-00021830: 2033 2073 616d 706c 6573 0a20 2020 2020   3 samples.     
-00021840: 2020 2020 2020 206d 696e 5f64 7572 203d         min_dur =
-00021850: 2033 202a 206e 702e 6469 6666 2873 656c   3 * np.diff(sel
-00021860: 662e 6d6e 652e 696e 7374 2e74 696d 6573  f.mne.inst.times
-00021870: 5b3a 325d 295b 305d 0a20 2020 2020 2020  [:2])[0].       
-00021880: 2020 2020 2072 656c 5f73 7465 7020 3d20       rel_step = 
-00021890: 7365 6c66 2e6d 6e65 2e64 7572 6174 696f  self.mne.duratio
-000218a0: 6e20 2a20 7374 6570 0a0a 2020 2020 2020  n * step..      
-000218b0: 2020 786d 6178 202b 3d20 7265 6c5f 7374    xmax += rel_st
-000218c0: 6570 0a0a 2020 2020 2020 2020 6966 2078  ep..        if x
-000218d0: 6d61 7820 2d20 786d 696e 203c 206d 696e  max - xmin < min
-000218e0: 5f64 7572 3a0a 2020 2020 2020 2020 2020  _dur:.          
-000218f0: 2020 786d 6178 203d 2078 6d69 6e20 2b20    xmax = xmin + 
-00021900: 6d69 6e5f 6475 720a 0a20 2020 2020 2020  min_dur..       
-00021910: 2069 6620 786d 6178 203e 2073 656c 662e   if xmax > self.
-00021920: 6d6e 652e 786d 6178 3a0a 2020 2020 2020  mne.xmax:.      
-00021930: 2020 2020 2020 6469 6666 203d 2078 6d61        diff = xma
-00021940: 7820 2d20 7365 6c66 2e6d 6e65 2e78 6d61  x - self.mne.xma
-00021950: 780a 2020 2020 2020 2020 2020 2020 786d  x.            xm
-00021960: 6178 203d 2073 656c 662e 6d6e 652e 786d  ax = self.mne.xm
-00021970: 6178 0a20 2020 2020 2020 2020 2020 2078  ax.            x
-00021980: 6d69 6e20 2d3d 2064 6966 660a 0a20 2020  min -= diff..   
-00021990: 2020 2020 2069 6620 786d 696e 203c 2030       if xmin < 0
-000219a0: 3a0a 2020 2020 2020 2020 2020 2020 786d  :.            xm
-000219b0: 696e 203d 2030 0a0a 2020 2020 2020 2020  in = 0..        
-000219c0: 7365 6c66 2e6d 6e65 2e61 785f 6873 6372  self.mne.ax_hscr
-000219d0: 6f6c 6c2e 7570 6461 7465 5f64 7572 6174  oll.update_durat
-000219e0: 696f 6e28 290a 2020 2020 2020 2020 7365  ion().        se
-000219f0: 6c66 2e6d 6e65 2e70 6c74 2e73 6574 5852  lf.mne.plt.setXR
-00021a00: 616e 6765 2878 6d69 6e2c 2078 6d61 782c  ange(xmin, xmax,
-00021a10: 2070 6164 6469 6e67 3d30 290a 0a20 2020   padding=0)..   
-00021a20: 2064 6566 2063 6861 6e67 655f 6e63 6861   def change_ncha
-00021a30: 6e28 7365 6c66 2c20 6368 6563 6b65 643d  n(self, checked=
-00021a40: 4661 6c73 652c 202a 2c20 7374 6570 293a  False, *, step):
-00021a50: 0a20 2020 2020 2020 2022 2222 4368 616e  .        """Chan
-00021a60: 6765 206e 756d 6265 7220 6f66 2063 6861  ge number of cha
-00021a70: 6e6e 656c 7320 6279 2073 7465 702e 2222  nnels by step.""
-00021a80: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-00021a90: 2073 656c 662e 6d6e 652e 6275 7474 6572   self.mne.butter
-00021aa0: 666c 793a 0a20 2020 2020 2020 2020 2020  fly:.           
-00021ab0: 2069 6620 7374 6570 203d 3d20 272b 6675   if step == '+fu
-00021ac0: 6c6c 273a 0a20 2020 2020 2020 2020 2020  ll':.           
-00021ad0: 2020 2020 2073 7465 7020 3d20 7365 6c66       step = self
-00021ae0: 2e6d 6e65 2e6e 5f63 6861 6e6e 656c 730a  .mne.n_channels.
-00021af0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00021b00: 2073 7465 7020 3d3d 2027 2d66 756c 6c27   step == '-full'
-00021b10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00021b20: 2020 7374 6570 203d 202d 2073 656c 662e    step = - self.
-00021b30: 6d6e 652e 6e5f 6368 616e 6e65 6c73 0a20  mne.n_channels. 
-00021b40: 2020 2020 2020 2020 2020 2079 6d69 6e2c             ymin,
-00021b50: 2079 6d61 7820 3d20 7365 6c66 2e6d 6e65   ymax = self.mne
-00021b60: 2e76 6965 7762 6f78 2e76 6965 7752 616e  .viewbox.viewRan
-00021b70: 6765 2829 5b31 5d0a 2020 2020 2020 2020  ge()[1].        
-00021b80: 2020 2020 796d 6178 202b 3d20 7374 6570      ymax += step
-00021b90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00021ba0: 796d 6178 203e 2073 656c 662e 6d6e 652e  ymax > self.mne.
-00021bb0: 796d 6178 3a0a 2020 2020 2020 2020 2020  ymax:.          
-00021bc0: 2020 2020 2020 796d 6178 203d 2073 656c        ymax = sel
-00021bd0: 662e 6d6e 652e 796d 6178 0a20 2020 2020  f.mne.ymax.     
-00021be0: 2020 2020 2020 2020 2020 2079 6d69 6e20             ymin 
-00021bf0: 2d3d 2073 7465 700a 0a20 2020 2020 2020  -= step..       
-00021c00: 2020 2020 2069 6620 796d 696e 203c 2030       if ymin < 0
-00021c10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00021c20: 2020 796d 696e 203d 2030 0a0a 2020 2020    ymin = 0..    
-00021c30: 2020 2020 2020 2020 6966 2079 6d61 7820          if ymax 
-00021c40: 2d20 796d 696e 203c 3d20 323a 0a20 2020  - ymin <= 2:.   
-00021c50: 2020 2020 2020 2020 2020 2020 2079 6d61               yma
-00021c60: 7820 3d20 796d 696e 202b 2032 0a0a 2020  x = ymin + 2..  
-00021c70: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00021c80: 6e65 2e61 785f 7673 6372 6f6c 6c2e 7570  ne.ax_vscroll.up
-00021c90: 6461 7465 5f6e 6368 616e 2829 0a20 2020  date_nchan().   
-00021ca0: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
-00021cb0: 652e 706c 742e 7365 7459 5261 6e67 6528  e.plt.setYRange(
-00021cc0: 796d 696e 2c20 796d 6178 2c20 7061 6464  ymin, ymax, padd
-00021cd0: 696e 673d 3029 0a0a 2020 2020 6465 6620  ing=0)..    def 
-00021ce0: 5f72 656d 6f76 655f 766c 696e 6528 7365  _remove_vline(se
-00021cf0: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-00021d00: 7365 6c66 2e6d 6e65 2e76 6c69 6e65 2069  self.mne.vline i
-00021d10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00021d20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00021d30: 6d6e 652e 6973 5f65 706f 6368 733a 0a20  mne.is_epochs:. 
-00021d40: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00021d50: 6f72 2076 6c69 6e65 2069 6e20 7365 6c66  or vline in self
-00021d60: 2e6d 6e65 2e76 6c69 6e65 3a0a 2020 2020  .mne.vline:.    
-00021d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021d80: 7365 6c66 2e6d 6e65 2e70 6c74 2e72 656d  self.mne.plt.rem
-00021d90: 6f76 6549 7465 6d28 766c 696e 6529 0a20  oveItem(vline). 
-00021da0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00021db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021dc0: 2073 656c 662e 6d6e 652e 706c 742e 7265   self.mne.plt.re
-00021dd0: 6d6f 7665 4974 656d 2873 656c 662e 6d6e  moveItem(self.mn
-00021de0: 652e 766c 696e 6529 0a0a 2020 2020 2020  e.vline)..      
-00021df0: 2020 7365 6c66 2e6d 6e65 2e76 6c69 6e65    self.mne.vline
-00021e00: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00021e10: 7365 6c66 2e6d 6e65 2e76 6c69 6e65 5f76  self.mne.vline_v
-00021e20: 6973 6962 6c65 203d 2046 616c 7365 0a20  isible = False. 
-00021e30: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-00021e40: 6f76 6572 7669 6577 5f62 6172 2e75 7064  overview_bar.upd
-00021e50: 6174 655f 766c 696e 6528 290a 0a20 2020  ate_vline()..   
-00021e60: 2064 6566 205f 6765 745f 766c 696e 655f   def _get_vline_
-00021e70: 7469 6d65 7328 7365 6c66 2c20 7429 3a0a  times(self, t):.
-00021e80: 2020 2020 2020 2020 7265 6c5f 7469 6d65          rel_time
-00021e90: 203d 2074 2025 2073 656c 662e 6d6e 652e   = t % self.mne.
-00021ea0: 6570 6f63 685f 6475 720a 2020 2020 2020  epoch_dur.      
-00021eb0: 2020 6162 735f 7469 6d65 203d 2073 656c    abs_time = sel
-00021ec0: 662e 6d6e 652e 7469 6d65 735b 305d 0a20  f.mne.times[0]. 
-00021ed0: 2020 2020 2020 2074 7320 3d20 6e70 2e61         ts = np.a
-00021ee0: 7261 6e67 6528 0a20 2020 2020 2020 2020  range(.         
-00021ef0: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-00021f00: 6e5f 6570 6f63 6873 2920 2a20 7365 6c66  n_epochs) * self
-00021f10: 2e6d 6e65 2e65 706f 6368 5f64 7572 202b  .mne.epoch_dur +
-00021f20: 2061 6273 5f74 696d 6520 2b20 7265 6c5f   abs_time + rel_
-00021f30: 7469 6d65 0a0a 2020 2020 2020 2020 7265  time..        re
-00021f40: 7475 726e 2074 730a 0a20 2020 2064 6566  turn ts..    def
-00021f50: 205f 766c 696e 655f 736c 6f74 2873 656c   _vline_slot(sel
-00021f60: 662c 206f 7269 675f 766c 696e 6529 3a0a  f, orig_vline):.
-00021f70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00021f80: 6d6e 652e 6973 5f65 706f 6368 733a 0a20  mne.is_epochs:. 
-00021f90: 2020 2020 2020 2020 2020 2074 7320 3d20             ts = 
-00021fa0: 7365 6c66 2e5f 6765 745f 766c 696e 655f  self._get_vline_
-00021fb0: 7469 6d65 7328 6f72 6967 5f76 6c69 6e65  times(orig_vline
-00021fc0: 2e76 616c 7565 2829 290a 2020 2020 2020  .value()).      
-00021fd0: 2020 2020 2020 666f 7220 766c 2c20 7874        for vl, xt
-00021fe0: 2069 6e20 7a69 7028 7365 6c66 2e6d 6e65   in zip(self.mne
-00021ff0: 2e76 6c69 6e65 2c20 7473 293a 0a20 2020  .vline, ts):.   
-00022000: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00022010: 766c 2021 3d20 6f72 6967 5f76 6c69 6e65  vl != orig_vline
-00022020: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00022030: 2020 2020 2020 766c 2e73 6574 506f 7328        vl.setPos(
-00022040: 7874 290a 2020 2020 2020 2020 7365 6c66  xt).        self
-00022050: 2e6d 6e65 2e6f 7665 7276 6965 775f 6261  .mne.overview_ba
-00022060: 722e 7570 6461 7465 5f76 6c69 6e65 2829  r.update_vline()
-00022070: 0a0a 2020 2020 6465 6620 5f61 6464 5f76  ..    def _add_v
-00022080: 6c69 6e65 2873 656c 662c 2074 293a 0a20  line(self, t):. 
-00022090: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-000220a0: 6e65 2e69 735f 6570 6f63 6873 3a0a 2020  ne.is_epochs:.  
-000220b0: 2020 2020 2020 2020 2020 7473 203d 2073            ts = s
-000220c0: 656c 662e 5f67 6574 5f76 6c69 6e65 5f74  elf._get_vline_t
-000220d0: 696d 6573 2874 290a 0a20 2020 2020 2020  imes(t)..       
-000220e0: 2020 2020 2023 2041 6464 2076 6c69 6e65       # Add vline
-000220f0: 2069 6620 4e6f 6e65 0a20 2020 2020 2020   if None.       
-00022100: 2020 2020 2069 6620 7365 6c66 2e6d 6e65       if self.mne
-00022110: 2e76 6c69 6e65 2069 7320 4e6f 6e65 3a0a  .vline is None:.
-00022120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022130: 7365 6c66 2e6d 6e65 2e76 6c69 6e65 203d  self.mne.vline =
-00022140: 206c 6973 7428 290a 2020 2020 2020 2020   list().        
-00022150: 2020 2020 2020 2020 666f 7220 7874 2069          for xt i
-00022160: 6e20 7473 3a0a 2020 2020 2020 2020 2020  n ts:.          
-00022170: 2020 2020 2020 2020 2020 6570 6f5f 6964            epo_id
-00022180: 7820 3d20 6e70 2e63 6c69 7028 0a20 2020  x = np.clip(.   
-00022190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000221a0: 2020 2020 2020 2020 206e 702e 7365 6172           np.sear
-000221b0: 6368 736f 7274 6564 2873 656c 662e 6d6e  chsorted(self.mn
-000221c0: 652e 626f 756e 6461 7279 5f74 696d 6573  e.boundary_times
-000221d0: 2c20 7874 2920 2d20 312c 0a20 2020 2020  , xt) - 1,.     
-000221e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000221f0: 2020 2020 2020 2030 2c20 6c65 6e28 7365         0, len(se
-00022200: 6c66 2e6d 6e65 2e69 6e73 7429 290a 2020  lf.mne.inst)).  
+0001f100: 2020 2020 2020 2020 2020 2020 2027 496e               'In
+0001f110: 6372 6561 7365 2073 686f 776e 2063 6861  crease shown cha
+0001f120: 6e6e 656c 7320 2831 3029 275d 0a20 2020  nnels (10)'].   
+0001f130: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+0001f140: 2020 2020 2020 2020 272d 273a 207b 0a20          '-': {. 
+0001f150: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001f160: 7174 5f6b 6579 273a 2051 742e 4b65 795f  qt_key': Qt.Key_
+0001f170: 4d69 6e75 732c 0a20 2020 2020 2020 2020  Minus,.         
+0001f180: 2020 2020 2020 2027 736c 6f74 273a 205b         'slot': [
+0001f190: 7365 6c66 2e73 6361 6c65 5f61 6c6c 5d2c  self.scale_all],
+0001f1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f1b0: 2027 6b77 273a 2027 7374 6570 272c 0a20   'kw': 'step',. 
+0001f1c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001f1d0: 7061 7261 6d65 7465 7227 3a20 5b34 202f  parameter': [4 /
+0001f1e0: 2035 5d2c 0a20 2020 2020 2020 2020 2020   5],.           
+0001f1f0: 2020 2020 2027 6465 7363 7269 7074 696f       'descriptio
+0001f200: 6e27 3a20 5b27 4465 6372 6561 7365 2053  n': ['Decrease S
+0001f210: 6361 6c65 275d 0a20 2020 2020 2020 2020  cale'].         
+0001f220: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+0001f230: 2020 272b 273a 207b 0a20 2020 2020 2020    '+': {.       
+0001f240: 2020 2020 2020 2020 2027 7174 5f6b 6579           'qt_key
+0001f250: 273a 2051 742e 4b65 795f 506c 7573 2c0a  ': Qt.Key_Plus,.
+0001f260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f270: 2773 6c6f 7427 3a20 5b73 656c 662e 7363  'slot': [self.sc
+0001f280: 616c 655f 616c 6c5d 2c0a 2020 2020 2020  ale_all],.      
+0001f290: 2020 2020 2020 2020 2020 276b 7727 3a20            'kw': 
+0001f2a0: 2773 7465 7027 2c0a 2020 2020 2020 2020  'step',.        
+0001f2b0: 2020 2020 2020 2020 2770 6172 616d 6574          'paramet
+0001f2c0: 6572 273a 205b 3520 2f20 345d 2c0a 2020  er': [5 / 4],.  
+0001f2d0: 2020 2020 2020 2020 2020 2020 2020 2764                'd
+0001f2e0: 6573 6372 6970 7469 6f6e 273a 205b 2749  escription': ['I
+0001f2f0: 6e63 7265 6173 6520 5363 616c 6527 5d0a  ncrease Scale'].
+0001f300: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+0001f310: 2020 2020 2020 2020 2020 2027 3d27 3a20             '=': 
+0001f320: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+0001f330: 2020 2771 745f 6b65 7927 3a20 5174 2e4b    'qt_key': Qt.K
+0001f340: 6579 5f45 7175 616c 2c0a 2020 2020 2020  ey_Equal,.      
+0001f350: 2020 2020 2020 2020 2020 2773 6c6f 7427            'slot'
+0001f360: 3a20 5b73 656c 662e 7363 616c 655f 616c  : [self.scale_al
+0001f370: 6c5d 2c0a 2020 2020 2020 2020 2020 2020  l],.            
+0001f380: 2020 2020 276b 7727 3a20 2773 7465 7027      'kw': 'step'
+0001f390: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001f3a0: 2020 2770 6172 616d 6574 6572 273a 205b    'parameter': [
+0001f3b0: 3520 2f20 345d 2c0a 2020 2020 2020 2020  5 / 4],.        
+0001f3c0: 2020 2020 2020 2020 2764 6573 6372 6970          'descrip
+0001f3d0: 7469 6f6e 273a 205b 2749 6e63 7265 6173  tion': ['Increas
+0001f3e0: 6520 5363 616c 6527 5d0a 2020 2020 2020  e Scale'].      
+0001f3f0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+0001f400: 2020 2020 2027 6127 3a20 7b0a 2020 2020       'a': {.    
+0001f410: 2020 2020 2020 2020 2020 2020 2771 745f              'qt_
+0001f420: 6b65 7927 3a20 5174 2e4b 6579 5f41 2c0a  key': Qt.Key_A,.
+0001f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f440: 2773 6c6f 7427 3a20 5b73 656c 662e 5f74  'slot': [self._t
+0001f450: 6f67 676c 655f 616e 6e6f 7461 7469 6f6e  oggle_annotation
+0001f460: 5f66 6967 2c0a 2020 2020 2020 2020 2020  _fig,.          
+0001f470: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001f480: 656c 662e 5f74 6f67 676c 655f 616e 6e6f  elf._toggle_anno
+0001f490: 7461 7469 6f6e 735d 2c0a 2020 2020 2020  tations],.      
+0001f4a0: 2020 2020 2020 2020 2020 276d 6f64 6966            'modif
+0001f4b0: 6965 7227 3a20 5b4e 6f6e 652c 2027 5368  ier': [None, 'Sh
+0001f4c0: 6966 7427 5d2c 0a20 2020 2020 2020 2020  ift'],.         
+0001f4d0: 2020 2020 2020 2027 6465 7363 7269 7074         'descript
+0001f4e0: 696f 6e27 3a20 5b27 546f 6767 6c65 2041  ion': ['Toggle A
+0001f4f0: 6e6e 6f74 6174 696f 6e2d 546f 6f6c 272c  nnotation-Tool',
+0001f500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f520: 2027 546f 6767 6c65 2041 6e6e 6f74 6174   'Toggle Annotat
+0001f530: 696f 6e73 2076 6973 6962 6c65 275d 0a20  ions visible']. 
+0001f540: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+0001f550: 2020 2020 2020 2020 2020 2762 273a 207b            'b': {
+0001f560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f570: 2027 7174 5f6b 6579 273a 2051 742e 4b65   'qt_key': Qt.Ke
+0001f580: 795f 422c 0a20 2020 2020 2020 2020 2020  y_B,.           
+0001f590: 2020 2020 2027 736c 6f74 273a 205b 7365       'slot': [se
+0001f5a0: 6c66 2e5f 746f 6767 6c65 5f62 7574 7465  lf._toggle_butte
+0001f5b0: 7266 6c79 5d2c 0a20 2020 2020 2020 2020  rfly],.         
+0001f5c0: 2020 2020 2020 2027 6465 7363 7269 7074         'descript
+0001f5d0: 696f 6e27 3a20 5b27 546f 6767 6c65 2042  ion': ['Toggle B
+0001f5e0: 7574 7465 7266 6c79 275d 0a20 2020 2020  utterfly'].     
+0001f5f0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+0001f600: 2020 2020 2020 2764 273a 207b 0a20 2020        'd': {.   
+0001f610: 2020 2020 2020 2020 2020 2020 2027 7174               'qt
+0001f620: 5f6b 6579 273a 2051 742e 4b65 795f 442c  _key': Qt.Key_D,
+0001f630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f640: 2027 736c 6f74 273a 205b 7365 6c66 2e5f   'slot': [self._
+0001f650: 746f 6767 6c65 5f64 635d 2c0a 2020 2020  toggle_dc],.    
+0001f660: 2020 2020 2020 2020 2020 2020 2764 6573              'des
+0001f670: 6372 6970 7469 6f6e 273a 205b 2754 6f67  cription': ['Tog
+0001f680: 676c 6520 4443 2d43 6f72 7265 6374 696f  gle DC-Correctio
+0001f690: 6e27 5d0a 2020 2020 2020 2020 2020 2020  n'].            
+0001f6a0: 7d2c 0a20 2020 2020 2020 2020 2020 2027  },.            '
+0001f6b0: 6527 3a20 7b0a 2020 2020 2020 2020 2020  e': {.          
+0001f6c0: 2020 2020 2020 2771 745f 6b65 7927 3a20        'qt_key': 
+0001f6d0: 5174 2e4b 6579 5f45 2c0a 2020 2020 2020  Qt.Key_E,.      
+0001f6e0: 2020 2020 2020 2020 2020 2773 6c6f 7427            'slot'
+0001f6f0: 3a20 5b73 656c 662e 5f74 6f67 676c 655f  : [self._toggle_
+0001f700: 6576 656e 7473 5d2c 0a20 2020 2020 2020  events],.       
+0001f710: 2020 2020 2020 2020 2027 6465 7363 7269           'descri
+0001f720: 7074 696f 6e27 3a20 5b27 546f 6767 6c65  ption': ['Toggle
+0001f730: 2045 7665 6e74 7320 7669 7369 626c 6527   Events visible'
+0001f740: 5d0a 2020 2020 2020 2020 2020 2020 7d2c  ].            },
+0001f750: 0a20 2020 2020 2020 2020 2020 2027 6827  .            'h'
+0001f760: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+0001f770: 2020 2020 2771 745f 6b65 7927 3a20 5174      'qt_key': Qt
+0001f780: 2e4b 6579 5f48 2c0a 2020 2020 2020 2020  .Key_H,.        
+0001f790: 2020 2020 2020 2020 2773 6c6f 7427 3a20          'slot': 
+0001f7a0: 5b73 656c 662e 5f74 6f67 676c 655f 6570  [self._toggle_ep
+0001f7b0: 6f63 685f 6869 7374 6f67 7261 6d5d 2c0a  och_histogram],.
+0001f7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f7d0: 2764 6573 6372 6970 7469 6f6e 273a 205b  'description': [
+0001f7e0: 2754 6f67 676c 6520 4570 6f63 682d 4869  'Toggle Epoch-Hi
+0001f7f0: 7374 6f67 7261 6d27 5d0a 2020 2020 2020  stogram'].      
+0001f800: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+0001f810: 2020 2020 2027 6a27 3a20 7b0a 2020 2020       'j': {.    
+0001f820: 2020 2020 2020 2020 2020 2020 2771 745f              'qt_
+0001f830: 6b65 7927 3a20 5174 2e4b 6579 5f4a 2c0a  key': Qt.Key_J,.
+0001f840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f850: 2773 6c6f 7427 3a20 5b73 656c 662e 5f74  'slot': [self._t
+0001f860: 6f67 676c 655f 7072 6f6a 5f66 6967 2c0a  oggle_proj_fig,.
+0001f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f880: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
+0001f890: 6f67 676c 655f 616c 6c5f 7072 6f6a 735d  oggle_all_projs]
+0001f8a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001f8b0: 2020 276d 6f64 6966 6965 7227 3a20 5b4e    'modifier': [N
+0001f8c0: 6f6e 652c 2027 5368 6966 7427 5d2c 0a20  one, 'Shift'],. 
+0001f8d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001f8e0: 6465 7363 7269 7074 696f 6e27 3a20 5b27  description': ['
+0001f8f0: 546f 6767 6c65 2050 726f 6a65 6374 696f  Toggle Projectio
+0001f900: 6e20 4669 6775 7265 272c 0a20 2020 2020  n Figure',.     
+0001f910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f920: 2020 2020 2020 2020 2020 2027 546f 6767             'Togg
+0001f930: 6c65 2061 6c6c 2070 726f 6a65 6374 696f  le all projectio
+0001f940: 6e73 275d 0a20 2020 2020 2020 2020 2020  ns'].           
+0001f950: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+0001f960: 276c 273a 207b 0a20 2020 2020 2020 2020  'l': {.         
+0001f970: 2020 2020 2020 2027 7174 5f6b 6579 273a         'qt_key':
+0001f980: 2051 742e 4b65 795f 4c2c 0a20 2020 2020   Qt.Key_L,.     
+0001f990: 2020 2020 2020 2020 2020 2027 736c 6f74             'slot
+0001f9a0: 273a 205b 7365 6c66 2e5f 746f 6767 6c65  ': [self._toggle
+0001f9b0: 5f61 6e74 6961 6c69 6173 696e 675d 2c0a  _antialiasing],.
+0001f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f9d0: 2764 6573 6372 6970 7469 6f6e 273a 205b  'description': [
+0001f9e0: 2754 6f67 676c 6520 416e 7469 616c 6961  'Toggle Antialia
+0001f9f0: 7369 6e67 275d 0a20 2020 2020 2020 2020  sing'].         
+0001fa00: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+0001fa10: 2020 276f 273a 207b 0a20 2020 2020 2020    'o': {.       
+0001fa20: 2020 2020 2020 2020 2027 7174 5f6b 6579           'qt_key
+0001fa30: 273a 2051 742e 4b65 795f 4f2c 0a20 2020  ': Qt.Key_O,.   
+0001fa40: 2020 2020 2020 2020 2020 2020 2027 736c               'sl
+0001fa50: 6f74 273a 205b 7365 6c66 2e5f 746f 6767  ot': [self._togg
+0001fa60: 6c65 5f6f 7665 7276 6965 775f 6261 725d  le_overview_bar]
+0001fa70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001fa80: 2020 2764 6573 6372 6970 7469 6f6e 273a    'description':
+0001fa90: 205b 2754 6f67 676c 6520 4f76 6572 7669   ['Toggle Overvi
+0001faa0: 6577 2d42 6172 275d 0a20 2020 2020 2020  ew-Bar'].       
+0001fab0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+0001fac0: 2020 2020 2774 273a 207b 0a20 2020 2020      't': {.     
+0001fad0: 2020 2020 2020 2020 2020 2027 7174 5f6b             'qt_k
+0001fae0: 6579 273a 2051 742e 4b65 795f 542c 0a20  ey': Qt.Key_T,. 
+0001faf0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001fb00: 736c 6f74 273a 205b 7365 6c66 2e5f 746f  slot': [self._to
+0001fb10: 6767 6c65 5f74 696d 655f 666f 726d 6174  ggle_time_format
+0001fb20: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0001fb30: 2020 2027 6465 7363 7269 7074 696f 6e27     'description'
+0001fb40: 3a20 5b27 546f 6767 6c65 2054 696d 652d  : ['Toggle Time-
+0001fb50: 466f 726d 6174 275d 0a20 2020 2020 2020  Format'].       
+0001fb60: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+0001fb70: 2020 2020 2773 273a 207b 0a20 2020 2020      's': {.     
+0001fb80: 2020 2020 2020 2020 2020 2027 7174 5f6b             'qt_k
+0001fb90: 6579 273a 2051 742e 4b65 795f 532c 0a20  ey': Qt.Key_S,. 
+0001fba0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001fbb0: 736c 6f74 273a 205b 7365 6c66 2e5f 746f  slot': [self._to
+0001fbc0: 6767 6c65 5f73 6361 6c65 6261 7273 5d2c  ggle_scalebars],
+0001fbd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fbe0: 2027 6465 7363 7269 7074 696f 6e27 3a20   'description': 
+0001fbf0: 5b27 546f 6767 6c65 2053 6361 6c65 6261  ['Toggle Scaleba
+0001fc00: 7273 275d 0a20 2020 2020 2020 2020 2020  rs'].           
+0001fc10: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+0001fc20: 2777 273a 207b 0a20 2020 2020 2020 2020  'w': {.         
+0001fc30: 2020 2020 2020 2027 7174 5f6b 6579 273a         'qt_key':
+0001fc40: 2051 742e 4b65 795f 572c 0a20 2020 2020   Qt.Key_W,.     
+0001fc50: 2020 2020 2020 2020 2020 2027 736c 6f74             'slot
+0001fc60: 273a 205b 7365 6c66 2e5f 746f 6767 6c65  ': [self._toggle
+0001fc70: 5f77 6869 7465 6e69 6e67 5d2c 0a20 2020  _whitening],.   
+0001fc80: 2020 2020 2020 2020 2020 2020 2027 6465               'de
+0001fc90: 7363 7269 7074 696f 6e27 3a20 5b27 546f  scription': ['To
+0001fca0: 6767 6c65 2057 6869 7465 6e69 6e67 275d  ggle Whitening']
+0001fcb0: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+0001fcc0: 2020 2020 2020 2020 2020 2020 2778 273a              'x':
+0001fcd0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+0001fce0: 2020 2027 7174 5f6b 6579 273a 2051 742e     'qt_key': Qt.
+0001fcf0: 4b65 795f 582c 0a20 2020 2020 2020 2020  Key_X,.         
+0001fd00: 2020 2020 2020 2027 736c 6f74 273a 205b         'slot': [
+0001fd10: 7365 6c66 2e5f 746f 6767 6c65 5f63 726f  self._toggle_cro
+0001fd20: 7373 6861 6972 5d2c 0a20 2020 2020 2020  sshair],.       
+0001fd30: 2020 2020 2020 2020 2027 6465 7363 7269           'descri
+0001fd40: 7074 696f 6e27 3a20 5b27 546f 6767 6c65  ption': ['Toggle
+0001fd50: 2043 726f 7373 6861 6972 275d 0a20 2020   Crosshair'].   
+0001fd60: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+0001fd70: 2020 2020 2020 2020 277a 273a 207b 0a20          'z': {. 
+0001fd80: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001fd90: 7174 5f6b 6579 273a 2051 742e 4b65 795f  qt_key': Qt.Key_
+0001fda0: 5a2c 0a20 2020 2020 2020 2020 2020 2020  Z,.             
+0001fdb0: 2020 2027 736c 6f74 273a 205b 7365 6c66     'slot': [self
+0001fdc0: 2e5f 746f 6767 6c65 5f7a 656e 6d6f 6465  ._toggle_zenmode
+0001fdd0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0001fde0: 2020 2027 6465 7363 7269 7074 696f 6e27     'description'
+0001fdf0: 3a20 5b27 546f 6767 6c65 205a 656e 2d4d  : ['Toggle Zen-M
+0001fe00: 6f64 6527 5d0a 2020 2020 2020 2020 2020  ode'].          
+0001fe10: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+0001fe20: 2027 3f27 3a20 7b0a 2020 2020 2020 2020   '?': {.        
+0001fe30: 2020 2020 2020 2020 2771 745f 6b65 7927          'qt_key'
+0001fe40: 3a20 5174 2e4b 6579 5f51 7565 7374 696f  : Qt.Key_Questio
+0001fe50: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+0001fe60: 2020 2027 736c 6f74 273a 205b 7365 6c66     'slot': [self
+0001fe70: 2e5f 746f 6767 6c65 5f68 656c 705f 6669  ._toggle_help_fi
+0001fe80: 675d 2c0a 2020 2020 2020 2020 2020 2020  g],.            
+0001fe90: 2020 2020 2764 6573 6372 6970 7469 6f6e      'description
+0001fea0: 273a 205b 2753 686f 7720 4865 6c70 275d  ': ['Show Help']
+0001feb0: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+0001fec0: 2020 2020 2020 2020 2020 2020 2766 3131              'f11
+0001fed0: 273a 207b 0a20 2020 2020 2020 2020 2020  ': {.           
+0001fee0: 2020 2020 2027 7174 5f6b 6579 273a 2051       'qt_key': Q
+0001fef0: 742e 4b65 795f 4631 312c 0a20 2020 2020  t.Key_F11,.     
+0001ff00: 2020 2020 2020 2020 2020 2027 736c 6f74             'slot
+0001ff10: 273a 205b 7365 6c66 2e5f 746f 6767 6c65  ': [self._toggle
+0001ff20: 5f66 756c 6c73 6372 6565 6e5d 2c0a 2020  _fullscreen],.  
+0001ff30: 2020 2020 2020 2020 2020 2020 2020 2764                'd
+0001ff40: 6573 6372 6970 7469 6f6e 273a 205b 2754  escription': ['T
+0001ff50: 6f67 676c 6520 4675 6c6c 2d53 6372 6565  oggle Full-Scree
+0001ff60: 6e27 5d0a 2020 2020 2020 2020 2020 2020  n'].            
+0001ff70: 7d2c 0a20 2020 2020 2020 2020 2020 2027  },.            '
+0001ff80: 6573 6361 7065 273a 207b 0a20 2020 2020  escape': {.     
+0001ff90: 2020 2020 2020 2020 2020 2027 7174 5f6b             'qt_k
+0001ffa0: 6579 273a 2051 742e 4b65 795f 4573 6361  ey': Qt.Key_Esca
+0001ffb0: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
+0001ffc0: 2020 2020 2773 6c6f 7427 3a20 5b73 656c      'slot': [sel
+0001ffd0: 662e 5f63 6865 636b 5f63 6c6f 7365 5d2c  f._check_close],
+0001ffe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fff0: 2027 6465 7363 7269 7074 696f 6e27 3a20   'description': 
+00020000: 5b27 436c 6f73 6527 5d0a 2020 2020 2020  ['Close'].      
+00020010: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00020020: 2020 2020 2023 204a 7573 7420 666f 7220       # Just for 
+00020030: 7465 7374 696e 670a 2020 2020 2020 2020  testing.        
+00020040: 2020 2020 2765 6e74 6572 273a 207b 0a20      'enter': {. 
+00020050: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00020060: 7174 5f6b 6579 273a 2051 742e 4b65 795f  qt_key': Qt.Key_
+00020070: 456e 7465 720a 2020 2020 2020 2020 2020  Enter.          
+00020080: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00020090: 2027 2027 3a20 7b0a 2020 2020 2020 2020   ' ': {.        
+000200a0: 2020 2020 2020 2020 2771 745f 6b65 7927          'qt_key'
+000200b0: 3a20 5174 2e4b 6579 5f53 7061 6365 0a20  : Qt.Key_Space. 
+000200c0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+000200d0: 2020 2020 207d 0a20 2020 2020 2020 2069       }.        i
+000200e0: 6620 7365 6c66 2e6d 6e65 2e69 735f 6570  f self.mne.is_ep
+000200f0: 6f63 6873 3a0a 2020 2020 2020 2020 2020  ochs:.          
+00020100: 2020 2320 4469 7361 626c 6520 7469 6d65    # Disable time
+00020110: 2066 6f72 6d61 7420 746f 6767 6c69 6e67   format toggling
+00020120: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
+00020130: 2073 656c 662e 6d6e 652e 6b65 7962 6f61   self.mne.keyboa
+00020140: 7264 5f73 686f 7274 6375 7473 5b27 7427  rd_shortcuts['t'
+00020150: 5d0a 0a20 2020 2064 6566 205f 6869 6470  ]..    def _hidp
+00020160: 695f 6d6b 5065 6e28 7365 6c66 2c20 2a61  i_mkPen(self, *a
+00020170: 7267 732c 202a 2a6b 7761 7267 7329 3a0a  rgs, **kwargs):.
+00020180: 2020 2020 2020 2020 6b77 6172 6773 5b27          kwargs['
+00020190: 7769 6474 6827 5d20 3d20 7365 6c66 2e5f  width'] = self._
+000201a0: 7069 7865 6c5f 7261 7469 6f20 2a20 6b77  pixel_ratio * kw
+000201b0: 6172 6773 2e67 6574 2827 7769 6474 6827  args.get('width'
+000201c0: 2c20 312e 290a 2020 2020 2020 2020 7265  , 1.).        re
+000201d0: 7475 726e 206d 6b50 656e 282a 6172 6773  turn mkPen(*args
+000201e0: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
+000201f0: 2064 6566 205f 7570 6461 7465 5f79 6178   def _update_yax
+00020200: 6973 5f6c 6162 656c 7328 7365 6c66 293a  is_labels(self):
+00020210: 0a20 2020 2020 2020 2073 656c 662e 6d6e  .        self.mn
+00020220: 652e 6368 616e 6e65 6c5f 6178 6973 2e72  e.channel_axis.r
+00020230: 6570 6169 6e74 2829 0a0a 2020 2020 6465  epaint()..    de
+00020240: 6620 5f61 6464 5f73 6361 6c65 6261 7273  f _add_scalebars
+00020250: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00020260: 2222 2241 6464 2073 6361 6c65 6261 7273  """Add scalebars
+00020270: 2066 6f72 2061 6c6c 2063 6861 6e6e 656c   for all channel
+00020280: 2d74 7970 6573 2e0a 0a20 2020 2020 2020  -types...       
+00020290: 2028 7363 656e 6520 6861 6e64 6c65 7320   (scene handles 
+000202a0: 7368 6f77 696e 6720 7468 656d 2069 6e20  showing them in 
+000202b0: 7768 656e 2069 6e20 7669 6577 0a20 2020  when in view.   
+000202c0: 2020 2020 2072 616e 6765 290a 2020 2020       range).    
+000202d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000202e0: 7365 6c66 2e6d 6e65 2e73 6361 6c65 6261  self.mne.scaleba
+000202f0: 7273 2e63 6c65 6172 2829 0a20 2020 2020  rs.clear().     
+00020300: 2020 2023 2054 6f20 6b65 6570 206f 7264     # To keep ord
+00020310: 6572 2028 6e70 2e75 6e69 7175 6520 736f  er (np.unique so
+00020320: 7274 7329 0a20 2020 2020 2020 206f 7264  rts).        ord
+00020330: 6572 6564 5f74 7970 6573 203d 2073 656c  ered_types = sel
+00020340: 662e 6d6e 652e 6368 5f74 7970 6573 5b73  f.mne.ch_types[s
+00020350: 656c 662e 6d6e 652e 6368 5f6f 7264 6572  elf.mne.ch_order
+00020360: 5d0a 2020 2020 2020 2020 756e 6971 7565  ].        unique
+00020370: 5f74 7970 655f 6964 7873 203d 206e 702e  _type_idxs = np.
+00020380: 756e 6971 7565 286f 7264 6572 6564 5f74  unique(ordered_t
+00020390: 7970 6573 2c0a 2020 2020 2020 2020 2020  ypes,.          
+000203a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000203b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000203c0: 6e5f 696e 6465 783d 5472 7565 295b 315d  n_index=True)[1]
+000203d0: 0a20 2020 2020 2020 2063 685f 7479 7065  .        ch_type
+000203e0: 735f 6f72 6465 7265 6420 3d20 5b6f 7264  s_ordered = [ord
+000203f0: 6572 6564 5f74 7970 6573 5b69 6478 5d20  ered_types[idx] 
+00020400: 666f 7220 6964 780a 2020 2020 2020 2020  for idx.        
+00020410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020420: 2020 2020 696e 2073 6f72 7465 6428 756e      in sorted(un
+00020430: 6971 7565 5f74 7970 655f 6964 7873 295d  ique_type_idxs)]
+00020440: 0a20 2020 2020 2020 2066 6f72 2063 685f  .        for ch_
+00020450: 7479 7065 2069 6e20 5b63 7420 666f 7220  type in [ct for 
+00020460: 6374 2069 6e20 6368 5f74 7970 6573 5f6f  ct in ch_types_o
+00020470: 7264 6572 6564 0a20 2020 2020 2020 2020  rdered.         
+00020480: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00020490: 6620 6374 2021 3d20 2773 7469 6d27 2061  f ct != 'stim' a
+000204a0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+000204b0: 2020 2020 2020 2020 2020 2063 7420 696e             ct in
+000204c0: 2073 656c 662e 6d6e 652e 7363 616c 696e   self.mne.scalin
+000204d0: 6773 2061 6e64 0a20 2020 2020 2020 2020  gs and.         
+000204e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000204f0: 7420 696e 2067 6574 6174 7472 2873 656c  t in getattr(sel
+00020500: 662e 6d6e 652c 2027 756e 6974 7327 2c20  f.mne, 'units', 
+00020510: 7b7d 2920 616e 640a 2020 2020 2020 2020  {}) and.        
+00020520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020530: 6374 2069 6e20 6765 7461 7474 7228 7365  ct in getattr(se
+00020540: 6c66 2e6d 6e65 2c20 2775 6e69 745f 7363  lf.mne, 'unit_sc
+00020550: 616c 696e 6773 272c 207b 7d29 5d3a 0a20  alings', {})]:. 
+00020560: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00020570: 5f62 6172 203d 2053 6361 6c65 4261 7228  _bar = ScaleBar(
+00020580: 7365 6c66 2e6d 6e65 2c20 6368 5f74 7970  self.mne, ch_typ
+00020590: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
+000205a0: 656c 662e 6d6e 652e 7363 616c 6562 6172  elf.mne.scalebar
+000205b0: 735b 6368 5f74 7970 655d 203d 2073 6361  s[ch_type] = sca
+000205c0: 6c65 5f62 6172 0a20 2020 2020 2020 2020  le_bar.         
+000205d0: 2020 2073 656c 662e 6d6e 652e 706c 742e     self.mne.plt.
+000205e0: 6164 6449 7465 6d28 7363 616c 655f 6261  addItem(scale_ba
+000205f0: 7229 0a0a 2020 2020 2020 2020 2020 2020  r)..            
+00020600: 7363 616c 655f 6261 725f 7465 7874 203d  scale_bar_text =
+00020610: 2053 6361 6c65 4261 7254 6578 7428 7365   ScaleBarText(se
+00020620: 6c66 2e6d 6e65 2c20 6368 5f74 7970 6529  lf.mne, ch_type)
+00020630: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00020640: 662e 6d6e 652e 7363 616c 6562 6172 5f74  f.mne.scalebar_t
+00020650: 6578 7473 5b63 685f 7479 7065 5d20 3d20  exts[ch_type] = 
+00020660: 7363 616c 655f 6261 725f 7465 7874 0a20  scale_bar_text. 
+00020670: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00020680: 6d6e 652e 706c 742e 6164 6449 7465 6d28  mne.plt.addItem(
+00020690: 7363 616c 655f 6261 725f 7465 7874 290a  scale_bar_text).
+000206a0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+000206b0: 6574 5f73 6361 6c65 6261 7273 5f76 6973  et_scalebars_vis
+000206c0: 6962 6c65 2873 656c 662e 6d6e 652e 7363  ible(self.mne.sc
+000206d0: 616c 6562 6172 735f 7669 7369 626c 6529  alebars_visible)
+000206e0: 0a0a 2020 2020 6465 6620 5f75 7064 6174  ..    def _updat
+000206f0: 655f 7363 616c 6562 6172 5f78 5f70 6f73  e_scalebar_x_pos
+00020700: 6974 696f 6e73 2873 656c 6629 3a0a 2020  itions(self):.  
+00020710: 2020 2020 2020 6966 2073 656c 662e 6d6e        if self.mn
+00020720: 652e 7363 616c 6562 6172 735f 7669 7369  e.scalebars_visi
+00020730: 626c 653a 0a20 2020 2020 2020 2020 2020  ble:.           
+00020740: 2066 6f72 2073 6361 6c65 6261 7220 696e   for scalebar in
+00020750: 2073 656c 662e 6d6e 652e 7363 616c 6562   self.mne.scaleb
+00020760: 6172 732e 7661 6c75 6573 2829 3a0a 2020  ars.values():.  
+00020770: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00020780: 616c 6562 6172 2e75 7064 6174 655f 785f  alebar.update_x_
+00020790: 706f 7369 7469 6f6e 2829 0a0a 2020 2020  position()..    
+000207a0: 2020 2020 2020 2020 666f 7220 7363 616c          for scal
+000207b0: 6562 6172 5f74 6578 7420 696e 2073 656c  ebar_text in sel
+000207c0: 662e 6d6e 652e 7363 616c 6562 6172 5f74  f.mne.scalebar_t
+000207d0: 6578 7473 2e76 616c 7565 7328 293a 0a20  exts.values():. 
+000207e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000207f0: 6361 6c65 6261 725f 7465 7874 2e75 7064  calebar_text.upd
+00020800: 6174 655f 785f 706f 7369 7469 6f6e 2829  ate_x_position()
+00020810: 0a0a 2020 2020 6465 6620 5f75 7064 6174  ..    def _updat
+00020820: 655f 7363 616c 6562 6172 5f79 5f70 6f73  e_scalebar_y_pos
+00020830: 6974 696f 6e73 2873 656c 6629 3a0a 2020  itions(self):.  
+00020840: 2020 2020 2020 6966 2073 656c 662e 6d6e        if self.mn
+00020850: 652e 7363 616c 6562 6172 735f 7669 7369  e.scalebars_visi
+00020860: 626c 653a 0a20 2020 2020 2020 2020 2020  ble:.           
+00020870: 2066 6f72 2073 6361 6c65 6261 7220 696e   for scalebar in
+00020880: 2073 656c 662e 6d6e 652e 7363 616c 6562   self.mne.scaleb
+00020890: 6172 732e 7661 6c75 6573 2829 3a0a 2020  ars.values():.  
+000208a0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+000208b0: 616c 6562 6172 2e75 7064 6174 655f 795f  alebar.update_y_
+000208c0: 706f 7369 7469 6f6e 2829 0a0a 2020 2020  position()..    
+000208d0: 2020 2020 2020 2020 666f 7220 7363 616c          for scal
+000208e0: 6562 6172 5f74 6578 7420 696e 2073 656c  ebar_text in sel
+000208f0: 662e 6d6e 652e 7363 616c 6562 6172 5f74  f.mne.scalebar_t
+00020900: 6578 7473 2e76 616c 7565 7328 293a 0a20  exts.values():. 
+00020910: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00020920: 6361 6c65 6261 725f 7465 7874 2e75 7064  calebar_text.upd
+00020930: 6174 655f 795f 706f 7369 7469 6f6e 2829  ate_y_position()
+00020940: 0a0a 2020 2020 6465 6620 5f75 7064 6174  ..    def _updat
+00020950: 655f 7363 616c 6562 6172 5f76 616c 7565  e_scalebar_value
+00020960: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00020970: 2066 6f72 2073 6361 6c65 6261 725f 7465   for scalebar_te
+00020980: 7874 2069 6e20 7365 6c66 2e6d 6e65 2e73  xt in self.mne.s
+00020990: 6361 6c65 6261 725f 7465 7874 732e 7661  calebar_texts.va
+000209a0: 6c75 6573 2829 3a0a 2020 2020 2020 2020  lues():.        
+000209b0: 2020 2020 7363 616c 6562 6172 5f74 6578      scalebar_tex
+000209c0: 742e 7570 6461 7465 5f76 616c 7565 2829  t.update_value()
+000209d0: 0a0a 2020 2020 6465 6620 5f73 6574 5f73  ..    def _set_s
+000209e0: 6361 6c65 6261 7273 5f76 6973 6962 6c65  calebars_visible
+000209f0: 2873 656c 662c 2076 6973 6962 6c65 293a  (self, visible):
+00020a00: 0a20 2020 2020 2020 2066 6f72 2073 6361  .        for sca
+00020a10: 6c65 6261 7220 696e 2073 656c 662e 6d6e  lebar in self.mn
+00020a20: 652e 7363 616c 6562 6172 732e 7661 6c75  e.scalebars.valu
+00020a30: 6573 2829 3a0a 2020 2020 2020 2020 2020  es():.          
+00020a40: 2020 7363 616c 6562 6172 2e73 6574 5669    scalebar.setVi
+00020a50: 7369 626c 6528 7669 7369 626c 6529 0a0a  sible(visible)..
+00020a60: 2020 2020 2020 2020 666f 7220 7363 616c          for scal
+00020a70: 6562 6172 5f74 6578 7420 696e 2073 656c  ebar_text in sel
+00020a80: 662e 6d6e 652e 7363 616c 6562 6172 5f74  f.mne.scalebar_t
+00020a90: 6578 7473 2e76 616c 7565 7328 293a 0a20  exts.values():. 
+00020aa0: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00020ab0: 6261 725f 7465 7874 2e73 6574 5669 7369  bar_text.setVisi
+00020ac0: 626c 6528 7669 7369 626c 6529 0a0a 2020  ble(visible)..  
+00020ad0: 2020 2020 2020 7365 6c66 2e5f 7570 6461        self._upda
+00020ae0: 7465 5f73 6361 6c65 6261 725f 795f 706f  te_scalebar_y_po
+00020af0: 7369 7469 6f6e 7328 290a 0a20 2020 2064  sitions()..    d
+00020b00: 6566 205f 746f 6767 6c65 5f73 6361 6c65  ef _toggle_scale
+00020b10: 6261 7273 2873 656c 6629 3a0a 2020 2020  bars(self):.    
+00020b20: 2020 2020 7365 6c66 2e6d 6e65 2e73 6361      self.mne.sca
+00020b30: 6c65 6261 7273 5f76 6973 6962 6c65 203d  lebars_visible =
+00020b40: 206e 6f74 2073 656c 662e 6d6e 652e 7363   not self.mne.sc
+00020b50: 616c 6562 6172 735f 7669 7369 626c 650a  alebars_visible.
+00020b60: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
+00020b70: 745f 7363 616c 6562 6172 735f 7669 7369  t_scalebars_visi
+00020b80: 626c 6528 7365 6c66 2e6d 6e65 2e73 6361  ble(self.mne.sca
+00020b90: 6c65 6261 7273 5f76 6973 6962 6c65 290a  lebars_visible).
+00020ba0: 0a20 2020 2064 6566 205f 6f76 6572 7669  .    def _overvi
+00020bb0: 6577 5f6d 6f64 655f 6368 616e 6765 6428  ew_mode_changed(
+00020bc0: 7365 6c66 2c20 6e65 775f 6d6f 6465 293a  self, new_mode):
+00020bd0: 0a20 2020 2020 2020 2073 656c 662e 6d6e  .        self.mn
+00020be0: 652e 6f76 6572 7669 6577 5f6d 6f64 6520  e.overview_mode 
+00020bf0: 3d20 6e65 775f 6d6f 6465 0a20 2020 2020  = new_mode.     
+00020c00: 2020 2073 656c 662e 6d6e 652e 6f76 6572     self.mne.over
+00020c10: 7669 6577 5f62 6172 2e73 6574 5f62 6163  view_bar.set_bac
+00020c20: 6b67 726f 756e 6428 290a 2020 2020 2020  kground().      
+00020c30: 2020 6966 206e 6f74 2073 656c 662e 6d6e    if not self.mn
+00020c40: 652e 6f76 6572 7669 6577 5f62 6172 2e69  e.overview_bar.i
+00020c50: 7356 6973 6962 6c65 2829 3a0a 2020 2020  sVisible():.    
+00020c60: 2020 2020 2020 2020 7365 6c66 2e5f 746f          self._to
+00020c70: 6767 6c65 5f6f 7665 7276 6965 775f 6261  ggle_overview_ba
+00020c80: 7228 290a 0a20 2020 2064 6566 205f 6f76  r()..    def _ov
+00020c90: 6572 7669 6577 5f72 6164 696f 5f63 6c69  erview_radio_cli
+00020ca0: 636b 6564 2873 656c 662c 2063 6865 636b  cked(self, check
+00020cb0: 6564 2c20 2a2c 206d 656e 752c 206e 6577  ed, *, menu, new
+00020cc0: 5f6d 6f64 6529 3a0a 2020 2020 2020 2020  _mode):.        
+00020cd0: 6d65 6e75 2e63 6c6f 7365 2829 0a20 2020  menu.close().   
+00020ce0: 2020 2020 2073 656c 662e 5f6f 7665 7276       self._overv
+00020cf0: 6965 775f 6d6f 6465 5f63 6861 6e67 6564  iew_mode_changed
+00020d00: 286e 6577 5f6d 6f64 653d 6e65 775f 6d6f  (new_mode=new_mo
+00020d10: 6465 290a 0a20 2020 2064 6566 2073 6361  de)..    def sca
+00020d20: 6c65 5f61 6c6c 2873 656c 662c 2063 6865  le_all(self, che
+00020d30: 636b 6564 3d46 616c 7365 2c20 2a2c 2073  cked=False, *, s
+00020d40: 7465 7029 3a0a 2020 2020 2020 2020 2222  tep):.        ""
+00020d50: 2253 6361 6c65 2061 6c6c 2074 7261 6365  "Scale all trace
+00020d60: 7320 6279 206d 756c 7469 706c 7969 6e67  s by multiplying
+00020d70: 2077 6974 6820 7374 6570 2e22 2222 0a20   with step.""". 
+00020d80: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
+00020d90: 7363 616c 655f 6661 6374 6f72 202a 3d20  scale_factor *= 
+00020da0: 7374 6570 0a0a 2020 2020 2020 2020 2320  step..        # 
+00020db0: 5265 6170 706c 7920 636c 6970 7069 6e67  Reapply clipping
+00020dc0: 2069 6620 6e65 6365 7373 6172 790a 2020   if necessary.  
+00020dd0: 2020 2020 2020 6966 2073 656c 662e 6d6e        if self.mn
+00020de0: 652e 636c 6970 7069 6e67 2069 7320 6e6f  e.clipping is no
+00020df0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00020e00: 2020 2020 7365 6c66 2e5f 7570 6461 7465      self._update
+00020e10: 5f64 6174 6128 290a 0a20 2020 2020 2020  _data()..       
+00020e20: 2023 2053 6361 6c65 2054 7261 6365 7320   # Scale Traces 
+00020e30: 2862 7920 7363 616c 696e 6720 7468 6520  (by scaling the 
+00020e40: 4974 656d 2c20 6e6f 7420 7468 6520 6461  Item, not the da
+00020e50: 7461 290a 2020 2020 2020 2020 666f 7220  ta).        for 
+00020e60: 6c69 6e65 2069 6e20 7365 6c66 2e6d 6e65  line in self.mne
+00020e70: 2e74 7261 6365 733a 0a20 2020 2020 2020  .traces:.       
+00020e80: 2020 2020 206c 696e 652e 7570 6461 7465       line.update
+00020e90: 5f73 6361 6c65 2829 0a0a 2020 2020 2020  _scale()..      
+00020ea0: 2020 2320 5570 6461 7465 2053 6361 6c65    # Update Scale
+00020eb0: 6261 7273 0a20 2020 2020 2020 2073 656c  bars.        sel
+00020ec0: 662e 5f75 7064 6174 655f 7363 616c 6562  f._update_scaleb
+00020ed0: 6172 5f76 616c 7565 7328 290a 0a20 2020  ar_values()..   
+00020ee0: 2064 6566 2068 7363 726f 6c6c 2873 656c   def hscroll(sel
+00020ef0: 662c 2073 7465 7029 3a0a 2020 2020 2020  f, step):.      
+00020f00: 2020 2222 2253 6372 6f6c 6c20 686f 7269    """Scroll hori
+00020f10: 7a6f 6e74 616c 6c79 2062 7920 7374 6570  zontally by step
+00020f20: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
+00020f30: 6973 696e 7374 616e 6365 2873 7465 702c  isinstance(step,
+00020f40: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+00020f50: 2020 2069 6620 7374 6570 2069 6e20 2827     if step in ('
+00020f60: 2d66 756c 6c27 2c20 272b 6675 6c6c 2729  -full', '+full')
+00020f70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00020f80: 2020 7265 6c5f 7374 6570 203d 2073 656c    rel_step = sel
+00020f90: 662e 6d6e 652e 6475 7261 7469 6f6e 0a20  f.mne.duration. 
+00020fa0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00020fb0: 6620 7374 6570 203d 3d20 272d 6675 6c6c  f step == '-full
+00020fc0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+00020fd0: 2020 2020 2020 2072 656c 5f73 7465 7020         rel_step 
+00020fe0: 3d20 7265 6c5f 7374 6570 202a 202d 310a  = rel_step * -1.
+00020ff0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00021000: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00021010: 2020 6173 7365 7274 2073 7465 7020 696e    assert step in
+00021020: 2028 276c 6566 7427 2c20 2772 6967 6874   ('left', 'right
+00021030: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+00021040: 2020 2069 6620 7365 6c66 2e6d 6e65 2e69     if self.mne.i
+00021050: 735f 6570 6f63 6873 3a0a 2020 2020 2020  s_epochs:.      
+00021060: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00021070: 6c5f 7374 6570 203d 2073 656c 662e 6d6e  l_step = self.mn
+00021080: 652e 6475 7261 7469 6f6e 202f 2073 656c  e.duration / sel
+00021090: 662e 6d6e 652e 6e5f 6570 6f63 6873 0a20  f.mne.n_epochs. 
+000210a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000210b0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000210c0: 2020 2020 2020 2020 2072 656c 5f73 7465           rel_ste
+000210d0: 7020 3d20 302e 3235 202a 2073 656c 662e  p = 0.25 * self.
+000210e0: 6d6e 652e 6475 7261 7469 6f6e 0a20 2020  mne.duration.   
+000210f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00021100: 7374 6570 203d 3d20 276c 6566 7427 3a0a  step == 'left':.
+00021110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021120: 2020 2020 7265 6c5f 7374 6570 203d 2072      rel_step = r
+00021130: 656c 5f73 7465 7020 2a20 2d31 0a20 2020  el_step * -1.   
+00021140: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00021150: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00021160: 6e65 2e69 735f 6570 6f63 6873 3a0a 2020  ne.is_epochs:.  
+00021170: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00021180: 6c5f 7374 6570 203d 2028 0a20 2020 2020  l_step = (.     
+00021190: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000211a0: 702e 7369 676e 2873 7465 7029 202a 2073  p.sign(step) * s
+000211b0: 656c 662e 6d6e 652e 6475 7261 7469 6f6e  elf.mne.duration
+000211c0: 202f 2073 656c 662e 6d6e 652e 6e5f 6570   / self.mne.n_ep
+000211d0: 6f63 6873 0a20 2020 2020 2020 2020 2020  ochs.           
+000211e0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000211f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00021200: 2020 2020 2020 2020 2072 656c 5f73 7465           rel_ste
+00021210: 7020 3d20 280a 2020 2020 2020 2020 2020  p = (.          
+00021220: 2020 2020 2020 2020 2020 7374 6570 202a            step *
+00021230: 2073 656c 662e 6d6e 652e 6475 7261 7469   self.mne.durati
+00021240: 6f6e 202f 2073 656c 662e 6d6e 652e 7363  on / self.mne.sc
+00021250: 726f 6c6c 5f73 656e 7369 7469 7669 7479  roll_sensitivity
+00021260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021270: 2029 0a20 2020 2020 2020 2064 656c 2073   ).        del s
+00021280: 7465 700a 0a20 2020 2020 2020 2023 2047  tep..        # G
+00021290: 6574 2063 7572 7265 6e74 2072 616e 6765  et current range
+000212a0: 2061 6e64 2061 6464 2073 7465 7020 746f   and add step to
+000212b0: 2069 740a 2020 2020 2020 2020 786d 696e   it.        xmin
+000212c0: 2c20 786d 6178 203d 205b 6920 2b20 7265  , xmax = [i + re
+000212d0: 6c5f 7374 6570 2066 6f72 2069 2069 6e20  l_step for i in 
+000212e0: 7365 6c66 2e6d 6e65 2e76 6965 7762 6f78  self.mne.viewbox
+000212f0: 2e76 6965 7752 616e 6765 2829 5b30 5d5d  .viewRange()[0]]
+00021300: 0a0a 2020 2020 2020 2020 6966 2078 6d69  ..        if xmi
+00021310: 6e20 3c20 303a 0a20 2020 2020 2020 2020  n < 0:.         
+00021320: 2020 2078 6d69 6e20 3d20 300a 2020 2020     xmin = 0.    
+00021330: 2020 2020 2020 2020 786d 6178 203d 2078          xmax = x
+00021340: 6d69 6e20 2b20 7365 6c66 2e6d 6e65 2e64  min + self.mne.d
+00021350: 7572 6174 696f 6e0a 2020 2020 2020 2020  uration.        
+00021360: 656c 6966 2078 6d61 7820 3e20 7365 6c66  elif xmax > self
+00021370: 2e6d 6e65 2e78 6d61 783a 0a20 2020 2020  .mne.xmax:.     
+00021380: 2020 2020 2020 2078 6d61 7820 3d20 7365         xmax = se
+00021390: 6c66 2e6d 6e65 2e78 6d61 780a 2020 2020  lf.mne.xmax.    
+000213a0: 2020 2020 2020 2020 786d 696e 203d 2078          xmin = x
+000213b0: 6d61 7820 2d20 7365 6c66 2e6d 6e65 2e64  max - self.mne.d
+000213c0: 7572 6174 696f 6e0a 0a20 2020 2020 2020  uration..       
+000213d0: 2073 656c 662e 6d6e 652e 706c 742e 7365   self.mne.plt.se
+000213e0: 7458 5261 6e67 6528 786d 696e 2c20 786d  tXRange(xmin, xm
+000213f0: 6178 2c20 7061 6464 696e 673d 3029 0a0a  ax, padding=0)..
+00021400: 2020 2020 6465 6620 7673 6372 6f6c 6c28      def vscroll(
+00021410: 7365 6c66 2c20 7374 6570 293a 0a20 2020  self, step):.   
+00021420: 2020 2020 2022 2222 5363 726f 6c6c 2076       """Scroll v
+00021430: 6572 7469 6361 6c6c 7920 6279 2073 7465  ertically by ste
+00021440: 702e 2222 220a 2020 2020 2020 2020 6966  p.""".        if
+00021450: 2073 656c 662e 6d6e 652e 6669 675f 7365   self.mne.fig_se
+00021460: 6c65 6374 696f 6e20 6973 206e 6f74 204e  lection is not N
+00021470: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00021480: 2069 6620 7374 6570 203d 3d20 272b 6675   if step == '+fu
+00021490: 6c6c 273a 0a20 2020 2020 2020 2020 2020  ll':.           
+000214a0: 2020 2020 2073 7465 7020 3d20 310a 2020       step = 1.  
+000214b0: 2020 2020 2020 2020 2020 656c 6966 2073            elif s
+000214c0: 7465 7020 3d3d 2027 2d66 756c 6c27 3a0a  tep == '-full':.
+000214d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000214e0: 7374 6570 203d 202d 310a 2020 2020 2020  step = -1.      
+000214f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00021500: 2020 2020 2020 2020 2020 2020 7374 6570              step
+00021510: 203d 2069 6e74 2873 7465 7029 0a20 2020   = int(step).   
+00021520: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
+00021530: 652e 6669 675f 7365 6c65 6374 696f 6e2e  e.fig_selection.
+00021540: 5f73 6372 6f6c 6c5f 7365 6c65 6374 696f  _scroll_selectio
+00021550: 6e28 7374 6570 290a 2020 2020 2020 2020  n(step).        
+00021560: 656c 6966 2073 656c 662e 6d6e 652e 6275  elif self.mne.bu
+00021570: 7474 6572 666c 793a 0a20 2020 2020 2020  tterfly:.       
+00021580: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00021590: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000215a0: 2020 2020 2020 2320 4765 7420 6375 7272        # Get curr
+000215b0: 656e 7420 7261 6e67 6520 616e 6420 6164  ent range and ad
+000215c0: 6420 7374 6570 2074 6f20 6974 0a20 2020  d step to it.   
+000215d0: 2020 2020 2020 2020 2069 6620 7374 6570           if step
+000215e0: 203d 3d20 272b 6675 6c6c 273a 0a20 2020   == '+full':.   
+000215f0: 2020 2020 2020 2020 2020 2020 2073 7465               ste
+00021600: 7020 3d20 7365 6c66 2e6d 6e65 2e6e 5f63  p = self.mne.n_c
+00021610: 6861 6e6e 656c 730a 2020 2020 2020 2020  hannels.        
+00021620: 2020 2020 656c 6966 2073 7465 7020 3d3d      elif step ==
+00021630: 2027 2d66 756c 6c27 3a0a 2020 2020 2020   '-full':.      
+00021640: 2020 2020 2020 2020 2020 7374 6570 203d            step =
+00021650: 202d 2073 656c 662e 6d6e 652e 6e5f 6368   - self.mne.n_ch
+00021660: 616e 6e65 6c73 0a20 2020 2020 2020 2020  annels.         
+00021670: 2020 2079 6d69 6e2c 2079 6d61 7820 3d20     ymin, ymax = 
+00021680: 5b69 202b 2073 7465 7020 666f 7220 6920  [i + step for i 
+00021690: 696e 2073 656c 662e 6d6e 652e 7669 6577  in self.mne.view
+000216a0: 626f 782e 7669 6577 5261 6e67 6528 295b  box.viewRange()[
+000216b0: 315d 5d0a 0a20 2020 2020 2020 2020 2020  1]]..           
+000216c0: 2069 6620 796d 696e 203c 2030 3a0a 2020   if ymin < 0:.  
+000216d0: 2020 2020 2020 2020 2020 2020 2020 796d                ym
+000216e0: 696e 203d 2030 0a20 2020 2020 2020 2020  in = 0.         
+000216f0: 2020 2020 2020 2079 6d61 7820 3d20 7365         ymax = se
+00021700: 6c66 2e6d 6e65 2e6e 5f63 6861 6e6e 656c  lf.mne.n_channel
+00021710: 7320 2b20 310a 2020 2020 2020 2020 2020  s + 1.          
+00021720: 2020 656c 6966 2079 6d61 7820 3e20 7365    elif ymax > se
+00021730: 6c66 2e6d 6e65 2e79 6d61 783a 0a20 2020  lf.mne.ymax:.   
+00021740: 2020 2020 2020 2020 2020 2020 2079 6d61               yma
+00021750: 7820 3d20 7365 6c66 2e6d 6e65 2e79 6d61  x = self.mne.yma
+00021760: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
+00021770: 2020 796d 696e 203d 2079 6d61 7820 2d20    ymin = ymax - 
+00021780: 7365 6c66 2e6d 6e65 2e6e 5f63 6861 6e6e  self.mne.n_chann
+00021790: 656c 7320 2d20 310a 0a20 2020 2020 2020  els - 1..       
+000217a0: 2020 2020 2073 656c 662e 6d6e 652e 706c       self.mne.pl
+000217b0: 742e 7365 7459 5261 6e67 6528 796d 696e  t.setYRange(ymin
+000217c0: 2c20 796d 6178 2c20 7061 6464 696e 673d  , ymax, padding=
+000217d0: 3029 0a0a 2020 2020 6465 6620 6368 616e  0)..    def chan
+000217e0: 6765 5f64 7572 6174 696f 6e28 7365 6c66  ge_duration(self
+000217f0: 2c20 6368 6563 6b65 643d 4661 6c73 652c  , checked=False,
+00021800: 202a 2c20 7374 6570 293a 0a20 2020 2020   *, step):.     
+00021810: 2020 2022 2222 4368 616e 6765 2064 7572     """Change dur
+00021820: 6174 696f 6e20 6279 2073 7465 702e 2222  ation by step.""
+00021830: 220a 2020 2020 2020 2020 786d 696e 2c20  ".        xmin, 
+00021840: 786d 6178 203d 2073 656c 662e 6d6e 652e  xmax = self.mne.
+00021850: 7669 6577 626f 782e 7669 6577 5261 6e67  viewbox.viewRang
+00021860: 6528 295b 305d 0a0a 2020 2020 2020 2020  e()[0]..        
+00021870: 6966 2073 656c 662e 6d6e 652e 6973 5f65  if self.mne.is_e
+00021880: 706f 6368 733a 0a20 2020 2020 2020 2020  pochs:.         
+00021890: 2020 2023 2075 7365 2074 6865 206c 656e     # use the len
+000218a0: 6774 6820 6f66 206f 6e65 2065 706f 6368  gth of one epoch
+000218b0: 2061 7320 6475 7261 7469 6f6e 2063 6861   as duration cha
+000218c0: 6e67 650a 2020 2020 2020 2020 2020 2020  nge.            
+000218d0: 6d69 6e5f 6475 7220 3d20 6c65 6e28 7365  min_dur = len(se
+000218e0: 6c66 2e6d 6e65 2e69 6e73 742e 7469 6d65  lf.mne.inst.time
+000218f0: 7329 202f 2073 656c 662e 6d6e 652e 696e  s) / self.mne.in
+00021900: 666f 5b27 7366 7265 7127 5d0a 2020 2020  fo['sfreq'].    
+00021910: 2020 2020 2020 2020 7374 6570 5f64 6972          step_dir
+00021920: 203d 2028 3120 6966 2073 7465 7020 3e20   = (1 if step > 
+00021930: 3020 656c 7365 202d 3129 0a20 2020 2020  0 else -1).     
+00021940: 2020 2020 2020 2072 656c 5f73 7465 7020         rel_step 
+00021950: 3d20 6d69 6e5f 6475 7220 2a20 7374 6570  = min_dur * step
+00021960: 5f64 6972 0a20 2020 2020 2020 2020 2020  _dir.           
+00021970: 2073 656c 662e 6d6e 652e 6e5f 6570 6f63   self.mne.n_epoc
+00021980: 6873 203d 206e 702e 636c 6970 2873 656c  hs = np.clip(sel
+00021990: 662e 6d6e 652e 6e5f 6570 6f63 6873 202b  f.mne.n_epochs +
+000219a0: 2073 7465 705f 6469 722c 0a20 2020 2020   step_dir,.     
+000219b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000219c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000219d0: 2020 2031 2c20 6c65 6e28 7365 6c66 2e6d     1, len(self.m
+000219e0: 6e65 2e69 6e73 7429 290a 2020 2020 2020  ne.inst)).      
+000219f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00021a00: 2020 2020 2320 6e65 7665 7220 7368 6f77      # never show
+00021a10: 2066 6577 6572 2074 6861 6e20 3320 7361   fewer than 3 sa
+00021a20: 6d70 6c65 730a 2020 2020 2020 2020 2020  mples.          
+00021a30: 2020 6d69 6e5f 6475 7220 3d20 3320 2a20    min_dur = 3 * 
+00021a40: 6e70 2e64 6966 6628 7365 6c66 2e6d 6e65  np.diff(self.mne
+00021a50: 2e69 6e73 742e 7469 6d65 735b 3a32 5d29  .inst.times[:2])
+00021a60: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00021a70: 7265 6c5f 7374 6570 203d 2073 656c 662e  rel_step = self.
+00021a80: 6d6e 652e 6475 7261 7469 6f6e 202a 2073  mne.duration * s
+00021a90: 7465 700a 0a20 2020 2020 2020 2078 6d61  tep..        xma
+00021aa0: 7820 2b3d 2072 656c 5f73 7465 700a 0a20  x += rel_step.. 
+00021ab0: 2020 2020 2020 2069 6620 786d 6178 202d         if xmax -
+00021ac0: 2078 6d69 6e20 3c20 6d69 6e5f 6475 723a   xmin < min_dur:
+00021ad0: 0a20 2020 2020 2020 2020 2020 2078 6d61  .            xma
+00021ae0: 7820 3d20 786d 696e 202b 206d 696e 5f64  x = xmin + min_d
+00021af0: 7572 0a0a 2020 2020 2020 2020 6966 2078  ur..        if x
+00021b00: 6d61 7820 3e20 7365 6c66 2e6d 6e65 2e78  max > self.mne.x
+00021b10: 6d61 783a 0a20 2020 2020 2020 2020 2020  max:.           
+00021b20: 2064 6966 6620 3d20 786d 6178 202d 2073   diff = xmax - s
+00021b30: 656c 662e 6d6e 652e 786d 6178 0a20 2020  elf.mne.xmax.   
+00021b40: 2020 2020 2020 2020 2078 6d61 7820 3d20           xmax = 
+00021b50: 7365 6c66 2e6d 6e65 2e78 6d61 780a 2020  self.mne.xmax.  
+00021b60: 2020 2020 2020 2020 2020 786d 696e 202d            xmin -
+00021b70: 3d20 6469 6666 0a0a 2020 2020 2020 2020  = diff..        
+00021b80: 6966 2078 6d69 6e20 3c20 303a 0a20 2020  if xmin < 0:.   
+00021b90: 2020 2020 2020 2020 2078 6d69 6e20 3d20           xmin = 
+00021ba0: 300a 0a20 2020 2020 2020 2073 656c 662e  0..        self.
+00021bb0: 6d6e 652e 6178 5f68 7363 726f 6c6c 2e75  mne.ax_hscroll.u
+00021bc0: 7064 6174 655f 6475 7261 7469 6f6e 2829  pdate_duration()
+00021bd0: 0a20 2020 2020 2020 2073 656c 662e 6d6e  .        self.mn
+00021be0: 652e 706c 742e 7365 7458 5261 6e67 6528  e.plt.setXRange(
+00021bf0: 786d 696e 2c20 786d 6178 2c20 7061 6464  xmin, xmax, padd
+00021c00: 696e 673d 3029 0a0a 2020 2020 6465 6620  ing=0)..    def 
+00021c10: 6368 616e 6765 5f6e 6368 616e 2873 656c  change_nchan(sel
+00021c20: 662c 2063 6865 636b 6564 3d46 616c 7365  f, checked=False
+00021c30: 2c20 2a2c 2073 7465 7029 3a0a 2020 2020  , *, step):.    
+00021c40: 2020 2020 2222 2243 6861 6e67 6520 6e75      """Change nu
+00021c50: 6d62 6572 206f 6620 6368 616e 6e65 6c73  mber of channels
+00021c60: 2062 7920 7374 6570 2e22 2222 0a20 2020   by step.""".   
+00021c70: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00021c80: 2e6d 6e65 2e62 7574 7465 7266 6c79 3a0a  .mne.butterfly:.
+00021c90: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00021ca0: 7465 7020 3d3d 2027 2b66 756c 6c27 3a0a  tep == '+full':.
+00021cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021cc0: 7374 6570 203d 2073 656c 662e 6d6e 652e  step = self.mne.
+00021cd0: 6e5f 6368 616e 6e65 6c73 0a20 2020 2020  n_channels.     
+00021ce0: 2020 2020 2020 2065 6c69 6620 7374 6570         elif step
+00021cf0: 203d 3d20 272d 6675 6c6c 273a 0a20 2020   == '-full':.   
+00021d00: 2020 2020 2020 2020 2020 2020 2073 7465               ste
+00021d10: 7020 3d20 2d20 7365 6c66 2e6d 6e65 2e6e  p = - self.mne.n
+00021d20: 5f63 6861 6e6e 656c 730a 2020 2020 2020  _channels.      
+00021d30: 2020 2020 2020 796d 696e 2c20 796d 6178        ymin, ymax
+00021d40: 203d 2073 656c 662e 6d6e 652e 7669 6577   = self.mne.view
+00021d50: 626f 782e 7669 6577 5261 6e67 6528 295b  box.viewRange()[
+00021d60: 315d 0a20 2020 2020 2020 2020 2020 2079  1].            y
+00021d70: 6d61 7820 2b3d 2073 7465 700a 2020 2020  max += step.    
+00021d80: 2020 2020 2020 2020 6966 2079 6d61 7820          if ymax 
+00021d90: 3e20 7365 6c66 2e6d 6e65 2e79 6d61 783a  > self.mne.ymax:
+00021da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021db0: 2079 6d61 7820 3d20 7365 6c66 2e6d 6e65   ymax = self.mne
+00021dc0: 2e79 6d61 780a 2020 2020 2020 2020 2020  .ymax.          
+00021dd0: 2020 2020 2020 796d 696e 202d 3d20 7374        ymin -= st
+00021de0: 6570 0a0a 2020 2020 2020 2020 2020 2020  ep..            
+00021df0: 6966 2079 6d69 6e20 3c20 303a 0a20 2020  if ymin < 0:.   
+00021e00: 2020 2020 2020 2020 2020 2020 2079 6d69               ymi
+00021e10: 6e20 3d20 300a 0a20 2020 2020 2020 2020  n = 0..         
+00021e20: 2020 2069 6620 796d 6178 202d 2079 6d69     if ymax - ymi
+00021e30: 6e20 3c3d 2032 3a0a 2020 2020 2020 2020  n <= 2:.        
+00021e40: 2020 2020 2020 2020 796d 6178 203d 2079          ymax = y
+00021e50: 6d69 6e20 2b20 320a 0a20 2020 2020 2020  min + 2..       
+00021e60: 2020 2020 2073 656c 662e 6d6e 652e 6178       self.mne.ax
+00021e70: 5f76 7363 726f 6c6c 2e75 7064 6174 655f  _vscroll.update_
+00021e80: 6e63 6861 6e28 290a 2020 2020 2020 2020  nchan().        
+00021e90: 2020 2020 7365 6c66 2e6d 6e65 2e70 6c74      self.mne.plt
+00021ea0: 2e73 6574 5952 616e 6765 2879 6d69 6e2c  .setYRange(ymin,
+00021eb0: 2079 6d61 782c 2070 6164 6469 6e67 3d30   ymax, padding=0
+00021ec0: 290a 0a20 2020 2064 6566 205f 7265 6d6f  )..    def _remo
+00021ed0: 7665 5f76 6c69 6e65 2873 656c 6629 3a0a  ve_vline(self):.
+00021ee0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00021ef0: 6d6e 652e 766c 696e 6520 6973 206e 6f74  mne.vline is not
+00021f00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00021f10: 2020 2069 6620 7365 6c66 2e6d 6e65 2e69     if self.mne.i
+00021f20: 735f 6570 6f63 6873 3a0a 2020 2020 2020  s_epochs:.      
+00021f30: 2020 2020 2020 2020 2020 666f 7220 766c            for vl
+00021f40: 696e 6520 696e 2073 656c 662e 6d6e 652e  ine in self.mne.
+00021f50: 766c 696e 653a 0a20 2020 2020 2020 2020  vline:.         
+00021f60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00021f70: 6d6e 652e 706c 742e 7265 6d6f 7665 4974  mne.plt.removeIt
+00021f80: 656d 2876 6c69 6e65 290a 2020 2020 2020  em(vline).      
+00021f90: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00021fa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00021fb0: 2e6d 6e65 2e70 6c74 2e72 656d 6f76 6549  .mne.plt.removeI
+00021fc0: 7465 6d28 7365 6c66 2e6d 6e65 2e76 6c69  tem(self.mne.vli
+00021fd0: 6e65 290a 0a20 2020 2020 2020 2073 656c  ne)..        sel
+00021fe0: 662e 6d6e 652e 766c 696e 6520 3d20 4e6f  f.mne.vline = No
+00021ff0: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+00022000: 6d6e 652e 766c 696e 655f 7669 7369 626c  mne.vline_visibl
+00022010: 6520 3d20 4661 6c73 650a 2020 2020 2020  e = False.      
+00022020: 2020 7365 6c66 2e6d 6e65 2e6f 7665 7276    self.mne.overv
+00022030: 6965 775f 6261 722e 7570 6461 7465 5f76  iew_bar.update_v
+00022040: 6c69 6e65 2829 0a0a 2020 2020 6465 6620  line()..    def 
+00022050: 5f67 6574 5f76 6c69 6e65 5f74 696d 6573  _get_vline_times
+00022060: 2873 656c 662c 2074 293a 0a20 2020 2020  (self, t):.     
+00022070: 2020 2072 656c 5f74 696d 6520 3d20 7420     rel_time = t 
+00022080: 2520 7365 6c66 2e6d 6e65 2e65 706f 6368  % self.mne.epoch
+00022090: 5f64 7572 0a20 2020 2020 2020 2061 6273  _dur.        abs
+000220a0: 5f74 696d 6520 3d20 7365 6c66 2e6d 6e65  _time = self.mne
+000220b0: 2e74 696d 6573 5b30 5d0a 2020 2020 2020  .times[0].      
+000220c0: 2020 7473 203d 206e 702e 6172 616e 6765    ts = np.arange
+000220d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000220e0: 2020 7365 6c66 2e6d 6e65 2e6e 5f65 706f    self.mne.n_epo
+000220f0: 6368 7329 202a 2073 656c 662e 6d6e 652e  chs) * self.mne.
+00022100: 6570 6f63 685f 6475 7220 2b20 6162 735f  epoch_dur + abs_
+00022110: 7469 6d65 202b 2072 656c 5f74 696d 650a  time + rel_time.
+00022120: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00022130: 7473 0a0a 2020 2020 6465 6620 5f76 6c69  ts..    def _vli
+00022140: 6e65 5f73 6c6f 7428 7365 6c66 2c20 6f72  ne_slot(self, or
+00022150: 6967 5f76 6c69 6e65 293a 0a20 2020 2020  ig_vline):.     
+00022160: 2020 2069 6620 7365 6c66 2e6d 6e65 2e69     if self.mne.i
+00022170: 735f 6570 6f63 6873 3a0a 2020 2020 2020  s_epochs:.      
+00022180: 2020 2020 2020 7473 203d 2073 656c 662e        ts = self.
+00022190: 5f67 6574 5f76 6c69 6e65 5f74 696d 6573  _get_vline_times
+000221a0: 286f 7269 675f 766c 696e 652e 7661 6c75  (orig_vline.valu
+000221b0: 6528 2929 0a20 2020 2020 2020 2020 2020  e()).           
+000221c0: 2066 6f72 2076 6c2c 2078 7420 696e 207a   for vl, xt in z
+000221d0: 6970 2873 656c 662e 6d6e 652e 766c 696e  ip(self.mne.vlin
+000221e0: 652c 2074 7329 3a0a 2020 2020 2020 2020  e, ts):.        
+000221f0: 2020 2020 2020 2020 6966 2076 6c20 213d          if vl !=
+00022200: 206f 7269 675f 766c 696e 653a 0a20 2020   orig_vline:.   
 00022210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022220: 2020 626d 696e 2c20 626d 6178 203d 2073    bmin, bmax = s
-00022230: 656c 662e 6d6e 652e 626f 756e 6461 7279  elf.mne.boundary
-00022240: 5f74 696d 6573 5b65 706f 5f69 6478 3a65  _times[epo_idx:e
-00022250: 706f 5f69 6478 202b 2032 5d0a 2020 2020  po_idx + 2].    
-00022260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022270: 2320 4176 6f69 6420 6f66 662d 6279 2d6f  # Avoid off-by-o
-00022280: 6e65 2d65 7272 6f72 2061 7420 626d 6178  ne-error at bmax
-00022290: 2066 6f72 2056 6c69 6e65 4c61 6265 6c0a   for VlineLabel.
-000222a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000222b0: 2020 2020 626d 6178 202d 3d20 3120 2f20      bmax -= 1 / 
-000222c0: 7365 6c66 2e6d 6e65 2e69 6e66 6f5b 2773  self.mne.info['s
-000222d0: 6672 6571 275d 0a20 2020 2020 2020 2020  freq'].         
-000222e0: 2020 2020 2020 2020 2020 2076 6c20 3d20             vl = 
-000222f0: 564c 696e 6528 7365 6c66 2e6d 6e65 2c20  VLine(self.mne, 
-00022300: 7874 2c20 626f 756e 6473 3d28 626d 696e  xt, bounds=(bmin
-00022310: 2c20 626d 6178 2929 0a20 2020 2020 2020  , bmax)).       
-00022320: 2020 2020 2020 2020 2020 2020 2023 2053               # S
-00022330: 686f 756c 6420 6f6e 6c79 2062 6520 656d  hould only be em
-00022340: 6974 7465 6420 7768 656e 2064 7261 6767  itted when dragg
-00022350: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
-00022360: 2020 2020 2020 2076 6c2e 7369 6750 6f73         vl.sigPos
-00022370: 6974 696f 6e43 6861 6e67 6546 696e 6973  itionChangeFinis
-00022380: 6865 642e 636f 6e6e 6563 7428 7365 6c66  hed.connect(self
-00022390: 2e5f 766c 696e 655f 736c 6f74 290a 2020  ._vline_slot).  
-000223a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000223b0: 2020 7365 6c66 2e6d 6e65 2e76 6c69 6e65    self.mne.vline
-000223c0: 2e61 7070 656e 6428 766c 290a 2020 2020  .append(vl).    
+00022220: 2076 6c2e 7365 7450 6f73 2878 7429 0a20   vl.setPos(xt). 
+00022230: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
+00022240: 6f76 6572 7669 6577 5f62 6172 2e75 7064  overview_bar.upd
+00022250: 6174 655f 766c 696e 6528 290a 0a20 2020  ate_vline()..   
+00022260: 2064 6566 205f 6164 645f 766c 696e 6528   def _add_vline(
+00022270: 7365 6c66 2c20 7429 3a0a 2020 2020 2020  self, t):.      
+00022280: 2020 6966 2073 656c 662e 6d6e 652e 6973    if self.mne.is
+00022290: 5f65 706f 6368 733a 0a20 2020 2020 2020  _epochs:.       
+000222a0: 2020 2020 2074 7320 3d20 7365 6c66 2e5f       ts = self._
+000222b0: 6765 745f 766c 696e 655f 7469 6d65 7328  get_vline_times(
+000222c0: 7429 0a0a 2020 2020 2020 2020 2020 2020  t)..            
+000222d0: 2320 4164 6420 766c 696e 6520 6966 204e  # Add vline if N
+000222e0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000222f0: 6966 2073 656c 662e 6d6e 652e 766c 696e  if self.mne.vlin
+00022300: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+00022310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00022320: 6d6e 652e 766c 696e 6520 3d20 6c69 7374  mne.vline = list
+00022330: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00022340: 2020 2066 6f72 2078 7420 696e 2074 733a     for xt in ts:
+00022350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022360: 2020 2020 2065 706f 5f69 6478 203d 206e       epo_idx = n
+00022370: 702e 636c 6970 280a 2020 2020 2020 2020  p.clip(.        
+00022380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022390: 2020 2020 6e70 2e73 6561 7263 6873 6f72      np.searchsor
+000223a0: 7465 6428 7365 6c66 2e6d 6e65 2e62 6f75  ted(self.mne.bou
+000223b0: 6e64 6172 795f 7469 6d65 732c 2078 7429  ndary_times, xt)
+000223c0: 202d 2031 2c0a 2020 2020 2020 2020 2020   - 1,.          
 000223d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000223e0: 7365 6c66 2e6d 6e65 2e70 6c74 2e61 6464  self.mne.plt.add
-000223f0: 4974 656d 2876 6c29 0a20 2020 2020 2020  Item(vl).       
-00022400: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00022410: 2020 2020 2020 2020 2020 2066 6f72 2076             for v
-00022420: 6c2c 2078 7420 696e 207a 6970 2873 656c  l, xt in zip(sel
-00022430: 662e 6d6e 652e 766c 696e 652c 2074 7329  f.mne.vline, ts)
-00022440: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00022450: 2020 2020 2020 766c 2e73 6574 506f 7328        vl.setPos(
-00022460: 7874 290a 2020 2020 2020 2020 656c 7365  xt).        else
-00022470: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00022480: 2073 656c 662e 6d6e 652e 766c 696e 6520   self.mne.vline 
-00022490: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-000224a0: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
-000224b0: 652e 766c 696e 6520 3d20 564c 696e 6528  e.vline = VLine(
-000224c0: 7365 6c66 2e6d 6e65 2c20 742c 2062 6f75  self.mne, t, bou
-000224d0: 6e64 733d 2830 2c20 7365 6c66 2e6d 6e65  nds=(0, self.mne
-000224e0: 2e78 6d61 7829 290a 2020 2020 2020 2020  .xmax)).        
-000224f0: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
-00022500: 2e76 6c69 6e65 2e73 6967 506f 7369 7469  .vline.sigPositi
-00022510: 6f6e 4368 616e 6765 4669 6e69 7368 6564  onChangeFinished
-00022520: 2e63 6f6e 6e65 6374 280a 2020 2020 2020  .connect(.      
-00022530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022540: 2020 7365 6c66 2e5f 766c 696e 655f 736c    self._vline_sl
-00022550: 6f74 290a 2020 2020 2020 2020 2020 2020  ot).            
-00022560: 2020 2020 7365 6c66 2e6d 6e65 2e70 6c74      self.mne.plt
-00022570: 2e61 6464 4974 656d 2873 656c 662e 6d6e  .addItem(self.mn
-00022580: 652e 766c 696e 6529 0a20 2020 2020 2020  e.vline).       
-00022590: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000225a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000225b0: 6d6e 652e 766c 696e 652e 7365 7450 6f73  mne.vline.setPos
-000225c0: 2874 290a 0a20 2020 2020 2020 2073 656c  (t)..        sel
-000225d0: 662e 6d6e 652e 766c 696e 655f 7669 7369  f.mne.vline_visi
-000225e0: 626c 6520 3d20 5472 7565 0a20 2020 2020  ble = True.     
-000225f0: 2020 2073 656c 662e 6d6e 652e 6f76 6572     self.mne.over
-00022600: 7669 6577 5f62 6172 2e75 7064 6174 655f  view_bar.update_
-00022610: 766c 696e 6528 290a 0a20 2020 2064 6566  vline()..    def
-00022620: 205f 6d6f 7573 655f 6d6f 7665 6428 7365   _mouse_moved(se
-00022630: 6c66 2c20 706f 7329 3a0a 2020 2020 2020  lf, pos):.      
-00022640: 2020 2222 2253 686f 7720 4372 6f73 7368    """Show Crossh
-00022650: 6169 7220 6966 2065 6e61 626c 6564 2061  air if enabled a
-00022660: 7420 6d6f 7573 6520 6d6f 7665 2e22 2222  t mouse move."""
-00022670: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00022680: 2e6d 6e65 2e63 726f 7373 6861 6972 5f65  .mne.crosshair_e
-00022690: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
-000226a0: 2020 2020 6966 2073 656c 662e 6d6e 652e      if self.mne.
-000226b0: 706c 742e 7363 656e 6542 6f75 6e64 696e  plt.sceneBoundin
-000226c0: 6752 6563 7428 292e 636f 6e74 6169 6e73  gRect().contains
-000226d0: 2870 6f73 293a 0a20 2020 2020 2020 2020  (pos):.         
-000226e0: 2020 2020 2020 206d 6f75 7365 506f 696e         mousePoin
-000226f0: 7420 3d20 7365 6c66 2e6d 6e65 2e76 6965  t = self.mne.vie
-00022700: 7762 6f78 2e6d 6170 5363 656e 6554 6f56  wbox.mapSceneToV
-00022710: 6965 7728 706f 7329 0a20 2020 2020 2020  iew(pos).       
-00022720: 2020 2020 2020 2020 2078 2c20 7920 3d20           x, y = 
-00022730: 6d6f 7573 6550 6f69 6e74 2e78 2829 2c20  mousePoint.x(), 
-00022740: 6d6f 7573 6550 6f69 6e74 2e79 2829 0a20  mousePoint.y(). 
-00022750: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00022760: 6620 2830 203c 3d20 7820 3c3d 2073 656c  f (0 <= x <= sel
-00022770: 662e 6d6e 652e 786d 6178 2061 6e64 0a20  f.mne.xmax and. 
-00022780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022790: 2020 2020 2020 2030 203c 3d20 7920 3c3d         0 <= y <=
-000227a0: 2073 656c 662e 6d6e 652e 796d 6178 293a   self.mne.ymax):
-000227b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000227c0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-000227d0: 2e6d 6e65 2e63 726f 7373 6861 6972 3a0a  .mne.crosshair:.
-000227e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000227f0: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
-00022800: 2e63 726f 7373 6861 6972 203d 2043 726f  .crosshair = Cro
-00022810: 7373 6861 6972 2873 656c 662e 6d6e 6529  sshair(self.mne)
-00022820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022830: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
-00022840: 652e 706c 742e 6164 6449 7465 6d28 7365  e.plt.addItem(se
-00022850: 6c66 2e6d 6e65 2e63 726f 7373 6861 6972  lf.mne.crosshair
-00022860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00022870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022880: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00022890: 676e 6f72 6542 6f75 6e64 733d 5472 7565  gnoreBounds=True
-000228a0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-000228b0: 2020 2020 2020 2023 2047 6574 2079 706f         # Get ypo
-000228c0: 7320 6672 6f6d 2074 7261 6365 0a20 2020  s from trace.   
-000228d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000228e0: 2074 7261 6365 203d 205b 7472 2066 6f72   trace = [tr for
-000228f0: 2074 7220 696e 2073 656c 662e 6d6e 652e   tr in self.mne.
-00022900: 7472 6163 6573 2069 660a 2020 2020 2020  traces if.      
-00022910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022920: 2020 2020 2020 2074 722e 7970 6f73 202d         tr.ypos -
-00022930: 2030 2e35 203c 2079 203c 2074 722e 7970   0.5 < y < tr.yp
-00022940: 6f73 202b 2030 2e35 5d0a 2020 2020 2020  os + 0.5].      
-00022950: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00022960: 206c 656e 2874 7261 6365 2920 3d3d 2031   len(trace) == 1
-00022970: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00022980: 2020 2020 2020 2020 2020 7472 6163 6520            trace 
-00022990: 3d20 7472 6163 655b 305d 0a20 2020 2020  = trace[0].     
+000223e0: 2020 302c 206c 656e 2873 656c 662e 6d6e    0, len(self.mn
+000223f0: 652e 696e 7374 2929 0a20 2020 2020 2020  e.inst)).       
+00022400: 2020 2020 2020 2020 2020 2020 2062 6d69               bmi
+00022410: 6e2c 2062 6d61 7820 3d20 7365 6c66 2e6d  n, bmax = self.m
+00022420: 6e65 2e62 6f75 6e64 6172 795f 7469 6d65  ne.boundary_time
+00022430: 735b 6570 6f5f 6964 783a 6570 6f5f 6964  s[epo_idx:epo_id
+00022440: 7820 2b20 325d 0a20 2020 2020 2020 2020  x + 2].         
+00022450: 2020 2020 2020 2020 2020 2023 2041 766f             # Avo
+00022460: 6964 206f 6666 2d62 792d 6f6e 652d 6572  id off-by-one-er
+00022470: 726f 7220 6174 2062 6d61 7820 666f 7220  ror at bmax for 
+00022480: 566c 696e 654c 6162 656c 0a20 2020 2020  VlineLabel.     
+00022490: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+000224a0: 6d61 7820 2d3d 2031 202f 2073 656c 662e  max -= 1 / self.
+000224b0: 6d6e 652e 696e 666f 5b27 7366 7265 7127  mne.info['sfreq'
+000224c0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000224d0: 2020 2020 2020 766c 203d 2056 4c69 6e65        vl = VLine
+000224e0: 2873 656c 662e 6d6e 652c 2078 742c 2062  (self.mne, xt, b
+000224f0: 6f75 6e64 733d 2862 6d69 6e2c 2062 6d61  ounds=(bmin, bma
+00022500: 7829 290a 2020 2020 2020 2020 2020 2020  x)).            
+00022510: 2020 2020 2020 2020 2320 5368 6f75 6c64          # Should
+00022520: 206f 6e6c 7920 6265 2065 6d69 7474 6564   only be emitted
+00022530: 2077 6865 6e20 6472 6167 6765 640a 2020   when dragged.  
+00022540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022550: 2020 766c 2e73 6967 506f 7369 7469 6f6e    vl.sigPosition
+00022560: 4368 616e 6765 4669 6e69 7368 6564 2e63  ChangeFinished.c
+00022570: 6f6e 6e65 6374 2873 656c 662e 5f76 6c69  onnect(self._vli
+00022580: 6e65 5f73 6c6f 7429 0a20 2020 2020 2020  ne_slot).       
+00022590: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000225a0: 662e 6d6e 652e 766c 696e 652e 6170 7065  f.mne.vline.appe
+000225b0: 6e64 2876 6c29 0a20 2020 2020 2020 2020  nd(vl).         
+000225c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000225d0: 6d6e 652e 706c 742e 6164 6449 7465 6d28  mne.plt.addItem(
+000225e0: 766c 290a 2020 2020 2020 2020 2020 2020  vl).            
+000225f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00022600: 2020 2020 2020 666f 7220 766c 2c20 7874        for vl, xt
+00022610: 2069 6e20 7a69 7028 7365 6c66 2e6d 6e65   in zip(self.mne
+00022620: 2e76 6c69 6e65 2c20 7473 293a 0a20 2020  .vline, ts):.   
+00022630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022640: 2076 6c2e 7365 7450 6f73 2878 7429 0a20   vl.setPos(xt). 
+00022650: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00022660: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00022670: 2e6d 6e65 2e76 6c69 6e65 2069 7320 4e6f  .mne.vline is No
+00022680: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00022690: 2020 2020 7365 6c66 2e6d 6e65 2e76 6c69      self.mne.vli
+000226a0: 6e65 203d 2056 4c69 6e65 2873 656c 662e  ne = VLine(self.
+000226b0: 6d6e 652c 2074 2c20 626f 756e 6473 3d28  mne, t, bounds=(
+000226c0: 302c 2073 656c 662e 6d6e 652e 786d 6178  0, self.mne.xmax
+000226d0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000226e0: 2020 2073 656c 662e 6d6e 652e 766c 696e     self.mne.vlin
+000226f0: 652e 7369 6750 6f73 6974 696f 6e43 6861  e.sigPositionCha
+00022700: 6e67 6546 696e 6973 6865 642e 636f 6e6e  ngeFinished.conn
+00022710: 6563 7428 0a20 2020 2020 2020 2020 2020  ect(.           
+00022720: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00022730: 662e 5f76 6c69 6e65 5f73 6c6f 7429 0a20  f._vline_slot). 
+00022740: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00022750: 656c 662e 6d6e 652e 706c 742e 6164 6449  elf.mne.plt.addI
+00022760: 7465 6d28 7365 6c66 2e6d 6e65 2e76 6c69  tem(self.mne.vli
+00022770: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
+00022780: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00022790: 2020 2020 2020 7365 6c66 2e6d 6e65 2e76        self.mne.v
+000227a0: 6c69 6e65 2e73 6574 506f 7328 7429 0a0a  line.setPos(t)..
+000227b0: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
+000227c0: 2e76 6c69 6e65 5f76 6973 6962 6c65 203d  .vline_visible =
+000227d0: 2054 7275 650a 2020 2020 2020 2020 7365   True.        se
+000227e0: 6c66 2e6d 6e65 2e6f 7665 7276 6965 775f  lf.mne.overview_
+000227f0: 6261 722e 7570 6461 7465 5f76 6c69 6e65  bar.update_vline
+00022800: 2829 0a0a 2020 2020 6465 6620 5f6d 6f75  ()..    def _mou
+00022810: 7365 5f6d 6f76 6564 2873 656c 662c 2070  se_moved(self, p
+00022820: 6f73 293a 0a20 2020 2020 2020 2022 2222  os):.        """
+00022830: 5368 6f77 2043 726f 7373 6861 6972 2069  Show Crosshair i
+00022840: 6620 656e 6162 6c65 6420 6174 206d 6f75  f enabled at mou
+00022850: 7365 206d 6f76 652e 2222 220a 2020 2020  se move.""".    
+00022860: 2020 2020 6966 2073 656c 662e 6d6e 652e      if self.mne.
+00022870: 6372 6f73 7368 6169 725f 656e 6162 6c65  crosshair_enable
+00022880: 643a 0a20 2020 2020 2020 2020 2020 2069  d:.            i
+00022890: 6620 7365 6c66 2e6d 6e65 2e70 6c74 2e73  f self.mne.plt.s
+000228a0: 6365 6e65 426f 756e 6469 6e67 5265 6374  ceneBoundingRect
+000228b0: 2829 2e63 6f6e 7461 696e 7328 706f 7329  ().contains(pos)
+000228c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000228d0: 2020 6d6f 7573 6550 6f69 6e74 203d 2073    mousePoint = s
+000228e0: 656c 662e 6d6e 652e 7669 6577 626f 782e  elf.mne.viewbox.
+000228f0: 6d61 7053 6365 6e65 546f 5669 6577 2870  mapSceneToView(p
+00022900: 6f73 290a 2020 2020 2020 2020 2020 2020  os).            
+00022910: 2020 2020 782c 2079 203d 206d 6f75 7365      x, y = mouse
+00022920: 506f 696e 742e 7828 292c 206d 6f75 7365  Point.x(), mouse
+00022930: 506f 696e 742e 7928 290a 2020 2020 2020  Point.y().      
+00022940: 2020 2020 2020 2020 2020 6966 2028 3020            if (0 
+00022950: 3c3d 2078 203c 3d20 7365 6c66 2e6d 6e65  <= x <= self.mne
+00022960: 2e78 6d61 7820 616e 640a 2020 2020 2020  .xmax and.      
+00022970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022980: 2020 3020 3c3d 2079 203c 3d20 7365 6c66    0 <= y <= self
+00022990: 2e6d 6e65 2e79 6d61 7829 3a0a 2020 2020  .mne.ymax):.    
 000229a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000229b0: 2020 2069 6478 203d 206e 702e 7365 6172     idx = np.sear
-000229c0: 6368 736f 7274 6564 2873 656c 662e 6d6e  chsorted(self.mn
-000229d0: 652e 7469 6d65 732c 2078 290a 2020 2020  e.times, x).    
-000229e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000229f0: 2020 2020 6966 2073 656c 662e 6d6e 652e      if self.mne.
-00022a00: 6461 7461 5f70 7265 636f 6d70 7574 6564  data_precomputed
-00022a10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00022a20: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00022a30: 7461 203d 2073 656c 662e 6d6e 652e 6461  ta = self.mne.da
-00022a40: 7461 5b74 7261 6365 2e6f 7264 6572 5f69  ta[trace.order_i
-00022a50: 6478 5d0a 2020 2020 2020 2020 2020 2020  dx].            
-00022a60: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00022a70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00022a80: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00022a90: 7461 203d 2073 656c 662e 6d6e 652e 6461  ta = self.mne.da
-00022aa0: 7461 5b74 7261 6365 2e72 616e 6765 5f69  ta[trace.range_i
-00022ab0: 6478 5d0a 2020 2020 2020 2020 2020 2020  dx].            
-00022ac0: 2020 2020 2020 2020 2020 2020 7976 616c              yval
-00022ad0: 7565 203d 2064 6174 615b 6964 785d 0a20  ue = data[idx]. 
-00022ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022af0: 2020 2020 2020 2079 7368 6f77 6e20 3d20         yshown = 
-00022b00: 7976 616c 7565 202b 2074 7261 6365 2e79  yvalue + trace.y
-00022b10: 706f 730a 2020 2020 2020 2020 2020 2020  pos.            
-00022b20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00022b30: 2e6d 6e65 2e63 726f 7373 6861 6972 2e73  .mne.crosshair.s
-00022b40: 6574 5f64 6174 6128 782c 2079 7368 6f77  et_data(x, yshow
-00022b50: 6e29 0a0a 2020 2020 2020 2020 2020 2020  n)..            
-00022b60: 2020 2020 2020 2020 2020 2020 2320 7265              # re
-00022b70: 6c61 7469 7665 2078 2066 6f72 2065 706f  lative x for epo
-00022b80: 6368 730a 2020 2020 2020 2020 2020 2020  chs.            
-00022b90: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00022ba0: 656c 662e 6d6e 652e 6973 5f65 706f 6368  elf.mne.is_epoch
-00022bb0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00022bc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00022bd0: 656c 5f69 6478 203d 2069 6478 2025 206c  el_idx = idx % l
-00022be0: 656e 2873 656c 662e 6d6e 652e 696e 7374  en(self.mne.inst
-00022bf0: 2e74 696d 6573 290a 2020 2020 2020 2020  .times).        
+000229b0: 6966 206e 6f74 2073 656c 662e 6d6e 652e  if not self.mne.
+000229c0: 6372 6f73 7368 6169 723a 0a20 2020 2020  crosshair:.     
+000229d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000229e0: 2020 2073 656c 662e 6d6e 652e 6372 6f73     self.mne.cros
+000229f0: 7368 6169 7220 3d20 4372 6f73 7368 6169  shair = Crosshai
+00022a00: 7228 7365 6c66 2e6d 6e65 290a 2020 2020  r(self.mne).    
+00022a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a20: 2020 2020 7365 6c66 2e6d 6e65 2e70 6c74      self.mne.plt
+00022a30: 2e61 6464 4974 656d 2873 656c 662e 6d6e  .addItem(self.mn
+00022a40: 652e 6372 6f73 7368 6169 722c 0a20 2020  e.crosshair,.   
+00022a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a70: 2020 2020 2020 2020 2020 6967 6e6f 7265            ignore
+00022a80: 426f 756e 6473 3d54 7275 6529 0a0a 2020  Bounds=True)..  
+00022a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022aa0: 2020 2320 4765 7420 7970 6f73 2066 726f    # Get ypos fro
+00022ab0: 6d20 7472 6163 650a 2020 2020 2020 2020  m trace.        
+00022ac0: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+00022ad0: 6520 3d20 5b74 7220 666f 7220 7472 2069  e = [tr for tr i
+00022ae0: 6e20 7365 6c66 2e6d 6e65 2e74 7261 6365  n self.mne.trace
+00022af0: 7320 6966 0a20 2020 2020 2020 2020 2020  s if.           
+00022b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b10: 2020 7472 2e79 706f 7320 2d20 302e 3520    tr.ypos - 0.5 
+00022b20: 3c20 7920 3c20 7472 2e79 706f 7320 2b20  < y < tr.ypos + 
+00022b30: 302e 355d 0a20 2020 2020 2020 2020 2020  0.5].           
+00022b40: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00022b50: 7472 6163 6529 203d 3d20 313a 0a20 2020  trace) == 1:.   
+00022b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b70: 2020 2020 2074 7261 6365 203d 2074 7261       trace = tra
+00022b80: 6365 5b30 5d0a 2020 2020 2020 2020 2020  ce[0].          
+00022b90: 2020 2020 2020 2020 2020 2020 2020 6964                id
+00022ba0: 7820 3d20 6e70 2e73 6561 7263 6873 6f72  x = np.searchsor
+00022bb0: 7465 6428 7365 6c66 2e6d 6e65 2e74 696d  ted(self.mne.tim
+00022bc0: 6573 2c20 7829 0a20 2020 2020 2020 2020  es, x).         
+00022bd0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00022be0: 6620 7365 6c66 2e6d 6e65 2e64 6174 615f  f self.mne.data_
+00022bf0: 7072 6563 6f6d 7075 7465 643a 0a20 2020  precomputed:.   
 00022c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022c10: 2020 2020 7820 3d20 7365 6c66 2e6d 6e65      x = self.mne
-00022c20: 2e69 6e73 742e 7469 6d65 735b 7265 6c5f  .inst.times[rel_
-00022c30: 6964 785d 0a0a 2020 2020 2020 2020 2020  idx]..          
-00022c40: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00022c50: 6e65 6761 7469 7665 2062 6563 6175 7365  negative because
-00022c60: 2070 6c6f 7420 6973 2069 6e76 6572 7465   plot is inverte
-00022c70: 6420 666f 7220 590a 2020 2020 2020 2020  d for Y.        
-00022c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022c90: 7363 616c 6572 203d 202d 3120 6966 2073  scaler = -1 if s
-00022ca0: 656c 662e 6d6e 652e 6275 7474 6572 666c  elf.mne.butterfl
-00022cb0: 7920 656c 7365 202d 320a 2020 2020 2020  y else -2.      
-00022cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022cd0: 2020 696e 765f 6e6f 726d 203d 2028 7363    inv_norm = (sc
-00022ce0: 616c 6572 202a 0a20 2020 2020 2020 2020  aler *.         
-00022cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022d00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00022d10: 6d6e 652e 7363 616c 696e 6773 5b74 7261  mne.scalings[tra
-00022d20: 6365 2e63 685f 7479 7065 5d20 2a0a 2020  ce.ch_type] *.  
-00022d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022c10: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
+00022c20: 7365 6c66 2e6d 6e65 2e64 6174 615b 7472  self.mne.data[tr
+00022c30: 6163 652e 6f72 6465 725f 6964 785d 0a20  ace.order_idx]. 
+00022c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022c50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00022c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022c70: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
+00022c80: 7365 6c66 2e6d 6e65 2e64 6174 615b 7472  self.mne.data[tr
+00022c90: 6163 652e 7261 6e67 655f 6964 785d 0a20  ace.range_idx]. 
+00022ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022cb0: 2020 2020 2020 2079 7661 6c75 6520 3d20         yvalue = 
+00022cc0: 6461 7461 5b69 6478 5d0a 2020 2020 2020  data[idx].      
+00022cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022ce0: 2020 7973 686f 776e 203d 2079 7661 6c75    yshown = yvalu
+00022cf0: 6520 2b20 7472 6163 652e 7970 6f73 0a20  e + trace.ypos. 
+00022d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022d10: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
+00022d20: 6372 6f73 7368 6169 722e 7365 745f 6461  crosshair.set_da
+00022d30: 7461 2878 2c20 7973 686f 776e 290a 0a20  ta(x, yshown).. 
 00022d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022d50: 2020 7365 6c66 2e6d 6e65 2e75 6e69 745f    self.mne.unit_
-00022d60: 7363 616c 696e 6773 5b74 7261 6365 2e63  scalings[trace.c
-00022d70: 685f 7479 7065 5d20 2f0a 2020 2020 2020  h_type] /.      
-00022d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022d90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00022da0: 6c66 2e6d 6e65 2e73 6361 6c65 5f66 6163  lf.mne.scale_fac
-00022db0: 746f 7229 0a20 2020 2020 2020 2020 2020  tor).           
-00022dc0: 2020 2020 2020 2020 2020 2020 206c 6162               lab
-00022dd0: 656c 203d 2066 277b 5f73 696d 706c 6966  el = f'{_simplif
-00022de0: 795f 666c 6f61 7428 7976 616c 7565 202a  y_float(yvalue *
-00022df0: 2069 6e76 5f6e 6f72 6d29 7d20 2720 5c0a   inv_norm)} ' \.
-00022e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022e20: 6627 7b73 656c 662e 6d6e 652e 756e 6974  f'{self.mne.unit
-00022e30: 735b 7472 6163 652e 6368 5f74 7970 655d  s[trace.ch_type]
-00022e40: 7d27 0a20 2020 2020 2020 2020 2020 2020  }'.             
-00022e50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00022e60: 7374 6174 7573 4261 7228 292e 7368 6f77  statusBar().show
-00022e70: 4d65 7373 6167 6528 6627 783d 7b78 3a2e  Message(f'x={x:.
-00022e80: 3366 7d20 732c 2027 0a20 2020 2020 2020  3f} s, '.       
-00022e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022eb0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-00022ec0: 793d 7b6c 6162 656c 7d27 290a 0a20 2020  y={label}')..   
-00022ed0: 2064 6566 205f 746f 6767 6c65 5f63 726f   def _toggle_cro
-00022ee0: 7373 6861 6972 2873 656c 6629 3a0a 2020  sshair(self):.  
-00022ef0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e63        self.mne.c
-00022f00: 726f 7373 6861 6972 5f65 6e61 626c 6564  rosshair_enabled
-00022f10: 203d 206e 6f74 2073 656c 662e 6d6e 652e   = not self.mne.
-00022f20: 6372 6f73 7368 6169 725f 656e 6162 6c65  crosshair_enable
-00022f30: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00022f40: 662e 6d6e 652e 6372 6f73 7368 6169 723a  f.mne.crosshair:
-00022f50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00022f60: 662e 6d6e 652e 706c 742e 7265 6d6f 7665  f.mne.plt.remove
-00022f70: 4974 656d 2873 656c 662e 6d6e 652e 6372  Item(self.mne.cr
-00022f80: 6f73 7368 6169 7229 0a20 2020 2020 2020  osshair).       
-00022f90: 2020 2020 2073 656c 662e 6d6e 652e 6372       self.mne.cr
-00022fa0: 6f73 7368 6169 7220 3d20 4e6f 6e65 0a0a  osshair = None..
-00022fb0: 2020 2020 6465 6620 5f78 7261 6e67 655f      def _xrange_
-00022fc0: 6368 616e 6765 6428 7365 6c66 2c20 5f2c  changed(self, _,
-00022fd0: 2078 7261 6e67 6529 3a0a 2020 2020 2020   xrange):.      
-00022fe0: 2020 2320 5570 6461 7465 2064 6174 610a    # Update data.
-00022ff0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00023000: 6d6e 652e 6973 5f65 706f 6368 733a 0a20  mne.is_epochs:. 
-00023010: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00023020: 6c66 2e6d 6e65 2e76 6c69 6e65 2069 7320  lf.mne.vline is 
-00023030: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00023040: 2020 2020 2020 2020 2020 7265 6c5f 766c            rel_vl
-00023050: 5f74 203d 2073 656c 662e 6d6e 652e 766c  _t = self.mne.vl
-00023060: 696e 655b 305d 2e76 616c 7565 2829 205c  ine[0].value() \
-00023070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023080: 2020 2020 2020 2020 2020 2020 2d20 7365              - se
-00023090: 6c66 2e6d 6e65 2e62 6f75 6e64 6172 795f  lf.mne.boundary_
-000230a0: 7469 6d65 735b 7365 6c66 2e6d 6e65 2e65  times[self.mne.e
-000230b0: 706f 6368 5f69 6478 5d5b 305d 0a0a 2020  poch_idx][0]..  
-000230c0: 2020 2020 2020 2020 2020 2320 4465 7065            # Depe
-000230d0: 6e64 7320 6f6e 206f 6e6c 7920 616c 6c6f  nds on only allo
-000230e0: 7769 6e67 2078 7261 6e67 6520 7368 6f77  wing xrange show
-000230f0: 696e 6720 6675 6c6c 2065 706f 6368 730a  ing full epochs.
-00023100: 2020 2020 2020 2020 2020 2020 626f 756e              boun
-00023110: 6461 7279 5f69 6478 7320 3d20 6e70 2e73  dary_idxs = np.s
-00023120: 6561 7263 6873 6f72 7465 6428 7365 6c66  earchsorted(self
-00023130: 2e6d 6e65 2e6d 6964 706f 696e 7473 2c20  .mne.midpoints, 
-00023140: 7872 616e 6765 290a 2020 2020 2020 2020  xrange).        
-00023150: 2020 2020 7365 6c66 2e6d 6e65 2e65 706f      self.mne.epo
-00023160: 6368 5f69 6478 203d 206e 702e 6172 616e  ch_idx = np.aran
-00023170: 6765 282a 626f 756e 6461 7279 5f69 6478  ge(*boundary_idx
-00023180: 7329 0a0a 2020 2020 2020 2020 2020 2020  s)..            
-00023190: 2320 5570 6461 7465 2063 6f6c 6f72 730a  # Update colors.
-000231a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000231b0: 7472 6163 6520 696e 2073 656c 662e 6d6e  trace in self.mn
-000231c0: 652e 7472 6163 6573 3a0a 2020 2020 2020  e.traces:.      
-000231d0: 2020 2020 2020 2020 2020 7472 6163 652e            trace.
-000231e0: 7570 6461 7465 5f63 6f6c 6f72 2829 0a0a  update_color()..
-000231f0: 2020 2020 2020 2020 2020 2020 2320 5570              # Up
-00023200: 6461 7465 2076 6c69 6e65 730a 2020 2020  date vlines.    
-00023210: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00023220: 6d6e 652e 766c 696e 6520 6973 206e 6f74  mne.vline is not
-00023230: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00023240: 2020 2020 2020 2066 6f72 2062 6d69 6e2c         for bmin,
-00023250: 2062 6d61 782c 2076 6c20 696e 207a 6970   bmax, vl in zip
-00023260: 2873 656c 662e 6d6e 652e 626f 756e 6461  (self.mne.bounda
-00023270: 7279 5f74 696d 6573 5b0a 2020 2020 2020  ry_times[.      
-00023280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000232a0: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
-000232b0: 2e65 706f 6368 5f69 6478 5d2c 0a20 2020  .epoch_idx],.   
-000232c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000232d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000232e0: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-000232f0: 626f 756e 6461 7279 5f74 696d 6573 5b0a  boundary_times[.
-00023300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023320: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00023330: 6c66 2e6d 6e65 2e65 706f 6368 5f69 6478  lf.mne.epoch_idx
-00023340: 202b 2031 5d2c 0a20 2020 2020 2020 2020   + 1],.         
-00023350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023370: 2073 656c 662e 6d6e 652e 766c 696e 6529   self.mne.vline)
-00023380: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00023390: 2020 2020 2020 2320 4176 6f69 6420 6f66        # Avoid of
-000233a0: 662d 6279 2d6f 6e65 2d65 7272 6f72 2061  f-by-one-error a
-000233b0: 7420 626d 6178 2066 6f72 2056 6c69 6e65  t bmax for Vline
-000233c0: 4c61 6265 6c0a 2020 2020 2020 2020 2020  Label.          
-000233d0: 2020 2020 2020 2020 2020 626d 6178 202d            bmax -
-000233e0: 3d20 3120 2f20 7365 6c66 2e6d 6e65 2e69  = 1 / self.mne.i
-000233f0: 6e66 6f5b 2773 6672 6571 275d 0a20 2020  nfo['sfreq'].   
-00023400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023410: 2076 6c2e 7365 7442 6f75 6e64 7328 2862   vl.setBounds((b
-00023420: 6d69 6e2c 2062 6d61 7829 290a 2020 2020  min, bmax)).    
-00023430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023440: 766c 2e73 6574 5661 6c75 6528 626d 696e  vl.setValue(bmin
-00023450: 202b 2072 656c 5f76 6c5f 7429 0a0a 2020   + rel_vl_t)..  
-00023460: 2020 2020 2020 7365 6c66 2e6d 6e65 2e74        self.mne.t
-00023470: 5f73 7461 7274 203d 2078 7261 6e67 655b  _start = xrange[
-00023480: 305d 0a20 2020 2020 2020 2073 656c 662e  0].        self.
-00023490: 6d6e 652e 6475 7261 7469 6f6e 203d 2078  mne.duration = x
-000234a0: 7261 6e67 655b 315d 202d 2078 7261 6e67  range[1] - xrang
-000234b0: 655b 305d 0a0a 2020 2020 2020 2020 7365  e[0]..        se
-000234c0: 6c66 2e5f 7265 6472 6177 2875 7064 6174  lf._redraw(updat
-000234d0: 655f 6461 7461 3d54 7275 6529 0a0a 2020  e_data=True)..  
-000234e0: 2020 2020 2020 2320 5570 6461 7465 2054        # Update T
-000234f0: 696d 652d 4261 720a 2020 2020 2020 2020  ime-Bar.        
-00023500: 7365 6c66 2e6d 6e65 2e61 785f 6873 6372  self.mne.ax_hscr
-00023510: 6f6c 6c2e 7570 6461 7465 5f76 616c 7565  oll.update_value
-00023520: 2878 7261 6e67 655b 305d 290a 0a20 2020  (xrange[0])..   
-00023530: 2020 2020 2023 2055 7064 6174 6520 4f76       # Update Ov
-00023540: 6572 7669 6577 2d42 6172 0a20 2020 2020  erview-Bar.     
-00023550: 2020 2073 656c 662e 6d6e 652e 6f76 6572     self.mne.over
-00023560: 7669 6577 5f62 6172 2e75 7064 6174 655f  view_bar.update_
-00023570: 7669 6577 7261 6e67 6528 290a 0a20 2020  viewrange()..   
-00023580: 2020 2020 2023 2055 7064 6174 6520 5363       # Update Sc
-00023590: 616c 6562 6172 730a 2020 2020 2020 2020  alebars.        
-000235a0: 7365 6c66 2e5f 7570 6461 7465 5f73 6361  self._update_sca
-000235b0: 6c65 6261 725f 785f 706f 7369 7469 6f6e  lebar_x_position
-000235c0: 7328 290a 0a20 2020 2020 2020 2023 2055  s()..        # U
-000235d0: 7064 6174 6520 616e 6e6f 7461 7469 6f6e  pdate annotation
-000235e0: 730a 2020 2020 2020 2020 7365 6c66 2e5f  s.        self._
-000235f0: 7570 6461 7465 5f72 6567 696f 6e73 5f76  update_regions_v
-00023600: 6973 6962 6c65 2829 0a0a 2020 2020 6465  isible()..    de
-00023610: 6620 5f79 7261 6e67 655f 6368 616e 6765  f _yrange_change
-00023620: 6428 7365 6c66 2c20 5f2c 2079 7261 6e67  d(self, _, yrang
-00023630: 6529 3a0a 2020 2020 2020 2020 6966 206e  e):.        if n
-00023640: 6f74 2073 656c 662e 6d6e 652e 6275 7474  ot self.mne.butt
-00023650: 6572 666c 793a 0a20 2020 2020 2020 2020  erfly:.         
-00023660: 2020 2069 6620 6e6f 7420 7365 6c66 2e6d     if not self.m
-00023670: 6e65 2e66 6967 5f73 656c 6563 7469 6f6e  ne.fig_selection
-00023680: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00023690: 2020 2320 5570 6461 7465 2070 6963 6b73    # Update picks
-000236a0: 2061 6e64 2064 6174 610a 2020 2020 2020   and data.      
-000236b0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-000236c0: 6e65 2e63 685f 7374 6172 7420 3d20 6e70  ne.ch_start = np
-000236d0: 2e63 6c69 7028 726f 756e 6428 7972 616e  .clip(round(yran
-000236e0: 6765 5b30 5d29 2c20 302c 0a20 2020 2020  ge[0]), 0,.     
-000236f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023710: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
-00023720: 6d6e 652e 6368 5f6f 7264 6572 290a 2020  mne.ch_order).  
-00023730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023750: 2020 2020 2020 2020 2020 2d20 7365 6c66            - self
-00023760: 2e6d 6e65 2e6e 5f63 6861 6e6e 656c 7329  .mne.n_channels)
-00023770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023780: 2073 656c 662e 6d6e 652e 6e5f 6368 616e   self.mne.n_chan
-00023790: 6e65 6c73 203d 2072 6f75 6e64 2879 7261  nels = round(yra
-000237a0: 6e67 655b 315d 202d 2079 7261 6e67 655b  nge[1] - yrange[
-000237b0: 305d 202d 2031 290a 2020 2020 2020 2020  0] - 1).        
-000237c0: 2020 2020 2020 2020 7365 6c66 2e5f 7570          self._up
-000237d0: 6461 7465 5f70 6963 6b73 2829 0a20 2020  date_picks().   
-000237e0: 2020 2020 2020 2020 2020 2020 2023 2055               # U
-000237f0: 7064 6174 6520 4368 616e 6e65 6c2d 4261  pdate Channel-Ba
-00023800: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00023810: 2020 7365 6c66 2e6d 6e65 2e61 785f 7673    self.mne.ax_vs
-00023820: 6372 6f6c 6c2e 7570 6461 7465 5f76 616c  croll.update_val
-00023830: 7565 2873 656c 662e 6d6e 652e 6368 5f73  ue(self.mne.ch_s
-00023840: 7461 7274 290a 2020 2020 2020 2020 2020  tart).          
-00023850: 2020 7365 6c66 2e5f 7570 6461 7465 5f64    self._update_d
-00023860: 6174 6128 290a 0a20 2020 2020 2020 2023  ata()..        #
-00023870: 2055 7064 6174 6520 4f76 6572 7669 6577   Update Overview
-00023880: 2d42 6172 0a20 2020 2020 2020 2073 656c  -Bar.        sel
-00023890: 662e 6d6e 652e 6f76 6572 7669 6577 5f62  f.mne.overview_b
-000238a0: 6172 2e75 7064 6174 655f 7669 6577 7261  ar.update_viewra
-000238b0: 6e67 6528 290a 0a20 2020 2020 2020 2023  nge()..        #
-000238c0: 2055 7064 6174 6520 5363 616c 6562 6172   Update Scalebar
-000238d0: 730a 2020 2020 2020 2020 7365 6c66 2e5f  s.        self._
-000238e0: 7570 6461 7465 5f73 6361 6c65 6261 725f  update_scalebar_
-000238f0: 795f 706f 7369 7469 6f6e 7328 290a 0a20  y_positions().. 
-00023900: 2020 2020 2020 206f 6666 5f74 7261 6365         off_trace
-00023910: 7320 3d20 5b74 7220 666f 7220 7472 2069  s = [tr for tr i
-00023920: 6e20 7365 6c66 2e6d 6e65 2e74 7261 6365  n self.mne.trace
-00023930: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00023940: 2020 2020 2020 2020 6966 2074 722e 6368          if tr.ch
-00023950: 5f69 6478 206e 6f74 2069 6e20 7365 6c66  _idx not in self
-00023960: 2e6d 6e65 2e70 6963 6b73 5d0a 2020 2020  .mne.picks].    
-00023970: 2020 2020 6164 645f 6964 7873 203d 205b      add_idxs = [
-00023980: 7020 666f 7220 7020 696e 2073 656c 662e  p for p in self.
-00023990: 6d6e 652e 7069 636b 730a 2020 2020 2020  mne.picks.      
-000239a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000239b0: 2070 206e 6f74 2069 6e20 5b74 722e 6368   p not in [tr.ch
-000239c0: 5f69 6478 2066 6f72 2074 7220 696e 2073  _idx for tr in s
-000239d0: 656c 662e 6d6e 652e 7472 6163 6573 5d5d  elf.mne.traces]]
-000239e0: 0a0a 2020 2020 2020 2020 2320 5570 6461  ..        # Upda
-000239f0: 7465 2072 616e 6765 5f69 6478 2066 6f72  te range_idx for
-00023a00: 2074 7261 6365 7320 7768 6963 6820 6a75   traces which ju
-00023a10: 7374 2073 6869 6674 6564 2069 6e20 792d  st shifted in y-
-00023a20: 706f 7369 7469 6f6e 0a20 2020 2020 2020  position.       
-00023a30: 2066 6f72 2074 7261 6365 2069 6e20 5b74   for trace in [t
-00023a40: 7220 666f 7220 7472 2069 6e20 7365 6c66  r for tr in self
-00023a50: 2e6d 6e65 2e74 7261 6365 7320 6966 2074  .mne.traces if t
-00023a60: 7220 6e6f 7420 696e 206f 6666 5f74 7261  r not in off_tra
-00023a70: 6365 735d 3a0a 2020 2020 2020 2020 2020  ces]:.          
-00023a80: 2020 7472 6163 652e 7570 6461 7465 5f72    trace.update_r
-00023a90: 616e 6765 5f69 6478 2829 0a0a 2020 2020  ange_idx()..    
-00023aa0: 2020 2020 2320 5570 6461 7465 206e 756d      # Update num
-00023ab0: 6265 7220 6f66 2074 7261 6365 732e 0a20  ber of traces.. 
-00023ac0: 2020 2020 2020 2074 7261 6365 5f64 6966         trace_dif
-00023ad0: 6620 3d20 6c65 6e28 7365 6c66 2e6d 6e65  f = len(self.mne
-00023ae0: 2e70 6963 6b73 2920 2d20 6c65 6e28 7365  .picks) - len(se
-00023af0: 6c66 2e6d 6e65 2e74 7261 6365 7329 0a0a  lf.mne.traces)..
-00023b00: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
-00023b10: 2075 6e6e 6563 6573 7361 7279 2074 7261   unnecessary tra
-00023b20: 6365 732e 0a20 2020 2020 2020 2069 6620  ces..        if 
-00023b30: 7472 6163 655f 6469 6666 203c 2030 3a0a  trace_diff < 0:.
-00023b40: 2020 2020 2020 2020 2020 2020 2320 4f6e              # On
-00023b50: 6c79 2072 656d 6f76 6520 6672 6f6d 2074  ly remove from t
-00023b60: 7261 6365 7320 6e6f 7420 696e 2070 6963  races not in pic
-00023b70: 6b73 2e0a 2020 2020 2020 2020 2020 2020  ks..            
-00023b80: 7265 6d6f 7665 5f74 7261 6365 7320 3d20  remove_traces = 
-00023b90: 6f66 665f 7472 6163 6573 5b3a 6162 7328  off_traces[:abs(
-00023ba0: 7472 6163 655f 6469 6666 295d 0a20 2020  trace_diff)].   
-00023bb0: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
-00023bc0: 6365 2069 6e20 7265 6d6f 7665 5f74 7261  ce in remove_tra
-00023bd0: 6365 733a 0a20 2020 2020 2020 2020 2020  ces:.           
-00023be0: 2020 2020 2074 7261 6365 2e72 656d 6f76       trace.remov
-00023bf0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00023c00: 2020 2020 6f66 665f 7472 6163 6573 2e72      off_traces.r
-00023c10: 656d 6f76 6528 7472 6163 6529 0a0a 2020  emove(trace)..  
-00023c20: 2020 2020 2020 2320 4164 6420 6e65 7720        # Add new 
-00023c30: 7472 6163 6573 2069 6620 6e65 6365 7373  traces if necess
-00023c40: 6172 792e 0a20 2020 2020 2020 2069 6620  ary..        if 
-00023c50: 7472 6163 655f 6469 6666 203e 2030 3a0a  trace_diff > 0:.
-00023c60: 2020 2020 2020 2020 2020 2020 2320 4d61              # Ma
-00023c70: 6b65 2063 6f70 7920 746f 2061 766f 6964  ke copy to avoid
-00023c80: 2073 6b69 7070 696e 6720 6974 6572 6174   skipping iterat
-00023c90: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
-00023ca0: 2069 6478 735f 636f 7079 203d 2061 6464   idxs_copy = add
-00023cb0: 5f69 6478 732e 636f 7079 2829 0a20 2020  _idxs.copy().   
-00023cc0: 2020 2020 2020 2020 2066 6f72 2061 6964           for aid
-00023cd0: 7820 696e 2069 6478 735f 636f 7079 5b3a  x in idxs_copy[:
-00023ce0: 7472 6163 655f 6469 6666 5d3a 0a20 2020  trace_diff]:.   
-00023cf0: 2020 2020 2020 2020 2020 2020 2044 6174               Dat
-00023d00: 6154 7261 6365 2873 656c 662c 2061 6964  aTrace(self, aid
-00023d10: 7829 0a20 2020 2020 2020 2020 2020 2020  x).             
-00023d20: 2020 2061 6464 5f69 6478 732e 7265 6d6f     add_idxs.remo
-00023d30: 7665 2861 6964 7829 0a0a 2020 2020 2020  ve(aidx)..      
-00023d40: 2020 2320 5570 6461 7465 2064 6174 6120    # Update data 
-00023d50: 6f66 2074 7261 6365 7320 6f75 7473 6964  of traces outsid
-00023d60: 6520 6f66 2079 7261 6e67 6520 2872 6575  e of yrange (reu
-00023d70: 7365 2072 656d 6169 6e69 6e67 2074 7261  se remaining tra
-00023d80: 6365 2d69 7465 6d73 290a 2020 2020 2020  ce-items).      
-00023d90: 2020 666f 7220 7472 6163 652c 2063 685f    for trace, ch_
-00023da0: 6964 7820 696e 207a 6970 286f 6666 5f74  idx in zip(off_t
-00023db0: 7261 6365 732c 2061 6464 5f69 6478 7329  races, add_idxs)
-00023dc0: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-00023dd0: 6163 652e 7365 745f 6368 5f69 6478 2863  ace.set_ch_idx(c
-00023de0: 685f 6964 7829 0a20 2020 2020 2020 2020  h_idx).         
-00023df0: 2020 2074 7261 6365 2e75 7064 6174 655f     trace.update_
-00023e00: 636f 6c6f 7228 290a 2020 2020 2020 2020  color().        
-00023e10: 2020 2020 7472 6163 652e 7570 6461 7465      trace.update
-00023e20: 5f64 6174 6128 290a 0a20 2020 2023 2023  _data()..    # #
-00023e30: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
-00023e40: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
-00023e50: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
-00023e60: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
-00023e70: 2023 2023 2023 2023 0a20 2020 2023 2044   # # # #.    # D
-00023e80: 4154 4120 4841 4e44 4c49 4e47 0a20 2020  ATA HANDLING.   
-00023e90: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
-00023ea0: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
-00023eb0: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
-00023ec0: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
-00023ed0: 2023 2023 2023 2023 2023 2023 0a20 2020   # # # # # #.   
-00023ee0: 2064 6566 205f 6170 706c 795f 646f 776e   def _apply_down
-00023ef0: 7361 6d70 6c69 6e67 2873 656c 6629 3a0a  sampling(self):.
-00023f00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00023f10: 2020 2020 4765 7420 6473 2d66 6163 746f      Get ds-facto
-00023f20: 7220 616e 6420 6170 706c 7920 6473 2077  r and apply ds w
-00023f30: 6974 6820 6f6e 6520 6f66 206d 756c 7469  ith one of multi
-00023f40: 706c 6520 6d65 7468 6f64 732e 0a0a 2020  ple methods...  
-00023f50: 2020 2020 2020 5468 6520 6d65 7468 6f64        The method
-00023f60: 7320 6172 6520 7461 6b65 6e20 6672 6f6d  s are taken from
-00023f70: 2050 6c6f 7444 6174 6149 7465 6d20 696e   PlotDataItem in
-00023f80: 2070 7971 7467 7261 7068 0a20 2020 2020   pyqtgraph.     
-00023f90: 2020 2061 6e64 2061 646a 7573 7465 6420     and adjusted 
-00023fa0: 746f 206d 756c 7469 2d63 6861 6e6e 656c  to multi-channel
-00023fb0: 2064 6174 612e 0a20 2020 2020 2020 2022   data..        "
-00023fc0: 2222 0a20 2020 2020 2020 2023 2047 6574  "".        # Get
-00023fd0: 2044 6f77 6e73 616d 706c 696e 672d 4661   Downsampling-Fa
-00023fe0: 6374 6f72 0a20 2020 2020 2020 2023 2041  ctor.        # A
-00023ff0: 7574 6f2d 446f 776e 7361 6d70 6c69 6e67  uto-Downsampling
-00024000: 2066 726f 6d20 7079 7174 6772 6170 680a   from pyqtgraph.
-00024010: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00024020: 6d6e 652e 646f 776e 7361 6d70 6c69 6e67  mne.downsampling
-00024030: 203d 3d20 2761 7574 6f27 3a0a 2020 2020   == 'auto':.    
-00024040: 2020 2020 2020 2020 6473 203d 2031 0a20          ds = 1. 
-00024050: 2020 2020 2020 2020 2020 2069 6620 616c             if al
-00024060: 6c28 5b68 6173 6174 7472 2873 656c 662e  l([hasattr(self.
-00024070: 6d6e 652c 2061 2920 666f 7220 6120 696e  mne, a) for a in
-00024080: 205b 2776 6965 7762 6f78 272c 2027 7469   ['viewbox', 'ti
-00024090: 6d65 7327 5d5d 293a 0a20 2020 2020 2020  mes']]):.       
-000240a0: 2020 2020 2020 2020 2076 6220 3d20 7365           vb = se
-000240b0: 6c66 2e6d 6e65 2e76 6965 7762 6f78 0a20  lf.mne.viewbox. 
-000240c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000240d0: 6620 7662 2069 7320 6e6f 7420 4e6f 6e65  f vb is not None
-000240e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000240f0: 2020 2020 2020 7669 6577 5f72 616e 6765        view_range
-00024100: 203d 2076 622e 7669 6577 5265 6374 2829   = vb.viewRect()
-00024110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024120: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00024130: 2020 2020 2020 2020 2020 2076 6965 775f             view_
-00024140: 7261 6e67 6520 3d20 4e6f 6e65 0a20 2020  range = None.   
-00024150: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00024160: 7669 6577 5f72 616e 6765 2069 7320 6e6f  view_range is no
-00024170: 7420 4e6f 6e65 2061 6e64 206c 656e 2873  t None and len(s
-00024180: 656c 662e 6d6e 652e 7469 6d65 7329 203e  elf.mne.times) >
-00024190: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-000241a0: 2020 2020 2020 2020 6478 203d 2066 6c6f          dx = flo
-000241b0: 6174 2873 656c 662e 6d6e 652e 7469 6d65  at(self.mne.time
-000241c0: 735b 2d31 5d20 2d20 7365 6c66 2e6d 6e65  s[-1] - self.mne
-000241d0: 2e74 696d 6573 5b30 5d29 202f 2028 0a20  .times[0]) / (. 
-000241e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000241f0: 2020 2020 2020 2020 2020 206c 656e 2873             len(s
-00024200: 656c 662e 6d6e 652e 7469 6d65 7329 202d  elf.mne.times) -
-00024210: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
-00024220: 2020 2020 2020 2020 6966 2064 7820 213d          if dx !=
-00024230: 2030 2e30 3a0a 2020 2020 2020 2020 2020   0.0:.          
-00024240: 2020 2020 2020 2020 2020 2020 2020 7830                x0
-00024250: 203d 2076 6965 775f 7261 6e67 652e 6c65   = view_range.le
-00024260: 6674 2829 202f 2064 780a 2020 2020 2020  ft() / dx.      
-00024270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024280: 2020 7831 203d 2076 6965 775f 7261 6e67    x1 = view_rang
-00024290: 652e 7269 6768 7428 2920 2f20 6478 0a20  e.right() / dx. 
-000242a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000242b0: 2020 2020 2020 2077 6964 7468 203d 2076         width = v
-000242c0: 622e 7769 6474 6828 290a 2020 2020 2020  b.width().      
+00022d50: 2020 2020 2020 2023 2072 656c 6174 6976         # relativ
+00022d60: 6520 7820 666f 7220 6570 6f63 6873 0a20  e x for epochs. 
+00022d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022d80: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00022d90: 6e65 2e69 735f 6570 6f63 6873 3a0a 2020  ne.is_epochs:.  
+00022da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022db0: 2020 2020 2020 2020 2020 7265 6c5f 6964            rel_id
+00022dc0: 7820 3d20 6964 7820 2520 6c65 6e28 7365  x = idx % len(se
+00022dd0: 6c66 2e6d 6e65 2e69 6e73 742e 7469 6d65  lf.mne.inst.time
+00022de0: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00022df0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00022e00: 203d 2073 656c 662e 6d6e 652e 696e 7374   = self.mne.inst
+00022e10: 2e74 696d 6573 5b72 656c 5f69 6478 5d0a  .times[rel_idx].
+00022e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022e30: 2020 2020 2020 2020 2023 206e 6567 6174           # negat
+00022e40: 6976 6520 6265 6361 7573 6520 706c 6f74  ive because plot
+00022e50: 2069 7320 696e 7665 7274 6564 2066 6f72   is inverted for
+00022e60: 2059 0a20 2020 2020 2020 2020 2020 2020   Y.             
+00022e70: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00022e80: 7220 3d20 2d31 2069 6620 7365 6c66 2e6d  r = -1 if self.m
+00022e90: 6e65 2e62 7574 7465 7266 6c79 2065 6c73  ne.butterfly els
+00022ea0: 6520 2d32 0a20 2020 2020 2020 2020 2020  e -2.           
+00022eb0: 2020 2020 2020 2020 2020 2020 2069 6e76               inv
+00022ec0: 5f6e 6f72 6d20 3d20 2873 6361 6c65 7220  _norm = (scaler 
+00022ed0: 2a0a 2020 2020 2020 2020 2020 2020 2020  *.              
+00022ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022ef0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e73        self.mne.s
+00022f00: 6361 6c69 6e67 735b 7472 6163 652e 6368  calings[trace.ch
+00022f10: 5f74 7970 655d 202a 0a20 2020 2020 2020  _type] *.       
+00022f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022f30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00022f40: 662e 6d6e 652e 756e 6974 5f73 6361 6c69  f.mne.unit_scali
+00022f50: 6e67 735b 7472 6163 652e 6368 5f74 7970  ngs[trace.ch_typ
+00022f60: 655d 202f 0a20 2020 2020 2020 2020 2020  e] /.           
+00022f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022f80: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
+00022f90: 652e 7363 616c 655f 6661 6374 6f72 290a  e.scale_factor).
+00022fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022fb0: 2020 2020 2020 2020 6c61 6265 6c20 3d20          label = 
+00022fc0: 6627 7b5f 7369 6d70 6c69 6679 5f66 6c6f  f'{_simplify_flo
+00022fd0: 6174 2879 7661 6c75 6520 2a20 696e 765f  at(yvalue * inv_
+00022fe0: 6e6f 726d 297d 2027 205c 0a20 2020 2020  norm)} ' \.     
+00022ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023000: 2020 2020 2020 2020 2020 2066 277b 7365             f'{se
+00023010: 6c66 2e6d 6e65 2e75 6e69 7473 5b74 7261  lf.mne.units[tra
+00023020: 6365 2e63 685f 7479 7065 5d7d 270a 2020  ce.ch_type]}'.  
+00023030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023040: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00023050: 7342 6172 2829 2e73 686f 774d 6573 7361  sBar().showMessa
+00023060: 6765 2866 2778 3d7b 783a 2e33 667d 2073  ge(f'x={x:.3f} s
+00023070: 2c20 270a 2020 2020 2020 2020 2020 2020  , '.            
+00023080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000230a0: 2020 2020 2020 2020 2066 2779 3d7b 6c61           f'y={la
+000230b0: 6265 6c7d 2729 0a0a 2020 2020 6465 6620  bel}')..    def 
+000230c0: 5f74 6f67 676c 655f 6372 6f73 7368 6169  _toggle_crosshai
+000230d0: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+000230e0: 2073 656c 662e 6d6e 652e 6372 6f73 7368   self.mne.crossh
+000230f0: 6169 725f 656e 6162 6c65 6420 3d20 6e6f  air_enabled = no
+00023100: 7420 7365 6c66 2e6d 6e65 2e63 726f 7373  t self.mne.cross
+00023110: 6861 6972 5f65 6e61 626c 6564 0a20 2020  hair_enabled.   
+00023120: 2020 2020 2069 6620 7365 6c66 2e6d 6e65       if self.mne
+00023130: 2e63 726f 7373 6861 6972 3a0a 2020 2020  .crosshair:.    
+00023140: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
+00023150: 2e70 6c74 2e72 656d 6f76 6549 7465 6d28  .plt.removeItem(
+00023160: 7365 6c66 2e6d 6e65 2e63 726f 7373 6861  self.mne.crossha
+00023170: 6972 290a 2020 2020 2020 2020 2020 2020  ir).            
+00023180: 7365 6c66 2e6d 6e65 2e63 726f 7373 6861  self.mne.crossha
+00023190: 6972 203d 204e 6f6e 650a 0a20 2020 2064  ir = None..    d
+000231a0: 6566 205f 7872 616e 6765 5f63 6861 6e67  ef _xrange_chang
+000231b0: 6564 2873 656c 662c 205f 2c20 7872 616e  ed(self, _, xran
+000231c0: 6765 293a 0a20 2020 2020 2020 2023 2055  ge):.        # U
+000231d0: 7064 6174 6520 6461 7461 0a20 2020 2020  pdate data.     
+000231e0: 2020 2069 6620 7365 6c66 2e6d 6e65 2e69     if self.mne.i
+000231f0: 735f 6570 6f63 6873 3a0a 2020 2020 2020  s_epochs:.      
+00023200: 2020 2020 2020 6966 2073 656c 662e 6d6e        if self.mn
+00023210: 652e 766c 696e 6520 6973 206e 6f74 204e  e.vline is not N
+00023220: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00023230: 2020 2020 2072 656c 5f76 6c5f 7420 3d20       rel_vl_t = 
+00023240: 7365 6c66 2e6d 6e65 2e76 6c69 6e65 5b30  self.mne.vline[0
+00023250: 5d2e 7661 6c75 6528 2920 5c0a 2020 2020  ].value() \.    
+00023260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023270: 2020 2020 2020 202d 2073 656c 662e 6d6e         - self.mn
+00023280: 652e 626f 756e 6461 7279 5f74 696d 6573  e.boundary_times
+00023290: 5b73 656c 662e 6d6e 652e 6570 6f63 685f  [self.mne.epoch_
+000232a0: 6964 785d 5b30 5d0a 0a20 2020 2020 2020  idx][0]..       
+000232b0: 2020 2020 2023 2044 6570 656e 6473 206f       # Depends o
+000232c0: 6e20 6f6e 6c79 2061 6c6c 6f77 696e 6720  n only allowing 
+000232d0: 7872 616e 6765 2073 686f 7769 6e67 2066  xrange showing f
+000232e0: 756c 6c20 6570 6f63 6873 0a20 2020 2020  ull epochs.     
+000232f0: 2020 2020 2020 2062 6f75 6e64 6172 795f         boundary_
+00023300: 6964 7873 203d 206e 702e 7365 6172 6368  idxs = np.search
+00023310: 736f 7274 6564 2873 656c 662e 6d6e 652e  sorted(self.mne.
+00023320: 6d69 6470 6f69 6e74 732c 2078 7261 6e67  midpoints, xrang
+00023330: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
+00023340: 656c 662e 6d6e 652e 6570 6f63 685f 6964  elf.mne.epoch_id
+00023350: 7820 3d20 6e70 2e61 7261 6e67 6528 2a62  x = np.arange(*b
+00023360: 6f75 6e64 6172 795f 6964 7873 290a 0a20  oundary_idxs).. 
+00023370: 2020 2020 2020 2020 2020 2023 2055 7064             # Upd
+00023380: 6174 6520 636f 6c6f 7273 0a20 2020 2020  ate colors.     
+00023390: 2020 2020 2020 2066 6f72 2074 7261 6365         for trace
+000233a0: 2069 6e20 7365 6c66 2e6d 6e65 2e74 7261   in self.mne.tra
+000233b0: 6365 733a 0a20 2020 2020 2020 2020 2020  ces:.           
+000233c0: 2020 2020 2074 7261 6365 2e75 7064 6174       trace.updat
+000233d0: 655f 636f 6c6f 7228 290a 0a20 2020 2020  e_color()..     
+000233e0: 2020 2020 2020 2023 2055 7064 6174 6520         # Update 
+000233f0: 766c 696e 6573 0a20 2020 2020 2020 2020  vlines.         
+00023400: 2020 2069 6620 7365 6c66 2e6d 6e65 2e76     if self.mne.v
+00023410: 6c69 6e65 2069 7320 6e6f 7420 4e6f 6e65  line is not None
+00023420: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00023430: 2020 666f 7220 626d 696e 2c20 626d 6178    for bmin, bmax
+00023440: 2c20 766c 2069 6e20 7a69 7028 7365 6c66  , vl in zip(self
+00023450: 2e6d 6e65 2e62 6f75 6e64 6172 795f 7469  .mne.boundary_ti
+00023460: 6d65 735b 0a20 2020 2020 2020 2020 2020  mes[.           
+00023470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023490: 2020 2073 656c 662e 6d6e 652e 6570 6f63     self.mne.epoc
+000234a0: 685f 6964 785d 2c0a 2020 2020 2020 2020  h_idx],.        
+000234b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000234c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000234d0: 2020 7365 6c66 2e6d 6e65 2e62 6f75 6e64    self.mne.bound
+000234e0: 6172 795f 7469 6d65 735b 0a20 2020 2020  ary_times[.     
+000234f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023510: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
+00023520: 652e 6570 6f63 685f 6964 7820 2b20 315d  e.epoch_idx + 1]
+00023530: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00023540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00023560: 2e6d 6e65 2e76 6c69 6e65 293a 0a20 2020  .mne.vline):.   
+00023570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023580: 2023 2041 766f 6964 206f 6666 2d62 792d   # Avoid off-by-
+00023590: 6f6e 652d 6572 726f 7220 6174 2062 6d61  one-error at bma
+000235a0: 7820 666f 7220 566c 696e 654c 6162 656c  x for VlineLabel
+000235b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000235c0: 2020 2020 2062 6d61 7820 2d3d 2031 202f       bmax -= 1 /
+000235d0: 2073 656c 662e 6d6e 652e 696e 666f 5b27   self.mne.info['
+000235e0: 7366 7265 7127 5d0a 2020 2020 2020 2020  sfreq'].        
+000235f0: 2020 2020 2020 2020 2020 2020 766c 2e73              vl.s
+00023600: 6574 426f 756e 6473 2828 626d 696e 2c20  etBounds((bmin, 
+00023610: 626d 6178 2929 0a20 2020 2020 2020 2020  bmax)).         
+00023620: 2020 2020 2020 2020 2020 2076 6c2e 7365             vl.se
+00023630: 7456 616c 7565 2862 6d69 6e20 2b20 7265  tValue(bmin + re
+00023640: 6c5f 766c 5f74 290a 0a20 2020 2020 2020  l_vl_t)..       
+00023650: 2073 656c 662e 6d6e 652e 745f 7374 6172   self.mne.t_star
+00023660: 7420 3d20 7872 616e 6765 5b30 5d0a 2020  t = xrange[0].  
+00023670: 2020 2020 2020 7365 6c66 2e6d 6e65 2e64        self.mne.d
+00023680: 7572 6174 696f 6e20 3d20 7872 616e 6765  uration = xrange
+00023690: 5b31 5d20 2d20 7872 616e 6765 5b30 5d0a  [1] - xrange[0].
+000236a0: 0a20 2020 2020 2020 2073 656c 662e 5f72  .        self._r
+000236b0: 6564 7261 7728 7570 6461 7465 5f64 6174  edraw(update_dat
+000236c0: 613d 5472 7565 290a 0a20 2020 2020 2020  a=True)..       
+000236d0: 2023 2055 7064 6174 6520 5469 6d65 2d42   # Update Time-B
+000236e0: 6172 0a20 2020 2020 2020 2073 656c 662e  ar.        self.
+000236f0: 6d6e 652e 6178 5f68 7363 726f 6c6c 2e75  mne.ax_hscroll.u
+00023700: 7064 6174 655f 7661 6c75 6528 7872 616e  pdate_value(xran
+00023710: 6765 5b30 5d29 0a0a 2020 2020 2020 2020  ge[0])..        
+00023720: 2320 5570 6461 7465 204f 7665 7276 6965  # Update Overvie
+00023730: 772d 4261 720a 2020 2020 2020 2020 7365  w-Bar.        se
+00023740: 6c66 2e6d 6e65 2e6f 7665 7276 6965 775f  lf.mne.overview_
+00023750: 6261 722e 7570 6461 7465 5f76 6965 7772  bar.update_viewr
+00023760: 616e 6765 2829 0a0a 2020 2020 2020 2020  ange()..        
+00023770: 2320 5570 6461 7465 2053 6361 6c65 6261  # Update Scaleba
+00023780: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
+00023790: 5f75 7064 6174 655f 7363 616c 6562 6172  _update_scalebar
+000237a0: 5f78 5f70 6f73 6974 696f 6e73 2829 0a0a  _x_positions()..
+000237b0: 2020 2020 2020 2020 2320 5570 6461 7465          # Update
+000237c0: 2061 6e6e 6f74 6174 696f 6e73 0a20 2020   annotations.   
+000237d0: 2020 2020 2073 656c 662e 5f75 7064 6174       self._updat
+000237e0: 655f 7265 6769 6f6e 735f 7669 7369 626c  e_regions_visibl
+000237f0: 6528 290a 0a20 2020 2064 6566 205f 7972  e()..    def _yr
+00023800: 616e 6765 5f63 6861 6e67 6564 2873 656c  ange_changed(sel
+00023810: 662c 205f 2c20 7972 616e 6765 293a 0a20  f, _, yrange):. 
+00023820: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00023830: 6c66 2e6d 6e65 2e62 7574 7465 7266 6c79  lf.mne.butterfly
+00023840: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00023850: 206e 6f74 2073 656c 662e 6d6e 652e 6669   not self.mne.fi
+00023860: 675f 7365 6c65 6374 696f 6e3a 0a20 2020  g_selection:.   
+00023870: 2020 2020 2020 2020 2020 2020 2023 2055               # U
+00023880: 7064 6174 6520 7069 636b 7320 616e 6420  pdate picks and 
+00023890: 6461 7461 0a20 2020 2020 2020 2020 2020  data.           
+000238a0: 2020 2020 2073 656c 662e 6d6e 652e 6368       self.mne.ch
+000238b0: 5f73 7461 7274 203d 206e 702e 636c 6970  _start = np.clip
+000238c0: 2872 6f75 6e64 2879 7261 6e67 655b 305d  (round(yrange[0]
+000238d0: 292c 2030 2c0a 2020 2020 2020 2020 2020  ), 0,.          
+000238e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000238f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023900: 2020 6c65 6e28 7365 6c66 2e6d 6e65 2e63    len(self.mne.c
+00023910: 685f 6f72 6465 7229 0a20 2020 2020 2020  h_order).       
+00023920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023940: 2020 2020 202d 2073 656c 662e 6d6e 652e       - self.mne.
+00023950: 6e5f 6368 616e 6e65 6c73 290a 2020 2020  n_channels).    
+00023960: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00023970: 2e6d 6e65 2e6e 5f63 6861 6e6e 656c 7320  .mne.n_channels 
+00023980: 3d20 726f 756e 6428 7972 616e 6765 5b31  = round(yrange[1
+00023990: 5d20 2d20 7972 616e 6765 5b30 5d20 2d20  ] - yrange[0] - 
+000239a0: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
+000239b0: 2020 2073 656c 662e 5f75 7064 6174 655f     self._update_
+000239c0: 7069 636b 7328 290a 2020 2020 2020 2020  picks().        
+000239d0: 2020 2020 2020 2020 2320 5570 6461 7465          # Update
+000239e0: 2043 6861 6e6e 656c 2d42 6172 0a20 2020   Channel-Bar.   
+000239f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00023a00: 662e 6d6e 652e 6178 5f76 7363 726f 6c6c  f.mne.ax_vscroll
+00023a10: 2e75 7064 6174 655f 7661 6c75 6528 7365  .update_value(se
+00023a20: 6c66 2e6d 6e65 2e63 685f 7374 6172 7429  lf.mne.ch_start)
+00023a30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00023a40: 662e 5f75 7064 6174 655f 6461 7461 2829  f._update_data()
+00023a50: 0a0a 2020 2020 2020 2020 2320 5570 6461  ..        # Upda
+00023a60: 7465 204f 7665 7276 6965 772d 4261 720a  te Overview-Bar.
+00023a70: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
+00023a80: 2e6f 7665 7276 6965 775f 6261 722e 7570  .overview_bar.up
+00023a90: 6461 7465 5f76 6965 7772 616e 6765 2829  date_viewrange()
+00023aa0: 0a0a 2020 2020 2020 2020 2320 5570 6461  ..        # Upda
+00023ab0: 7465 2053 6361 6c65 6261 7273 0a20 2020  te Scalebars.   
+00023ac0: 2020 2020 2073 656c 662e 5f75 7064 6174       self._updat
+00023ad0: 655f 7363 616c 6562 6172 5f79 5f70 6f73  e_scalebar_y_pos
+00023ae0: 6974 696f 6e73 2829 0a0a 2020 2020 2020  itions()..      
+00023af0: 2020 6f66 665f 7472 6163 6573 203d 205b    off_traces = [
+00023b00: 7472 2066 6f72 2074 7220 696e 2073 656c  tr for tr in sel
+00023b10: 662e 6d6e 652e 7472 6163 6573 0a20 2020  f.mne.traces.   
+00023b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023b30: 2020 2069 6620 7472 2e63 685f 6964 7820     if tr.ch_idx 
+00023b40: 6e6f 7420 696e 2073 656c 662e 6d6e 652e  not in self.mne.
+00023b50: 7069 636b 735d 0a20 2020 2020 2020 2061  picks].        a
+00023b60: 6464 5f69 6478 7320 3d20 5b70 2066 6f72  dd_idxs = [p for
+00023b70: 2070 2069 6e20 7365 6c66 2e6d 6e65 2e70   p in self.mne.p
+00023b80: 6963 6b73 0a20 2020 2020 2020 2020 2020  icks.           
+00023b90: 2020 2020 2020 2020 2069 6620 7020 6e6f           if p no
+00023ba0: 7420 696e 205b 7472 2e63 685f 6964 7820  t in [tr.ch_idx 
+00023bb0: 666f 7220 7472 2069 6e20 7365 6c66 2e6d  for tr in self.m
+00023bc0: 6e65 2e74 7261 6365 735d 5d0a 0a20 2020  ne.traces]]..   
+00023bd0: 2020 2020 2023 2055 7064 6174 6520 7261       # Update ra
+00023be0: 6e67 655f 6964 7820 666f 7220 7472 6163  nge_idx for trac
+00023bf0: 6573 2077 6869 6368 206a 7573 7420 7368  es which just sh
+00023c00: 6966 7465 6420 696e 2079 2d70 6f73 6974  ifted in y-posit
+00023c10: 696f 6e0a 2020 2020 2020 2020 666f 7220  ion.        for 
+00023c20: 7472 6163 6520 696e 205b 7472 2066 6f72  trace in [tr for
+00023c30: 2074 7220 696e 2073 656c 662e 6d6e 652e   tr in self.mne.
+00023c40: 7472 6163 6573 2069 6620 7472 206e 6f74  traces if tr not
+00023c50: 2069 6e20 6f66 665f 7472 6163 6573 5d3a   in off_traces]:
+00023c60: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
+00023c70: 6365 2e75 7064 6174 655f 7261 6e67 655f  ce.update_range_
+00023c80: 6964 7828 290a 0a20 2020 2020 2020 2023  idx()..        #
+00023c90: 2055 7064 6174 6520 6e75 6d62 6572 206f   Update number o
+00023ca0: 6620 7472 6163 6573 2e0a 2020 2020 2020  f traces..      
+00023cb0: 2020 7472 6163 655f 6469 6666 203d 206c    trace_diff = l
+00023cc0: 656e 2873 656c 662e 6d6e 652e 7069 636b  en(self.mne.pick
+00023cd0: 7329 202d 206c 656e 2873 656c 662e 6d6e  s) - len(self.mn
+00023ce0: 652e 7472 6163 6573 290a 0a20 2020 2020  e.traces)..     
+00023cf0: 2020 2023 2052 656d 6f76 6520 756e 6e65     # Remove unne
+00023d00: 6365 7373 6172 7920 7472 6163 6573 2e0a  cessary traces..
+00023d10: 2020 2020 2020 2020 6966 2074 7261 6365          if trace
+00023d20: 5f64 6966 6620 3c20 303a 0a20 2020 2020  _diff < 0:.     
+00023d30: 2020 2020 2020 2023 204f 6e6c 7920 7265         # Only re
+00023d40: 6d6f 7665 2066 726f 6d20 7472 6163 6573  move from traces
+00023d50: 206e 6f74 2069 6e20 7069 636b 732e 0a20   not in picks.. 
+00023d60: 2020 2020 2020 2020 2020 2072 656d 6f76             remov
+00023d70: 655f 7472 6163 6573 203d 206f 6666 5f74  e_traces = off_t
+00023d80: 7261 6365 735b 3a61 6273 2874 7261 6365  races[:abs(trace
+00023d90: 5f64 6966 6629 5d0a 2020 2020 2020 2020  _diff)].        
+00023da0: 2020 2020 666f 7220 7472 6163 6520 696e      for trace in
+00023db0: 2072 656d 6f76 655f 7472 6163 6573 3a0a   remove_traces:.
+00023dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023dd0: 7472 6163 652e 7265 6d6f 7665 2829 0a20  trace.remove(). 
+00023de0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00023df0: 6666 5f74 7261 6365 732e 7265 6d6f 7665  ff_traces.remove
+00023e00: 2874 7261 6365 290a 0a20 2020 2020 2020  (trace)..       
+00023e10: 2023 2041 6464 206e 6577 2074 7261 6365   # Add new trace
+00023e20: 7320 6966 206e 6563 6573 7361 7279 2e0a  s if necessary..
+00023e30: 2020 2020 2020 2020 6966 2074 7261 6365          if trace
+00023e40: 5f64 6966 6620 3e20 303a 0a20 2020 2020  _diff > 0:.     
+00023e50: 2020 2020 2020 2023 204d 616b 6520 636f         # Make co
+00023e60: 7079 2074 6f20 6176 6f69 6420 736b 6970  py to avoid skip
+00023e70: 7069 6e67 2069 7465 7261 7469 6f6e 2e0a  ping iteration..
+00023e80: 2020 2020 2020 2020 2020 2020 6964 7873              idxs
+00023e90: 5f63 6f70 7920 3d20 6164 645f 6964 7873  _copy = add_idxs
+00023ea0: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
+00023eb0: 2020 2020 666f 7220 6169 6478 2069 6e20      for aidx in 
+00023ec0: 6964 7873 5f63 6f70 795b 3a74 7261 6365  idxs_copy[:trace
+00023ed0: 5f64 6966 665d 3a0a 2020 2020 2020 2020  _diff]:.        
+00023ee0: 2020 2020 2020 2020 4461 7461 5472 6163          DataTrac
+00023ef0: 6528 7365 6c66 2c20 6169 6478 290a 2020  e(self, aidx).  
+00023f00: 2020 2020 2020 2020 2020 2020 2020 6164                ad
+00023f10: 645f 6964 7873 2e72 656d 6f76 6528 6169  d_idxs.remove(ai
+00023f20: 6478 290a 0a20 2020 2020 2020 2023 2055  dx)..        # U
+00023f30: 7064 6174 6520 6461 7461 206f 6620 7472  pdate data of tr
+00023f40: 6163 6573 206f 7574 7369 6465 206f 6620  aces outside of 
+00023f50: 7972 616e 6765 2028 7265 7573 6520 7265  yrange (reuse re
+00023f60: 6d61 696e 696e 6720 7472 6163 652d 6974  maining trace-it
+00023f70: 656d 7329 0a20 2020 2020 2020 2066 6f72  ems).        for
+00023f80: 2074 7261 6365 2c20 6368 5f69 6478 2069   trace, ch_idx i
+00023f90: 6e20 7a69 7028 6f66 665f 7472 6163 6573  n zip(off_traces
+00023fa0: 2c20 6164 645f 6964 7873 293a 0a20 2020  , add_idxs):.   
+00023fb0: 2020 2020 2020 2020 2074 7261 6365 2e73           trace.s
+00023fc0: 6574 5f63 685f 6964 7828 6368 5f69 6478  et_ch_idx(ch_idx
+00023fd0: 290a 2020 2020 2020 2020 2020 2020 7472  ).            tr
+00023fe0: 6163 652e 7570 6461 7465 5f63 6f6c 6f72  ace.update_color
+00023ff0: 2829 0a20 2020 2020 2020 2020 2020 2074  ().            t
+00024000: 7261 6365 2e75 7064 6174 655f 6461 7461  race.update_data
+00024010: 2829 0a0a 2020 2020 2320 2320 2320 2320  ()..    # # # # 
+00024020: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
+00024030: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
+00024040: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
+00024050: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
+00024060: 2320 230a 2020 2020 2320 4441 5441 2048  # #.    # DATA H
+00024070: 414e 444c 494e 470a 2020 2020 2320 2320  ANDLING.    # # 
+00024080: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
+00024090: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
+000240a0: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
+000240b0: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
+000240c0: 2320 2320 2320 230a 2020 2020 6465 6620  # # # #.    def 
+000240d0: 5f61 7070 6c79 5f64 6f77 6e73 616d 706c  _apply_downsampl
+000240e0: 696e 6728 7365 6c66 293a 0a20 2020 2020  ing(self):.     
+000240f0: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
+00024100: 6574 2064 732d 6661 6374 6f72 2061 6e64  et ds-factor and
+00024110: 2061 7070 6c79 2064 7320 7769 7468 206f   apply ds with o
+00024120: 6e65 206f 6620 6d75 6c74 6970 6c65 206d  ne of multiple m
+00024130: 6574 686f 6473 2e0a 0a20 2020 2020 2020  ethods...       
+00024140: 2054 6865 206d 6574 686f 6473 2061 7265   The methods are
+00024150: 2074 616b 656e 2066 726f 6d20 506c 6f74   taken from Plot
+00024160: 4461 7461 4974 656d 2069 6e20 7079 7174  DataItem in pyqt
+00024170: 6772 6170 680a 2020 2020 2020 2020 616e  graph.        an
+00024180: 6420 6164 6a75 7374 6564 2074 6f20 6d75  d adjusted to mu
+00024190: 6c74 692d 6368 616e 6e65 6c20 6461 7461  lti-channel data
+000241a0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000241b0: 2020 2020 2020 2320 4765 7420 446f 776e        # Get Down
+000241c0: 7361 6d70 6c69 6e67 2d46 6163 746f 720a  sampling-Factor.
+000241d0: 2020 2020 2020 2020 2320 4175 746f 2d44          # Auto-D
+000241e0: 6f77 6e73 616d 706c 696e 6720 6672 6f6d  ownsampling from
+000241f0: 2070 7971 7467 7261 7068 0a20 2020 2020   pyqtgraph.     
+00024200: 2020 2069 6620 7365 6c66 2e6d 6e65 2e64     if self.mne.d
+00024210: 6f77 6e73 616d 706c 696e 6720 3d3d 2027  ownsampling == '
+00024220: 6175 746f 273a 0a20 2020 2020 2020 2020  auto':.         
+00024230: 2020 2064 7320 3d20 310a 2020 2020 2020     ds = 1.      
+00024240: 2020 2020 2020 6966 2061 6c6c 285b 6861        if all([ha
+00024250: 7361 7474 7228 7365 6c66 2e6d 6e65 2c20  sattr(self.mne, 
+00024260: 6129 2066 6f72 2061 2069 6e20 5b27 7669  a) for a in ['vi
+00024270: 6577 626f 7827 2c20 2774 696d 6573 275d  ewbox', 'times']
+00024280: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+00024290: 2020 2020 7662 203d 2073 656c 662e 6d6e      vb = self.mn
+000242a0: 652e 7669 6577 626f 780a 2020 2020 2020  e.viewbox.      
+000242b0: 2020 2020 2020 2020 2020 6966 2076 6220            if vb 
+000242c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
 000242d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000242e0: 2020 6966 2077 6964 7468 2021 3d20 302e    if width != 0.
-000242f0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-00024300: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00024310: 2041 7574 6f2d 446f 776e 7361 6d70 6c69   Auto-Downsampli
-00024320: 6e67 2077 6974 6820 3520 7361 6d70 6c65  ng with 5 sample
-00024330: 7320 7065 7220 7069 7865 6c0a 2020 2020  s per pixel.    
-00024340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024350: 2020 2020 2020 2020 6473 203d 2069 6e74          ds = int
-00024360: 286d 6178 2831 2c20 2878 3120 2d20 7830  (max(1, (x1 - x0
-00024370: 2920 2f20 2877 6964 7468 202a 2035 2929  ) / (width * 5))
-00024380: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00024390: 2020 2020 2020 2020 2020 2020 6473 203d              ds =
-000243a0: 2073 656c 662e 6d6e 652e 646f 776e 7361   self.mne.downsa
-000243b0: 6d70 6c69 6e67 0a0a 2020 2020 2020 2020  mpling..        
-000243c0: 2320 4170 706c 7920 446f 776e 7361 6d70  # Apply Downsamp
-000243d0: 6c69 6e67 0a20 2020 2020 2020 2069 6620  ling.        if 
-000243e0: 6473 206e 6f74 2069 6e20 5b4e 6f6e 652c  ds not in [None,
-000243f0: 2031 5d3a 0a20 2020 2020 2020 2020 2020   1]:.           
-00024400: 2074 696d 6573 203d 2073 656c 662e 6d6e   times = self.mn
-00024410: 652e 7469 6d65 730a 2020 2020 2020 2020  e.times.        
-00024420: 2020 2020 6461 7461 203d 2073 656c 662e      data = self.
-00024430: 6d6e 652e 6461 7461 0a20 2020 2020 2020  mne.data.       
-00024440: 2020 2020 206e 5f63 6820 3d20 6461 7461       n_ch = data
-00024450: 2e73 6861 7065 5b30 5d0a 0a20 2020 2020  .shape[0]..     
-00024460: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-00024470: 6e65 2e64 735f 6d65 7468 6f64 203d 3d20  ne.ds_method == 
-00024480: 2773 7562 7361 6d70 6c65 273a 0a20 2020  'subsample':.   
-00024490: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-000244a0: 6573 203d 2074 696d 6573 5b3a 3a64 735d  es = times[::ds]
-000244b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000244c0: 2064 6174 6120 3d20 6461 7461 5b3a 2c20   data = data[:, 
-000244d0: 3a3a 6473 5d0a 0a20 2020 2020 2020 2020  ::ds]..         
-000244e0: 2020 2065 6c69 6620 7365 6c66 2e6d 6e65     elif self.mne
-000244f0: 2e64 735f 6d65 7468 6f64 203d 3d20 276d  .ds_method == 'm
-00024500: 6561 6e27 3a0a 2020 2020 2020 2020 2020  ean':.          
-00024510: 2020 2020 2020 6e20 3d20 6c65 6e28 7469        n = len(ti
-00024520: 6d65 7329 202f 2f20 6473 0a20 2020 2020  mes) // ds.     
-00024530: 2020 2020 2020 2020 2020 2023 2073 7461             # sta
-00024540: 7274 206f 6620 782d 7661 6c75 6573 0a20  rt of x-values. 
-00024550: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00024560: 2074 7279 2074 6f20 7365 6c65 6374 2061   try to select a
-00024570: 2073 6f6d 6577 6861 7420 6365 6e74 6572   somewhat center
-00024580: 6564 2070 6f69 6e74 0a20 2020 2020 2020  ed point.       
-00024590: 2020 2020 2020 2020 2073 7478 203d 2064           stx = d
-000245a0: 7320 2f2f 2032 0a20 2020 2020 2020 2020  s // 2.         
-000245b0: 2020 2020 2020 2074 696d 6573 203d 2074         times = t
-000245c0: 696d 6573 5b73 7478 3a73 7478 202b 206e  imes[stx:stx + n
-000245d0: 202a 2064 733a 6473 5d0a 2020 2020 2020   * ds:ds].      
-000245e0: 2020 2020 2020 2020 2020 7273 5f64 6174            rs_dat
-000245f0: 6120 3d20 6461 7461 5b3a 2c20 3a6e 202a  a = data[:, :n *
-00024600: 2064 735d 2e72 6573 6861 7065 286e 5f63   ds].reshape(n_c
-00024610: 682c 206e 2c20 6473 290a 2020 2020 2020  h, n, ds).      
-00024620: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00024630: 2072 735f 6461 7461 2e6d 6561 6e28 6178   rs_data.mean(ax
-00024640: 6973 3d32 290a 0a20 2020 2020 2020 2020  is=2)..         
-00024650: 2020 2065 6c69 6620 7365 6c66 2e6d 6e65     elif self.mne
-00024660: 2e64 735f 6d65 7468 6f64 203d 3d20 2770  .ds_method == 'p
-00024670: 6561 6b27 3a0a 2020 2020 2020 2020 2020  eak':.          
-00024680: 2020 2020 2020 6e20 3d20 6c65 6e28 7469        n = len(ti
-00024690: 6d65 7329 202f 2f20 6473 0a20 2020 2020  mes) // ds.     
-000246a0: 2020 2020 2020 2020 2020 2023 2073 7461             # sta
-000246b0: 7274 206f 6620 782d 7661 6c75 6573 0a20  rt of x-values. 
-000246c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000246d0: 2074 7279 2074 6f20 7365 6c65 6374 2061   try to select a
-000246e0: 2073 6f6d 6577 6861 7420 6365 6e74 6572   somewhat center
-000246f0: 6564 2070 6f69 6e74 0a20 2020 2020 2020  ed point.       
-00024700: 2020 2020 2020 2020 2073 7478 203d 2064           stx = d
-00024710: 7320 2f2f 2032 0a0a 2020 2020 2020 2020  s // 2..        
-00024720: 2020 2020 2020 2020 7831 203d 206e 702e          x1 = np.
-00024730: 656d 7074 7928 286e 2c20 3229 290a 2020  empty((n, 2)).  
-00024740: 2020 2020 2020 2020 2020 2020 2020 7831                x1
-00024750: 5b3a 5d20 3d20 7469 6d65 735b 7374 783a  [:] = times[stx:
-00024760: 7374 7820 2b20 6e20 2a20 6473 3a64 732c  stx + n * ds:ds,
-00024770: 206e 702e 6e65 7761 7869 735d 0a20 2020   np.newaxis].   
-00024780: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-00024790: 6573 203d 2078 312e 7265 7368 6170 6528  es = x1.reshape(
-000247a0: 6e20 2a20 3229 0a0a 2020 2020 2020 2020  n * 2)..        
-000247b0: 2020 2020 2020 2020 7931 203d 206e 702e          y1 = np.
-000247c0: 656d 7074 7928 286e 5f63 682c 206e 2c20  empty((n_ch, n, 
-000247d0: 3229 290a 2020 2020 2020 2020 2020 2020  2)).            
-000247e0: 2020 2020 7932 203d 2064 6174 615b 3a2c      y2 = data[:,
-000247f0: 203a 6e20 2a20 6473 5d2e 7265 7368 6170   :n * ds].reshap
-00024800: 6528 286e 5f63 682c 206e 2c20 6473 2929  e((n_ch, n, ds))
-00024810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024820: 2079 315b 3a2c 203a 2c20 305d 203d 2079   y1[:, :, 0] = y
-00024830: 322e 6d61 7828 6178 6973 3d32 290a 2020  2.max(axis=2).  
-00024840: 2020 2020 2020 2020 2020 2020 2020 7931                y1
-00024850: 5b3a 2c20 3a2c 2031 5d20 3d20 7932 2e6d  [:, :, 1] = y2.m
-00024860: 696e 2861 7869 733d 3229 0a20 2020 2020  in(axis=2).     
-00024870: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-00024880: 3d20 7931 2e72 6573 6861 7065 2828 6e5f  = y1.reshape((n_
-00024890: 6368 2c20 6e20 2a20 3229 290a 0a20 2020  ch, n * 2))..   
-000248a0: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
-000248b0: 652e 7469 6d65 732c 2073 656c 662e 6d6e  e.times, self.mn
-000248c0: 652e 6461 7461 203d 2074 696d 6573 2c20  e.data = times, 
-000248d0: 6461 7461 0a0a 2020 2020 6465 6620 5f73  data..    def _s
-000248e0: 686f 775f 7072 6f63 6573 7328 7365 6c66  how_process(self
-000248f0: 2c20 6d65 7373 6167 6529 3a0a 2020 2020  , message):.    
-00024900: 2020 2020 6966 2073 656c 662e 6d6e 652e      if self.mne.
-00024910: 6c6f 6164 5f70 726f 6772 6573 7362 6172  load_progressbar
-00024920: 2e69 7356 6973 6962 6c65 2829 3a0a 2020  .isVisible():.  
-00024930: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00024940: 6e65 2e6c 6f61 645f 7072 6f67 7265 7373  ne.load_progress
-00024950: 6261 722e 6869 6465 2829 0a20 2020 2020  bar.hide().     
-00024960: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-00024970: 6c6f 6164 5f70 726f 675f 6c61 6265 6c2e  load_prog_label.
-00024980: 6869 6465 2829 0a20 2020 2020 2020 2073  hide().        s
-00024990: 656c 662e 7374 6174 7573 4261 7228 292e  elf.statusBar().
-000249a0: 7368 6f77 4d65 7373 6167 6528 6d65 7373  showMessage(mess
-000249b0: 6167 6529 0a0a 2020 2020 6465 6620 5f70  age)..    def _p
-000249c0: 7265 636f 6d70 7574 655f 6669 6e69 7368  recompute_finish
-000249d0: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
-000249e0: 2020 7365 6c66 2e73 7461 7475 7342 6172    self.statusBar
-000249f0: 2829 2e73 686f 774d 6573 7361 6765 2827  ().showMessage('
-00024a00: 4c6f 6164 696e 6720 4669 6e69 7368 6564  Loading Finished
-00024a10: 272c 2035 290a 2020 2020 2020 2020 7365  ', 5).        se
-00024a20: 6c66 2e6d 6e65 2e64 6174 615f 7072 6563  lf.mne.data_prec
-00024a30: 6f6d 7075 7465 6420 3d20 5472 7565 0a0a  omputed = True..
-00024a40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00024a50: 6d6e 652e 6f76 6572 7669 6577 5f6d 6f64  mne.overview_mod
-00024a60: 6520 3d3d 2027 7a73 636f 7265 273a 0a20  e == 'zscore':. 
-00024a70: 2020 2020 2020 2020 2020 2023 2053 686f             # Sho
-00024a80: 7720 6c6f 6164 6564 206f 7665 7276 6965  w loaded overvie
-00024a90: 7720 696d 6167 650a 2020 2020 2020 2020  w image.        
-00024aa0: 2020 2020 7365 6c66 2e6d 6e65 2e6f 7665      self.mne.ove
-00024ab0: 7276 6965 775f 6261 722e 7365 745f 6261  rview_bar.set_ba
-00024ac0: 636b 6772 6f75 6e64 2829 0a0a 2020 2020  ckground()..    
-00024ad0: 2020 2020 6966 2073 656c 662e 5f72 6572      if self._rer
-00024ae0: 756e 5f6c 6f61 645f 7468 7265 6164 3a0a  un_load_thread:.
-00024af0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00024b00: 2e5f 7265 7275 6e5f 6c6f 6164 5f74 6872  ._rerun_load_thr
-00024b10: 6561 6420 3d20 4661 6c73 650a 2020 2020  ead = False.    
-00024b20: 2020 2020 2020 2020 7365 6c66 2e5f 696e          self._in
-00024b30: 6974 5f70 7265 636f 6d70 7574 6528 290a  it_precompute().
-00024b40: 0a20 2020 2064 6566 205f 696e 6974 5f70  .    def _init_p
-00024b50: 7265 636f 6d70 7574 6528 7365 6c66 293a  recompute(self):
-00024b60: 0a20 2020 2020 2020 2023 2052 656d 6f76  .        # Remov
-00024b70: 6520 7072 6576 696f 7573 6c79 206c 6f61  e previously loa
-00024b80: 6465 6420 6461 7461 0a20 2020 2020 2020  ded data.       
-00024b90: 2073 656c 662e 6d6e 652e 6461 7461 5f70   self.mne.data_p
-00024ba0: 7265 636f 6d70 7574 6564 203d 2046 616c  recomputed = Fal
-00024bb0: 7365 0a20 2020 2020 2020 2069 6620 616c  se.        if al
-00024bc0: 6c28 5b68 6173 6174 7472 2873 656c 662e  l([hasattr(self.
-00024bd0: 6d6e 652c 2073 7429 0a20 2020 2020 2020  mne, st).       
-00024be0: 2020 2020 2020 2020 2066 6f72 2073 7420           for st 
-00024bf0: 696e 205b 2767 6c6f 6261 6c5f 6461 7461  in ['global_data
-00024c00: 272c 2027 676c 6f62 616c 5f74 696d 6573  ', 'global_times
-00024c10: 275d 5d29 3a0a 2020 2020 2020 2020 2020  ']]):.          
-00024c20: 2020 6465 6c20 7365 6c66 2e6d 6e65 2e67    del self.mne.g
-00024c30: 6c6f 6261 6c5f 6461 7461 2c20 7365 6c66  lobal_data, self
-00024c40: 2e6d 6e65 2e67 6c6f 6261 6c5f 7469 6d65  .mne.global_time
-00024c50: 730a 2020 2020 2020 2020 6763 2e63 6f6c  s.        gc.col
-00024c60: 6c65 6374 2829 0a0a 2020 2020 2020 2020  lect()..        
-00024c70: 6966 2073 656c 662e 6d6e 652e 7072 6563  if self.mne.prec
-00024c80: 6f6d 7075 7465 203d 3d20 2761 7574 6f27  ompute == 'auto'
-00024c90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00024ca0: 6c66 2e6d 6e65 2e65 6e61 626c 655f 7072  lf.mne.enable_pr
-00024cb0: 6563 6f6d 7075 7465 203d 2073 656c 662e  ecompute = self.
-00024cc0: 5f63 6865 636b 5f73 7061 6365 5f66 6f72  _check_space_for
-00024cd0: 5f70 7265 636f 6d70 7574 6528 290a 2020  _precompute().  
-00024ce0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-00024cf0: 7461 6e63 6528 7365 6c66 2e6d 6e65 2e70  tance(self.mne.p
-00024d00: 7265 636f 6d70 7574 652c 2062 6f6f 6c29  recompute, bool)
-00024d10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00024d20: 6c66 2e6d 6e65 2e65 6e61 626c 655f 7072  lf.mne.enable_pr
-00024d30: 6563 6f6d 7075 7465 203d 2073 656c 662e  ecompute = self.
-00024d40: 6d6e 652e 7072 6563 6f6d 7075 7465 0a0a  mne.precompute..
-00024d50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00024d60: 6d6e 652e 656e 6162 6c65 5f70 7265 636f  mne.enable_preco
-00024d70: 6d70 7574 653a 0a20 2020 2020 2020 2020  mpute:.         
-00024d80: 2020 2023 2053 7461 7274 2070 7265 636f     # Start preco
-00024d90: 6d70 7574 6520 7468 7265 6164 0a20 2020  mpute thread.   
-00024da0: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
-00024db0: 652e 6c6f 6164 5f70 726f 6772 6573 7362  e.load_progressb
-00024dc0: 6172 2e73 686f 7728 290a 2020 2020 2020  ar.show().      
-00024dd0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e6c        self.mne.l
-00024de0: 6f61 645f 7072 6f67 5f6c 6162 656c 2e73  oad_prog_label.s
-00024df0: 686f 7728 290a 2020 2020 2020 2020 2020  how().          
-00024e00: 2020 7365 6c66 2e6c 6f61 645f 7468 7265    self.load_thre
-00024e10: 6164 2e73 7461 7274 2829 0a0a 2020 2020  ad.start()..    
-00024e20: 6465 6620 5f72 6572 756e 5f70 7265 636f  def _rerun_preco
-00024e30: 6d70 7574 6528 7365 6c66 293a 0a20 2020  mpute(self):.   
-00024e40: 2020 2020 2069 6620 7365 6c66 2e6c 6f61       if self.loa
-00024e50: 645f 7468 7265 6164 2e69 7352 756e 6e69  d_thread.isRunni
-00024e60: 6e67 2829 3a0a 2020 2020 2020 2020 2020  ng():.          
-00024e70: 2020 7365 6c66 2e5f 7265 7275 6e5f 6c6f    self._rerun_lo
-00024e80: 6164 5f74 6872 6561 6420 3d20 5472 7565  ad_thread = True
-00024e90: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00024ea0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00024eb0: 5f69 6e69 745f 7072 6563 6f6d 7075 7465  _init_precompute
-00024ec0: 2829 0a0a 2020 2020 6465 6620 5f63 6865  ()..    def _che
-00024ed0: 636b 5f73 7061 6365 5f66 6f72 5f70 7265  ck_space_for_pre
-00024ee0: 636f 6d70 7574 6528 7365 6c66 293a 0a20  compute(self):. 
-00024ef0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00024f00: 2020 2020 2020 2020 696d 706f 7274 2070          import p
-00024f10: 7375 7469 6c0a 2020 2020 2020 2020 6578  sutil.        ex
-00024f20: 6365 7074 2049 6d70 6f72 7445 7272 6f72  cept ImportError
-00024f30: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-00024f40: 6767 6572 2e69 6e66 6f28 2746 7265 6520  gger.info('Free 
-00024f50: 5241 4d20 7370 6163 6520 636f 756c 6420  RAM space could 
-00024f60: 6e6f 7420 6265 2064 6574 6572 6d69 6e65  not be determine
-00024f70: 6420 6265 6361 7573 6527 0a20 2020 2020  d because'.     
-00024f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024f90: 2020 2027 2270 7375 7469 6c22 2069 7320     '"psutil" is 
-00024fa0: 6e6f 7420 696e 7374 616c 6c65 642e 2027  not installed. '
-00024fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024fc0: 2020 2020 2020 2020 2027 5365 7474 696e           'Settin
-00024fd0: 6720 7072 6563 6f6d 7075 7465 2074 6f20  g precompute to 
-00024fe0: 4661 6c73 652e 2729 0a20 2020 2020 2020  False.').       
-00024ff0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00025000: 650a 2020 2020 2020 2020 656c 7365 3a0a  e.        else:.
-00025010: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00025020: 656c 662e 6d6e 652e 6973 5f65 706f 6368  elf.mne.is_epoch
-00025030: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00025040: 2020 2066 696c 6573 203d 205b 7365 6c66     files = [self
-00025050: 2e6d 6e65 2e69 6e73 742e 6669 6c65 6e61  .mne.inst.filena
-00025060: 6d65 5d0a 2020 2020 2020 2020 2020 2020  me].            
-00025070: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00025080: 2020 2020 2020 6669 6c65 7320 3d20 7365        files = se
-00025090: 6c66 2e6d 6e65 2e69 6e73 742e 6669 6c65  lf.mne.inst.file
-000250a0: 6e61 6d65 730a 2020 2020 2020 2020 2020  names.          
-000250b0: 2020 6966 2066 696c 6573 5b30 5d20 6973    if files[0] is
-000250c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000250d0: 2020 2020 2020 2020 2020 2023 2047 6574             # Get
-000250e0: 2064 6973 6b2d 7370 6163 6520 6f66 2072   disk-space of r
-000250f0: 6177 2d66 696c 6528 7329 0a20 2020 2020  aw-file(s).     
-00025100: 2020 2020 2020 2020 2020 2064 6973 6b5f             disk_
-00025110: 7370 6163 6520 3d20 300a 2020 2020 2020  space = 0.      
-00025120: 2020 2020 2020 2020 2020 666f 7220 666e            for fn
-00025130: 2069 6e20 6669 6c65 733a 0a20 2020 2020   in files:.     
-00025140: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00025150: 6973 6b5f 7370 6163 6520 2b3d 2067 6574  isk_space += get
-00025160: 7369 7a65 2866 6e29 0a0a 2020 2020 2020  size(fn)..      
-00025170: 2020 2020 2020 2020 2020 2320 4465 7465            # Dete
-00025180: 726d 696e 6520 6578 7065 6374 6564 2052  rmine expected R
-00025190: 414d 2073 7061 6365 2062 6173 6564 206f  AM space based o
-000251a0: 6e20 6f72 6967 5f66 6f72 6d61 740a 2020  n orig_format.  
-000251b0: 2020 2020 2020 2020 2020 2020 2020 666d                fm
-000251c0: 745f 6d75 6c74 6970 6c69 6572 7320 3d20  t_multipliers = 
-000251d0: 7b27 646f 7562 6c65 273a 2031 2c0a 2020  {'double': 1,.  
-000251e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000251f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025200: 2027 7369 6e67 6c65 273a 2032 2c0a 2020   'single': 2,.  
-00025210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025230: 2027 696e 7427 3a20 322c 0a20 2020 2020   'int': 2,.     
-00025240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025250: 2020 2020 2020 2020 2020 2020 2020 2773                's
-00025260: 686f 7274 273a 2034 7d0a 0a20 2020 2020  hort': 4}..     
-00025270: 2020 2020 2020 2020 2020 2023 2045 706f             # Epo
-00025280: 6368 7320 616e 6420 4943 4120 646f 6e27  chs and ICA don'
-00025290: 7420 6861 7665 2074 6869 7320 6174 7472  t have this attr
-000252a0: 6962 7574 652c 2061 7373 756d 6520 7369  ibute, assume si
-000252b0: 6e67 6c65 0a20 2020 2020 2020 2020 2020  ngle.           
-000252c0: 2020 2020 2023 206f 6e20 6469 736b 0a20       # on disk. 
-000252d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000252e0: 6d74 203d 2067 6574 6174 7472 2873 656c  mt = getattr(sel
-000252f0: 662e 6d6e 652e 696e 7374 2c20 276f 7269  f.mne.inst, 'ori
-00025300: 675f 666f 726d 6174 272c 2027 7369 6e67  g_format', 'sing
-00025310: 6c65 2729 0a20 2020 2020 2020 2020 2020  le').           
-00025320: 2020 2020 2023 2041 7070 6c79 2073 697a       # Apply siz
-00025330: 6520 6368 616e 6765 2074 6f20 3634 2d62  e change to 64-b
-00025340: 6974 2066 6c6f 6174 2069 6e20 6d65 6d6f  it float in memo
-00025350: 7279 0a20 2020 2020 2020 2020 2020 2020  ry.             
-00025360: 2020 2023 2028 2a20 3220 6265 6361 7573     # (* 2 becaus
-00025370: 6520 7768 656e 206c 6f61 6469 6e67 2064  e when loading d
-00025380: 6174 6120 7769 6c6c 2062 6520 6c6f 6164  ata will be load
-00025390: 6564 2069 6e74 6f20 6120 636f 7079 0a20  ed into a copy. 
-000253a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000253b0: 206f 6620 7365 6c66 2e6d 6e65 2e69 6e73   of self.mne.ins
-000253c0: 742e 5f64 6174 6120 746f 2061 7070 6c79  t._data to apply
-000253d0: 2070 726f 6365 7373 696e 672e 0a20 2020   processing..   
-000253e0: 2020 2020 2020 2020 2020 2020 2065 7870               exp
-000253f0: 6563 7465 645f 7261 6d20 3d20 6469 736b  ected_ram = disk
-00025400: 5f73 7061 6365 202a 2066 6d74 5f6d 756c  _space * fmt_mul
-00025410: 7469 706c 6965 7273 5b66 6d74 5d20 2a20  tipliers[fmt] * 
-00025420: 320a 2020 2020 2020 2020 2020 2020 656c  2.            el
-00025430: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00025440: 2020 2020 6578 7065 6374 6564 5f72 616d      expected_ram
-00025450: 203d 2073 7973 2e67 6574 7369 7a65 6f66   = sys.getsizeof
-00025460: 2873 656c 662e 6d6e 652e 696e 7374 2e5f  (self.mne.inst._
-00025470: 6461 7461 290a 0a20 2020 2020 2020 2020  data)..         
-00025480: 2020 2023 2047 6574 2061 7661 696c 6162     # Get availab
-00025490: 6c65 2052 414d 0a20 2020 2020 2020 2020  le RAM.         
-000254a0: 2020 2066 7265 655f 7261 6d20 3d20 7073     free_ram = ps
-000254b0: 7574 696c 2e76 6972 7475 616c 5f6d 656d  util.virtual_mem
-000254c0: 6f72 7928 292e 6672 6565 0a0a 2020 2020  ory().free..    
-000254d0: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-000254e0: 5f72 616d 5f73 7472 203d 2073 697a 656f  _ram_str = sizeo
-000254f0: 665f 666d 7428 6578 7065 6374 6564 5f72  f_fmt(expected_r
-00025500: 616d 290a 2020 2020 2020 2020 2020 2020  am).            
-00025510: 6672 6565 5f72 616d 5f73 7472 203d 2073  free_ram_str = s
-00025520: 697a 656f 665f 666d 7428 6672 6565 5f72  izeof_fmt(free_r
-00025530: 616d 290a 2020 2020 2020 2020 2020 2020  am).            
-00025540: 6c65 6674 5f72 616d 5f73 7472 203d 2073  left_ram_str = s
-00025550: 697a 656f 665f 666d 7428 6672 6565 5f72  izeof_fmt(free_r
-00025560: 616d 202d 2065 7870 6563 7465 645f 7261  am - expected_ra
-00025570: 6d29 0a0a 2020 2020 2020 2020 2020 2020  m)..            
-00025580: 6966 2065 7870 6563 7465 645f 7261 6d20  if expected_ram 
-00025590: 3c20 6672 6565 5f72 616d 3a0a 2020 2020  < free_ram:.    
-000255a0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-000255b0: 6572 2e64 6562 7567 2827 5468 6520 6461  er.debug('The da
-000255c0: 7461 2070 7265 636f 6d70 7574 6564 2066  ta precomputed f
-000255d0: 6f72 2076 6973 7561 6c69 7a61 7469 6f6e  or visualization
-000255e0: 2074 616b 6573 2027 0a20 2020 2020 2020   takes '.       
-000255f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025600: 2020 2020 2020 6627 7b65 7870 6563 7465        f'{expecte
-00025610: 645f 7261 6d5f 7374 727d 2077 6974 6820  d_ram_str} with 
-00025620: 7b6c 6566 745f 7261 6d5f 7374 727d 206f  {left_ram_str} o
-00025630: 6620 270a 2020 2020 2020 2020 2020 2020  f '.            
-00025640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025650: 2066 2752 414d 206c 6566 742e 2729 0a20   f'RAM left.'). 
-00025660: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00025670: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-00025680: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00025690: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-000256a0: 6765 722e 6465 6275 6728 6627 5468 6520  ger.debug(f'The 
-000256b0: 7072 6563 6f6d 7075 7465 6420 6461 7461  precomputed data
-000256c0: 2077 6974 6820 7b65 7870 6563 7465 645f   with {expected_
-000256d0: 7261 6d5f 7374 727d 2027 0a20 2020 2020  ram_str} '.     
-000256e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000256f0: 2020 2020 2020 2020 6627 7769 6c6c 2073          f'will s
-00025700: 7572 7061 7373 2079 6f75 7220 6375 7272  urpass your curr
-00025710: 656e 7420 7b66 7265 655f 7261 6d5f 7374  ent {free_ram_st
-00025720: 727d 2027 0a20 2020 2020 2020 2020 2020  r} '.           
-00025730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025740: 2020 6627 6f66 2066 7265 6520 5241 4d2e    f'of free RAM.
-00025750: 5c6e 270a 2020 2020 2020 2020 2020 2020  \n'.            
-00025760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025770: 2027 5468 7573 2070 7265 636f 6d70 7574   'Thus precomput
-00025780: 6520 7769 6c6c 2062 6520 7365 7420 746f  e will be set to
-00025790: 2046 616c 7365 2e5c 6e27 0a20 2020 2020   False.\n'.     
-000257a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257b0: 2020 2020 2020 2020 2728 4966 2079 6f75          '(If you
-000257c0: 2077 616e 7420 746f 2070 7265 636f 6d70   want to precomp
-000257d0: 7574 6520 6e65 7665 7274 6865 6c65 7373  ute nevertheless
-000257e0: 2c20 270a 2020 2020 2020 2020 2020 2020  , '.            
-000257f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025800: 2027 7468 656e 2073 6574 2070 7265 636f   'then set preco
-00025810: 6d70 7574 6520 746f 2054 7275 6520 696e  mpute to True in
-00025820: 7374 6561 6420 6f66 2022 6175 746f 2229  stead of "auto")
-00025830: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00025840: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00025850: 0a20 2020 2064 6566 205f 7072 6f63 6573  .    def _proces
-00025860: 735f 6461 7461 2873 656c 662c 2064 6174  s_data(self, dat
-00025870: 612c 2073 7461 7274 2c20 7374 6f70 2c20  a, start, stop, 
-00025880: 7069 636b 732c 0a20 2020 2020 2020 2020  picks,.         
-00025890: 2020 2020 2020 2020 2020 2020 2073 6967               sig
-000258a0: 6e61 6c73 3d4e 6f6e 6529 3a0a 2020 2020  nals=None):.    
-000258b0: 2020 2020 6461 7461 203d 2073 7570 6572      data = super
-000258c0: 2829 2e5f 7072 6f63 6573 735f 6461 7461  ()._process_data
-000258d0: 2864 6174 612c 2073 7461 7274 2c20 7374  (data, start, st
-000258e0: 6f70 2c20 7069 636b 732c 2073 6967 6e61  op, picks, signa
-000258f0: 6c73 290a 0a20 2020 2020 2020 2023 2049  ls)..        # I
-00025900: 6e76 6572 7420 4461 7461 2074 6f20 6265  nvert Data to be
-00025910: 2064 6973 706c 6179 6564 2066 726f 6d20   displayed from 
-00025920: 746f 7020 6f6e 2069 6e76 6572 7465 6420  top on inverted 
-00025930: 592d 4178 6973 0a20 2020 2020 2020 2064  Y-Axis.        d
-00025940: 6174 6120 2a3d 202d 310a 0a20 2020 2020  ata *= -1..     
-00025950: 2020 2072 6574 7572 6e20 6461 7461 0a0a     return data..
-00025960: 2020 2020 6465 6620 5f75 7064 6174 655f      def _update_
-00025970: 6461 7461 2873 656c 6629 3a0a 2020 2020  data(self):.    
-00025980: 2020 2020 6966 2073 656c 662e 6d6e 652e      if self.mne.
-00025990: 6461 7461 5f70 7265 636f 6d70 7574 6564  data_precomputed
-000259a0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-000259b0: 6765 7420 7374 6172 742f 7374 6f70 2d73  get start/stop-s
-000259c0: 616d 706c 6573 0a20 2020 2020 2020 2020  amples.         
-000259d0: 2020 2073 7461 7274 2c20 7374 6f70 203d     start, stop =
-000259e0: 2073 656c 662e 5f67 6574 5f73 7461 7274   self._get_start
-000259f0: 5f73 746f 7028 290a 2020 2020 2020 2020  _stop().        
-00025a00: 2020 2020 7365 6c66 2e6d 6e65 2e74 696d      self.mne.tim
-00025a10: 6573 203d 2073 656c 662e 6d6e 652e 676c  es = self.mne.gl
-00025a20: 6f62 616c 5f74 696d 6573 5b73 7461 7274  obal_times[start
-00025a30: 3a73 746f 705d 0a20 2020 2020 2020 2020  :stop].         
-00025a40: 2020 2073 656c 662e 6d6e 652e 6461 7461     self.mne.data
-00025a50: 203d 2073 656c 662e 6d6e 652e 676c 6f62   = self.mne.glob
-00025a60: 616c 5f64 6174 615b 3a2c 2073 7461 7274  al_data[:, start
-00025a70: 3a73 746f 705d 0a0a 2020 2020 2020 2020  :stop]..        
-00025a80: 2020 2020 2320 7265 6d6f 7665 2044 4320      # remove DC 
-00025a90: 6c6f 6361 6c6c 790a 2020 2020 2020 2020  locally.        
-00025aa0: 2020 2020 6966 2073 656c 662e 6d6e 652e      if self.mne.
-00025ab0: 7265 6d6f 7665 5f64 633a 0a20 2020 2020  remove_dc:.     
-00025ac0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00025ad0: 6d6e 652e 6461 7461 203d 2073 656c 662e  mne.data = self.
-00025ae0: 6d6e 652e 6461 7461 202d 205c 0a20 2020  mne.data - \.   
-00025af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00025b10: 662e 6d6e 652e 6461 7461 2e6d 6561 6e28  f.mne.data.mean(
-00025b20: 6178 6973 3d31 2c20 6b65 6570 6469 6d73  axis=1, keepdims
-00025b30: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
-00025b40: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00025b50: 2020 2320 5768 696c 6520 6461 7461 2069    # While data i
-00025b60: 7320 6e6f 7420 7072 6563 6f6d 7075 7465  s not precompute
-00025b70: 6420 6765 7420 6461 7461 206f 6e6c 7920  d get data only 
-00025b80: 6672 6f6d 2073 686f 776e 2072 616e 6765  from shown range
-00025b90: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-00025ba0: 2023 2070 726f 6365 7373 206f 6e6c 7920   # process only 
-00025bb0: 7468 6f73 652e 0a20 2020 2020 2020 2020  those..         
-00025bc0: 2020 2073 7570 6572 2829 2e5f 7570 6461     super()._upda
-00025bd0: 7465 5f64 6174 6128 290a 0a20 2020 2020  te_data()..     
-00025be0: 2020 2023 2049 6e69 7469 616c 697a 6520     # Initialize 
-00025bf0: 6465 6369 6d0a 2020 2020 2020 2020 7365  decim.        se
-00025c00: 6c66 2e6d 6e65 2e64 6563 696d 5f64 6174  lf.mne.decim_dat
-00025c10: 6120 3d20 6e70 2e6f 6e65 735f 6c69 6b65  a = np.ones_like
-00025c20: 2873 656c 662e 6d6e 652e 7069 636b 7329  (self.mne.picks)
-00025c30: 0a20 2020 2020 2020 2064 6174 615f 7069  .        data_pi
-00025c40: 636b 735f 6d61 736b 203d 206e 702e 696e  cks_mask = np.in
-00025c50: 3164 2873 656c 662e 6d6e 652e 7069 636b  1d(self.mne.pick
-00025c60: 732c 2073 656c 662e 6d6e 652e 7069 636b  s, self.mne.pick
-00025c70: 735f 6461 7461 290a 2020 2020 2020 2020  s_data).        
-00025c80: 7365 6c66 2e6d 6e65 2e64 6563 696d 5f64  self.mne.decim_d
-00025c90: 6174 615b 6461 7461 5f70 6963 6b73 5f6d  ata[data_picks_m
-00025ca0: 6173 6b5d 203d 2073 656c 662e 6d6e 652e  ask] = self.mne.
-00025cb0: 6465 6369 6d0a 0a20 2020 2020 2020 2023  decim..        #
-00025cc0: 2041 7070 6c79 2063 6c69 7070 696e 670a   Apply clipping.
-00025cd0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00025ce0: 6d6e 652e 636c 6970 7069 6e67 203d 3d20  mne.clipping == 
-00025cf0: 2763 6c61 6d70 273a 0a20 2020 2020 2020  'clamp':.       
-00025d00: 2020 2020 2073 656c 662e 6d6e 652e 6461       self.mne.da
-00025d10: 7461 203d 206e 702e 636c 6970 2873 656c  ta = np.clip(sel
-00025d20: 662e 6d6e 652e 6461 7461 2c20 2d30 2e35  f.mne.data, -0.5
-00025d30: 2c20 302e 3529 0a20 2020 2020 2020 2065  , 0.5).        e
-00025d40: 6c69 6620 7365 6c66 2e6d 6e65 2e63 6c69  lif self.mne.cli
-00025d50: 7070 696e 6720 6973 206e 6f74 204e 6f6e  pping is not Non
-00025d60: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00025d70: 656c 662e 6d6e 652e 6461 7461 203d 2073  elf.mne.data = s
-00025d80: 656c 662e 6d6e 652e 6461 7461 2e63 6f70  elf.mne.data.cop
-00025d90: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-00025da0: 7365 6c66 2e6d 6e65 2e64 6174 615b 6162  self.mne.data[ab
-00025db0: 7328 7365 6c66 2e6d 6e65 2e64 6174 6120  s(self.mne.data 
-00025dc0: 2a20 7365 6c66 2e6d 6e65 2e73 6361 6c65  * self.mne.scale
-00025dd0: 5f66 6163 746f 7229 0a20 2020 2020 2020  _factor).       
-00025de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025df0: 2020 203e 2073 656c 662e 6d6e 652e 636c     > self.mne.cl
-00025e00: 6970 7069 6e67 5d20 3d20 6e70 2e6e 616e  ipping] = np.nan
-00025e10: 0a0a 2020 2020 2020 2020 2320 4170 706c  ..        # Appl
-00025e20: 7920 446f 776e 7361 6d70 6c69 6e67 2028  y Downsampling (
-00025e30: 6966 2065 6e61 626c 6564 290a 2020 2020  if enabled).    
-00025e40: 2020 2020 7365 6c66 2e5f 6170 706c 795f      self._apply_
-00025e50: 646f 776e 7361 6d70 6c69 6e67 2829 0a0a  downsampling()..
-00025e60: 2020 2020 6465 6620 5f67 6574 5f7a 7363      def _get_zsc
-00025e70: 6f72 6528 7365 6c66 2c20 6461 7461 293a  ore(self, data):
-00025e80: 0a20 2020 2020 2020 2023 2052 6573 6861  .        # Resha
-00025e90: 7065 2064 6174 6120 746f 2072 6561 736f  pe data to reaso
-00025ea0: 6e61 626c 6520 7369 7a65 2066 6f72 2064  nable size for d
-00025eb0: 6973 706c 6179 0a20 2020 2020 2020 2073  isplay.        s
-00025ec0: 6372 6565 6e5f 6765 6f6d 6574 7279 203d  creen_geometry =
-00025ed0: 205f 7363 7265 656e 5f67 656f 6d65 7472   _screen_geometr
-00025ee0: 7928 7365 6c66 290a 2020 2020 2020 2020  y(self).        
-00025ef0: 6966 2073 6372 6565 6e5f 6765 6f6d 6574  if screen_geomet
-00025f00: 7279 2069 7320 4e6f 6e65 3a0a 2020 2020  ry is None:.    
-00025f10: 2020 2020 2020 2020 6d61 785f 7069 7865          max_pixe
-00025f20: 6c5f 7769 6474 6820 3d20 3338 3430 2020  l_width = 3840  
-00025f30: 2320 6465 6661 756c 743d 5548 440a 2020  # default=UHD.  
-00025f40: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00025f50: 2020 2020 2020 2020 6d61 785f 7069 7865          max_pixe
-00025f60: 6c5f 7769 6474 6820 3d20 7363 7265 656e  l_width = screen
-00025f70: 5f67 656f 6d65 7472 792e 7769 6474 6828  _geometry.width(
-00025f80: 290a 2020 2020 2020 2020 636f 6c6c 6170  ).        collap
-00025f90: 7365 5f62 7920 3d20 6461 7461 2e73 6861  se_by = data.sha
-00025fa0: 7065 5b31 5d20 2f2f 206d 6178 5f70 6978  pe[1] // max_pix
-00025fb0: 656c 5f77 6964 7468 0a20 2020 2020 2020  el_width.       
-00025fc0: 2064 6174 6120 3d20 6461 7461 5b3a 2c20   data = data[:, 
-00025fd0: 3a6d 6178 5f70 6978 656c 5f77 6964 7468  :max_pixel_width
-00025fe0: 202a 2063 6f6c 6c61 7073 655f 6279 5d0a   * collapse_by].
-00025ff0: 2020 2020 2020 2020 6966 2063 6f6c 6c61          if colla
-00026000: 7073 655f 6279 203e 2030 3a0a 2020 2020  pse_by > 0:.    
-00026010: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00026020: 6174 612e 7265 7368 6170 6528 6461 7461  ata.reshape(data
-00026030: 2e73 6861 7065 5b30 5d2c 206d 6178 5f70  .shape[0], max_p
-00026040: 6978 656c 5f77 6964 7468 2c20 636f 6c6c  ixel_width, coll
-00026050: 6170 7365 5f62 7929 0a20 2020 2020 2020  apse_by).       
-00026060: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-00026070: 2e6d 6561 6e28 6178 6973 3d32 290a 2020  .mean(axis=2).  
-00026080: 2020 2020 2020 7a20 3d20 7a73 636f 7265        z = zscore
-00026090: 2864 6174 612c 2061 7869 733d 3129 0a20  (data, axis=1). 
-000260a0: 2020 2020 2020 2069 6620 7a2e 7369 7a65         if z.size
-000260b0: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
-000260c0: 2020 7a6d 696e 203d 206e 702e 6d69 6e28    zmin = np.min(
-000260d0: 7a2c 2061 7869 733d 3129 0a20 2020 2020  z, axis=1).     
-000260e0: 2020 2020 2020 207a 6d61 7820 3d20 6e70         zmax = np
-000260f0: 2e6d 6178 287a 2c20 6178 6973 3d31 290a  .max(z, axis=1).
-00026100: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
-00026110: 6f6e 7665 7274 2069 6e74 6f20 5247 4241  onvert into RGBA
-00026120: 0a20 2020 2020 2020 2020 2020 207a 7267  .            zrg
-00026130: 6261 203d 206e 702e 656d 7074 7928 282a  ba = np.empty((*
-00026140: 7a2e 7368 6170 652c 2034 2929 0a20 2020  z.shape, 4)).   
-00026150: 2020 2020 2020 2020 2066 6f72 2072 6f77           for row
-00026160: 5f69 6478 2c20 726f 7720 696e 2065 6e75  _idx, row in enu
-00026170: 6d65 7261 7465 287a 293a 0a20 2020 2020  merate(z):.     
-00026180: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-00026190: 6f6c 5f69 6478 2c20 7661 6c75 6520 696e  ol_idx, value in
-000261a0: 2065 6e75 6d65 7261 7465 2872 6f77 293a   enumerate(row):
-000261b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000261c0: 2020 2020 2069 6620 6d61 7468 2e69 736e       if math.isn
-000261d0: 616e 2876 616c 7565 293a 0a20 2020 2020  an(value):.     
-000261e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000261f0: 2020 2076 616c 7565 203d 2030 0a20 2020     value = 0.   
-00026200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026210: 2069 6620 7661 6c75 6520 3d3d 2030 3a0a   if value == 0:.
-00026220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026230: 2020 2020 2020 2020 7267 6261 203d 205b          rgba = [
-00026240: 302c 2030 2c20 302c 2030 5d0a 2020 2020  0, 0, 0, 0].    
-00026250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026260: 656c 6966 2076 616c 7565 203c 2030 3a0a  elif value < 0:.
-00026270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026280: 2020 2020 2020 2020 616c 7068 6120 3d20          alpha = 
-00026290: 696e 7428 3235 3520 2a20 7661 6c75 6520  int(255 * value 
-000262a0: 2f20 6162 7328 7a6d 696e 5b72 6f77 5f69  / abs(zmin[row_i
-000262b0: 6478 5d29 290a 2020 2020 2020 2020 2020  dx])).          
-000262c0: 2020 2020 2020 2020 2020 2020 2020 7267                rg
-000262d0: 6261 203d 205b 302c 2030 2c20 3235 352c  ba = [0, 0, 255,
-000262e0: 2061 6c70 6861 5d0a 2020 2020 2020 2020   alpha].        
-000262f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00026300: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00026310: 2020 2020 2020 2020 2020 616c 7068 6120            alpha 
-00026320: 3d20 696e 7428 3235 3520 2a20 7661 6c75  = int(255 * valu
-00026330: 6520 2f20 7a6d 6178 5b72 6f77 5f69 6478  e / zmax[row_idx
-00026340: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00026350: 2020 2020 2020 2020 2020 2072 6762 6120             rgba 
-00026360: 3d20 5b32 3535 2c20 302c 2030 2c20 616c  = [255, 0, 0, al
-00026370: 7068 615d 0a0a 2020 2020 2020 2020 2020  pha]..          
-00026380: 2020 2020 2020 2020 2020 7a72 6762 615b            zrgba[
-00026390: 726f 775f 6964 782c 2063 6f6c 5f69 6478  row_idx, col_idx
-000263a0: 5d20 3d20 7267 6261 0a0a 2020 2020 2020  ] = rgba..      
-000263b0: 2020 2020 2020 7a72 6762 6120 3d20 6e70        zrgba = np
-000263c0: 2e72 6571 7569 7265 287a 7267 6261 2c20  .require(zrgba, 
-000263d0: 6e70 2e75 696e 7438 2c20 2743 2729 0a0a  np.uint8, 'C')..
-000263e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000263f0: 2e6d 6e65 2e7a 7363 6f72 655f 7267 6261  .mne.zscore_rgba
-00026400: 203d 207a 7267 6261 0a0a 2020 2020 2320   = zrgba..    # 
-00026410: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
-00026420: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
-00026430: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
-00026440: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
-00026450: 2320 2320 2320 2320 230a 2020 2020 2320  # # # # #.    # 
-00026460: 414e 4e4f 5441 5449 4f4e 530a 2020 2020  ANNOTATIONS.    
-00026470: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
-00026480: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
-00026490: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
-000264a0: 2320 2320 2320 2320 2320 2320 2320 2320  # # # # # # # # 
-000264b0: 2320 2320 2320 2320 2320 230a 2020 2020  # # # # # #.    
-000264c0: 6465 6620 5f61 6464 5f72 6567 696f 6e28  def _add_region(
-000264d0: 7365 6c66 2c20 706c 6f74 5f6f 6e73 6574  self, plot_onset
-000264e0: 2c20 6475 7261 7469 6f6e 2c20 6465 7363  , duration, desc
-000264f0: 7269 7074 696f 6e2c 202a 2c20 7265 6769  ription, *, regi
-00026500: 6f6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  on=None):.      
-00026510: 2020 6966 206e 6f74 2072 6567 696f 6e3a    if not region:
-00026520: 0a20 2020 2020 2020 2020 2020 2072 6567  .            reg
-00026530: 696f 6e20 3d20 416e 6e6f 7452 6567 696f  ion = AnnotRegio
-00026540: 6e28 7365 6c66 2e6d 6e65 2c20 6465 7363  n(self.mne, desc
-00026550: 7269 7074 696f 6e3d 6465 7363 7269 7074  ription=descript
-00026560: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00026570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026580: 2020 2020 2020 7661 6c75 6573 3d28 706c        values=(pl
-00026590: 6f74 5f6f 6e73 6574 2c20 706c 6f74 5f6f  ot_onset, plot_o
-000265a0: 6e73 6574 202b 2064 7572 6174 696f 6e29  nset + duration)
-000265b0: 290a 2020 2020 2020 2020 2320 4164 6420  ).        # Add 
-000265c0: 7265 6769 6f6e 2074 6f20 6c69 7374 2061  region to list a
-000265d0: 6e64 2070 6c6f 740a 2020 2020 2020 2020  nd plot.        
-000265e0: 7365 6c66 2e6d 6e65 2e72 6567 696f 6e73  self.mne.regions
-000265f0: 2e61 7070 656e 6428 7265 6769 6f6e 290a  .append(region).
-00026600: 0a20 2020 2020 2020 2023 2043 6f6e 6e65  .        # Conne
-00026610: 6374 2073 6967 6e61 6c73 206f 6620 7265  ct signals of re
-00026620: 6769 6f6e 0a20 2020 2020 2020 2072 6567  gion.        reg
-00026630: 696f 6e2e 7265 6769 6f6e 4368 616e 6765  ion.regionChange
-00026640: 4669 6e69 7368 6564 2e63 6f6e 6e65 6374  Finished.connect
-00026650: 2873 656c 662e 5f72 6567 696f 6e5f 6368  (self._region_ch
-00026660: 616e 6765 6429 0a20 2020 2020 2020 2072  anged).        r
-00026670: 6567 696f 6e2e 676f 7453 656c 6563 7465  egion.gotSelecte
-00026680: 642e 636f 6e6e 6563 7428 7365 6c66 2e5f  d.connect(self._
-00026690: 7265 6769 6f6e 5f73 656c 6563 7465 6429  region_selected)
-000266a0: 0a20 2020 2020 2020 2072 6567 696f 6e2e  .        region.
-000266b0: 7265 6d6f 7665 5265 7175 6573 7465 642e  removeRequested.
-000266c0: 636f 6e6e 6563 7428 7365 6c66 2e5f 7265  connect(self._re
-000266d0: 6d6f 7665 5f72 6567 696f 6e29 0a20 2020  move_region).   
-000266e0: 2020 2020 2073 656c 662e 6d6e 652e 7669       self.mne.vi
-000266f0: 6577 626f 782e 7369 6759 5261 6e67 6543  ewbox.sigYRangeC
-00026700: 6861 6e67 6564 2e63 6f6e 6e65 6374 2872  hanged.connect(r
-00026710: 6567 696f 6e2e 7570 6461 7465 5f6c 6162  egion.update_lab
-00026720: 656c 5f70 6f73 290a 2020 2020 2020 2020  el_pos).        
-00026730: 7265 6769 6f6e 2e75 7064 6174 655f 6c61  region.update_la
-00026740: 6265 6c5f 706f 7328 290a 2020 2020 2020  bel_pos().      
-00026750: 2020 7265 7475 726e 2072 6567 696f 6e0a    return region.
-00026760: 0a20 2020 2064 6566 205f 7265 6d6f 7665  .    def _remove
-00026770: 5f72 6567 696f 6e28 7365 6c66 2c20 7265  _region(self, re
-00026780: 6769 6f6e 2c20 6672 6f6d 5f61 6e6e 6f74  gion, from_annot
-00026790: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
-000267a0: 2320 5265 6d6f 7665 2066 726f 6d20 7368  # Remove from sh
-000267b0: 6f77 6e20 7265 6769 6f6e 730a 2020 2020  own regions.    
-000267c0: 2020 2020 6966 2072 6567 696f 6e2e 6c61      if region.la
-000267d0: 6265 6c5f 6974 656d 2069 6e20 7365 6c66  bel_item in self
-000267e0: 2e6d 6e65 2e70 6c74 2e69 7465 6d73 3a0a  .mne.plt.items:.
-000267f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00026800: 2e6d 6e65 2e70 6c74 2e72 656d 6f76 6549  .mne.plt.removeI
-00026810: 7465 6d28 7265 6769 6f6e 2e6c 6162 656c  tem(region.label
-00026820: 5f69 7465 6d29 0a20 2020 2020 2020 2069  _item).        i
-00026830: 6620 7265 6769 6f6e 2069 6e20 7365 6c66  f region in self
-00026840: 2e6d 6e65 2e70 6c74 2e69 7465 6d73 3a0a  .mne.plt.items:.
-00026850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00026860: 2e6d 6e65 2e70 6c74 2e72 656d 6f76 6549  .mne.plt.removeI
-00026870: 7465 6d28 7265 6769 6f6e 290a 0a20 2020  tem(region)..   
-00026880: 2020 2020 2023 2052 656d 6f76 6520 6672       # Remove fr
-00026890: 6f6d 2061 6c6c 2072 6567 696f 6e73 0a20  om all regions. 
-000268a0: 2020 2020 2020 2069 6620 7265 6769 6f6e         if region
-000268b0: 2069 6e20 7365 6c66 2e6d 6e65 2e72 6567   in self.mne.reg
-000268c0: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
-000268d0: 2020 7365 6c66 2e6d 6e65 2e72 6567 696f    self.mne.regio
-000268e0: 6e73 2e72 656d 6f76 6528 7265 6769 6f6e  ns.remove(region
-000268f0: 290a 0a20 2020 2020 2020 2023 2052 6573  )..        # Res
-00026900: 6574 2073 656c 6563 7465 6420 7265 6769  et selected regi
-00026910: 6f6e 0a20 2020 2020 2020 2069 6620 7265  on.        if re
-00026920: 6769 6f6e 203d 3d20 7365 6c66 2e6d 6e65  gion == self.mne
-00026930: 2e73 656c 6563 7465 645f 7265 6769 6f6e  .selected_region
-00026940: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00026950: 6c66 2e6d 6e65 2e73 656c 6563 7465 645f  lf.mne.selected_
-00026960: 7265 6769 6f6e 203d 204e 6f6e 650a 0a20  region = None.. 
-00026970: 2020 2020 2020 2023 2052 656d 6f76 6520         # Remove 
-00026980: 6672 6f6d 2061 6e6e 6f74 6174 696f 6e73  from annotations
-00026990: 0a20 2020 2020 2020 2069 6620 6672 6f6d  .        if from
-000269a0: 5f61 6e6e 6f74 3a0a 2020 2020 2020 2020  _annot:.        
-000269b0: 2020 2020 6964 7820 3d20 7365 6c66 2e5f      idx = self._
-000269c0: 6765 745f 6f6e 7365 745f 6964 7828 7265  get_onset_idx(re
-000269d0: 6769 6f6e 2e67 6574 5265 6769 6f6e 2829  gion.getRegion()
-000269e0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
-000269f0: 2073 656c 662e 6d6e 652e 696e 7374 2e61   self.mne.inst.a
-00026a00: 6e6e 6f74 6174 696f 6e73 2e64 656c 6574  nnotations.delet
-00026a10: 6528 6964 7829 0a0a 2020 2020 2020 2020  e(idx)..        
-00026a20: 2320 5570 6461 7465 204f 7665 7276 6965  # Update Overvie
-00026a30: 772d 4261 720a 2020 2020 2020 2020 7365  w-Bar.        se
-00026a40: 6c66 2e6d 6e65 2e6f 7665 7276 6965 775f  lf.mne.overview_
-00026a50: 6261 722e 7570 6461 7465 5f61 6e6e 6f74  bar.update_annot
-00026a60: 6174 696f 6e73 2829 0a0a 2020 2020 6465  ations()..    de
-00026a70: 6620 5f72 6567 696f 6e5f 7365 6c65 6374  f _region_select
-00026a80: 6564 2873 656c 662c 2072 6567 696f 6e29  ed(self, region)
-00026a90: 3a0a 2020 2020 2020 2020 6f6c 645f 7265  :.        old_re
-00026aa0: 6769 6f6e 203d 2073 656c 662e 6d6e 652e  gion = self.mne.
-00026ab0: 7365 6c65 6374 6564 5f72 6567 696f 6e0a  selected_region.
-00026ac0: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
-00026ad0: 2073 656c 6563 7465 642d 7374 6174 7573   selected-status
-00026ae0: 2066 726f 6d20 6f6c 6420 7265 6769 6f6e   from old region
-00026af0: 0a20 2020 2020 2020 2069 6620 6f6c 645f  .        if old_
-00026b00: 7265 6769 6f6e 2061 6e64 206f 6c64 5f72  region and old_r
-00026b10: 6567 696f 6e20 213d 2072 6567 696f 6e3a  egion != region:
-00026b20: 0a20 2020 2020 2020 2020 2020 206f 6c64  .            old
-00026b30: 5f72 6567 696f 6e2e 7365 6c65 6374 2846  _region.select(F
-00026b40: 616c 7365 290a 2020 2020 2020 2020 7365  alse).        se
-00026b50: 6c66 2e6d 6e65 2e73 656c 6563 7465 645f  lf.mne.selected_
-00026b60: 7265 6769 6f6e 203d 2072 6567 696f 6e0a  region = region.
-00026b70: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
-00026b80: 2e66 6967 5f61 6e6e 6f74 6174 696f 6e2e  .fig_annotation.
-00026b90: 7570 6461 7465 5f76 616c 7565 7328 7265  update_values(re
-00026ba0: 6769 6f6e 290a 0a20 2020 2064 6566 205f  gion)..    def _
-00026bb0: 6765 745f 6f6e 7365 745f 6964 7828 7365  get_onset_idx(se
-00026bc0: 6c66 2c20 706c 6f74 5f6f 6e73 6574 293a  lf, plot_onset):
-00026bd0: 0a20 2020 2020 2020 206f 6e73 6574 203d  .        onset =
-00026be0: 205f 7379 6e63 5f6f 6e73 6574 2873 656c   _sync_onset(sel
-00026bf0: 662e 6d6e 652e 696e 7374 2c20 706c 6f74  f.mne.inst, plot
-00026c00: 5f6f 6e73 6574 2c20 696e 7665 7273 653d  _onset, inverse=
-00026c10: 5472 7565 290a 2020 2020 2020 2020 6964  True).        id
-00026c20: 7820 3d20 6e70 2e77 6865 7265 2873 656c  x = np.where(sel
-00026c30: 662e 6d6e 652e 696e 7374 2e61 6e6e 6f74  f.mne.inst.annot
-00026c40: 6174 696f 6e73 2e6f 6e73 6574 203d 3d20  ations.onset == 
-00026c50: 6f6e 7365 7429 5b30 5d5b 305d 0a20 2020  onset)[0][0].   
-00026c60: 2020 2020 2072 6574 7572 6e20 6964 780a       return idx.
-00026c70: 0a20 2020 2064 6566 205f 7265 6769 6f6e  .    def _region
-00026c80: 5f63 6861 6e67 6564 2873 656c 662c 2072  _changed(self, r
-00026c90: 6567 696f 6e29 3a0a 2020 2020 2020 2020  egion):.        
-00026ca0: 7267 6e20 3d20 7265 6769 6f6e 2e67 6574  rgn = region.get
-00026cb0: 5265 6769 6f6e 2829 0a20 2020 2020 2020  Region().       
-00026cc0: 2072 6567 696f 6e2e 7365 6c65 6374 2854   region.select(T
-00026cd0: 7275 6529 0a20 2020 2020 2020 2069 6478  rue).        idx
-00026ce0: 203d 2073 656c 662e 5f67 6574 5f6f 6e73   = self._get_ons
-00026cf0: 6574 5f69 6478 2872 6567 696f 6e2e 6f6c  et_idx(region.ol
-00026d00: 645f 6f6e 7365 7429 0a0a 2020 2020 2020  d_onset)..      
-00026d10: 2020 2320 5570 6461 7465 2053 7069 6e62    # Update Spinb
-00026d20: 6f78 6573 206f 6620 416e 6e6f 742d 446f  oxes of Annot-Do
-00026d30: 636b 0a20 2020 2020 2020 2073 656c 662e  ck.        self.
-00026d40: 6d6e 652e 6669 675f 616e 6e6f 7461 7469  mne.fig_annotati
-00026d50: 6f6e 2e75 7064 6174 655f 7661 6c75 6573  on.update_values
-00026d60: 2872 6567 696f 6e29 0a0a 2020 2020 2020  (region)..      
-00026d70: 2020 2320 4368 616e 6765 2061 6e6e 6f74    # Change annot
-00026d80: 6174 696f 6e73 0a20 2020 2020 2020 2073  ations.        s
-00026d90: 656c 662e 6d6e 652e 696e 7374 2e61 6e6e  elf.mne.inst.ann
-00026da0: 6f74 6174 696f 6e73 2e6f 6e73 6574 5b69  otations.onset[i
-00026db0: 6478 5d20 3d20 5f73 796e 635f 6f6e 7365  dx] = _sync_onse
-00026dc0: 7428 7365 6c66 2e6d 6e65 2e69 6e73 742c  t(self.mne.inst,
-00026dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026e00: 2020 2020 2020 2020 2020 2020 7267 6e5b              rgn[
-00026e10: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
-00026e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026e40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00026e50: 6e76 6572 7365 3d54 7275 6529 0a20 2020  nverse=True).   
-00026e60: 2020 2020 2073 656c 662e 6d6e 652e 696e       self.mne.in
-00026e70: 7374 2e61 6e6e 6f74 6174 696f 6e73 2e64  st.annotations.d
-00026e80: 7572 6174 696f 6e5b 6964 785d 203d 2072  uration[idx] = r
-00026e90: 676e 5b31 5d20 2d20 7267 6e5b 305d 0a0a  gn[1] - rgn[0]..
-00026ea0: 2020 2020 2020 2020 2320 5570 6461 7465          # Update
-00026eb0: 206f 7665 7276 6965 772d 6261 720a 2020   overview-bar.  
-00026ec0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e6f        self.mne.o
-00026ed0: 7665 7276 6965 775f 6261 722e 7570 6461  verview_bar.upda
-00026ee0: 7465 5f61 6e6e 6f74 6174 696f 6e73 2829  te_annotations()
-00026ef0: 0a0a 2020 2020 6465 6620 5f64 7261 775f  ..    def _draw_
-00026f00: 616e 6e6f 7461 7469 6f6e 7328 7365 6c66  annotations(self
-00026f10: 293a 0a20 2020 2020 2020 2023 2041 6c6c  ):.        # All
-00026f20: 2072 6567 696f 6e73 2061 7265 2063 6f6e   regions are con
-00026f30: 7374 616e 746c 7920 6164 6465 6420 746f  stantly added to
-00026f40: 2074 6865 2053 6365 6e65 2061 6e64 2068   the Scene and h
-00026f50: 616e 646c 6564 2062 7920 5174 0a20 2020  andled by Qt.   
-00026f60: 2020 2020 2023 2077 6869 6368 2069 7320       # which is 
-00026f70: 6661 7374 6572 2074 6861 6e20 6861 6e64  faster than hand
-00026f80: 6c69 6e67 2061 6464 696e 672f 7265 6d6f  ling adding/remo
-00026f90: 7669 6e67 2069 6e20 5079 7468 6f6e 2e0a  ving in Python..
-00026fa0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00026fb0: 2020 6465 6620 5f69 6e69 745f 616e 6e6f    def _init_anno
-00026fc0: 745f 6d6f 6465 2873 656c 6629 3a0a 2020  t_mode(self):.  
-00026fd0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e61        self.mne.a
-00026fe0: 6e6e 6f74 6174 696f 6e73 5f76 6973 6962  nnotations_visib
-00026ff0: 6c65 203d 2054 7275 650a 2020 2020 2020  le = True.      
-00027000: 2020 7365 6c66 2e6d 6e65 2e6e 6577 5f61    self.mne.new_a
-00027010: 6e6e 6f74 6174 696f 6e5f 6c61 6265 6c73  nnotation_labels
-00027020: 203d 2073 656c 662e 5f67 6574 5f61 6e6e   = self._get_ann
-00027030: 6f74 6174 696f 6e5f 6c61 6265 6c73 2829  otation_labels()
-00027040: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00027050: 7365 6c66 2e6d 6e65 2e6e 6577 5f61 6e6e  self.mne.new_ann
-00027060: 6f74 6174 696f 6e5f 6c61 6265 6c73 2920  otation_labels) 
-00027070: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
-00027080: 2073 656c 662e 6d6e 652e 6375 7272 656e   self.mne.curren
-00027090: 745f 6465 7363 7269 7074 696f 6e20 3d20  t_description = 
-000270a0: 7365 6c66 2e6d 6e65 2e6e 6577 5f61 6e6e  self.mne.new_ann
-000270b0: 6f74 6174 696f 6e5f 6c61 6265 6c73 5b30  otation_labels[0
-000270c0: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-000270d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000270e0: 2e6d 6e65 2e63 7572 7265 6e74 5f64 6573  .mne.current_des
-000270f0: 6372 6970 7469 6f6e 203d 204e 6f6e 650a  cription = None.
-00027100: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
-00027110: 7475 705f 616e 6e6f 7461 7469 6f6e 5f63  tup_annotation_c
-00027120: 6f6c 6f72 7328 290a 2020 2020 2020 2020  olors().        
-00027130: 7365 6c66 2e6d 6e65 2e72 6567 696f 6e73  self.mne.regions
-00027140: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
-00027150: 2020 7365 6c66 2e6d 6e65 2e73 656c 6563    self.mne.selec
-00027160: 7465 645f 7265 6769 6f6e 203d 204e 6f6e  ted_region = Non
-00027170: 650a 0a20 2020 2020 2020 2023 2049 6e69  e..        # Ini
-00027180: 7469 616c 697a 6520 416e 6e6f 7461 7469  tialize Annotati
-00027190: 6f6e 2d44 6f63 6b0a 2020 2020 2020 2020  on-Dock.        
-000271a0: 6578 6973 7469 6e67 5f64 6f63 6b20 3d20  existing_dock = 
-000271b0: 6765 7461 7474 7228 7365 6c66 2e6d 6e65  getattr(self.mne
-000271c0: 2c20 2766 6967 5f61 6e6e 6f74 6174 696f  , 'fig_annotatio
-000271d0: 6e27 2c20 4e6f 6e65 290a 2020 2020 2020  n', None).      
-000271e0: 2020 6966 2065 7869 7374 696e 675f 646f    if existing_do
-000271f0: 636b 2069 7320 4e6f 6e65 3a0a 2020 2020  ck is None:.    
-00027200: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
-00027210: 2e66 6967 5f61 6e6e 6f74 6174 696f 6e20  .fig_annotation 
-00027220: 3d20 416e 6e6f 7461 7469 6f6e 446f 636b  = AnnotationDock
-00027230: 2873 656c 6629 0a20 2020 2020 2020 2020  (self).         
-00027240: 2020 2073 656c 662e 6164 6444 6f63 6b57     self.addDockW
-00027250: 6964 6765 7428 5174 2e54 6f70 446f 636b  idget(Qt.TopDock
-00027260: 5769 6467 6574 4172 6561 2c20 7365 6c66  WidgetArea, self
-00027270: 2e6d 6e65 2e66 6967 5f61 6e6e 6f74 6174  .mne.fig_annotat
-00027280: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
-00027290: 2073 656c 662e 6d6e 652e 6669 675f 616e   self.mne.fig_an
-000272a0: 6e6f 7461 7469 6f6e 2e73 6574 5669 7369  notation.setVisi
-000272b0: 626c 6528 4661 6c73 6529 0a0a 2020 2020  ble(False)..    
-000272c0: 2020 2020 2320 4164 6420 616e 6e6f 7461      # Add annota
-000272d0: 7469 6f6e 7320 6173 2072 6567 696f 6e73  tions as regions
-000272e0: 0a20 2020 2020 2020 2066 6f72 2061 6e6e  .        for ann
-000272f0: 6f74 2069 6e20 7365 6c66 2e6d 6e65 2e69  ot in self.mne.i
-00027300: 6e73 742e 616e 6e6f 7461 7469 6f6e 733a  nst.annotations:
-00027310: 0a20 2020 2020 2020 2020 2020 2070 6c6f  .            plo
-00027320: 745f 6f6e 7365 7420 3d20 5f73 796e 635f  t_onset = _sync_
-00027330: 6f6e 7365 7428 7365 6c66 2e6d 6e65 2e69  onset(self.mne.i
-00027340: 6e73 742c 2061 6e6e 6f74 5b27 6f6e 7365  nst, annot['onse
-00027350: 7427 5d29 0a20 2020 2020 2020 2020 2020  t']).           
-00027360: 2064 7572 6174 696f 6e20 3d20 616e 6e6f   duration = anno
-00027370: 745b 2764 7572 6174 696f 6e27 5d0a 2020  t['duration'].  
-00027380: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00027390: 7074 696f 6e20 3d20 616e 6e6f 745b 2764  ption = annot['d
-000273a0: 6573 6372 6970 7469 6f6e 275d 0a20 2020  escription'].   
-000273b0: 2020 2020 2020 2020 2072 6567 696f 6e20           region 
-000273c0: 3d20 7365 6c66 2e5f 6164 645f 7265 6769  = self._add_regi
-000273d0: 6f6e 2870 6c6f 745f 6f6e 7365 742c 2064  on(plot_onset, d
-000273e0: 7572 6174 696f 6e2c 2064 6573 6372 6970  uration, descrip
-000273f0: 7469 6f6e 290a 2020 2020 2020 2020 2020  tion).          
-00027400: 2020 7265 6769 6f6e 2e75 7064 6174 655f    region.update_
-00027410: 7669 7369 626c 6528 4661 6c73 6529 0a0a  visible(False)..
-00027420: 2020 2020 2020 2020 2320 496e 6974 6961          # Initia
-00027430: 6c69 7a65 2073 686f 7769 6e67 2061 6e6e  lize showing ann
-00027440: 6f74 6174 696f 6e20 7769 6467 6574 730a  otation widgets.
-00027450: 2020 2020 2020 2020 7365 6c66 2e5f 6368          self._ch
-00027460: 616e 6765 5f61 6e6e 6f74 5f6d 6f64 6528  ange_annot_mode(
-00027470: 290a 0a20 2020 2064 6566 205f 6368 616e  )..    def _chan
-00027480: 6765 5f61 6e6e 6f74 5f6d 6f64 6528 7365  ge_annot_mode(se
-00027490: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-000274a0: 6e6f 7420 7365 6c66 2e6d 6e65 2e61 6e6e  not self.mne.ann
-000274b0: 6f74 6174 696f 6e5f 6d6f 6465 3a0a 2020  otation_mode:.  
-000274c0: 2020 2020 2020 2020 2020 2320 5265 7365            # Rese
-000274d0: 7420 5769 6467 6574 7320 696e 2041 6e6e  t Widgets in Ann
-000274e0: 6f74 6174 696f 6e2d 4669 6775 7265 0a20  otation-Figure. 
-000274f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00027500: 6d6e 652e 6669 675f 616e 6e6f 7461 7469  mne.fig_annotati
-00027510: 6f6e 2e72 6573 6574 2829 0a0a 2020 2020  on.reset()..    
-00027520: 2020 2020 2320 5368 6f77 2041 6e6e 6f74      # Show Annot
-00027530: 6174 696f 6e2d 446f 636b 2069 6620 6163  ation-Dock if ac
-00027540: 7469 7661 7465 642e 0a20 2020 2020 2020  tivated..       
-00027550: 2073 656c 662e 6d6e 652e 6669 675f 616e   self.mne.fig_an
-00027560: 6e6f 7461 7469 6f6e 2e73 6574 5669 7369  notation.setVisi
-00027570: 626c 6528 7365 6c66 2e6d 6e65 2e61 6e6e  ble(self.mne.ann
-00027580: 6f74 6174 696f 6e5f 6d6f 6465 290a 0a20  otation_mode).. 
-00027590: 2020 2020 2020 2023 204d 616b 6520 5265         # Make Re
-000275a0: 6769 6f6e 7320 6d6f 7661 626c 6520 6966  gions movable if
-000275b0: 2061 6374 6976 6174 6564 2061 6e64 206d   activated and m
-000275c0: 6f76 6520 696e 746f 2066 6f72 6567 726f  ove into foregro
-000275d0: 756e 640a 2020 2020 2020 2020 666f 7220  und.        for 
-000275e0: 7265 6769 6f6e 2069 6e20 7365 6c66 2e6d  region in self.m
-000275f0: 6e65 2e72 6567 696f 6e73 3a0a 2020 2020  ne.regions:.    
-00027600: 2020 2020 2020 2020 7265 6769 6f6e 2e73          region.s
-00027610: 6574 4d6f 7661 626c 6528 7365 6c66 2e6d  etMovable(self.m
-00027620: 6e65 2e61 6e6e 6f74 6174 696f 6e5f 6d6f  ne.annotation_mo
-00027630: 6465 290a 2020 2020 2020 2020 2020 2020  de).            
-00027640: 6966 2073 656c 662e 6d6e 652e 616e 6e6f  if self.mne.anno
-00027650: 7461 7469 6f6e 5f6d 6f64 653a 0a20 2020  tation_mode:.   
-00027660: 2020 2020 2020 2020 2020 2020 2072 6567               reg
-00027670: 696f 6e2e 7365 745a 5661 6c75 6528 3229  ion.setZValue(2)
-00027680: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00027690: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000276a0: 2020 2072 6567 696f 6e2e 7365 745a 5661     region.setZVa
-000276b0: 6c75 6528 3029 0a0a 2020 2020 2020 2020  lue(0)..        
-000276c0: 2320 4164 642f 5265 6d6f 7665 2073 656c  # Add/Remove sel
-000276d0: 6563 7469 6f6e 2d72 6563 7461 6e67 6c65  ection-rectangle
-000276e0: 2e0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-000276f0: 662e 6d6e 652e 7365 6c65 6374 6564 5f72  f.mne.selected_r
-00027700: 6567 696f 6e3a 0a20 2020 2020 2020 2020  egion:.         
-00027710: 2020 2073 656c 662e 6d6e 652e 7365 6c65     self.mne.sele
-00027720: 6374 6564 5f72 6567 696f 6e2e 7365 6c65  cted_region.sele
-00027730: 6374 2873 656c 662e 6d6e 652e 616e 6e6f  ct(self.mne.anno
-00027740: 7461 7469 6f6e 5f6d 6f64 6529 0a0a 2020  tation_mode)..  
-00027750: 2020 6465 6620 5f74 6f67 676c 655f 616e    def _toggle_an
-00027760: 6e6f 7461 7469 6f6e 5f66 6967 2873 656c  notation_fig(sel
-00027770: 6629 3a0a 2020 2020 2020 2020 6966 206e  f):.        if n
-00027780: 6f74 2073 656c 662e 6d6e 652e 6973 5f65  ot self.mne.is_e
-00027790: 706f 6368 733a 0a20 2020 2020 2020 2020  pochs:.         
-000277a0: 2020 2073 656c 662e 6d6e 652e 616e 6e6f     self.mne.anno
-000277b0: 7461 7469 6f6e 5f6d 6f64 6520 3d20 6e6f  tation_mode = no
-000277c0: 7420 7365 6c66 2e6d 6e65 2e61 6e6e 6f74  t self.mne.annot
-000277d0: 6174 696f 6e5f 6d6f 6465 0a20 2020 2020  ation_mode.     
-000277e0: 2020 2020 2020 2073 656c 662e 5f63 6861         self._cha
-000277f0: 6e67 655f 616e 6e6f 745f 6d6f 6465 2829  nge_annot_mode()
-00027800: 0a0a 2020 2020 6465 6620 5f75 7064 6174  ..    def _updat
-00027810: 655f 7265 6769 6f6e 735f 7669 7369 626c  e_regions_visibl
-00027820: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00027830: 2069 6620 7365 6c66 2e6d 6e65 2e69 735f   if self.mne.is_
-00027840: 6570 6f63 6873 3a0a 2020 2020 2020 2020  epochs:.        
-00027850: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00027860: 2020 2073 7461 7274 203d 2073 656c 662e     start = self.
-00027870: 6d6e 652e 745f 7374 6172 740a 2020 2020  mne.t_start.    
-00027880: 2020 2020 7374 6f70 203d 2073 7461 7274      stop = start
-00027890: 202b 2073 656c 662e 6d6e 652e 6475 7261   + self.mne.dura
-000278a0: 7469 6f6e 0a20 2020 2020 2020 2066 6f72  tion.        for
-000278b0: 2072 6567 696f 6e20 696e 2073 656c 662e   region in self.
-000278c0: 6d6e 652e 7265 6769 6f6e 733a 0a20 2020  mne.regions:.   
-000278d0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000278e0: 2e6d 6e65 2e76 6973 6962 6c65 5f61 6e6e  .mne.visible_ann
-000278f0: 6f74 6174 696f 6e73 5b72 6567 696f 6e2e  otations[region.
-00027900: 6465 7363 7269 7074 696f 6e5d 3a0a 2020  description]:.  
-00027910: 2020 2020 2020 2020 2020 2020 2020 7267                rg
-00027920: 6e20 3d20 7265 6769 6f6e 2e67 6574 5265  n = region.getRe
-00027930: 6769 6f6e 2829 0a20 2020 2020 2020 2020  gion().         
-00027940: 2020 2020 2020 2023 2041 766f 6964 204e         # Avoid N
-00027950: 756d 5079 2062 6f6f 6c20 6865 7265 0a20  umPy bool here. 
-00027960: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00027970: 6973 6962 6c65 203d 2062 6f6f 6c28 7267  isible = bool(rg
-00027980: 6e5b 305d 203c 3d20 7374 6f70 2061 6e64  n[0] <= stop and
-00027990: 2072 676e 5b31 5d20 3e3d 2073 7461 7274   rgn[1] >= start
-000279a0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000279b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000279c0: 2020 2020 7669 7369 626c 6520 3d20 4661      visible = Fa
-000279d0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-000279e0: 7265 6769 6f6e 2e75 7064 6174 655f 7669  region.update_vi
-000279f0: 7369 626c 6528 7669 7369 626c 6529 0a20  sible(visible). 
-00027a00: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-00027a10: 6f76 6572 7669 6577 5f62 6172 2e75 7064  overview_bar.upd
-00027a20: 6174 655f 616e 6e6f 7461 7469 6f6e 7328  ate_annotations(
-00027a30: 290a 0a20 2020 2064 6566 205f 7365 745f  )..    def _set_
-00027a40: 616e 6e6f 7461 7469 6f6e 735f 7669 7369  annotations_visi
-00027a50: 626c 6528 7365 6c66 2c20 7669 7369 626c  ble(self, visibl
-00027a60: 6529 3a0a 2020 2020 2020 2020 666f 7220  e):.        for 
-00027a70: 6465 7363 7220 696e 2073 656c 662e 6d6e  descr in self.mn
-00027a80: 652e 7669 7369 626c 655f 616e 6e6f 7461  e.visible_annota
-00027a90: 7469 6f6e 733a 0a20 2020 2020 2020 2020  tions:.         
-00027aa0: 2020 2073 656c 662e 6d6e 652e 7669 7369     self.mne.visi
-00027ab0: 626c 655f 616e 6e6f 7461 7469 6f6e 735b  ble_annotations[
-00027ac0: 6465 7363 725d 203d 2076 6973 6962 6c65  descr] = visible
-00027ad0: 0a20 2020 2020 2020 2073 656c 662e 5f75  .        self._u
-00027ae0: 7064 6174 655f 7265 6769 6f6e 735f 7669  pdate_regions_vi
-00027af0: 7369 626c 6528 290a 0a20 2020 2064 6566  sible()..    def
-00027b00: 205f 746f 6767 6c65 5f61 6e6e 6f74 6174   _toggle_annotat
-00027b10: 696f 6e73 2873 656c 6629 3a0a 2020 2020  ions(self):.    
-00027b20: 2020 2020 7365 6c66 2e6d 6e65 2e61 6e6e      self.mne.ann
-00027b30: 6f74 6174 696f 6e73 5f76 6973 6962 6c65  otations_visible
-00027b40: 203d 206e 6f74 2073 656c 662e 6d6e 652e   = not self.mne.
-00027b50: 616e 6e6f 7461 7469 6f6e 735f 7669 7369  annotations_visi
-00027b60: 626c 650a 2020 2020 2020 2020 7365 6c66  ble.        self
-00027b70: 2e5f 7365 745f 616e 6e6f 7461 7469 6f6e  ._set_annotation
-00027b80: 735f 7669 7369 626c 6528 7365 6c66 2e6d  s_visible(self.m
-00027b90: 6e65 2e61 6e6e 6f74 6174 696f 6e73 5f76  ne.annotations_v
-00027ba0: 6973 6962 6c65 290a 0a20 2020 2064 6566  isible)..    def
-00027bb0: 205f 6170 706c 795f 7570 6461 7465 5f70   _apply_update_p
-00027bc0: 726f 6a65 6374 6f72 7328 7365 6c66 2c20  rojectors(self, 
-00027bd0: 746f 6767 6c65 5f61 6c6c 3d46 616c 7365  toggle_all=False
-00027be0: 293a 0a20 2020 2020 2020 2069 6620 746f  ):.        if to
-00027bf0: 6767 6c65 5f61 6c6c 3a0a 2020 2020 2020  ggle_all:.      
-00027c00: 2020 2020 2020 6f6e 203d 2073 656c 662e        on = self.
-00027c10: 6d6e 652e 7072 6f6a 735f 6f6e 0a20 2020  mne.projs_on.   
-00027c20: 2020 2020 2020 2020 2061 7070 6c69 6564           applied
-00027c30: 203d 2073 656c 662e 6d6e 652e 7072 6f6a   = self.mne.proj
-00027c40: 735f 6163 7469 7665 0a20 2020 2020 2020  s_active.       
-00027c50: 2020 2020 2076 616c 7565 203d 2046 616c       value = Fal
-00027c60: 7365 2069 6620 616c 6c28 6f6e 2920 656c  se if all(on) el
-00027c70: 7365 2054 7275 650a 2020 2020 2020 2020  se True.        
-00027c80: 2020 2020 6e65 775f 7374 6174 6520 3d20      new_state = 
-00027c90: 6e70 2e66 756c 6c5f 6c69 6b65 286f 6e2c  np.full_like(on,
-00027ca0: 2076 616c 7565 290a 2020 2020 2020 2020   value).        
-00027cb0: 2020 2020 2320 416c 7761 7973 2061 6374      # Always act
-00027cc0: 6976 6174 6520 6170 706c 6965 6420 7072  ivate applied pr
-00027cd0: 6f6a 6563 7469 6f6e 730a 2020 2020 2020  ojections.      
-00027ce0: 2020 2020 2020 6e65 775f 7374 6174 655b        new_state[
-00027cf0: 6170 706c 6965 645d 203d 2054 7275 650a  applied] = True.
-00027d00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00027d10: 2e6d 6e65 2e70 726f 6a73 5f6f 6e20 3d20  .mne.projs_on = 
-00027d20: 6e65 775f 7374 6174 650a 2020 2020 2020  new_state.      
-00027d30: 2020 7365 6c66 2e5f 7570 6461 7465 5f70    self._update_p
-00027d40: 726f 6a65 6374 6f72 2829 0a20 2020 2020  rojector().     
-00027d50: 2020 2023 2049 6620 6461 7461 2077 6173     # If data was
-00027d60: 2070 7265 636f 6d70 7574 6564 2069 7420   precomputed it 
-00027d70: 6e65 6564 7320 746f 2062 6520 7072 6563  needs to be prec
-00027d80: 6f6d 7075 7465 6420 6167 6169 6e2e 0a20  omputed again.. 
-00027d90: 2020 2020 2020 2073 656c 662e 5f72 6572         self._rer
-00027da0: 756e 5f70 7265 636f 6d70 7574 6528 290a  un_precompute().
-00027db0: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
-00027dc0: 6472 6177 2829 0a0a 2020 2020 6465 6620  draw()..    def 
-00027dd0: 5f74 6f67 676c 655f 7072 6f6a 5f66 6967  _toggle_proj_fig
-00027de0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00027df0: 6966 2073 656c 662e 6d6e 652e 6669 675f  if self.mne.fig_
-00027e00: 7072 6f6a 2069 7320 4e6f 6e65 3a0a 2020  proj is None:.  
-00027e10: 2020 2020 2020 2020 2020 5072 6f6a 4469            ProjDi
-00027e20: 616c 6f67 2873 656c 662c 206e 616d 653d  alog(self, name=
-00027e30: 2766 6967 5f70 726f 6a27 290a 2020 2020  'fig_proj').    
-00027e40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00027e50: 2020 2020 2020 7365 6c66 2e6d 6e65 2e66        self.mne.f
-00027e60: 6967 5f70 726f 6a2e 636c 6f73 6528 290a  ig_proj.close().
-00027e70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00027e80: 2e6d 6e65 2e66 6967 5f70 726f 6a20 3d20  .mne.fig_proj = 
-00027e90: 4e6f 6e65 0a0a 2020 2020 6465 6620 5f74  None..    def _t
-00027ea0: 6f67 676c 655f 616c 6c5f 7072 6f6a 7328  oggle_all_projs(
-00027eb0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-00027ec0: 6620 7365 6c66 2e6d 6e65 2e66 6967 5f70  f self.mne.fig_p
-00027ed0: 726f 6a20 6973 204e 6f6e 653a 0a20 2020  roj is None:.   
-00027ee0: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
-00027ef0: 7070 6c79 5f75 7064 6174 655f 7072 6f6a  pply_update_proj
-00027f00: 6563 746f 7273 2874 6f67 676c 655f 616c  ectors(toggle_al
-00027f10: 6c3d 5472 7565 290a 2020 2020 2020 2020  l=True).        
-00027f20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00027f30: 2020 7365 6c66 2e6d 6e65 2e66 6967 5f70    self.mne.fig_p
-00027f40: 726f 6a2e 746f 6767 6c65 5f61 6c6c 2829  roj.toggle_all()
-00027f50: 0a0a 2020 2020 6465 6620 5f74 6f67 676c  ..    def _toggl
-00027f60: 655f 7768 6974 656e 696e 6728 7365 6c66  e_whitening(self
-00027f70: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
-00027f80: 2829 2e5f 746f 6767 6c65 5f77 6869 7465  ()._toggle_white
-00027f90: 6e69 6e67 2829 0a20 2020 2020 2020 2023  ning().        #
-00027fa0: 2049 6620 6461 7461 2077 6173 2070 7265   If data was pre
-00027fb0: 636f 6d70 7574 6564 2069 7420 6e65 6564  computed it need
-00027fc0: 7320 746f 2062 6520 7072 6563 6f6d 7075  s to be precompu
-00027fd0: 7465 6420 6167 6169 6e2e 0a20 2020 2020  ted again..     
-00027fe0: 2020 2073 656c 662e 5f72 6572 756e 5f70     self._rerun_p
-00027ff0: 7265 636f 6d70 7574 6528 290a 2020 2020  recompute().    
-00028000: 2020 2020 7365 6c66 2e5f 7265 6472 6177      self._redraw
-00028010: 2829 0a0a 2020 2020 6465 6620 5f74 6f67  ()..    def _tog
-00028020: 676c 655f 7365 7474 696e 6773 5f66 6967  gle_settings_fig
-00028030: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00028040: 6966 2073 656c 662e 6d6e 652e 6669 675f  if self.mne.fig_
-00028050: 7365 7474 696e 6773 2069 7320 4e6f 6e65  settings is None
-00028060: 3a0a 2020 2020 2020 2020 2020 2020 5365  :.            Se
-00028070: 7474 696e 6773 4469 616c 6f67 2873 656c  ttingsDialog(sel
-00028080: 662c 206e 616d 653d 2766 6967 5f73 6574  f, name='fig_set
-00028090: 7469 6e67 7327 290a 2020 2020 2020 2020  tings').        
-000280a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000280b0: 2020 7365 6c66 2e6d 6e65 2e66 6967 5f73    self.mne.fig_s
-000280c0: 6574 7469 6e67 732e 636c 6f73 6528 290a  ettings.close().
-000280d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000280e0: 2e6d 6e65 2e66 6967 5f73 6574 7469 6e67  .mne.fig_setting
-000280f0: 7320 3d20 4e6f 6e65 0a0a 2020 2020 6465  s = None..    de
-00028100: 6620 5f74 6f67 676c 655f 6865 6c70 5f66  f _toggle_help_f
-00028110: 6967 2873 656c 6629 3a0a 2020 2020 2020  ig(self):.      
-00028120: 2020 6966 2073 656c 662e 6d6e 652e 6669    if self.mne.fi
-00028130: 675f 6865 6c70 2069 7320 4e6f 6e65 3a0a  g_help is None:.
-00028140: 2020 2020 2020 2020 2020 2020 4865 6c70              Help
-00028150: 4469 616c 6f67 2873 656c 662c 206e 616d  Dialog(self, nam
-00028160: 653d 2766 6967 5f68 656c 7027 290a 2020  e='fig_help').  
-00028170: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00028180: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
-00028190: 2e66 6967 5f68 656c 702e 636c 6f73 6528  .fig_help.close(
-000281a0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000281b0: 6c66 2e6d 6e65 2e66 6967 5f68 656c 7020  lf.mne.fig_help 
-000281c0: 3d20 4e6f 6e65 0a0a 2020 2020 6465 6620  = None..    def 
-000281d0: 5f73 6574 5f62 7574 7465 7266 6c79 2873  _set_butterfly(s
-000281e0: 656c 662c 2062 7574 7465 7266 6c79 293a  elf, butterfly):
-000281f0: 0a20 2020 2020 2020 2073 656c 662e 6d6e  .        self.mn
-00028200: 652e 6275 7474 6572 666c 7920 3d20 6275  e.butterfly = bu
-00028210: 7474 6572 666c 790a 2020 2020 2020 2020  tterfly.        
-00028220: 7365 6c66 2e5f 7570 6461 7465 5f70 6963  self._update_pic
-00028230: 6b73 2829 0a20 2020 2020 2020 2073 656c  ks().        sel
-00028240: 662e 5f75 7064 6174 655f 6461 7461 2829  f._update_data()
-00028250: 0a0a 2020 2020 2020 2020 6966 2062 7574  ..        if but
-00028260: 7465 7266 6c79 2061 6e64 2073 656c 662e  terfly and self.
-00028270: 6d6e 652e 6669 675f 7365 6c65 6374 696f  mne.fig_selectio
-00028280: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00028290: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000282a0: 6d6e 652e 7365 6c65 6374 696f 6e5f 7970  mne.selection_yp
-000282b0: 6f73 5f64 6963 742e 636c 6561 7228 290a  os_dict.clear().
-000282c0: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
-000282d0: 6374 696f 6e73 5f64 6963 7420 3d20 7365  ctions_dict = se
-000282e0: 6c66 2e5f 6d61 6b65 5f62 7574 7465 7266  lf._make_butterf
-000282f0: 6c79 5f73 656c 6563 7469 6f6e 735f 6469  ly_selections_di
-00028300: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
-00028310: 2066 6f72 2069 6478 2c20 7069 636b 7320   for idx, picks 
-00028320: 696e 2065 6e75 6d65 7261 7465 2873 656c  in enumerate(sel
-00028330: 6563 7469 6f6e 735f 6469 6374 2e76 616c  ections_dict.val
-00028340: 7565 7328 2929 3a0a 2020 2020 2020 2020  ues()):.        
-00028350: 2020 2020 2020 2020 666f 7220 7069 636b          for pick
-00028360: 2069 6e20 7069 636b 733a 0a20 2020 2020   in picks:.     
-00028370: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00028380: 656c 662e 6d6e 652e 7365 6c65 6374 696f  elf.mne.selectio
-00028390: 6e5f 7970 6f73 5f64 6963 745b 7069 636b  n_ypos_dict[pick
-000283a0: 5d20 3d20 6964 7820 2b20 310a 2020 2020  ] = idx + 1.    
-000283b0: 2020 2020 2020 2020 796d 6178 203d 206c          ymax = l
-000283c0: 656e 2873 656c 6563 7469 6f6e 735f 6469  en(selections_di
-000283d0: 6374 2920 2b20 310a 2020 2020 2020 2020  ct) + 1.        
-000283e0: 2020 2020 7365 6c66 2e6d 6e65 2e79 6d61      self.mne.yma
-000283f0: 7820 3d20 796d 6178 0a20 2020 2020 2020  x = ymax.       
-00028400: 2020 2020 2073 656c 662e 6d6e 652e 706c       self.mne.pl
-00028410: 742e 7365 744c 696d 6974 7328 794d 6178  t.setLimits(yMax
-00028420: 3d79 6d61 7829 0a20 2020 2020 2020 2020  =ymax).         
-00028430: 2020 2073 656c 662e 6d6e 652e 706c 742e     self.mne.plt.
-00028440: 7365 7459 5261 6e67 6528 302c 2079 6d61  setYRange(0, yma
-00028450: 782c 2070 6164 6469 6e67 3d30 290a 2020  x, padding=0).  
-00028460: 2020 2020 2020 656c 6966 2062 7574 7465        elif butte
-00028470: 7266 6c79 3a0a 2020 2020 2020 2020 2020  rfly:.          
-00028480: 2020 796d 6178 203d 206c 656e 2873 656c    ymax = len(sel
-00028490: 662e 6d6e 652e 6275 7474 6572 666c 795f  f.mne.butterfly_
-000284a0: 7479 7065 5f6f 7264 6572 2920 2b20 310a  type_order) + 1.
-000284b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000284c0: 2e6d 6e65 2e79 6d61 7820 3d20 796d 6178  .mne.ymax = ymax
-000284d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000284e0: 662e 6d6e 652e 706c 742e 7365 744c 696d  f.mne.plt.setLim
-000284f0: 6974 7328 794d 6178 3d79 6d61 7829 0a20  its(yMax=ymax). 
-00028500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00028510: 6d6e 652e 706c 742e 7365 7459 5261 6e67  mne.plt.setYRang
-00028520: 6528 302c 2079 6d61 782c 2070 6164 6469  e(0, ymax, paddi
-00028530: 6e67 3d30 290a 2020 2020 2020 2020 656c  ng=0).        el
-00028540: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00028550: 7365 6c66 2e6d 6e65 2e79 6d61 7820 3d20  self.mne.ymax = 
-00028560: 6c65 6e28 7365 6c66 2e6d 6e65 2e63 685f  len(self.mne.ch_
-00028570: 6f72 6465 7229 202b 2031 0a20 2020 2020  order) + 1.     
-00028580: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
-00028590: 706c 742e 7365 744c 696d 6974 7328 794d  plt.setLimits(yM
-000285a0: 6178 3d73 656c 662e 6d6e 652e 796d 6178  ax=self.mne.ymax
-000285b0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000285c0: 6c66 2e6d 6e65 2e70 6c74 2e73 6574 5952  lf.mne.plt.setYR
-000285d0: 616e 6765 2873 656c 662e 6d6e 652e 6368  ange(self.mne.ch
-000285e0: 5f73 7461 7274 2c0a 2020 2020 2020 2020  _start,.        
-000285f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028600: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00028610: 6d6e 652e 6368 5f73 7461 7274 202b 2073  mne.ch_start + s
-00028620: 656c 662e 6d6e 652e 6e5f 6368 616e 6e65  elf.mne.n_channe
-00028630: 6c73 202b 2031 2c0a 2020 2020 2020 2020  ls + 1,.        
-00028640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028650: 2020 2020 2020 2020 2020 2070 6164 6469             paddi
-00028660: 6e67 3d30 290a 0a20 2020 2020 2020 2069  ng=0)..        i
-00028670: 6620 7365 6c66 2e6d 6e65 2e66 6967 5f73  f self.mne.fig_s
-00028680: 656c 6563 7469 6f6e 2069 7320 6e6f 7420  election is not 
-00028690: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000286a0: 2020 2320 5570 6461 7465 2053 656c 6563    # Update Selec
-000286b0: 7469 6f6e 2d44 6961 6c6f 670a 2020 2020  tion-Dialog.    
-000286c0: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
-000286d0: 2e66 6967 5f73 656c 6563 7469 6f6e 2e5f  .fig_selection._
-000286e0: 7374 796c 655f 6275 7474 6572 666c 7928  style_butterfly(
-000286f0: 290a 0a20 2020 2020 2020 2023 2053 6574  )..        # Set
-00028700: 2076 6572 7469 6361 6c20 7363 726f 6c6c   vertical scroll
-00028710: 6261 7220 7669 7369 626c 650a 2020 2020  bar visible.    
-00028720: 2020 2020 7365 6c66 2e6d 6e65 2e61 785f      self.mne.ax_
-00028730: 7673 6372 6f6c 6c2e 7365 7456 6973 6962  vscroll.setVisib
-00028740: 6c65 286e 6f74 2062 7574 7465 7266 6c79  le(not butterfly
-00028750: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
-00028760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028770: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00028780: 6d6e 652e 6669 675f 7365 6c65 6374 696f  mne.fig_selectio
-00028790: 6e20 6973 206e 6f74 204e 6f6e 6529 0a0a  n is not None)..
-000287a0: 2020 2020 2020 2020 2320 7570 6461 7465          # update
-000287b0: 206f 7665 7276 6965 772d 6261 720a 2020   overview-bar.  
-000287c0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e6f        self.mne.o
-000287d0: 7665 7276 6965 775f 6261 722e 7570 6461  verview_bar.upda
-000287e0: 7465 5f76 6965 7772 616e 6765 2829 0a0a  te_viewrange()..
-000287f0: 2020 2020 2020 2020 2320 7570 6461 7465          # update
-00028800: 2079 706f 7320 616e 6420 636f 6c6f 7220   ypos and color 
-00028810: 666f 7220 6275 7474 6572 666c 792d 6d6f  for butterfly-mo
-00028820: 6465 0a20 2020 2020 2020 2066 6f72 2074  de.        for t
-00028830: 7261 6365 2069 6e20 7365 6c66 2e6d 6e65  race in self.mne
-00028840: 2e74 7261 6365 733a 0a20 2020 2020 2020  .traces:.       
-00028850: 2020 2020 2074 7261 6365 2e75 7064 6174       trace.updat
-00028860: 655f 636f 6c6f 7228 290a 2020 2020 2020  e_color().      
-00028870: 2020 2020 2020 7472 6163 652e 7570 6461        trace.upda
-00028880: 7465 5f79 706f 7328 290a 0a20 2020 2020  te_ypos()..     
-00028890: 2020 2073 656c 662e 5f64 7261 775f 7472     self._draw_tr
-000288a0: 6163 6573 2829 0a0a 2020 2020 6465 6620  aces()..    def 
-000288b0: 5f74 6f67 676c 655f 6275 7474 6572 666c  _toggle_butterfl
-000288c0: 7928 7365 6c66 293a 0a20 2020 2020 2020  y(self):.       
-000288d0: 2069 6620 7365 6c66 2e6d 6e65 2e69 6e73   if self.mne.ins
-000288e0: 7461 6e63 655f 7479 7065 2021 3d20 2769  tance_type != 'i
-000288f0: 6361 273a 0a20 2020 2020 2020 2020 2020  ca':.           
-00028900: 2073 656c 662e 5f73 6574 5f62 7574 7465   self._set_butte
-00028910: 7266 6c79 286e 6f74 2073 656c 662e 6d6e  rfly(not self.mn
-00028920: 652e 6275 7474 6572 666c 7929 0a0a 2020  e.butterfly)..  
-00028930: 2020 6465 6620 5f74 6f67 676c 655f 6463    def _toggle_dc
-00028940: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00028950: 7365 6c66 2e6d 6e65 2e72 656d 6f76 655f  self.mne.remove_
-00028960: 6463 203d 206e 6f74 2073 656c 662e 6d6e  dc = not self.mn
-00028970: 652e 7265 6d6f 7665 5f64 630a 2020 2020  e.remove_dc.    
-00028980: 2020 2020 7365 6c66 2e5f 7265 6472 6177      self._redraw
-00028990: 2829 0a0a 2020 2020 6465 6620 5f74 6f67  ()..    def _tog
-000289a0: 676c 655f 6570 6f63 685f 6869 7374 6f67  gle_epoch_histog
-000289b0: 7261 6d28 7365 6c66 293a 0a20 2020 2020  ram(self):.     
-000289c0: 2020 2066 6967 203d 2073 656c 662e 5f63     fig = self._c
-000289d0: 7265 6174 655f 6570 6f63 685f 6869 7374  reate_epoch_hist
-000289e0: 6f67 7261 6d28 290a 2020 2020 2020 2020  ogram().        
-000289f0: 7365 6c66 2e5f 6765 745f 646c 675f 6672  self._get_dlg_fr
-00028a00: 6f6d 5f6d 706c 2866 6967 290a 0a20 2020  om_mpl(fig)..   
-00028a10: 2064 6566 205f 7365 745f 6576 656e 7473   def _set_events
-00028a20: 5f76 6973 6962 6c65 2873 656c 662c 2076  _visible(self, v
-00028a30: 6973 6962 6c65 293a 0a20 2020 2020 2020  isible):.       
-00028a40: 2066 6f72 2065 7665 6e74 5f6c 696e 6520   for event_line 
-00028a50: 696e 2073 656c 662e 6d6e 652e 6576 656e  in self.mne.even
-00028a60: 745f 6c69 6e65 733a 0a20 2020 2020 2020  t_lines:.       
-00028a70: 2020 2020 2065 7665 6e74 5f6c 696e 652e       event_line.
-00028a80: 7365 7456 6973 6962 6c65 2876 6973 6962  setVisible(visib
-00028a90: 6c65 290a 0a20 2020 2020 2020 2073 656c  le)..        sel
-00028aa0: 662e 6d6e 652e 6f76 6572 7669 6577 5f62  f.mne.overview_b
-00028ab0: 6172 2e75 7064 6174 655f 6576 656e 7473  ar.update_events
-00028ac0: 2829 0a0a 2020 2020 6465 6620 5f74 6f67  ()..    def _tog
-00028ad0: 676c 655f 6576 656e 7473 2873 656c 6629  gle_events(self)
-00028ae0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00028af0: 662e 6d6e 652e 6576 656e 745f 6e75 6d73  f.mne.event_nums
-00028b00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00028b10: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00028b20: 6e65 2e65 7665 6e74 735f 7669 7369 626c  ne.events_visibl
-00028b30: 6520 3d20 6e6f 7420 7365 6c66 2e6d 6e65  e = not self.mne
-00028b40: 2e65 7665 6e74 735f 7669 7369 626c 650a  .events_visible.
-00028b50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00028b60: 2e5f 7365 745f 6576 656e 7473 5f76 6973  ._set_events_vis
-00028b70: 6962 6c65 2873 656c 662e 6d6e 652e 6576  ible(self.mne.ev
-00028b80: 656e 7473 5f76 6973 6962 6c65 290a 0a20  ents_visible).. 
-00028b90: 2020 2064 6566 205f 746f 6767 6c65 5f74     def _toggle_t
-00028ba0: 696d 655f 666f 726d 6174 2873 656c 6629  ime_format(self)
-00028bb0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00028bc0: 662e 6d6e 652e 7469 6d65 5f66 6f72 6d61  f.mne.time_forma
-00028bd0: 7420 3d3d 2027 666c 6f61 7427 3a0a 2020  t == 'float':.  
-00028be0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00028bf0: 6e65 2e74 696d 655f 666f 726d 6174 203d  ne.time_format =
-00028c00: 2027 636c 6f63 6b27 0a20 2020 2020 2020   'clock'.       
-00028c10: 2020 2020 2073 656c 662e 6d6e 652e 7469       self.mne.ti
-00028c20: 6d65 5f61 7869 732e 7365 744c 6162 656c  me_axis.setLabel
-00028c30: 2874 6578 743d 2754 696d 6520 6f66 2064  (text='Time of d
-00028c40: 6179 2729 0a20 2020 2020 2020 2065 6c73  ay').        els
-00028c50: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00028c60: 656c 662e 6d6e 652e 7469 6d65 5f66 6f72  elf.mne.time_for
-00028c70: 6d61 7420 3d20 2766 6c6f 6174 270a 2020  mat = 'float'.  
-00028c80: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00028c90: 6e65 2e74 696d 655f 6178 6973 2e73 6574  ne.time_axis.set
-00028ca0: 4c61 6265 6c28 7465 7874 3d27 5469 6d65  Label(text='Time
-00028cb0: 272c 2075 6e69 7473 3d27 7327 290a 2020  ', units='s').  
-00028cc0: 2020 2020 2020 7365 6c66 2e5f 7570 6461        self._upda
-00028cd0: 7465 5f79 6178 6973 5f6c 6162 656c 7328  te_yaxis_labels(
-00028ce0: 290a 0a20 2020 2064 6566 205f 746f 6767  )..    def _togg
-00028cf0: 6c65 5f66 756c 6c73 6372 6565 6e28 7365  le_fullscreen(se
-00028d00: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-00028d10: 7365 6c66 2e69 7346 756c 6c53 6372 6565  self.isFullScree
-00028d20: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
-00028d30: 2073 656c 662e 7368 6f77 4e6f 726d 616c   self.showNormal
-00028d40: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
-00028d50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00028d60: 662e 7368 6f77 4675 6c6c 5363 7265 656e  f.showFullScreen
-00028d70: 2829 0a0a 2020 2020 6465 6620 5f74 6f67  ()..    def _tog
-00028d80: 676c 655f 616e 7469 616c 6961 7369 6e67  gle_antialiasing
-00028d90: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00028da0: 7365 6c66 2e6d 6e65 2e61 6e74 6961 6c69  self.mne.antiali
-00028db0: 6173 696e 6720 3d20 6e6f 7420 7365 6c66  asing = not self
-00028dc0: 2e6d 6e65 2e61 6e74 6961 6c69 6173 696e  .mne.antialiasin
-00028dd0: 670a 2020 2020 2020 2020 7365 6c66 2e5f  g.        self._
-00028de0: 7265 6472 6177 2829 0a0a 2020 2020 6465  redraw()..    de
-00028df0: 6620 5f74 6f67 676c 655f 6f76 6572 7669  f _toggle_overvi
-00028e00: 6577 5f62 6172 2873 656c 6629 3a0a 2020  ew_bar(self):.  
-00028e10: 2020 2020 2020 7669 7369 626c 6520 3d20        visible = 
-00028e20: 6e6f 7420 7365 6c66 2e6d 6e65 2e6f 7665  not self.mne.ove
-00028e30: 7276 6965 775f 6261 722e 6973 5669 7369  rview_bar.isVisi
-00028e40: 626c 6528 290a 2020 2020 2020 2020 666f  ble().        fo
-00028e50: 7220 6974 656d 2069 6e20 7365 6c66 2e6d  r item in self.m
-00028e60: 6e65 2e6f 7665 7276 6965 775f 6d65 6e75  ne.overview_menu
-00028e70: 2e61 6374 696f 6e73 2829 3a0a 2020 2020  .actions():.    
-00028e80: 2020 2020 2020 2020 6966 2069 7465 6d2e          if item.
-00028e90: 7465 7874 2829 203d 3d20 2756 6973 6962  text() == 'Visib
-00028ea0: 6c65 273a 0a20 2020 2020 2020 2020 2020  le':.           
-00028eb0: 2020 2020 2069 7465 6d2e 7365 7443 6865       item.setChe
-00028ec0: 636b 6564 2876 6973 6962 6c65 290a 2020  cked(visible).  
-00028ed0: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00028ee0: 6561 6b0a 2020 2020 2020 2020 7365 6c66  eak.        self
-00028ef0: 2e6d 6e65 2e6f 7665 7276 6965 775f 6261  .mne.overview_ba
-00028f00: 722e 7365 7456 6973 6962 6c65 2876 6973  r.setVisible(vis
-00028f10: 6962 6c65 290a 0a20 2020 2064 6566 205f  ible)..    def _
-00028f20: 746f 6767 6c65 5f7a 656e 6d6f 6465 2873  toggle_zenmode(s
-00028f30: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-00028f40: 6c66 2e6d 6e65 2e73 6372 6f6c 6c62 6172  lf.mne.scrollbar
-00028f50: 735f 7669 7369 626c 6520 3d20 6e6f 7420  s_visible = not 
-00028f60: 7365 6c66 2e6d 6e65 2e73 6372 6f6c 6c62  self.mne.scrollb
-00028f70: 6172 735f 7669 7369 626c 650a 2020 2020  ars_visible.    
-00028f80: 2020 2020 666f 7220 6261 7220 696e 205b      for bar in [
-00028f90: 7365 6c66 2e6d 6e65 2e61 785f 6873 6372  self.mne.ax_hscr
-00028fa0: 6f6c 6c2c 2073 656c 662e 6d6e 652e 6178  oll, self.mne.ax
-00028fb0: 5f76 7363 726f 6c6c 5d3a 0a20 2020 2020  _vscroll]:.     
-00028fc0: 2020 2020 2020 2062 6172 2e73 6574 5669         bar.setVi
-00028fd0: 7369 626c 6528 7365 6c66 2e6d 6e65 2e73  sible(self.mne.s
-00028fe0: 6372 6f6c 6c62 6172 735f 7669 7369 626c  crollbars_visibl
-00028ff0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-00029000: 6d6e 652e 746f 6f6c 6261 722e 7365 7456  mne.toolbar.setV
-00029010: 6973 6962 6c65 2873 656c 662e 6d6e 652e  isible(self.mne.
-00029020: 7363 726f 6c6c 6261 7273 5f76 6973 6962  scrollbars_visib
-00029030: 6c65 290a 0a20 2020 2064 6566 205f 6e65  le)..    def _ne
-00029040: 775f 6368 696c 645f 6669 6775 7265 2873  w_child_figure(s
-00029050: 656c 662c 2066 6967 5f6e 616d 652c 2077  elf, fig_name, w
-00029060: 696e 646f 775f 7469 746c 652c 202a 2a6b  indow_title, **k
-00029070: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-00029080: 6672 6f6d 206d 6174 706c 6f74 6c69 622e  from matplotlib.
-00029090: 6669 6775 7265 2069 6d70 6f72 7420 4669  figure import Fi
-000290a0: 6775 7265 0a20 2020 2020 2020 2066 6967  gure.        fig
-000290b0: 203d 2046 6967 7572 6528 2a2a 6b77 6172   = Figure(**kwar
-000290c0: 6773 290a 2020 2020 2020 2020 2320 5061  gs).        # Pa
-000290d0: 7373 2077 696e 646f 7720 7469 746c 6520  ss window title 
-000290e0: 616e 6420 6669 675f 6e61 6d65 206f 6e0a  and fig_name on.
-000290f0: 2020 2020 2020 2020 6966 2066 6967 5f6e          if fig_n
-00029100: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-00029110: 0a20 2020 2020 2020 2020 2020 2066 6967  .            fig
-00029120: 2e66 6967 5f6e 616d 6520 3d20 6669 675f  .fig_name = fig_
-00029130: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
-00029140: 7769 6e64 6f77 5f74 6974 6c65 2069 7320  window_title is 
-00029150: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00029160: 2020 2020 2020 6669 672e 7469 746c 6520        fig.title 
-00029170: 3d20 7769 6e64 6f77 5f74 6974 6c65 0a20  = window_title. 
-00029180: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
-00029190: 670a 0a20 2020 2064 6566 205f 6765 745f  g..    def _get_
-000291a0: 7769 6467 6574 5f66 726f 6d5f 6d70 6c28  widget_from_mpl(
-000291b0: 7365 6c66 2c20 6669 6729 3a0a 2020 2020  self, fig):.    
-000291c0: 2020 2020 6361 6e76 6173 203d 2046 6967      canvas = Fig
-000291d0: 7572 6543 616e 7661 7351 5441 6767 2866  ureCanvasQTAgg(f
-000291e0: 6967 290a 2020 2020 2020 2020 6361 6e76  ig).        canv
-000291f0: 6173 2e73 6574 466f 6375 7350 6f6c 6963  as.setFocusPolic
-00029200: 7928 5174 2e46 6f63 7573 506f 6c69 6379  y(Qt.FocusPolicy
-00029210: 2851 742e 5374 726f 6e67 466f 6375 7320  (Qt.StrongFocus 
-00029220: 7c20 5174 2e57 6865 656c 466f 6375 7329  | Qt.WheelFocus)
-00029230: 290a 2020 2020 2020 2020 6361 6e76 6173  ).        canvas
-00029240: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
-00029250: 2020 2020 2320 5061 7373 2077 696e 646f      # Pass windo
-00029260: 7720 7469 746c 6520 616e 6420 6669 675f  w title and fig_
-00029270: 6e61 6d65 206f 6e0a 2020 2020 2020 2020  name on.        
-00029280: 6966 2068 6173 6174 7472 2866 6967 2c20  if hasattr(fig, 
-00029290: 2766 6967 5f6e 616d 6527 293a 0a20 2020  'fig_name'):.   
-000292a0: 2020 2020 2020 2020 2063 616e 7661 732e           canvas.
-000292b0: 6669 675f 6e61 6d65 203d 2066 6967 2e66  fig_name = fig.f
-000292c0: 6967 5f6e 616d 650a 2020 2020 2020 2020  ig_name.        
-000292d0: 6966 2068 6173 6174 7472 2866 6967 2c20  if hasattr(fig, 
-000292e0: 2774 6974 6c65 2729 3a0a 2020 2020 2020  'title'):.      
-000292f0: 2020 2020 2020 6361 6e76 6173 2e74 6974        canvas.tit
-00029300: 6c65 203d 2066 6967 2e74 6974 6c65 0a0a  le = fig.title..
-00029310: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00029320: 616e 7661 730a 0a20 2020 2064 6566 205f  anvas..    def _
-00029330: 6765 745f 646c 675f 6672 6f6d 5f6d 706c  get_dlg_from_mpl
-00029340: 2873 656c 662c 2066 6967 293a 0a20 2020  (self, fig):.   
-00029350: 2020 2020 2063 616e 7661 7320 3d20 7365       canvas = se
-00029360: 6c66 2e5f 6765 745f 7769 6467 6574 5f66  lf._get_widget_f
-00029370: 726f 6d5f 6d70 6c28 6669 6729 0a20 2020  rom_mpl(fig).   
-00029380: 2020 2020 2023 2050 6173 7320 7769 6e64       # Pass wind
-00029390: 6f77 2074 6974 6c65 2061 6e64 2066 6967  ow title and fig
-000293a0: 5f6e 616d 6520 6f6e 0a20 2020 2020 2020  _name on.       
-000293b0: 2069 6620 6861 7361 7474 7228 6361 6e76   if hasattr(canv
-000293c0: 6173 2c20 2766 6967 5f6e 616d 6527 293a  as, 'fig_name'):
-000293d0: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-000293e0: 6520 3d20 6361 6e76 6173 2e66 6967 5f6e  e = canvas.fig_n
-000293f0: 616d 650a 2020 2020 2020 2020 656c 7365  ame.        else
-00029400: 3a0a 2020 2020 2020 2020 2020 2020 6e61  :.            na
-00029410: 6d65 203d 204e 6f6e 650a 2020 2020 2020  me = None.      
-00029420: 2020 6966 2068 6173 6174 7472 2863 616e    if hasattr(can
-00029430: 7661 732c 2027 7469 746c 6527 293a 0a20  vas, 'title'):. 
-00029440: 2020 2020 2020 2020 2020 2074 6974 6c65             title
-00029450: 203d 2063 616e 7661 732e 7469 746c 650a   = canvas.title.
-00029460: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00029470: 2020 2020 2020 2020 2020 7469 746c 6520            title 
-00029480: 3d20 4e6f 6e65 0a20 2020 2020 2020 2064  = None.        d
-00029490: 6c67 203d 205f 4261 7365 4469 616c 6f67  lg = _BaseDialog
-000294a0: 2873 656c 662c 2077 6964 6765 743d 6361  (self, widget=ca
-000294b0: 6e76 6173 2c20 7469 746c 653d 7469 746c  nvas, title=titl
-000294c0: 652c 206e 616d 653d 6e61 6d65 290a 2020  e, name=name).  
-000294d0: 2020 2020 2020 646c 672e 7368 6f77 2829        dlg.show()
-000294e0: 0a0a 2020 2020 6465 6620 5f63 7265 6174  ..    def _creat
-000294f0: 655f 6368 5f63 6f6e 7465 7874 5f66 6967  e_ch_context_fig
-00029500: 2873 656c 662c 2069 6478 293a 0a20 2020  (self, idx):.   
-00029510: 2020 2020 2066 6967 203d 2073 7570 6572       fig = super
-00029520: 2829 2e5f 6372 6561 7465 5f63 685f 636f  ()._create_ch_co
-00029530: 6e74 6578 745f 6669 6728 6964 7829 0a20  ntext_fig(idx). 
-00029540: 2020 2020 2020 2069 6620 6669 6720 6973         if fig is
-00029550: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00029560: 2020 2020 2020 2073 656c 662e 5f67 6574         self._get
-00029570: 5f64 6c67 5f66 726f 6d5f 6d70 6c28 6669  _dlg_from_mpl(fi
-00029580: 6729 0a0a 2020 2020 6465 6620 5f74 6f67  g)..    def _tog
-00029590: 676c 655f 6570 6f63 685f 6869 7374 6f67  gle_epoch_histog
-000295a0: 7261 6d6d 2873 656c 6629 3a0a 2020 2020  ramm(self):.    
-000295b0: 2020 2020 6966 2073 656c 662e 6d6e 652e      if self.mne.
-000295c0: 6973 5f65 706f 6368 733a 0a20 2020 2020  is_epochs:.     
-000295d0: 2020 2020 2020 2066 6967 203d 2073 656c         fig = sel
-000295e0: 662e 5f63 7265 6174 655f 6570 6f63 685f  f._create_epoch_
-000295f0: 6869 7374 6f67 7261 6d28 290a 2020 2020  histogram().    
-00029600: 2020 2020 2020 2020 6966 2066 6967 2069          if fig i
-00029610: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00029620: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00029630: 2e5f 6765 745f 646c 675f 6672 6f6d 5f6d  ._get_dlg_from_m
-00029640: 706c 2866 6967 290a 0a20 2020 2064 6566  pl(fig)..    def
-00029650: 205f 6372 6561 7465 5f73 656c 6563 7469   _create_selecti
-00029660: 6f6e 5f66 6967 2873 656c 6629 3a0a 2020  on_fig(self):.  
-00029670: 2020 2020 2020 6966 206e 6f74 2061 6e79        if not any
-00029680: 285b 6973 696e 7374 616e 6365 2866 6967  ([isinstance(fig
-00029690: 2c20 5365 6c65 6374 696f 6e44 6961 6c6f  , SelectionDialo
-000296a0: 6729 2066 6f72 0a20 2020 2020 2020 2020  g) for.         
-000296b0: 2020 2020 2020 2020 2020 2066 6967 2069             fig i
-000296c0: 6e20 7365 6c66 2e6d 6e65 2e63 6869 6c64  n self.mne.child
-000296d0: 5f66 6967 735d 293a 0a20 2020 2020 2020  _figs]):.       
-000296e0: 2020 2020 2053 656c 6563 7469 6f6e 4469       SelectionDi
-000296f0: 616c 6f67 2873 656c 6629 0a0a 2020 2020  alog(self)..    
-00029700: 6465 6620 6d65 7373 6167 655f 626f 7828  def message_box(
-00029710: 7365 6c66 2c20 7465 7874 2c20 696e 666f  self, text, info
-00029720: 5f74 6578 743d 4e6f 6e65 2c20 6275 7474  _text=None, butt
-00029730: 6f6e 733d 4e6f 6e65 2c0a 2020 2020 2020  ons=None,.      
-00029740: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00029750: 6661 756c 745f 6275 7474 6f6e 3d4e 6f6e  fault_button=Non
-00029760: 652c 2069 636f 6e3d 4e6f 6e65 2c20 6d6f  e, icon=None, mo
-00029770: 6461 6c3d 5472 7565 293a 2020 2320 6e6f  dal=True):  # no
-00029780: 7161 3a20 4431 3032 0a20 2020 2020 2020  qa: D102.       
-00029790: 2073 656c 662e 6d73 675f 626f 782e 7365   self.msg_box.se
-000297a0: 7454 6578 7428 6627 3c66 6f6e 7420 7369  tText(f'<font si
-000297b0: 7a65 3d22 2b32 223e 3c62 3e7b 7465 7874  ze="+2"><b>{text
-000297c0: 7d3c 2f62 3e3c 2f66 6f6e 743e 2729 0a20  }</b></font>'). 
-000297d0: 2020 2020 2020 2069 6620 696e 666f 5f74         if info_t
-000297e0: 6578 7420 6973 206e 6f74 204e 6f6e 653a  ext is not None:
-000297f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00029800: 662e 6d73 675f 626f 782e 7365 7449 6e66  f.msg_box.setInf
-00029810: 6f72 6d61 7469 7665 5465 7874 2869 6e66  ormativeText(inf
-00029820: 6f5f 7465 7874 290a 2020 2020 2020 2020  o_text).        
-00029830: 6966 2062 7574 746f 6e73 2069 7320 6e6f  if buttons is no
-00029840: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00029850: 2020 2020 7365 6c66 2e6d 7367 5f62 6f78      self.msg_box
-00029860: 2e73 6574 5374 616e 6461 7264 4275 7474  .setStandardButt
-00029870: 6f6e 7328 6275 7474 6f6e 7329 0a20 2020  ons(buttons).   
-00029880: 2020 2020 2069 6620 6465 6661 756c 745f       if default_
-00029890: 6275 7474 6f6e 2069 7320 6e6f 7420 4e6f  button is not No
-000298a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000298b0: 7365 6c66 2e6d 7367 5f62 6f78 2e73 6574  self.msg_box.set
-000298c0: 4465 6661 756c 7442 7574 746f 6e28 6465  DefaultButton(de
-000298d0: 6661 756c 745f 6275 7474 6f6e 290a 2020  fault_button).  
-000298e0: 2020 2020 2020 6966 2069 636f 6e20 6973        if icon is
-000298f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00029900: 2020 2020 2020 2073 656c 662e 6d73 675f         self.msg_
-00029910: 626f 782e 7365 7449 636f 6e28 6963 6f6e  box.setIcon(icon
-00029920: 290a 0a20 2020 2020 2020 2023 2041 6c6c  )..        # All
-00029930: 6f77 2069 6e74 6572 6163 7469 6e67 2077  ow interacting w
-00029940: 6974 6820 6d65 7373 6167 655f 626f 7820  ith message_box 
-00029950: 696e 2074 6573 742d 6d6f 6465 2e0a 2020  in test-mode..  
-00029960: 2020 2020 2020 2320 5365 7420 6d6f 6461        # Set moda
-00029970: 6c3d 4661 6c73 6520 6f6e 6c79 2069 6620  l=False only if 
-00029980: 6e6f 2072 6574 7572 6e20 7661 6c75 6520  no return value 
-00029990: 6973 2065 7870 6563 7465 642e 0a20 2020  is expected..   
-000299a0: 2020 2020 2073 656c 662e 6d73 675f 626f       self.msg_bo
-000299b0: 782e 7365 744d 6f64 616c 2846 616c 7365  x.setModal(False
-000299c0: 2069 6620 7365 6c66 2e74 6573 745f 6d6f   if self.test_mo
-000299d0: 6465 2065 6c73 6520 6d6f 6461 6c29 0a20  de else modal). 
-000299e0: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-000299f0: 6573 745f 6d6f 6465 206f 7220 6e6f 7420  est_mode or not 
-00029a00: 6d6f 6461 6c3a 0a20 2020 2020 2020 2020  modal:.         
-00029a10: 2020 2073 656c 662e 6d73 675f 626f 782e     self.msg_box.
-00029a20: 7368 6f77 2829 0a20 2020 2020 2020 2065  show().        e
-00029a30: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00029a40: 2072 6574 7572 6e20 7365 6c66 2e6d 7367   return self.msg
-00029a50: 5f62 6f78 2e65 7865 6328 290a 0a20 2020  _box.exec()..   
-00029a60: 2064 6566 206b 6579 5072 6573 7345 7665   def keyPressEve
-00029a70: 6e74 2873 656c 662c 2065 7665 6e74 293a  nt(self, event):
-00029a80: 0a20 2020 2020 2020 2022 2222 4375 7374  .        """Cust
-00029a90: 6f6d 697a 6520 6b65 7920 7072 6573 7320  omize key press 
-00029aa0: 6576 656e 7473 2e22 2222 0a20 2020 2020  events.""".     
-00029ab0: 2020 2023 204f 6e20 4d61 634f 7320 6164     # On MacOs ad
-00029ac0: 6469 7469 6f6e 616c 6c79 204b 6579 7061  ditionally Keypa
-00029ad0: 644d 6f64 6966 6965 7220 6973 2073 6574  dModifier is set
-00029ae0: 2077 6865 6e20 6172 726f 772d 6b65 7973   when arrow-keys
-00029af0: 0a20 2020 2020 2020 2023 2061 7265 2070  .        # are p
-00029b00: 7265 7373 6564 2e0a 2020 2020 2020 2020  ressed..        
-00029b10: 6d6f 6473 203d 2065 7665 6e74 2e6d 6f64  mods = event.mod
-00029b20: 6966 6965 7273 2829 0a20 2020 2020 2020  ifiers().       
-00029b30: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00029b40: 2020 6d6f 6473 203d 2069 6e74 286d 6f64    mods = int(mod
-00029b50: 7329 2020 2320 5079 5174 203c 2035 2e31  s)  # PyQt < 5.1
-00029b60: 330a 2020 2020 2020 2020 6578 6365 7074  3.        except
-00029b70: 2045 7863 6570 7469 6f6e 3a0a 2020 2020   Exception:.    
-00029b80: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-00029b90: 2020 2020 206d 6f64 6966 6965 7273 203d       modifiers =
-00029ba0: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-00029bb0: 5368 6966 7427 3a20 626f 6f6c 2851 742e  Shift': bool(Qt.
-00029bc0: 5368 6966 744d 6f64 6966 6965 7220 2620  ShiftModifier & 
-00029bd0: 6d6f 6473 292c 0a20 2020 2020 2020 2020  mods),.         
-00029be0: 2020 2027 4374 726c 273a 2062 6f6f 6c28     'Ctrl': bool(
-00029bf0: 5174 2e43 6f6e 7472 6f6c 4d6f 6469 6669  Qt.ControlModifi
-00029c00: 6572 2026 206d 6f64 7329 2c0a 2020 2020  er & mods),.    
-00029c10: 2020 2020 7d0a 2020 2020 2020 2020 666f      }.        fo
-00029c20: 7220 6b65 795f 6e61 6d65 2069 6e20 7365  r key_name in se
-00029c30: 6c66 2e6d 6e65 2e6b 6579 626f 6172 645f  lf.mne.keyboard_
-00029c40: 7368 6f72 7463 7574 733a 0a20 2020 2020  shortcuts:.     
-00029c50: 2020 2020 2020 206b 6579 5f64 6963 7420         key_dict 
-00029c60: 3d20 7365 6c66 2e6d 6e65 2e6b 6579 626f  = self.mne.keybo
-00029c70: 6172 645f 7368 6f72 7463 7574 735b 6b65  ard_shortcuts[ke
-00029c80: 795f 6e61 6d65 5d0a 2020 2020 2020 2020  y_name].        
-00029c90: 2020 2020 6966 206b 6579 5f64 6963 745b      if key_dict[
-00029ca0: 2771 745f 6b65 7927 5d20 3d3d 2065 7665  'qt_key'] == eve
-00029cb0: 6e74 2e6b 6579 2829 2061 6e64 2027 736c  nt.key() and 'sl
-00029cc0: 6f74 2720 696e 206b 6579 5f64 6963 743a  ot' in key_dict:
-00029cd0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00029ce0: 2020 6d6f 645f 6964 7820 3d20 300a 2020    mod_idx = 0.  
-00029cf0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00029d00: 4765 7420 6d6f 6469 6669 6572 0a20 2020  Get modifier.   
-00029d10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00029d20: 276d 6f64 6966 6965 7227 2069 6e20 6b65  'modifier' in ke
-00029d30: 795f 6469 6374 3a0a 2020 2020 2020 2020  y_dict:.        
-00029d40: 2020 2020 2020 2020 2020 2020 6d6f 6473              mods
-00029d50: 203d 205b 6d6f 6469 6669 6572 735b 6d6f   = [modifiers[mo
-00029d60: 645d 2066 6f72 206d 6f64 2069 6e20 6d6f  d] for mod in mo
-00029d70: 6469 6669 6572 735d 0a20 2020 2020 2020  difiers].       
-00029d80: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00029d90: 616e 7928 6d6f 6473 293a 0a20 2020 2020  any(mods):.     
-00029da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029db0: 2020 2023 204e 6f20 6d75 6c74 6970 6c65     # No multiple
-00029dc0: 206d 6f64 6966 6965 7273 2073 7570 706f   modifiers suppo
-00029dd0: 7274 6564 2079 6574 0a20 2020 2020 2020  rted yet.       
-00029de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029df0: 206d 6f64 203d 205b 6d6f 6420 666f 7220   mod = [mod for 
-00029e00: 6d6f 6420 696e 206d 6f64 6966 6965 7273  mod in modifiers
-00029e10: 2069 6620 6d6f 6469 6669 6572 735b 6d6f   if modifiers[mo
-00029e20: 645d 5d5b 305d 0a20 2020 2020 2020 2020  d]][0].         
-00029e30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00029e40: 6620 6d6f 6420 696e 206b 6579 5f64 6963  f mod in key_dic
-00029e50: 745b 276d 6f64 6966 6965 7227 5d3a 0a20  t['modifier']:. 
-00029e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029e70: 2020 2020 2020 2020 2020 206d 6f64 5f69             mod_i
-00029e80: 6478 203d 206b 6579 5f64 6963 745b 276d  dx = key_dict['m
-00029e90: 6f64 6966 6965 7227 5d2e 696e 6465 7828  odifier'].index(
-00029ea0: 6d6f 6429 0a0a 2020 2020 2020 2020 2020  mod)..          
-00029eb0: 2020 2020 2020 736c 6f74 5f69 6478 203d        slot_idx =
-00029ec0: 206d 6f64 5f69 6478 2069 6620 6d6f 645f   mod_idx if mod_
-00029ed0: 6964 7820 3c20 6c65 6e28 6b65 795f 6469  idx < len(key_di
-00029ee0: 6374 5b27 736c 6f74 275d 2920 656c 7365  ct['slot']) else
-00029ef0: 2030 0a20 2020 2020 2020 2020 2020 2020   0.             
-00029f00: 2020 2073 6c6f 7420 3d20 6b65 795f 6469     slot = key_di
-00029f10: 6374 5b27 736c 6f74 275d 5b73 6c6f 745f  ct['slot'][slot_
-00029f20: 6964 785d 0a0a 2020 2020 2020 2020 2020  idx]..          
-00029f30: 2020 2020 2020 6966 2027 7061 7261 6d65        if 'parame
-00029f40: 7465 7227 2069 6e20 6b65 795f 6469 6374  ter' in key_dict
-00029f50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00029f60: 2020 2020 2020 7061 7261 6d5f 6964 7820        param_idx 
-00029f70: 3d20 286d 6f64 5f69 6478 2069 6620 6d6f  = (mod_idx if mo
-00029f80: 645f 6964 7820 3c0a 2020 2020 2020 2020  d_idx <.        
-00029f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029fa0: 2020 2020 2020 2020 206c 656e 286b 6579           len(key
-00029fb0: 5f64 6963 745b 2770 6172 616d 6574 6572  _dict['parameter
-00029fc0: 275d 2920 656c 7365 2030 290a 2020 2020  ']) else 0).    
-00029fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029fe0: 7661 6c20 3d20 6b65 795f 6469 6374 5b27  val = key_dict['
-00029ff0: 7061 7261 6d65 7465 7227 5d5b 7061 7261  parameter'][para
-0002a000: 6d5f 6964 785d 0a20 2020 2020 2020 2020  m_idx].         
-0002a010: 2020 2020 2020 2020 2020 2069 6620 276b             if 'k
-0002a020: 7727 2069 6e20 6b65 795f 6469 6374 3a0a  w' in key_dict:.
-0002a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a040: 2020 2020 2020 2020 736c 6f74 282a 2a7b          slot(**{
-0002a050: 6b65 795f 6469 6374 5b27 6b77 275d 3a20  key_dict['kw']: 
-0002a060: 7661 6c7d 290a 2020 2020 2020 2020 2020  val}).          
-0002a070: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0002a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a090: 2020 2020 2020 2020 736c 6f74 2876 616c          slot(val
-0002a0a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002a0b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0002a0c0: 2020 2020 2020 2020 2020 2020 736c 6f74              slot
-0002a0d0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-0002a0e0: 2020 2020 6272 6561 6b0a 0a20 2020 2064      break..    d
-0002a0f0: 6566 205f 6472 6177 5f74 7261 6365 7328  ef _draw_traces(
-0002a100: 7365 6c66 293a 0a20 2020 2020 2020 2023  self):.        #
-0002a110: 2055 7064 6174 6520 6461 7461 2069 6e20   Update data in 
-0002a120: 7472 6163 6573 2028 3d64 7261 7769 6e67  traces (=drawing
-0002a130: 2074 7261 6365 7329 0a20 2020 2020 2020   traces).       
-0002a140: 2066 6f72 2074 7261 6365 2069 6e20 7365   for trace in se
-0002a150: 6c66 2e6d 6e65 2e74 7261 6365 733a 0a20  lf.mne.traces:. 
-0002a160: 2020 2020 2020 2020 2020 2023 2055 7064             # Upd
-0002a170: 6174 6520 6461 7461 0a20 2020 2020 2020  ate data.       
-0002a180: 2020 2020 2074 7261 6365 2e75 7064 6174       trace.updat
-0002a190: 655f 6461 7461 2829 0a0a 2020 2020 6465  e_data()..    de
-0002a1a0: 6620 5f67 6574 5f73 697a 6528 7365 6c66  f _get_size(self
-0002a1b0: 293a 0a20 2020 2020 2020 2069 6e63 685f  ):.        inch_
-0002a1c0: 7769 6474 6820 3d20 7365 6c66 2e77 6964  width = self.wid
-0002a1d0: 7468 2829 202f 2073 656c 662e 6c6f 6769  th() / self.logi
-0002a1e0: 6361 6c44 7069 5828 290a 2020 2020 2020  calDpiX().      
-0002a1f0: 2020 696e 6368 5f68 6569 6768 7420 3d20    inch_height = 
-0002a200: 7365 6c66 2e68 6569 6768 7428 2920 2f20  self.height() / 
-0002a210: 7365 6c66 2e6c 6f67 6963 616c 4470 6959  self.logicalDpiY
-0002a220: 2829 0a0a 2020 2020 2020 2020 7265 7475  ()..        retu
-0002a230: 726e 2069 6e63 685f 7769 6474 682c 2069  rn inch_width, i
-0002a240: 6e63 685f 6865 6967 6874 0a0a 2020 2020  nch_height..    
-0002a250: 6465 6620 5f66 616b 655f 6b65 7970 7265  def _fake_keypre
-0002a260: 7373 2873 656c 662c 206b 6579 2c20 6669  ss(self, key, fi
-0002a270: 673d 4e6f 6e65 293a 0a20 2020 2020 2020  g=None):.       
-0002a280: 2066 6967 203d 2066 6967 206f 7220 7365   fig = fig or se
-0002a290: 6c66 0a0a 2020 2020 2020 2020 6966 206b  lf..        if k
-0002a2a0: 6579 2e69 7375 7070 6572 2829 3a0a 2020  ey.isupper():.  
-0002a2b0: 2020 2020 2020 2020 2020 6b65 7920 3d20            key = 
-0002a2c0: 6b65 792e 6c6f 7765 7228 290a 2020 2020  key.lower().    
-0002a2d0: 2020 2020 2020 2020 6d6f 6469 6669 6572          modifier
-0002a2e0: 203d 2051 742e 5368 6966 744d 6f64 6966   = Qt.ShiftModif
-0002a2f0: 6965 720a 2020 2020 2020 2020 656c 6966  ier.        elif
-0002a300: 206b 6579 2e73 7461 7274 7377 6974 6828   key.startswith(
-0002a310: 2773 6869 6674 2b27 293a 0a20 2020 2020  'shift+'):.     
-0002a320: 2020 2020 2020 206b 6579 203d 206b 6579         key = key
-0002a330: 5b36 3a5d 0a20 2020 2020 2020 2020 2020  [6:].           
-0002a340: 206d 6f64 6966 6965 7220 3d20 5174 2e53   modifier = Qt.S
-0002a350: 6869 6674 4d6f 6469 6669 6572 0a20 2020  hiftModifier.   
-0002a360: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0002a370: 2020 2020 2020 206d 6f64 6966 6965 7220         modifier 
-0002a380: 3d20 5174 2e4e 6f4d 6f64 6966 6965 720a  = Qt.NoModifier.
-0002a390: 0a20 2020 2020 2020 2023 2055 7365 2070  .        # Use p
-0002a3a0: 7974 6573 742d 7174 2773 2065 7863 6570  ytest-qt's excep
-0002a3b0: 7469 6f6e 2d68 6f6f 6b0a 2020 2020 2020  tion-hook.      
-0002a3c0: 2020 7769 7468 2063 6170 7475 7265 5f65    with capture_e
-0002a3d0: 7863 6570 7469 6f6e 7328 2920 6173 2065  xceptions() as e
-0002a3e0: 7863 6570 7469 6f6e 733a 0a20 2020 2020  xceptions:.     
-0002a3f0: 2020 2020 2020 2051 5465 7374 2e6b 6579         QTest.key
-0002a400: 5072 6573 7328 6669 672c 2073 656c 662e  Press(fig, self.
-0002a410: 6d6e 652e 6b65 7962 6f61 7264 5f73 686f  mne.keyboard_sho
-0002a420: 7274 6375 7473 5b6b 6579 5d5b 2771 745f  rtcuts[key]['qt_
-0002a430: 6b65 7927 5d2c 0a20 2020 2020 2020 2020  key'],.         
-0002a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a450: 2020 6d6f 6469 6669 6572 290a 0a20 2020    modifier)..   
-0002a460: 2020 2020 2066 6f72 2065 7863 2069 6e20       for exc in 
-0002a470: 6578 6365 7074 696f 6e73 3a0a 2020 2020  exceptions:.    
-0002a480: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
-0002a490: 6e74 696d 6545 7272 6f72 2866 2754 6865  ntimeError(f'The
-0002a4a0: 7265 2061 7320 6265 656e 2061 6e20 7b65  re as been an {e
-0002a4b0: 7863 5b30 5d7d 2069 6e73 6964 6520 7468  xc[0]} inside th
-0002a4c0: 6520 5174 2027 0a20 2020 2020 2020 2020  e Qt '.         
-0002a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a4e0: 2020 2020 2020 6627 6576 656e 7420 6c6f        f'event lo
-0002a4f0: 6f70 2028 6c6f 6f6b 2061 626f 7665 2066  op (look above f
-0002a500: 6f72 2074 7261 6365 6261 636b 292e 2729  or traceback).')
-0002a510: 0a0a 2020 2020 6465 6620 5f66 616b 655f  ..    def _fake_
-0002a520: 636c 6963 6b28 7365 6c66 2c20 706f 696e  click(self, poin
-0002a530: 742c 2061 6464 5f70 6f69 6e74 733d 4e6f  t, add_points=No
-0002a540: 6e65 2c20 6669 673d 4e6f 6e65 2c20 6178  ne, fig=None, ax
-0002a550: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-0002a560: 2020 2020 2020 2020 2020 2078 666f 726d             xform
-0002a570: 3d27 6178 272c 2062 7574 746f 6e3d 312c  ='ax', button=1,
-0002a580: 206b 696e 643d 2770 7265 7373 2729 3a0a   kind='press'):.
-0002a590: 2020 2020 2020 2020 6164 645f 706f 696e          add_poin
-0002a5a0: 7473 203d 2061 6464 5f70 6f69 6e74 7320  ts = add_points 
-0002a5b0: 6f72 206c 6973 7428 290a 2020 2020 2020  or list().      
-0002a5c0: 2020 2320 5761 6974 2075 6e74 696c 2057    # Wait until W
-0002a5d0: 696e 646f 7720 6973 2066 756c 6c79 2073  indow is fully s
-0002a5e0: 686f 776e 2e0a 2020 2020 2020 2020 5154  hown..        QT
-0002a5f0: 6573 742e 7157 6169 7446 6f72 5769 6e64  est.qWaitForWind
-0002a600: 6f77 4578 706f 7365 6428 7365 6c66 290a  owExposed(self).
-0002a610: 2020 2020 2020 2020 2320 5363 656e 652d          # Scene-
-0002a620: 4469 6d65 6e73 696f 6e73 2073 7469 6c6c  Dimensions still
-0002a630: 2073 6565 6d20 746f 2063 6861 6e67 6520   seem to change 
-0002a640: 746f 2066 696e 616c 2073 7461 7465 2077  to final state w
-0002a650: 6865 6e20 7761 6974 696e 670a 2020 2020  hen waiting.    
-0002a660: 2020 2020 2320 666f 7220 6120 7368 6f72      # for a shor
-0002a670: 7420 7469 6d65 2e0a 2020 2020 2020 2020  t time..        
-0002a680: 5154 6573 742e 7157 6169 7428 3130 290a  QTest.qWait(10).
-0002a690: 0a20 2020 2020 2020 2023 2051 743a 2072  .        # Qt: r
-0002a6a0: 6967 6874 2d62 7574 746f 6e3d 322c 206d  ight-button=2, m
-0002a6b0: 6174 706c 6f74 6c69 623a 2072 6967 6874  atplotlib: right
-0002a6c0: 2d62 7574 746f 6e3d 330a 2020 2020 2020  -button=3.      
-0002a6d0: 2020 6966 2062 7574 746f 6e20 3d3d 2031    if button == 1
-0002a6e0: 3a0a 2020 2020 2020 2020 2020 2020 6275  :.            bu
-0002a6f0: 7474 6f6e 203d 2051 742e 4c65 6674 4275  tton = Qt.LeftBu
-0002a700: 7474 6f6e 0a20 2020 2020 2020 2065 6c73  tton.        els
-0002a710: 653a 0a20 2020 2020 2020 2020 2020 2062  e:.            b
-0002a720: 7574 746f 6e20 3d20 5174 2e52 6967 6874  utton = Qt.Right
-0002a730: 4275 7474 6f6e 0a0a 2020 2020 2020 2020  Button..        
-0002a740: 2320 466f 7220 5174 2c20 6669 6720 6f72  # For Qt, fig or
-0002a750: 2061 7820 626f 7468 2077 6f75 6c64 2062   ax both would b
-0002a760: 6520 7468 6520 7769 6467 6574 2074 6f20  e the widget to 
-0002a770: 7465 7374 2069 6e74 6572 6163 7469 6f6e  test interaction
-0002a780: 206f 6e2e 0a20 2020 2020 2020 2023 2049   on..        # I
-0002a790: 6620 5669 6577 0a20 2020 2020 2020 2066  f View.        f
-0002a7a0: 6967 203d 2061 7820 6f72 2066 6967 206f  ig = ax or fig o
-0002a7b0: 7220 7365 6c66 2e6d 6e65 2e76 6965 770a  r self.mne.view.
-0002a7c0: 0a20 2020 2020 2020 2069 6620 7866 6f72  .        if xfor
-0002a7d0: 6d20 3d3d 2027 6178 273a 0a20 2020 2020  m == 'ax':.     
-0002a7e0: 2020 2020 2020 2023 2046 6f72 2051 742c         # For Qt,
-0002a7f0: 2074 6865 2065 7175 6976 616c 656e 7420   the equivalent 
-0002a800: 6f66 206d 6174 706c 6f74 6c69 6273 2074  of matplotlibs t
-0002a810: 7261 6e73 4178 6573 0a20 2020 2020 2020  ransAxes.       
-0002a820: 2020 2020 2023 2077 6f75 6c64 2062 6520       # would be 
-0002a830: 6120 7472 616e 7366 6f72 6d61 7469 6f6e  a transformation
-0002a840: 2074 6f20 5669 6577 2043 6f6f 7264 696e   to View Coordin
-0002a850: 6174 6573 2e0a 2020 2020 2020 2020 2020  ates..          
-0002a860: 2020 2320 4275 7420 666f 7220 7468 6520    # But for the 
-0002a870: 5669 6577 2074 6f70 2d6c 6566 7420 6973  View top-left is
-0002a880: 2028 302c 2030 2920 616e 6420 626f 7474   (0, 0) and bott
-0002a890: 6f6d 2d72 6967 6874 2069 730a 2020 2020  om-right is.    
-0002a8a0: 2020 2020 2020 2020 2320 2876 6965 772d          # (view-
-0002a8b0: 7769 6474 682c 2076 6965 772d 6865 6967  width, view-heig
-0002a8c0: 6874 292e 0a20 2020 2020 2020 2020 2020  ht)..           
-0002a8d0: 2076 6965 775f 7769 6474 6820 3d20 6669   view_width = fi
-0002a8e0: 672e 7769 6474 6828 290a 2020 2020 2020  g.width().      
-0002a8f0: 2020 2020 2020 7669 6577 5f68 6569 6768        view_heigh
-0002a900: 7420 3d20 6669 672e 6865 6967 6874 2829  t = fig.height()
-0002a910: 0a20 2020 2020 2020 2020 2020 2078 203d  .            x =
-0002a920: 2076 6965 775f 7769 6474 6820 2a20 706f   view_width * po
-0002a930: 696e 745b 305d 0a20 2020 2020 2020 2020  int[0].         
-0002a940: 2020 2079 203d 2076 6965 775f 6865 6967     y = view_heig
-0002a950: 6874 202a 2028 3120 2d20 706f 696e 745b  ht * (1 - point[
-0002a960: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
-0002a970: 706f 696e 7420 3d20 506f 696e 7428 782c  point = Point(x,
-0002a980: 2079 290a 2020 2020 2020 2020 2020 2020   y).            
-0002a990: 666f 7220 6964 782c 2061 706f 696e 7420  for idx, apoint 
-0002a9a0: 696e 2065 6e75 6d65 7261 7465 2861 6464  in enumerate(add
-0002a9b0: 5f70 6f69 6e74 7329 3a0a 2020 2020 2020  _points):.      
-0002a9c0: 2020 2020 2020 2020 2020 7832 203d 2076            x2 = v
-0002a9d0: 6965 775f 7769 6474 6820 2a20 6170 6f69  iew_width * apoi
-0002a9e0: 6e74 5b30 5d0a 2020 2020 2020 2020 2020  nt[0].          
-0002a9f0: 2020 2020 2020 7932 203d 2076 6965 775f        y2 = view_
-0002aa00: 6865 6967 6874 202a 2028 3120 2d20 6170  height * (1 - ap
-0002aa10: 6f69 6e74 5b31 5d29 0a20 2020 2020 2020  oint[1]).       
-0002aa20: 2020 2020 2020 2020 2061 6464 5f70 6f69           add_poi
-0002aa30: 6e74 735b 6964 785d 203d 2050 6f69 6e74  nts[idx] = Point
-0002aa40: 2878 322c 2079 3229 0a0a 2020 2020 2020  (x2, y2)..      
-0002aa50: 2020 656c 6966 2078 666f 726d 203d 3d20    elif xform == 
-0002aa60: 2764 6174 6127 3a0a 2020 2020 2020 2020  'data':.        
-0002aa70: 2020 2020 2320 466f 7220 5174 2c20 7468      # For Qt, th
-0002aa80: 6520 6571 7569 7661 6c65 6e74 206f 6620  e equivalent of 
-0002aa90: 6d61 7470 6c6f 746c 6962 7320 7472 616e  matplotlibs tran
-0002aaa0: 7344 6174 610a 2020 2020 2020 2020 2020  sData.          
-0002aab0: 2020 2320 776f 756c 6420 6265 2061 2074    # would be a t
-0002aac0: 7261 6e73 666f 726d 6174 696f 6e20 746f  ransformation to
-0002aad0: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
-0002aae0: 6865 2063 6f6f 7264 696e 6174 6520 7379  he coordinate sy
-0002aaf0: 7374 656d 206f 6620 7468 6520 5669 6577  stem of the View
-0002ab00: 426f 782e 0a20 2020 2020 2020 2020 2020  Box..           
-0002ab10: 2023 2054 6869 7320 6f6e 6c79 2077 6f72   # This only wor
-0002ab20: 6b73 206f 6e20 7468 6520 5669 6577 2028  ks on the View (
-0002ab30: 7365 6c66 2e6d 6e65 2e76 6965 7729 0a20  self.mne.view). 
-0002ab40: 2020 2020 2020 2020 2020 2066 6967 203d             fig =
-0002ab50: 2073 656c 662e 6d6e 652e 7669 6577 0a20   self.mne.view. 
-0002ab60: 2020 2020 2020 2020 2020 2070 6f69 6e74             point
-0002ab70: 203d 2073 656c 662e 6d6e 652e 7669 6577   = self.mne.view
-0002ab80: 626f 782e 6d61 7056 6965 7754 6f53 6365  box.mapViewToSce
-0002ab90: 6e65 2850 6f69 6e74 282a 706f 696e 7429  ne(Point(*point)
-0002aba0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-0002abb0: 7220 6964 782c 2061 706f 696e 7420 696e  r idx, apoint in
-0002abc0: 2065 6e75 6d65 7261 7465 2861 6464 5f70   enumerate(add_p
-0002abd0: 6f69 6e74 7329 3a0a 2020 2020 2020 2020  oints):.        
-0002abe0: 2020 2020 2020 2020 6164 645f 706f 696e          add_poin
-0002abf0: 7473 5b69 6478 5d20 3d20 7365 6c66 2e6d  ts[idx] = self.m
-0002ac00: 6e65 2e76 6965 7762 6f78 2e6d 6170 5669  ne.viewbox.mapVi
-0002ac10: 6577 546f 5363 656e 6528 0a20 2020 2020  ewToScene(.     
-0002ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ac30: 2020 2050 6f69 6e74 282a 6170 6f69 6e74     Point(*apoint
-0002ac40: 2929 0a0a 2020 2020 2020 2020 656c 6966  ))..        elif
-0002ac50: 2078 666f 726d 203d 3d20 276e 6f6e 6527   xform == 'none'
-0002ac60: 206f 7220 7866 6f72 6d20 6973 204e 6f6e   or xform is Non
-0002ac70: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-0002ac80: 6620 6973 696e 7374 616e 6365 2870 6f69  f isinstance(poi
-0002ac90: 6e74 2c20 2874 7570 6c65 2c20 6c69 7374  nt, (tuple, list
-0002aca0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-0002acb0: 2020 2020 706f 696e 7420 3d20 506f 696e      point = Poin
-0002acc0: 7428 2a70 6f69 6e74 290a 2020 2020 2020  t(*point).      
-0002acd0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0002ace0: 2020 2020 2020 2020 2020 2020 706f 696e              poin
-0002acf0: 7420 3d20 506f 696e 7428 706f 696e 7429  t = Point(point)
-0002ad00: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0002ad10: 2069 6478 2c20 6170 6f69 6e74 2069 6e20   idx, apoint in 
-0002ad20: 656e 756d 6572 6174 6528 6164 645f 706f  enumerate(add_po
-0002ad30: 696e 7473 293a 0a20 2020 2020 2020 2020  ints):.         
-0002ad40: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-0002ad50: 616e 6365 2861 706f 696e 742c 2028 7475  ance(apoint, (tu
-0002ad60: 706c 652c 206c 6973 7429 293a 0a20 2020  ple, list)):.   
-0002ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ad80: 2061 6464 5f70 6f69 6e74 735b 6964 785d   add_points[idx]
-0002ad90: 203d 2050 6f69 6e74 282a 6170 6f69 6e74   = Point(*apoint
-0002ada0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0002adb0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0002adc0: 2020 2020 2020 2020 2020 2020 6164 645f              add_
-0002add0: 706f 696e 7473 5b69 6478 5d20 3d20 506f  points[idx] = Po
-0002ade0: 696e 7428 6170 6f69 6e74 290a 0a20 2020  int(apoint)..   
-0002adf0: 2020 2020 2023 2055 7365 2070 7974 6573       # Use pytes
-0002ae00: 742d 7174 2773 2065 7863 6570 7469 6f6e  t-qt's exception
-0002ae10: 2d68 6f6f 6b0a 2020 2020 2020 2020 7769  -hook.        wi
-0002ae20: 7468 2063 6170 7475 7265 5f65 7863 6570  th capture_excep
-0002ae30: 7469 6f6e 7328 2920 6173 2065 7863 6570  tions() as excep
-0002ae40: 7469 6f6e 733a 0a20 2020 2020 2020 2020  tions:.         
-0002ae50: 2020 2077 6964 6765 7420 3d20 6669 672e     widget = fig.
-0002ae60: 7669 6577 706f 7274 2829 2069 6620 6973  viewport() if is
-0002ae70: 696e 7374 616e 6365 2866 6967 2c20 5147  instance(fig, QG
-0002ae80: 7261 7068 6963 7356 6965 7729 2065 6c73  raphicsView) els
-0002ae90: 6520 6669 670a 2020 2020 2020 2020 2020  e fig.          
-0002aea0: 2020 6966 206b 696e 6420 3d3d 2027 7072    if kind == 'pr
-0002aeb0: 6573 7327 3a0a 2020 2020 2020 2020 2020  ess':.          
-0002aec0: 2020 2020 2020 2320 616c 7761 7973 2063        # always c
-0002aed0: 6c69 636b 2062 6563 6175 7365 206d 6f73  lick because mos
-0002aee0: 7420 696e 7465 7261 6374 6976 6974 7920  t interactivity 
-0002aef0: 636f 6d65 7320 666f 726d 0a20 2020 2020  comes form.     
-0002af00: 2020 2020 2020 2020 2020 2023 206d 6f75             # mou
-0002af10: 7365 436c 6963 6b45 7665 6e74 2066 726f  seClickEvent fro
-0002af20: 6d20 7079 7174 6772 6170 6820 286a 7573  m pyqtgraph (jus
-0002af30: 7420 7072 6573 7320 646f 6573 6e27 7420  t press doesn't 
-0002af40: 7375 6666 6963 650a 2020 2020 2020 2020  suffice.        
-0002af50: 2020 2020 2020 2020 2320 6865 7265 292e          # here).
-0002af60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002af70: 205f 6d6f 7573 6543 6c69 636b 2877 6964   _mouseClick(wid
-0002af80: 6765 743d 7769 6467 6574 2c20 706f 733d  get=widget, pos=
-0002af90: 706f 696e 742c 2062 7574 746f 6e3d 6275  point, button=bu
-0002afa0: 7474 6f6e 290a 2020 2020 2020 2020 2020  tton).          
-0002afb0: 2020 656c 6966 206b 696e 6420 3d3d 2027    elif kind == '
-0002afc0: 7265 6c65 6173 6527 3a0a 2020 2020 2020  release':.      
-0002afd0: 2020 2020 2020 2020 2020 5f6d 6f75 7365            _mouse
-0002afe0: 5265 6c65 6173 6528 7769 6467 6574 3d77  Release(widget=w
-0002aff0: 6964 6765 742c 2070 6f73 3d70 6f69 6e74  idget, pos=point
-0002b000: 2c20 6275 7474 6f6e 3d62 7574 746f 6e29  , button=button)
-0002b010: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-0002b020: 6620 6b69 6e64 203d 3d20 276d 6f74 696f  f kind == 'motio
-0002b030: 6e27 3a0a 2020 2020 2020 2020 2020 2020  n':.            
-0002b040: 2020 2020 5f6d 6f75 7365 4d6f 7665 2877      _mouseMove(w
-0002b050: 6964 6765 743d 7769 6467 6574 2c20 706f  idget=widget, po
-0002b060: 733d 706f 696e 742c 2062 7574 746f 6e73  s=point, buttons
-0002b070: 3d62 7574 746f 6e29 0a20 2020 2020 2020  =button).       
-0002b080: 2020 2020 2065 6c69 6620 6b69 6e64 203d       elif kind =
-0002b090: 3d20 2764 7261 6727 3a0a 2020 2020 2020  = 'drag':.      
-0002b0a0: 2020 2020 2020 2020 2020 5f6d 6f75 7365            _mouse
-0002b0b0: 4472 6167 2877 6964 6765 743d 7769 6467  Drag(widget=widg
-0002b0c0: 6574 2c20 706f 7369 7469 6f6e 733d 5b70  et, positions=[p
-0002b0d0: 6f69 6e74 5d20 2b20 6164 645f 706f 696e  oint] + add_poin
-0002b0e0: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-0002b0f0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0002b100: 7574 746f 6e3d 6275 7474 6f6e 290a 0a20  utton=button).. 
-0002b110: 2020 2020 2020 2066 6f72 2065 7863 2069         for exc i
-0002b120: 6e20 6578 6365 7074 696f 6e73 3a0a 2020  n exceptions:.  
-0002b130: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0002b140: 5275 6e74 696d 6545 7272 6f72 2866 2754  RuntimeError(f'T
-0002b150: 6865 7265 2061 7320 6265 656e 2061 6e20  here as been an 
-0002b160: 7b65 7863 5b30 5d7d 2069 6e73 6964 6520  {exc[0]} inside 
-0002b170: 7468 6520 5174 2027 0a20 2020 2020 2020  the Qt '.       
-0002b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b190: 2020 2020 2020 2020 6627 6576 656e 7420          f'event 
-0002b1a0: 6c6f 6f70 2028 6c6f 6f6b 2061 626f 7665  loop (look above
-0002b1b0: 2066 6f72 2074 7261 6365 6261 636b 292e   for traceback).
-0002b1c0: 2729 0a0a 2020 2020 2020 2020 2320 5761  ')..        # Wa
-0002b1d0: 6974 696e 6720 736f 6d65 2074 696d 6520  iting some time 
-0002b1e0: 666f 7220 6576 656e 7473 2074 6f20 6265  for events to be
-0002b1f0: 2070 726f 6365 7373 6564 2e0a 2020 2020   processed..    
-0002b200: 2020 2020 5154 6573 742e 7157 6169 7428      QTest.qWait(
-0002b210: 3530 290a 0a20 2020 2064 6566 205f 6661  50)..    def _fa
-0002b220: 6b65 5f73 6372 6f6c 6c28 7365 6c66 2c20  ke_scroll(self, 
-0002b230: 782c 2079 2c20 7374 6570 2c20 6669 673d  x, y, step, fig=
-0002b240: 4e6f 6e65 293a 0a20 2020 2020 2020 2023  None):.        #
-0002b250: 2051 5465 7374 2064 6f65 736e 2774 2073   QTest doesn't s
-0002b260: 7570 706f 7274 2073 696d 756c 6174 696e  upport simulatin
-0002b270: 6720 7363 726f 6c6c 696e 672d 7768 6565  g scrolling-whee
-0002b280: 6c0a 2020 2020 2020 2020 7365 6c66 2e76  l.        self.v
-0002b290: 7363 726f 6c6c 2873 7465 7029 0a0a 2020  scroll(step)..  
-0002b2a0: 2020 6465 6620 5f63 6c69 636b 5f63 685f    def _click_ch_
-0002b2b0: 6e61 6d65 2873 656c 662c 2063 685f 696e  name(self, ch_in
-0002b2c0: 6465 782c 2062 7574 746f 6e29 3a0a 2020  dex, button):.  
-0002b2d0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e63        self.mne.c
-0002b2e0: 6861 6e6e 656c 5f61 7869 732e 7265 7061  hannel_axis.repa
-0002b2f0: 696e 7428 290a 2020 2020 2020 2020 2320  int().        # 
-0002b300: 5761 6974 2062 6563 6175 7365 2063 6861  Wait because cha
-0002b310: 6e6e 656c 2d61 7869 7320 6d61 7920 6e65  nnel-axis may ne
-0002b320: 6564 2074 696d 650a 2020 2020 2020 2020  ed time.        
-0002b330: 2320 2863 616d 6520 7570 2077 6974 6820  # (came up with 
-0002b340: 7465 7374 5f65 706f 6368 733a 3a74 6573  test_epochs::tes
-0002b350: 745f 706c 6f74 5f65 706f 6368 735f 636c  t_plot_epochs_cl
-0002b360: 6963 6b73 290a 2020 2020 2020 2020 5154  icks).        QT
-0002b370: 6573 742e 7157 6169 7428 3130 3029 0a20  est.qWait(100). 
-0002b380: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0002b390: 6c66 2e6d 6e65 2e62 7574 7465 7266 6c79  lf.mne.butterfly
-0002b3a0: 3a0a 2020 2020 2020 2020 2020 2020 6368  :.            ch
-0002b3b0: 5f6e 616d 6520 3d20 7365 6c66 2e6d 6e65  _name = self.mne
-0002b3c0: 2e63 685f 6e61 6d65 735b 7365 6c66 2e6d  .ch_names[self.m
-0002b3d0: 6e65 2e70 6963 6b73 5b63 685f 696e 6465  ne.picks[ch_inde
-0002b3e0: 785d 5d0a 2020 2020 2020 2020 2020 2020  x]].            
-0002b3f0: 7872 616e 6765 2c20 7972 616e 6765 203d  xrange, yrange =
-0002b400: 2073 656c 662e 6d6e 652e 6368 616e 6e65   self.mne.channe
-0002b410: 6c5f 6178 6973 2e63 685f 7465 7874 735b  l_axis.ch_texts[
-0002b420: 6368 5f6e 616d 655d 0a20 2020 2020 2020  ch_name].       
-0002b430: 2020 2020 2078 203d 206e 702e 6d65 616e       x = np.mean
-0002b440: 2878 7261 6e67 6529 0a20 2020 2020 2020  (xrange).       
-0002b450: 2020 2020 2079 203d 206e 702e 6d65 616e       y = np.mean
-0002b460: 2879 7261 6e67 6529 0a0a 2020 2020 2020  (yrange)..      
-0002b470: 2020 2020 2020 7365 6c66 2e5f 6661 6b65        self._fake
-0002b480: 5f63 6c69 636b 2828 782c 2079 292c 2066  _click((x, y), f
-0002b490: 6967 3d73 656c 662e 6d6e 652e 7669 6577  ig=self.mne.view
-0002b4a0: 2c20 6275 7474 6f6e 3d62 7574 746f 6e2c  , button=button,
-0002b4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b4c0: 2020 2020 2020 2020 2020 2020 2020 7866                xf
-0002b4d0: 6f72 6d3d 276e 6f6e 6527 290a 0a20 2020  orm='none')..   
-0002b4e0: 2064 6566 205f 7265 7369 7a65 5f62 795f   def _resize_by_
-0002b4f0: 6661 6374 6f72 2873 656c 662c 2066 6163  factor(self, fac
-0002b500: 746f 7229 3a0a 2020 2020 2020 2020 7061  tor):.        pa
-0002b510: 7373 0a0a 2020 2020 6465 6620 5f67 6574  ss..    def _get
-0002b520: 5f74 6963 6b6c 6162 656c 7328 7365 6c66  _ticklabels(self
-0002b530: 2c20 6f72 6965 6e74 6174 696f 6e29 3a0a  , orientation):.
-0002b540: 2020 2020 2020 2020 6966 206f 7269 656e          if orien
-0002b550: 7461 7469 6f6e 203d 3d20 2778 273a 0a20  tation == 'x':. 
-0002b560: 2020 2020 2020 2020 2020 2061 7820 3d20             ax = 
-0002b570: 7365 6c66 2e6d 6e65 2e74 696d 655f 6178  self.mne.time_ax
-0002b580: 6973 0a20 2020 2020 2020 2065 6c73 653a  is.        else:
-0002b590: 0a20 2020 2020 2020 2020 2020 2061 7820  .            ax 
-0002b5a0: 3d20 7365 6c66 2e6d 6e65 2e63 6861 6e6e  = self.mne.chann
-0002b5b0: 656c 5f61 7869 730a 0a20 2020 2020 2020  el_axis..       
-0002b5c0: 2072 6574 7572 6e20 6c69 7374 2861 782e   return list(ax.
-0002b5d0: 6765 745f 6c61 6265 6c73 2829 290a 0a20  get_labels()).. 
-0002b5e0: 2020 2064 6566 205f 6765 745f 7363 616c     def _get_scal
-0002b5f0: 655f 6261 725f 7465 7874 7328 7365 6c66  e_bar_texts(self
-0002b600: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-0002b610: 6e20 7475 706c 6528 742e 746f 506c 6169  n tuple(t.toPlai
-0002b620: 6e54 6578 7428 2920 666f 7220 7420 696e  nText() for t in
-0002b630: 2073 656c 662e 6d6e 652e 7363 616c 6562   self.mne.scaleb
-0002b640: 6172 5f74 6578 7473 2e76 616c 7565 7328  ar_texts.values(
-0002b650: 2929 0a0a 2020 2020 6465 6620 7368 6f77  ))..    def show
-0002b660: 2873 656c 6629 3a20 2023 206e 6f71 613a  (self):  # noqa:
-0002b670: 2044 3130 320a 2020 2020 2020 2020 2320   D102.        # 
-0002b680: 5365 7420 7261 6973 655f 7769 6e64 6f77  Set raise_window
-0002b690: 206c 696b 6520 6d61 7470 6c6f 746c 6962   like matplotlib
-0002b6a0: 2069 6620 706f 7373 6962 6c65 0a20 2020   if possible.   
-0002b6b0: 2020 2020 2073 7570 6572 2829 2e73 686f       super().sho
-0002b6c0: 7728 290a 2020 2020 2020 2020 5f71 745f  w().        _qt_
-0002b6d0: 7261 6973 655f 7769 6e64 6f77 2873 656c  raise_window(sel
-0002b6e0: 6629 0a0a 2020 2020 6465 6620 5f63 6c6f  f)..    def _clo
-0002b6f0: 7365 5f65 7665 6e74 2873 656c 662c 2066  se_event(self, f
-0002b700: 6967 3d4e 6f6e 6529 3a0a 2020 2020 2020  ig=None):.      
-0002b710: 2020 2222 2246 6f72 6365 2063 616c 6c69    """Force calli
-0002b720: 6e67 206f 6620 7468 6520 4d50 4c20 6669  ng of the MPL fi
-0002b730: 6775 7265 2063 6c6f 7365 2065 7665 6e74  gure close event
-0002b740: 2e22 2222 0a20 2020 2020 2020 2066 6967  .""".        fig
-0002b750: 203d 2066 6967 206f 7220 7365 6c66 0a20   = fig or self. 
-0002b760: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
-0002b770: 7228 6669 672c 2027 6361 6e76 6173 2729  r(fig, 'canvas')
-0002b780: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-0002b790: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0002b7a0: 2020 2066 6967 2e63 616e 7661 732e 636c     fig.canvas.cl
-0002b7b0: 6f73 655f 6576 656e 7428 290a 2020 2020  ose_event().    
-0002b7c0: 2020 2020 2020 2020 6578 6365 7074 2056          except V
-0002b7d0: 616c 7565 4572 726f 723a 2020 2320 6f6c  alueError:  # ol
-0002b7e0: 6420 6d70 6c20 7769 7468 2051 740a 2020  d mpl with Qt.  
-0002b7f0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0002b800: 7373 2020 2320 7072 6167 6d61 3a20 6e6f  ss  # pragma: no
-0002b810: 2063 6f76 6572 0a20 2020 2020 2020 2065   cover.        e
-0002b820: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0002b830: 2066 6967 2e63 6c6f 7365 2829 0a0a 2020   fig.close()..  
-0002b840: 2020 6465 6620 5f63 6865 636b 5f63 6c6f    def _check_clo
-0002b850: 7365 2873 656c 6629 3a0a 2020 2020 2020  se(self):.      
-0002b860: 2020 2222 2243 6c6f 7365 2061 6e6e 6f74    """Close annot
-0002b870: 6174 696f 6e73 2d6d 6f64 6520 6265 666f  ations-mode befo
-0002b880: 7265 2063 6c6f 7369 6e67 2074 6865 2062  re closing the b
-0002b890: 726f 7773 6572 2e22 2222 0a20 2020 2020  rowser.""".     
-0002b8a0: 2020 2069 6620 7365 6c66 2e6d 6e65 2e61     if self.mne.a
-0002b8b0: 6e6e 6f74 6174 696f 6e5f 6d6f 6465 3a0a  nnotation_mode:.
-0002b8c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002b8d0: 2e5f 746f 6767 6c65 5f61 6e6e 6f74 6174  ._toggle_annotat
-0002b8e0: 696f 6e5f 6669 6728 290a 2020 2020 2020  ion_fig().      
-0002b8f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0002b900: 2020 2020 7365 6c66 2e63 6c6f 7365 2829      self.close()
-0002b910: 0a0a 2020 2020 6465 6620 636c 6f73 6545  ..    def closeE
-0002b920: 7665 6e74 2873 656c 662c 2065 7665 6e74  vent(self, event
-0002b930: 293a 0a20 2020 2020 2020 2022 2222 4375  ):.        """Cu
-0002b940: 7374 6f6d 697a 6520 636c 6f73 6520 6576  stomize close ev
-0002b950: 656e 742e 2222 220a 2020 2020 2020 2020  ent.""".        
-0002b960: 6576 656e 742e 6163 6365 7074 2829 0a20  event.accept(). 
-0002b970: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
-0002b980: 7228 7365 6c66 2c20 276d 6e65 2729 3a0a  r(self, 'mne'):.
-0002b990: 2020 2020 2020 2020 2020 2020 2320 4578              # Ex
-0002b9a0: 706c 6963 6974 2064 6973 636f 6e6e 6563  plicit disconnec
-0002b9b0: 7473 2074 6f20 6176 6f69 6420 7265 6665  ts to avoid refe
-0002b9c0: 7265 6e63 6520 6379 636c 6573 2074 6861  rence cycles tha
-0002b9d0: 7420 6763 2063 616e 2774 0a20 2020 2020  t gc can't.     
-0002b9e0: 2020 2020 2020 2023 2070 726f 7065 726c         # properl
-0002b9f0: 7920 7265 736f 6c76 6520 2829 0a20 2020  y resolve ().   
-0002ba00: 2020 2020 2020 2020 2069 6620 6861 7361           if hasa
-0002ba10: 7474 7228 7365 6c66 2e6d 6e65 2c20 2770  ttr(self.mne, 'p
-0002ba20: 6c74 2729 3a0a 2020 2020 2020 2020 2020  lt'):.          
-0002ba30: 2020 2020 2020 5f64 6973 636f 6e6e 6563        _disconnec
-0002ba40: 7428 7365 6c66 2e6d 6e65 2e70 6c74 2e73  t(self.mne.plt.s
-0002ba50: 6967 5852 616e 6765 4368 616e 6765 6429  igXRangeChanged)
-0002ba60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002ba70: 205f 6469 7363 6f6e 6e65 6374 2873 656c   _disconnect(sel
-0002ba80: 662e 6d6e 652e 706c 742e 7369 6759 5261  f.mne.plt.sigYRa
-0002ba90: 6e67 6543 6861 6e67 6564 290a 2020 2020  ngeChanged).    
-0002baa0: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
-0002bab0: 7472 2873 656c 662e 6d6e 652c 2027 746f  tr(self.mne, 'to
-0002bac0: 6f6c 6261 7227 293a 0a20 2020 2020 2020  olbar'):.       
-0002bad0: 2020 2020 2020 2020 2066 6f72 2061 6374           for act
-0002bae0: 696f 6e20 696e 2073 656c 662e 6d6e 652e  ion in self.mne.
-0002baf0: 746f 6f6c 6261 722e 6163 7469 6f6e 7328  toolbar.actions(
-0002bb00: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0002bb10: 2020 2020 2020 2061 6c6c 6f77 5f65 7272         allow_err
-0002bb20: 6f72 203d 2061 6374 696f 6e2e 7465 7874  or = action.text
-0002bb30: 2829 203d 3d20 2727 0a20 2020 2020 2020  () == ''.       
-0002bb40: 2020 2020 2020 2020 2020 2020 205f 6469               _di
-0002bb50: 7363 6f6e 6e65 6374 2861 6374 696f 6e2e  sconnect(action.
-0002bb60: 7472 6967 6765 7265 642c 2061 6c6c 6f77  triggered, allow
-0002bb70: 5f65 7272 6f72 3d61 6c6c 6f77 5f65 7272  _error=allow_err
-0002bb80: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
-0002bb90: 2320 5361 7665 2073 6574 7469 6e67 7320  # Save settings 
-0002bba0: 676f 696e 6720 696e 746f 2051 5365 7474  going into QSett
-0002bbb0: 696e 6773 2e0a 2020 2020 2020 2020 2020  ings..          
-0002bbc0: 2020 666f 7220 7173 6574 7469 6e67 2069    for qsetting i
-0002bbd0: 6e20 7173 6574 7469 6e67 735f 7061 7261  n qsettings_para
-0002bbe0: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-0002bbf0: 2020 2020 7661 6c75 6520 3d20 6765 7461      value = geta
-0002bc00: 7474 7228 7365 6c66 2e6d 6e65 2c20 7173  ttr(self.mne, qs
-0002bc10: 6574 7469 6e67 290a 2020 2020 2020 2020  etting).        
-0002bc20: 2020 2020 2020 2020 5153 6574 7469 6e67          QSetting
-0002bc30: 7328 292e 7365 7456 616c 7565 2871 7365  s().setValue(qse
-0002bc40: 7474 696e 672c 2076 616c 7565 290a 2020  tting, value).  
-0002bc50: 2020 2020 2020 2020 2020 666f 7220 6174            for at
-0002bc60: 7472 2069 6e20 2827 6b65 7962 6f61 7264  tr in ('keyboard
-0002bc70: 5f73 686f 7274 6375 7473 272c 2027 7472  _shortcuts', 'tr
-0002bc80: 6163 6573 272c 2027 706c 7427 2c20 2774  aces', 'plt', 't
-0002bc90: 6f6f 6c62 6172 272c 0a20 2020 2020 2020  oolbar',.       
-0002bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bcb0: 2020 2766 6967 5f61 6e6e 6f74 6174 696f    'fig_annotatio
-0002bcc0: 6e27 293a 0a20 2020 2020 2020 2020 2020  n'):.           
-0002bcd0: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
-0002bce0: 7365 6c66 2e6d 6e65 2c20 6174 7472 293a  self.mne, attr):
-0002bcf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002bd00: 2020 2020 2064 656c 6174 7472 2873 656c       delattr(sel
-0002bd10: 662e 6d6e 652c 2061 7474 7229 0a20 2020  f.mne, attr).   
-0002bd20: 2020 2020 2020 2020 2069 6620 6861 7361           if hasa
-0002bd30: 7474 7228 7365 6c66 2e6d 6e65 2c20 2763  ttr(self.mne, 'c
-0002bd40: 6869 6c64 5f66 6967 7327 293a 0a20 2020  hild_figs'):.   
-0002bd50: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0002bd60: 2066 6967 2069 6e20 7365 6c66 2e6d 6e65   fig in self.mne
-0002bd70: 2e63 6869 6c64 5f66 6967 733a 0a20 2020  .child_figs:.   
-0002bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bd90: 2066 6967 2e63 6c6f 7365 2829 0a20 2020   fig.close().   
-0002bda0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0002bdb0: 662e 6d6e 652e 6368 696c 645f 6669 6773  f.mne.child_figs
-0002bdc0: 2e63 6c65 6172 2829 0a20 2020 2020 2020  .clear().       
-0002bdd0: 2020 2020 2066 6f72 2061 7474 7220 696e       for attr in
-0002bde0: 2028 2774 7261 6365 7327 2c20 2765 7665   ('traces', 'eve
-0002bdf0: 6e74 5f6c 696e 6573 272c 2027 7265 6769  nt_lines', 'regi
-0002be00: 6f6e 7327 293a 0a20 2020 2020 2020 2020  ons'):.         
-0002be10: 2020 2020 2020 2067 6574 6174 7472 2873         getattr(s
-0002be20: 656c 662e 6d6e 652c 2061 7474 722c 205b  elf.mne, attr, [
-0002be30: 5d29 2e63 6c65 6172 2829 0a20 2020 2020  ]).clear().     
-0002be40: 2020 2020 2020 2069 6620 6765 7461 7474         if getatt
-0002be50: 7228 7365 6c66 2e6d 6e65 2c20 2776 6c69  r(self.mne, 'vli
-0002be60: 6e65 272c 204e 6f6e 6529 2069 7320 6e6f  ne', None) is no
-0002be70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002be80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002be90: 6d6e 652e 6973 5f65 706f 6368 733a 0a20  mne.is_epochs:. 
-0002bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002beb0: 2020 2066 6f72 2076 6c20 696e 2073 656c     for vl in sel
-0002bec0: 662e 6d6e 652e 766c 696e 653a 0a20 2020  f.mne.vline:.   
-0002bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bee0: 2020 2020 205f 6469 7363 6f6e 6e65 6374       _disconnect
-0002bef0: 2876 6c2e 7369 6750 6f73 6974 696f 6e43  (vl.sigPositionC
-0002bf00: 6861 6e67 6546 696e 6973 6865 6429 0a20  hangeFinished). 
-0002bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bf20: 2020 2073 656c 662e 6d6e 652e 766c 696e     self.mne.vlin
-0002bf30: 652e 636c 6561 7228 290a 2020 2020 2020  e.clear().      
-0002bf40: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0002bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bf60: 2020 2020 5f64 6973 636f 6e6e 6563 7428      _disconnect(
-0002bf70: 7365 6c66 2e6d 6e65 2e76 6c69 6e65 2e73  self.mne.vline.s
-0002bf80: 6967 506f 7369 7469 6f6e 4368 616e 6765  igPositionChange
-0002bf90: 4669 6e69 7368 6564 290a 2020 2020 2020  Finished).      
-0002bfa0: 2020 6966 2067 6574 6174 7472 2873 656c    if getattr(sel
-0002bfb0: 662c 2027 6c6f 6164 5f74 6872 6561 6427  f, 'load_thread'
-0002bfc0: 2c20 4e6f 6e65 2920 6973 206e 6f74 204e  , None) is not N
-0002bfd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002bfe0: 2073 656c 662e 6c6f 6164 5f74 6872 6561   self.load_threa
-0002bff0: 642e 636c 6561 6e28 290a 2020 2020 2020  d.clean().      
-0002c000: 2020 2020 2020 7365 6c66 2e6c 6f61 645f        self.load_
-0002c010: 7468 7265 6164 203d 204e 6f6e 650a 0a20  thread = None.. 
-0002c020: 2020 2020 2020 2023 2052 656d 6f76 6520         # Remove 
-0002c030: 7365 6c66 2066 726f 6d20 6272 6f77 7365  self from browse
-0002c040: 725f 696e 7374 616e 6365 7320 696e 2067  r_instances in g
-0002c050: 6c6f 6261 6c73 0a20 2020 2020 2020 2069  lobals.        i
-0002c060: 6620 7365 6c66 2069 6e20 5f62 726f 7773  f self in _brows
-0002c070: 6572 5f69 6e73 7461 6e63 6573 3a0a 2020  er_instances:.  
-0002c080: 2020 2020 2020 2020 2020 5f62 726f 7773            _brows
-0002c090: 6572 5f69 6e73 7461 6e63 6573 2e72 656d  er_instances.rem
-0002c0a0: 6f76 6528 7365 6c66 290a 2020 2020 2020  ove(self).      
-0002c0b0: 2020 7365 6c66 2e5f 636c 6f73 6528 6576    self._close(ev
-0002c0c0: 656e 7429 0a20 2020 2020 2020 2073 656c  ent).        sel
-0002c0d0: 662e 676f 7443 6c6f 7365 642e 656d 6974  f.gotClosed.emit
-0002c0e0: 2829 0a20 2020 2020 2020 2023 204d 616b  ().        # Mak
-0002c0f0: 6520 7375 7265 2069 7420 6765 7473 2064  e sure it gets d
-0002c100: 656c 6574 6564 2061 6674 6572 2069 7420  eleted after it 
-0002c110: 7761 7320 636c 6f73 6564 2e0a 2020 2020  was closed..    
-0002c120: 2020 2020 7365 6c66 2e64 656c 6574 654c      self.deleteL
-0002c130: 6174 6572 2829 0a20 2020 2020 2020 2073  ater().        s
-0002c140: 656c 662e 5f63 6c6f 7365 6420 3d20 5472  elf._closed = Tr
-0002c150: 7565 0a0a 2020 2020 6465 6620 5f66 616b  ue..    def _fak
-0002c160: 655f 636c 6963 6b5f 6f6e 5f74 6f6f 6c62  e_click_on_toolb
-0002c170: 6172 5f61 6374 696f 6e28 7365 6c66 2c20  ar_action(self, 
-0002c180: 6163 7469 6f6e 5f6e 616d 652c 2077 6169  action_name, wai
-0002c190: 745f 6166 7465 723d 3530 3029 3a0a 2020  t_after=500):.  
-0002c1a0: 2020 2020 2020 2222 2254 7269 6767 6572        """Trigger
-0002c1b0: 2065 7665 6e74 2061 7373 6f63 6961 7465   event associate
-0002c1c0: 6420 7769 7468 2061 6374 696f 6e20 2761  d with action 'a
-0002c1d0: 6374 696f 6e5f 6e61 6d65 2720 696e 2074  ction_name' in t
-0002c1e0: 6f6f 6c62 6172 2e22 2222 0a20 2020 2020  oolbar.""".     
-0002c1f0: 2020 2066 6f72 2061 6374 696f 6e20 696e     for action in
-0002c200: 2073 656c 662e 6d6e 652e 746f 6f6c 6261   self.mne.toolba
-0002c210: 722e 6163 7469 6f6e 7328 293a 0a20 2020  r.actions():.   
-0002c220: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0002c230: 6163 7469 6f6e 2e69 7353 6570 6172 6174  action.isSeparat
-0002c240: 6f72 2829 3a0a 2020 2020 2020 2020 2020  or():.          
-0002c250: 2020 2020 2020 6966 2061 6374 696f 6e2e        if action.
-0002c260: 6963 6f6e 5465 7874 2829 203d 3d20 6163  iconText() == ac
-0002c270: 7469 6f6e 5f6e 616d 653a 0a20 2020 2020  tion_name:.     
-0002c280: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0002c290: 6374 696f 6e2e 7472 6967 6765 7228 290a  ction.trigger().
-0002c2a0: 2020 2020 2020 2020 5154 6573 742e 7157          QTest.qW
-0002c2b0: 6169 7428 7761 6974 5f61 6674 6572 290a  ait(wait_after).
-0002c2c0: 0a0a 6465 6620 5f67 6574 5f6e 5f66 6967  ..def _get_n_fig
-0002c2d0: 7328 293a 0a20 2020 2023 2057 6169 7420  s():.    # Wait 
-0002c2e0: 666f 7220 6120 7368 6f72 7420 7469 6d65  for a short time
-0002c2f0: 2074 6f20 6c65 7420 7468 6520 5174 2d6c   to let the Qt-l
-0002c300: 6f6f 7020 636c 6561 6e20 7570 0a20 2020  oop clean up.   
-0002c310: 2051 5465 7374 2e71 5761 6974 2831 3030   QTest.qWait(100
-0002c320: 290a 2020 2020 7265 7475 726e 206c 656e  ).    return len
-0002c330: 285b 7769 6e64 6f77 2066 6f72 2077 696e  ([window for win
-0002c340: 646f 7720 696e 2051 4170 706c 6963 6174  dow in QApplicat
-0002c350: 696f 6e2e 746f 704c 6576 656c 5769 6e64  ion.topLevelWind
-0002c360: 6f77 7328 290a 2020 2020 2020 2020 2020  ows().          
-0002c370: 2020 2020 2020 6966 2077 696e 646f 772e        if window.
-0002c380: 6973 5669 7369 626c 6528 295d 290a 0a0a  isVisible()])...
-0002c390: 6465 6620 5f63 6c6f 7365 5f61 6c6c 2829  def _close_all()
-0002c3a0: 3a0a 2020 2020 6966 206c 656e 2851 4170  :.    if len(QAp
-0002c3b0: 706c 6963 6174 696f 6e2e 746f 704c 6576  plication.topLev
-0002c3c0: 656c 5769 6e64 6f77 7328 2929 203e 2030  elWindows()) > 0
-0002c3d0: 3a0a 2020 2020 2020 2020 5141 7070 6c69  :.        QAppli
-0002c3e0: 6361 7469 6f6e 2e63 6c6f 7365 416c 6c57  cation.closeAllW
-0002c3f0: 696e 646f 7773 2829 0a0a 0a23 206d 6f75  indows()...# mou
-0002c400: 7365 2074 6573 7469 6e67 2066 756e 6374  se testing funct
-0002c410: 696f 6e73 2061 6461 7074 6564 2066 726f  ions adapted fro
-0002c420: 6d20 7079 7174 6772 6170 680a 2320 2870  m pyqtgraph.# (p
-0002c430: 7971 7467 7261 7068 2e74 6573 7473 2e75  yqtgraph.tests.u
-0002c440: 695f 7465 7374 696e 672e 7079 290a 6465  i_testing.py).de
-0002c450: 6620 5f6d 6f75 7365 5072 6573 7328 7769  f _mousePress(wi
-0002c460: 6467 6574 2c20 706f 732c 2062 7574 746f  dget, pos, butto
-0002c470: 6e2c 206d 6f64 6966 6965 723d 4e6f 6e65  n, modifier=None
-0002c480: 293a 0a20 2020 2069 6620 6d6f 6469 6669  ):.    if modifi
-0002c490: 6572 2069 7320 4e6f 6e65 3a0a 2020 2020  er is None:.    
-0002c4a0: 2020 2020 6d6f 6469 6669 6572 203d 2051      modifier = Q
-0002c4b0: 742e 4b65 7962 6f61 7264 4d6f 6469 6669  t.KeyboardModifi
-0002c4c0: 6572 2e4e 6f4d 6f64 6966 6965 720a 2020  er.NoModifier.  
-0002c4d0: 2020 6576 656e 7420 3d20 514d 6f75 7365    event = QMouse
-0002c4e0: 4576 656e 7428 5145 7665 6e74 2e54 7970  Event(QEvent.Typ
-0002c4f0: 652e 4d6f 7573 6542 7574 746f 6e50 7265  e.MouseButtonPre
-0002c500: 7373 2c20 706f 732c 2062 7574 746f 6e2c  ss, pos, button,
-0002c510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002c520: 2020 2020 2020 2020 2051 742e 4d6f 7573           Qt.Mous
-0002c530: 6542 7574 746f 6e2e 4e6f 4275 7474 6f6e  eButton.NoButton
-0002c540: 2c20 6d6f 6469 6669 6572 290a 2020 2020  , modifier).    
-0002c550: 5141 7070 6c69 6361 7469 6f6e 2e73 656e  QApplication.sen
-0002c560: 6445 7665 6e74 2877 6964 6765 742c 2065  dEvent(widget, e
-0002c570: 7665 6e74 290a 0a0a 6465 6620 5f6d 6f75  vent)...def _mou
-0002c580: 7365 5265 6c65 6173 6528 7769 6467 6574  seRelease(widget
-0002c590: 2c20 706f 732c 2062 7574 746f 6e2c 206d  , pos, button, m
-0002c5a0: 6f64 6966 6965 723d 4e6f 6e65 293a 0a20  odifier=None):. 
-0002c5b0: 2020 2069 6620 6d6f 6469 6669 6572 2069     if modifier i
-0002c5c0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0002c5d0: 6d6f 6469 6669 6572 203d 2051 742e 4b65  modifier = Qt.Ke
-0002c5e0: 7962 6f61 7264 4d6f 6469 6669 6572 2e4e  yboardModifier.N
-0002c5f0: 6f4d 6f64 6966 6965 720a 2020 2020 6576  oModifier.    ev
-0002c600: 656e 7420 3d20 514d 6f75 7365 4576 656e  ent = QMouseEven
-0002c610: 7428 5145 7665 6e74 2e54 7970 652e 4d6f  t(QEvent.Type.Mo
-0002c620: 7573 6542 7574 746f 6e52 656c 6561 7365  useButtonRelease
-0002c630: 2c20 706f 732c 0a20 2020 2020 2020 2020  , pos,.         
-0002c640: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0002c650: 7574 746f 6e2c 2051 742e 4d6f 7573 6542  utton, Qt.MouseB
-0002c660: 7574 746f 6e2e 4e6f 4275 7474 6f6e 2c20  utton.NoButton, 
-0002c670: 6d6f 6469 6669 6572 290a 2020 2020 5141  modifier).    QA
-0002c680: 7070 6c69 6361 7469 6f6e 2e73 656e 6445  pplication.sendE
-0002c690: 7665 6e74 2877 6964 6765 742c 2065 7665  vent(widget, eve
-0002c6a0: 6e74 290a 0a0a 6465 6620 5f6d 6f75 7365  nt)...def _mouse
-0002c6b0: 4d6f 7665 2877 6964 6765 742c 2070 6f73  Move(widget, pos
-0002c6c0: 2c20 6275 7474 6f6e 733d 4e6f 6e65 2c20  , buttons=None, 
-0002c6d0: 6d6f 6469 6669 6572 3d4e 6f6e 6529 3a0a  modifier=None):.
-0002c6e0: 2020 2020 6966 2062 7574 746f 6e73 2069      if buttons i
-0002c6f0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0002c700: 6275 7474 6f6e 7320 3d20 5174 2e4d 6f75  buttons = Qt.Mou
-0002c710: 7365 4275 7474 6f6e 2e4e 6f42 7574 746f  seButton.NoButto
-0002c720: 6e0a 2020 2020 6966 206d 6f64 6966 6965  n.    if modifie
-0002c730: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
-0002c740: 2020 206d 6f64 6966 6965 7220 3d20 5174     modifier = Qt
-0002c750: 2e4b 6579 626f 6172 644d 6f64 6966 6965  .KeyboardModifie
-0002c760: 722e 4e6f 4d6f 6469 6669 6572 0a20 2020  r.NoModifier.   
-0002c770: 2065 7665 6e74 203d 2051 4d6f 7573 6545   event = QMouseE
-0002c780: 7665 6e74 2851 4576 656e 742e 5479 7065  vent(QEvent.Type
-0002c790: 2e4d 6f75 7365 4d6f 7665 2c20 706f 732c  .MouseMove, pos,
-0002c7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002c7b0: 2020 2020 2020 2020 2051 742e 4d6f 7573           Qt.Mous
-0002c7c0: 6542 7574 746f 6e2e 4e6f 4275 7474 6f6e  eButton.NoButton
-0002c7d0: 2c20 6275 7474 6f6e 732c 206d 6f64 6966  , buttons, modif
-0002c7e0: 6965 7229 0a20 2020 2051 4170 706c 6963  ier).    QApplic
-0002c7f0: 6174 696f 6e2e 7365 6e64 4576 656e 7428  ation.sendEvent(
-0002c800: 7769 6467 6574 2c20 6576 656e 7429 0a0a  widget, event)..
-0002c810: 0a64 6566 205f 6d6f 7573 6543 6c69 636b  .def _mouseClick
-0002c820: 2877 6964 6765 742c 2070 6f73 2c20 6275  (widget, pos, bu
-0002c830: 7474 6f6e 2c20 6d6f 6469 6669 6572 3d4e  tton, modifier=N
-0002c840: 6f6e 6529 3a0a 2020 2020 5f6d 6f75 7365  one):.    _mouse
-0002c850: 4d6f 7665 2877 6964 6765 742c 2070 6f73  Move(widget, pos
-0002c860: 290a 2020 2020 5f6d 6f75 7365 5072 6573  ).    _mousePres
-0002c870: 7328 7769 6467 6574 2c20 706f 732c 2062  s(widget, pos, b
-0002c880: 7574 746f 6e2c 206d 6f64 6966 6965 7229  utton, modifier)
-0002c890: 0a20 2020 205f 6d6f 7573 6552 656c 6561  .    _mouseRelea
-0002c8a0: 7365 2877 6964 6765 742c 2070 6f73 2c20  se(widget, pos, 
-0002c8b0: 6275 7474 6f6e 2c20 6d6f 6469 6669 6572  button, modifier
-0002c8c0: 290a 0a0a 6465 6620 5f6d 6f75 7365 4472  )...def _mouseDr
-0002c8d0: 6167 2877 6964 6765 742c 2070 6f73 6974  ag(widget, posit
-0002c8e0: 696f 6e73 2c20 6275 7474 6f6e 2c20 6d6f  ions, button, mo
-0002c8f0: 6469 6669 6572 3d4e 6f6e 6529 3a0a 2020  difier=None):.  
-0002c900: 2020 5f6d 6f75 7365 4d6f 7665 2877 6964    _mouseMove(wid
-0002c910: 6765 742c 2070 6f73 6974 696f 6e73 5b30  get, positions[0
-0002c920: 5d29 0a20 2020 205f 6d6f 7573 6550 7265  ]).    _mousePre
-0002c930: 7373 2877 6964 6765 742c 2070 6f73 6974  ss(widget, posit
-0002c940: 696f 6e73 5b30 5d2c 2062 7574 746f 6e2c  ions[0], button,
-0002c950: 206d 6f64 6966 6965 7229 0a20 2020 2023   modifier).    #
-0002c960: 2044 656c 6179 2066 6f72 2031 3020 6d73   Delay for 10 ms
-0002c970: 2066 6f72 2064 7261 6720 746f 2062 6520   for drag to be 
-0002c980: 7265 636f 676e 697a 6564 2e0a 2020 2020  recognized..    
-0002c990: 5154 6573 742e 7157 6169 7428 3130 290a  QTest.qWait(10).
-0002c9a0: 2020 2020 666f 7220 706f 7320 696e 2070      for pos in p
-0002c9b0: 6f73 6974 696f 6e73 5b31 3a5d 3a0a 2020  ositions[1:]:.  
-0002c9c0: 2020 2020 2020 5f6d 6f75 7365 4d6f 7665        _mouseMove
-0002c9d0: 2877 6964 6765 742c 2070 6f73 2c20 6275  (widget, pos, bu
-0002c9e0: 7474 6f6e 2c20 6d6f 6469 6669 6572 290a  tton, modifier).
-0002c9f0: 2020 2020 5f6d 6f75 7365 5265 6c65 6173      _mouseReleas
-0002ca00: 6528 7769 6467 6574 2c20 706f 7369 7469  e(widget, positi
-0002ca10: 6f6e 735b 2d31 5d2c 2062 7574 746f 6e2c  ons[-1], button,
-0002ca20: 206d 6f64 6966 6965 7229 0a0a 0a23 206d   modifier)...# m
-0002ca30: 6f64 6966 6965 6420 6672 6f6d 3a20 6874  odified from: ht
-0002ca40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0002ca50: 2f70 7976 6973 7461 2f70 7976 6973 7461  /pyvista/pyvista
-0002ca60: 7174 0a64 6566 205f 7365 7475 705f 6970  qt.def _setup_ip
-0002ca70: 7974 686f 6e28 6970 7974 686f 6e3d 4e6f  ython(ipython=No
-0002ca80: 6e65 293a 0a20 2020 2023 2069 7079 7468  ne):.    # ipyth
-0002ca90: 6f6e 206d 6167 6963 0a20 2020 2069 6620  on magic.    if 
-0002caa0: 7363 6f6f 6279 2e69 6e5f 6970 7974 686f  scooby.in_ipytho
-0002cab0: 6e28 293a 0a20 2020 2020 2020 2066 726f  n():.        fro
-0002cac0: 6d20 4950 7974 686f 6e20 696d 706f 7274  m IPython import
-0002cad0: 2067 6574 5f69 7079 7468 6f6e 0a20 2020   get_ipython.   
-0002cae0: 2020 2020 2069 7079 7468 6f6e 203d 2067       ipython = g
-0002caf0: 6574 5f69 7079 7468 6f6e 2829 0a20 2020  et_ipython().   
-0002cb00: 2020 2020 2069 7079 7468 6f6e 2e72 756e       ipython.run
-0002cb10: 5f6c 696e 655f 6d61 6769 6328 2267 7569  _line_magic("gui
-0002cb20: 222c 2022 7174 2229 0a20 2020 2020 2020  ", "qt").       
-0002cb30: 2066 726f 6d20 4950 7974 686f 6e2e 6578   from IPython.ex
-0002cb40: 7465 726e 616c 2e71 745f 666f 725f 6b65  ternal.qt_for_ke
-0002cb50: 726e 656c 2069 6d70 6f72 7420 5174 4775  rnel import QtGu
-0002cb60: 690a 2020 2020 2020 2020 5174 4775 692e  i.        QtGui.
-0002cb70: 5141 7070 6c69 6361 7469 6f6e 2e69 6e73  QApplication.ins
-0002cb80: 7461 6e63 6528 290a 2020 2020 7265 7475  tance().    retu
-0002cb90: 726e 2069 7079 7468 6f6e 0a0a 0a64 6566  rn ipython...def
-0002cba0: 205f 7174 5f69 6e69 745f 6963 6f6e 7328   _qt_init_icons(
-0002cbb0: 293a 0a20 2020 2066 726f 6d20 7174 7079  ):.    from qtpy
-0002cbc0: 2e51 7447 7569 2069 6d70 6f72 7420 5149  .QtGui import QI
-0002cbd0: 636f 6e0a 2020 2020 6963 6f6e 735f 7061  con.    icons_pa
-0002cbe0: 7468 203d 2066 227b 5061 7468 285f 5f66  th = f"{Path(__f
-0002cbf0: 696c 655f 5f29 2e70 6172 656e 747d 2f69  ile__).parent}/i
-0002cc00: 636f 6e73 220a 2020 2020 5149 636f 6e2e  cons".    QIcon.
-0002cc10: 7365 7454 6865 6d65 5365 6172 6368 5061  setThemeSearchPa
-0002cc20: 7468 7328 5b69 636f 6e73 5f70 6174 685d  ths([icons_path]
-0002cc30: 290a 2020 2020 7265 7475 726e 2069 636f  ).    return ico
-0002cc40: 6e73 5f70 6174 680a 0a0a 6465 6620 5f69  ns_path...def _i
-0002cc50: 6e69 745f 6272 6f77 7365 7228 2a2a 6b77  nit_browser(**kw
-0002cc60: 6172 6773 293a 0a20 2020 205f 7365 7475  args):.    _setu
-0002cc70: 705f 6970 7974 686f 6e28 290a 2020 2020  p_ipython().    
-0002cc80: 7365 7443 6f6e 6669 674f 7074 696f 6e28  setConfigOption(
-0002cc90: 2765 6e61 626c 6545 7870 6572 696d 656e  'enableExperimen
-0002cca0: 7461 6c27 2c20 5472 7565 290a 2020 2020  tal', True).    
-0002ccb0: 6170 705f 6b77 6172 6773 203d 2064 6963  app_kwargs = dic
-0002ccc0: 7428 290a 2020 2020 6966 206b 7761 7267  t().    if kwarg
-0002ccd0: 732e 6765 7428 2773 706c 6173 6827 2c20  s.get('splash', 
-0002cce0: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
-0002ccf0: 6170 705f 6b77 6172 6773 5b27 7370 6c61  app_kwargs['spla
-0002cd00: 7368 275d 203d 2027 496e 6974 6961 6c69  sh'] = 'Initiali
-0002cd10: 7a69 6e67 206d 6e65 2d71 742d 6272 6f77  zing mne-qt-brow
-0002cd20: 7365 722e 2e2e 270a 2020 2020 6f75 7420  ser...'.    out 
-0002cd30: 3d20 5f69 6e69 745f 6d6e 655f 7174 6170  = _init_mne_qtap
-0002cd40: 7028 7067 5f61 7070 3d54 7275 652c 202a  p(pg_app=True, *
-0002cd50: 2a61 7070 5f6b 7761 7267 7329 0a20 2020  *app_kwargs).   
-0002cd60: 2069 6620 2773 706c 6173 6827 2069 6e20   if 'splash' in 
-0002cd70: 6170 705f 6b77 6172 6773 3a0a 2020 2020  app_kwargs:.    
-0002cd80: 2020 2020 6b77 6172 6773 5b27 7370 6c61      kwargs['spla
-0002cd90: 7368 275d 203d 206f 7574 5b31 5d20 2023  sh'] = out[1]  #
-0002cda0: 2072 6574 7572 6e65 6420 6173 2073 6563   returned as sec
-0002cdb0: 6f6e 6420 656c 656d 656e 740a 2020 2020  ond element.    
-0002cdc0: 6272 6f77 7365 7220 3d20 4d4e 4551 7442  browser = MNEQtB
-0002cdd0: 726f 7773 6572 282a 2a6b 7761 7267 7329  rowser(**kwargs)
-0002cde0: 0a0a 2020 2020 7265 7475 726e 2062 726f  ..    return bro
-0002cdf0: 7773 6572 0a0a 0a63 6c61 7373 2050 7951  wser...class PyQ
-0002ce00: 7447 7261 7068 4272 6f77 7365 7228 4d4e  tGraphBrowser(MN
-0002ce10: 4551 7442 726f 7773 6572 293a 2020 2320  EQtBrowser):  # 
-0002ce20: 6e6f 7161 3a20 4431 3031 0a20 2020 2070  noqa: D101.    p
-0002ce30: 6173 7320 2023 206a 7573 7420 666f 7220  ass  # just for 
-0002ce40: 6261 636b 7761 7264 2063 6f6d 7061 7420  backward compat 
-0002ce50: 7769 7468 204d 4e45 2031 2e30 2073 6372  with MNE 1.0 scr
-0002ce60: 6170 696e 670a                           aping.
+000242e0: 2076 6965 775f 7261 6e67 6520 3d20 7662   view_range = vb
+000242f0: 2e76 6965 7752 6563 7428 290a 2020 2020  .viewRect().    
+00024300: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00024310: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00024320: 2020 2020 2020 7669 6577 5f72 616e 6765        view_range
+00024330: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00024340: 2020 2020 2020 2020 6966 2076 6965 775f          if view_
+00024350: 7261 6e67 6520 6973 206e 6f74 204e 6f6e  range is not Non
+00024360: 6520 616e 6420 6c65 6e28 7365 6c66 2e6d  e and len(self.m
+00024370: 6e65 2e74 696d 6573 2920 3e20 313a 0a20  ne.times) > 1:. 
+00024380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024390: 2020 2064 7820 3d20 666c 6f61 7428 7365     dx = float(se
+000243a0: 6c66 2e6d 6e65 2e74 696d 6573 5b2d 315d  lf.mne.times[-1]
+000243b0: 202d 2073 656c 662e 6d6e 652e 7469 6d65   - self.mne.time
+000243c0: 735b 305d 2920 2f20 280a 2020 2020 2020  s[0]) / (.      
+000243d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000243e0: 2020 2020 2020 6c65 6e28 7365 6c66 2e6d        len(self.m
+000243f0: 6e65 2e74 696d 6573 2920 2d20 3129 0a20  ne.times) - 1). 
+00024400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024410: 2020 2069 6620 6478 2021 3d20 302e 303a     if dx != 0.0:
+00024420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024430: 2020 2020 2020 2020 2078 3020 3d20 7669           x0 = vi
+00024440: 6577 5f72 616e 6765 2e6c 6566 7428 2920  ew_range.left() 
+00024450: 2f20 6478 0a20 2020 2020 2020 2020 2020  / dx.           
+00024460: 2020 2020 2020 2020 2020 2020 2078 3120               x1 
+00024470: 3d20 7669 6577 5f72 616e 6765 2e72 6967  = view_range.rig
+00024480: 6874 2829 202f 2064 780a 2020 2020 2020  ht() / dx.      
+00024490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000244a0: 2020 7769 6474 6820 3d20 7662 2e77 6964    width = vb.wid
+000244b0: 7468 2829 0a20 2020 2020 2020 2020 2020  th().           
+000244c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000244d0: 7769 6474 6820 213d 2030 2e30 3a0a 2020  width != 0.0:.  
+000244e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000244f0: 2020 2020 2020 2020 2020 2320 4175 746f            # Auto
+00024500: 2d44 6f77 6e73 616d 706c 696e 6720 7769  -Downsampling wi
+00024510: 7468 2035 2073 616d 706c 6573 2070 6572  th 5 samples per
+00024520: 2070 6978 656c 0a20 2020 2020 2020 2020   pixel.         
+00024530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024540: 2020 2064 7320 3d20 696e 7428 6d61 7828     ds = int(max(
+00024550: 312c 2028 7831 202d 2078 3029 202f 2028  1, (x1 - x0) / (
+00024560: 7769 6474 6820 2a20 3529 2929 0a20 2020  width * 5))).   
+00024570: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00024580: 2020 2020 2020 2064 7320 3d20 7365 6c66         ds = self
+00024590: 2e6d 6e65 2e64 6f77 6e73 616d 706c 696e  .mne.downsamplin
+000245a0: 670a 0a20 2020 2020 2020 2023 2041 7070  g..        # App
+000245b0: 6c79 2044 6f77 6e73 616d 706c 696e 670a  ly Downsampling.
+000245c0: 2020 2020 2020 2020 6966 2064 7320 6e6f          if ds no
+000245d0: 7420 696e 205b 4e6f 6e65 2c20 315d 3a0a  t in [None, 1]:.
+000245e0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+000245f0: 7320 3d20 7365 6c66 2e6d 6e65 2e74 696d  s = self.mne.tim
+00024600: 6573 0a20 2020 2020 2020 2020 2020 2064  es.            d
+00024610: 6174 6120 3d20 7365 6c66 2e6d 6e65 2e64  ata = self.mne.d
+00024620: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
+00024630: 6e5f 6368 203d 2064 6174 612e 7368 6170  n_ch = data.shap
+00024640: 655b 305d 0a0a 2020 2020 2020 2020 2020  e[0]..          
+00024650: 2020 6966 2073 656c 662e 6d6e 652e 6473    if self.mne.ds
+00024660: 5f6d 6574 686f 6420 3d3d 2027 7375 6273  _method == 'subs
+00024670: 616d 706c 6527 3a0a 2020 2020 2020 2020  ample':.        
+00024680: 2020 2020 2020 2020 7469 6d65 7320 3d20          times = 
+00024690: 7469 6d65 735b 3a3a 6473 5d0a 2020 2020  times[::ds].    
+000246a0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+000246b0: 203d 2064 6174 615b 3a2c 203a 3a64 735d   = data[:, ::ds]
+000246c0: 0a0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+000246d0: 6966 2073 656c 662e 6d6e 652e 6473 5f6d  if self.mne.ds_m
+000246e0: 6574 686f 6420 3d3d 2027 6d65 616e 273a  ethod == 'mean':
+000246f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024700: 206e 203d 206c 656e 2874 696d 6573 2920   n = len(times) 
+00024710: 2f2f 2064 730a 2020 2020 2020 2020 2020  // ds.          
+00024720: 2020 2020 2020 2320 7374 6172 7420 6f66        # start of
+00024730: 2078 2d76 616c 7565 730a 2020 2020 2020   x-values.      
+00024740: 2020 2020 2020 2020 2020 2320 7472 7920            # try 
+00024750: 746f 2073 656c 6563 7420 6120 736f 6d65  to select a some
+00024760: 7768 6174 2063 656e 7465 7265 6420 706f  what centered po
+00024770: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+00024780: 2020 2020 7374 7820 3d20 6473 202f 2f20      stx = ds // 
+00024790: 320a 2020 2020 2020 2020 2020 2020 2020  2.              
+000247a0: 2020 7469 6d65 7320 3d20 7469 6d65 735b    times = times[
+000247b0: 7374 783a 7374 7820 2b20 6e20 2a20 6473  stx:stx + n * ds
+000247c0: 3a64 735d 0a20 2020 2020 2020 2020 2020  :ds].           
+000247d0: 2020 2020 2072 735f 6461 7461 203d 2064       rs_data = d
+000247e0: 6174 615b 3a2c 203a 6e20 2a20 6473 5d2e  ata[:, :n * ds].
+000247f0: 7265 7368 6170 6528 6e5f 6368 2c20 6e2c  reshape(n_ch, n,
+00024800: 2064 7329 0a20 2020 2020 2020 2020 2020   ds).           
+00024810: 2020 2020 2064 6174 6120 3d20 7273 5f64       data = rs_d
+00024820: 6174 612e 6d65 616e 2861 7869 733d 3229  ata.mean(axis=2)
+00024830: 0a0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00024840: 6966 2073 656c 662e 6d6e 652e 6473 5f6d  if self.mne.ds_m
+00024850: 6574 686f 6420 3d3d 2027 7065 616b 273a  ethod == 'peak':
+00024860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024870: 206e 203d 206c 656e 2874 696d 6573 2920   n = len(times) 
+00024880: 2f2f 2064 730a 2020 2020 2020 2020 2020  // ds.          
+00024890: 2020 2020 2020 2320 7374 6172 7420 6f66        # start of
+000248a0: 2078 2d76 616c 7565 730a 2020 2020 2020   x-values.      
+000248b0: 2020 2020 2020 2020 2020 2320 7472 7920            # try 
+000248c0: 746f 2073 656c 6563 7420 6120 736f 6d65  to select a some
+000248d0: 7768 6174 2063 656e 7465 7265 6420 706f  what centered po
+000248e0: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+000248f0: 2020 2020 7374 7820 3d20 6473 202f 2f20      stx = ds // 
+00024900: 320a 0a20 2020 2020 2020 2020 2020 2020  2..             
+00024910: 2020 2078 3120 3d20 6e70 2e65 6d70 7479     x1 = np.empty
+00024920: 2828 6e2c 2032 2929 0a20 2020 2020 2020  ((n, 2)).       
+00024930: 2020 2020 2020 2020 2078 315b 3a5d 203d           x1[:] =
+00024940: 2074 696d 6573 5b73 7478 3a73 7478 202b   times[stx:stx +
+00024950: 206e 202a 2064 733a 6473 2c20 6e70 2e6e   n * ds:ds, np.n
+00024960: 6577 6178 6973 5d0a 2020 2020 2020 2020  ewaxis].        
+00024970: 2020 2020 2020 2020 7469 6d65 7320 3d20          times = 
+00024980: 7831 2e72 6573 6861 7065 286e 202a 2032  x1.reshape(n * 2
+00024990: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+000249a0: 2020 2079 3120 3d20 6e70 2e65 6d70 7479     y1 = np.empty
+000249b0: 2828 6e5f 6368 2c20 6e2c 2032 2929 0a20  ((n_ch, n, 2)). 
+000249c0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+000249d0: 3220 3d20 6461 7461 5b3a 2c20 3a6e 202a  2 = data[:, :n *
+000249e0: 2064 735d 2e72 6573 6861 7065 2828 6e5f   ds].reshape((n_
+000249f0: 6368 2c20 6e2c 2064 7329 290a 2020 2020  ch, n, ds)).    
+00024a00: 2020 2020 2020 2020 2020 2020 7931 5b3a              y1[:
+00024a10: 2c20 3a2c 2030 5d20 3d20 7932 2e6d 6178  , :, 0] = y2.max
+00024a20: 2861 7869 733d 3229 0a20 2020 2020 2020  (axis=2).       
+00024a30: 2020 2020 2020 2020 2079 315b 3a2c 203a           y1[:, :
+00024a40: 2c20 315d 203d 2079 322e 6d69 6e28 6178  , 1] = y2.min(ax
+00024a50: 6973 3d32 290a 2020 2020 2020 2020 2020  is=2).          
+00024a60: 2020 2020 2020 6461 7461 203d 2079 312e        data = y1.
+00024a70: 7265 7368 6170 6528 286e 5f63 682c 206e  reshape((n_ch, n
+00024a80: 202a 2032 2929 0a0a 2020 2020 2020 2020   * 2))..        
+00024a90: 2020 2020 7365 6c66 2e6d 6e65 2e74 696d      self.mne.tim
+00024aa0: 6573 2c20 7365 6c66 2e6d 6e65 2e64 6174  es, self.mne.dat
+00024ab0: 6120 3d20 7469 6d65 732c 2064 6174 610a  a = times, data.
+00024ac0: 0a20 2020 2064 6566 205f 7368 6f77 5f70  .    def _show_p
+00024ad0: 726f 6365 7373 2873 656c 662c 206d 6573  rocess(self, mes
+00024ae0: 7361 6765 293a 0a20 2020 2020 2020 2069  sage):.        i
+00024af0: 6620 7365 6c66 2e6d 6e65 2e6c 6f61 645f  f self.mne.load_
+00024b00: 7072 6f67 7265 7373 6261 722e 6973 5669  progressbar.isVi
+00024b10: 7369 626c 6528 293a 0a20 2020 2020 2020  sible():.       
+00024b20: 2020 2020 2073 656c 662e 6d6e 652e 6c6f       self.mne.lo
+00024b30: 6164 5f70 726f 6772 6573 7362 6172 2e68  ad_progressbar.h
+00024b40: 6964 6528 290a 2020 2020 2020 2020 2020  ide().          
+00024b50: 2020 7365 6c66 2e6d 6e65 2e6c 6f61 645f    self.mne.load_
+00024b60: 7072 6f67 5f6c 6162 656c 2e68 6964 6528  prog_label.hide(
+00024b70: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00024b80: 7461 7475 7342 6172 2829 2e73 686f 774d  tatusBar().showM
+00024b90: 6573 7361 6765 286d 6573 7361 6765 290a  essage(message).
+00024ba0: 0a20 2020 2064 6566 205f 7072 6563 6f6d  .    def _precom
+00024bb0: 7075 7465 5f66 696e 6973 6865 6428 7365  pute_finished(se
+00024bc0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+00024bd0: 662e 7374 6174 7573 4261 7228 292e 7368  f.statusBar().sh
+00024be0: 6f77 4d65 7373 6167 6528 274c 6f61 6469  owMessage('Loadi
+00024bf0: 6e67 2046 696e 6973 6865 6427 2c20 3529  ng Finished', 5)
+00024c00: 0a20 2020 2020 2020 2073 656c 662e 6d6e  .        self.mn
+00024c10: 652e 6461 7461 5f70 7265 636f 6d70 7574  e.data_precomput
+00024c20: 6564 203d 2054 7275 650a 0a20 2020 2020  ed = True..     
+00024c30: 2020 2069 6620 7365 6c66 2e6d 6e65 2e6f     if self.mne.o
+00024c40: 7665 7276 6965 775f 6d6f 6465 203d 3d20  verview_mode == 
+00024c50: 277a 7363 6f72 6527 3a0a 2020 2020 2020  'zscore':.      
+00024c60: 2020 2020 2020 2320 5368 6f77 206c 6f61        # Show loa
+00024c70: 6465 6420 6f76 6572 7669 6577 2069 6d61  ded overview ima
+00024c80: 6765 0a20 2020 2020 2020 2020 2020 2073  ge.            s
+00024c90: 656c 662e 6d6e 652e 6f76 6572 7669 6577  elf.mne.overview
+00024ca0: 5f62 6172 2e73 6574 5f62 6163 6b67 726f  _bar.set_backgro
+00024cb0: 756e 6428 290a 0a20 2020 2020 2020 2069  und()..        i
+00024cc0: 6620 7365 6c66 2e5f 7265 7275 6e5f 6c6f  f self._rerun_lo
+00024cd0: 6164 5f74 6872 6561 643a 0a20 2020 2020  ad_thread:.     
+00024ce0: 2020 2020 2020 2073 656c 662e 5f72 6572         self._rer
+00024cf0: 756e 5f6c 6f61 645f 7468 7265 6164 203d  un_load_thread =
+00024d00: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+00024d10: 2020 2073 656c 662e 5f69 6e69 745f 7072     self._init_pr
+00024d20: 6563 6f6d 7075 7465 2829 0a0a 2020 2020  ecompute()..    
+00024d30: 6465 6620 5f69 6e69 745f 7072 6563 6f6d  def _init_precom
+00024d40: 7075 7465 2873 656c 6629 3a0a 2020 2020  pute(self):.    
+00024d50: 2020 2020 2320 5265 6d6f 7665 2070 7265      # Remove pre
+00024d60: 7669 6f75 736c 7920 6c6f 6164 6564 2064  viously loaded d
+00024d70: 6174 610a 2020 2020 2020 2020 7365 6c66  ata.        self
+00024d80: 2e6d 6e65 2e64 6174 615f 7072 6563 6f6d  .mne.data_precom
+00024d90: 7075 7465 6420 3d20 4661 6c73 650a 2020  puted = False.  
+00024da0: 2020 2020 2020 6966 2061 6c6c 285b 6861        if all([ha
+00024db0: 7361 7474 7228 7365 6c66 2e6d 6e65 2c20  sattr(self.mne, 
+00024dc0: 7374 290a 2020 2020 2020 2020 2020 2020  st).            
+00024dd0: 2020 2020 666f 7220 7374 2069 6e20 5b27      for st in ['
+00024de0: 676c 6f62 616c 5f64 6174 6127 2c20 2767  global_data', 'g
+00024df0: 6c6f 6261 6c5f 7469 6d65 7327 5d5d 293a  lobal_times']]):
+00024e00: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
+00024e10: 2073 656c 662e 6d6e 652e 676c 6f62 616c   self.mne.global
+00024e20: 5f64 6174 612c 2073 656c 662e 6d6e 652e  _data, self.mne.
+00024e30: 676c 6f62 616c 5f74 696d 6573 0a20 2020  global_times.   
+00024e40: 2020 2020 2067 632e 636f 6c6c 6563 7428       gc.collect(
+00024e50: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+00024e60: 6c66 2e6d 6e65 2e70 7265 636f 6d70 7574  lf.mne.precomput
+00024e70: 6520 3d3d 2027 6175 746f 273a 0a20 2020  e == 'auto':.   
+00024e80: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
+00024e90: 652e 656e 6162 6c65 5f70 7265 636f 6d70  e.enable_precomp
+00024ea0: 7574 6520 3d20 7365 6c66 2e5f 6368 6563  ute = self._chec
+00024eb0: 6b5f 7370 6163 655f 666f 725f 7072 6563  k_space_for_prec
+00024ec0: 6f6d 7075 7465 2829 0a20 2020 2020 2020  ompute().       
+00024ed0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00024ee0: 2873 656c 662e 6d6e 652e 7072 6563 6f6d  (self.mne.precom
+00024ef0: 7075 7465 2c20 626f 6f6c 293a 0a20 2020  pute, bool):.   
+00024f00: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
+00024f10: 652e 656e 6162 6c65 5f70 7265 636f 6d70  e.enable_precomp
+00024f20: 7574 6520 3d20 7365 6c66 2e6d 6e65 2e70  ute = self.mne.p
+00024f30: 7265 636f 6d70 7574 650a 0a20 2020 2020  recompute..     
+00024f40: 2020 2069 6620 7365 6c66 2e6d 6e65 2e65     if self.mne.e
+00024f50: 6e61 626c 655f 7072 6563 6f6d 7075 7465  nable_precompute
+00024f60: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00024f70: 5374 6172 7420 7072 6563 6f6d 7075 7465  Start precompute
+00024f80: 2074 6872 6561 640a 2020 2020 2020 2020   thread.        
+00024f90: 2020 2020 7365 6c66 2e6d 6e65 2e6c 6f61      self.mne.loa
+00024fa0: 645f 7072 6f67 7265 7373 6261 722e 7368  d_progressbar.sh
+00024fb0: 6f77 2829 0a20 2020 2020 2020 2020 2020  ow().           
+00024fc0: 2073 656c 662e 6d6e 652e 6c6f 6164 5f70   self.mne.load_p
+00024fd0: 726f 675f 6c61 6265 6c2e 7368 6f77 2829  rog_label.show()
+00024fe0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00024ff0: 662e 6c6f 6164 5f74 6872 6561 642e 7374  f.load_thread.st
+00025000: 6172 7428 290a 0a20 2020 2064 6566 205f  art()..    def _
+00025010: 7265 7275 6e5f 7072 6563 6f6d 7075 7465  rerun_precompute
+00025020: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00025030: 6966 2073 656c 662e 6c6f 6164 5f74 6872  if self.load_thr
+00025040: 6561 642e 6973 5275 6e6e 696e 6728 293a  ead.isRunning():
+00025050: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00025060: 662e 5f72 6572 756e 5f6c 6f61 645f 7468  f._rerun_load_th
+00025070: 7265 6164 203d 2054 7275 650a 2020 2020  read = True.    
+00025080: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00025090: 2020 2020 2020 7365 6c66 2e5f 696e 6974        self._init
+000250a0: 5f70 7265 636f 6d70 7574 6528 290a 0a20  _precompute().. 
+000250b0: 2020 2064 6566 205f 6368 6563 6b5f 7370     def _check_sp
+000250c0: 6163 655f 666f 725f 7072 6563 6f6d 7075  ace_for_precompu
+000250d0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+000250e0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000250f0: 2020 2069 6d70 6f72 7420 7073 7574 696c     import psutil
+00025100: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+00025110: 496d 706f 7274 4572 726f 723a 0a20 2020  ImportError:.   
+00025120: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00025130: 696e 666f 2827 4672 6565 2052 414d 2073  info('Free RAM s
+00025140: 7061 6365 2063 6f75 6c64 206e 6f74 2062  pace could not b
+00025150: 6520 6465 7465 726d 696e 6564 2062 6563  e determined bec
+00025160: 6175 7365 270a 2020 2020 2020 2020 2020  ause'.          
+00025170: 2020 2020 2020 2020 2020 2020 2020 2722                '"
+00025180: 7073 7574 696c 2220 6973 206e 6f74 2069  psutil" is not i
+00025190: 6e73 7461 6c6c 6564 2e20 270a 2020 2020  nstalled. '.    
+000251a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000251b0: 2020 2020 2753 6574 7469 6e67 2070 7265      'Setting pre
+000251c0: 636f 6d70 7574 6520 746f 2046 616c 7365  compute to False
+000251d0: 2e27 290a 2020 2020 2020 2020 2020 2020  .').            
+000251e0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+000251f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00025200: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00025210: 6e65 2e69 735f 6570 6f63 6873 3a0a 2020  ne.is_epochs:.  
+00025220: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00025230: 6c65 7320 3d20 5b73 656c 662e 6d6e 652e  les = [self.mne.
+00025240: 696e 7374 2e66 696c 656e 616d 655d 0a20  inst.filename]. 
+00025250: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00025260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025270: 2066 696c 6573 203d 2073 656c 662e 6d6e   files = self.mn
+00025280: 652e 696e 7374 2e66 696c 656e 616d 6573  e.inst.filenames
+00025290: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000252a0: 6669 6c65 735b 305d 2069 7320 6e6f 7420  files[0] is not 
+000252b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000252c0: 2020 2020 2020 2320 4765 7420 6469 736b        # Get disk
+000252d0: 2d73 7061 6365 206f 6620 7261 772d 6669  -space of raw-fi
+000252e0: 6c65 2873 290a 2020 2020 2020 2020 2020  le(s).          
+000252f0: 2020 2020 2020 6469 736b 5f73 7061 6365        disk_space
+00025300: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
+00025310: 2020 2020 2066 6f72 2066 6e20 696e 2066       for fn in f
+00025320: 696c 6573 3a0a 2020 2020 2020 2020 2020  iles:.          
+00025330: 2020 2020 2020 2020 2020 6469 736b 5f73            disk_s
+00025340: 7061 6365 202b 3d20 6765 7473 697a 6528  pace += getsize(
+00025350: 666e 290a 0a20 2020 2020 2020 2020 2020  fn)..           
+00025360: 2020 2020 2023 2044 6574 6572 6d69 6e65       # Determine
+00025370: 2065 7870 6563 7465 6420 5241 4d20 7370   expected RAM sp
+00025380: 6163 6520 6261 7365 6420 6f6e 206f 7269  ace based on ori
+00025390: 675f 666f 726d 6174 0a20 2020 2020 2020  g_format.       
+000253a0: 2020 2020 2020 2020 2066 6d74 5f6d 756c           fmt_mul
+000253b0: 7469 706c 6965 7273 203d 207b 2764 6f75  tipliers = {'dou
+000253c0: 626c 6527 3a20 312c 0a20 2020 2020 2020  ble': 1,.       
+000253d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000253e0: 2020 2020 2020 2020 2020 2020 2773 696e              'sin
+000253f0: 676c 6527 3a20 322c 0a20 2020 2020 2020  gle': 2,.       
+00025400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025410: 2020 2020 2020 2020 2020 2020 2769 6e74              'int
+00025420: 273a 2032 2c0a 2020 2020 2020 2020 2020  ': 2,.          
+00025430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025440: 2020 2020 2020 2020 2027 7368 6f72 7427           'short'
+00025450: 3a20 347d 0a0a 2020 2020 2020 2020 2020  : 4}..          
+00025460: 2020 2020 2020 2320 4570 6f63 6873 2061        # Epochs a
+00025470: 6e64 2049 4341 2064 6f6e 2774 2068 6176  nd ICA don't hav
+00025480: 6520 7468 6973 2061 7474 7269 6275 7465  e this attribute
+00025490: 2c20 6173 7375 6d65 2073 696e 676c 650a  , assume single.
+000254a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000254b0: 2320 6f6e 2064 6973 6b0a 2020 2020 2020  # on disk.      
+000254c0: 2020 2020 2020 2020 2020 666d 7420 3d20            fmt = 
+000254d0: 6765 7461 7474 7228 7365 6c66 2e6d 6e65  getattr(self.mne
+000254e0: 2e69 6e73 742c 2027 6f72 6967 5f66 6f72  .inst, 'orig_for
+000254f0: 6d61 7427 2c20 2773 696e 676c 6527 290a  mat', 'single').
+00025500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025510: 2320 4170 706c 7920 7369 7a65 2063 6861  # Apply size cha
+00025520: 6e67 6520 746f 2036 342d 6269 7420 666c  nge to 64-bit fl
+00025530: 6f61 7420 696e 206d 656d 6f72 790a 2020  oat in memory.  
+00025540: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00025550: 282a 2032 2062 6563 6175 7365 2077 6865  (* 2 because whe
+00025560: 6e20 6c6f 6164 696e 6720 6461 7461 2077  n loading data w
+00025570: 696c 6c20 6265 206c 6f61 6465 6420 696e  ill be loaded in
+00025580: 746f 2061 2063 6f70 790a 2020 2020 2020  to a copy.      
+00025590: 2020 2020 2020 2020 2020 2320 6f66 2073            # of s
+000255a0: 656c 662e 6d6e 652e 696e 7374 2e5f 6461  elf.mne.inst._da
+000255b0: 7461 2074 6f20 6170 706c 7920 7072 6f63  ta to apply proc
+000255c0: 6573 7369 6e67 2e0a 2020 2020 2020 2020  essing..        
+000255d0: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+000255e0: 5f72 616d 203d 2064 6973 6b5f 7370 6163  _ram = disk_spac
+000255f0: 6520 2a20 666d 745f 6d75 6c74 6970 6c69  e * fmt_multipli
+00025600: 6572 735b 666d 745d 202a 2032 0a20 2020  ers[fmt] * 2.   
+00025610: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00025620: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00025630: 7870 6563 7465 645f 7261 6d20 3d20 7379  xpected_ram = sy
+00025640: 732e 6765 7473 697a 656f 6628 7365 6c66  s.getsizeof(self
+00025650: 2e6d 6e65 2e69 6e73 742e 5f64 6174 6129  .mne.inst._data)
+00025660: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00025670: 4765 7420 6176 6169 6c61 626c 6520 5241  Get available RA
+00025680: 4d0a 2020 2020 2020 2020 2020 2020 6672  M.            fr
+00025690: 6565 5f72 616d 203d 2070 7375 7469 6c2e  ee_ram = psutil.
+000256a0: 7669 7274 7561 6c5f 6d65 6d6f 7279 2829  virtual_memory()
+000256b0: 2e66 7265 650a 0a20 2020 2020 2020 2020  .free..         
+000256c0: 2020 2065 7870 6563 7465 645f 7261 6d5f     expected_ram_
+000256d0: 7374 7220 3d20 7369 7a65 6f66 5f66 6d74  str = sizeof_fmt
+000256e0: 2865 7870 6563 7465 645f 7261 6d29 0a20  (expected_ram). 
+000256f0: 2020 2020 2020 2020 2020 2066 7265 655f             free_
+00025700: 7261 6d5f 7374 7220 3d20 7369 7a65 6f66  ram_str = sizeof
+00025710: 5f66 6d74 2866 7265 655f 7261 6d29 0a20  _fmt(free_ram). 
+00025720: 2020 2020 2020 2020 2020 206c 6566 745f             left_
+00025730: 7261 6d5f 7374 7220 3d20 7369 7a65 6f66  ram_str = sizeof
+00025740: 5f66 6d74 2866 7265 655f 7261 6d20 2d20  _fmt(free_ram - 
+00025750: 6578 7065 6374 6564 5f72 616d 290a 0a20  expected_ram).. 
+00025760: 2020 2020 2020 2020 2020 2069 6620 6578             if ex
+00025770: 7065 6374 6564 5f72 616d 203c 2066 7265  pected_ram < fre
+00025780: 655f 7261 6d3a 0a20 2020 2020 2020 2020  e_ram:.         
+00025790: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+000257a0: 6275 6728 2754 6865 2064 6174 6120 7072  bug('The data pr
+000257b0: 6563 6f6d 7075 7465 6420 666f 7220 7669  ecomputed for vi
+000257c0: 7375 616c 697a 6174 696f 6e20 7461 6b65  sualization take
+000257d0: 7320 270a 2020 2020 2020 2020 2020 2020  s '.            
+000257e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000257f0: 2066 277b 6578 7065 6374 6564 5f72 616d   f'{expected_ram
+00025800: 5f73 7472 7d20 7769 7468 207b 6c65 6674  _str} with {left
+00025810: 5f72 616d 5f73 7472 7d20 6f66 2027 0a20  _ram_str} of '. 
+00025820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025830: 2020 2020 2020 2020 2020 2020 6627 5241              f'RA
+00025840: 4d20 6c65 6674 2e27 290a 2020 2020 2020  M left.').      
+00025850: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00025860: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+00025870: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00025880: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00025890: 6562 7567 2866 2754 6865 2070 7265 636f  ebug(f'The preco
+000258a0: 6d70 7574 6564 2064 6174 6120 7769 7468  mputed data with
+000258b0: 207b 6578 7065 6374 6564 5f72 616d 5f73   {expected_ram_s
+000258c0: 7472 7d20 270a 2020 2020 2020 2020 2020  tr} '.          
+000258d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000258e0: 2020 2066 2777 696c 6c20 7375 7270 6173     f'will surpas
+000258f0: 7320 796f 7572 2063 7572 7265 6e74 207b  s your current {
+00025900: 6672 6565 5f72 616d 5f73 7472 7d20 270a  free_ram_str} '.
+00025910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025920: 2020 2020 2020 2020 2020 2020 2066 276f               f'o
+00025930: 6620 6672 6565 2052 414d 2e5c 6e27 0a20  f free RAM.\n'. 
+00025940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025950: 2020 2020 2020 2020 2020 2020 2754 6875              'Thu
+00025960: 7320 7072 6563 6f6d 7075 7465 2077 696c  s precompute wil
+00025970: 6c20 6265 2073 6574 2074 6f20 4661 6c73  l be set to Fals
+00025980: 652e 5c6e 270a 2020 2020 2020 2020 2020  e.\n'.          
+00025990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000259a0: 2020 2027 2849 6620 796f 7520 7761 6e74     '(If you want
+000259b0: 2074 6f20 7072 6563 6f6d 7075 7465 206e   to precompute n
+000259c0: 6576 6572 7468 656c 6573 732c 2027 0a20  evertheless, '. 
+000259d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000259e0: 2020 2020 2020 2020 2020 2020 2774 6865              'the
+000259f0: 6e20 7365 7420 7072 6563 6f6d 7075 7465  n set precompute
+00025a00: 2074 6f20 5472 7565 2069 6e73 7465 6164   to True instead
+00025a10: 206f 6620 2261 7574 6f22 2927 290a 2020   of "auto")').  
+00025a20: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00025a30: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+00025a40: 6465 6620 5f70 726f 6365 7373 5f64 6174  def _process_dat
+00025a50: 6128 7365 6c66 2c20 6461 7461 2c20 7374  a(self, data, st
+00025a60: 6172 742c 2073 746f 702c 2070 6963 6b73  art, stop, picks
+00025a70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00025a80: 2020 2020 2020 2020 7369 676e 616c 733d          signals=
+00025a90: 4e6f 6e65 293a 0a20 2020 2020 2020 2064  None):.        d
+00025aa0: 6174 6120 3d20 7375 7065 7228 292e 5f70  ata = super()._p
+00025ab0: 726f 6365 7373 5f64 6174 6128 6461 7461  rocess_data(data
+00025ac0: 2c20 7374 6172 742c 2073 746f 702c 2070  , start, stop, p
+00025ad0: 6963 6b73 2c20 7369 676e 616c 7329 0a0a  icks, signals)..
+00025ae0: 2020 2020 2020 2020 2320 496e 7665 7274          # Invert
+00025af0: 2044 6174 6120 746f 2062 6520 6469 7370   Data to be disp
+00025b00: 6c61 7965 6420 6672 6f6d 2074 6f70 206f  layed from top o
+00025b10: 6e20 696e 7665 7274 6564 2059 2d41 7869  n inverted Y-Axi
+00025b20: 730a 2020 2020 2020 2020 6461 7461 202a  s.        data *
+00025b30: 3d20 2d31 0a0a 2020 2020 2020 2020 7265  = -1..        re
+00025b40: 7475 726e 2064 6174 610a 0a20 2020 2064  turn data..    d
+00025b50: 6566 205f 7570 6461 7465 5f64 6174 6128  ef _update_data(
+00025b60: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+00025b70: 6620 7365 6c66 2e6d 6e65 2e64 6174 615f  f self.mne.data_
+00025b80: 7072 6563 6f6d 7075 7465 643a 0a20 2020  precomputed:.   
+00025b90: 2020 2020 2020 2020 2023 2067 6574 2073           # get s
+00025ba0: 7461 7274 2f73 746f 702d 7361 6d70 6c65  tart/stop-sample
+00025bb0: 730a 2020 2020 2020 2020 2020 2020 7374  s.            st
+00025bc0: 6172 742c 2073 746f 7020 3d20 7365 6c66  art, stop = self
+00025bd0: 2e5f 6765 745f 7374 6172 745f 7374 6f70  ._get_start_stop
+00025be0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00025bf0: 656c 662e 6d6e 652e 7469 6d65 7320 3d20  elf.mne.times = 
+00025c00: 7365 6c66 2e6d 6e65 2e67 6c6f 6261 6c5f  self.mne.global_
+00025c10: 7469 6d65 735b 7374 6172 743a 7374 6f70  times[start:stop
+00025c20: 5d0a 2020 2020 2020 2020 2020 2020 7365  ].            se
+00025c30: 6c66 2e6d 6e65 2e64 6174 6120 3d20 7365  lf.mne.data = se
+00025c40: 6c66 2e6d 6e65 2e67 6c6f 6261 6c5f 6461  lf.mne.global_da
+00025c50: 7461 5b3a 2c20 7374 6172 743a 7374 6f70  ta[:, start:stop
+00025c60: 5d0a 0a20 2020 2020 2020 2020 2020 2023  ]..            #
+00025c70: 2072 656d 6f76 6520 4443 206c 6f63 616c   remove DC local
+00025c80: 6c79 0a20 2020 2020 2020 2020 2020 2069  ly.            i
+00025c90: 6620 7365 6c66 2e6d 6e65 2e72 656d 6f76  f self.mne.remov
+00025ca0: 655f 6463 3a0a 2020 2020 2020 2020 2020  e_dc:.          
+00025cb0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e64        self.mne.d
+00025cc0: 6174 6120 3d20 7365 6c66 2e6d 6e65 2e64  ata = self.mne.d
+00025cd0: 6174 6120 2d20 5c0a 2020 2020 2020 2020  ata - \.        
+00025ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025cf0: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
+00025d00: 2e64 6174 612e 6d65 616e 2861 7869 733d  .data.mean(axis=
+00025d10: 312c 206b 6565 7064 696d 733d 5472 7565  1, keepdims=True
+00025d20: 290a 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
+00025d30: 0a20 2020 2020 2020 2020 2020 2023 2057  .            # W
+00025d40: 6869 6c65 2064 6174 6120 6973 206e 6f74  hile data is not
+00025d50: 2070 7265 636f 6d70 7574 6564 2067 6574   precomputed get
+00025d60: 2064 6174 6120 6f6e 6c79 2066 726f 6d20   data only from 
+00025d70: 7368 6f77 6e20 7261 6e67 6520 616e 640a  shown range and.
+00025d80: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
+00025d90: 6f63 6573 7320 6f6e 6c79 2074 686f 7365  ocess only those
+00025da0: 2e0a 2020 2020 2020 2020 2020 2020 7375  ..            su
+00025db0: 7065 7228 292e 5f75 7064 6174 655f 6461  per()._update_da
+00025dc0: 7461 2829 0a0a 2020 2020 2020 2020 2320  ta()..        # 
+00025dd0: 496e 6974 6961 6c69 7a65 2064 6563 696d  Initialize decim
+00025de0: 0a20 2020 2020 2020 2073 656c 662e 6d6e  .        self.mn
+00025df0: 652e 6465 6369 6d5f 6461 7461 203d 206e  e.decim_data = n
+00025e00: 702e 6f6e 6573 5f6c 696b 6528 7365 6c66  p.ones_like(self
+00025e10: 2e6d 6e65 2e70 6963 6b73 290a 2020 2020  .mne.picks).    
+00025e20: 2020 2020 6461 7461 5f70 6963 6b73 5f6d      data_picks_m
+00025e30: 6173 6b20 3d20 6e70 2e69 6e31 6428 7365  ask = np.in1d(se
+00025e40: 6c66 2e6d 6e65 2e70 6963 6b73 2c20 7365  lf.mne.picks, se
+00025e50: 6c66 2e6d 6e65 2e70 6963 6b73 5f64 6174  lf.mne.picks_dat
+00025e60: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
+00025e70: 6d6e 652e 6465 6369 6d5f 6461 7461 5b64  mne.decim_data[d
+00025e80: 6174 615f 7069 636b 735f 6d61 736b 5d20  ata_picks_mask] 
+00025e90: 3d20 7365 6c66 2e6d 6e65 2e64 6563 696d  = self.mne.decim
+00025ea0: 0a0a 2020 2020 2020 2020 2320 4170 706c  ..        # Appl
+00025eb0: 7920 636c 6970 7069 6e67 0a20 2020 2020  y clipping.     
+00025ec0: 2020 2069 6620 7365 6c66 2e6d 6e65 2e63     if self.mne.c
+00025ed0: 6c69 7070 696e 6720 3d3d 2027 636c 616d  lipping == 'clam
+00025ee0: 7027 3a0a 2020 2020 2020 2020 2020 2020  p':.            
+00025ef0: 7365 6c66 2e6d 6e65 2e64 6174 6120 3d20  self.mne.data = 
+00025f00: 6e70 2e63 6c69 7028 7365 6c66 2e6d 6e65  np.clip(self.mne
+00025f10: 2e64 6174 612c 202d 302e 352c 2030 2e35  .data, -0.5, 0.5
+00025f20: 290a 2020 2020 2020 2020 656c 6966 2073  ).        elif s
+00025f30: 656c 662e 6d6e 652e 636c 6970 7069 6e67  elf.mne.clipping
+00025f40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00025f50: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00025f60: 6e65 2e64 6174 6120 3d20 7365 6c66 2e6d  ne.data = self.m
+00025f70: 6e65 2e64 6174 612e 636f 7079 2829 0a20  ne.data.copy(). 
+00025f80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00025f90: 6d6e 652e 6461 7461 5b61 6273 2873 656c  mne.data[abs(sel
+00025fa0: 662e 6d6e 652e 6461 7461 202a 2073 656c  f.mne.data * sel
+00025fb0: 662e 6d6e 652e 7363 616c 655f 6661 6374  f.mne.scale_fact
+00025fc0: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
+00025fd0: 2020 2020 2020 2020 2020 2020 2020 3e20                > 
+00025fe0: 7365 6c66 2e6d 6e65 2e63 6c69 7070 696e  self.mne.clippin
+00025ff0: 675d 203d 206e 702e 6e61 6e0a 0a20 2020  g] = np.nan..   
+00026000: 2020 2020 2023 2041 7070 6c79 2044 6f77       # Apply Dow
+00026010: 6e73 616d 706c 696e 6720 2869 6620 656e  nsampling (if en
+00026020: 6162 6c65 6429 0a20 2020 2020 2020 2073  abled).        s
+00026030: 656c 662e 5f61 7070 6c79 5f64 6f77 6e73  elf._apply_downs
+00026040: 616d 706c 696e 6728 290a 0a20 2020 2064  ampling()..    d
+00026050: 6566 205f 6765 745f 7a73 636f 7265 2873  ef _get_zscore(s
+00026060: 656c 662c 2064 6174 6129 3a0a 2020 2020  elf, data):.    
+00026070: 2020 2020 2320 5265 7368 6170 6520 6461      # Reshape da
+00026080: 7461 2074 6f20 7265 6173 6f6e 6162 6c65  ta to reasonable
+00026090: 2073 697a 6520 666f 7220 6469 7370 6c61   size for displa
+000260a0: 790a 2020 2020 2020 2020 7363 7265 656e  y.        screen
+000260b0: 5f67 656f 6d65 7472 7920 3d20 5f73 6372  _geometry = _scr
+000260c0: 6565 6e5f 6765 6f6d 6574 7279 2873 656c  een_geometry(sel
+000260d0: 6629 0a20 2020 2020 2020 2069 6620 7363  f).        if sc
+000260e0: 7265 656e 5f67 656f 6d65 7472 7920 6973  reen_geometry is
+000260f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00026100: 2020 206d 6178 5f70 6978 656c 5f77 6964     max_pixel_wid
+00026110: 7468 203d 2033 3834 3020 2023 2064 6566  th = 3840  # def
+00026120: 6175 6c74 3d55 4844 0a20 2020 2020 2020  ault=UHD.       
+00026130: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00026140: 2020 206d 6178 5f70 6978 656c 5f77 6964     max_pixel_wid
+00026150: 7468 203d 2073 6372 6565 6e5f 6765 6f6d  th = screen_geom
+00026160: 6574 7279 2e77 6964 7468 2829 0a20 2020  etry.width().   
+00026170: 2020 2020 2063 6f6c 6c61 7073 655f 6279       collapse_by
+00026180: 203d 2064 6174 612e 7368 6170 655b 315d   = data.shape[1]
+00026190: 202f 2f20 6d61 785f 7069 7865 6c5f 7769   // max_pixel_wi
+000261a0: 6474 680a 2020 2020 2020 2020 6461 7461  dth.        data
+000261b0: 203d 2064 6174 615b 3a2c 203a 6d61 785f   = data[:, :max_
+000261c0: 7069 7865 6c5f 7769 6474 6820 2a20 636f  pixel_width * co
+000261d0: 6c6c 6170 7365 5f62 795d 0a20 2020 2020  llapse_by].     
+000261e0: 2020 2069 6620 636f 6c6c 6170 7365 5f62     if collapse_b
+000261f0: 7920 3e20 303a 0a20 2020 2020 2020 2020  y > 0:.         
+00026200: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+00026210: 6573 6861 7065 2864 6174 612e 7368 6170  eshape(data.shap
+00026220: 655b 305d 2c20 6d61 785f 7069 7865 6c5f  e[0], max_pixel_
+00026230: 7769 6474 682c 2063 6f6c 6c61 7073 655f  width, collapse_
+00026240: 6279 290a 2020 2020 2020 2020 2020 2020  by).            
+00026250: 6461 7461 203d 2064 6174 612e 6d65 616e  data = data.mean
+00026260: 2861 7869 733d 3229 0a20 2020 2020 2020  (axis=2).       
+00026270: 207a 203d 207a 7363 6f72 6528 6461 7461   z = zscore(data
+00026280: 2c20 6178 6973 3d31 290a 2020 2020 2020  , axis=1).      
+00026290: 2020 6966 207a 2e73 697a 6520 3e20 303a    if z.size > 0:
+000262a0: 0a20 2020 2020 2020 2020 2020 207a 6d69  .            zmi
+000262b0: 6e20 3d20 6e70 2e6d 696e 287a 2c20 6178  n = np.min(z, ax
+000262c0: 6973 3d31 290a 2020 2020 2020 2020 2020  is=1).          
+000262d0: 2020 7a6d 6178 203d 206e 702e 6d61 7828    zmax = np.max(
+000262e0: 7a2c 2061 7869 733d 3129 0a0a 2020 2020  z, axis=1)..    
+000262f0: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
+00026300: 7420 696e 746f 2052 4742 410a 2020 2020  t into RGBA.    
+00026310: 2020 2020 2020 2020 7a72 6762 6120 3d20          zrgba = 
+00026320: 6e70 2e65 6d70 7479 2828 2a7a 2e73 6861  np.empty((*z.sha
+00026330: 7065 2c20 3429 290a 2020 2020 2020 2020  pe, 4)).        
+00026340: 2020 2020 666f 7220 726f 775f 6964 782c      for row_idx,
+00026350: 2072 6f77 2069 6e20 656e 756d 6572 6174   row in enumerat
+00026360: 6528 7a29 3a0a 2020 2020 2020 2020 2020  e(z):.          
+00026370: 2020 2020 2020 666f 7220 636f 6c5f 6964        for col_id
+00026380: 782c 2076 616c 7565 2069 6e20 656e 756d  x, value in enum
+00026390: 6572 6174 6528 726f 7729 3a0a 2020 2020  erate(row):.    
+000263a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000263b0: 6966 206d 6174 682e 6973 6e61 6e28 7661  if math.isnan(va
+000263c0: 6c75 6529 3a0a 2020 2020 2020 2020 2020  lue):.          
+000263d0: 2020 2020 2020 2020 2020 2020 2020 7661                va
+000263e0: 6c75 6520 3d20 300a 2020 2020 2020 2020  lue = 0.        
+000263f0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+00026400: 616c 7565 203d 3d20 303a 0a20 2020 2020  alue == 0:.     
+00026410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026420: 2020 2072 6762 6120 3d20 5b30 2c20 302c     rgba = [0, 0,
+00026430: 2030 2c20 305d 0a20 2020 2020 2020 2020   0, 0].         
+00026440: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00026450: 7661 6c75 6520 3c20 303a 0a20 2020 2020  value < 0:.     
+00026460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026470: 2020 2061 6c70 6861 203d 2069 6e74 2832     alpha = int(2
+00026480: 3535 202a 2076 616c 7565 202f 2061 6273  55 * value / abs
+00026490: 287a 6d69 6e5b 726f 775f 6964 785d 2929  (zmin[row_idx]))
+000264a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000264b0: 2020 2020 2020 2020 2072 6762 6120 3d20           rgba = 
+000264c0: 5b30 2c20 302c 2032 3535 2c20 616c 7068  [0, 0, 255, alph
+000264d0: 615d 0a20 2020 2020 2020 2020 2020 2020  a].             
+000264e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000264f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026500: 2020 2020 2061 6c70 6861 203d 2069 6e74       alpha = int
+00026510: 2832 3535 202a 2076 616c 7565 202f 207a  (255 * value / z
+00026520: 6d61 785b 726f 775f 6964 785d 290a 2020  max[row_idx]).  
+00026530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026540: 2020 2020 2020 7267 6261 203d 205b 3235        rgba = [25
+00026550: 352c 2030 2c20 302c 2061 6c70 6861 5d0a  5, 0, 0, alpha].
+00026560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026570: 2020 2020 207a 7267 6261 5b72 6f77 5f69       zrgba[row_i
+00026580: 6478 2c20 636f 6c5f 6964 785d 203d 2072  dx, col_idx] = r
+00026590: 6762 610a 0a20 2020 2020 2020 2020 2020  gba..           
+000265a0: 207a 7267 6261 203d 206e 702e 7265 7175   zrgba = np.requ
+000265b0: 6972 6528 7a72 6762 612c 206e 702e 7569  ire(zrgba, np.ui
+000265c0: 6e74 382c 2027 4327 290a 0a20 2020 2020  nt8, 'C')..     
+000265d0: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
+000265e0: 7a73 636f 7265 5f72 6762 6120 3d20 7a72  zscore_rgba = zr
+000265f0: 6762 610a 0a20 2020 2023 2023 2023 2023  gba..    # # # #
+00026600: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
+00026610: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
+00026620: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
+00026630: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
+00026640: 2023 2023 0a20 2020 2023 2041 4e4e 4f54   # #.    # ANNOT
+00026650: 4154 494f 4e53 0a20 2020 2023 2023 2023  ATIONS.    # # #
+00026660: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
+00026670: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
+00026680: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
+00026690: 2023 2023 2023 2023 2023 2023 2023 2023   # # # # # # # #
+000266a0: 2023 2023 2023 0a20 2020 2064 6566 205f   # # #.    def _
+000266b0: 6164 645f 7265 6769 6f6e 2873 656c 662c  add_region(self,
+000266c0: 2070 6c6f 745f 6f6e 7365 742c 2064 7572   plot_onset, dur
+000266d0: 6174 696f 6e2c 2064 6573 6372 6970 7469  ation, descripti
+000266e0: 6f6e 2c20 2a2c 2072 6567 696f 6e3d 4e6f  on, *, region=No
+000266f0: 6e65 293a 0a20 2020 2020 2020 2069 6620  ne):.        if 
+00026700: 6e6f 7420 7265 6769 6f6e 3a0a 2020 2020  not region:.    
+00026710: 2020 2020 2020 2020 7265 6769 6f6e 203d          region =
+00026720: 2041 6e6e 6f74 5265 6769 6f6e 2873 656c   AnnotRegion(sel
+00026730: 662e 6d6e 652c 2064 6573 6372 6970 7469  f.mne, descripti
+00026740: 6f6e 3d64 6573 6372 6970 7469 6f6e 2c0a  on=description,.
+00026750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026770: 2076 616c 7565 733d 2870 6c6f 745f 6f6e   values=(plot_on
+00026780: 7365 742c 2070 6c6f 745f 6f6e 7365 7420  set, plot_onset 
+00026790: 2b20 6475 7261 7469 6f6e 2929 0a20 2020  + duration)).   
+000267a0: 2020 2020 2023 2041 6464 2072 6567 696f       # Add regio
+000267b0: 6e20 746f 206c 6973 7420 616e 6420 706c  n to list and pl
+000267c0: 6f74 0a20 2020 2020 2020 2073 656c 662e  ot.        self.
+000267d0: 6d6e 652e 7265 6769 6f6e 732e 6170 7065  mne.regions.appe
+000267e0: 6e64 2872 6567 696f 6e29 0a0a 2020 2020  nd(region)..    
+000267f0: 2020 2020 2320 436f 6e6e 6563 7420 7369      # Connect si
+00026800: 676e 616c 7320 6f66 2072 6567 696f 6e0a  gnals of region.
+00026810: 2020 2020 2020 2020 7265 6769 6f6e 2e72          region.r
+00026820: 6567 696f 6e43 6861 6e67 6546 696e 6973  egionChangeFinis
+00026830: 6865 642e 636f 6e6e 6563 7428 7365 6c66  hed.connect(self
+00026840: 2e5f 7265 6769 6f6e 5f63 6861 6e67 6564  ._region_changed
+00026850: 290a 2020 2020 2020 2020 7265 6769 6f6e  ).        region
+00026860: 2e67 6f74 5365 6c65 6374 6564 2e63 6f6e  .gotSelected.con
+00026870: 6e65 6374 2873 656c 662e 5f72 6567 696f  nect(self._regio
+00026880: 6e5f 7365 6c65 6374 6564 290a 2020 2020  n_selected).    
+00026890: 2020 2020 7265 6769 6f6e 2e72 656d 6f76      region.remov
+000268a0: 6552 6571 7565 7374 6564 2e63 6f6e 6e65  eRequested.conne
+000268b0: 6374 2873 656c 662e 5f72 656d 6f76 655f  ct(self._remove_
+000268c0: 7265 6769 6f6e 290a 2020 2020 2020 2020  region).        
+000268d0: 7365 6c66 2e6d 6e65 2e76 6965 7762 6f78  self.mne.viewbox
+000268e0: 2e73 6967 5952 616e 6765 4368 616e 6765  .sigYRangeChange
+000268f0: 642e 636f 6e6e 6563 7428 7265 6769 6f6e  d.connect(region
+00026900: 2e75 7064 6174 655f 6c61 6265 6c5f 706f  .update_label_po
+00026910: 7329 0a20 2020 2020 2020 2072 6567 696f  s).        regio
+00026920: 6e2e 7570 6461 7465 5f6c 6162 656c 5f70  n.update_label_p
+00026930: 6f73 2829 0a20 2020 2020 2020 2072 6574  os().        ret
+00026940: 7572 6e20 7265 6769 6f6e 0a0a 2020 2020  urn region..    
+00026950: 6465 6620 5f72 656d 6f76 655f 7265 6769  def _remove_regi
+00026960: 6f6e 2873 656c 662c 2072 6567 696f 6e2c  on(self, region,
+00026970: 2066 726f 6d5f 616e 6e6f 743d 5472 7565   from_annot=True
+00026980: 293a 0a20 2020 2020 2020 2023 2052 656d  ):.        # Rem
+00026990: 6f76 6520 6672 6f6d 2073 686f 776e 2072  ove from shown r
+000269a0: 6567 696f 6e73 0a20 2020 2020 2020 2069  egions.        i
+000269b0: 6620 7265 6769 6f6e 2e6c 6162 656c 5f69  f region.label_i
+000269c0: 7465 6d20 696e 2073 656c 662e 6d6e 652e  tem in self.mne.
+000269d0: 706c 742e 6974 656d 733a 0a20 2020 2020  plt.items:.     
+000269e0: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
+000269f0: 706c 742e 7265 6d6f 7665 4974 656d 2872  plt.removeItem(r
+00026a00: 6567 696f 6e2e 6c61 6265 6c5f 6974 656d  egion.label_item
+00026a10: 290a 2020 2020 2020 2020 6966 2072 6567  ).        if reg
+00026a20: 696f 6e20 696e 2073 656c 662e 6d6e 652e  ion in self.mne.
+00026a30: 706c 742e 6974 656d 733a 0a20 2020 2020  plt.items:.     
+00026a40: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
+00026a50: 706c 742e 7265 6d6f 7665 4974 656d 2872  plt.removeItem(r
+00026a60: 6567 696f 6e29 0a0a 2020 2020 2020 2020  egion)..        
+00026a70: 2320 5265 6d6f 7665 2066 726f 6d20 616c  # Remove from al
+00026a80: 6c20 7265 6769 6f6e 730a 2020 2020 2020  l regions.      
+00026a90: 2020 6966 2072 6567 696f 6e20 696e 2073    if region in s
+00026aa0: 656c 662e 6d6e 652e 7265 6769 6f6e 733a  elf.mne.regions:
+00026ab0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00026ac0: 662e 6d6e 652e 7265 6769 6f6e 732e 7265  f.mne.regions.re
+00026ad0: 6d6f 7665 2872 6567 696f 6e29 0a0a 2020  move(region)..  
+00026ae0: 2020 2020 2020 2320 5265 7365 7420 7365        # Reset se
+00026af0: 6c65 6374 6564 2072 6567 696f 6e0a 2020  lected region.  
+00026b00: 2020 2020 2020 6966 2072 6567 696f 6e20        if region 
+00026b10: 3d3d 2073 656c 662e 6d6e 652e 7365 6c65  == self.mne.sele
+00026b20: 6374 6564 5f72 6567 696f 6e3a 0a20 2020  cted_region:.   
+00026b30: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
+00026b40: 652e 7365 6c65 6374 6564 5f72 6567 696f  e.selected_regio
+00026b50: 6e20 3d20 4e6f 6e65 0a0a 2020 2020 2020  n = None..      
+00026b60: 2020 2320 5265 6d6f 7665 2066 726f 6d20    # Remove from 
+00026b70: 616e 6e6f 7461 7469 6f6e 730a 2020 2020  annotations.    
+00026b80: 2020 2020 6966 2066 726f 6d5f 616e 6e6f      if from_anno
+00026b90: 743a 0a20 2020 2020 2020 2020 2020 2069  t:.            i
+00026ba0: 6478 203d 2073 656c 662e 5f67 6574 5f6f  dx = self._get_o
+00026bb0: 6e73 6574 5f69 6478 2872 6567 696f 6e2e  nset_idx(region.
+00026bc0: 6765 7452 6567 696f 6e28 295b 305d 290a  getRegion()[0]).
+00026bd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00026be0: 2e6d 6e65 2e69 6e73 742e 616e 6e6f 7461  .mne.inst.annota
+00026bf0: 7469 6f6e 732e 6465 6c65 7465 2869 6478  tions.delete(idx
+00026c00: 290a 0a20 2020 2020 2020 2023 2055 7064  )..        # Upd
+00026c10: 6174 6520 4f76 6572 7669 6577 2d42 6172  ate Overview-Bar
+00026c20: 0a20 2020 2020 2020 2073 656c 662e 6d6e  .        self.mn
+00026c30: 652e 6f76 6572 7669 6577 5f62 6172 2e75  e.overview_bar.u
+00026c40: 7064 6174 655f 616e 6e6f 7461 7469 6f6e  pdate_annotation
+00026c50: 7328 290a 0a20 2020 2064 6566 205f 7265  s()..    def _re
+00026c60: 6769 6f6e 5f73 656c 6563 7465 6428 7365  gion_selected(se
+00026c70: 6c66 2c20 7265 6769 6f6e 293a 0a20 2020  lf, region):.   
+00026c80: 2020 2020 206f 6c64 5f72 6567 696f 6e20       old_region 
+00026c90: 3d20 7365 6c66 2e6d 6e65 2e73 656c 6563  = self.mne.selec
+00026ca0: 7465 645f 7265 6769 6f6e 0a20 2020 2020  ted_region.     
+00026cb0: 2020 2023 2052 656d 6f76 6520 7365 6c65     # Remove sele
+00026cc0: 6374 6564 2d73 7461 7475 7320 6672 6f6d  cted-status from
+00026cd0: 206f 6c64 2072 6567 696f 6e0a 2020 2020   old region.    
+00026ce0: 2020 2020 6966 206f 6c64 5f72 6567 696f      if old_regio
+00026cf0: 6e20 616e 6420 6f6c 645f 7265 6769 6f6e  n and old_region
+00026d00: 2021 3d20 7265 6769 6f6e 3a0a 2020 2020   != region:.    
+00026d10: 2020 2020 2020 2020 6f6c 645f 7265 6769          old_regi
+00026d20: 6f6e 2e73 656c 6563 7428 4661 6c73 6529  on.select(False)
+00026d30: 0a20 2020 2020 2020 2073 656c 662e 6d6e  .        self.mn
+00026d40: 652e 7365 6c65 6374 6564 5f72 6567 696f  e.selected_regio
+00026d50: 6e20 3d20 7265 6769 6f6e 0a20 2020 2020  n = region.     
+00026d60: 2020 2073 656c 662e 6d6e 652e 6669 675f     self.mne.fig_
+00026d70: 616e 6e6f 7461 7469 6f6e 2e75 7064 6174  annotation.updat
+00026d80: 655f 7661 6c75 6573 2872 6567 696f 6e29  e_values(region)
+00026d90: 0a0a 2020 2020 6465 6620 5f67 6574 5f6f  ..    def _get_o
+00026da0: 6e73 6574 5f69 6478 2873 656c 662c 2070  nset_idx(self, p
+00026db0: 6c6f 745f 6f6e 7365 7429 3a0a 2020 2020  lot_onset):.    
+00026dc0: 2020 2020 6f6e 7365 7420 3d20 5f73 796e      onset = _syn
+00026dd0: 635f 6f6e 7365 7428 7365 6c66 2e6d 6e65  c_onset(self.mne
+00026de0: 2e69 6e73 742c 2070 6c6f 745f 6f6e 7365  .inst, plot_onse
+00026df0: 742c 2069 6e76 6572 7365 3d54 7275 6529  t, inverse=True)
+00026e00: 0a20 2020 2020 2020 2069 6478 203d 206e  .        idx = n
+00026e10: 702e 7768 6572 6528 7365 6c66 2e6d 6e65  p.where(self.mne
+00026e20: 2e69 6e73 742e 616e 6e6f 7461 7469 6f6e  .inst.annotation
+00026e30: 732e 6f6e 7365 7420 3d3d 206f 6e73 6574  s.onset == onset
+00026e40: 295b 305d 5b30 5d0a 2020 2020 2020 2020  )[0][0].        
+00026e50: 7265 7475 726e 2069 6478 0a0a 2020 2020  return idx..    
+00026e60: 6465 6620 5f72 6567 696f 6e5f 6368 616e  def _region_chan
+00026e70: 6765 6428 7365 6c66 2c20 7265 6769 6f6e  ged(self, region
+00026e80: 293a 0a20 2020 2020 2020 2072 676e 203d  ):.        rgn =
+00026e90: 2072 6567 696f 6e2e 6765 7452 6567 696f   region.getRegio
+00026ea0: 6e28 290a 2020 2020 2020 2020 7265 6769  n().        regi
+00026eb0: 6f6e 2e73 656c 6563 7428 5472 7565 290a  on.select(True).
+00026ec0: 2020 2020 2020 2020 6964 7820 3d20 7365          idx = se
+00026ed0: 6c66 2e5f 6765 745f 6f6e 7365 745f 6964  lf._get_onset_id
+00026ee0: 7828 7265 6769 6f6e 2e6f 6c64 5f6f 6e73  x(region.old_ons
+00026ef0: 6574 290a 0a20 2020 2020 2020 2023 2055  et)..        # U
+00026f00: 7064 6174 6520 5370 696e 626f 7865 7320  pdate Spinboxes 
+00026f10: 6f66 2041 6e6e 6f74 2d44 6f63 6b0a 2020  of Annot-Dock.  
+00026f20: 2020 2020 2020 7365 6c66 2e6d 6e65 2e66        self.mne.f
+00026f30: 6967 5f61 6e6e 6f74 6174 696f 6e2e 7570  ig_annotation.up
+00026f40: 6461 7465 5f76 616c 7565 7328 7265 6769  date_values(regi
+00026f50: 6f6e 290a 0a20 2020 2020 2020 2023 2043  on)..        # C
+00026f60: 6861 6e67 6520 616e 6e6f 7461 7469 6f6e  hange annotation
+00026f70: 730a 2020 2020 2020 2020 7365 6c66 2e6d  s.        self.m
+00026f80: 6e65 2e69 6e73 742e 616e 6e6f 7461 7469  ne.inst.annotati
+00026f90: 6f6e 732e 6f6e 7365 745b 6964 785d 203d  ons.onset[idx] =
+00026fa0: 205f 7379 6e63 5f6f 6e73 6574 2873 656c   _sync_onset(sel
+00026fb0: 662e 6d6e 652e 696e 7374 2c0a 2020 2020  f.mne.inst,.    
+00026fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026ff0: 2020 2020 2020 2072 676e 5b30 5d2c 0a20         rgn[0],. 
+00027000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027030: 2020 2020 2020 2020 2020 696e 7665 7273            invers
+00027040: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+00027050: 7365 6c66 2e6d 6e65 2e69 6e73 742e 616e  self.mne.inst.an
+00027060: 6e6f 7461 7469 6f6e 732e 6475 7261 7469  notations.durati
+00027070: 6f6e 5b69 6478 5d20 3d20 7267 6e5b 315d  on[idx] = rgn[1]
+00027080: 202d 2072 676e 5b30 5d0a 0a20 2020 2020   - rgn[0]..     
+00027090: 2020 2023 2055 7064 6174 6520 6f76 6572     # Update over
+000270a0: 7669 6577 2d62 6172 0a20 2020 2020 2020  view-bar.       
+000270b0: 2073 656c 662e 6d6e 652e 6f76 6572 7669   self.mne.overvi
+000270c0: 6577 5f62 6172 2e75 7064 6174 655f 616e  ew_bar.update_an
+000270d0: 6e6f 7461 7469 6f6e 7328 290a 0a20 2020  notations()..   
+000270e0: 2064 6566 205f 6472 6177 5f61 6e6e 6f74   def _draw_annot
+000270f0: 6174 696f 6e73 2873 656c 6629 3a0a 2020  ations(self):.  
+00027100: 2020 2020 2020 2320 416c 6c20 7265 6769        # All regi
+00027110: 6f6e 7320 6172 6520 636f 6e73 7461 6e74  ons are constant
+00027120: 6c79 2061 6464 6564 2074 6f20 7468 6520  ly added to the 
+00027130: 5363 656e 6520 616e 6420 6861 6e64 6c65  Scene and handle
+00027140: 6420 6279 2051 740a 2020 2020 2020 2020  d by Qt.        
+00027150: 2320 7768 6963 6820 6973 2066 6173 7465  # which is faste
+00027160: 7220 7468 616e 2068 616e 646c 696e 6720  r than handling 
+00027170: 6164 6469 6e67 2f72 656d 6f76 696e 6720  adding/removing 
+00027180: 696e 2050 7974 686f 6e2e 0a20 2020 2020  in Python..     
+00027190: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+000271a0: 205f 696e 6974 5f61 6e6e 6f74 5f6d 6f64   _init_annot_mod
+000271b0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000271c0: 2073 656c 662e 6d6e 652e 616e 6e6f 7461   self.mne.annota
+000271d0: 7469 6f6e 735f 7669 7369 626c 6520 3d20  tions_visible = 
+000271e0: 5472 7565 0a20 2020 2020 2020 2073 656c  True.        sel
+000271f0: 662e 6d6e 652e 6e65 775f 616e 6e6f 7461  f.mne.new_annota
+00027200: 7469 6f6e 5f6c 6162 656c 7320 3d20 7365  tion_labels = se
+00027210: 6c66 2e5f 6765 745f 616e 6e6f 7461 7469  lf._get_annotati
+00027220: 6f6e 5f6c 6162 656c 7328 290a 2020 2020  on_labels().    
+00027230: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
+00027240: 6d6e 652e 6e65 775f 616e 6e6f 7461 7469  mne.new_annotati
+00027250: 6f6e 5f6c 6162 656c 7329 203e 2030 3a0a  on_labels) > 0:.
+00027260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00027270: 2e6d 6e65 2e63 7572 7265 6e74 5f64 6573  .mne.current_des
+00027280: 6372 6970 7469 6f6e 203d 2073 656c 662e  cription = self.
+00027290: 6d6e 652e 6e65 775f 616e 6e6f 7461 7469  mne.new_annotati
+000272a0: 6f6e 5f6c 6162 656c 735b 305d 0a20 2020  on_labels[0].   
+000272b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000272c0: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
+000272d0: 6375 7272 656e 745f 6465 7363 7269 7074  current_descript
+000272e0: 696f 6e20 3d20 4e6f 6e65 0a20 2020 2020  ion = None.     
+000272f0: 2020 2073 656c 662e 5f73 6574 7570 5f61     self._setup_a
+00027300: 6e6e 6f74 6174 696f 6e5f 636f 6c6f 7273  nnotation_colors
+00027310: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00027320: 6d6e 652e 7265 6769 6f6e 7320 3d20 6c69  mne.regions = li
+00027330: 7374 2829 0a20 2020 2020 2020 2073 656c  st().        sel
+00027340: 662e 6d6e 652e 7365 6c65 6374 6564 5f72  f.mne.selected_r
+00027350: 6567 696f 6e20 3d20 4e6f 6e65 0a0a 2020  egion = None..  
+00027360: 2020 2020 2020 2320 496e 6974 6961 6c69        # Initiali
+00027370: 7a65 2041 6e6e 6f74 6174 696f 6e2d 446f  ze Annotation-Do
+00027380: 636b 0a20 2020 2020 2020 2065 7869 7374  ck.        exist
+00027390: 696e 675f 646f 636b 203d 2067 6574 6174  ing_dock = getat
+000273a0: 7472 2873 656c 662e 6d6e 652c 2027 6669  tr(self.mne, 'fi
+000273b0: 675f 616e 6e6f 7461 7469 6f6e 272c 204e  g_annotation', N
+000273c0: 6f6e 6529 0a20 2020 2020 2020 2069 6620  one).        if 
+000273d0: 6578 6973 7469 6e67 5f64 6f63 6b20 6973  existing_dock is
+000273e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000273f0: 2020 2073 656c 662e 6d6e 652e 6669 675f     self.mne.fig_
+00027400: 616e 6e6f 7461 7469 6f6e 203d 2041 6e6e  annotation = Ann
+00027410: 6f74 6174 696f 6e44 6f63 6b28 7365 6c66  otationDock(self
+00027420: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00027430: 6c66 2e61 6464 446f 636b 5769 6467 6574  lf.addDockWidget
+00027440: 2851 742e 546f 7044 6f63 6b57 6964 6765  (Qt.TopDockWidge
+00027450: 7441 7265 612c 2073 656c 662e 6d6e 652e  tArea, self.mne.
+00027460: 6669 675f 616e 6e6f 7461 7469 6f6e 290a  fig_annotation).
+00027470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00027480: 2e6d 6e65 2e66 6967 5f61 6e6e 6f74 6174  .mne.fig_annotat
+00027490: 696f 6e2e 7365 7456 6973 6962 6c65 2846  ion.setVisible(F
+000274a0: 616c 7365 290a 0a20 2020 2020 2020 2023  alse)..        #
+000274b0: 2041 6464 2061 6e6e 6f74 6174 696f 6e73   Add annotations
+000274c0: 2061 7320 7265 6769 6f6e 730a 2020 2020   as regions.    
+000274d0: 2020 2020 666f 7220 616e 6e6f 7420 696e      for annot in
+000274e0: 2073 656c 662e 6d6e 652e 696e 7374 2e61   self.mne.inst.a
+000274f0: 6e6e 6f74 6174 696f 6e73 3a0a 2020 2020  nnotations:.    
+00027500: 2020 2020 2020 2020 706c 6f74 5f6f 6e73          plot_ons
+00027510: 6574 203d 205f 7379 6e63 5f6f 6e73 6574  et = _sync_onset
+00027520: 2873 656c 662e 6d6e 652e 696e 7374 2c20  (self.mne.inst, 
+00027530: 616e 6e6f 745b 276f 6e73 6574 275d 290a  annot['onset']).
+00027540: 2020 2020 2020 2020 2020 2020 6475 7261              dura
+00027550: 7469 6f6e 203d 2061 6e6e 6f74 5b27 6475  tion = annot['du
+00027560: 7261 7469 6f6e 275d 0a20 2020 2020 2020  ration'].       
+00027570: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00027580: 203d 2061 6e6e 6f74 5b27 6465 7363 7269   = annot['descri
+00027590: 7074 696f 6e27 5d0a 2020 2020 2020 2020  ption'].        
+000275a0: 2020 2020 7265 6769 6f6e 203d 2073 656c      region = sel
+000275b0: 662e 5f61 6464 5f72 6567 696f 6e28 706c  f._add_region(pl
+000275c0: 6f74 5f6f 6e73 6574 2c20 6475 7261 7469  ot_onset, durati
+000275d0: 6f6e 2c20 6465 7363 7269 7074 696f 6e29  on, description)
+000275e0: 0a20 2020 2020 2020 2020 2020 2072 6567  .            reg
+000275f0: 696f 6e2e 7570 6461 7465 5f76 6973 6962  ion.update_visib
+00027600: 6c65 2846 616c 7365 290a 0a20 2020 2020  le(False)..     
+00027610: 2020 2023 2049 6e69 7469 616c 697a 6520     # Initialize 
+00027620: 7368 6f77 696e 6720 616e 6e6f 7461 7469  showing annotati
+00027630: 6f6e 2077 6964 6765 7473 0a20 2020 2020  on widgets.     
+00027640: 2020 2073 656c 662e 5f63 6861 6e67 655f     self._change_
+00027650: 616e 6e6f 745f 6d6f 6465 2829 0a0a 2020  annot_mode()..  
+00027660: 2020 6465 6620 5f63 6861 6e67 655f 616e    def _change_an
+00027670: 6e6f 745f 6d6f 6465 2873 656c 6629 3a0a  not_mode(self):.
+00027680: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00027690: 656c 662e 6d6e 652e 616e 6e6f 7461 7469  elf.mne.annotati
+000276a0: 6f6e 5f6d 6f64 653a 0a20 2020 2020 2020  on_mode:.       
+000276b0: 2020 2020 2023 2052 6573 6574 2057 6964       # Reset Wid
+000276c0: 6765 7473 2069 6e20 416e 6e6f 7461 7469  gets in Annotati
+000276d0: 6f6e 2d46 6967 7572 650a 2020 2020 2020  on-Figure.      
+000276e0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e66        self.mne.f
+000276f0: 6967 5f61 6e6e 6f74 6174 696f 6e2e 7265  ig_annotation.re
+00027700: 7365 7428 290a 0a20 2020 2020 2020 2023  set()..        #
+00027710: 2053 686f 7720 416e 6e6f 7461 7469 6f6e   Show Annotation
+00027720: 2d44 6f63 6b20 6966 2061 6374 6976 6174  -Dock if activat
+00027730: 6564 2e0a 2020 2020 2020 2020 7365 6c66  ed..        self
+00027740: 2e6d 6e65 2e66 6967 5f61 6e6e 6f74 6174  .mne.fig_annotat
+00027750: 696f 6e2e 7365 7456 6973 6962 6c65 2873  ion.setVisible(s
+00027760: 656c 662e 6d6e 652e 616e 6e6f 7461 7469  elf.mne.annotati
+00027770: 6f6e 5f6d 6f64 6529 0a0a 2020 2020 2020  on_mode)..      
+00027780: 2020 2320 4d61 6b65 2052 6567 696f 6e73    # Make Regions
+00027790: 206d 6f76 6162 6c65 2069 6620 6163 7469   movable if acti
+000277a0: 7661 7465 6420 616e 6420 6d6f 7665 2069  vated and move i
+000277b0: 6e74 6f20 666f 7265 6772 6f75 6e64 0a20  nto foreground. 
+000277c0: 2020 2020 2020 2066 6f72 2072 6567 696f         for regio
+000277d0: 6e20 696e 2073 656c 662e 6d6e 652e 7265  n in self.mne.re
+000277e0: 6769 6f6e 733a 0a20 2020 2020 2020 2020  gions:.         
+000277f0: 2020 2072 6567 696f 6e2e 7365 744d 6f76     region.setMov
+00027800: 6162 6c65 2873 656c 662e 6d6e 652e 616e  able(self.mne.an
+00027810: 6e6f 7461 7469 6f6e 5f6d 6f64 6529 0a20  notation_mode). 
+00027820: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00027830: 6c66 2e6d 6e65 2e61 6e6e 6f74 6174 696f  lf.mne.annotatio
+00027840: 6e5f 6d6f 6465 3a0a 2020 2020 2020 2020  n_mode:.        
+00027850: 2020 2020 2020 2020 7265 6769 6f6e 2e73          region.s
+00027860: 6574 5a56 616c 7565 2832 290a 2020 2020  etZValue(2).    
+00027870: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00027880: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00027890: 6769 6f6e 2e73 6574 5a56 616c 7565 2830  gion.setZValue(0
+000278a0: 290a 0a20 2020 2020 2020 2023 2041 6464  )..        # Add
+000278b0: 2f52 656d 6f76 6520 7365 6c65 6374 696f  /Remove selectio
+000278c0: 6e2d 7265 6374 616e 676c 652e 0a20 2020  n-rectangle..   
+000278d0: 2020 2020 2069 6620 7365 6c66 2e6d 6e65       if self.mne
+000278e0: 2e73 656c 6563 7465 645f 7265 6769 6f6e  .selected_region
+000278f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00027900: 6c66 2e6d 6e65 2e73 656c 6563 7465 645f  lf.mne.selected_
+00027910: 7265 6769 6f6e 2e73 656c 6563 7428 7365  region.select(se
+00027920: 6c66 2e6d 6e65 2e61 6e6e 6f74 6174 696f  lf.mne.annotatio
+00027930: 6e5f 6d6f 6465 290a 0a20 2020 2064 6566  n_mode)..    def
+00027940: 205f 746f 6767 6c65 5f61 6e6e 6f74 6174   _toggle_annotat
+00027950: 696f 6e5f 6669 6728 7365 6c66 293a 0a20  ion_fig(self):. 
+00027960: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00027970: 6c66 2e6d 6e65 2e69 735f 6570 6f63 6873  lf.mne.is_epochs
+00027980: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00027990: 6c66 2e6d 6e65 2e61 6e6e 6f74 6174 696f  lf.mne.annotatio
+000279a0: 6e5f 6d6f 6465 203d 206e 6f74 2073 656c  n_mode = not sel
+000279b0: 662e 6d6e 652e 616e 6e6f 7461 7469 6f6e  f.mne.annotation
+000279c0: 5f6d 6f64 650a 2020 2020 2020 2020 2020  _mode.          
+000279d0: 2020 7365 6c66 2e5f 6368 616e 6765 5f61    self._change_a
+000279e0: 6e6e 6f74 5f6d 6f64 6528 290a 0a20 2020  nnot_mode()..   
+000279f0: 2064 6566 205f 7570 6461 7465 5f72 6567   def _update_reg
+00027a00: 696f 6e73 5f76 6973 6962 6c65 2873 656c  ions_visible(sel
+00027a10: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+00027a20: 656c 662e 6d6e 652e 6973 5f65 706f 6368  elf.mne.is_epoch
+00027a30: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+00027a40: 6574 7572 6e0a 2020 2020 2020 2020 7374  eturn.        st
+00027a50: 6172 7420 3d20 7365 6c66 2e6d 6e65 2e74  art = self.mne.t
+00027a60: 5f73 7461 7274 0a20 2020 2020 2020 2073  _start.        s
+00027a70: 746f 7020 3d20 7374 6172 7420 2b20 7365  top = start + se
+00027a80: 6c66 2e6d 6e65 2e64 7572 6174 696f 6e0a  lf.mne.duration.
+00027a90: 2020 2020 2020 2020 666f 7220 7265 6769          for regi
+00027aa0: 6f6e 2069 6e20 7365 6c66 2e6d 6e65 2e72  on in self.mne.r
+00027ab0: 6567 696f 6e73 3a0a 2020 2020 2020 2020  egions:.        
+00027ac0: 2020 2020 6966 2073 656c 662e 6d6e 652e      if self.mne.
+00027ad0: 7669 7369 626c 655f 616e 6e6f 7461 7469  visible_annotati
+00027ae0: 6f6e 735b 7265 6769 6f6e 2e64 6573 6372  ons[region.descr
+00027af0: 6970 7469 6f6e 5d3a 0a20 2020 2020 2020  iption]:.       
+00027b00: 2020 2020 2020 2020 2072 676e 203d 2072           rgn = r
+00027b10: 6567 696f 6e2e 6765 7452 6567 696f 6e28  egion.getRegion(
+00027b20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00027b30: 2020 2320 4176 6f69 6420 4e75 6d50 7920    # Avoid NumPy 
+00027b40: 626f 6f6c 2068 6572 650a 2020 2020 2020  bool here.      
+00027b50: 2020 2020 2020 2020 2020 7669 7369 626c            visibl
+00027b60: 6520 3d20 626f 6f6c 2872 676e 5b30 5d20  e = bool(rgn[0] 
+00027b70: 3c3d 2073 746f 7020 616e 6420 7267 6e5b  <= stop and rgn[
+00027b80: 315d 203e 3d20 7374 6172 7429 0a20 2020  1] >= start).   
+00027b90: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00027ba0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00027bb0: 6973 6962 6c65 203d 2046 616c 7365 0a20  isible = False. 
+00027bc0: 2020 2020 2020 2020 2020 2072 6567 696f             regio
+00027bd0: 6e2e 7570 6461 7465 5f76 6973 6962 6c65  n.update_visible
+00027be0: 2876 6973 6962 6c65 290a 2020 2020 2020  (visible).      
+00027bf0: 2020 7365 6c66 2e6d 6e65 2e6f 7665 7276    self.mne.overv
+00027c00: 6965 775f 6261 722e 7570 6461 7465 5f61  iew_bar.update_a
+00027c10: 6e6e 6f74 6174 696f 6e73 2829 0a0a 2020  nnotations()..  
+00027c20: 2020 6465 6620 5f73 6574 5f61 6e6e 6f74    def _set_annot
+00027c30: 6174 696f 6e73 5f76 6973 6962 6c65 2873  ations_visible(s
+00027c40: 656c 662c 2076 6973 6962 6c65 293a 0a20  elf, visible):. 
+00027c50: 2020 2020 2020 2066 6f72 2064 6573 6372         for descr
+00027c60: 2069 6e20 7365 6c66 2e6d 6e65 2e76 6973   in self.mne.vis
+00027c70: 6962 6c65 5f61 6e6e 6f74 6174 696f 6e73  ible_annotations
+00027c80: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00027c90: 6c66 2e6d 6e65 2e76 6973 6962 6c65 5f61  lf.mne.visible_a
+00027ca0: 6e6e 6f74 6174 696f 6e73 5b64 6573 6372  nnotations[descr
+00027cb0: 5d20 3d20 7669 7369 626c 650a 2020 2020  ] = visible.    
+00027cc0: 2020 2020 7365 6c66 2e5f 7570 6461 7465      self._update
+00027cd0: 5f72 6567 696f 6e73 5f76 6973 6962 6c65  _regions_visible
+00027ce0: 2829 0a0a 2020 2020 6465 6620 5f74 6f67  ()..    def _tog
+00027cf0: 676c 655f 616e 6e6f 7461 7469 6f6e 7328  gle_annotations(
+00027d00: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00027d10: 656c 662e 6d6e 652e 616e 6e6f 7461 7469  elf.mne.annotati
+00027d20: 6f6e 735f 7669 7369 626c 6520 3d20 6e6f  ons_visible = no
+00027d30: 7420 7365 6c66 2e6d 6e65 2e61 6e6e 6f74  t self.mne.annot
+00027d40: 6174 696f 6e73 5f76 6973 6962 6c65 0a20  ations_visible. 
+00027d50: 2020 2020 2020 2073 656c 662e 5f73 6574         self._set
+00027d60: 5f61 6e6e 6f74 6174 696f 6e73 5f76 6973  _annotations_vis
+00027d70: 6962 6c65 2873 656c 662e 6d6e 652e 616e  ible(self.mne.an
+00027d80: 6e6f 7461 7469 6f6e 735f 7669 7369 626c  notations_visibl
+00027d90: 6529 0a0a 2020 2020 6465 6620 5f61 7070  e)..    def _app
+00027da0: 6c79 5f75 7064 6174 655f 7072 6f6a 6563  ly_update_projec
+00027db0: 746f 7273 2873 656c 662c 2074 6f67 676c  tors(self, toggl
+00027dc0: 655f 616c 6c3d 4661 6c73 6529 3a0a 2020  e_all=False):.  
+00027dd0: 2020 2020 2020 6966 2074 6f67 676c 655f        if toggle_
+00027de0: 616c 6c3a 0a20 2020 2020 2020 2020 2020  all:.           
+00027df0: 206f 6e20 3d20 7365 6c66 2e6d 6e65 2e70   on = self.mne.p
+00027e00: 726f 6a73 5f6f 6e0a 2020 2020 2020 2020  rojs_on.        
+00027e10: 2020 2020 6170 706c 6965 6420 3d20 7365      applied = se
+00027e20: 6c66 2e6d 6e65 2e70 726f 6a73 5f61 6374  lf.mne.projs_act
+00027e30: 6976 650a 2020 2020 2020 2020 2020 2020  ive.            
+00027e40: 7661 6c75 6520 3d20 4661 6c73 6520 6966  value = False if
+00027e50: 2061 6c6c 286f 6e29 2065 6c73 6520 5472   all(on) else Tr
+00027e60: 7565 0a20 2020 2020 2020 2020 2020 206e  ue.            n
+00027e70: 6577 5f73 7461 7465 203d 206e 702e 6675  ew_state = np.fu
+00027e80: 6c6c 5f6c 696b 6528 6f6e 2c20 7661 6c75  ll_like(on, valu
+00027e90: 6529 0a20 2020 2020 2020 2020 2020 2023  e).            #
+00027ea0: 2041 6c77 6179 7320 6163 7469 7661 7465   Always activate
+00027eb0: 2061 7070 6c69 6564 2070 726f 6a65 6374   applied project
+00027ec0: 696f 6e73 0a20 2020 2020 2020 2020 2020  ions.           
+00027ed0: 206e 6577 5f73 7461 7465 5b61 7070 6c69   new_state[appli
+00027ee0: 6564 5d20 3d20 5472 7565 0a20 2020 2020  ed] = True.     
+00027ef0: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
+00027f00: 7072 6f6a 735f 6f6e 203d 206e 6577 5f73  projs_on = new_s
+00027f10: 7461 7465 0a20 2020 2020 2020 2073 656c  tate.        sel
+00027f20: 662e 5f75 7064 6174 655f 7072 6f6a 6563  f._update_projec
+00027f30: 746f 7228 290a 2020 2020 2020 2020 2320  tor().        # 
+00027f40: 4966 2064 6174 6120 7761 7320 7072 6563  If data was prec
+00027f50: 6f6d 7075 7465 6420 6974 206e 6565 6473  omputed it needs
+00027f60: 2074 6f20 6265 2070 7265 636f 6d70 7574   to be precomput
+00027f70: 6564 2061 6761 696e 2e0a 2020 2020 2020  ed again..      
+00027f80: 2020 7365 6c66 2e5f 7265 7275 6e5f 7072    self._rerun_pr
+00027f90: 6563 6f6d 7075 7465 2829 0a20 2020 2020  ecompute().     
+00027fa0: 2020 2073 656c 662e 5f72 6564 7261 7728     self._redraw(
+00027fb0: 290a 0a20 2020 2064 6566 205f 746f 6767  )..    def _togg
+00027fc0: 6c65 5f70 726f 6a5f 6669 6728 7365 6c66  le_proj_fig(self
+00027fd0: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+00027fe0: 6c66 2e6d 6e65 2e66 6967 5f70 726f 6a20  lf.mne.fig_proj 
+00027ff0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00028000: 2020 2020 2050 726f 6a44 6961 6c6f 6728       ProjDialog(
+00028010: 7365 6c66 2c20 6e61 6d65 3d27 6669 675f  self, name='fig_
+00028020: 7072 6f6a 2729 0a20 2020 2020 2020 2065  proj').        e
+00028030: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00028040: 2073 656c 662e 6d6e 652e 6669 675f 7072   self.mne.fig_pr
+00028050: 6f6a 2e63 6c6f 7365 2829 0a20 2020 2020  oj.close().     
+00028060: 2020 2020 2020 2073 656c 662e 6d6e 652e         self.mne.
+00028070: 6669 675f 7072 6f6a 203d 204e 6f6e 650a  fig_proj = None.
+00028080: 0a20 2020 2064 6566 205f 746f 6767 6c65  .    def _toggle
+00028090: 5f61 6c6c 5f70 726f 6a73 2873 656c 6629  _all_projs(self)
+000280a0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+000280b0: 662e 6d6e 652e 6669 675f 7072 6f6a 2069  f.mne.fig_proj i
+000280c0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000280d0: 2020 2020 7365 6c66 2e5f 6170 706c 795f      self._apply_
+000280e0: 7570 6461 7465 5f70 726f 6a65 6374 6f72  update_projector
+000280f0: 7328 746f 6767 6c65 5f61 6c6c 3d54 7275  s(toggle_all=Tru
+00028100: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
+00028110: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00028120: 662e 6d6e 652e 6669 675f 7072 6f6a 2e74  f.mne.fig_proj.t
+00028130: 6f67 676c 655f 616c 6c28 290a 0a20 2020  oggle_all()..   
+00028140: 2064 6566 205f 746f 6767 6c65 5f77 6869   def _toggle_whi
+00028150: 7465 6e69 6e67 2873 656c 6629 3a0a 2020  tening(self):.  
+00028160: 2020 2020 2020 6966 2073 656c 662e 6d6e        if self.mn
+00028170: 652e 6e6f 6973 655f 636f 7620 6973 206e  e.noise_cov is n
+00028180: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00028190: 2020 2020 2073 7570 6572 2829 2e5f 746f       super()._to
+000281a0: 6767 6c65 5f77 6869 7465 6e69 6e67 2829  ggle_whitening()
+000281b0: 0a20 2020 2020 2020 2020 2020 2023 2049  .            # I
+000281c0: 6620 6461 7461 2077 6173 2070 7265 636f  f data was preco
+000281d0: 6d70 7574 6564 2069 7420 6e65 6564 7320  mputed it needs 
+000281e0: 746f 2062 6520 7072 6563 6f6d 7075 7465  to be precompute
+000281f0: 6420 6167 6169 6e2e 0a20 2020 2020 2020  d again..       
+00028200: 2020 2020 2073 656c 662e 5f72 6572 756e       self._rerun
+00028210: 5f70 7265 636f 6d70 7574 6528 290a 2020  _precompute().  
+00028220: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00028230: 7265 6472 6177 2829 0a0a 2020 2020 6465  redraw()..    de
+00028240: 6620 5f74 6f67 676c 655f 7365 7474 696e  f _toggle_settin
+00028250: 6773 5f66 6967 2873 656c 6629 3a0a 2020  gs_fig(self):.  
+00028260: 2020 2020 2020 6966 2073 656c 662e 6d6e        if self.mn
+00028270: 652e 6669 675f 7365 7474 696e 6773 2069  e.fig_settings i
+00028280: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00028290: 2020 2020 5365 7474 696e 6773 4469 616c      SettingsDial
+000282a0: 6f67 2873 656c 662c 206e 616d 653d 2766  og(self, name='f
+000282b0: 6967 5f73 6574 7469 6e67 7327 290a 2020  ig_settings').  
+000282c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000282d0: 2020 2020 2020 2020 7365 6c66 2e6d 6e65          self.mne
+000282e0: 2e66 6967 5f73 6574 7469 6e67 732e 636c  .fig_settings.cl
+000282f0: 6f73 6528 290a 2020 2020 2020 2020 2020  ose().          
+00028300: 2020 7365 6c66 2e6d 6e65 2e66 6967 5f73    self.mne.fig_s
+00028310: 6574 7469 6e67 7320 3d20 4e6f 6e65 0a0a  ettings = None..
+00028320: 2020 2020 6465 6620 5f74 6f67 676c 655f      def _toggle_
+00028330: 6865 6c70 5f66 6967 2873 656c 6629 3a0a  help_fig(self):.
+00028340: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00028350: 6d6e 652e 6669 675f 6865 6c70 2069 7320  mne.fig_help is 
+00028360: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00028370: 2020 4865 6c70 4469 616c 6f67 2873 656c    HelpDialog(sel
+00028380: 662c 206e 616d 653d 2766 6967 5f68 656c  f, name='fig_hel
+00028390: 7027 290a 2020 2020 2020 2020 656c 7365  p').        else
+000283a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000283b0: 6c66 2e6d 6e65 2e66 6967 5f68 656c 702e  lf.mne.fig_help.
+000283c0: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
+000283d0: 2020 2020 7365 6c66 2e6d 6e65 2e66 6967      self.mne.fig
+000283e0: 5f68 656c 7020 3d20 4e6f 6e65 0a0a 2020  _help = None..  
+000283f0: 2020 6465 6620 5f73 6574 5f62 7574 7465    def _set_butte
+00028400: 7266 6c79 2873 656c 662c 2062 7574 7465  rfly(self, butte
+00028410: 7266 6c79 293a 0a20 2020 2020 2020 2073  rfly):.        s
+00028420: 656c 662e 6d6e 652e 6275 7474 6572 666c  elf.mne.butterfl
+00028430: 7920 3d20 6275 7474 6572 666c 790a 2020  y = butterfly.  
+00028440: 2020 2020 2020 7365 6c66 2e5f 7570 6461        self._upda
+00028450: 7465 5f70 6963 6b73 2829 0a20 2020 2020  te_picks().     
+00028460: 2020 2073 656c 662e 5f75 7064 6174 655f     self._update_
+00028470: 6461 7461 2829 0a0a 2020 2020 2020 2020  data()..        
+00028480: 6966 2062 7574 7465 7266 6c79 2061 6e64  if butterfly and
+00028490: 2073 656c 662e 6d6e 652e 6669 675f 7365   self.mne.fig_se
+000284a0: 6c65 6374 696f 6e20 6973 206e 6f74 204e  lection is not N
+000284b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000284c0: 2073 656c 662e 6d6e 652e 7365 6c65 6374   self.mne.select
+000284d0: 696f 6e5f 7970 6f73 5f64 6963 742e 636c  ion_ypos_dict.cl
+000284e0: 6561 7228 290a 2020 2020 2020 2020 2020  ear().          
+000284f0: 2020 7365 6c65 6374 696f 6e73 5f64 6963    selections_dic
+00028500: 7420 3d20 7365 6c66 2e5f 6d61 6b65 5f62  t = self._make_b
+00028510: 7574 7465 7266 6c79 5f73 656c 6563 7469  utterfly_selecti
+00028520: 6f6e 735f 6469 6374 2829 0a20 2020 2020  ons_dict().     
+00028530: 2020 2020 2020 2066 6f72 2069 6478 2c20         for idx, 
+00028540: 7069 636b 7320 696e 2065 6e75 6d65 7261  picks in enumera
+00028550: 7465 2873 656c 6563 7469 6f6e 735f 6469  te(selections_di
+00028560: 6374 2e76 616c 7565 7328 2929 3a0a 2020  ct.values()):.  
+00028570: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00028580: 7220 7069 636b 2069 6e20 7069 636b 733a  r pick in picks:
+00028590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000285a0: 2020 2020 2073 656c 662e 6d6e 652e 7365       self.mne.se
+000285b0: 6c65 6374 696f 6e5f 7970 6f73 5f64 6963  lection_ypos_dic
+000285c0: 745b 7069 636b 5d20 3d20 6964 7820 2b20  t[pick] = idx + 
+000285d0: 310a 2020 2020 2020 2020 2020 2020 796d  1.            ym
+000285e0: 6178 203d 206c 656e 2873 656c 6563 7469  ax = len(selecti
+000285f0: 6f6e 735f 6469 6374 2920 2b20 310a 2020  ons_dict) + 1.  
+00028600: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00028610: 6e65 2e79 6d61 7820 3d20 796d 6178 0a20  ne.ymax = ymax. 
+00028620: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00028630: 6d6e 652e 706c 742e 7365 744c 696d 6974  mne.plt.setLimit
+00028640: 7328 794d 6178 3d79 6d61 7829 0a20 2020  s(yMax=ymax).   
+00028650: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
+00028660: 652e 706c 742e 7365 7459 5261 6e67 6528  e.plt.setYRange(
+00028670: 302c 2079 6d61 782c 2070 6164 6469 6e67  0, ymax, padding
+00028680: 3d30 290a 2020 2020 2020 2020 656c 6966  =0).        elif
+00028690: 2062 7574 7465 7266 6c79 3a0a 2020 2020   butterfly:.    
+000286a0: 2020 2020 2020 2020 796d 6178 203d 206c          ymax = l
+000286b0: 656e 2873 656c 662e 6d6e 652e 6275 7474  en(self.mne.butt
+000286c0: 6572 666c 795f 7479 7065 5f6f 7264 6572  erfly_type_order
+000286d0: 2920 2b20 310a 2020 2020 2020 2020 2020  ) + 1.          
+000286e0: 2020 7365 6c66 2e6d 6e65 2e79 6d61 7820    self.mne.ymax 
+000286f0: 3d20 796d 6178 0a20 2020 2020 2020 2020  = ymax.         
+00028700: 2020 2073 656c 662e 6d6e 652e 706c 742e     self.mne.plt.
+00028710: 7365 744c 696d 6974 7328 794d 6178 3d79  setLimits(yMax=y
+00028720: 6d61 7829 0a20 2020 2020 2020 2020 2020  max).           
+00028730: 2073 656c 662e 6d6e 652e 706c 742e 7365   self.mne.plt.se
+00028740: 7459 5261 6e67 6528 302c 2079 6d61 782c  tYRange(0, ymax,
+00028750: 2070 6164 6469 6e67 3d30 290a 2020 2020   padding=0).    
+00028760: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00028770: 2020 2020 2020 7365 6c66 2e6d 6e65 2e79        self.mne.y
+00028780: 6d61 7820 3d20 6c65 6e28 7365 6c66 2e6d  max = len(self.m
+00028790: 6e65 2e63 685f 6f72 6465 7229 202b 2031  ne.ch_order) + 1
+000287a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000287b0: 662e 6d6e 652e 706c 742e 7365 744c 696d  f.mne.plt.setLim
+000287c0: 6974 7328 794d 6178 3d73 656c 662e 6d6e  its(yMax=self.mn
+000287d0: 652e 796d 6178 290a 2020 2020 2020 2020  e.ymax).        
+000287e0: 2020 2020 7365 6c66 2e6d 6e65 2e70 6c74      self.mne.plt
+000287f0: 2e73 6574 5952 616e 6765 2873 656c 662e  .setYRange(self.
+00028800: 6d6e 652e 6368 5f73 7461 7274 2c0a 2020  mne.ch_start,.  
+00028810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028830: 2073 656c 662e 6d6e 652e 6368 5f73 7461   self.mne.ch_sta
+00028840: 7274 202b 2073 656c 662e 6d6e 652e 6e5f  rt + self.mne.n_
+00028850: 6368 616e 6e65 6c73 202b 2031 2c0a 2020  channels + 1,.  
+00028860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028880: 2070 6164 6469 6e67 3d30 290a 0a20 2020   padding=0)..   
+00028890: 2020 2020 2069 6620 7365 6c66 2e6d 6e65       if self.mne
+000288a0: 2e66 6967 5f73 656c 6563 7469 6f6e 2069  .fig_selection i
+000288b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000288c0: 2020 2020 2020 2020 2320 5570 6461 7465          # Update
+000288d0: 2053 656c 6563 7469 6f6e 2d44 6961 6c6f   Selection-Dialo
+000288e0: 670a 2020 2020 2020 2020 2020 2020 7365  g.            se
+000288f0: 6c66 2e6d 6e65 2e66 6967 5f73 656c 6563  lf.mne.fig_selec
+00028900: 7469 6f6e 2e5f 7374 796c 655f 6275 7474  tion._style_butt
+00028910: 6572 666c 7928 290a 0a20 2020 2020 2020  erfly()..       
+00028920: 2023 2053 6574 2076 6572 7469 6361 6c20   # Set vertical 
+00028930: 7363 726f 6c6c 6261 7220 7669 7369 626c  scrollbar visibl
+00028940: 650a 2020 2020 2020 2020 7365 6c66 2e6d  e.        self.m
+00028950: 6e65 2e61 785f 7673 6372 6f6c 6c2e 7365  ne.ax_vscroll.se
+00028960: 7456 6973 6962 6c65 286e 6f74 2062 7574  tVisible(not but
+00028970: 7465 7266 6c79 206f 720a 2020 2020 2020  terfly or.      
+00028980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000289a0: 2073 656c 662e 6d6e 652e 6669 675f 7365   self.mne.fig_se
+000289b0: 6c65 6374 696f 6e20 6973 206e 6f74 204e  lection is not N
+000289c0: 6f6e 6529 0a0a 2020 2020 2020 2020 2320  one)..        # 
+000289d0: 7570 6461 7465 206f 7665 7276 6965 772d  update overview-
+000289e0: 6261 720a 2020 2020 2020 2020 7365 6c66  bar.        self
+000289f0: 2e6d 6e65 2e6f 7665 7276 6965 775f 6261  .mne.overview_ba
+00028a00: 722e 7570 6461 7465 5f76 6965 7772 616e  r.update_viewran
+00028a10: 6765 2829 0a0a 2020 2020 2020 2020 2320  ge()..        # 
+00028a20: 7570 6461 7465 2079 706f 7320 616e 6420  update ypos and 
+00028a30: 636f 6c6f 7220 666f 7220 6275 7474 6572  color for butter
+00028a40: 666c 792d 6d6f 6465 0a20 2020 2020 2020  fly-mode.       
+00028a50: 2066 6f72 2074 7261 6365 2069 6e20 7365   for trace in se
+00028a60: 6c66 2e6d 6e65 2e74 7261 6365 733a 0a20  lf.mne.traces:. 
+00028a70: 2020 2020 2020 2020 2020 2074 7261 6365             trace
+00028a80: 2e75 7064 6174 655f 636f 6c6f 7228 290a  .update_color().
+00028a90: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+00028aa0: 652e 7570 6461 7465 5f79 706f 7328 290a  e.update_ypos().
+00028ab0: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
+00028ac0: 7261 775f 7472 6163 6573 2829 0a0a 2020  raw_traces()..  
+00028ad0: 2020 6465 6620 5f74 6f67 676c 655f 6275    def _toggle_bu
+00028ae0: 7474 6572 666c 7928 7365 6c66 293a 0a20  tterfly(self):. 
+00028af0: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00028b00: 6e65 2e69 6e73 7461 6e63 655f 7479 7065  ne.instance_type
+00028b10: 2021 3d20 2769 6361 273a 0a20 2020 2020   != 'ica':.     
+00028b20: 2020 2020 2020 2073 656c 662e 5f73 6574         self._set
+00028b30: 5f62 7574 7465 7266 6c79 286e 6f74 2073  _butterfly(not s
+00028b40: 656c 662e 6d6e 652e 6275 7474 6572 666c  elf.mne.butterfl
+00028b50: 7929 0a0a 2020 2020 6465 6620 5f74 6f67  y)..    def _tog
+00028b60: 676c 655f 6463 2873 656c 6629 3a0a 2020  gle_dc(self):.  
+00028b70: 2020 2020 2020 7365 6c66 2e6d 6e65 2e72        self.mne.r
+00028b80: 656d 6f76 655f 6463 203d 206e 6f74 2073  emove_dc = not s
+00028b90: 656c 662e 6d6e 652e 7265 6d6f 7665 5f64  elf.mne.remove_d
+00028ba0: 630a 2020 2020 2020 2020 7365 6c66 2e5f  c.        self._
+00028bb0: 7265 6472 6177 2829 0a0a 2020 2020 6465  redraw()..    de
+00028bc0: 6620 5f74 6f67 676c 655f 6570 6f63 685f  f _toggle_epoch_
+00028bd0: 6869 7374 6f67 7261 6d28 7365 6c66 293a  histogram(self):
+00028be0: 0a20 2020 2020 2020 2066 6967 203d 2073  .        fig = s
+00028bf0: 656c 662e 5f63 7265 6174 655f 6570 6f63  elf._create_epoc
+00028c00: 685f 6869 7374 6f67 7261 6d28 290a 2020  h_histogram().  
+00028c10: 2020 2020 2020 7365 6c66 2e5f 6765 745f        self._get_
+00028c20: 646c 675f 6672 6f6d 5f6d 706c 2866 6967  dlg_from_mpl(fig
+00028c30: 290a 0a20 2020 2064 6566 205f 7365 745f  )..    def _set_
+00028c40: 6576 656e 7473 5f76 6973 6962 6c65 2873  events_visible(s
+00028c50: 656c 662c 2076 6973 6962 6c65 293a 0a20  elf, visible):. 
+00028c60: 2020 2020 2020 2066 6f72 2065 7665 6e74         for event
+00028c70: 5f6c 696e 6520 696e 2073 656c 662e 6d6e  _line in self.mn
+00028c80: 652e 6576 656e 745f 6c69 6e65 733a 0a20  e.event_lines:. 
+00028c90: 2020 2020 2020 2020 2020 2065 7665 6e74             event
+00028ca0: 5f6c 696e 652e 7365 7456 6973 6962 6c65  _line.setVisible
+00028cb0: 2876 6973 6962 6c65 290a 0a20 2020 2020  (visible)..     
+00028cc0: 2020 2073 656c 662e 6d6e 652e 6f76 6572     self.mne.over
+00028cd0: 7669 6577 5f62 6172 2e75 7064 6174 655f  view_bar.update_
+00028ce0: 6576 656e 7473 2829 0a0a 2020 2020 6465  events()..    de
+00028cf0: 6620 5f74 6f67 676c 655f 6576 656e 7473  f _toggle_events
+00028d00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00028d10: 6966 2073 656c 662e 6d6e 652e 6576 656e  if self.mne.even
+00028d20: 745f 6e75 6d73 2069 7320 6e6f 7420 4e6f  t_nums is not No
+00028d30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00028d40: 7365 6c66 2e6d 6e65 2e65 7665 6e74 735f  self.mne.events_
+00028d50: 7669 7369 626c 6520 3d20 6e6f 7420 7365  visible = not se
+00028d60: 6c66 2e6d 6e65 2e65 7665 6e74 735f 7669  lf.mne.events_vi
+00028d70: 7369 626c 650a 2020 2020 2020 2020 2020  sible.          
+00028d80: 2020 7365 6c66 2e5f 7365 745f 6576 656e    self._set_even
+00028d90: 7473 5f76 6973 6962 6c65 2873 656c 662e  ts_visible(self.
+00028da0: 6d6e 652e 6576 656e 7473 5f76 6973 6962  mne.events_visib
+00028db0: 6c65 290a 0a20 2020 2064 6566 205f 746f  le)..    def _to
+00028dc0: 6767 6c65 5f74 696d 655f 666f 726d 6174  ggle_time_format
+00028dd0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00028de0: 6966 2073 656c 662e 6d6e 652e 7469 6d65  if self.mne.time
+00028df0: 5f66 6f72 6d61 7420 3d3d 2027 666c 6f61  _format == 'floa
+00028e00: 7427 3a0a 2020 2020 2020 2020 2020 2020  t':.            
+00028e10: 7365 6c66 2e6d 6e65 2e74 696d 655f 666f  self.mne.time_fo
+00028e20: 726d 6174 203d 2027 636c 6f63 6b27 0a20  rmat = 'clock'. 
+00028e30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00028e40: 6d6e 652e 7469 6d65 5f61 7869 732e 7365  mne.time_axis.se
+00028e50: 744c 6162 656c 2874 6578 743d 2754 696d  tLabel(text='Tim
+00028e60: 6520 6f66 2064 6179 2729 0a20 2020 2020  e of day').     
+00028e70: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00028e80: 2020 2020 2073 656c 662e 6d6e 652e 7469       self.mne.ti
+00028e90: 6d65 5f66 6f72 6d61 7420 3d20 2766 6c6f  me_format = 'flo
+00028ea0: 6174 270a 2020 2020 2020 2020 2020 2020  at'.            
+00028eb0: 7365 6c66 2e6d 6e65 2e74 696d 655f 6178  self.mne.time_ax
+00028ec0: 6973 2e73 6574 4c61 6265 6c28 7465 7874  is.setLabel(text
+00028ed0: 3d27 5469 6d65 272c 2075 6e69 7473 3d27  ='Time', units='
+00028ee0: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
+00028ef0: 2e5f 7570 6461 7465 5f79 6178 6973 5f6c  ._update_yaxis_l
+00028f00: 6162 656c 7328 290a 0a20 2020 2064 6566  abels()..    def
+00028f10: 205f 746f 6767 6c65 5f66 756c 6c73 6372   _toggle_fullscr
+00028f20: 6565 6e28 7365 6c66 293a 0a20 2020 2020  een(self):.     
+00028f30: 2020 2069 6620 7365 6c66 2e69 7346 756c     if self.isFul
+00028f40: 6c53 6372 6565 6e28 293a 0a20 2020 2020  lScreen():.     
+00028f50: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
+00028f60: 4e6f 726d 616c 2829 0a20 2020 2020 2020  Normal().       
+00028f70: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00028f80: 2020 2073 656c 662e 7368 6f77 4675 6c6c     self.showFull
+00028f90: 5363 7265 656e 2829 0a0a 2020 2020 6465  Screen()..    de
+00028fa0: 6620 5f74 6f67 676c 655f 616e 7469 616c  f _toggle_antial
+00028fb0: 6961 7369 6e67 2873 656c 6629 3a0a 2020  iasing(self):.  
+00028fc0: 2020 2020 2020 7365 6c66 2e6d 6e65 2e61        self.mne.a
+00028fd0: 6e74 6961 6c69 6173 696e 6720 3d20 6e6f  ntialiasing = no
+00028fe0: 7420 7365 6c66 2e6d 6e65 2e61 6e74 6961  t self.mne.antia
+00028ff0: 6c69 6173 696e 670a 2020 2020 2020 2020  liasing.        
+00029000: 7365 6c66 2e5f 7265 6472 6177 2829 0a0a  self._redraw()..
+00029010: 2020 2020 6465 6620 5f74 6f67 676c 655f      def _toggle_
+00029020: 6f76 6572 7669 6577 5f62 6172 2873 656c  overview_bar(sel
+00029030: 6629 3a0a 2020 2020 2020 2020 7669 7369  f):.        visi
+00029040: 626c 6520 3d20 6e6f 7420 7365 6c66 2e6d  ble = not self.m
+00029050: 6e65 2e6f 7665 7276 6965 775f 6261 722e  ne.overview_bar.
+00029060: 6973 5669 7369 626c 6528 290a 2020 2020  isVisible().    
+00029070: 2020 2020 666f 7220 6974 656d 2069 6e20      for item in 
+00029080: 7365 6c66 2e6d 6e65 2e6f 7665 7276 6965  self.mne.overvie
+00029090: 775f 6d65 6e75 2e61 6374 696f 6e73 2829  w_menu.actions()
+000290a0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000290b0: 2069 7465 6d2e 7465 7874 2829 203d 3d20   item.text() == 
+000290c0: 2756 6973 6962 6c65 273a 0a20 2020 2020  'Visible':.     
+000290d0: 2020 2020 2020 2020 2020 2069 7465 6d2e             item.
+000290e0: 7365 7443 6865 636b 6564 2876 6973 6962  setChecked(visib
+000290f0: 6c65 290a 2020 2020 2020 2020 2020 2020  le).            
+00029100: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+00029110: 2020 7365 6c66 2e6d 6e65 2e6f 7665 7276    self.mne.overv
+00029120: 6965 775f 6261 722e 7365 7456 6973 6962  iew_bar.setVisib
+00029130: 6c65 2876 6973 6962 6c65 290a 0a20 2020  le(visible)..   
+00029140: 2064 6566 205f 746f 6767 6c65 5f7a 656e   def _toggle_zen
+00029150: 6d6f 6465 2873 656c 6629 3a0a 2020 2020  mode(self):.    
+00029160: 2020 2020 7365 6c66 2e6d 6e65 2e73 6372      self.mne.scr
+00029170: 6f6c 6c62 6172 735f 7669 7369 626c 6520  ollbars_visible 
+00029180: 3d20 6e6f 7420 7365 6c66 2e6d 6e65 2e73  = not self.mne.s
+00029190: 6372 6f6c 6c62 6172 735f 7669 7369 626c  crollbars_visibl
+000291a0: 650a 2020 2020 2020 2020 666f 7220 6261  e.        for ba
+000291b0: 7220 696e 205b 7365 6c66 2e6d 6e65 2e61  r in [self.mne.a
+000291c0: 785f 6873 6372 6f6c 6c2c 2073 656c 662e  x_hscroll, self.
+000291d0: 6d6e 652e 6178 5f76 7363 726f 6c6c 5d3a  mne.ax_vscroll]:
+000291e0: 0a20 2020 2020 2020 2020 2020 2062 6172  .            bar
+000291f0: 2e73 6574 5669 7369 626c 6528 7365 6c66  .setVisible(self
+00029200: 2e6d 6e65 2e73 6372 6f6c 6c62 6172 735f  .mne.scrollbars_
+00029210: 7669 7369 626c 6529 0a20 2020 2020 2020  visible).       
+00029220: 2073 656c 662e 6d6e 652e 746f 6f6c 6261   self.mne.toolba
+00029230: 722e 7365 7456 6973 6962 6c65 2873 656c  r.setVisible(sel
+00029240: 662e 6d6e 652e 7363 726f 6c6c 6261 7273  f.mne.scrollbars
+00029250: 5f76 6973 6962 6c65 290a 0a20 2020 2064  _visible)..    d
+00029260: 6566 205f 6e65 775f 6368 696c 645f 6669  ef _new_child_fi
+00029270: 6775 7265 2873 656c 662c 2066 6967 5f6e  gure(self, fig_n
+00029280: 616d 652c 2077 696e 646f 775f 7469 746c  ame, window_titl
+00029290: 652c 202a 2a6b 7761 7267 7329 3a0a 2020  e, **kwargs):.  
+000292a0: 2020 2020 2020 6672 6f6d 206d 6174 706c        from matpl
+000292b0: 6f74 6c69 622e 6669 6775 7265 2069 6d70  otlib.figure imp
+000292c0: 6f72 7420 4669 6775 7265 0a20 2020 2020  ort Figure.     
+000292d0: 2020 2066 6967 203d 2046 6967 7572 6528     fig = Figure(
+000292e0: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
+000292f0: 2020 2320 5061 7373 2077 696e 646f 7720    # Pass window 
+00029300: 7469 746c 6520 616e 6420 6669 675f 6e61  title and fig_na
+00029310: 6d65 206f 6e0a 2020 2020 2020 2020 6966  me on.        if
+00029320: 2066 6967 5f6e 616d 6520 6973 206e 6f74   fig_name is not
+00029330: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00029340: 2020 2066 6967 2e66 6967 5f6e 616d 6520     fig.fig_name 
+00029350: 3d20 6669 675f 6e61 6d65 0a20 2020 2020  = fig_name.     
+00029360: 2020 2069 6620 7769 6e64 6f77 5f74 6974     if window_tit
+00029370: 6c65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  le is not None:.
+00029380: 2020 2020 2020 2020 2020 2020 6669 672e              fig.
+00029390: 7469 746c 6520 3d20 7769 6e64 6f77 5f74  title = window_t
+000293a0: 6974 6c65 0a20 2020 2020 2020 2072 6574  itle.        ret
+000293b0: 7572 6e20 6669 670a 0a20 2020 2064 6566  urn fig..    def
+000293c0: 205f 6765 745f 7769 6467 6574 5f66 726f   _get_widget_fro
+000293d0: 6d5f 6d70 6c28 7365 6c66 2c20 6669 6729  m_mpl(self, fig)
+000293e0: 3a0a 2020 2020 2020 2020 6361 6e76 6173  :.        canvas
+000293f0: 203d 2046 6967 7572 6543 616e 7661 7351   = FigureCanvasQ
+00029400: 5441 6767 2866 6967 290a 2020 2020 2020  TAgg(fig).      
+00029410: 2020 6361 6e76 6173 2e73 6574 466f 6375    canvas.setFocu
+00029420: 7350 6f6c 6963 7928 5174 2e46 6f63 7573  sPolicy(Qt.Focus
+00029430: 506f 6c69 6379 2851 742e 5374 726f 6e67  Policy(Qt.Strong
+00029440: 466f 6375 7320 7c20 5174 2e57 6865 656c  Focus | Qt.Wheel
+00029450: 466f 6375 7329 290a 2020 2020 2020 2020  Focus)).        
+00029460: 6361 6e76 6173 2e73 6574 466f 6375 7328  canvas.setFocus(
+00029470: 290a 2020 2020 2020 2020 2320 5061 7373  ).        # Pass
+00029480: 2077 696e 646f 7720 7469 746c 6520 616e   window title an
+00029490: 6420 6669 675f 6e61 6d65 206f 6e0a 2020  d fig_name on.  
+000294a0: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
+000294b0: 2866 6967 2c20 2766 6967 5f6e 616d 6527  (fig, 'fig_name'
+000294c0: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+000294d0: 616e 7661 732e 6669 675f 6e61 6d65 203d  anvas.fig_name =
+000294e0: 2066 6967 2e66 6967 5f6e 616d 650a 2020   fig.fig_name.  
+000294f0: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
+00029500: 2866 6967 2c20 2774 6974 6c65 2729 3a0a  (fig, 'title'):.
+00029510: 2020 2020 2020 2020 2020 2020 6361 6e76              canv
+00029520: 6173 2e74 6974 6c65 203d 2066 6967 2e74  as.title = fig.t
+00029530: 6974 6c65 0a0a 2020 2020 2020 2020 7265  itle..        re
+00029540: 7475 726e 2063 616e 7661 730a 0a20 2020  turn canvas..   
+00029550: 2064 6566 205f 6765 745f 646c 675f 6672   def _get_dlg_fr
+00029560: 6f6d 5f6d 706c 2873 656c 662c 2066 6967  om_mpl(self, fig
+00029570: 293a 0a20 2020 2020 2020 2063 616e 7661  ):.        canva
+00029580: 7320 3d20 7365 6c66 2e5f 6765 745f 7769  s = self._get_wi
+00029590: 6467 6574 5f66 726f 6d5f 6d70 6c28 6669  dget_from_mpl(fi
+000295a0: 6729 0a20 2020 2020 2020 2023 2050 6173  g).        # Pas
+000295b0: 7320 7769 6e64 6f77 2074 6974 6c65 2061  s window title a
+000295c0: 6e64 2066 6967 5f6e 616d 6520 6f6e 0a20  nd fig_name on. 
+000295d0: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
+000295e0: 7228 6361 6e76 6173 2c20 2766 6967 5f6e  r(canvas, 'fig_n
+000295f0: 616d 6527 293a 0a20 2020 2020 2020 2020  ame'):.         
+00029600: 2020 206e 616d 6520 3d20 6361 6e76 6173     name = canvas
+00029610: 2e66 6967 5f6e 616d 650a 2020 2020 2020  .fig_name.      
+00029620: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00029630: 2020 2020 6e61 6d65 203d 204e 6f6e 650a      name = None.
+00029640: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
+00029650: 7472 2863 616e 7661 732c 2027 7469 746c  tr(canvas, 'titl
+00029660: 6527 293a 0a20 2020 2020 2020 2020 2020  e'):.           
+00029670: 2074 6974 6c65 203d 2063 616e 7661 732e   title = canvas.
+00029680: 7469 746c 650a 2020 2020 2020 2020 656c  title.        el
+00029690: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000296a0: 7469 746c 6520 3d20 4e6f 6e65 0a20 2020  title = None.   
+000296b0: 2020 2020 2064 6c67 203d 205f 4261 7365       dlg = _Base
+000296c0: 4469 616c 6f67 2873 656c 662c 2077 6964  Dialog(self, wid
+000296d0: 6765 743d 6361 6e76 6173 2c20 7469 746c  get=canvas, titl
+000296e0: 653d 7469 746c 652c 206e 616d 653d 6e61  e=title, name=na
+000296f0: 6d65 290a 2020 2020 2020 2020 646c 672e  me).        dlg.
+00029700: 7368 6f77 2829 0a0a 2020 2020 6465 6620  show()..    def 
+00029710: 5f63 7265 6174 655f 6368 5f63 6f6e 7465  _create_ch_conte
+00029720: 7874 5f66 6967 2873 656c 662c 2069 6478  xt_fig(self, idx
+00029730: 293a 0a20 2020 2020 2020 2066 6967 203d  ):.        fig =
+00029740: 2073 7570 6572 2829 2e5f 6372 6561 7465   super()._create
+00029750: 5f63 685f 636f 6e74 6578 745f 6669 6728  _ch_context_fig(
+00029760: 6964 7829 0a20 2020 2020 2020 2069 6620  idx).        if 
+00029770: 6669 6720 6973 206e 6f74 204e 6f6e 653a  fig is not None:
+00029780: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00029790: 662e 5f67 6574 5f64 6c67 5f66 726f 6d5f  f._get_dlg_from_
+000297a0: 6d70 6c28 6669 6729 0a0a 2020 2020 6465  mpl(fig)..    de
+000297b0: 6620 5f74 6f67 676c 655f 6570 6f63 685f  f _toggle_epoch_
+000297c0: 6869 7374 6f67 7261 6d6d 2873 656c 6629  histogramm(self)
+000297d0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+000297e0: 662e 6d6e 652e 6973 5f65 706f 6368 733a  f.mne.is_epochs:
+000297f0: 0a20 2020 2020 2020 2020 2020 2066 6967  .            fig
+00029800: 203d 2073 656c 662e 5f63 7265 6174 655f   = self._create_
+00029810: 6570 6f63 685f 6869 7374 6f67 7261 6d28  epoch_histogram(
+00029820: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00029830: 2066 6967 2069 7320 6e6f 7420 4e6f 6e65   fig is not None
+00029840: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00029850: 2020 7365 6c66 2e5f 6765 745f 646c 675f    self._get_dlg_
+00029860: 6672 6f6d 5f6d 706c 2866 6967 290a 0a20  from_mpl(fig).. 
+00029870: 2020 2064 6566 205f 6372 6561 7465 5f73     def _create_s
+00029880: 656c 6563 7469 6f6e 5f66 6967 2873 656c  election_fig(sel
+00029890: 6629 3a0a 2020 2020 2020 2020 6966 206e  f):.        if n
+000298a0: 6f74 2061 6e79 285b 6973 696e 7374 616e  ot any([isinstan
+000298b0: 6365 2866 6967 2c20 5365 6c65 6374 696f  ce(fig, Selectio
+000298c0: 6e44 6961 6c6f 6729 2066 6f72 0a20 2020  nDialog) for.   
+000298d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000298e0: 2066 6967 2069 6e20 7365 6c66 2e6d 6e65   fig in self.mne
+000298f0: 2e63 6869 6c64 5f66 6967 735d 293a 0a20  .child_figs]):. 
+00029900: 2020 2020 2020 2020 2020 2053 656c 6563             Selec
+00029910: 7469 6f6e 4469 616c 6f67 2873 656c 6629  tionDialog(self)
+00029920: 0a0a 2020 2020 6465 6620 6d65 7373 6167  ..    def messag
+00029930: 655f 626f 7828 7365 6c66 2c20 7465 7874  e_box(self, text
+00029940: 2c20 696e 666f 5f74 6578 743d 4e6f 6e65  , info_text=None
+00029950: 2c20 6275 7474 6f6e 733d 4e6f 6e65 2c0a  , buttons=None,.
+00029960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029970: 2020 2020 6465 6661 756c 745f 6275 7474      default_butt
+00029980: 6f6e 3d4e 6f6e 652c 2069 636f 6e3d 4e6f  on=None, icon=No
+00029990: 6e65 2c20 6d6f 6461 6c3d 5472 7565 293a  ne, modal=True):
+000299a0: 2020 2320 6e6f 7161 3a20 4431 3032 0a20    # noqa: D102. 
+000299b0: 2020 2020 2020 2073 656c 662e 6d73 675f         self.msg_
+000299c0: 626f 782e 7365 7454 6578 7428 6627 3c66  box.setText(f'<f
+000299d0: 6f6e 7420 7369 7a65 3d22 2b32 223e 3c62  ont size="+2"><b
+000299e0: 3e7b 7465 7874 7d3c 2f62 3e3c 2f66 6f6e  >{text}</b></fon
+000299f0: 743e 2729 0a20 2020 2020 2020 2069 6620  t>').        if 
+00029a00: 696e 666f 5f74 6578 7420 6973 206e 6f74  info_text is not
+00029a10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00029a20: 2020 2073 656c 662e 6d73 675f 626f 782e     self.msg_box.
+00029a30: 7365 7449 6e66 6f72 6d61 7469 7665 5465  setInformativeTe
+00029a40: 7874 2869 6e66 6f5f 7465 7874 290a 2020  xt(info_text).  
+00029a50: 2020 2020 2020 6966 2062 7574 746f 6e73        if buttons
+00029a60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00029a70: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00029a80: 7367 5f62 6f78 2e73 6574 5374 616e 6461  sg_box.setStanda
+00029a90: 7264 4275 7474 6f6e 7328 6275 7474 6f6e  rdButtons(button
+00029aa0: 7329 0a20 2020 2020 2020 2069 6620 6465  s).        if de
+00029ab0: 6661 756c 745f 6275 7474 6f6e 2069 7320  fault_button is 
+00029ac0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00029ad0: 2020 2020 2020 7365 6c66 2e6d 7367 5f62        self.msg_b
+00029ae0: 6f78 2e73 6574 4465 6661 756c 7442 7574  ox.setDefaultBut
+00029af0: 746f 6e28 6465 6661 756c 745f 6275 7474  ton(default_butt
+00029b00: 6f6e 290a 2020 2020 2020 2020 6966 2069  on).        if i
+00029b10: 636f 6e20 6973 206e 6f74 204e 6f6e 653a  con is not None:
+00029b20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00029b30: 662e 6d73 675f 626f 782e 7365 7449 636f  f.msg_box.setIco
+00029b40: 6e28 6963 6f6e 290a 0a20 2020 2020 2020  n(icon)..       
+00029b50: 2023 2041 6c6c 6f77 2069 6e74 6572 6163   # Allow interac
+00029b60: 7469 6e67 2077 6974 6820 6d65 7373 6167  ting with messag
+00029b70: 655f 626f 7820 696e 2074 6573 742d 6d6f  e_box in test-mo
+00029b80: 6465 2e0a 2020 2020 2020 2020 2320 5365  de..        # Se
+00029b90: 7420 6d6f 6461 6c3d 4661 6c73 6520 6f6e  t modal=False on
+00029ba0: 6c79 2069 6620 6e6f 2072 6574 7572 6e20  ly if no return 
+00029bb0: 7661 6c75 6520 6973 2065 7870 6563 7465  value is expecte
+00029bc0: 642e 0a20 2020 2020 2020 2073 656c 662e  d..        self.
+00029bd0: 6d73 675f 626f 782e 7365 744d 6f64 616c  msg_box.setModal
+00029be0: 2846 616c 7365 2069 6620 7365 6c66 2e74  (False if self.t
+00029bf0: 6573 745f 6d6f 6465 2065 6c73 6520 6d6f  est_mode else mo
+00029c00: 6461 6c29 0a20 2020 2020 2020 2069 6620  dal).        if 
+00029c10: 7365 6c66 2e74 6573 745f 6d6f 6465 206f  self.test_mode o
+00029c20: 7220 6e6f 7420 6d6f 6461 6c3a 0a20 2020  r not modal:.   
+00029c30: 2020 2020 2020 2020 2073 656c 662e 6d73           self.ms
+00029c40: 675f 626f 782e 7368 6f77 2829 0a20 2020  g_box.show().   
+00029c50: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00029c60: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00029c70: 6c66 2e6d 7367 5f62 6f78 2e65 7865 6328  lf.msg_box.exec(
+00029c80: 290a 0a20 2020 2064 6566 206b 6579 5072  )..    def keyPr
+00029c90: 6573 7345 7665 6e74 2873 656c 662c 2065  essEvent(self, e
+00029ca0: 7665 6e74 293a 0a20 2020 2020 2020 2022  vent):.        "
+00029cb0: 2222 4375 7374 6f6d 697a 6520 6b65 7920  ""Customize key 
+00029cc0: 7072 6573 7320 6576 656e 7473 2e22 2222  press events."""
+00029cd0: 0a20 2020 2020 2020 2023 204f 6e20 4d61  .        # On Ma
+00029ce0: 634f 7320 6164 6469 7469 6f6e 616c 6c79  cOs additionally
+00029cf0: 204b 6579 7061 644d 6f64 6966 6965 7220   KeypadModifier 
+00029d00: 6973 2073 6574 2077 6865 6e20 6172 726f  is set when arro
+00029d10: 772d 6b65 7973 0a20 2020 2020 2020 2023  w-keys.        #
+00029d20: 2061 7265 2070 7265 7373 6564 2e0a 2020   are pressed..  
+00029d30: 2020 2020 2020 6d6f 6473 203d 2065 7665        mods = eve
+00029d40: 6e74 2e6d 6f64 6966 6965 7273 2829 0a20  nt.modifiers(). 
+00029d50: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00029d60: 2020 2020 2020 2020 6d6f 6473 203d 2069          mods = i
+00029d70: 6e74 286d 6f64 7329 2020 2320 5079 5174  nt(mods)  # PyQt
+00029d80: 203c 2035 2e31 330a 2020 2020 2020 2020   < 5.13.        
+00029d90: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00029da0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+00029db0: 7373 0a20 2020 2020 2020 206d 6f64 6966  ss.        modif
+00029dc0: 6965 7273 203d 207b 0a20 2020 2020 2020  iers = {.       
+00029dd0: 2020 2020 2027 5368 6966 7427 3a20 626f       'Shift': bo
+00029de0: 6f6c 2851 742e 5368 6966 744d 6f64 6966  ol(Qt.ShiftModif
+00029df0: 6965 7220 2620 6d6f 6473 292c 0a20 2020  ier & mods),.   
+00029e00: 2020 2020 2020 2020 2027 4374 726c 273a           'Ctrl':
+00029e10: 2062 6f6f 6c28 5174 2e43 6f6e 7472 6f6c   bool(Qt.Control
+00029e20: 4d6f 6469 6669 6572 2026 206d 6f64 7329  Modifier & mods)
+00029e30: 2c0a 2020 2020 2020 2020 7d0a 2020 2020  ,.        }.    
+00029e40: 2020 2020 666f 7220 6b65 795f 6e61 6d65      for key_name
+00029e50: 2069 6e20 7365 6c66 2e6d 6e65 2e6b 6579   in self.mne.key
+00029e60: 626f 6172 645f 7368 6f72 7463 7574 733a  board_shortcuts:
+00029e70: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
+00029e80: 5f64 6963 7420 3d20 7365 6c66 2e6d 6e65  _dict = self.mne
+00029e90: 2e6b 6579 626f 6172 645f 7368 6f72 7463  .keyboard_shortc
+00029ea0: 7574 735b 6b65 795f 6e61 6d65 5d0a 2020  uts[key_name].  
+00029eb0: 2020 2020 2020 2020 2020 6966 206b 6579            if key
+00029ec0: 5f64 6963 745b 2771 745f 6b65 7927 5d20  _dict['qt_key'] 
+00029ed0: 3d3d 2065 7665 6e74 2e6b 6579 2829 2061  == event.key() a
+00029ee0: 6e64 2027 736c 6f74 2720 696e 206b 6579  nd 'slot' in key
+00029ef0: 5f64 6963 743a 0a0a 2020 2020 2020 2020  _dict:..        
+00029f00: 2020 2020 2020 2020 6d6f 645f 6964 7820          mod_idx 
+00029f10: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
+00029f20: 2020 2020 2320 4765 7420 6d6f 6469 6669      # Get modifi
+00029f30: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
+00029f40: 2020 2069 6620 276d 6f64 6966 6965 7227     if 'modifier'
+00029f50: 2069 6e20 6b65 795f 6469 6374 3a0a 2020   in key_dict:.  
+00029f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029f70: 2020 6d6f 6473 203d 205b 6d6f 6469 6669    mods = [modifi
+00029f80: 6572 735b 6d6f 645d 2066 6f72 206d 6f64  ers[mod] for mod
+00029f90: 2069 6e20 6d6f 6469 6669 6572 735d 0a20   in modifiers]. 
+00029fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029fb0: 2020 2069 6620 616e 7928 6d6f 6473 293a     if any(mods):
+00029fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029fd0: 2020 2020 2020 2020 2023 204e 6f20 6d75           # No mu
+00029fe0: 6c74 6970 6c65 206d 6f64 6966 6965 7273  ltiple modifiers
+00029ff0: 2073 7570 706f 7274 6564 2079 6574 0a20   supported yet. 
+0002a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a010: 2020 2020 2020 206d 6f64 203d 205b 6d6f         mod = [mo
+0002a020: 6420 666f 7220 6d6f 6420 696e 206d 6f64  d for mod in mod
+0002a030: 6966 6965 7273 2069 6620 6d6f 6469 6669  ifiers if modifi
+0002a040: 6572 735b 6d6f 645d 5d5b 305d 0a20 2020  ers[mod]][0].   
+0002a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a060: 2020 2020 2069 6620 6d6f 6420 696e 206b       if mod in k
+0002a070: 6579 5f64 6963 745b 276d 6f64 6966 6965  ey_dict['modifie
+0002a080: 7227 5d3a 0a20 2020 2020 2020 2020 2020  r']:.           
+0002a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a0a0: 206d 6f64 5f69 6478 203d 206b 6579 5f64   mod_idx = key_d
+0002a0b0: 6963 745b 276d 6f64 6966 6965 7227 5d2e  ict['modifier'].
+0002a0c0: 696e 6465 7828 6d6f 6429 0a0a 2020 2020  index(mod)..    
+0002a0d0: 2020 2020 2020 2020 2020 2020 736c 6f74              slot
+0002a0e0: 5f69 6478 203d 206d 6f64 5f69 6478 2069  _idx = mod_idx i
+0002a0f0: 6620 6d6f 645f 6964 7820 3c20 6c65 6e28  f mod_idx < len(
+0002a100: 6b65 795f 6469 6374 5b27 736c 6f74 275d  key_dict['slot']
+0002a110: 2920 656c 7365 2030 0a20 2020 2020 2020  ) else 0.       
+0002a120: 2020 2020 2020 2020 2073 6c6f 7420 3d20           slot = 
+0002a130: 6b65 795f 6469 6374 5b27 736c 6f74 275d  key_dict['slot']
+0002a140: 5b73 6c6f 745f 6964 785d 0a0a 2020 2020  [slot_idx]..    
+0002a150: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+0002a160: 7061 7261 6d65 7465 7227 2069 6e20 6b65  parameter' in ke
+0002a170: 795f 6469 6374 3a0a 2020 2020 2020 2020  y_dict:.        
+0002a180: 2020 2020 2020 2020 2020 2020 7061 7261              para
+0002a190: 6d5f 6964 7820 3d20 286d 6f64 5f69 6478  m_idx = (mod_idx
+0002a1a0: 2069 6620 6d6f 645f 6964 7820 3c0a 2020   if mod_idx <.  
+0002a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a1c0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0002a1d0: 656e 286b 6579 5f64 6963 745b 2770 6172  en(key_dict['par
+0002a1e0: 616d 6574 6572 275d 2920 656c 7365 2030  ameter']) else 0
+0002a1f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0002a200: 2020 2020 2020 7661 6c20 3d20 6b65 795f        val = key_
+0002a210: 6469 6374 5b27 7061 7261 6d65 7465 7227  dict['parameter'
+0002a220: 5d5b 7061 7261 6d5f 6964 785d 0a20 2020  ][param_idx].   
+0002a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a240: 2069 6620 276b 7727 2069 6e20 6b65 795f   if 'kw' in key_
+0002a250: 6469 6374 3a0a 2020 2020 2020 2020 2020  dict:.          
+0002a260: 2020 2020 2020 2020 2020 2020 2020 736c                sl
+0002a270: 6f74 282a 2a7b 6b65 795f 6469 6374 5b27  ot(**{key_dict['
+0002a280: 6b77 275d 3a20 7661 6c7d 290a 2020 2020  kw']: val}).    
+0002a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a2a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0002a2b0: 2020 2020 2020 2020 2020 2020 2020 736c                sl
+0002a2c0: 6f74 2876 616c 290a 2020 2020 2020 2020  ot(val).        
+0002a2d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0002a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a2f0: 2020 736c 6f74 2829 0a0a 2020 2020 2020    slot()..      
+0002a300: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+0002a310: 0a20 2020 2064 6566 205f 6472 6177 5f74  .    def _draw_t
+0002a320: 7261 6365 7328 7365 6c66 293a 0a20 2020  races(self):.   
+0002a330: 2020 2020 2023 2055 7064 6174 6520 6461       # Update da
+0002a340: 7461 2069 6e20 7472 6163 6573 2028 3d64  ta in traces (=d
+0002a350: 7261 7769 6e67 2074 7261 6365 7329 0a20  rawing traces). 
+0002a360: 2020 2020 2020 2066 6f72 2074 7261 6365         for trace
+0002a370: 2069 6e20 7365 6c66 2e6d 6e65 2e74 7261   in self.mne.tra
+0002a380: 6365 733a 0a20 2020 2020 2020 2020 2020  ces:.           
+0002a390: 2023 2055 7064 6174 6520 6461 7461 0a20   # Update data. 
+0002a3a0: 2020 2020 2020 2020 2020 2074 7261 6365             trace
+0002a3b0: 2e75 7064 6174 655f 6461 7461 2829 0a0a  .update_data()..
+0002a3c0: 2020 2020 6465 6620 5f67 6574 5f73 697a      def _get_siz
+0002a3d0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0002a3e0: 2069 6e63 685f 7769 6474 6820 3d20 7365   inch_width = se
+0002a3f0: 6c66 2e77 6964 7468 2829 202f 2073 656c  lf.width() / sel
+0002a400: 662e 6c6f 6769 6361 6c44 7069 5828 290a  f.logicalDpiX().
+0002a410: 2020 2020 2020 2020 696e 6368 5f68 6569          inch_hei
+0002a420: 6768 7420 3d20 7365 6c66 2e68 6569 6768  ght = self.heigh
+0002a430: 7428 2920 2f20 7365 6c66 2e6c 6f67 6963  t() / self.logic
+0002a440: 616c 4470 6959 2829 0a0a 2020 2020 2020  alDpiY()..      
+0002a450: 2020 7265 7475 726e 2069 6e63 685f 7769    return inch_wi
+0002a460: 6474 682c 2069 6e63 685f 6865 6967 6874  dth, inch_height
+0002a470: 0a0a 2020 2020 6465 6620 5f66 616b 655f  ..    def _fake_
+0002a480: 6b65 7970 7265 7373 2873 656c 662c 206b  keypress(self, k
+0002a490: 6579 2c20 6669 673d 4e6f 6e65 293a 0a20  ey, fig=None):. 
+0002a4a0: 2020 2020 2020 2066 6967 203d 2066 6967         fig = fig
+0002a4b0: 206f 7220 7365 6c66 0a0a 2020 2020 2020   or self..      
+0002a4c0: 2020 6966 206b 6579 2e69 7375 7070 6572    if key.isupper
+0002a4d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0002a4e0: 6b65 7920 3d20 6b65 792e 6c6f 7765 7228  key = key.lower(
+0002a4f0: 290a 2020 2020 2020 2020 2020 2020 6d6f  ).            mo
+0002a500: 6469 6669 6572 203d 2051 742e 5368 6966  difier = Qt.Shif
+0002a510: 744d 6f64 6966 6965 720a 2020 2020 2020  tModifier.      
+0002a520: 2020 656c 6966 206b 6579 2e73 7461 7274    elif key.start
+0002a530: 7377 6974 6828 2773 6869 6674 2b27 293a  swith('shift+'):
+0002a540: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
+0002a550: 203d 206b 6579 5b36 3a5d 0a20 2020 2020   = key[6:].     
+0002a560: 2020 2020 2020 206d 6f64 6966 6965 7220         modifier 
+0002a570: 3d20 5174 2e53 6869 6674 4d6f 6469 6669  = Qt.ShiftModifi
+0002a580: 6572 0a20 2020 2020 2020 2065 6c73 653a  er.        else:
+0002a590: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
+0002a5a0: 6966 6965 7220 3d20 5174 2e4e 6f4d 6f64  ifier = Qt.NoMod
+0002a5b0: 6966 6965 720a 0a20 2020 2020 2020 2023  ifier..        #
+0002a5c0: 2055 7365 2070 7974 6573 742d 7174 2773   Use pytest-qt's
+0002a5d0: 2065 7863 6570 7469 6f6e 2d68 6f6f 6b0a   exception-hook.
+0002a5e0: 2020 2020 2020 2020 7769 7468 2063 6170          with cap
+0002a5f0: 7475 7265 5f65 7863 6570 7469 6f6e 7328  ture_exceptions(
+0002a600: 2920 6173 2065 7863 6570 7469 6f6e 733a  ) as exceptions:
+0002a610: 0a20 2020 2020 2020 2020 2020 2051 5465  .            QTe
+0002a620: 7374 2e6b 6579 5072 6573 7328 6669 672c  st.keyPress(fig,
+0002a630: 2073 656c 662e 6d6e 652e 6b65 7962 6f61   self.mne.keyboa
+0002a640: 7264 5f73 686f 7274 6375 7473 5b6b 6579  rd_shortcuts[key
+0002a650: 5d5b 2771 745f 6b65 7927 5d2c 0a20 2020  ]['qt_key'],.   
+0002a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a670: 2020 2020 2020 2020 6d6f 6469 6669 6572          modifier
+0002a680: 290a 0a20 2020 2020 2020 2066 6f72 2065  )..        for e
+0002a690: 7863 2069 6e20 6578 6365 7074 696f 6e73  xc in exceptions
+0002a6a0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0002a6b0: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
+0002a6c0: 2866 2754 6865 7265 2061 7320 6265 656e  (f'There as been
+0002a6d0: 2061 6e20 7b65 7863 5b30 5d7d 2069 6e73   an {exc[0]} ins
+0002a6e0: 6964 6520 7468 6520 5174 2027 0a20 2020  ide the Qt '.   
+0002a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a700: 2020 2020 2020 2020 2020 2020 6627 6576              f'ev
+0002a710: 656e 7420 6c6f 6f70 2028 6c6f 6f6b 2061  ent loop (look a
+0002a720: 626f 7665 2066 6f72 2074 7261 6365 6261  bove for traceba
+0002a730: 636b 292e 2729 0a0a 2020 2020 6465 6620  ck).')..    def 
+0002a740: 5f66 616b 655f 636c 6963 6b28 7365 6c66  _fake_click(self
+0002a750: 2c20 706f 696e 742c 2061 6464 5f70 6f69  , point, add_poi
+0002a760: 6e74 733d 4e6f 6e65 2c20 6669 673d 4e6f  nts=None, fig=No
+0002a770: 6e65 2c20 6178 3d4e 6f6e 652c 0a20 2020  ne, ax=None,.   
+0002a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a790: 2078 666f 726d 3d27 6178 272c 2062 7574   xform='ax', but
+0002a7a0: 746f 6e3d 312c 206b 696e 643d 2770 7265  ton=1, kind='pre
+0002a7b0: 7373 2729 3a0a 2020 2020 2020 2020 6164  ss'):.        ad
+0002a7c0: 645f 706f 696e 7473 203d 2061 6464 5f70  d_points = add_p
+0002a7d0: 6f69 6e74 7320 6f72 206c 6973 7428 290a  oints or list().
+0002a7e0: 2020 2020 2020 2020 2320 5761 6974 2075          # Wait u
+0002a7f0: 6e74 696c 2057 696e 646f 7720 6973 2066  ntil Window is f
+0002a800: 756c 6c79 2073 686f 776e 2e0a 2020 2020  ully shown..    
+0002a810: 2020 2020 5154 6573 742e 7157 6169 7446      QTest.qWaitF
+0002a820: 6f72 5769 6e64 6f77 4578 706f 7365 6428  orWindowExposed(
+0002a830: 7365 6c66 290a 2020 2020 2020 2020 2320  self).        # 
+0002a840: 5363 656e 652d 4469 6d65 6e73 696f 6e73  Scene-Dimensions
+0002a850: 2073 7469 6c6c 2073 6565 6d20 746f 2063   still seem to c
+0002a860: 6861 6e67 6520 746f 2066 696e 616c 2073  hange to final s
+0002a870: 7461 7465 2077 6865 6e20 7761 6974 696e  tate when waitin
+0002a880: 670a 2020 2020 2020 2020 2320 666f 7220  g.        # for 
+0002a890: 6120 7368 6f72 7420 7469 6d65 2e0a 2020  a short time..  
+0002a8a0: 2020 2020 2020 5154 6573 742e 7157 6169        QTest.qWai
+0002a8b0: 7428 3130 290a 0a20 2020 2020 2020 2023  t(10)..        #
+0002a8c0: 2051 743a 2072 6967 6874 2d62 7574 746f   Qt: right-butto
+0002a8d0: 6e3d 322c 206d 6174 706c 6f74 6c69 623a  n=2, matplotlib:
+0002a8e0: 2072 6967 6874 2d62 7574 746f 6e3d 330a   right-button=3.
+0002a8f0: 2020 2020 2020 2020 6966 2062 7574 746f          if butto
+0002a900: 6e20 3d3d 2031 3a0a 2020 2020 2020 2020  n == 1:.        
+0002a910: 2020 2020 6275 7474 6f6e 203d 2051 742e      button = Qt.
+0002a920: 4c65 6674 4275 7474 6f6e 0a20 2020 2020  LeftButton.     
+0002a930: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0002a940: 2020 2020 2062 7574 746f 6e20 3d20 5174       button = Qt
+0002a950: 2e52 6967 6874 4275 7474 6f6e 0a0a 2020  .RightButton..  
+0002a960: 2020 2020 2020 2320 466f 7220 5174 2c20        # For Qt, 
+0002a970: 6669 6720 6f72 2061 7820 626f 7468 2077  fig or ax both w
+0002a980: 6f75 6c64 2062 6520 7468 6520 7769 6467  ould be the widg
+0002a990: 6574 2074 6f20 7465 7374 2069 6e74 6572  et to test inter
+0002a9a0: 6163 7469 6f6e 206f 6e2e 0a20 2020 2020  action on..     
+0002a9b0: 2020 2023 2049 6620 5669 6577 0a20 2020     # If View.   
+0002a9c0: 2020 2020 2066 6967 203d 2061 7820 6f72       fig = ax or
+0002a9d0: 2066 6967 206f 7220 7365 6c66 2e6d 6e65   fig or self.mne
+0002a9e0: 2e76 6965 770a 0a20 2020 2020 2020 2069  .view..        i
+0002a9f0: 6620 7866 6f72 6d20 3d3d 2027 6178 273a  f xform == 'ax':
+0002aa00: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
+0002aa10: 6f72 2051 742c 2074 6865 2065 7175 6976  or Qt, the equiv
+0002aa20: 616c 656e 7420 6f66 206d 6174 706c 6f74  alent of matplot
+0002aa30: 6c69 6273 2074 7261 6e73 4178 6573 0a20  libs transAxes. 
+0002aa40: 2020 2020 2020 2020 2020 2023 2077 6f75             # wou
+0002aa50: 6c64 2062 6520 6120 7472 616e 7366 6f72  ld be a transfor
+0002aa60: 6d61 7469 6f6e 2074 6f20 5669 6577 2043  mation to View C
+0002aa70: 6f6f 7264 696e 6174 6573 2e0a 2020 2020  oordinates..    
+0002aa80: 2020 2020 2020 2020 2320 4275 7420 666f          # But fo
+0002aa90: 7220 7468 6520 5669 6577 2074 6f70 2d6c  r the View top-l
+0002aaa0: 6566 7420 6973 2028 302c 2030 2920 616e  eft is (0, 0) an
+0002aab0: 6420 626f 7474 6f6d 2d72 6967 6874 2069  d bottom-right i
+0002aac0: 730a 2020 2020 2020 2020 2020 2020 2320  s.            # 
+0002aad0: 2876 6965 772d 7769 6474 682c 2076 6965  (view-width, vie
+0002aae0: 772d 6865 6967 6874 292e 0a20 2020 2020  w-height)..     
+0002aaf0: 2020 2020 2020 2076 6965 775f 7769 6474         view_widt
+0002ab00: 6820 3d20 6669 672e 7769 6474 6828 290a  h = fig.width().
+0002ab10: 2020 2020 2020 2020 2020 2020 7669 6577              view
+0002ab20: 5f68 6569 6768 7420 3d20 6669 672e 6865  _height = fig.he
+0002ab30: 6967 6874 2829 0a20 2020 2020 2020 2020  ight().         
+0002ab40: 2020 2078 203d 2076 6965 775f 7769 6474     x = view_widt
+0002ab50: 6820 2a20 706f 696e 745b 305d 0a20 2020  h * point[0].   
+0002ab60: 2020 2020 2020 2020 2079 203d 2076 6965           y = vie
+0002ab70: 775f 6865 6967 6874 202a 2028 3120 2d20  w_height * (1 - 
+0002ab80: 706f 696e 745b 315d 290a 2020 2020 2020  point[1]).      
+0002ab90: 2020 2020 2020 706f 696e 7420 3d20 506f        point = Po
+0002aba0: 696e 7428 782c 2079 290a 2020 2020 2020  int(x, y).      
+0002abb0: 2020 2020 2020 666f 7220 6964 782c 2061        for idx, a
+0002abc0: 706f 696e 7420 696e 2065 6e75 6d65 7261  point in enumera
+0002abd0: 7465 2861 6464 5f70 6f69 6e74 7329 3a0a  te(add_points):.
+0002abe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002abf0: 7832 203d 2076 6965 775f 7769 6474 6820  x2 = view_width 
+0002ac00: 2a20 6170 6f69 6e74 5b30 5d0a 2020 2020  * apoint[0].    
+0002ac10: 2020 2020 2020 2020 2020 2020 7932 203d              y2 =
+0002ac20: 2076 6965 775f 6865 6967 6874 202a 2028   view_height * (
+0002ac30: 3120 2d20 6170 6f69 6e74 5b31 5d29 0a20  1 - apoint[1]). 
+0002ac40: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0002ac50: 6464 5f70 6f69 6e74 735b 6964 785d 203d  dd_points[idx] =
+0002ac60: 2050 6f69 6e74 2878 322c 2079 3229 0a0a   Point(x2, y2)..
+0002ac70: 2020 2020 2020 2020 656c 6966 2078 666f          elif xfo
+0002ac80: 726d 203d 3d20 2764 6174 6127 3a0a 2020  rm == 'data':.  
+0002ac90: 2020 2020 2020 2020 2020 2320 466f 7220            # For 
+0002aca0: 5174 2c20 7468 6520 6571 7569 7661 6c65  Qt, the equivale
+0002acb0: 6e74 206f 6620 6d61 7470 6c6f 746c 6962  nt of matplotlib
+0002acc0: 7320 7472 616e 7344 6174 610a 2020 2020  s transData.    
+0002acd0: 2020 2020 2020 2020 2320 776f 756c 6420          # would 
+0002ace0: 6265 2061 2074 7261 6e73 666f 726d 6174  be a transformat
+0002acf0: 696f 6e20 746f 0a20 2020 2020 2020 2020  ion to.         
+0002ad00: 2020 2023 2074 6865 2063 6f6f 7264 696e     # the coordin
+0002ad10: 6174 6520 7379 7374 656d 206f 6620 7468  ate system of th
+0002ad20: 6520 5669 6577 426f 782e 0a20 2020 2020  e ViewBox..     
+0002ad30: 2020 2020 2020 2023 2054 6869 7320 6f6e         # This on
+0002ad40: 6c79 2077 6f72 6b73 206f 6e20 7468 6520  ly works on the 
+0002ad50: 5669 6577 2028 7365 6c66 2e6d 6e65 2e76  View (self.mne.v
+0002ad60: 6965 7729 0a20 2020 2020 2020 2020 2020  iew).           
+0002ad70: 2066 6967 203d 2073 656c 662e 6d6e 652e   fig = self.mne.
+0002ad80: 7669 6577 0a20 2020 2020 2020 2020 2020  view.           
+0002ad90: 2070 6f69 6e74 203d 2073 656c 662e 6d6e   point = self.mn
+0002ada0: 652e 7669 6577 626f 782e 6d61 7056 6965  e.viewbox.mapVie
+0002adb0: 7754 6f53 6365 6e65 2850 6f69 6e74 282a  wToScene(Point(*
+0002adc0: 706f 696e 7429 290a 2020 2020 2020 2020  point)).        
+0002add0: 2020 2020 666f 7220 6964 782c 2061 706f      for idx, apo
+0002ade0: 696e 7420 696e 2065 6e75 6d65 7261 7465  int in enumerate
+0002adf0: 2861 6464 5f70 6f69 6e74 7329 3a0a 2020  (add_points):.  
+0002ae00: 2020 2020 2020 2020 2020 2020 2020 6164                ad
+0002ae10: 645f 706f 696e 7473 5b69 6478 5d20 3d20  d_points[idx] = 
+0002ae20: 7365 6c66 2e6d 6e65 2e76 6965 7762 6f78  self.mne.viewbox
+0002ae30: 2e6d 6170 5669 6577 546f 5363 656e 6528  .mapViewToScene(
+0002ae40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002ae50: 2020 2020 2020 2020 2050 6f69 6e74 282a           Point(*
+0002ae60: 6170 6f69 6e74 2929 0a0a 2020 2020 2020  apoint))..      
+0002ae70: 2020 656c 6966 2078 666f 726d 203d 3d20    elif xform == 
+0002ae80: 276e 6f6e 6527 206f 7220 7866 6f72 6d20  'none' or xform 
+0002ae90: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0002aea0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+0002aeb0: 6365 2870 6f69 6e74 2c20 2874 7570 6c65  ce(point, (tuple
+0002aec0: 2c20 6c69 7374 2929 3a0a 2020 2020 2020  , list)):.      
+0002aed0: 2020 2020 2020 2020 2020 706f 696e 7420            point 
+0002aee0: 3d20 506f 696e 7428 2a70 6f69 6e74 290a  = Point(*point).
+0002aef0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0002af00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002af10: 2020 706f 696e 7420 3d20 506f 696e 7428    point = Point(
+0002af20: 706f 696e 7429 0a20 2020 2020 2020 2020  point).         
+0002af30: 2020 2066 6f72 2069 6478 2c20 6170 6f69     for idx, apoi
+0002af40: 6e74 2069 6e20 656e 756d 6572 6174 6528  nt in enumerate(
+0002af50: 6164 645f 706f 696e 7473 293a 0a20 2020  add_points):.   
+0002af60: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0002af70: 6973 696e 7374 616e 6365 2861 706f 696e  isinstance(apoin
+0002af80: 742c 2028 7475 706c 652c 206c 6973 7429  t, (tuple, list)
+0002af90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0002afa0: 2020 2020 2020 2061 6464 5f70 6f69 6e74         add_point
+0002afb0: 735b 6964 785d 203d 2050 6f69 6e74 282a  s[idx] = Point(*
+0002afc0: 6170 6f69 6e74 290a 2020 2020 2020 2020  apoint).        
+0002afd0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0002afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002aff0: 2020 6164 645f 706f 696e 7473 5b69 6478    add_points[idx
+0002b000: 5d20 3d20 506f 696e 7428 6170 6f69 6e74  ] = Point(apoint
+0002b010: 290a 0a20 2020 2020 2020 2023 2055 7365  )..        # Use
+0002b020: 2070 7974 6573 742d 7174 2773 2065 7863   pytest-qt's exc
+0002b030: 6570 7469 6f6e 2d68 6f6f 6b0a 2020 2020  eption-hook.    
+0002b040: 2020 2020 7769 7468 2063 6170 7475 7265      with capture
+0002b050: 5f65 7863 6570 7469 6f6e 7328 2920 6173  _exceptions() as
+0002b060: 2065 7863 6570 7469 6f6e 733a 0a20 2020   exceptions:.   
+0002b070: 2020 2020 2020 2020 2077 6964 6765 7420           widget 
+0002b080: 3d20 6669 672e 7669 6577 706f 7274 2829  = fig.viewport()
+0002b090: 2069 6620 6973 696e 7374 616e 6365 2866   if isinstance(f
+0002b0a0: 6967 2c20 5147 7261 7068 6963 7356 6965  ig, QGraphicsVie
+0002b0b0: 7729 2065 6c73 6520 6669 670a 2020 2020  w) else fig.    
+0002b0c0: 2020 2020 2020 2020 6966 206b 696e 6420          if kind 
+0002b0d0: 3d3d 2027 7072 6573 7327 3a0a 2020 2020  == 'press':.    
+0002b0e0: 2020 2020 2020 2020 2020 2020 2320 616c              # al
+0002b0f0: 7761 7973 2063 6c69 636b 2062 6563 6175  ways click becau
+0002b100: 7365 206d 6f73 7420 696e 7465 7261 6374  se most interact
+0002b110: 6976 6974 7920 636f 6d65 7320 666f 726d  ivity comes form
+0002b120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b130: 2023 206d 6f75 7365 436c 6963 6b45 7665   # mouseClickEve
+0002b140: 6e74 2066 726f 6d20 7079 7174 6772 6170  nt from pyqtgrap
+0002b150: 6820 286a 7573 7420 7072 6573 7320 646f  h (just press do
+0002b160: 6573 6e27 7420 7375 6666 6963 650a 2020  esn't suffice.  
+0002b170: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0002b180: 6865 7265 292e 0a20 2020 2020 2020 2020  here)..         
+0002b190: 2020 2020 2020 205f 6d6f 7573 6543 6c69         _mouseCli
+0002b1a0: 636b 2877 6964 6765 743d 7769 6467 6574  ck(widget=widget
+0002b1b0: 2c20 706f 733d 706f 696e 742c 2062 7574  , pos=point, but
+0002b1c0: 746f 6e3d 6275 7474 6f6e 290a 2020 2020  ton=button).    
+0002b1d0: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
+0002b1e0: 6420 3d3d 2027 7265 6c65 6173 6527 3a0a  d == 'release':.
+0002b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b200: 5f6d 6f75 7365 5265 6c65 6173 6528 7769  _mouseRelease(wi
+0002b210: 6467 6574 3d77 6964 6765 742c 2070 6f73  dget=widget, pos
+0002b220: 3d70 6f69 6e74 2c20 6275 7474 6f6e 3d62  =point, button=b
+0002b230: 7574 746f 6e29 0a20 2020 2020 2020 2020  utton).         
+0002b240: 2020 2065 6c69 6620 6b69 6e64 203d 3d20     elif kind == 
+0002b250: 276d 6f74 696f 6e27 3a0a 2020 2020 2020  'motion':.      
+0002b260: 2020 2020 2020 2020 2020 5f6d 6f75 7365            _mouse
+0002b270: 4d6f 7665 2877 6964 6765 743d 7769 6467  Move(widget=widg
+0002b280: 6574 2c20 706f 733d 706f 696e 742c 2062  et, pos=point, b
+0002b290: 7574 746f 6e73 3d62 7574 746f 6e29 0a20  uttons=button). 
+0002b2a0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0002b2b0: 6b69 6e64 203d 3d20 2764 7261 6727 3a0a  kind == 'drag':.
+0002b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b2d0: 5f6d 6f75 7365 4472 6167 2877 6964 6765  _mouseDrag(widge
+0002b2e0: 743d 7769 6467 6574 2c20 706f 7369 7469  t=widget, positi
+0002b2f0: 6f6e 733d 5b70 6f69 6e74 5d20 2b20 6164  ons=[point] + ad
+0002b300: 645f 706f 696e 7473 2c0a 2020 2020 2020  d_points,.      
+0002b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b320: 2020 2020 2062 7574 746f 6e3d 6275 7474       button=butt
+0002b330: 6f6e 290a 0a20 2020 2020 2020 2066 6f72  on)..        for
+0002b340: 2065 7863 2069 6e20 6578 6365 7074 696f   exc in exceptio
+0002b350: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0002b360: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
+0002b370: 6f72 2866 2754 6865 7265 2061 7320 6265  or(f'There as be
+0002b380: 656e 2061 6e20 7b65 7863 5b30 5d7d 2069  en an {exc[0]} i
+0002b390: 6e73 6964 6520 7468 6520 5174 2027 0a20  nside the Qt '. 
+0002b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b3b0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+0002b3c0: 6576 656e 7420 6c6f 6f70 2028 6c6f 6f6b  event loop (look
+0002b3d0: 2061 626f 7665 2066 6f72 2074 7261 6365   above for trace
+0002b3e0: 6261 636b 292e 2729 0a0a 2020 2020 2020  back).')..      
+0002b3f0: 2020 2320 5761 6974 696e 6720 736f 6d65    # Waiting some
+0002b400: 2074 696d 6520 666f 7220 6576 656e 7473   time for events
+0002b410: 2074 6f20 6265 2070 726f 6365 7373 6564   to be processed
+0002b420: 2e0a 2020 2020 2020 2020 5154 6573 742e  ..        QTest.
+0002b430: 7157 6169 7428 3530 290a 0a20 2020 2064  qWait(50)..    d
+0002b440: 6566 205f 6661 6b65 5f73 6372 6f6c 6c28  ef _fake_scroll(
+0002b450: 7365 6c66 2c20 782c 2079 2c20 7374 6570  self, x, y, step
+0002b460: 2c20 6669 673d 4e6f 6e65 293a 0a20 2020  , fig=None):.   
+0002b470: 2020 2020 2023 2051 5465 7374 2064 6f65       # QTest doe
+0002b480: 736e 2774 2073 7570 706f 7274 2073 696d  sn't support sim
+0002b490: 756c 6174 696e 6720 7363 726f 6c6c 696e  ulating scrollin
+0002b4a0: 672d 7768 6565 6c0a 2020 2020 2020 2020  g-wheel.        
+0002b4b0: 7365 6c66 2e76 7363 726f 6c6c 2873 7465  self.vscroll(ste
+0002b4c0: 7029 0a0a 2020 2020 6465 6620 5f63 6c69  p)..    def _cli
+0002b4d0: 636b 5f63 685f 6e61 6d65 2873 656c 662c  ck_ch_name(self,
+0002b4e0: 2063 685f 696e 6465 782c 2062 7574 746f   ch_index, butto
+0002b4f0: 6e29 3a0a 2020 2020 2020 2020 7365 6c66  n):.        self
+0002b500: 2e6d 6e65 2e63 6861 6e6e 656c 5f61 7869  .mne.channel_axi
+0002b510: 732e 7265 7061 696e 7428 290a 2020 2020  s.repaint().    
+0002b520: 2020 2020 2320 5761 6974 2062 6563 6175      # Wait becau
+0002b530: 7365 2063 6861 6e6e 656c 2d61 7869 7320  se channel-axis 
+0002b540: 6d61 7920 6e65 6564 2074 696d 650a 2020  may need time.  
+0002b550: 2020 2020 2020 2320 2863 616d 6520 7570        # (came up
+0002b560: 2077 6974 6820 7465 7374 5f65 706f 6368   with test_epoch
+0002b570: 733a 3a74 6573 745f 706c 6f74 5f65 706f  s::test_plot_epo
+0002b580: 6368 735f 636c 6963 6b73 290a 2020 2020  chs_clicks).    
+0002b590: 2020 2020 5154 6573 742e 7157 6169 7428      QTest.qWait(
+0002b5a0: 3130 3029 0a20 2020 2020 2020 2069 6620  100).        if 
+0002b5b0: 6e6f 7420 7365 6c66 2e6d 6e65 2e62 7574  not self.mne.but
+0002b5c0: 7465 7266 6c79 3a0a 2020 2020 2020 2020  terfly:.        
+0002b5d0: 2020 2020 6368 5f6e 616d 6520 3d20 7365      ch_name = se
+0002b5e0: 6c66 2e6d 6e65 2e63 685f 6e61 6d65 735b  lf.mne.ch_names[
+0002b5f0: 7365 6c66 2e6d 6e65 2e70 6963 6b73 5b63  self.mne.picks[c
+0002b600: 685f 696e 6465 785d 5d0a 2020 2020 2020  h_index]].      
+0002b610: 2020 2020 2020 7872 616e 6765 2c20 7972        xrange, yr
+0002b620: 616e 6765 203d 2073 656c 662e 6d6e 652e  ange = self.mne.
+0002b630: 6368 616e 6e65 6c5f 6178 6973 2e63 685f  channel_axis.ch_
+0002b640: 7465 7874 735b 6368 5f6e 616d 655d 0a20  texts[ch_name]. 
+0002b650: 2020 2020 2020 2020 2020 2078 203d 206e             x = n
+0002b660: 702e 6d65 616e 2878 7261 6e67 6529 0a20  p.mean(xrange). 
+0002b670: 2020 2020 2020 2020 2020 2079 203d 206e             y = n
+0002b680: 702e 6d65 616e 2879 7261 6e67 6529 0a0a  p.mean(yrange)..
+0002b690: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002b6a0: 2e5f 6661 6b65 5f63 6c69 636b 2828 782c  ._fake_click((x,
+0002b6b0: 2079 292c 2066 6967 3d73 656c 662e 6d6e   y), fig=self.mn
+0002b6c0: 652e 7669 6577 2c20 6275 7474 6f6e 3d62  e.view, button=b
+0002b6d0: 7574 746f 6e2c 0a20 2020 2020 2020 2020  utton,.         
+0002b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b6f0: 2020 2020 7866 6f72 6d3d 276e 6f6e 6527      xform='none'
+0002b700: 290a 0a20 2020 2064 6566 205f 7265 7369  )..    def _resi
+0002b710: 7a65 5f62 795f 6661 6374 6f72 2873 656c  ze_by_factor(sel
+0002b720: 662c 2066 6163 746f 7229 3a0a 2020 2020  f, factor):.    
+0002b730: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+0002b740: 6620 5f67 6574 5f74 6963 6b6c 6162 656c  f _get_ticklabel
+0002b750: 7328 7365 6c66 2c20 6f72 6965 6e74 6174  s(self, orientat
+0002b760: 696f 6e29 3a0a 2020 2020 2020 2020 6966  ion):.        if
+0002b770: 206f 7269 656e 7461 7469 6f6e 203d 3d20   orientation == 
+0002b780: 2778 273a 0a20 2020 2020 2020 2020 2020  'x':.           
+0002b790: 2061 7820 3d20 7365 6c66 2e6d 6e65 2e74   ax = self.mne.t
+0002b7a0: 696d 655f 6178 6973 0a20 2020 2020 2020  ime_axis.       
+0002b7b0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0002b7c0: 2020 2061 7820 3d20 7365 6c66 2e6d 6e65     ax = self.mne
+0002b7d0: 2e63 6861 6e6e 656c 5f61 7869 730a 0a20  .channel_axis.. 
+0002b7e0: 2020 2020 2020 2072 6574 7572 6e20 6c69         return li
+0002b7f0: 7374 2861 782e 6765 745f 6c61 6265 6c73  st(ax.get_labels
+0002b800: 2829 290a 0a20 2020 2064 6566 205f 6765  ())..    def _ge
+0002b810: 745f 7363 616c 655f 6261 725f 7465 7874  t_scale_bar_text
+0002b820: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+0002b830: 2072 6574 7572 6e20 7475 706c 6528 742e   return tuple(t.
+0002b840: 746f 506c 6169 6e54 6578 7428 2920 666f  toPlainText() fo
+0002b850: 7220 7420 696e 2073 656c 662e 6d6e 652e  r t in self.mne.
+0002b860: 7363 616c 6562 6172 5f74 6578 7473 2e76  scalebar_texts.v
+0002b870: 616c 7565 7328 2929 0a0a 2020 2020 6465  alues())..    de
+0002b880: 6620 7368 6f77 2873 656c 6629 3a20 2023  f show(self):  #
+0002b890: 206e 6f71 613a 2044 3130 320a 2020 2020   noqa: D102.    
+0002b8a0: 2020 2020 2320 5365 7420 7261 6973 655f      # Set raise_
+0002b8b0: 7769 6e64 6f77 206c 696b 6520 6d61 7470  window like matp
+0002b8c0: 6c6f 746c 6962 2069 6620 706f 7373 6962  lotlib if possib
+0002b8d0: 6c65 0a20 2020 2020 2020 2073 7570 6572  le.        super
+0002b8e0: 2829 2e73 686f 7728 290a 2020 2020 2020  ().show().      
+0002b8f0: 2020 5f71 745f 7261 6973 655f 7769 6e64    _qt_raise_wind
+0002b900: 6f77 2873 656c 6629 0a0a 2020 2020 6465  ow(self)..    de
+0002b910: 6620 5f63 6c6f 7365 5f65 7665 6e74 2873  f _close_event(s
+0002b920: 656c 662c 2066 6967 3d4e 6f6e 6529 3a0a  elf, fig=None):.
+0002b930: 2020 2020 2020 2020 2222 2246 6f72 6365          """Force
+0002b940: 2063 616c 6c69 6e67 206f 6620 7468 6520   calling of the 
+0002b950: 4d50 4c20 6669 6775 7265 2063 6c6f 7365  MPL figure close
+0002b960: 2065 7665 6e74 2e22 2222 0a20 2020 2020   event.""".     
+0002b970: 2020 2066 6967 203d 2066 6967 206f 7220     fig = fig or 
+0002b980: 7365 6c66 0a20 2020 2020 2020 2069 6620  self.        if 
+0002b990: 6861 7361 7474 7228 6669 672c 2027 6361  hasattr(fig, 'ca
+0002b9a0: 6e76 6173 2729 3a0a 2020 2020 2020 2020  nvas'):.        
+0002b9b0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0002b9c0: 2020 2020 2020 2020 2066 6967 2e63 616e           fig.can
+0002b9d0: 7661 732e 636c 6f73 655f 6576 656e 7428  vas.close_event(
+0002b9e0: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+0002b9f0: 6365 7074 2056 616c 7565 4572 726f 723a  cept ValueError:
+0002ba00: 2020 2320 6f6c 6420 6d70 6c20 7769 7468    # old mpl with
+0002ba10: 2051 740a 2020 2020 2020 2020 2020 2020   Qt.            
+0002ba20: 2020 2020 7061 7373 2020 2320 7072 6167      pass  # prag
+0002ba30: 6d61 3a20 6e6f 2063 6f76 6572 0a20 2020  ma: no cover.   
+0002ba40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0002ba50: 2020 2020 2020 2066 6967 2e63 6c6f 7365         fig.close
+0002ba60: 2829 0a0a 2020 2020 6465 6620 5f63 6865  ()..    def _che
+0002ba70: 636b 5f63 6c6f 7365 2873 656c 6629 3a0a  ck_close(self):.
+0002ba80: 2020 2020 2020 2020 2222 2243 6c6f 7365          """Close
+0002ba90: 2061 6e6e 6f74 6174 696f 6e73 2d6d 6f64   annotations-mod
+0002baa0: 6520 6265 666f 7265 2063 6c6f 7369 6e67  e before closing
+0002bab0: 2074 6865 2062 726f 7773 6572 2e22 2222   the browser."""
+0002bac0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002bad0: 2e6d 6e65 2e61 6e6e 6f74 6174 696f 6e5f  .mne.annotation_
+0002bae0: 6d6f 6465 3a0a 2020 2020 2020 2020 2020  mode:.          
+0002baf0: 2020 7365 6c66 2e5f 746f 6767 6c65 5f61    self._toggle_a
+0002bb00: 6e6e 6f74 6174 696f 6e5f 6669 6728 290a  nnotation_fig().
+0002bb10: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0002bb20: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0002bb30: 6c6f 7365 2829 0a0a 2020 2020 6465 6620  lose()..    def 
+0002bb40: 636c 6f73 6545 7665 6e74 2873 656c 662c  closeEvent(self,
+0002bb50: 2065 7665 6e74 293a 0a20 2020 2020 2020   event):.       
+0002bb60: 2022 2222 4375 7374 6f6d 697a 6520 636c   """Customize cl
+0002bb70: 6f73 6520 6576 656e 742e 2222 220a 2020  ose event.""".  
+0002bb80: 2020 2020 2020 6576 656e 742e 6163 6365        event.acce
+0002bb90: 7074 2829 0a20 2020 2020 2020 2069 6620  pt().        if 
+0002bba0: 6861 7361 7474 7228 7365 6c66 2c20 276d  hasattr(self, 'm
+0002bbb0: 6e65 2729 3a0a 2020 2020 2020 2020 2020  ne'):.          
+0002bbc0: 2020 2320 4578 706c 6963 6974 2064 6973    # Explicit dis
+0002bbd0: 636f 6e6e 6563 7473 2074 6f20 6176 6f69  connects to avoi
+0002bbe0: 6420 7265 6665 7265 6e63 6520 6379 636c  d reference cycl
+0002bbf0: 6573 2074 6861 7420 6763 2063 616e 2774  es that gc can't
+0002bc00: 0a20 2020 2020 2020 2020 2020 2023 2070  .            # p
+0002bc10: 726f 7065 726c 7920 7265 736f 6c76 6520  roperly resolve 
+0002bc20: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
+0002bc30: 6620 6861 7361 7474 7228 7365 6c66 2e6d  f hasattr(self.m
+0002bc40: 6e65 2c20 2770 6c74 2729 3a0a 2020 2020  ne, 'plt'):.    
+0002bc50: 2020 2020 2020 2020 2020 2020 5f64 6973              _dis
+0002bc60: 636f 6e6e 6563 7428 7365 6c66 2e6d 6e65  connect(self.mne
+0002bc70: 2e70 6c74 2e73 6967 5852 616e 6765 4368  .plt.sigXRangeCh
+0002bc80: 616e 6765 6429 0a20 2020 2020 2020 2020  anged).         
+0002bc90: 2020 2020 2020 205f 6469 7363 6f6e 6e65         _disconne
+0002bca0: 6374 2873 656c 662e 6d6e 652e 706c 742e  ct(self.mne.plt.
+0002bcb0: 7369 6759 5261 6e67 6543 6861 6e67 6564  sigYRangeChanged
+0002bcc0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0002bcd0: 2068 6173 6174 7472 2873 656c 662e 6d6e   hasattr(self.mn
+0002bce0: 652c 2027 746f 6f6c 6261 7227 293a 0a20  e, 'toolbar'):. 
+0002bcf0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0002bd00: 6f72 2061 6374 696f 6e20 696e 2073 656c  or action in sel
+0002bd10: 662e 6d6e 652e 746f 6f6c 6261 722e 6163  f.mne.toolbar.ac
+0002bd20: 7469 6f6e 7328 293a 0a20 2020 2020 2020  tions():.       
+0002bd30: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+0002bd40: 6f77 5f65 7272 6f72 203d 2061 6374 696f  ow_error = actio
+0002bd50: 6e2e 7465 7874 2829 203d 3d20 2727 0a20  n.text() == ''. 
+0002bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bd70: 2020 205f 6469 7363 6f6e 6e65 6374 2861     _disconnect(a
+0002bd80: 6374 696f 6e2e 7472 6967 6765 7265 642c  ction.triggered,
+0002bd90: 2061 6c6c 6f77 5f65 7272 6f72 3d61 6c6c   allow_error=all
+0002bda0: 6f77 5f65 7272 6f72 290a 2020 2020 2020  ow_error).      
+0002bdb0: 2020 2020 2020 2320 5361 7665 2073 6574        # Save set
+0002bdc0: 7469 6e67 7320 676f 696e 6720 696e 746f  tings going into
+0002bdd0: 2051 5365 7474 696e 6773 2e0a 2020 2020   QSettings..    
+0002bde0: 2020 2020 2020 2020 666f 7220 7173 6574          for qset
+0002bdf0: 7469 6e67 2069 6e20 7173 6574 7469 6e67  ting in qsetting
+0002be00: 735f 7061 7261 6d73 3a0a 2020 2020 2020  s_params:.      
+0002be10: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
+0002be20: 3d20 6765 7461 7474 7228 7365 6c66 2e6d  = getattr(self.m
+0002be30: 6e65 2c20 7173 6574 7469 6e67 290a 2020  ne, qsetting).  
+0002be40: 2020 2020 2020 2020 2020 2020 2020 5153                QS
+0002be50: 6574 7469 6e67 7328 292e 7365 7456 616c  ettings().setVal
+0002be60: 7565 2871 7365 7474 696e 672c 2076 616c  ue(qsetting, val
+0002be70: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+0002be80: 666f 7220 6174 7472 2069 6e20 2827 6b65  for attr in ('ke
+0002be90: 7962 6f61 7264 5f73 686f 7274 6375 7473  yboard_shortcuts
+0002bea0: 272c 2027 7472 6163 6573 272c 2027 706c  ', 'traces', 'pl
+0002beb0: 7427 2c20 2774 6f6f 6c62 6172 272c 0a20  t', 'toolbar',. 
+0002bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bed0: 2020 2020 2020 2020 2766 6967 5f61 6e6e          'fig_ann
+0002bee0: 6f74 6174 696f 6e27 293a 0a20 2020 2020  otation'):.     
+0002bef0: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
+0002bf00: 7361 7474 7228 7365 6c66 2e6d 6e65 2c20  sattr(self.mne, 
+0002bf10: 6174 7472 293a 0a20 2020 2020 2020 2020  attr):.         
+0002bf20: 2020 2020 2020 2020 2020 2064 656c 6174             delat
+0002bf30: 7472 2873 656c 662e 6d6e 652c 2061 7474  tr(self.mne, att
+0002bf40: 7229 0a20 2020 2020 2020 2020 2020 2069  r).            i
+0002bf50: 6620 6861 7361 7474 7228 7365 6c66 2e6d  f hasattr(self.m
+0002bf60: 6e65 2c20 2763 6869 6c64 5f66 6967 7327  ne, 'child_figs'
+0002bf70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0002bf80: 2020 2066 6f72 2066 6967 2069 6e20 7365     for fig in se
+0002bf90: 6c66 2e6d 6e65 2e63 6869 6c64 5f66 6967  lf.mne.child_fig
+0002bfa0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0002bfb0: 2020 2020 2020 2066 6967 2e63 6c6f 7365         fig.close
+0002bfc0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0002bfd0: 2020 2073 656c 662e 6d6e 652e 6368 696c     self.mne.chil
+0002bfe0: 645f 6669 6773 2e63 6c65 6172 2829 0a20  d_figs.clear(). 
+0002bff0: 2020 2020 2020 2020 2020 2066 6f72 2061             for a
+0002c000: 7474 7220 696e 2028 2774 7261 6365 7327  ttr in ('traces'
+0002c010: 2c20 2765 7665 6e74 5f6c 696e 6573 272c  , 'event_lines',
+0002c020: 2027 7265 6769 6f6e 7327 293a 0a20 2020   'regions'):.   
+0002c030: 2020 2020 2020 2020 2020 2020 2067 6574               get
+0002c040: 6174 7472 2873 656c 662e 6d6e 652c 2061  attr(self.mne, a
+0002c050: 7474 722c 205b 5d29 2e63 6c65 6172 2829  ttr, []).clear()
+0002c060: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0002c070: 6765 7461 7474 7228 7365 6c66 2e6d 6e65  getattr(self.mne
+0002c080: 2c20 2776 6c69 6e65 272c 204e 6f6e 6529  , 'vline', None)
+0002c090: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002c0a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0002c0b0: 2073 656c 662e 6d6e 652e 6973 5f65 706f   self.mne.is_epo
+0002c0c0: 6368 733a 0a20 2020 2020 2020 2020 2020  chs:.           
+0002c0d0: 2020 2020 2020 2020 2066 6f72 2076 6c20           for vl 
+0002c0e0: 696e 2073 656c 662e 6d6e 652e 766c 696e  in self.mne.vlin
+0002c0f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0002c100: 2020 2020 2020 2020 2020 205f 6469 7363             _disc
+0002c110: 6f6e 6e65 6374 2876 6c2e 7369 6750 6f73  onnect(vl.sigPos
+0002c120: 6974 696f 6e43 6861 6e67 6546 696e 6973  itionChangeFinis
+0002c130: 6865 6429 0a20 2020 2020 2020 2020 2020  hed).           
+0002c140: 2020 2020 2020 2020 2073 656c 662e 6d6e           self.mn
+0002c150: 652e 766c 696e 652e 636c 6561 7228 290a  e.vline.clear().
+0002c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c170: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0002c180: 2020 2020 2020 2020 2020 5f64 6973 636f            _disco
+0002c190: 6e6e 6563 7428 7365 6c66 2e6d 6e65 2e76  nnect(self.mne.v
+0002c1a0: 6c69 6e65 2e73 6967 506f 7369 7469 6f6e  line.sigPosition
+0002c1b0: 4368 616e 6765 4669 6e69 7368 6564 290a  ChangeFinished).
+0002c1c0: 2020 2020 2020 2020 6966 2067 6574 6174          if getat
+0002c1d0: 7472 2873 656c 662c 2027 6c6f 6164 5f74  tr(self, 'load_t
+0002c1e0: 6872 6561 6427 2c20 4e6f 6e65 2920 6973  hread', None) is
+0002c1f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002c200: 2020 2020 2020 2073 656c 662e 6c6f 6164         self.load
+0002c210: 5f74 6872 6561 642e 636c 6561 6e28 290a  _thread.clean().
+0002c220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002c230: 2e6c 6f61 645f 7468 7265 6164 203d 204e  .load_thread = N
+0002c240: 6f6e 650a 0a20 2020 2020 2020 2023 2052  one..        # R
+0002c250: 656d 6f76 6520 7365 6c66 2066 726f 6d20  emove self from 
+0002c260: 6272 6f77 7365 725f 696e 7374 616e 6365  browser_instance
+0002c270: 7320 696e 2067 6c6f 6261 6c73 0a20 2020  s in globals.   
+0002c280: 2020 2020 2069 6620 7365 6c66 2069 6e20       if self in 
+0002c290: 5f62 726f 7773 6572 5f69 6e73 7461 6e63  _browser_instanc
+0002c2a0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0002c2b0: 5f62 726f 7773 6572 5f69 6e73 7461 6e63  _browser_instanc
+0002c2c0: 6573 2e72 656d 6f76 6528 7365 6c66 290a  es.remove(self).
+0002c2d0: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
+0002c2e0: 6f73 6528 6576 656e 7429 0a20 2020 2020  ose(event).     
+0002c2f0: 2020 2073 656c 662e 676f 7443 6c6f 7365     self.gotClose
+0002c300: 642e 656d 6974 2829 0a20 2020 2020 2020  d.emit().       
+0002c310: 2023 204d 616b 6520 7375 7265 2069 7420   # Make sure it 
+0002c320: 6765 7473 2064 656c 6574 6564 2061 6674  gets deleted aft
+0002c330: 6572 2069 7420 7761 7320 636c 6f73 6564  er it was closed
+0002c340: 2e0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+0002c350: 656c 6574 654c 6174 6572 2829 0a20 2020  eleteLater().   
+0002c360: 2020 2020 2073 656c 662e 5f63 6c6f 7365       self._close
+0002c370: 6420 3d20 5472 7565 0a0a 2020 2020 6465  d = True..    de
+0002c380: 6620 5f66 616b 655f 636c 6963 6b5f 6f6e  f _fake_click_on
+0002c390: 5f74 6f6f 6c62 6172 5f61 6374 696f 6e28  _toolbar_action(
+0002c3a0: 7365 6c66 2c20 6163 7469 6f6e 5f6e 616d  self, action_nam
+0002c3b0: 652c 2077 6169 745f 6166 7465 723d 3530  e, wait_after=50
+0002c3c0: 3029 3a0a 2020 2020 2020 2020 2222 2254  0):.        """T
+0002c3d0: 7269 6767 6572 2065 7665 6e74 2061 7373  rigger event ass
+0002c3e0: 6f63 6961 7465 6420 7769 7468 2061 6374  ociated with act
+0002c3f0: 696f 6e20 2761 6374 696f 6e5f 6e61 6d65  ion 'action_name
+0002c400: 2720 696e 2074 6f6f 6c62 6172 2e22 2222  ' in toolbar."""
+0002c410: 0a20 2020 2020 2020 2066 6f72 2061 6374  .        for act
+0002c420: 696f 6e20 696e 2073 656c 662e 6d6e 652e  ion in self.mne.
+0002c430: 746f 6f6c 6261 722e 6163 7469 6f6e 7328  toolbar.actions(
+0002c440: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+0002c450: 6620 6e6f 7420 6163 7469 6f6e 2e69 7353  f not action.isS
+0002c460: 6570 6172 6174 6f72 2829 3a0a 2020 2020  eparator():.    
+0002c470: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+0002c480: 6374 696f 6e2e 6963 6f6e 5465 7874 2829  ction.iconText()
+0002c490: 203d 3d20 6163 7469 6f6e 5f6e 616d 653a   == action_name:
+0002c4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c4b0: 2020 2020 2061 6374 696f 6e2e 7472 6967       action.trig
+0002c4c0: 6765 7228 290a 2020 2020 2020 2020 5154  ger().        QT
+0002c4d0: 6573 742e 7157 6169 7428 7761 6974 5f61  est.qWait(wait_a
+0002c4e0: 6674 6572 290a 0a0a 6465 6620 5f67 6574  fter)...def _get
+0002c4f0: 5f6e 5f66 6967 7328 293a 0a20 2020 2023  _n_figs():.    #
+0002c500: 2057 6169 7420 666f 7220 6120 7368 6f72   Wait for a shor
+0002c510: 7420 7469 6d65 2074 6f20 6c65 7420 7468  t time to let th
+0002c520: 6520 5174 2d6c 6f6f 7020 636c 6561 6e20  e Qt-loop clean 
+0002c530: 7570 0a20 2020 2051 5465 7374 2e71 5761  up.    QTest.qWa
+0002c540: 6974 2831 3030 290a 2020 2020 7265 7475  it(100).    retu
+0002c550: 726e 206c 656e 285b 7769 6e64 6f77 2066  rn len([window f
+0002c560: 6f72 2077 696e 646f 7720 696e 2051 4170  or window in QAp
+0002c570: 706c 6963 6174 696f 6e2e 746f 704c 6576  plication.topLev
+0002c580: 656c 5769 6e64 6f77 7328 290a 2020 2020  elWindows().    
+0002c590: 2020 2020 2020 2020 2020 2020 6966 2077              if w
+0002c5a0: 696e 646f 772e 6973 5669 7369 626c 6528  indow.isVisible(
+0002c5b0: 295d 290a 0a0a 6465 6620 5f63 6c6f 7365  )])...def _close
+0002c5c0: 5f61 6c6c 2829 3a0a 2020 2020 6966 206c  _all():.    if l
+0002c5d0: 656e 2851 4170 706c 6963 6174 696f 6e2e  en(QApplication.
+0002c5e0: 746f 704c 6576 656c 5769 6e64 6f77 7328  topLevelWindows(
+0002c5f0: 2929 203e 2030 3a0a 2020 2020 2020 2020  )) > 0:.        
+0002c600: 5141 7070 6c69 6361 7469 6f6e 2e63 6c6f  QApplication.clo
+0002c610: 7365 416c 6c57 696e 646f 7773 2829 0a0a  seAllWindows()..
+0002c620: 0a23 206d 6f75 7365 2074 6573 7469 6e67  .# mouse testing
+0002c630: 2066 756e 6374 696f 6e73 2061 6461 7074   functions adapt
+0002c640: 6564 2066 726f 6d20 7079 7174 6772 6170  ed from pyqtgrap
+0002c650: 680a 2320 2870 7971 7467 7261 7068 2e74  h.# (pyqtgraph.t
+0002c660: 6573 7473 2e75 695f 7465 7374 696e 672e  ests.ui_testing.
+0002c670: 7079 290a 6465 6620 5f6d 6f75 7365 5072  py).def _mousePr
+0002c680: 6573 7328 7769 6467 6574 2c20 706f 732c  ess(widget, pos,
+0002c690: 2062 7574 746f 6e2c 206d 6f64 6966 6965   button, modifie
+0002c6a0: 723d 4e6f 6e65 293a 0a20 2020 2069 6620  r=None):.    if 
+0002c6b0: 6d6f 6469 6669 6572 2069 7320 4e6f 6e65  modifier is None
+0002c6c0: 3a0a 2020 2020 2020 2020 6d6f 6469 6669  :.        modifi
+0002c6d0: 6572 203d 2051 742e 4b65 7962 6f61 7264  er = Qt.Keyboard
+0002c6e0: 4d6f 6469 6669 6572 2e4e 6f4d 6f64 6966  Modifier.NoModif
+0002c6f0: 6965 720a 2020 2020 6576 656e 7420 3d20  ier.    event = 
+0002c700: 514d 6f75 7365 4576 656e 7428 5145 7665  QMouseEvent(QEve
+0002c710: 6e74 2e54 7970 652e 4d6f 7573 6542 7574  nt.Type.MouseBut
+0002c720: 746f 6e50 7265 7373 2c20 706f 732c 2062  tonPress, pos, b
+0002c730: 7574 746f 6e2c 0a20 2020 2020 2020 2020  utton,.         
+0002c740: 2020 2020 2020 2020 2020 2020 2020 2051                 Q
+0002c750: 742e 4d6f 7573 6542 7574 746f 6e2e 4e6f  t.MouseButton.No
+0002c760: 4275 7474 6f6e 2c20 6d6f 6469 6669 6572  Button, modifier
+0002c770: 290a 2020 2020 5141 7070 6c69 6361 7469  ).    QApplicati
+0002c780: 6f6e 2e73 656e 6445 7665 6e74 2877 6964  on.sendEvent(wid
+0002c790: 6765 742c 2065 7665 6e74 290a 0a0a 6465  get, event)...de
+0002c7a0: 6620 5f6d 6f75 7365 5265 6c65 6173 6528  f _mouseRelease(
+0002c7b0: 7769 6467 6574 2c20 706f 732c 2062 7574  widget, pos, but
+0002c7c0: 746f 6e2c 206d 6f64 6966 6965 723d 4e6f  ton, modifier=No
+0002c7d0: 6e65 293a 0a20 2020 2069 6620 6d6f 6469  ne):.    if modi
+0002c7e0: 6669 6572 2069 7320 4e6f 6e65 3a0a 2020  fier is None:.  
+0002c7f0: 2020 2020 2020 6d6f 6469 6669 6572 203d        modifier =
+0002c800: 2051 742e 4b65 7962 6f61 7264 4d6f 6469   Qt.KeyboardModi
+0002c810: 6669 6572 2e4e 6f4d 6f64 6966 6965 720a  fier.NoModifier.
+0002c820: 2020 2020 6576 656e 7420 3d20 514d 6f75      event = QMou
+0002c830: 7365 4576 656e 7428 5145 7665 6e74 2e54  seEvent(QEvent.T
+0002c840: 7970 652e 4d6f 7573 6542 7574 746f 6e52  ype.MouseButtonR
+0002c850: 656c 6561 7365 2c20 706f 732c 0a20 2020  elease, pos,.   
+0002c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c870: 2020 2020 2062 7574 746f 6e2c 2051 742e       button, Qt.
+0002c880: 4d6f 7573 6542 7574 746f 6e2e 4e6f 4275  MouseButton.NoBu
+0002c890: 7474 6f6e 2c20 6d6f 6469 6669 6572 290a  tton, modifier).
+0002c8a0: 2020 2020 5141 7070 6c69 6361 7469 6f6e      QApplication
+0002c8b0: 2e73 656e 6445 7665 6e74 2877 6964 6765  .sendEvent(widge
+0002c8c0: 742c 2065 7665 6e74 290a 0a0a 6465 6620  t, event)...def 
+0002c8d0: 5f6d 6f75 7365 4d6f 7665 2877 6964 6765  _mouseMove(widge
+0002c8e0: 742c 2070 6f73 2c20 6275 7474 6f6e 733d  t, pos, buttons=
+0002c8f0: 4e6f 6e65 2c20 6d6f 6469 6669 6572 3d4e  None, modifier=N
+0002c900: 6f6e 6529 3a0a 2020 2020 6966 2062 7574  one):.    if but
+0002c910: 746f 6e73 2069 7320 4e6f 6e65 3a0a 2020  tons is None:.  
+0002c920: 2020 2020 2020 6275 7474 6f6e 7320 3d20        buttons = 
+0002c930: 5174 2e4d 6f75 7365 4275 7474 6f6e 2e4e  Qt.MouseButton.N
+0002c940: 6f42 7574 746f 6e0a 2020 2020 6966 206d  oButton.    if m
+0002c950: 6f64 6966 6965 7220 6973 204e 6f6e 653a  odifier is None:
+0002c960: 0a20 2020 2020 2020 206d 6f64 6966 6965  .        modifie
+0002c970: 7220 3d20 5174 2e4b 6579 626f 6172 644d  r = Qt.KeyboardM
+0002c980: 6f64 6966 6965 722e 4e6f 4d6f 6469 6669  odifier.NoModifi
+0002c990: 6572 0a20 2020 2065 7665 6e74 203d 2051  er.    event = Q
+0002c9a0: 4d6f 7573 6545 7665 6e74 2851 4576 656e  MouseEvent(QEven
+0002c9b0: 742e 5479 7065 2e4d 6f75 7365 4d6f 7665  t.Type.MouseMove
+0002c9c0: 2c20 706f 732c 0a20 2020 2020 2020 2020  , pos,.         
+0002c9d0: 2020 2020 2020 2020 2020 2020 2020 2051                 Q
+0002c9e0: 742e 4d6f 7573 6542 7574 746f 6e2e 4e6f  t.MouseButton.No
+0002c9f0: 4275 7474 6f6e 2c20 6275 7474 6f6e 732c  Button, buttons,
+0002ca00: 206d 6f64 6966 6965 7229 0a20 2020 2051   modifier).    Q
+0002ca10: 4170 706c 6963 6174 696f 6e2e 7365 6e64  Application.send
+0002ca20: 4576 656e 7428 7769 6467 6574 2c20 6576  Event(widget, ev
+0002ca30: 656e 7429 0a0a 0a64 6566 205f 6d6f 7573  ent)...def _mous
+0002ca40: 6543 6c69 636b 2877 6964 6765 742c 2070  eClick(widget, p
+0002ca50: 6f73 2c20 6275 7474 6f6e 2c20 6d6f 6469  os, button, modi
+0002ca60: 6669 6572 3d4e 6f6e 6529 3a0a 2020 2020  fier=None):.    
+0002ca70: 5f6d 6f75 7365 4d6f 7665 2877 6964 6765  _mouseMove(widge
+0002ca80: 742c 2070 6f73 290a 2020 2020 5f6d 6f75  t, pos).    _mou
+0002ca90: 7365 5072 6573 7328 7769 6467 6574 2c20  sePress(widget, 
+0002caa0: 706f 732c 2062 7574 746f 6e2c 206d 6f64  pos, button, mod
+0002cab0: 6966 6965 7229 0a20 2020 205f 6d6f 7573  ifier).    _mous
+0002cac0: 6552 656c 6561 7365 2877 6964 6765 742c  eRelease(widget,
+0002cad0: 2070 6f73 2c20 6275 7474 6f6e 2c20 6d6f   pos, button, mo
+0002cae0: 6469 6669 6572 290a 0a0a 6465 6620 5f6d  difier)...def _m
+0002caf0: 6f75 7365 4472 6167 2877 6964 6765 742c  ouseDrag(widget,
+0002cb00: 2070 6f73 6974 696f 6e73 2c20 6275 7474   positions, butt
+0002cb10: 6f6e 2c20 6d6f 6469 6669 6572 3d4e 6f6e  on, modifier=Non
+0002cb20: 6529 3a0a 2020 2020 5f6d 6f75 7365 4d6f  e):.    _mouseMo
+0002cb30: 7665 2877 6964 6765 742c 2070 6f73 6974  ve(widget, posit
+0002cb40: 696f 6e73 5b30 5d29 0a20 2020 205f 6d6f  ions[0]).    _mo
+0002cb50: 7573 6550 7265 7373 2877 6964 6765 742c  usePress(widget,
+0002cb60: 2070 6f73 6974 696f 6e73 5b30 5d2c 2062   positions[0], b
+0002cb70: 7574 746f 6e2c 206d 6f64 6966 6965 7229  utton, modifier)
+0002cb80: 0a20 2020 2023 2044 656c 6179 2066 6f72  .    # Delay for
+0002cb90: 2031 3020 6d73 2066 6f72 2064 7261 6720   10 ms for drag 
+0002cba0: 746f 2062 6520 7265 636f 676e 697a 6564  to be recognized
+0002cbb0: 2e0a 2020 2020 5154 6573 742e 7157 6169  ..    QTest.qWai
+0002cbc0: 7428 3130 290a 2020 2020 666f 7220 706f  t(10).    for po
+0002cbd0: 7320 696e 2070 6f73 6974 696f 6e73 5b31  s in positions[1
+0002cbe0: 3a5d 3a0a 2020 2020 2020 2020 5f6d 6f75  :]:.        _mou
+0002cbf0: 7365 4d6f 7665 2877 6964 6765 742c 2070  seMove(widget, p
+0002cc00: 6f73 2c20 6275 7474 6f6e 2c20 6d6f 6469  os, button, modi
+0002cc10: 6669 6572 290a 2020 2020 5f6d 6f75 7365  fier).    _mouse
+0002cc20: 5265 6c65 6173 6528 7769 6467 6574 2c20  Release(widget, 
+0002cc30: 706f 7369 7469 6f6e 735b 2d31 5d2c 2062  positions[-1], b
+0002cc40: 7574 746f 6e2c 206d 6f64 6966 6965 7229  utton, modifier)
+0002cc50: 0a0a 0a23 206d 6f64 6966 6965 6420 6672  ...# modified fr
+0002cc60: 6f6d 3a20 6874 7470 733a 2f2f 6769 7468  om: https://gith
+0002cc70: 7562 2e63 6f6d 2f70 7976 6973 7461 2f70  ub.com/pyvista/p
+0002cc80: 7976 6973 7461 7174 0a64 6566 205f 7365  yvistaqt.def _se
+0002cc90: 7475 705f 6970 7974 686f 6e28 6970 7974  tup_ipython(ipyt
+0002cca0: 686f 6e3d 4e6f 6e65 293a 0a20 2020 2023  hon=None):.    #
+0002ccb0: 2069 7079 7468 6f6e 206d 6167 6963 0a20   ipython magic. 
+0002ccc0: 2020 2069 6620 7363 6f6f 6279 2e69 6e5f     if scooby.in_
+0002ccd0: 6970 7974 686f 6e28 293a 0a20 2020 2020  ipython():.     
+0002cce0: 2020 2066 726f 6d20 4950 7974 686f 6e20     from IPython 
+0002ccf0: 696d 706f 7274 2067 6574 5f69 7079 7468  import get_ipyth
+0002cd00: 6f6e 0a20 2020 2020 2020 2069 7079 7468  on.        ipyth
+0002cd10: 6f6e 203d 2067 6574 5f69 7079 7468 6f6e  on = get_ipython
+0002cd20: 2829 0a20 2020 2020 2020 2069 7079 7468  ().        ipyth
+0002cd30: 6f6e 2e72 756e 5f6c 696e 655f 6d61 6769  on.run_line_magi
+0002cd40: 6328 2267 7569 222c 2022 7174 2229 0a20  c("gui", "qt"). 
+0002cd50: 2020 2020 2020 2066 726f 6d20 4950 7974         from IPyt
+0002cd60: 686f 6e2e 6578 7465 726e 616c 2e71 745f  hon.external.qt_
+0002cd70: 666f 725f 6b65 726e 656c 2069 6d70 6f72  for_kernel impor
+0002cd80: 7420 5174 4775 690a 2020 2020 2020 2020  t QtGui.        
+0002cd90: 5174 4775 692e 5141 7070 6c69 6361 7469  QtGui.QApplicati
+0002cda0: 6f6e 2e69 6e73 7461 6e63 6528 290a 2020  on.instance().  
+0002cdb0: 2020 7265 7475 726e 2069 7079 7468 6f6e    return ipython
+0002cdc0: 0a0a 0a64 6566 205f 7174 5f69 6e69 745f  ...def _qt_init_
+0002cdd0: 6963 6f6e 7328 293a 0a20 2020 2066 726f  icons():.    fro
+0002cde0: 6d20 7174 7079 2e51 7447 7569 2069 6d70  m qtpy.QtGui imp
+0002cdf0: 6f72 7420 5149 636f 6e0a 2020 2020 6963  ort QIcon.    ic
+0002ce00: 6f6e 735f 7061 7468 203d 2066 227b 5061  ons_path = f"{Pa
+0002ce10: 7468 285f 5f66 696c 655f 5f29 2e70 6172  th(__file__).par
+0002ce20: 656e 747d 2f69 636f 6e73 220a 2020 2020  ent}/icons".    
+0002ce30: 5149 636f 6e2e 7365 7454 6865 6d65 5365  QIcon.setThemeSe
+0002ce40: 6172 6368 5061 7468 7328 5b69 636f 6e73  archPaths([icons
+0002ce50: 5f70 6174 685d 290a 2020 2020 7265 7475  _path]).    retu
+0002ce60: 726e 2069 636f 6e73 5f70 6174 680a 0a0a  rn icons_path...
+0002ce70: 6465 6620 5f69 6e69 745f 6272 6f77 7365  def _init_browse
+0002ce80: 7228 2a2a 6b77 6172 6773 293a 0a20 2020  r(**kwargs):.   
+0002ce90: 205f 7365 7475 705f 6970 7974 686f 6e28   _setup_ipython(
+0002cea0: 290a 2020 2020 7365 7443 6f6e 6669 674f  ).    setConfigO
+0002ceb0: 7074 696f 6e28 2765 6e61 626c 6545 7870  ption('enableExp
+0002cec0: 6572 696d 656e 7461 6c27 2c20 5472 7565  erimental', True
+0002ced0: 290a 2020 2020 6170 705f 6b77 6172 6773  ).    app_kwargs
+0002cee0: 203d 2064 6963 7428 290a 2020 2020 6966   = dict().    if
+0002cef0: 206b 7761 7267 732e 6765 7428 2773 706c   kwargs.get('spl
+0002cf00: 6173 6827 2c20 4661 6c73 6529 3a0a 2020  ash', False):.  
+0002cf10: 2020 2020 2020 6170 705f 6b77 6172 6773        app_kwargs
+0002cf20: 5b27 7370 6c61 7368 275d 203d 2027 496e  ['splash'] = 'In
+0002cf30: 6974 6961 6c69 7a69 6e67 206d 6e65 2d71  itializing mne-q
+0002cf40: 742d 6272 6f77 7365 722e 2e2e 270a 2020  t-browser...'.  
+0002cf50: 2020 6f75 7420 3d20 5f69 6e69 745f 6d6e    out = _init_mn
+0002cf60: 655f 7174 6170 7028 7067 5f61 7070 3d54  e_qtapp(pg_app=T
+0002cf70: 7275 652c 202a 2a61 7070 5f6b 7761 7267  rue, **app_kwarg
+0002cf80: 7329 0a20 2020 2069 6620 2773 706c 6173  s).    if 'splas
+0002cf90: 6827 2069 6e20 6170 705f 6b77 6172 6773  h' in app_kwargs
+0002cfa0: 3a0a 2020 2020 2020 2020 6b77 6172 6773  :.        kwargs
+0002cfb0: 5b27 7370 6c61 7368 275d 203d 206f 7574  ['splash'] = out
+0002cfc0: 5b31 5d20 2023 2072 6574 7572 6e65 6420  [1]  # returned 
+0002cfd0: 6173 2073 6563 6f6e 6420 656c 656d 656e  as second elemen
+0002cfe0: 740a 2020 2020 6272 6f77 7365 7220 3d20  t.    browser = 
+0002cff0: 4d4e 4551 7442 726f 7773 6572 282a 2a6b  MNEQtBrowser(**k
+0002d000: 7761 7267 7329 0a0a 2020 2020 7265 7475  wargs)..    retu
+0002d010: 726e 2062 726f 7773 6572 0a0a 0a63 6c61  rn browser...cla
+0002d020: 7373 2050 7951 7447 7261 7068 4272 6f77  ss PyQtGraphBrow
+0002d030: 7365 7228 4d4e 4551 7442 726f 7773 6572  ser(MNEQtBrowser
+0002d040: 293a 2020 2320 6e6f 7161 3a20 4431 3031  ):  # noqa: D101
+0002d050: 0a20 2020 2070 6173 7320 2023 206a 7573  .    pass  # jus
+0002d060: 7420 666f 7220 6261 636b 7761 7264 2063  t for backward c
+0002d070: 6f6d 7061 7420 7769 7468 204d 4e45 2031  ompat with MNE 1
+0002d080: 2e30 2073 6372 6170 696e 670a            .0 scraping.
```

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/conftest.py` & `mne-qt-browser-0.5.1/mne_qt_browser/conftest.py`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/less_channels.svg` & `mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/less_channels.svg`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/less_time.svg` & `mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/less_time.svg`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/more_channels.svg` & `mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/more_channels.svg`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/more_time.svg` & `mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/more_time.svg`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/icons/dark/actions/settings.svg` & `mne-qt-browser-0.5.1/mne_qt_browser/icons/dark/actions/settings.svg`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/less_channels.svg` & `mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/less_channels.svg`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/less_time.svg` & `mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/less_time.svg`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/more_channels.svg` & `mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/more_channels.svg`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/more_time.svg` & `mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/more_time.svg`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/icons/light/actions/settings.svg` & `mne-qt-browser-0.5.1/mne_qt_browser/icons/light/actions/settings.svg`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/tests/test_pg_specific.py` & `mne-qt-browser-0.5.1/mne_qt_browser/tests/test_pg_specific.py`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser/tests/test_speed.py` & `mne-qt-browser-0.5.1/mne_qt_browser/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser.egg-info/PKG-INFO` & `mne-qt-browser-0.5.1/mne_qt_browser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mne-qt-browser
-Version: 0.5.0
+Version: 0.5.1
 Summary: A new backend based on pyqtgraph for the 2D-Data-Browser in MNE-Python
 Author-email: Martin Schulz <dev@earthman-music.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2021-2022, authors of mne-qt-browser
         All rights reserved.
```

### Comparing `mne-qt-browser-0.5.0/mne_qt_browser.egg-info/SOURCES.txt` & `mne-qt-browser-0.5.1/mne_qt_browser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/pyproject.toml` & `mne-qt-browser-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mne-qt-browser-0.5.0/screenshot.png` & `mne-qt-browser-0.5.1/screenshot.png`

 * *Files identical despite different names*

