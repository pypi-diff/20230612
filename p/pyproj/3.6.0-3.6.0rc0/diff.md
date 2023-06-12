# Comparing `tmp/pyproj-3.6.0.tar.gz` & `tmp/pyproj-3.6.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproj-3.6.0.tar", last modified: Mon Jun 12 13:28:26 2023, max compression
+gzip compressed data, was "pyproj-3.6.0rc0.tar", last modified: Fri Jun  9 01:25:20 2023, max compression
```

## Comparing `pyproj-3.6.0.tar` & `pyproj-3.6.0rc0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:28:26.049971 pyproj-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-12 13:27:32.000000 pyproj-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-12 13:27:32.000000 pyproj-3.6.0/LICENSE_proj
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-12 13:27:32.000000 pyproj-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-12 13:27:32.000000 pyproj-3.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    30154 2023-06-12 13:28:26.049971 pyproj-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28684 2023-06-12 13:27:32.000000 pyproj-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:28:26.037971 pyproj-3.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/advanced_examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:28:26.041971 pyproj-3.6.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/aoi.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:28:26.041971 pyproj-3.6.0/docs/api/crs/
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/crs/coordinate_operation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/crs/coordinate_system.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/crs/crs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/crs/datum.rst
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/crs/enums.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/crs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/datadir.rst
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/enums.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/geod.rst
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/global_context.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/list.rst
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/network.rst
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/proj.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/show_versions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/sync.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/api/transformer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/build_crs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/build_crs_cf.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/cli.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2031 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/crs_compatibility.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15702 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/gotchas.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26440 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:28:26.041971 pyproj-3.6.0/docs/media/
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/media/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/media/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/media/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/media/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/optimize_transformations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/past_versions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-12 13:27:32.000000 pyproj-3.6.0/docs/transformation_grids.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:28:26.045971 pyproj-3.6.0/pyproj/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_compat.pxd
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_compat.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_crs.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_crs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    92777 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_crs.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_datadir.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_datadir.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_datadir.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_geod.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_geod.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20903 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_geod.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_network.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_network.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_show_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_sync.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_sync.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_transformer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_transformer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39998 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/_transformer.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/aoi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/base.pxi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:28:26.045971 pyproj-3.6.0/pyproj/crs/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/crs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27038 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/crs/_cf1x8.py
--rw-r--r--   0 runner    (1001) docker     (123)    57878 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/crs/coordinate_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/crs/coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    64099 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/crs/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/crs/datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/crs/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/database.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/database.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/datadir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    44078 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/geod.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/list.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    21319 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/proj.pxi
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/proj.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    44983 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproj/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:28:26.045971 pyproj-3.6.0/pyproj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30154 2023-06-12 13:28:26.000000 pyproj-3.6.0/pyproj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-12 13:28:26.000000 pyproj-3.6.0/pyproj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:28:26.000000 pyproj-3.6.0/pyproj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-12 13:28:26.000000 pyproj-3.6.0/pyproj.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:28:25.000000 pyproj-3.6.0/pyproj.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 13:28:26.000000 pyproj-3.6.0/pyproj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 13:28:26.000000 pyproj-3.6.0/pyproj.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-12 13:27:32.000000 pyproj-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-12 13:27:32.000000 pyproj-3.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:28:26.049971 pyproj-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-06-12 13:27:32.000000 pyproj-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:28:26.049971 pyproj-3.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:28:26.049971 pyproj-3.6.0/test/crs/
--rw-r--r--   0 runner    (1001) docker     (123)    55605 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/crs/test_crs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69167 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/crs/test_crs_cf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/crs/test_crs_coordinate_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/crs/test_crs_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/crs/test_crs_datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/crs/test_crs_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/crs/test_crs_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/sample.out
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_aoi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_awips221.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_datadir.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_datum_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_doctest_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_exception_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    27348 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_geod.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_proj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_show_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    56570 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-12 13:27:32.000000 pyproj-3.6.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.867084 pyproj-3.6.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/LICENSE_proj
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    30157 2023-06-09 01:25:20.863084 pyproj-3.6.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28684 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.839084 pyproj-3.6.0rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/advanced_examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.839084 pyproj-3.6.0rc0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/aoi.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.843084 pyproj-3.6.0rc0/docs/api/crs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/crs/coordinate_operation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/crs/coordinate_system.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/crs/crs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/crs/datum.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/crs/enums.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/crs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/datadir.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/enums.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/geod.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/global_context.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/network.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/proj.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/show_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/sync.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/transformer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/build_crs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/build_crs_cf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/cli.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2031 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/crs_compatibility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15702 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/gotchas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26440 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.843084 pyproj-3.6.0rc0/docs/media/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/media/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/media/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/media/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/media/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/optimize_transformations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/past_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/transformation_grids.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.855084 pyproj-3.6.0rc0/pyproj/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_compat.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_compat.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_crs.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_crs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    92777 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_crs.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_datadir.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_datadir.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_datadir.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_geod.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_geod.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20903 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_geod.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_network.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_network.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_sync.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_sync.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_transformer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_transformer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39998 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_transformer.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/base.pxi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.859084 pyproj-3.6.0rc0/pyproj/crs/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27038 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/_cf1x8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57878 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/coordinate_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64099 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/database.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/database.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/datadir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44078 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/geod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/list.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21319 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/proj.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/proj.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44983 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.855084 pyproj-3.6.0rc0/pyproj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30157 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 01:25:20.867084 pyproj-3.6.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.863084 pyproj-3.6.0rc0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.863084 pyproj-3.6.0rc0/test/crs/
+-rw-r--r--   0 runner    (1001) docker     (123)    55605 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69167 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs_coordinate_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs_datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/sample.out
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_aoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_awips221.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_datadir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_datum_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_doctest_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_exception_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27348 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_geod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_proj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56570 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_utils.py
```

### Comparing `pyproj-3.6.0/LICENSE` & `pyproj-3.6.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/LICENSE_proj` & `pyproj-3.6.0rc0/LICENSE_proj`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/Makefile` & `pyproj-3.6.0rc0/Makefile`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/PKG-INFO` & `pyproj-3.6.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproj
-Version: 3.6.0
+Version: 3.6.0rc0
 Summary: Python interface to PROJ (cartographic projections and coordinate transformations library)
 Home-page: https://github.com/pyproj4/pyproj
 Author-email: Jeff Whitaker <jeffrey.s.whitaker@noaa.gov>
 Maintainer: pyproj contributors
 License: MIT
 Project-URL: homepage, https://pyproj4.github.io/pyproj/
 Project-URL: documentation, https://pyproj4.github.io/pyproj/
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: pyproj Version: 3.6.0 Summary: Python interface to
-PROJ (cartographic projections and coordinate transformations library) Home-
+Metadata-Version: 2.1 Name: pyproj Version: 3.6.0rc0 Summary: Python interface
+to PROJ (cartographic projections and coordinate transformations library) Home-
 page: https://github.com/pyproj4/pyproj Author-email: Jeff Whitaker
 s.whitaker@noaa.gov> Maintainer: pyproj contributors License: MIT Project-URL:
 homepage, https://pyproj4.github.io/pyproj/ Project-URL: documentation, https:/
 /pyproj4.github.io/pyproj/ Project-URL: repository, https://github.com/pyproj4/
 pyproj Project-URL: changelog, https://pyproj4.github.io/pyproj/stable/
 history.html Keywords: GIS,map,geospatial,coordinate-systems,coordinate-
 transformation,cartographic-projection,geodesic Classifier: Development Status
```

### Comparing `pyproj-3.6.0/README.md` & `pyproj-3.6.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/Makefile` & `pyproj-3.6.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/advanced_examples.rst` & `pyproj-3.6.0rc0/docs/advanced_examples.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/api/crs/coordinate_operation.rst` & `pyproj-3.6.0rc0/docs/api/crs/coordinate_operation.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/api/crs/coordinate_system.rst` & `pyproj-3.6.0rc0/docs/api/crs/coordinate_system.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/api/crs/crs.rst` & `pyproj-3.6.0rc0/docs/api/crs/crs.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/api/crs/datum.rst` & `pyproj-3.6.0rc0/docs/api/crs/datum.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/api/crs/enums.rst` & `pyproj-3.6.0rc0/docs/api/crs/enums.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/api/database.rst` & `pyproj-3.6.0rc0/docs/api/database.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/api/global_context.rst` & `pyproj-3.6.0rc0/docs/api/global_context.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/api/list.rst` & `pyproj-3.6.0rc0/docs/api/list.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/api/transformer.rst` & `pyproj-3.6.0rc0/docs/api/transformer.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/build_crs.rst` & `pyproj-3.6.0rc0/docs/build_crs.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/build_crs_cf.rst` & `pyproj-3.6.0rc0/docs/build_crs_cf.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/conf.py` & `pyproj-3.6.0rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/crs_compatibility.rst` & `pyproj-3.6.0rc0/docs/crs_compatibility.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/examples.rst` & `pyproj-3.6.0rc0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/gotchas.rst` & `pyproj-3.6.0rc0/docs/gotchas.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/history.rst` & `pyproj-3.6.0rc0/docs/history.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/index.rst` & `pyproj-3.6.0rc0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/installation.rst` & `pyproj-3.6.0rc0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/make.bat` & `pyproj-3.6.0rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/media/icon.png` & `pyproj-3.6.0rc0/docs/media/icon.png`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/media/icon.svg` & `pyproj-3.6.0rc0/docs/media/icon.svg`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/media/logo.png` & `pyproj-3.6.0rc0/docs/media/logo.png`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/media/logo.svg` & `pyproj-3.6.0rc0/docs/media/logo.svg`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/past_versions.rst` & `pyproj-3.6.0rc0/docs/past_versions.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/docs/transformation_grids.rst` & `pyproj-3.6.0rc0/docs/transformation_grids.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/__init__.py` & `pyproj-3.6.0rc0/pyproj/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 from pyproj.transformer import (  # noqa: F401 pylint: disable=unused-import
     Transformer,
     itransform,
     proj_version_str,
     transform,
 )
 
-__version__ = "3.6.0"
+__version__ = "3.6.0rc0"
 __all__ = [
     "Proj",
     "Geod",
     "CRS",
     "Transformer",
     "transform",
     "itransform",
```

### Comparing `pyproj-3.6.0/pyproj/__main__.py` & `pyproj-3.6.0rc0/pyproj/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/_compat.pyx` & `pyproj-3.6.0rc0/pyproj/_compat.pyx`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/_crs.pxd` & `pyproj-3.6.0rc0/pyproj/_crs.pxd`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/_crs.pyi` & `pyproj-3.6.0rc0/pyproj/_crs.pyi`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/_crs.pyx` & `pyproj-3.6.0rc0/pyproj/_crs.pyx`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/_datadir.pyx` & `pyproj-3.6.0rc0/pyproj/_datadir.pyx`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/_geod.pxd` & `pyproj-3.6.0rc0/pyproj/_geod.pxd`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/_geod.pyi` & `pyproj-3.6.0rc0/pyproj/_geod.pyi`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/_geod.pyx` & `pyproj-3.6.0rc0/pyproj/_geod.pyx`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/_network.pyx` & `pyproj-3.6.0rc0/pyproj/_network.pyx`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/_show_versions.py` & `pyproj-3.6.0rc0/pyproj/_show_versions.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/_transformer.pxd` & `pyproj-3.6.0rc0/pyproj/_transformer.pxd`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/_transformer.pyi` & `pyproj-3.6.0rc0/pyproj/_transformer.pyi`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/_transformer.pyx` & `pyproj-3.6.0rc0/pyproj/_transformer.pyx`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/aoi.py` & `pyproj-3.6.0rc0/pyproj/aoi.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/base.pxi` & `pyproj-3.6.0rc0/pyproj/base.pxi`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/crs/__init__.py` & `pyproj-3.6.0rc0/pyproj/crs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/crs/_cf1x8.py` & `pyproj-3.6.0rc0/pyproj/crs/_cf1x8.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/crs/coordinate_operation.py` & `pyproj-3.6.0rc0/pyproj/crs/coordinate_operation.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/crs/coordinate_system.py` & `pyproj-3.6.0rc0/pyproj/crs/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/crs/crs.py` & `pyproj-3.6.0rc0/pyproj/crs/crs.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/crs/datum.py` & `pyproj-3.6.0rc0/pyproj/crs/datum.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/crs/enums.py` & `pyproj-3.6.0rc0/pyproj/crs/enums.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/database.pyi` & `pyproj-3.6.0rc0/pyproj/database.pyi`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/database.pyx` & `pyproj-3.6.0rc0/pyproj/database.pyx`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/datadir.py` & `pyproj-3.6.0rc0/pyproj/datadir.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/enums.py` & `pyproj-3.6.0rc0/pyproj/enums.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/exceptions.py` & `pyproj-3.6.0rc0/pyproj/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/geod.py` & `pyproj-3.6.0rc0/pyproj/geod.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/list.pyx` & `pyproj-3.6.0rc0/pyproj/list.pyx`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/network.py` & `pyproj-3.6.0rc0/pyproj/network.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/proj.pxi` & `pyproj-3.6.0rc0/pyproj/proj.pxi`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/proj.py` & `pyproj-3.6.0rc0/pyproj/proj.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/sync.py` & `pyproj-3.6.0rc0/pyproj/sync.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/transformer.py` & `pyproj-3.6.0rc0/pyproj/transformer.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj/utils.py` & `pyproj-3.6.0rc0/pyproj/utils.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproj.egg-info/PKG-INFO` & `pyproj-3.6.0rc0/pyproj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproj
-Version: 3.6.0
+Version: 3.6.0rc0
 Summary: Python interface to PROJ (cartographic projections and coordinate transformations library)
 Home-page: https://github.com/pyproj4/pyproj
 Author-email: Jeff Whitaker <jeffrey.s.whitaker@noaa.gov>
 Maintainer: pyproj contributors
 License: MIT
 Project-URL: homepage, https://pyproj4.github.io/pyproj/
 Project-URL: documentation, https://pyproj4.github.io/pyproj/
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: pyproj Version: 3.6.0 Summary: Python interface to
-PROJ (cartographic projections and coordinate transformations library) Home-
+Metadata-Version: 2.1 Name: pyproj Version: 3.6.0rc0 Summary: Python interface
+to PROJ (cartographic projections and coordinate transformations library) Home-
 page: https://github.com/pyproj4/pyproj Author-email: Jeff Whitaker
 s.whitaker@noaa.gov> Maintainer: pyproj contributors License: MIT Project-URL:
 homepage, https://pyproj4.github.io/pyproj/ Project-URL: documentation, https:/
 /pyproj4.github.io/pyproj/ Project-URL: repository, https://github.com/pyproj4/
 pyproj Project-URL: changelog, https://pyproj4.github.io/pyproj/stable/
 history.html Keywords: GIS,map,geospatial,coordinate-systems,coordinate-
 transformation,cartographic-projection,geodesic Classifier: Development Status
```

### Comparing `pyproj-3.6.0/pyproj.egg-info/SOURCES.txt` & `pyproj-3.6.0rc0/pyproj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/pyproject.toml` & `pyproj-3.6.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/setup.py` & `pyproj-3.6.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/conftest.py` & `pyproj-3.6.0rc0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/crs/test_crs.py` & `pyproj-3.6.0rc0/test/crs/test_crs.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/crs/test_crs_cf.py` & `pyproj-3.6.0rc0/test/crs/test_crs_cf.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/crs/test_crs_coordinate_operation.py` & `pyproj-3.6.0rc0/test/crs/test_crs_coordinate_operation.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/crs/test_crs_coordinate_system.py` & `pyproj-3.6.0rc0/test/crs/test_crs_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/crs/test_crs_datum.py` & `pyproj-3.6.0rc0/test/crs/test_crs_datum.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/crs/test_crs_json.py` & `pyproj-3.6.0rc0/test/crs/test_crs_json.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/crs/test_crs_maker.py` & `pyproj-3.6.0rc0/test/crs/test_crs_maker.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/sample.out` & `pyproj-3.6.0rc0/test/sample.out`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_aoi.py` & `pyproj-3.6.0rc0/test/test_aoi.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_awips221.py` & `pyproj-3.6.0rc0/test/test_awips221.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_cli.py` & `pyproj-3.6.0rc0/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_database.py` & `pyproj-3.6.0rc0/test/test_database.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_datadir.py` & `pyproj-3.6.0rc0/test/test_datadir.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_datum.py` & `pyproj-3.6.0rc0/test/test_datum.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_datum_shift.py` & `pyproj-3.6.0rc0/test/test_datum_shift.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_doctest_wrapper.py` & `pyproj-3.6.0rc0/test/test_doctest_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_geod.py` & `pyproj-3.6.0rc0/test/test_geod.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_list.py` & `pyproj-3.6.0rc0/test/test_list.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_network.py` & `pyproj-3.6.0rc0/test/test_network.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_pickle.py` & `pyproj-3.6.0rc0/test/test_pickle.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_proj.py` & `pyproj-3.6.0rc0/test/test_proj.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_show_versions.py` & `pyproj-3.6.0rc0/test/test_show_versions.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_sync.py` & `pyproj-3.6.0rc0/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_transform.py` & `pyproj-3.6.0rc0/test/test_transform.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_transformer.py` & `pyproj-3.6.0rc0/test/test_transformer.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.6.0/test/test_utils.py` & `pyproj-3.6.0rc0/test/test_utils.py`

 * *Files identical despite different names*

