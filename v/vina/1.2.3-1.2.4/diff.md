# Comparing `tmp/vina-1.2.3.tar.gz` & `tmp/vina-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vina-1.2.3.tar", last modified: Mon Nov  8 20:03:27 2021, max compression
+gzip compressed data, was "vina-1.2.4.tar", last modified: Mon Jun 12 17:59:27 2023, max compression
```

## Comparing `vina-1.2.3.tar` & `vina-1.2.4.tar`

### file list

```diff
@@ -1,81 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 20:03:27.874960 vina-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-11-08 20:02:50.486720 vina-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2849 2021-11-08 20:03:27.874960 vina-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2021-11-08 20:02:50.486720 vina-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-08 20:02:50.486720 vina-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)    15307 2021-11-08 20:02:50.486720 vina-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 20:03:27.862960 vina-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 20:03:27.874960 vina-1.2.3/src/lib/
--rwxr-xr-x   0 runner    (1001) docker     (121)    11024 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/ad4cache.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2417 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/ad4cache.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     2174 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/array3d.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     2098 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/atom.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1114 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/atom_base.h
--rwxr-xr-x   0 runner    (1001) docker     (121)    12956 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/atom_constants.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     2985 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/atom_type.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     3951 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/bfgs.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1307 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/brick.h
--rwxr-xr-x   0 runner    (1001) docker     (121)    13077 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/cache.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2515 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/cache.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     9259 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/common.h
--rwxr-xr-x   0 runner    (1001) docker     (121)    11290 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/conf.h
--rw-r--r--   0 runner    (1001) docker     (121)     6035 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/conf_independent.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3600 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/conf_independent.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1977 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/convert_substring.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1914 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/coords.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1068 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/coords.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1404 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/curl.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1766 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/file.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     4083 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/grid.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2288 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/grid.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1988 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/grid_dim.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1186 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/igrid.h
--rwxr-xr-x   0 runner    (1001) docker     (121)      863 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/incrementable.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1025 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/int_pow.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1821 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/macros.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     4503 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/matrix.h
--rwxr-xr-x   0 runner    (1001) docker     (121)    35312 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/model.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     9258 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/model.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     2952 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/monte_carlo.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1714 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/monte_carlo.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     2242 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/mutate.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)      906 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/mutate.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     7027 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/non_cache.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1376 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/non_cache.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     5325 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/parallel.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     3001 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/parallel_mc.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1211 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/parallel_mc.h
--rwxr-xr-x   0 runner    (1001) docker     (121)      848 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/parallel_progress.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1551 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/parallel_progress.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1373 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/parse_error.h
--rwxr-xr-x   0 runner    (1001) docker     (121)    25747 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/parse_pdbqt.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1213 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/parse_pdbqt.h
--rw-r--r--   0 runner    (1001) docker     (121)    16464 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/potentials.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     9027 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/precalculate.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1643 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/quasi_newton.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1171 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/quasi_newton.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     4408 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/quaternion.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     3019 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/quaternion.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     3091 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/random.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1487 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/random.h
--rw-r--r--   0 runner    (1001) docker     (121)     5291 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/scoring_function.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     2796 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/szv_grid.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1200 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/szv_grid.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     8614 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/tree.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1131 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/triangular_matrix_index.h
--rw-r--r--   0 runner    (1001) docker     (121)     2792 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2021-11-08 20:02:50.882727 vina-1.2.3/src/lib/utils.h
--rw-r--r--   0 runner    (1001) docker     (121)    36285 2021-11-08 20:02:50.886727 vina-1.2.3/src/lib/vina.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6445 2021-11-08 20:02:50.886727 vina-1.2.3/src/lib/vina.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 20:03:27.874960 vina-1.2.3/src/main/
--rw-r--r--   0 runner    (1001) docker     (121)    21621 2021-11-08 20:02:50.886727 vina-1.2.3/src/main/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 20:03:27.874960 vina-1.2.3/src/split/
--rw-r--r--   0 runner    (1001) docker     (121)     7701 2021-11-08 20:02:50.886727 vina-1.2.3/src/split/split.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 20:03:27.874960 vina-1.2.3/vina/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-11-08 20:02:50.486720 vina-1.2.3/vina/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2021-11-08 20:02:50.486720 vina-1.2.3/vina/autodock_vina.i
--rw-r--r--   0 runner    (1001) docker     (121)      696 2021-11-08 20:02:50.486720 vina-1.2.3/vina/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-11-08 20:02:50.486720 vina-1.2.3/vina/vina.i
--rw-r--r--   0 runner    (1001) docker     (121)    18896 2021-11-08 20:02:50.486720 vina-1.2.3/vina/vina.py
--rw-r--r--   0 runner    (1001) docker     (121)    16204 2021-11-08 20:02:50.486720 vina-1.2.3/vina/vina_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    32257 2021-11-08 20:02:50.486720 vina-1.2.3/vina/vina_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:59:27.886716 vina-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 17:58:58.318707 vina-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-12 17:59:27.886716 vina-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-12 17:58:58.318707 vina-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-12 17:58:58.318707 vina-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-12 17:58:58.318707 vina-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:59:27.882716 vina-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:59:27.886716 vina-1.2.4/src/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11024 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/ad4cache.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/ad4cache.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2174 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/array3d.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2098 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/atom.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/atom_base.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12956 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/atom_constants.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2985 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/atom_type.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3951 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/bfgs.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/brick.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12995 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/cache.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2515 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/cache.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9259 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/common.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11290 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/conf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/conf_independent.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/conf_independent.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1977 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/convert_substring.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1914 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/coords.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/coords.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/curl.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/file.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4083 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/grid.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2288 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/grid.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/grid_dim.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/igrid.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/incrementable.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1025 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/int_pow.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1821 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/macros.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4503 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/matrix.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35551 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/model.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9313 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/model.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/monte_carlo.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/monte_carlo.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2242 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/mutate.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      906 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/mutate.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7027 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/non_cache.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1437 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/non_cache.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5325 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parallel.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3001 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parallel_mc.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parallel_mc.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parallel_progress.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1551 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parallel_progress.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1373 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parse_error.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25194 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parse_pdbqt.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1213 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/parse_pdbqt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/potentials.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9027 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/precalculate.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/quasi_newton.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/quasi_newton.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4408 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/quaternion.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3019 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/quaternion.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/random.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/random.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/scoring_function.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2796 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/szv_grid.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1200 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/szv_grid.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8614 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/tree.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1131 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/triangular_matrix_index.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36141 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/vina.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-06-12 17:58:58.690706 vina-1.2.4/src/lib/vina.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:59:27.886716 vina-1.2.4/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)    23410 2023-06-12 17:58:58.690706 vina-1.2.4/src/main/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:59:27.886716 vina-1.2.4/src/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-12 17:58:58.694706 vina-1.2.4/src/split/split.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:59:27.886716 vina-1.2.4/vina/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 17:58:58.318707 vina-1.2.4/vina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-12 17:58:58.318707 vina-1.2.4/vina/autodock_vina.i
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-12 17:58:58.318707 vina-1.2.4/vina/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 17:58:58.318707 vina-1.2.4/vina/vina.i
+-rw-r--r--   0 runner    (1001) docker     (123)    19294 2023-06-12 17:58:58.318707 vina-1.2.4/vina/vina.py
```

### Comparing `vina-1.2.3/LICENSE` & `vina-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/PKG-INFO` & `vina-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: vina
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python interface to AutoDock Vina
 Home-page: https://ccsb.scripps.edu/
 Author: Diogo Santos Martins, Jerome Eberhardt, Andreas F. Tillack, Stefano Forli
 Author-email: forli@scripps.edu
 License: Apache-2.0
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
@@ -21,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.5.*
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AutoDock Vina - Python API
 
 ### Requirements
 
@@ -80,9 +79,7 @@
 
 ### Full documentation
 
 The installation instructions, documentation and tutorials can be found on [readthedocs.org](https://autodock-vina.readthedocs.io/en/latest/).
 
 ### Citations
 * Trott, O., & Olson, A. J. (2010). AutoDock Vina: improving the speed and accuracy of docking with a new scoring function, efficient optimization, and multithreading. Journal of computational chemistry, 31(2), 455-461.
-
-
```

### Comparing `vina-1.2.3/README.md` & `vina-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/setup.py` & `vina-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 import glob
 import platform
 import re
 import shutil
 import subprocess
 import sys
-import sysconfig
 from setuptools.command.build_ext import build_ext
 from setuptools.command.install import install
 from distutils.command.clean import clean
 from setuptools import setup, Extension
 from distutils.command.build import build
 from distutils.command.sdist import sdist
 from distutils.errors import DistutilsExecError
@@ -37,15 +36,15 @@
         __import__(package_name)
         return True
     except ImportError:
         return False
 
 
 def in_conda():
-    return os.path.exists(os.path.join(sys.prefix, 'conda-meta'))
+    return 'CONDA_DEFAULT_ENV' in os.environ.keys()
 
 
 def find_version():
     """Extract the current version of AutoDock Vina.
     
     The version will be obtained from (in priority order):
     1. version.py (file created only when using GitHub Actions)
@@ -101,17 +100,18 @@
     # Warn if the (major, minor) version of the installed OB doesn't match these python bindings
     if not is_package_installed("openbabel"):
         raise RuntimeError("Error: Openbabel is not installed.")
 
     py_ver = StrictVersion(find_package_version('openbabel'))
     py_major_ver, py_minor_ver = py_ver.version[:2]
 
-    if in_conda:
+    if in_conda():
         # It means that Openbabel was installed in an Anaconda env
-        data_pathname = sysconfig.get_path('data')
+        data_pathname = os.environ["CONDA_PREFIX"]
+        return 'CONDA_DEFAULT_ENV' in os.environ.keys()
         include_dirs = data_pathname + os.path.sep + 'include' + os.path.sep + 'openbabel{}'.format(py_major_ver)
         library_dirs = data_pathname + os.path.sep + 'lib'
 
         if os.path.isdir(include_dirs):
             print('Open Babel location automatically determined in Anaconda.')
             return include_dirs, library_dirs
         else:
@@ -144,16 +144,16 @@
 
         print('Open Babel location was set to default location.')
         return include_dirs, library_dirs
 
 
 def locate_boost():
     """Try to locate boost."""
-    if in_conda:
-        data_pathname = sysconfig.get_path('data')
+    if in_conda():
+        data_pathname = os.environ["CONDA_PREFIX"]
         include_dirs = data_pathname + os.path.sep + 'include'
         library_dirs = data_pathname + os.path.sep + 'lib'
         
         if os.path.isdir(include_dirs + os.path.sep + 'boost'):
             print('Boost library location automatically determined in this conda environment.')
             return include_dirs, library_dirs
         else:
@@ -354,15 +354,15 @@
     long_description=open(os.path.join(base_dir, 'README.md')).read(),
     long_description_content_type="text/markdown",
     zip_safe=False,
     cmdclass={'build': CustomBuild, 'build_ext': CustomBuildExt, 'install': CustomInstall, 'sdist': CustomSdist},
     packages=['vina'],
     package_dir=package_dir,
     install_requires=['numpy>=1.18'],
-    python_requires='>=3.5.*',
+    python_requires='>=3.5',
     ext_modules=[obextension],
     #entry_points={"console_scripts": ["vina = vina.vina_cli:main"]},
     classifiers=[
         'Environment :: Console',
         'Environment :: Other Environment',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
```

### Comparing `vina-1.2.3/src/lib/ad4cache.cpp` & `vina-1.2.4/src/lib/ad4cache.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/ad4cache.h` & `vina-1.2.4/src/lib/ad4cache.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/array3d.h` & `vina-1.2.4/src/lib/array3d.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/atom.h` & `vina-1.2.4/src/lib/atom.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/atom_base.h` & `vina-1.2.4/src/lib/atom_base.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/atom_constants.h` & `vina-1.2.4/src/lib/atom_constants.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/atom_type.h` & `vina-1.2.4/src/lib/atom_type.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/bfgs.h` & `vina-1.2.4/src/lib/bfgs.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/brick.h` & `vina-1.2.4/src/lib/brick.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/cache.cpp` & `vina-1.2.4/src/lib/cache.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 }
 
 fl cache::eval(const model& m, fl v) const { // needs m.coords
 	fl e = 0;
 	sz nat = num_atom_types(atom_type::XS);
 
 	VINA_FOR(i, m.num_movable_atoms()) {
-		if(!m.is_atom_in_ligand(i)) continue; // we only want ligand - grid interaction
 		const atom& a = m.atoms[i];
 		sz t = a.get(atom_type::XS);
 
 		if (t >= nat) { continue; }
 		switch (t)
 		{
 			case XS_TYPE_G0:
```

### Comparing `vina-1.2.3/src/lib/cache.h` & `vina-1.2.4/src/lib/cache.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/common.h` & `vina-1.2.4/src/lib/common.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/conf.h` & `vina-1.2.4/src/lib/conf.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/conf_independent.cpp` & `vina-1.2.4/src/lib/conf_independent.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/conf_independent.h` & `vina-1.2.4/src/lib/conf_independent.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/convert_substring.h` & `vina-1.2.4/src/lib/convert_substring.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/coords.cpp` & `vina-1.2.4/src/lib/coords.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/coords.h` & `vina-1.2.4/src/lib/coords.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/curl.h` & `vina-1.2.4/src/lib/curl.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/file.h` & `vina-1.2.4/src/lib/file.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/grid.cpp` & `vina-1.2.4/src/lib/grid.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/grid.h` & `vina-1.2.4/src/lib/grid.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/grid_dim.h` & `vina-1.2.4/src/lib/grid_dim.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/igrid.h` & `vina-1.2.4/src/lib/igrid.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/incrementable.h` & `vina-1.2.4/src/lib/incrementable.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/int_pow.h` & `vina-1.2.4/src/lib/int_pow.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/macros.h` & `vina-1.2.4/src/lib/macros.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/matrix.h` & `vina-1.2.4/src/lib/matrix.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/model.cpp` & `vina-1.2.4/src/lib/model.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -219,15 +219,15 @@
 	- flex     - ligand   : YES (inter_pairs)
 	- flex_i   - flex_j   : YES (other_pairs) but append is used mostly for adding ligand
 	- ligand_i - ligand_j : YES (inter_pairs)
 	- macrocycle closure interactions: NO (1-2, 1-3, 1-4)
 	*/
 	VINA_FOR(i, m_num_movable_atoms) {
 		VINA_RANGE(j, m_num_movable_atoms, m_num_movable_atoms + m.m_num_movable_atoms) {
-			if (is_closure_clash(i, j)) continue; // 1-2, 1-3 or 1-4 interaction around CG-CG bond
+			if (is_closure_clash(i, j) || is_unmatched_closure_dummy(i, j)) continue;
 
 			const atom& a = atoms[i];
 			const atom& b = atoms[j];
 
 			sz t1 = a.get(atom_typing_used());
 			sz t2 = b.get(atom_typing_used());
 			sz n = num_atom_types(atom_typing_used());
@@ -512,28 +512,41 @@
 		(t1 == AD_TYPE_CG2 && t2 == AD_TYPE_G2) || (t2 == AD_TYPE_CG2 && t1 == AD_TYPE_G2) ||
 		(t1 == AD_TYPE_CG3 && t2 == AD_TYPE_G3) || (t2 == AD_TYPE_CG3 && t1 == AD_TYPE_G3))
 		return true;
 	else
 		return false;
 }
 
+// exclude pair if one atom is G0 but the other atom is not CG0
+bool model::is_unmatched_closure_dummy(sz i, sz j) const {
+	sz t1 = atoms[i].get(atom_type::AD);
+	sz t2 = atoms[j].get(atom_type::AD);
+	if ((t1==AD_TYPE_G0 && t2!=AD_TYPE_CG0) || (t2==AD_TYPE_G0 && t1!=AD_TYPE_CG0) ||
+    	(t1==AD_TYPE_G1 && t2!=AD_TYPE_CG1) || (t2==AD_TYPE_G1 && t1!=AD_TYPE_CG1) ||
+    	(t1==AD_TYPE_G2 && t2!=AD_TYPE_CG2) || (t2==AD_TYPE_G2 && t1!=AD_TYPE_CG2) ||
+    	(t1==AD_TYPE_G3 && t2!=AD_TYPE_CG3) || (t2==AD_TYPE_G3 && t1!=AD_TYPE_CG3))
+		return true;
+	else
+		return false;
+}
+
 void model::initialize_pairs(const distance_type_matrix& mobility) {
 	/* Interactions:
 	- ligand_i - ligand_i : YES (1-4 only) (ligand.pairs)
 	- flex_i   - flex_i   : YES (1-4 only) (other_pairs)
 	- flex_i   - flex_j   : YES (other_pairs)
 	- intra macrocycle closure interactions: NO (1-2, 1-3, 1-4)
 	*/
 	VINA_FOR_IN(i, atoms) {
 		sz i_lig = find_ligand(i);
 		szv bonded_atoms = bonded_to(i, 3);   // up to 1-4
 
 		VINA_RANGE(j, i + 1, atoms.size()) {
 			if (mobility(i, j) == DISTANCE_VARIABLE && !has(bonded_atoms, j)) {
-                if (is_closure_clash(i, j)) continue;  // 1-2, 1-3 or 1-4 interaction around CG-CG bond
+				if (is_closure_clash(i, j) || is_unmatched_closure_dummy(i, j)) continue;
 				
 				sz t1 = atoms[i].get(atom_typing_used());
 				sz t2 = atoms[j].get(atom_typing_used());
 				sz n  = num_atom_types(atom_typing_used());
 
 				if (t1 < n && t2 < n) { // exclude, say, Hydrogens
 					sz type_pair_index = triangular_matrix_index_permissive(n, t1, t2);
@@ -858,23 +871,14 @@
 		if (r2 < cutoff_sqr) {
 			fl this_e = p.eval_fast(pair.a, pair.b, r2);
 			curl(this_e, v[2]);
 			e += this_e;
 		}
 	}
 
-	// glue_i - glue_i and glue_i - glue_j interactions (no cutoff)
-	VINA_FOR_IN(i, glue_pairs) {
-		const interacting_pair& pair = glue_pairs[i];
-		fl r2 = vec_distance_sqr(coords[pair.a], coords[pair.b]);
-		fl this_e = p.eval_fast(pair.a, pair.b, r2);
-		curl(this_e, v[2]);
-		e += this_e;
-	}
-
 	return e;
 }
 
 fl model::rmsd_lower_bound_asymmetric(const model& x, const model& y) const { // actually static
 	sz n = x.m_num_movable_atoms; 
 	VINA_CHECK(n == y.m_num_movable_atoms);
 	fl sum = 0;
```

### Comparing `vina-1.2.3/src/lib/model.h` & `vina-1.2.4/src/lib/model.h`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,15 @@
 	
 	atom_index sz_to_atom_index(sz i) const; // grid_atoms, atoms
 	bool bonded_to_HD(const atom& a) const;
 	bool bonded_to_heteroatom(const atom& a) const;
 	void bonded_to(sz a, sz n, szv& out) const;
 	szv bonded_to(sz a, sz n) const;
     bool is_closure_clash(sz i, sz j) const;
+    bool is_unmatched_closure_dummy(sz i, sz j) const;
 	bool is_glue_pair(sz i, sz j) const;
 
 	void assign_bonds(const distance_type_matrix& mobility); // assign bonds based on relative mobility, distance and covalent length
 	void assign_types();
 	void initialize_pairs(const distance_type_matrix& mobility);
 	void initialize(const distance_type_matrix& mobility);
 	fl clash_penalty_aux(const interacting_pairs& pairs) const;
```

### Comparing `vina-1.2.3/src/lib/monte_carlo.cpp` & `vina-1.2.4/src/lib/monte_carlo.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/monte_carlo.h` & `vina-1.2.4/src/lib/monte_carlo.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/mutate.cpp` & `vina-1.2.4/src/lib/mutate.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/mutate.h` & `vina-1.2.4/src/lib/mutate.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/non_cache.cpp` & `vina-1.2.4/src/lib/non_cache.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/non_cache.h` & `vina-1.2.4/src/lib/non_cache.h`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 struct non_cache : public igrid {
     non_cache() {}
 	non_cache(const model& m, const grid_dims& gd_, const precalculate* p_, fl slope_);
 	virtual fl eval      (const model& m, fl v) const; // needs m.coords // clean up
 	virtual fl eval_intra(      model& m, fl v) const;
 	virtual fl eval_deriv(      model& m, fl v) const; // needs m.coords, sets m.minus_forces // clean up
-	bool within(const model& m, fl margin = 0.0001) const;
+	bool within(const model& m, fl margin = -0.0001) const; // negative margin ensures we stay inside (thanks Andreas!)
 	fl slope;
 private:
 	szv_grid sgrid;
 	grid_dims gd;
 	const precalculate* p;
 };
```

### Comparing `vina-1.2.3/src/lib/parallel.h` & `vina-1.2.4/src/lib/parallel.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/parallel_mc.cpp` & `vina-1.2.4/src/lib/parallel_mc.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/parallel_mc.h` & `vina-1.2.4/src/lib/parallel_mc.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/parallel_progress.cpp` & `vina-1.2.4/src/lib/parallel_progress.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/parallel_progress.h` & `vina-1.2.4/src/lib/parallel_progress.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/parse_error.h` & `vina-1.2.4/src/lib/parse_error.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/parse_pdbqt.cpp` & `vina-1.2.4/src/lib/parse_pdbqt.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -620,41 +620,28 @@
     }
 };
 
 
 model parse_ligand_pdbqt_from_file(const std::string& name, atom_type::t atype) { // can throw parse_error
     non_rigid_parsed nrp;
     context c;
-
-    try {
-        parse_pdbqt_ligand(make_path(name), nrp, c);
-    }
-    catch(pdbqt_parse_error& e) {
-        std::cerr << e.what();
-        exit(EXIT_FAILURE);
-    }
+    parse_pdbqt_ligand(make_path(name), nrp, c);
 
     pdbqt_initializer tmp(atype);
     tmp.initialize_from_nrp(nrp, c, true);
     tmp.initialize(nrp.mobility_matrix());
     return tmp.m;
 }
 
 model parse_ligand_pdbqt_from_string(const std::string& string_name, atom_type::t atype) { // can throw parse_error
     non_rigid_parsed nrp;
     context c;
 
-    try {
-        std::stringstream molstream(string_name);
-        parse_pdbqt_ligand(molstream, nrp, c);
-    }
-    catch(pdbqt_parse_error& e) {
-        std::cerr << e.what() << '\n';
-        exit(EXIT_FAILURE);
-    }
+    std::stringstream molstream(string_name);
+    parse_pdbqt_ligand(molstream, nrp, c);
 
     pdbqt_initializer tmp(atype);
     tmp.initialize_from_nrp(nrp, c, true);
     tmp.initialize(nrp.mobility_matrix());
     return tmp.m;
 }
 
@@ -668,31 +655,19 @@
 
     rigid r;
     non_rigid_parsed nrp;
     context c;
     pdbqt_initializer tmp(atype);
 
     if (!rigid_name.empty()) {
-        try {
-            parse_pdbqt_rigid(make_path(rigid_name), r);
-        }
-        catch(pdbqt_parse_error& e) {
-            std::cerr << e.what() << '\n';
-            exit(EXIT_FAILURE);
-        }
+        parse_pdbqt_rigid(make_path(rigid_name), r);
     }
     
     if (!flex_name.empty()) {
-        try {
-            parse_pdbqt_flex(make_path(flex_name), nrp, c);
-        }
-        catch(pdbqt_parse_error& e) {
-            std::cerr << e.what() << '\n';
-            exit(EXIT_FAILURE);
-        }
+        parse_pdbqt_flex(make_path(flex_name), nrp, c);
     }
 
     if (!rigid_name.empty()) {
         tmp.initialize_from_rigid(r);
         if (flex_name.empty()) {
             distance_type_matrix mobility_matrix;
             tmp.initialize(mobility_matrix);
```

### Comparing `vina-1.2.3/src/lib/parse_pdbqt.h` & `vina-1.2.4/src/lib/parse_pdbqt.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/potentials.h` & `vina-1.2.4/src/lib/potentials.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/precalculate.h` & `vina-1.2.4/src/lib/precalculate.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/quasi_newton.cpp` & `vina-1.2.4/src/lib/quasi_newton.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/quasi_newton.h` & `vina-1.2.4/src/lib/quasi_newton.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/quaternion.cpp` & `vina-1.2.4/src/lib/quaternion.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/quaternion.h` & `vina-1.2.4/src/lib/quaternion.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/random.cpp` & `vina-1.2.4/src/lib/random.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/random.h` & `vina-1.2.4/src/lib/random.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/scoring_function.h` & `vina-1.2.4/src/lib/scoring_function.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/szv_grid.cpp` & `vina-1.2.4/src/lib/szv_grid.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/szv_grid.h` & `vina-1.2.4/src/lib/szv_grid.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/tree.h` & `vina-1.2.4/src/lib/tree.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/triangular_matrix_index.h` & `vina-1.2.4/src/lib/triangular_matrix_index.h`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/src/lib/utils.cpp` & `vina-1.2.4/src/lib/utils.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -57,19 +57,32 @@
     std::string tmp = input_name;
     if (tmp.size() >= 6 && tmp.substr(tmp.size()-6, 6) == ".pdbqt")
         tmp.resize(tmp.size() - 6); // FIXME?
     return tmp + "_out.pdbqt";
 }
 
 
+std::string default_output(const std::string& input_name, int idx) {
+    std::string tmp = input_name;
+    if (tmp.size() >= 6 && tmp.substr(tmp.size()-6, 6) == ".pdbqt")
+        tmp.resize(tmp.size() - 6); // FIXME?
+    return tmp + "_instance" + std::to_string(idx) + "_out.pdbqt";
+}
+
+
 std::string default_output(const std::string& input_name, const std::string& directory_pathname) {
     return directory_pathname + separator() + default_output(input_name);
 }
 
 
+std::string default_output(const std::string& input_name, const std::string& directory_pathname, int idx) {
+    return directory_pathname + separator() + default_output(input_name, idx);
+}
+
+
 bool is_directory(const std::string& directory_pathname) {
   //Source: https://stackoverflow.com/questions/18100097/portable-way-to-check-if-directory-exists-windows-linux-c
   struct stat info;
 
     if (stat(directory_pathname.c_str(), &info) != 0) 
         return false;
     else if (info.st_mode & S_IFDIR)  // S_ISDIR() doesn't exist on my windows
```

### Comparing `vina-1.2.3/src/lib/utils.h` & `vina-1.2.4/src/lib/utils.h`

 * *Files 12% similar despite different names*

```diff
@@ -29,13 +29,15 @@
 #include "file.h"
 
 inline char separator();
 path make_path(const std::string& str);
 void doing(const std::string& str, int verbosity, int level=0);
 void done(int verbosity, int level=0);
 std::string default_output(const std::string& input_name);
+std::string default_output(const std::string& input_name, int i);
 std::string default_output(const std::string& input_name, const std::string& directory_pathname);
+std::string default_output(const std::string& input_name, const std::string& directory_pathname, int i);
 bool is_directory(const std::string& directory_pathname);
 std::string get_filename(const std::string& s);
 std::string get_file_contents(const std::string& filename);
 
 #endif
```

### Comparing `vina-1.2.3/src/lib/vina.cpp` & `vina-1.2.4/src/lib/vina.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -316,23 +316,20 @@
 	return box_dimensions;
 }
 
 void Vina::compute_vina_maps(double center_x, double center_y, double center_z, double size_x, double size_y, double size_z, double granularity, bool force_even_voxels) {
 	// Setup the search box
 	// Check first that the receptor was added
 	if (m_sf_choice == SF_AD42) {
-		std::cerr << "ERROR: Cannot compute Vina affinity maps using the AD4 scoring function.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("Cannot compute Vina affinity maps using the AD4 scoring function.");
 	} else if (!m_receptor_initialized) {
 		// m_model
-		std::cerr << "ERROR: Cannot compute Vina or Vinardo affinity maps. The (rigid) receptor was not initialized.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("Cannot compute Vina or Vinardo affinity maps. The (rigid) receptor was not initialized.");
 	} else if (size_x <= 0 || size_y <= 0 || size_z <= 0) {
-		std::cerr << "ERROR: Grid box dimensions must be greater than 0 Angstrom.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("Grid box dimensions must be greater than 0 Angstrom");
 	} else if (size_x * size_y * size_z > 27e3) {
 		std::cerr << "WARNING: Search space volume is greater than 27000 Angstrom^3 (See FAQ)\n";
 	}
 
 	grid_dims gd;
 	vec span(size_x, size_y, size_z);
 	vec center(center_x, center_y, center_z);
@@ -425,16 +422,15 @@
 	// Store in Vina object
 	m_map_initialized = true;
 }
 
 void Vina::write_maps(const std::string& map_prefix, const std::string& gpf_filename,
 					  const std::string& fld_filename, const std::string& receptor_filename) {
 	if (!m_map_initialized) {
-		std::cerr << "ERROR: Cannot write affinity maps. Affinity maps were not initialized.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("Cannot write affinity maps. Affinity maps were not initialized.");
 	}
 
 	szv atom_types;
 	atom_type::t atom_typing = m_scoring_function.get_atom_typing();
 
 	if (m_ligand_initialized)
 		atom_types = m_model.get_movable_atom_types(atom_typing);
@@ -457,21 +453,19 @@
 
 std::vector< std::vector<double> > Vina::get_poses_coordinates(int how_many, double energy_range) {
 	int n = 0;
 	double best_energy = 0;
 	std::vector< std::vector<double> > coordinates;
 
 	if (how_many < 0) {
-		std::cerr << "Error: number of poses asked must be greater than zero.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("number of poses asked must be greater than zero.");
 	}
 
 	if (energy_range < 0) {
-		std::cerr << "Error: energy range must be greater than zero.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("energy range must be greater than zero.");
 	}
 
 	if (!m_poses.empty()) {
 		// Get energy from the best conf
 		best_energy = m_poses[0].e;
 
 		VINA_FOR_IN(i, m_poses) {
@@ -501,21 +495,19 @@
 
 std::vector< std::vector<double> > Vina::get_poses_energies(int how_many, double energy_range) {
 	int n = 0;
 	double best_energy = 0;
 	std::vector< std::vector<double> > energies;
 
 	if (how_many < 0) {
-		std::cerr << "Error: number of poses asked must be greater than zero.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("number of poses asked must be greater than zero.");
 	}
 
 	if (energy_range < 0) {
-		std::cerr << "Error: energy range must be greater than zero.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("energy range must be greater than zero.");
 	}
 
 	if (!m_poses.empty()) {
 		// Get energy from the best conf
 		best_energy = m_poses[0].e;
 
 		VINA_FOR_IN(i, m_poses) {
@@ -566,21 +558,19 @@
 std::string Vina::get_poses(int how_many, double energy_range) {
 	int n = 0;
 	double best_energy = 0;
 	std::ostringstream out;
 	std::string remarks;
 
 	if (how_many < 0) {
-		std::cerr << "Error: number of poses written must be greater than zero.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("number of poses written must be greater than zero.");
 	}
 
 	if (energy_range < 0) {
-		std::cerr << "Error: energy range must be greater than zero.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("energy range must be greater than zero.");
 	}
 
 	if (!m_poses.empty()) {
 		// Get energy from the best conf
 		best_energy = m_poses[0].e;
 
 		VINA_FOR_IN(i, m_poses) {
@@ -639,19 +629,17 @@
 	m_model.write_structure(f, format_remark.str());
 }
 
 void Vina::randomize(const int max_steps) {
 	// Randomize ligand/flex residues conformation
 	// Check the box was defined
 	if (!m_ligand_initialized) {
-		std::cerr << "ERROR: Cannot do ligand randomization. Ligand(s) was(ere) not initialized.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("Cannot do ligand randomization. Ligand(s) was(ere) not initialized.");
 	} else if (!m_map_initialized) {
-		std::cerr << "ERROR: Cannot do ligand randomization. Affinity maps were not initialized.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("Cannot do ligand randomization. Affinity maps were not initialized.");
 	}
 
 	conf c;
 	int seed = generate_seed();
 	double penalty = 0;
 	double best_clash_penalty = 0;
 	std::stringstream sstm;
@@ -662,14 +650,15 @@
 	conf best_conf = init_conf;
 
 	sstm << "Randomize conformation (random seed: " << seed << ")";
 	doing(sstm.str(), m_verbosity, 0);
 	VINA_FOR(i, max_steps) {
 		c = init_conf;
 		c.randomize(m_grid.corner1(), m_grid.corner2(), generator);
+		m_model.set(c);
 		penalty = m_model.clash_penalty();
 
 		if (i == 0 || penalty < best_clash_penalty) {
 			best_conf = c;
 			best_clash_penalty = penalty;
 		}
 	}
@@ -679,15 +668,15 @@
 
 	if (m_verbosity > 1) {
 		std::cout << "Clash penalty: " << best_clash_penalty << "\n";
 	}
 }
 
 void Vina::show_score(const std::vector<double> energies) {
-	std::cout << "Estimated Free Energy of Binding   : " << std::fixed << std::setprecision(3) << energies[0] << " (kcal/mol) [=(1)+(2)+(3)+(4)]\n";
+	std::cout << "Estimated Free Energy of Binding   : " << std::fixed << std::setprecision(3) << energies[0] << " (kcal/mol) [=(1)+(2)+(3)-(4)]\n";
 	std::cout << "(1) Final Intermolecular Energy    : " << std::fixed << std::setprecision(3) << energies[1] + energies[2] << " (kcal/mol)\n";
 	std::cout << "    Ligand - Receptor              : " << std::fixed << std::setprecision(3) << energies[1] << " (kcal/mol)\n";
 	std::cout << "    Ligand - Flex side chains      : " << std::fixed << std::setprecision(3) << energies[2] << " (kcal/mol)\n";
 	std::cout << "(2) Final Total Internal Energy    : " << std::fixed << std::setprecision(3) << energies[3] + energies[4] + energies[5] << " (kcal/mol)\n";
 	std::cout << "    Ligand                         : " << std::fixed << std::setprecision(3) << energies[5] << " (kcal/mol)\n";
 	std::cout << "    Flex   - Receptor              : " << std::fixed << std::setprecision(3) << energies[3] << " (kcal/mol)\n";
 	std::cout << "    Flex   - Flex side chains      : " << std::fixed << std::setprecision(3) << energies[4] << " (kcal/mol)\n";
@@ -758,33 +747,30 @@
 	energies.push_back(intra_pairs);
 	energies.push_back(lig_intra);
 	energies.push_back(conf_independent);
 
 	if (m_sf_choice == SF_VINA  || m_sf_choice == SF_VINARDO) {
 		energies.push_back(intramolecular_energy);
 	} else {
-		energies.push_back(-intra);
+		energies.push_back(intra);
 	}
 
 	return energies;
 }
 
 std::vector<double> Vina::score() {
 	// Score the current conf in the model
 	// Check if ff and ligand were initialized
 	// Check if the ligand is not outside the box
 	if (!m_ligand_initialized) {
-		std::cerr << "ERROR: Cannot score the pose. Ligand(s) was(ere) not initialized.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("Cannot score the pose. Ligand(s) was(ere) not initialized.");
 	} else if (!m_map_initialized) {
-		std::cerr << "ERROR: Cannot score the pose. Affinity maps were not initialized.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("Cannot score the pose. Affinity maps were not initialized.");
 	} else if (!m_grid.is_in_grid(m_model)) {
-		std::cerr << "ERROR: The ligand is outside the grid box. Increase the size of the grid box or center it accordingly around the ligand.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("The ligand is outside the grid box. Increase the size of the grid box or center it accordingly around the ligand.");
 	}
 
 	double intramolecular_energy = 0;
 	const vec authentic_v(1000, 1000, 1000);
 
 	if(m_sf_choice == SF_VINA || m_sf_choice == SF_VINARDO) {
 		intramolecular_energy = m_model.eval_intramolecular(m_precalculated_byatom, m_grid, authentic_v);
@@ -840,22 +826,19 @@
 }
 
 std::vector<double> Vina::optimize(int max_steps) {
 	// Local optimization of the ligand conf
 	// Check if ff, box and ligand were initialized
 	// Check if the ligand is not outside the box
 	if (!m_ligand_initialized) {
-		std::cerr << "ERROR: Cannot do the optimization. Ligand(s) was(ere) not initialized.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("Cannot do the optimization. Ligand(s) was(ere) not initialized.");
 	} else if (!m_map_initialized) {
-		std::cerr << "ERROR: Cannot do the optimization. Affinity maps were not initialized.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("Cannot do the optimization. Affinity maps were not initialized.");
 	} else if (!m_grid.is_in_grid(m_model)) {
-		std::cerr << "ERROR: The ligand is outside the grid box. Increase the size of the grid box or center it accordingly around the ligand.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("The ligand is outside the grid box. Increase the size of the grid box or center it accordingly around the ligand.");
 	}
 
 	double e = 0;
 	conf c;
 
 	if (!m_poses.empty()) {
 		// if m_poses is not empty, it means that we did a docking before
@@ -880,22 +863,19 @@
 	return tmp;
 }
 
 void Vina::global_search(const int exhaustiveness, const int n_poses, const double min_rmsd, const int max_evals) {
 	// Vina search (Monte-carlo and local optimization)
 	// Check if ff, box and ligand were initialized
 	if (!m_ligand_initialized) {
-		std::cerr << "ERROR: Cannot do the global search. Ligand(s) was(ere) not initialized.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("Cannot do the global search. Ligand(s) was(ere) not initialized.");
 	} else if (!m_map_initialized) {
-		std::cerr << "ERROR: Cannot do the global search. Affinity maps were not initialized.\n";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("Cannot do the global search. Affinity maps were not initialized.");
 	} else if (exhaustiveness < 1) {
-		std::cerr << "ERROR: Exhaustiveness must be 1 or greater";
-		exit(EXIT_FAILURE);
+		throw vina_runtime_error("Exhaustiveness must be 1 or greater");
 	}
 
 	if (exhaustiveness < m_cpu) {
 		std::cerr << "WARNING: At low exhaustiveness, it may be impossible to utilize all CPUs.\n";
 	}
 
 	double e = 0;
@@ -960,14 +940,16 @@
 					poses[i].coords = m_model.get_heavy_atom_movable_coords();
 					if (!m_non_cache.within(m_model))
 						poses[i].e = max_fl;
 					m_non_cache.slope = slope;
 				}
 			}
 
+			poses.sort(); // order often changes after non_cache refinement
+			m_model.set(poses[0].c);
 			if (m_no_refine || !m_receptor_initialized)
 				intramolecular_energy = m_model.eval_intramolecular(m_precalculated_byatom, m_grid, authentic_v);
 			else
 				intramolecular_energy = m_model.eval_intramolecular(m_precalculated_byatom, m_non_cache, authentic_v);
 		}
 
 		VINA_FOR_IN(i, poses) {
@@ -988,16 +970,18 @@
 
 			if (m_verbosity > 1) {
 				std::cout << "FINAL ENERGY: \n";
 				show_score(energies);
 			}
 		}
 
-		// Since pose.e contains the final energy, we have to sort them again
-		poses.sort();
+		// In AD4, the unbound energy is intra for each pose, so order may have changed
+		// The order does not change in Vina because unbound is intra of the 1st pose
+		if (m_sf_choice == SF_AD42)
+			poses.sort();
 
 		// Now compute RMSD from the best model
 		// Necessary to do it in two pass for AD4 scoring function
 		m_model.set(poses[0].c);
 		best_model = m_model;
 
 		if (m_verbosity > 0) {
```

### Comparing `vina-1.2.3/src/lib/vina.h` & `vina-1.2.4/src/lib/vina.h`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,27 @@
 #include "quasi_newton.h"
 #include "coords.h" // add_to_output_container
 #include "utils.h"
 #include "scoring_function.h"
 #include "precalculate.h"
 
 
+class vina_runtime_error : public std::exception {
+public:
+    explicit vina_runtime_error(const std::string & message)
+            : m_message("\n\nVina runtime error: " + message + "\n") {}
+
+    virtual const char* what() const throw () {
+        return m_message.c_str();
+    }
+
+private:
+    const std::string m_message;
+};
+
 class Vina {
 public:
 	// Constructor
 	Vina(const std::string &sf_name="vina", int cpu=0, int seed=0, int verbosity=1, bool no_refine=false, std::function<void(double)>* progress_callback = NULL) {
 		m_verbosity = verbosity;
 		m_receptor_initialized = false;
 		m_ligand_initialized = false;
@@ -122,14 +135,15 @@
 	std::vector<double> grid_dimensions_from_ligand(double buffer_size=4);
 	void compute_vina_maps(double center_x, double center_y, double center_z,
 								  double size_x, double size_y, double size_z,
 								  double granularity=0.5, bool force_even_voxels=false);
 	void load_maps(std::string maps);
 	void randomize(const int max_steps=10000);
 	std::vector<double> score();
+	std::vector<double> score(double intramolecular_energy);
 	std::vector<double> optimize(const int max_steps=0);
 	void global_search(const int exhaustiveness=8, const int n_poses=20, const double min_rmsd=1.0, const int max_evals=0);
 	std::string get_poses(int how_many=9, double energy_range=3.0);
 	std::vector< std::vector<double> > get_poses_coordinates(int how_many=9, double energy_range=3.0);
 	std::vector< std::vector<double> > get_poses_energies(int how_many=9, double energy_range=3.0);
 	void write_pose(const std::string &output_name, const std::string &remark = std::string());
 	void write_poses(const std::string &output_name, int how_many=9, double energy_range=3.0);
@@ -164,13 +178,12 @@
 	bool m_no_refine;
 	std::function<void(double)>* m_progress_callback;
 
 	std::string vina_remarks(output_type& pose, fl lb, fl ub);
 	output_container remove_redundant(const output_container& in, fl min_rmsd);
 
 	void set_forcefield();
-	std::vector<double> score(double intramolecular_energy);
 	std::vector<double> optimize(output_type& out, const int max_steps=0);
 	int generate_seed(const int seed=0);
 };
 
 #endif
```

### Comparing `vina-1.2.3/src/main/main.cpp` & `vina-1.2.4/src/main/main.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -17,21 +17,24 @@
    Author: Dr. Oleg Trott <ot14@columbia.edu>, 
 		   The Olson Lab,
 		   The Scripps Research Institute
 
 */
 
 #include <iostream>
+#include <set>
 #include <string>
 #include <vector> // ligand paths
 #include <exception>
+#include "parse_error.h"
 #include <boost/program_options.hpp>
 #include "vina.h"
 #include "utils.h"
 #include "scoring_function.h"
+#include <unordered_map>
 
 struct usage_error : public std::runtime_error {
 	usage_error(const std::string& message) : std::runtime_error(message) {}
 };
 
 struct options_occurrence {
 	bool some;
@@ -128,14 +131,15 @@
 		int max_evals = 0;
 		int verbosity = 1;
 		int num_modes = 9;
 		double min_rmsd = 1.0;
 		double energy_range = 3.0;
 		double grid_spacing = 0.375;
 		double buffer_size = 4;
+		double unbound_energy = NAN;
 
 		// autodock4.2 weights
 		double weight_ad4_vdw   = 0.1662;
 		double weight_ad4_hb    = 0.1209;
 		double weight_ad4_elec  = 0.1406;
 		double weight_ad4_dsolv = 0.1322;
 		double weight_ad4_rot   = 0.2983;
@@ -197,14 +201,15 @@
 			("dir", value<std::string>(&out_dir), "output directory for batch mode")
 			("write_maps", value<std::string>(&out_maps), "output filename (directory + prefix name) for maps. Option --force_even_voxels may be needed to comply with .map format")
 		;
 		options_description advanced("Advanced options (see the manual)");
 		advanced.add_options()
 			("score_only",     bool_switch(&score_only),     "score only - search space can be omitted")
 			("local_only",     bool_switch(&local_only),     "do local search only")
+			("unbound_energy", value<double>(&unbound_energy)->default_value(unbound_energy), "Explicitly set the Unbound System's Energy for --score_only jobs")
 			("no_refine", bool_switch(&no_refine),  "when --receptor is provided, do not use explicit receptor atoms (instead of precalculated grids) for: (1) local optimization and scoring after docking, (2) --local_only jobs, and (3) --score_only jobs")
 			("force_even_voxels", bool_switch(&force_even_voxels),  "calculated grid maps will have an even number of voxels (intervals) in each dimension (odd number of grid points)")
 			("randomize_only", bool_switch(&randomize_only), "randomize input, attempting to avoid clashes")
 
 			("weight_gauss1", value<double>(&weight_gauss1)->default_value(weight_gauss1),                "gauss_1 weight")
 			("weight_gauss2", value<double>(&weight_gauss2)->default_value(weight_gauss2),                "gauss_2 weight")
 			("weight_repulsion", value<double>(&weight_repulsion)->default_value(weight_repulsion),       "repulsion weight")
@@ -431,59 +436,109 @@
 			}
 
 			if (randomize_only) {
 				v.randomize();
 				v.write_pose(out_name);
 			} else if (score_only) {
 				std::vector<double> energies;
-				energies = v.score();
+				if (std::isnan(unbound_energy)) {
+					energies = v.score();
+				} else {
+					energies = v.score(unbound_energy);
+				}
 				v.show_score(energies);
 			} else if (local_only) {
 				std::vector<double> energies;
 				energies = v.optimize();
 				v.write_pose(out_name);
 				v.show_score(energies);
 			} else {
 				v.global_search(exhaustiveness, num_modes, min_rmsd, max_evals);
 				v.write_poses(out_name, num_modes, energy_range);
 			}
 		} else if (vm.count("batch")) {
-			if (sf_name.compare("vina") == 0) {
+			if (sf_name.compare("vina") == 0 || sf_name.compare("vinardo") == 0) {
 				if (vm.count("maps")) {
 					v.load_maps(maps);
 				} else {
 					// Will compute maps for all Vina atom types
 					v.compute_vina_maps(center_x, center_y, center_z, size_x, size_y, size_z, grid_spacing);
 
 					if (vm.count("write_maps"))
 						v.write_maps(out_maps);
 				}
 			}
 
+			std::set<std::string> repeated_names;
+			std::set<std::string> raw_names;
+			std::string name;
 			VINA_RANGE(i, 0, batch_ligand_names.size()) {
-				v.set_ligand_from_file(batch_ligand_names[i]);
+				name = get_filename(batch_ligand_names[i]);
+				if (raw_names.count(name)) {
+					repeated_names.insert(name);
+				}
+				raw_names.insert(name);
+			}
+			std::unordered_map<std::string, int> instance_counter;
 
-				out_name = default_output(get_filename(batch_ligand_names[i]), out_dir);
+			std::size_t failed_ligand_parsing = 0;
+			VINA_RANGE(i, 0, batch_ligand_names.size()) {
+				name = get_filename(batch_ligand_names[i]);
+				if (repeated_names.count(name)) {
+					if (instance_counter.count(name)) {
+						instance_counter[name] += 1;
+					} else {
+						instance_counter[name] = 1;
+					}
+					out_name = default_output(name, out_dir, instance_counter[name]);
+				} else {
+					out_name = default_output(name, out_dir);
+				}
+
+				try {
+					v.set_ligand_from_file(batch_ligand_names[i]);
+				}
+				catch(pdbqt_parse_error& e) {
+					std::cerr << e.what();
+					std::cout << "Failed parsing " << batch_ligand_names[i] << ". Skipping it.\n";
+					failed_ligand_parsing++;
+					continue;
+				}
 
 				if (randomize_only) {
 					v.randomize();
 					v.write_pose(out_name);
 				} else if (score_only) {
-					v.score();
+					if (std::isnan(unbound_energy)) {
+						v.score();
+					} else {
+						v.score(unbound_energy);
+					}
 				} else if (local_only) {
 					v.optimize();
 					v.write_pose(out_name);
 				} else {
 					v.global_search(exhaustiveness, num_modes, min_rmsd, max_evals);
 					v.write_poses(out_name, num_modes, energy_range);
 				}
 			}
+			if (repeated_names.size()) {
+				std::cout << "Found " << repeated_names.size() << " repeated filenames in the input batch.\n";
+				std::cout << "The corresponding output filenames are suffixed with _instance<n>_out.pdbqt\n";
+			}
+			if (failed_ligand_parsing) {
+				std::cout << "Failed to parse " << failed_ligand_parsing << " ligands.\n";
+			}
 		}
 	}
 
+	catch(pdbqt_parse_error& e) {
+		std::cerr << e.what();
+		return 1;
+	}
 	catch(file_error& e) {
 		std::cerr << "\n\nError: could not open \"" << e.name.string() << "\" for " << (e.in ? "reading" : "writing") << ".\n";
 		return 1;
 	}
 	catch(boost::filesystem::filesystem_error& e) {
 		std::cerr << "\n\nFile system error: " << e.what() << '\n';
 		return 1;
```

### Comparing `vina-1.2.3/src/split/split.cpp` & `vina-1.2.4/src/split/split.cpp`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/vina/autodock_vina.i` & `vina-1.2.4/vina/autodock_vina.i`

 * *Files 26% similar despite different names*

```diff
@@ -60,16 +60,28 @@
 #include "quaternion.h"
 #include "random.h"
 #include "scoring_function.h"
 #include "szv_grid.h"
 #include "tree.h"
 #include "triangular_matrix_index.h"
 #include "utils.h"
+#include "vina.h"
 %}
 
+%include "exception.i"
+%exception {
+    try {
+        $action
+    } catch (const pdbqt_parse_error& e) {
+        SWIG_exception(SWIG_TypeError, e.what());
+    } catch (const vina_runtime_error& e) {
+        SWIG_exception(SWIG_RuntimeError, e.what());
+    }
+}
+
 // Set and reset dlopenflags so that plugin loading works fine for "import _openbabel"
 %pythonbegin %{
 import sys
 if sys.platform.find("linux") != -1:
     dlflags = sys.getdlopenflags()
     import ctypes
     sys.setdlopenflags(dlflags | ctypes.RTLD_GLOBAL)
```

### Comparing `vina-1.2.3/vina/utils.py` & `vina-1.2.4/vina/utils.py`

 * *Files identical despite different names*

### Comparing `vina-1.2.3/vina/vina.py` & `vina-1.2.4/vina/vina.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,15 +253,15 @@
         a, b, c = box_size
 
         self._vina.compute_vina_maps(x, y, z, a, b, c, spacing, force_even_voxels)
 
         self._center = center
         self._box_size = box_size
         self._spacing = spacing
-        self._voxels = np.ceil(np.array(box_size) / self._spacing).astype(np.int)
+        self._voxels = np.ceil(np.array(box_size) / self._spacing).astype(int)
 
         # Necessary step to know if we can write maps or not later
         if force_even_voxels:
             self._voxels[0] += int(self._voxels[0] % 2 == 1)
             self._voxels[1] += int(self._voxels[1] % 2 == 1)
             self._voxels[2] += int(self._voxels[2] % 2 == 1)
 
@@ -391,34 +391,45 @@
         if n_poses <= 0:
             raise ValueError('Error: number of poses written must be greater than zero.')
         elif energy_range <= 0:
             raise ValueError('Error: energy range must be greater than zero.')
 
         return np.around(self._vina.get_poses_energies(n_poses, energy_range), decimals=3)
 
-    def randomize(self):
-        """Randomize the input ligand conformation."""
-        self._vina.randomize()
+    def randomize(self, max_steps=10000):
+        """Randomize the input ligand conformation.
+
+        Args:
+            max_steps (int): Number of poses to generate for selection of the best one.
+
+        """
+        self._vina.randomize(max_steps)
     
-    def score(self):
+    def score(self, unbound_energy=None):
         """Score current pose.
 
+        Args:
+            unbound_energy (float): Optionally pass the unbound systems energy of the ligand.
+
         Returns:
             nadarray: Array of energies from current pose.
 
             Vina/Vinardo FF:
                 columns=[total, lig_inter, flex_inter, other_inter, flex_intra, lig_intra, torsions, lig_intra best pose]
             
             AutoDock FF:
                 columns=[total, lig_inter, flex_inter, other_inter, flex_intra, lig_intra, torsions, -lig_intra]
 
         """
         # It does not make sense to report energies with a precision higher than 3
         # since the coordinates precision is 3.
-        energies = np.around(self._vina.score(), decimals=3)
+        if unbound_energy is None:
+            energies = np.around(self._vina.score(), decimals=3)
+        else:
+            energies = np.around(self._vina.score(unbound_energy), decimals=3)
         return energies
 
     def optimize(self, max_steps=0):
         """Quick local BFGS energy optimization.
 
         Args:
             max_steps (int): Maximum number of local minimization steps (default: 0). When max_steps is equal to 0,
```

