# Comparing `tmp/teapy-0.1.2.tar.gz` & `tmp/teapy-0.1.3.tar.gz`

## Comparing `teapy-0.1.2.tar` & `teapy-0.1.3.tar`

### file list

```diff
@@ -1,81 +1,82 @@
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 teapy-0.1.2/Cargo.toml
--rw-r--r--   0     1001      123      891 2023-02-04 11:51:34.000000 teapy-0.1.2/.github/workflows/build.yaml
--rw-r--r--   0     1001      123     1097 2023-02-04 11:51:34.000000 teapy-0.1.2/.github/workflows/coverage.yaml
--rw-r--r--   0     1001      123     3361 2023-02-04 11:51:34.000000 teapy-0.1.2/.github/workflows/release_python.yaml
--rw-r--r--   0     1001      123     1272 2023-02-04 11:51:34.000000 teapy-0.1.2/.github/workflows/test_python.yaml
--rw-r--r--   0     1001      123       99 2023-02-04 11:51:34.000000 teapy-0.1.2/.gitignore
--rw-r--r--   0     1001      123     1049 2023-02-04 11:51:34.000000 teapy-0.1.2/LICENSE
--rw-r--r--   0     1001      123     1272 2023-02-04 11:51:34.000000 teapy-0.1.2/Makefile
--rw-r--r--   0     1001      123      441 2023-02-04 11:51:34.000000 teapy-0.1.2/README.md
--rw-r--r--   0     1001      123      195 2023-02-04 11:51:34.000000 teapy-0.1.2/build.requirements.txt
--rw-r--r--   0     1001      123      462 2023-02-04 11:51:34.000000 teapy-0.1.2/pyproject.toml
--rwxr-xr-x   0     1001      123      785 2023-02-04 11:52:06.000000 teapy-0.1.2/run-maturin-action.sh
--rw-r--r--   0     1001      123    13986 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/agg.rs
--rw-r--r--   0     1001      123    31986 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/arr_func.rs
--rw-r--r--   0     1001      123     4672 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/corr.rs
--rw-r--r--   0     1001      123     8363 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/datatype.rs
--rw-r--r--   0     1001      123      548 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/export.rs
--rw-r--r--   0     1001      123     9128 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/groupby.rs
--rw-r--r--   0     1001      123    15524 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/impls/impl_1d_method.rs
--rw-r--r--   0     1001      123     5221 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/impls/impl_linalg.rs
--rw-r--r--   0     1001      123    10397 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/impls/impl_method.rs
--rw-r--r--   0     1001      123     6475 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/impls/impl_numeric.rs
--rw-r--r--   0     1001      123     2897 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/impls/impl_traits.rs
--rw-r--r--   0     1001      123      114 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/impls/mod.rs
--rw-r--r--   0     1001      123    10337 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/iterators.rs
--rw-r--r--   0     1001      123     2886 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/join.rs
--rw-r--r--   0     1001      123     4906 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/lazy/auto_impl_own.rs
--rw-r--r--   0     1001      123     3247 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/lazy/expr_view.rs
--rw-r--r--   0     1001      123    14759 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/lazy/exprs.rs
--rw-r--r--   0     1001      123     1570 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/lazy/impl_cmp.rs
--rw-r--r--   0     1001      123      397 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/lazy/impl_mut.rs
--rw-r--r--   0     1001      123     2800 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/lazy/impl_ops.rs
--rw-r--r--   0     1001      123    22509 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/lazy/impl_own.rs
--rw-r--r--   0     1001      123    10070 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/lazy/impl_view.rs
--rw-r--r--   0     1001      123     8918 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/lazy/linalg.rs
--rw-r--r--   0     1001      123    38550 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/lazy/mod.rs
--rw-r--r--   0     1001      123    11490 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/macros.rs
--rw-r--r--   0     1001      123    21213 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/mod.rs
--rw-r--r--   0     1001      123      451 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/option_datetype.rs
--rw-r--r--   0     1001      123    11108 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/time.rs
--rw-r--r--   0     1001      123     1618 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/util_trait.rs
--rw-r--r--   0     1001      123     3680 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/utils/algos.rs
--rw-r--r--   0     1001      123     1746 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/utils/alloc.rs
--rw-r--r--   0     1001      123      195 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/utils/default_new.rs
--rw-r--r--   0     1001      123      185 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/utils/mod.rs
--rw-r--r--   0     1001      123    13468 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/window/compare.rs
--rw-r--r--   0     1001      123     6390 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/window/corr.rs
--rw-r--r--   0     1001      123    24023 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/window/feature.rs
--rw-r--r--   0     1001      123       75 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/window/mod.rs
--rw-r--r--   0     1001      123     9226 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/window/norm.rs
--rw-r--r--   0     1001      123    12965 2023-02-04 11:51:34.000000 teapy-0.1.2/src/arr/window/reg.rs
--rw-r--r--   0     1001      123     4974 2023-02-04 11:51:34.000000 teapy-0.1.2/src/eager_api.rs
--rw-r--r--   0     1001      123     2769 2023-02-04 11:51:34.000000 teapy-0.1.2/src/eager_macros.rs
--rw-r--r--   0     1001      123     4910 2023-02-04 11:51:34.000000 teapy-0.1.2/src/equity.rs
--rw-r--r--   0     1001      123     7797 2023-02-04 11:51:34.000000 teapy-0.1.2/src/from_py.rs
--rw-r--r--   0     1001      123     1041 2023-02-04 11:51:34.000000 teapy-0.1.2/src/lib.rs
--rw-r--r--   0     1001      123    37219 2023-02-04 11:51:34.000000 teapy-0.1.2/src/pylazy/datadict.rs
--rw-r--r--   0     1001      123      530 2023-02-04 11:51:34.000000 teapy-0.1.2/src/pylazy/export.rs
--rw-r--r--   0     1001      123     2628 2023-02-04 11:51:34.000000 teapy-0.1.2/src/pylazy/groupby.rs
--rw-r--r--   0     1001      123    83705 2023-02-04 11:51:34.000000 teapy-0.1.2/src/pylazy/impl_pyexpr.rs
--rw-r--r--   0     1001      123     1181 2023-02-04 11:51:34.000000 teapy-0.1.2/src/pylazy/mod.rs
--rw-r--r--   0     1001      123    19749 2023-02-04 11:51:34.000000 teapy-0.1.2/src/pylazy/pyexpr.rs
--rw-r--r--   0     1001      123    11374 2023-02-04 11:51:34.000000 teapy-0.1.2/src/pylazy/pyfunc.rs
--rw-r--r--   0     1001      123      454 2023-02-04 11:51:34.000000 teapy-0.1.2/src/pylazy/time.rs
--rw-r--r--   0     1001      123      392 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/__init__.py
--rw-r--r--   0     1001      123     5277 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/array_func.py
--rw-r--r--   0     1001      123     3184 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/converter.py
--rw-r--r--   0     1001      123     4175 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/datadict.py
--rw-r--r--   0     1001      123     6985 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/regression.py
--rw-r--r--   0     1001      123     3161 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/testing.py
--rw-r--r--   0     1001      123     7840 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/tests/test_array_func.py
--rw-r--r--   0     1001      123     3167 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/tests/test_common.py
--rw-r--r--   0     1001      123     2730 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/tests/window/test_compare.py
--rw-r--r--   0     1001      123     1227 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/tests/window/test_corr.py
--rw-r--r--   0     1001      123     4851 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/tests/window/test_feature.py
--rw-r--r--   0     1001      123     1694 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/tests/window/test_norm.py
--rw-r--r--   0     1001      123     2589 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/tests/window/test_reg.py
--rw-r--r--   0     1001      123     3660 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/window_func.py
--rw-r--r--   0     1001      123     5006 2023-02-04 11:51:34.000000 teapy-0.1.2/teapy/wrapper.py
--rw-r--r--   0     1001      123    44634 2023-02-04 11:51:34.000000 teapy-0.1.2/Cargo.lock
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 teapy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 teapy-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      123      891 2023-06-12 04:50:58.000000 teapy-0.1.3/.github/workflows/build.yaml
+-rw-r--r--   0     1001      123     1097 2023-06-12 04:50:58.000000 teapy-0.1.3/.github/workflows/coverage.yaml
+-rw-r--r--   0     1001      123     3240 2023-06-12 04:50:58.000000 teapy-0.1.3/.github/workflows/release_python.yaml
+-rw-r--r--   0     1001      123     1280 2023-06-12 04:50:58.000000 teapy-0.1.3/.github/workflows/test_python.yaml
+-rw-r--r--   0     1001      123      105 2023-06-12 04:50:58.000000 teapy-0.1.3/.gitignore
+-rw-r--r--   0     1001      123     1049 2023-06-12 04:50:58.000000 teapy-0.1.3/LICENSE
+-rw-r--r--   0     1001      123     1272 2023-06-12 04:50:58.000000 teapy-0.1.3/Makefile
+-rw-r--r--   0     1001      123      441 2023-06-12 04:50:58.000000 teapy-0.1.3/README.md
+-rw-r--r--   0     1001      123      195 2023-06-12 04:50:58.000000 teapy-0.1.3/build.requirements.txt
+-rw-r--r--   0     1001      123      462 2023-06-12 04:50:58.000000 teapy-0.1.3/pyproject.toml
+-rwxr-xr-x   0     1001      123      850 2023-06-12 04:51:27.000000 teapy-0.1.3/run-maturin-action.sh
+-rw-r--r--   0     1001      123    13986 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/agg.rs
+-rw-r--r--   0     1001      123    31986 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/arr_func.rs
+-rw-r--r--   0     1001      123     4672 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/corr.rs
+-rw-r--r--   0     1001      123     8363 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/datatype.rs
+-rw-r--r--   0     1001      123      548 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/export.rs
+-rw-r--r--   0     1001      123     9128 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/groupby.rs
+-rw-r--r--   0     1001      123    15524 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/impls/impl_1d_method.rs
+-rw-r--r--   0     1001      123     5221 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/impls/impl_linalg.rs
+-rw-r--r--   0     1001      123    10397 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/impls/impl_method.rs
+-rw-r--r--   0     1001      123     6606 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/impls/impl_numeric.rs
+-rw-r--r--   0     1001      123     3399 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/impls/impl_traits.rs
+-rw-r--r--   0     1001      123      114 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/impls/mod.rs
+-rw-r--r--   0     1001      123    10337 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/iterators.rs
+-rw-r--r--   0     1001      123     2886 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/join.rs
+-rw-r--r--   0     1001      123     4835 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/auto_impl_own.rs
+-rw-r--r--   0     1001      123     3247 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/expr_view.rs
+-rw-r--r--   0     1001      123    14759 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/exprs.rs
+-rw-r--r--   0     1001      123     1570 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/impl_cmp.rs
+-rw-r--r--   0     1001      123      397 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/impl_mut.rs
+-rw-r--r--   0     1001      123     2800 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/impl_ops.rs
+-rw-r--r--   0     1001      123    25019 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/impl_own.rs
+-rw-r--r--   0     1001      123    10697 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/impl_view.rs
+-rw-r--r--   0     1001      123     8918 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/linalg.rs
+-rw-r--r--   0     1001      123    41157 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/mod.rs
+-rw-r--r--   0     1001      123    40512 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/mod_test.rs
+-rw-r--r--   0     1001      123    11490 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/macros.rs
+-rw-r--r--   0     1001      123    21693 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/mod.rs
+-rw-r--r--   0     1001      123      451 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/option_datetype.rs
+-rw-r--r--   0     1001      123    11108 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/time.rs
+-rw-r--r--   0     1001      123     1618 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/util_trait.rs
+-rw-r--r--   0     1001      123     3680 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/utils/algos.rs
+-rw-r--r--   0     1001      123     1746 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/utils/alloc.rs
+-rw-r--r--   0     1001      123      195 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/utils/default_new.rs
+-rw-r--r--   0     1001      123      185 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/utils/mod.rs
+-rw-r--r--   0     1001      123    13468 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/window/compare.rs
+-rw-r--r--   0     1001      123     6390 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/window/corr.rs
+-rw-r--r--   0     1001      123    24023 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/window/feature.rs
+-rw-r--r--   0     1001      123       75 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/window/mod.rs
+-rw-r--r--   0     1001      123     9226 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/window/norm.rs
+-rw-r--r--   0     1001      123    12965 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/window/reg.rs
+-rw-r--r--   0     1001      123     4974 2023-06-12 04:50:58.000000 teapy-0.1.3/src/eager_api.rs
+-rw-r--r--   0     1001      123     2769 2023-06-12 04:50:58.000000 teapy-0.1.3/src/eager_macros.rs
+-rw-r--r--   0     1001      123     9340 2023-06-12 04:50:58.000000 teapy-0.1.3/src/equity.rs
+-rw-r--r--   0     1001      123     8298 2023-06-12 04:50:58.000000 teapy-0.1.3/src/from_py.rs
+-rw-r--r--   0     1001      123     1113 2023-06-12 04:50:58.000000 teapy-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      123    37387 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/datadict.rs
+-rw-r--r--   0     1001      123      530 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/export.rs
+-rw-r--r--   0     1001      123     2628 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/groupby.rs
+-rw-r--r--   0     1001      123    85968 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/impl_pyexpr.rs
+-rw-r--r--   0     1001      123     1200 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/mod.rs
+-rw-r--r--   0     1001      123    19759 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/pyexpr.rs
+-rw-r--r--   0     1001      123    15098 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/pyfunc.rs
+-rw-r--r--   0     1001      123      454 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/time.rs
+-rw-r--r--   0     1001      123      388 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/__init__.py
+-rw-r--r--   0     1001      123     5452 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/array_func.py
+-rw-r--r--   0     1001      123     3184 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/converter.py
+-rw-r--r--   0     1001      123     4264 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/datadict.py
+-rw-r--r--   0     1001      123     6985 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/regression.py
+-rw-r--r--   0     1001      123     3440 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/testing.py
+-rw-r--r--   0     1001      123     9870 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      123     3380 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/test_common.py
+-rw-r--r--   0     1001      123     3211 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      123     1418 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      123     5772 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      123     1995 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      123     3165 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      123     3660 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/window_func.py
+-rw-r--r--   0     1001      123     5751 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/wrapper.py
+-rw-r--r--   0     1001      123    44634 2023-06-12 04:50:58.000000 teapy-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 teapy-0.1.3/PKG-INFO
```

### Comparing `teapy-0.1.2/Cargo.toml` & `teapy-0.1.3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [package]
 name = "teapy"
-version = "0.1.2"
+version = "0.1.3"
 edition = "2021"
 
 [lib]
 name = "teapy"
-crate-type = ["cdylib"]
+crate-type = ["cdylib", "rlib"]
 
 [features]
 default = ["lazy", "eager_api", "blas"]
 lazy = ["window_func"]
 eager_api = ["window_func"]
 window_func = []
 blas = ["ndarray-linalg", "ndarray/blas", "lazy", "statrs", "lapack-sys"]
```

### Comparing `teapy-0.1.2/.github/workflows/build.yaml` & `teapy-0.1.3/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/.github/workflows/coverage.yaml` & `teapy-0.1.3/.github/workflows/coverage.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/.github/workflows/release_python.yaml` & `teapy-0.1.3/.github/workflows/release_python.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 on:
   push:
-      branches:
-        - master
       tags:
         - teapy*
 
 defaults:
   run:
     shell: bash
 
@@ -57,15 +55,15 @@
         with:
           python-version: '3.8'
 
       - name: Publish wheel
         uses: messense/maturin-action@v1
         env:
           MATURIN_PASSWORD: ${{ secrets.PYPI_SECRET }}
-          RUSTFLAGS: -C target-feature=+fxsr,+sse,+sse2,+sse3,+sse4.1,+sse4.2
+          RUSTFLAGS: -C target-feature=+fxsr,+sse,+sse2,+sse3,+sse4.1,+sse4.2,+popcnt,+avx,+fma
           CXXFLAGS: -stdlib=libc++
         with:
           rust-toolchain: nightly-2023-01-19
           maturin-version: '0.14.10'
           command: publish
           args: --no-sdist --skip-existing -o wheels -i python -u teamon
 
@@ -74,33 +72,29 @@
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.8'
 
 
-      - name: Set up Rust
-        uses: dtolnay/rust-toolchain@master
-        with:
-          toolchain: nightly-2023-01-19
-
       - name: Set up Rust targets
         run: rustup target add aarch64-apple-darwin
 
       - name: Publish wheel
         uses: messense/maturin-action@v1
         env:
           MATURIN_PASSWORD: ${{ secrets.PYPI_SECRET }}
         with:
           maturin-version: '0.14.10'
           command: publish
-          args: --target aarch64-apple-darwin --no-sdist -o wheels -i python -u teamon
+          args: --target aarch64-apple-darwin --skip-existing --no-sdist -o wheels -i python -u teamon
 
 
   # # the dependency of ndarry-linalg crate can not be build on manylinux-arrch64 currently
+  
   # # Needed for Docker on Apple M1
   # manylinux-aarch64:
   #   runs-on: ubuntu-latest
   #   steps:
   #     - uses: actions/checkout@v3
   #     - uses: actions/setup-python@v4
   #       with:
```

### Comparing `teapy-0.1.2/.github/workflows/test_python.yaml` & `teapy-0.1.3/.github/workflows/test_python.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -16,21 +16,21 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [ "3.8" ]
     steps:
       - uses: actions/checkout@v3
       - name: Install Rust
-        uses: actions-rs/toolchain@v1
+        uses: dtolnay/rust-toolchain@master
         with:
           toolchain: nightly-2023-01-19
-          override: true
+          # override: true
           components: rustfmt, clippy
       - name: Set up Python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r build.requirements.txt
       - name: Run formatting checks
```

### Comparing `teapy-0.1.2/LICENSE` & `teapy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/Makefile` & `teapy-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/run-maturin-action.sh` & `teapy-0.1.3/run-maturin-action.sh`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 set -e
 echo "::group::Install Rust"
 which rustup > /dev/null || curl --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --profile minimal --default-toolchain nightly-2023-01-19
 export PATH="$HOME/.cargo/bin:$PATH"
 rustup override set nightly-2023-01-19
 rustup component add llvm-tools-preview || true
 echo "::endgroup::"
-export PATH="$PATH:/opt/python/cp36-cp36m/bin:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin"
+export PATH="$PATH:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin:/opt/python/cp310-cp310/bin:/opt/python/cp311-cp311/bin"
 echo "::group::Install maturin"
 curl -L https://github.com/PyO3/maturin/releases/download/v0.14.10/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
 maturin --version || true
 which patchelf > /dev/null || python3 -m pip install patchelf
+python3 -m pip install cffi || true
 echo "::endgroup::"
 maturin publish --skip-existing -o wheels -u teamon
```

### Comparing `teapy-0.1.2/src/arr/agg.rs` & `teapy-0.1.3/src/arr/agg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/arr_func.rs` & `teapy-0.1.3/src/arr/arr_func.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/corr.rs` & `teapy-0.1.3/src/arr/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/datatype.rs` & `teapy-0.1.3/src/arr/datatype.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/export.rs` & `teapy-0.1.3/src/arr/export.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/groupby.rs` & `teapy-0.1.3/src/arr/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/impls/impl_1d_method.rs` & `teapy-0.1.3/src/arr/impls/impl_1d_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/impls/impl_linalg.rs` & `teapy-0.1.3/src/arr/impls/impl_linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/impls/impl_method.rs` & `teapy-0.1.3/src/arr/impls/impl_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/impls/impl_numeric.rs` & `teapy-0.1.3/src/arr/impls/impl_numeric.rs`

 * *Files 3% similar despite different names*

```diff
@@ -155,14 +155,21 @@
     pub fn abs(&self, _par: bool) -> Arr<T, D>
     where
         T: Signed + Send + Sync + Clone,
     {
         self.map(|v| abs(v.clone()))
     }
 
+    pub fn sign(&self, _par: bool) -> Arr<T, D>
+    where
+        T: Signed + Clone,
+    {
+        self.map(|v| v.signum())
+    }
+
     pub fn powi<S2, D2>(
         &self,
         rhs: &ArrBase<S2, D2>,
         par: bool,
     ) -> Arr<T, <D as DimMax<D2>>::Output>
     where
         D2: Dimension,
```

### Comparing `teapy-0.1.2/src/arr/iterators.rs` & `teapy-0.1.3/src/arr/iterators.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/join.rs` & `teapy-0.1.3/src/arr/join.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/lazy/auto_impl_own.rs` & `teapy-0.1.3/src/arr/lazy/auto_impl_own.rs`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
         }
     };
     (in1, [$($func: ident -> $otype:ident),* $(,)?], $other: tt) => {
         $(impl_view_lazy!(in1, $func -> $otype, $other);)*
     };
     (in1-inplace, $func:ident, $func_inplace: ident -> $otype:ident, ($($p:ident: $p_ty:ty),* $(,)?)) => {
         pub fn $func (self $(, $p: $p_ty)*) -> Expr<'a, $otype> {
-            // self.chain_view_f(move |arr| arr.$func($($p),*).into())
             self.chain_arr_f(move |arb_arr| {
                 use ArbArray::*;
                 match arb_arr {
                     View(arr) => arr.$func($($p),*).into(),
                     ViewMut(mut arr) => {
                         arr.$func_inplace($($p),*);
                         ViewMut(arr)
```

### Comparing `teapy-0.1.2/src/arr/lazy/expr_view.rs` & `teapy-0.1.3/src/arr/lazy/expr_view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/lazy/exprs.rs` & `teapy-0.1.3/src/arr/lazy/exprs.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/lazy/impl_cmp.rs` & `teapy-0.1.3/src/arr/lazy/impl_cmp.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/lazy/impl_ops.rs` & `teapy-0.1.3/src/arr/lazy/impl_ops.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/lazy/impl_own.rs` & `teapy-0.1.3/src/arr/lazy/impl_own.rs`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,35 @@
 use num::traits::{real::Real, AsPrimitive};
 use num::{Float, One, Signed, Zero};
 use pyo3::Python;
 use rayon::prelude::*;
 use statrs::distribution::ContinuousCDF;
 use std::mem;
 
+pub enum DropNaMethod {
+    Any,
+    All,
+}
+
 impl<'a, T> Expr<'a, T>
 where
     T: ExprElement + 'a,
 {
+    pub fn hint_arr_type(self) -> Expr<'a, &'a str> {
+        self.chain_arr_f(move |arb_arr| {
+            use ArbArray::*;
+            let out: Vec<&'a str> = match arb_arr {
+                View(_) => vec!["View"],
+                ViewMut(_) => vec!["ViewMut"],
+                Owned(_) => vec!["Owned"],
+            };
+            ArbArray::Owned(Arr1::from_vec(out).to_dimd().unwrap())
+        })
+    }
+
     pub fn full(shape: Expr<'a, usize>, value: Expr<'a, T>) -> Expr<'a, T>
     where
         T: Clone,
     {
         shape.chain_view_f(|sh| {
             let ndim = sh.ndim();
             let value = value.eval();
@@ -364,14 +381,21 @@
     pub fn abs(self, par: bool) -> Self
     where
         T: Signed + Clone,
     {
         self.chain_view_f(move |arr| arr.abs(par).into())
     }
 
+    pub fn sign(self, par: bool) -> Self
+    where
+        T: Signed + Clone,
+    {
+        self.chain_view_f(move |arr| arr.sign(par).into())
+    }
+
     pub fn powi(self, other: Expr<'a, i32>, par: bool) -> Self
     where
         T: Real,
     {
         self.chain_view_f(move |arr| arr.powi(&other.eval().view_arr(), par).into())
     }
 
@@ -437,14 +461,52 @@
                     .into_scalar(),
                 par,
             )
             .into()
         })
     }
 
+    pub fn dropna<'b: 'a>(self, axis: Expr<'a, usize>, how: DropNaMethod, par: bool) -> Self
+    where
+        T: Clone + Number,
+    {
+        self.chain_view_f(move |arr| {
+            let ndim = arr.ndim();
+            let axis = *axis
+                .eval()
+                .view_arr()
+                .to_dim0()
+                .expect("axis should be dim 0")
+                .into_scalar();
+            match ndim {
+                1 => arr
+                    .to_dim1()
+                    .unwrap()
+                    .remove_nan_1d()
+                    .to_dimd()
+                    .unwrap()
+                    .into(),
+                2 => {
+                    let arr = arr.to_dim2().unwrap();
+                    let mask = match (axis, how) {
+                        (0, DropNaMethod::Any) => arr.not_nan().all(1, par),
+                        (0, DropNaMethod::All) => arr.not_nan().any(1, par),
+                        (1, DropNaMethod::Any) => arr.not_nan().all(0, par),
+                        (1, DropNaMethod::All) => arr.not_nan().any(0, par),
+                        _ => panic!("axis should be 0 or 1 and how should be any or all"),
+                    };
+                    arr.filter(&mask, axis, par).to_dimd().unwrap().into()
+                }
+                dim => unimplemented!(
+                    "dropna only support 1d and 2d array currently, but the array is dim {dim}"
+                ),
+            }
+        })
+    }
+
     /// select on a given axis by a slice expression
     pub fn select_on_axis_by_expr(self, slc: Expr<'a, usize>, axis: Expr<'a, usize>) -> Self
     where
         T: Clone,
     {
         self.chain_view_f(move |arr| {
             let slc = slc.no_dim0().eval();
@@ -622,14 +684,27 @@
             };
             ndarray::stack(Axis(axis), &arrays)
                 .expect("Shape error when concatenate")
                 .wrap()
                 .into()
         })
     }
+
+    // pub fn apply_on_vec_arr<F>(self, func: F, axis: usize) -> Expr<'a, T>
+    // {
+    //     self.chain_f(|input| {
+    //         if let ExprOut::ArrVec(arr_vec) = input {
+    //             let view_vec = arr_vec.iter().map(|arr| arr.view()).collect_trusted();
+    //             use ndarray::Zip;
+    //             let shape =
+    //             let out = Vec::with_capacity(arr_vec.len());
+    //         }
+
+    //     })
+    // }
 }
 
 impl<'a> Expr<'a, bool> {
     pub fn any(self, axis: usize, par: bool) -> Self {
         self.chain_view_f(move |arr| arr.any(axis, par).into())
     }
```

### Comparing `teapy-0.1.2/src/arr/lazy/impl_view.rs` & `teapy-0.1.3/src/arr/lazy/impl_view.rs`

 * *Files 7% similar despite different names*

```diff
@@ -13,40 +13,56 @@
 where
     T: ExprElement + 'a,
 {
     /// # Safety
     ///
     /// the data for the array view should exist
     pub unsafe fn reshape(self, shape: Expr<'a, usize>) -> Self {
-        self.chain_view_f(|arr| {
+        self.chain_view_out_f(|arr| {
             let shape = shape.eval();
             let sh = shape.view_arr();
             let ndim = sh.ndim();
             if ndim == 0 {
                 let shape = sh.to_dim0().unwrap().into_scalar();
-                let out: ArbArray<'_, T> = arr
+                // let out: ArbArray<'_, T> = arr
+                //     .0
+                //     .into_shape(*shape)
+                //     .expect("Shape Error")
+                //     .wrap()
+                //     .to_dimd()
+                //     .unwrap()
+                //     .into();
+                // // safe because the view exist in lifetime 'a
+                // mem::transmute(out)
+                let out = arr
                     .0
                     .into_shape(*shape)
                     .expect("Shape Error")
                     .wrap()
                     .to_dimd()
-                    .unwrap()
-                    .into();
+                    .unwrap();
                 // safe because the view exist in lifetime 'a
                 mem::transmute(out)
             } else if ndim == 1 {
                 let shape = sh.to_dim1().unwrap();
-                let out: ArbArray<'_, T> = arr
+                // let out: ArbArray<'_, T> = arr
+                //     .0
+                //     .into_shape(shape.to_slice().unwrap())
+                //     .expect("Shape Error")
+                //     .wrap()
+                //     .to_dimd()
+                //     .unwrap()
+                //     .into();
+                let out = arr
                     .0
                     .into_shape(shape.to_slice().unwrap())
                     .expect("Shape Error")
                     .wrap()
                     .to_dimd()
-                    .unwrap()
-                    .into();
+                    .unwrap();
                 mem::transmute(out)
             } else {
                 panic!("the dim of shape should not be greater than 1")
             }
         })
     }
```

### Comparing `teapy-0.1.2/src/arr/lazy/linalg.rs` & `teapy-0.1.3/src/arr/lazy/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/lazy/mod.rs` & `teapy-0.1.3/src/arr/lazy/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 mod impl_ops;
 mod impl_own;
 mod impl_view;
 #[cfg(feature = "blas")]
 mod linalg;
 
 pub use exprs::Exprs;
+pub use impl_own::DropNaMethod;
 #[cfg(feature = "blas")]
 pub use linalg::OlsResult;
 use pyo3::{Python, ToPyObject};
 
 use super::{
     ArbArray, Arr1, ArrD, ArrOk, ArrViewD, ArrViewMutD, CollectTrustedToVec, DataType, DateTime,
     DefaultNew, EmptyNew, GetDataType, TimeDelta, TimeUnit,
@@ -88,14 +89,28 @@
     }
 
     /// Change the name of the Expression immediately
     pub fn rename(&mut self, name: String) {
         unsafe { self.e.lock().unwrap().get_mut::<T>().rename(name) }
     }
 
+    pub fn get_base_type(&self) -> &'static str {
+        unsafe { self.e.lock().unwrap().get::<T>().get_base_type() }
+    }
+
+    pub fn get_base_strong_count(&self) -> Result<usize, &'static str> {
+        unsafe {
+            self.e
+                .lock()
+                .unwrap()
+                .get::<T>()
+                .get_base_expr_strong_count()
+        }
+    }
+
     #[inline(always)]
     pub fn strong_count(&self) -> usize {
         Arc::strong_count(&self.e)
     }
 
     #[inline(always)]
     pub fn weak_count(&self) -> usize {
@@ -122,14 +137,15 @@
         unsafe { self.e.lock().unwrap().get::<T>().get_owned() }
     }
 
     pub fn split_vec_base(self, len: usize) -> Vec<Self>
     where
         T: Clone,
     {
+        // todo: improve performance
         let mut out = Vec::with_capacity(len);
         for i in 0..len {
             out.push(
                 self.clone()
                     .chain_f(move |base| base.into_arr_vec().remove(i).into()),
             );
         }
@@ -169,14 +185,26 @@
         F: FnOnce(ArrViewD<'_, T>) -> ArbArray<'a, T2> + Send + Sync + 'a,
         T2: ExprElement,
     {
         self.downcast().chain_view_f(f).into()
     }
 
     /// chain a new function to current function chain, the function accept
+    /// an array of type ArrViewD<'a, T> and return ArrViewD<'a, T2>
+    #[inline]
+    pub fn chain_view_out_f<F, T2>(self, f: F) -> Expr<'a, T2>
+    where
+        T2: 'a,
+        F: FnOnce(ArrViewD<'_, T>) -> ArrViewD<'a, T2> + Send + Sync + 'a,
+        T2: ExprElement,
+    {
+        self.downcast().chain_view_out_f(f).into()
+    }
+
+    /// chain a new function to current function chain, the function accept
     /// an array of type `ArrViewMutD<'a, T>` and modify inplace
     #[inline]
     pub fn chain_view_mut_f<F>(self, f: F) -> Expr<'a, T>
     where
         T: Clone,
         F: FnOnce(&mut ArrViewMutD<'_, T>) + Send + Sync + 'a,
     {
@@ -204,34 +232,34 @@
     #[inline]
     pub fn eval_inplace(&mut self) {
         unsafe { self.e.lock().unwrap().get_mut::<T>().eval_inplace() }
     }
 
     /// create a view of the output array
     #[inline]
-    pub(crate) fn try_view_arr(&self) -> Result<ArrViewD<'_, T>, &'static str> {
+    pub fn try_view_arr(&self) -> Result<ArrViewD<'_, T>, &'static str> {
         self.try_view()?.try_into_arr()
     }
 
     /// create a view of the output array
     #[inline]
-    pub(crate) fn view_arr(&self) -> ArrViewD<'_, T> {
+    pub fn view_arr(&self) -> ArrViewD<'_, T> {
         self.try_view_arr().expect("can not view as arr")
     }
 
     #[inline]
     pub fn view(&self) -> ExprOutView<'_, T> {
         self.try_view().unwrap()
     }
 
     #[inline]
     pub fn try_view(&self) -> Result<ExprOutView<'_, T>, &'static str> {
         let e = self.e.lock().unwrap();
         let view = unsafe { e.get::<T>().try_view()? };
-        unsafe { mem::transmute(view) }
+        Ok(unsafe { mem::transmute(view) })
     }
 
     /// execute the expression and copy the output
     #[inline]
     pub fn value(&mut self) -> ArrD<T>
     where
         T: Clone,
@@ -519,37 +547,34 @@
                                 let mut exprs_lock = exprs.lock().unwrap();
                                 if exprs_lock.step() != 0 {
                                     exprs_lock.eval_inplace();
                                 }
                                 // we should not modify the base expression
                                 // safety: the data of the base expression must exist
                                 if ref_count > 1 {
+                                    // panic!("ref_count = {} > 1", ref_count);
                                     let out: ExprOut<'_, T> = exprs_lock.view::<T>().unwrap().into();
                                     return mem::transmute(out)
                                 } else {
                                     mem::drop(exprs_lock);
-                                    Arc::try_unwrap(exprs)
-                                    .expect("Ref count is not 1")
-                                    .into_inner().expect("Poison exprs")
-                                    .downcast::<T>()
-                                    .into_out()
+                                    Expr {e:exprs, _type: PhantomData}.into_out()
                                 }
                             },
                             ExprBase::ExprVec(mut expr_vec) => {
                                 expr_vec.iter_mut().for_each(|e| {
                                     let mut expr_lock = e.lock().unwrap();
                                     if expr_lock.step() != 0 {
                                         expr_lock.eval_inplace();
                                     }
                                 });
                                 let expr_vec = expr_vec.into_iter().map(|e| {
                                     Expr {e, _type: PhantomData}
                                 }).collect_trusted();
                                 ExprOut::ExprVec(expr_vec)
-                            }
+                            },
                             #[cfg(feature="blas")] ExprBase::OlsRes(res) => res.into()
                         }
                     })
                 },)*
                 _ => unimplemented!("Not support dtype of function chain")
             }
         }
@@ -631,34 +656,45 @@
 impl Default for ExprBase<'_> {
     fn default() -> Self {
         ExprBase::Arr(Default::default())
     }
 }
 
 impl<'a, T: ExprElement> ExprInner<'a, T> {
-    #[allow(dead_code)]
-    pub fn new(arr: ExprOut<'a, T>, name: Option<String>) -> Self {
-        match arr {
-            ExprOut::Arr(arr) => Self::new_with_arr(arr, name),
-            #[cfg(feature = "blas")]
-            ExprOut::OlsRes(res) => ExprInner::<T> {
-                base: ExprBase::OlsRes(res),
-                func: EmptyNew::empty_new(),
-                step: 0,
-                owned: None,
-                name,
-                ref_expr: None,
-            },
-            ExprOut::ArrVec(_) => {
-                unimplemented!("Create an expression with a vector of array is not implemented")
-            }
-            ExprOut::ExprVec(expr_vec) => {
-                let expr_vec = expr_vec.into_iter().map(|e| e.e).collect_trusted();
-                Self::new_with_expr_vec(expr_vec, name)
-            }
+    // #[allow(dead_code)]
+    // pub fn new(arr: ExprOut<'a, T>, name: Option<String>) -> Self {
+    //     match arr {
+    //         ExprOut::Arr(arr) => Self::new_with_arr(arr, name),
+    //         #[cfg(feature = "blas")]
+    //         ExprOut::OlsRes(res) => ExprInner::<T> {
+    //             base: ExprBase::OlsRes(res),
+    //             func: EmptyNew::empty_new(),
+    //             step: 0,
+    //             owned: None,
+    //             name,
+    //             ref_expr: None,
+    //         },
+    //         ExprOut::ArrVec(_) => {
+    //             unimplemented!("Create an expression with a vector of array is not implemented")
+    //         }
+    //         ExprOut::ExprVec(expr_vec) => {
+    //             let expr_vec = expr_vec.into_iter().map(|e| e.e).collect_trusted();
+    //             Self::new_with_expr_vec(expr_vec, name)
+    //         }
+    //     }
+    // }
+
+    pub fn new_with_base(arr: ExprBase<'a>, name: Option<String>) -> Self {
+        ExprInner::<T> {
+            base: arr,
+            func: EmptyNew::empty_new(),
+            step: 0,
+            owned: None,
+            name,
+            ref_expr: None,
         }
     }
 
     pub fn new_with_arr(arr: ArbArray<'a, T>, name: Option<String>) -> Self {
         ExprInner::<T> {
             base: ExprBase::Arr(arr.into()),
             func: EmptyNew::empty_new(),
@@ -758,14 +794,34 @@
 
     /// rename inplace
     #[inline(always)]
     pub fn rename(&mut self, name: String) {
         self.name = Some(name)
     }
 
+    pub fn get_base_type(&self) -> &'static str {
+        match &self.base {
+            ExprBase::Expr(_) => "Expr",
+            ExprBase::ExprVec(_) => "ExprVec",
+            ExprBase::Arr(arr) => arr.get_type(),
+            ExprBase::ArrVec(_) => "ArrVec",
+            ExprBase::ArcArr(_) => "ArcArr",
+            #[cfg(feature = "blas")]
+            ExprBase::OlsRes(_) => "OlsRes",
+        }
+    }
+
+    pub fn get_base_expr_strong_count(&self) -> Result<usize, &'static str> {
+        if let ExprBase::Expr(expr) = &self.base {
+            Ok(Arc::strong_count(expr))
+        } else {
+            Err("The base of the expression is not Expr")
+        }
+    }
+
     #[inline(always)]
     pub fn set_base(&mut self, base: ExprBase<'a>) {
         self.base = base;
     }
 
     #[inline(always)]
     pub fn set_base_by_arr(&mut self, base: ArrOk<'a>) {
@@ -803,78 +859,70 @@
         self.owned = Some(owned);
     }
 
     #[inline(always)]
     /// Reset the function chain.
     pub fn reset_func(&mut self) {
         self.set_func(EmptyNew::empty_new());
-        // self.func = EmptyNew::empty_new();
     }
 
     #[inline(always)]
     /// Reset the function chain and the step.
     pub fn reset(&mut self) {
         self.set_step(0);
         self.reset_func();
     }
 
-    /// Execute the expression and get a new Expr with length 0
+    /// Execute the expression and get a new Expr with step 0
     #[inline]
     pub fn eval(mut self) -> Self {
         self.eval_inplace();
         self
     }
 
-    // /// Execute the expression by a new base and get a new Expr with length 0
-    // #[inline]
-    // pub fn eval_by(mut self, base: ExprBase<'a>) -> Self
-    // {
-    //     self.set_base(base);
-    //     self.eval()
-    // }
-
-    // /// Execute the expression inplace by a new base
-    // #[inline]
-    // pub fn eval_inplace_by(&mut self, base: ExprBase<'a>)
-    // {
-    //     self.set_base(base);
-    //     self.eval_inplace();
-    // }
-
     /// Execute the expression inplace
     #[inline]
     pub fn eval_inplace(&mut self) {
         if self.step() != 0 {
-            let out = if let ExprBase::Expr(base_expr) = &self.base {
-                // let base_step = base_expr.lock().unwrap().step();
-                // // if the new step is zero, we shouldn't evaluate if the ExprBase is another expression
-                // // we should keep a reference to the base expression
-                // if self.step == base_step {
-                //     return;
-                // }
-                let base_expr = base_expr.clone();
-                let base = mem::take(&mut self.base);
-                let default_func: FuncChainType<'a, T> = DefaultNew::default_new();
-                let func = mem::replace(&mut self.func, default_func);
-                let out = func(base);
-                self.set_owned(out.is_owned());
-                if !self.get_owned().unwrap() {
-                    // in this case we create a view on an expression,
-                    // so we should add a reference to the base expression
-                    self.ref_expr = Some(vec![base_expr]);
-                }
-                out
-            } else {
-                let base = mem::take(&mut self.base);
-                let default_func: FuncChainType<'a, T> = DefaultNew::default_new();
-                let func = mem::replace(&mut self.func, default_func);
-                let out = func(base);
-                self.set_owned(out.is_owned());
-                out
-            };
+            // we should not execute the expression if the step is zero because we may
+            // create a view on the base expression. we should keep the base expression
+            // as the expression base.
+
+            // let out = if let ExprBase::Expr(base_expr) = &self.base {
+            //     // let base_step = base_expr.lock().unwrap().step();
+            //     // // if the new step is zero, we shouldn't evaluate if the ExprBase is another expression
+            //     // // we should keep a reference to the base expression
+            //     // if self.step == base_step {
+            //     //     return;
+            //     // }
+            //     let base_expr = base_expr.clone();
+            //     let base = mem::take(&mut self.base);
+            //     let default_func: FuncChainType<'a, T> = DefaultNew::default_new();
+            //     let func = mem::replace(&mut self.func, default_func);
+            //     let out = func(base);
+            //     self.set_owned(out.is_owned());
+            //     if !self.get_owned().unwrap() {
+            //         // in this case we create a view on an expression,
+            //         // so we should add a reference to the base expression
+            //         self.ref_expr = Some(vec![base_expr]);
+            //     }
+            //     out
+            // } else {
+            //     let base = mem::take(&mut self.base);
+            //     let default_func: FuncChainType<'a, T> = DefaultNew::default_new();
+            //     let func = mem::replace(&mut self.func, default_func);
+            //     let out = func(base);
+            //     self.set_owned(out.is_owned());
+            //     out
+            // };
+            let base = mem::take(&mut self.base);
+            let default_func: FuncChainType<'a, T> = DefaultNew::default_new();
+            let func = mem::replace(&mut self.func, default_func);
+            let out = func(base);
+            self.set_owned(out.is_owned());
             match out {
                 ExprOut::Arr(arr) => self.set_base_by_arr(arr.into()),
                 ExprOut::ArrVec(arr_vec) => self.set_base_by_arr_vec(
                     arr_vec.into_iter().map(|arr| arr.into()).collect_trusted(),
                 ),
                 ExprOut::ExprVec(_expr_vec) => unimplemented!(
                     "Create a new expression with an vector of expression is not supported yet."
@@ -1038,14 +1086,43 @@
                 }
             }),
             ref_expr: None,
         }
     }
 
     /// chain a new function to current function chain, the function accept
+    /// an array of type `ArrViewD<'a, T>` and return `ArrViewD<'a, T2>`
+    pub fn chain_view_out_f<F, T2>(self, f: F) -> ExprInner<'a, T2>
+    where
+        F: FnOnce(ArrViewD<'_, T>) -> ArrViewD<'a, T2> + Send + Sync + 'a,
+        T2: ExprElement,
+    {
+        ExprInner::<'a, T2> {
+            base: self.base,
+            step: self.step + 1,
+            name: self.name.clone(),
+            owned: None,
+            func: Box::new(move |base: ExprBase<'a>| {
+                let base_expr: ExprsInner = ExprInner::<T>::new_with_base(base, self.name).into();
+                let base_expr = Arc::new(Mutex::new(base_expr));
+                if let Some(mut ref_expr) = self.ref_expr {
+                    ref_expr.push(base_expr.clone())
+                }
+                let arb_array = (self.func)(ExprBase::Expr(base_expr)).into_arr();
+                match arb_array {
+                    ArbArray::View(arr) => f(arr).into(),
+                    ArbArray::ViewMut(arr) => f(arr.view()).into(),
+                    ArbArray::Owned(arr) => f(arr.view()).into(),
+                }
+            }),
+            ref_expr: None,
+        }
+    }
+
+    /// chain a new function to current function chain, the function accept
     /// an array of type `ArrViewMutD<'a, T>` and modify inplace.
     pub fn chain_view_mut_f<F>(self, f: F) -> ExprInner<'a, T>
     where
         T: Clone,
         F: FnOnce(&mut ArrViewMutD<'_, T>) + Send + Sync + 'a,
     {
         ExprInner::<'a, T> {
@@ -1123,25 +1200,14 @@
             // safety: T and T2 are the same type
             unsafe { mem::transmute(self) }
         } else {
             self.chain_view_f(move |arr| arr.to_bool().into())
         }
     }
 
-    // /// Try casting to datetime type
-    // pub fn cast_datetime(self, unit: Option<TimeUnit>) -> ExprInner<'a, DateTime>
-    // where T: AsPrimitive<i64>,
-    // {
-    //     if (T::dtype() == DataType::DateTime) || unit.is_none() {
-    //         unsafe {mem::transmute(self)}
-    //     } else {
-    //         self.chain_view_f(move |arr| arr.to_datetime(unit.unwrap()).into())
-    //     }
-    // }
-
     /// Try casting to datetime type
     #[allow(clippy::unnecessary_unwrap)]
     pub fn cast_datetime(self, unit: Option<TimeUnit>) -> ExprInner<'a, DateTime>
     where
         T: AsPrimitive<i64>,
     {
         if (T::dtype() == DataType::DateTime) || unit.is_none() {
```

### Comparing `teapy-0.1.2/src/arr/macros.rs` & `teapy-0.1.3/src/arr/macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/mod.rs` & `teapy-0.1.3/src/arr/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 pub use groupby::{groupby, groupby_par};
 pub use iterators::{Iter, IterMut};
 pub use join::{join_left, JoinType};
 pub use util_trait::{CollectTrusted, CollectTrustedToVec, TrustedLen};
 pub use utils::{kh_sum, DefaultNew, EmptyNew};
 
 #[cfg(feature = "lazy")]
-pub use lazy::{Expr, ExprElement, ExprOut, ExprOutView, Exprs};
+pub use lazy::{DropNaMethod, Expr, ExprElement, ExprOut, ExprOutView, Exprs};
 
 pub use time::{DateTime, TimeDelta, TimeUnit};
 
 use ndarray::{
     Array, Array1, ArrayBase, Axis, Data, DataMut, DataOwned, Dimension, Ix0, Ix1, Ix2, IxDyn,
     OwnedRepr, RawArrayView, RawArrayViewMut, RawData, RawDataClone, RemoveAxis, ShapeBuilder,
     ShapeError, StrideShape, ViewRepr, Zip,
@@ -639,14 +639,28 @@
     }
 
     #[allow(unreachable_patterns)]
     pub fn ndim(&self) -> usize {
         match_arbarray!(self, a, { a.ndim() })
     }
 
+    #[inline]
+    pub fn is_owned(&self) -> bool {
+        matches!(self, ArbArray::Owned(_))
+    }
+
+    #[allow(unreachable_patterns)]
+    pub fn get_type(&self) -> &'static str {
+        match self {
+            ArbArray::Owned(_) => "Owned Array",
+            ArbArray::ViewMut(_) => "ViewMut Array",
+            ArbArray::View(_) => "View Array",
+        }
+    }
+
     #[allow(unreachable_patterns)]
     pub fn strides(&self) -> &[isize] {
         match_arbarray!(self, a, { a.strides() })
     }
 
     #[allow(unreachable_patterns)]
     pub fn as_ptr(&self) -> *const T {
@@ -728,14 +742,18 @@
         match_arr!(self, a, { a.raw_dim() })
     }
 
     pub fn ndim(&self) -> usize {
         match_arr!(self, a, { a.ndim() })
     }
 
+    pub fn get_type(&self) -> &'static str {
+        match_arr!(self, a, { a.get_type() })
+    }
+
     #[allow(unreachable_patterns)]
     pub fn as_ptr<T: GetDataType>(&self) -> *const T {
         // we have known the datatype of the enum ,so only one arm will be executed
         match_datatype_arm!(
             self,
             a,
             ArrOk,
```

### Comparing `teapy-0.1.2/src/arr/time.rs` & `teapy-0.1.3/src/arr/time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/util_trait.rs` & `teapy-0.1.3/src/arr/util_trait.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/utils/algos.rs` & `teapy-0.1.3/src/arr/utils/algos.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/utils/alloc.rs` & `teapy-0.1.3/src/arr/utils/alloc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/window/compare.rs` & `teapy-0.1.3/src/arr/window/compare.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/window/corr.rs` & `teapy-0.1.3/src/arr/window/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/window/feature.rs` & `teapy-0.1.3/src/arr/window/feature.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/window/norm.rs` & `teapy-0.1.3/src/arr/window/norm.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/arr/window/reg.rs` & `teapy-0.1.3/src/arr/window/reg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/eager_api.rs` & `teapy-0.1.3/src/eager_api.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/eager_macros.rs` & `teapy-0.1.3/src/eager_macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/from_py.rs` & `teapy-0.1.3/src/from_py.rs`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 };
 use numpy::{
     datetime::{units, Datetime},
     Element, PyArray, PyArray1, PyArrayDescr, PyArrayDyn,
 };
 use pyo3::{exceptions::PyValueError, FromPyObject, PyAny, PyObject, PyResult, Python, ToPyObject};
 
+#[cfg(feature = "lazy")]
+use crate::arr::DropNaMethod;
+use crate::arr::{CorrMethod, FillMethod, QuantileMethod, WinsorizeMethod};
+
 #[derive(Debug, Clone)]
 #[repr(transparent)]
 pub struct PyValue(pub PyObject);
 
 impl ToPyObject for PyValue {
     fn to_object(&self, py: Python<'_>) -> PyObject {
         self.0.to_object(py)
@@ -177,15 +181,14 @@
 pub enum GroupByKey<'py> {
     // Str(&'py PyArray1<PyObject>),
     I32(&'py PyArray1<i32>),
     I64(&'py PyArray1<i64>),
     Usize(&'py PyArray1<usize>),
 }
 
-use crate::arr::{CorrMethod, FillMethod, QuantileMethod, WinsorizeMethod};
 impl<'source> FromPyObject<'source> for CorrMethod {
     fn extract(ob: &'source PyAny) -> PyResult<Self> {
         let s: Option<&str> = ob.extract()?;
         let s = s.unwrap_or("pearson").to_lowercase();
         let out = match s.as_str() {
             "pearson" => CorrMethod::Pearson,
             "spearman" => CorrMethod::Spearman,
@@ -249,14 +252,28 @@
             "outer" => JoinType::Outer,
             _ => panic!("Not supported join method: {s}"),
         };
         Ok(out)
     }
 }
 
+#[cfg(feature = "lazy")]
+impl<'source> FromPyObject<'source> for DropNaMethod {
+    fn extract(ob: &'source PyAny) -> PyResult<Self> {
+        let s: Option<&str> = ob.extract()?;
+        let s = s.unwrap_or("any").to_lowercase();
+        let out = match s.as_str() {
+            "all" => DropNaMethod::All,
+            "any" => DropNaMethod::Any,
+            _ => panic!("Not supported dropna method: {s}"),
+        };
+        Ok(out)
+    }
+}
+
 pub trait NoDim0 {
     fn no_dim0(self, py: Python) -> PyResult<PyObject>;
 }
 
 impl<T, D> NoDim0 for &PyArray<T, D> {
     fn no_dim0(self, py: Python) -> PyResult<PyObject> {
         if self.ndim() == 0 {
```

### Comparing `teapy-0.1.2/src/lib.rs` & `teapy-0.1.3/src/lib.rs`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #[cfg(feature = "eager_api")]
 pub(crate) mod eager_macros;
 
 #[cfg(feature = "eager_api")]
 mod eager_api;
 
 #[cfg(feature = "lazy")]
-mod pylazy;
+pub mod pylazy;
 
 #[cfg(feature = "lazy")]
 mod equity;
 
 use pyo3::{pymodule, types::PyModule, wrap_pyfunction, PyResult, Python};
 
 #[cfg(feature = "eager_api")]
@@ -42,9 +42,10 @@
 }
 
 #[pymodule]
 fn teapy(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     add_lazy(m)?;
     add_eager(m)?;
     m.add_function(wrap_pyfunction!(equity::calc_digital_ret, m)?)?;
+    m.add_function(wrap_pyfunction!(equity::calc_ret_single, m)?)?;
     Ok(())
 }
```

### Comparing `teapy-0.1.2/src/pylazy/datadict.rs` & `teapy-0.1.3/src/pylazy/datadict.rs`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #[pyclass]
 #[derive(Clone)]
 pub struct PyDataDict {
     data: Vec<PyExpr>,
     column_map: Arc<Mutex<HashMap<String, usize>>>,
 }
 
+#[allow(clippy::missing_safety_doc)]
 impl PyDataDict {
     pub fn new(mut data: Vec<PyExpr>, columns: Option<Vec<String>>) -> Self {
         if let Some(columns) = columns {
             assert_eq!(data.len(), columns.len());
             let mut column_map =
                 HashMap::<String, usize>::with_capacity(data.len().max(PYDATADICT_INIT_SIZE));
             for (col_name, i) in zip(columns, 0..data.len()) {
@@ -57,14 +58,19 @@
     }
 
     #[inline(always)]
     pub fn len(&self) -> usize {
         self.data.len()
     }
 
+    #[inline(always)]
+    pub fn is_empty(&self) -> bool {
+        self.len() == 0
+    }
+
     // fn create_column_map(&mut self) {
     //     let mut column_map = HashMap::<String, usize>::with_capacity(self.data.len());
     //     let mut name_auto = 0;
     //     for i in 0..self.data.len() {
     //         // we must check the name of PyExpr
     //         let expr = unsafe { self.data.get_unchecked_mut(i) };
     //         if let Some(name) = expr.get_name() {
@@ -322,19 +328,20 @@
             }
         });
         Ok(())
     }
 }
 
 #[pymethods]
+#[allow(clippy::missing_safety_doc)]
 impl PyDataDict {
     #[new]
     #[pyo3(signature=(data, columns=None, copy=false))]
-    pub unsafe fn init(data: &PyAny, columns: Option<Vec<String>>, copy: bool) -> PyResult<Self> {
-        let data = parse_expr_list(data, copy)?;
+    pub fn init(data: &PyAny, columns: Option<Vec<String>>, copy: bool) -> PyResult<Self> {
+        let data = unsafe { parse_expr_list(data, copy)? };
         Ok(Self::new(data, columns))
     }
 
     #[allow(clippy::wrong_self_convention)]
     pub fn to_pd(&mut self) -> PyResult<PyObject> {
         self.eval_all()?;
         Python::with_gil(|py| {
@@ -546,15 +553,15 @@
         &mut self,
         window: usize,
         func: &PyAny,
         axis: usize,
         check: bool,
         py_kwargs: Option<&PyDict>,
     ) -> PyResult<Self> {
-        if self.len() == 0 {
+        if self.is_empty() {
             return Ok(self.clone());
         }
         if window == 0 {
             return Err(PyValueError::new_err("Window should be greater than 0"));
         }
         self.eval_all()?;
         let length = match_exprs!(&self.data[0].inner, expr, { expr.view_arr().shape()[axis] });
@@ -614,15 +621,15 @@
         duration: &str,
         func: &PyAny,
         index: Option<&str>,
         axis: usize,
         check: bool,
         py_kwargs: Option<&PyDict>,
     ) -> PyResult<Self> {
-        if self.len() == 0 {
+        if self.is_empty() {
             return Ok(self.clone());
         }
         self.eval_all()?;
         let index = if let Some(index) = index {
             self.get_by_str(index)
         } else {
             let mut dt_num = 0; // number of datetime expression in datadict
```

### Comparing `teapy-0.1.2/src/pylazy/export.rs` & `teapy-0.1.3/src/pylazy/export.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/pylazy/groupby.rs` & `teapy-0.1.3/src/pylazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/src/pylazy/impl_pyexpr.rs` & `teapy-0.1.3/src/pylazy/impl_pyexpr.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 use super::export::*;
 use super::pyfunc::{parse_expr, parse_expr_list, parse_expr_nocopy, where_};
-use crate::arr::{DateTime, ExprOut, ExprOutView, Number, TimeDelta, WinsorizeMethod};
+use crate::arr::{
+    DateTime, DropNaMethod, ExprOut, ExprOutView, Number, TimeDelta, WinsorizeMethod,
+};
 use crate::from_py::{NoDim0, PyValue};
 use ndarray::SliceInfoElem;
 use num::PrimInt;
 use pyo3::{pyclass::CompareOp, PyTraverseError, PyVisit};
 use std::iter::repeat;
 
 macro_rules! impl_py_matmul {
@@ -73,14 +75,15 @@
             }
         }
     };
 
 }
 
 #[pymethods]
+#[allow(clippy::missing_safety_doc)]
 impl PyExpr {
     #[new]
     #[pyo3(signature=(expr, name=None, copy=false))]
     pub unsafe fn new(expr: &PyAny, name: Option<String>, copy: bool) -> PyResult<Self> {
         let mut out = parse_expr(expr, copy)?;
         if let Some(name) = name {
             out.set_name(name);
@@ -103,14 +106,28 @@
             Object(_) => "Object",
             DateTime(_) => "DateTime",
             TimeDelta(_) => "TimeDelta",
             OpUsize(_) => "OptionUsize",
         }
     }
 
+    #[getter]
+    #[allow(unreachable_patterns)]
+    pub fn get_base_type(&self) -> &'static str {
+        match_exprs!(&self.inner, e, { e.get_base_type() })
+    }
+
+    #[getter]
+    #[allow(unreachable_patterns)]
+    pub fn get_base_strong_count(&self) -> PyResult<usize> {
+        match_exprs!(&self.inner, e, {
+            e.get_base_strong_count().map_err(PyValueError::new_err)
+        })
+    }
+
     fn __traverse__(&self, visit: PyVisit<'_>) -> Result<(), PyTraverseError> {
         if let Some(obj_vec) = &self.obj {
             for obj in obj_vec {
                 visit.call(obj)?
             }
         }
         Ok(())
@@ -187,15 +204,15 @@
     #[pyo3(name="eval", signature=(inplace=false))]
     #[allow(unreachable_patterns)]
     pub fn eval_py(&mut self, inplace: bool) -> Option<Self> {
         self.eval_inplace();
         if !inplace {
             Some(self.clone())
         } else {
-            self.eval_inplace();
+            // self.eval_inplace();
             None
         }
     }
 
     #[getter]
     #[allow(unreachable_patterns)]
     pub fn get_view(self: PyRefMut<Self>, py: Python) -> PyResult<PyObject> {
@@ -217,20 +234,24 @@
                 unsafe {
                     let container = PyAny::from_borrowed_ptr(py, self.as_ptr());
                     let out_view = expr.try_view().map_err(PyValueError::new_err)?;
                     if matches!(out_view, ExprOutView::ArrVec(_)) {
                         let out = out_view
                             .as_arr_vec()
                             .iter()
-                            .map(|arr| PyArray::borrow_from_array(arr, container))
-                            .collect_trusted();
-                        let out = out
-                            .into_iter()
-                            .map(|e| e.no_dim0(py).unwrap())
+                            .map(|arr| {
+                                PyArray::borrow_from_array(arr, container)
+                                    .no_dim0(py)
+                                    .unwrap()
+                            })
                             .collect_trusted();
+                        // let out = out
+                        //     .into_iter()
+                        //     .map(|e| e.no_dim0(py).unwrap())
+                        //     .collect_trusted();
                         Ok(out.into_py(py))
                     } else {
                         Ok(PyArray::borrow_from_array(out_view.as_arr(), container).no_dim0(py)?)
                     }
                 }
             },
             I32,
@@ -322,15 +343,15 @@
 
     #[allow(unreachable_patterns)]
     pub(crate) fn is_owned(&self) -> PyResult<bool> {
         match_exprs!(&self.inner, expr, {
             if let Some(owned) = expr.owned() {
                 Ok(owned)
             } else {
-                Err(PyValueError::new_err("expression is not evaluated"))
+                Err(PyValueError::new_err("Expression is not evaluated"))
             }
         })
     }
 
     #[allow(unreachable_patterns)]
     pub unsafe fn reshape(self: PyRef<Self>, shape: &PyAny) -> PyResult<Self> {
         let shape = parse_expr_nocopy(shape)?;
@@ -355,14 +376,19 @@
     }
 
     #[allow(unreachable_patterns)]
     pub fn ref_count(&mut self) -> usize {
         match_exprs!(&self.inner, expr, { expr.ref_count() })
     }
 
+    #[allow(unreachable_patterns)]
+    pub fn hint_arr_type(&mut self) -> Self {
+        match_exprs!(&self.inner, expr, { expr.clone().hint_arr_type().into() })
+    }
+
     unsafe fn __add__(&self, other: &PyAny) -> PyResult<Self> {
         let other = parse_expr_nocopy(other)?;
         let (obj, obj2) = (self.obj(), other.obj());
         use Exprs::*;
         let out = match (&self.inner, &other.inner) {
             (F64(_), _) | (_, F64(_)) => (self.clone().cast_f64()? + other.cast_f64()?)
                 .to_py(obj)
@@ -813,14 +839,27 @@
     /// Returns the cube root of each element.
     pub fn cbrt(&self) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().exp2().to_py(self.obj())
         })
     }
 
+    /// Returns the sign of each element.
+    fn sign(&self) -> PyResult<Self> {
+        Ok(match_exprs!(
+            &self.inner,
+            e,
+            { e.clone().sign(false).to_py(self.obj()) },
+            F64,
+            F32,
+            I32,
+            I64
+        ))
+    }
+
     /// Returns the natural logarithm of each element.
     pub fn ln(&self) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().ln().to_py(self.obj())
         })
     }
 
@@ -1192,14 +1231,44 @@
                 .filter(mask.cast_bool()?, axis.cast_usize()?, par)
                 .to_py(self.obj())
                 .add_obj(obj)
                 .add_obj(obj2)
         }))
     }
 
+    #[pyo3(signature=(axis=None, how=DropNaMethod::Any, par=false))]
+    pub unsafe fn dropna(
+        &self,
+        axis: Option<&PyAny>,
+        how: DropNaMethod,
+        par: bool,
+    ) -> PyResult<Self> {
+        let axis = if let Some(axis) = axis {
+            parse_expr_nocopy(axis)?
+        } else {
+            0.into()
+        };
+        let obj = axis.obj();
+        Ok(match_exprs!(
+            &self.inner,
+            expr,
+            {
+                expr.clone()
+                    .dropna(axis.cast_usize()?, how, par)
+                    .to_py(self.obj())
+                    .add_obj(obj)
+            },
+            F32,
+            F64,
+            I32,
+            I64,
+            Usize
+        ))
+    }
+
     pub fn is_nan(&self) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().is_nan().to_py(self.obj())
         })
     }
 
     pub fn not_nan(&self) -> Self {
@@ -1468,48 +1537,58 @@
             expr.clone()
                 .split_group(group, rev, axis, par)
                 .to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(other, stable=false, axis=0, par=false))]
-    pub fn cov(&self, other: Self, stable: bool, axis: usize, par: bool) -> Self {
+    pub unsafe fn cov(
+        &self,
+        other: &PyAny,
+        stable: bool,
+        axis: usize,
+        par: bool,
+    ) -> PyResult<Self> {
+        let other = parse_expr_nocopy(other)?;
         let obj = other.obj();
-        match_exprs!(
+        let res = match_exprs!(
             (&self.inner, e1, F64, F32, I64, I32),
             (&other.inner, e2, F64, F32, I64, I32),
             {
                 e1.clone()
                     .cov(e2.clone(), stable, axis, par)
                     .to_py(self.obj())
                     .add_obj(obj)
             }
-        )
+        );
+        Ok(res)
     }
 
     #[pyo3(signature=(other, method=CorrMethod::Pearson, stable=false, axis=0, par=false))]
-    pub fn corr(
+    pub unsafe fn corr(
         &self,
-        other: Self,
+        other: &PyAny,
         method: CorrMethod,
         stable: bool,
         axis: usize,
         par: bool,
-    ) -> Self {
+    ) -> PyResult<Self> {
+        let other = parse_expr_nocopy(other)?;
         let obj = other.obj();
-        match_exprs!(
+        let res = match_exprs!(
             (&self.inner, e1, F64, F32, I64, I32),
             (&other.inner, e2, F64, F32, I64, I32),
             {
                 e1.clone()
                     .corr(e2.clone(), method, stable, axis, par)
                     .to_py(self.obj())
                     .add_obj(obj)
             }
-        )
+        );
+        Ok(res)
     }
 
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, axis=0, par=false))]
     pub fn ts_argmin(&self, window: usize, min_periods: usize, axis: usize, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
@@ -1609,58 +1688,62 @@
             F32,
             I64
         )
     }
 
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(other, window, min_periods=1, stable=false, axis=0, par=false))]
-    pub fn ts_cov(
+    pub unsafe fn ts_cov(
         &self,
-        other: Self,
+        other: &PyAny,
         window: usize,
         min_periods: usize,
         stable: bool,
         axis: usize,
         par: bool,
-    ) -> Self {
+    ) -> PyResult<Self> {
+        let other = parse_expr_nocopy(other)?;
         let obj = other.obj();
-        match_exprs!(
+        let res = match_exprs!(
             (&self.inner, e1, F64, F32, I64, I32),
             (&other.inner, e2, F64, F32, I64, I32),
             {
                 e1.clone()
                     .ts_cov(e2.clone(), window, min_periods, stable, axis, par)
                     .to_py(self.obj())
                     .add_obj(obj)
             }
-        )
+        );
+        Ok(res)
     }
 
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(other, window, min_periods=1, stable=false, axis=0, par=false))]
-    pub fn ts_corr(
+    pub unsafe fn ts_corr(
         &self,
-        other: Self,
+        other: &PyAny,
         window: usize,
         min_periods: usize,
         stable: bool,
         axis: usize,
         par: bool,
-    ) -> Self {
+    ) -> PyResult<Self> {
+        let other = parse_expr_nocopy(other)?;
         let obj = other.obj();
-        match_exprs!(
+        let res = match_exprs!(
             (&self.inner, e1, F64, F32, I64, I32),
             (&other.inner, e2, F64, F32, I64, I32),
             {
                 e1.clone()
                     .ts_corr(e2.clone(), window, min_periods, stable, axis, par)
                     .to_py(self.obj())
                     .add_obj(obj)
             }
-        )
+        );
+        Ok(res)
     }
 
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_sum(
         &self,
         window: usize,
@@ -1974,15 +2057,15 @@
             I32,
             F32,
             I64
         )
     }
 
     #[cfg(feature = "window_func")]
-    #[pyo3(signature=(method, value=None, axis=0, par=false))]
+    #[pyo3(signature=(method=FillMethod::Ffill, value=None, axis=0, par=false))]
     pub fn fillna(&self, method: FillMethod, value: Option<f64>, axis: usize, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .fillna(method, value, axis, par)
                 .to_py(self.obj())
         })
     }
```

### Comparing `teapy-0.1.2/src/pylazy/mod.rs` & `teapy-0.1.3/src/pylazy/mod.rs`

 * *Files 7% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 mod pyfunc;
 mod time;
 
 pub use datadict::PyDataDict;
 pub use groupby::PyGroupBy;
 pub use pyexpr::PyExpr;
 pub use pyfunc::{
-    arange, concat_expr, datetime, eval, from_pandas, full, get_newey_west_adjust_s, parse_expr,
-    parse_expr_list, parse_expr_nocopy, timedelta, where_py,
+    arange, concat_expr, concat_expr_py, datetime, eval, from_pandas, full,
+    get_newey_west_adjust_s, parse_expr, parse_expr_list, parse_expr_nocopy, timedelta, where_py,
 };
 
 use pyo3::prelude::{wrap_pyfunction, PyModule, PyResult};
 
 pub(crate) fn add_lazy(m: &PyModule) -> PyResult<()> {
     m.add_class::<PyExpr>()?;
     m.add_class::<PyDataDict>()?;
     m.add_class::<PyGroupBy>()?;
-    m.add_function(wrap_pyfunction!(concat_expr, m)?)?;
+    m.add_function(wrap_pyfunction!(concat_expr_py, m)?)?;
     m.add_function(wrap_pyfunction!(eval, m)?)?;
     m.add_function(wrap_pyfunction!(where_py, m)?)?;
     m.add_function(wrap_pyfunction!(full, m)?)?;
     m.add_function(wrap_pyfunction!(arange, m)?)?;
     m.add_function(wrap_pyfunction!(datetime, m)?)?;
     m.add_function(wrap_pyfunction!(timedelta, m)?)?;
     m.add_function(wrap_pyfunction!(from_pandas, m)?)?;
```

### Comparing `teapy-0.1.2/src/pylazy/pyexpr.rs` & `teapy-0.1.3/src/pylazy/pyexpr.rs`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 use super::export::*;
 use crate::{
     arr::{ArbArray, DateTime, ExprElement, Number, TimeDelta, TimeUnit},
     from_py::PyValue,
 };
 
-#[pyclass]
+#[pyclass(subclass)]
 #[derive(Clone, Default)]
 pub struct PyExpr {
     pub inner: Exprs<'static>,
     pub obj: Option<Vec<PyObject>>,
 }
 
 impl From<Exprs<'static>> for PyExpr {
```

### Comparing `teapy-0.1.2/teapy/array_func.py` & `teapy-0.1.3/teapy/array_func.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from warnings import warn
 
 import numpy as np
 
 from . import teapy as _tp
-from .wrapper import wrap
+from .wrapper import default_wrapper, impl_by_lazy, wrap
 
 __all__ = [
     "sum",
     "min",
     "max",
     "mean",
     "median",
@@ -24,18 +24,20 @@
     "corr",
     "fillna",
     "zscore",
     "winsorize",
     "remove_nan",
     "split_group",
     "clip",
+    "shift",
 ]
 
 
-@wrap("array_agg_func")
+# @wrap("array_agg_func")
+@impl_by_lazy()
 def sum(arr, stable=False, axis=0, par=False):
     """
     Sum of array elements in a given axis.
 
     Parameters
     ----------
     arr : np.ndarray, pd.Series, pd.DataFrame, tuple, list
@@ -50,105 +52,111 @@
     Returns
     -------
     array_like.
 
     """
 
 
-@wrap("array_agg_func")
+# @wrap("array_agg_func")
+@impl_by_lazy()
 def min(arr, axis=0, par=False):
     pass
 
 
-@wrap("array_agg_func")
+@impl_by_lazy()
 def max(arr, axis=0, par=False):
     pass
 
 
-@wrap("array_agg_func")
+@impl_by_lazy()
 def mean(arr, stable=False, axis=0, par=False):
     pass
 
 
-@wrap("array_agg_func")
+@impl_by_lazy()
 def median(arr, axis=0, par=False):
     pass
 
 
-@wrap("array_agg_func")
+@impl_by_lazy()
 def quantile(arr, q, method="Linear", axis=0, par=False):
     pass
 
 
-@wrap("array_agg_func")
+@impl_by_lazy()
 def std(arr, stable=False, axis=0, par=False):
     pass
 
 
-@wrap("array_agg_func")
+@impl_by_lazy()
 def var(arr, stable=False, axis=0, par=False):
     pass
 
 
-@wrap("array_agg_func")
+@impl_by_lazy()
 def skew(arr, stable=False, axis=0, par=False):
     pass
 
 
-@wrap("array_agg_func")
+@impl_by_lazy()
 def kurt(arr, stable=False, axis=0, par=False):
     pass
 
 
-@wrap("array_agg_func")
+@impl_by_lazy()
 def count_nan(arr, axis=0, par=False):
     pass
 
 
-@wrap("array_agg_func")
+@impl_by_lazy()
 def count_notnan(arr, axis=0, par=False):
     pass
 
 
-@wrap("array_func")
+# @wrap("array_func")
+@impl_by_lazy()
 def argsort(arr, axis=0, par=False, rev=False):
     pass
 
 
-@wrap("array_agg_func2")
+# @wrap("array_agg_func2")
+@impl_by_lazy("default2")
 def cov(arr1, arr2, stable=False, axis=0, par=False):
     pass
 
 
-@wrap("array_agg_func2")
+@impl_by_lazy("default2")
 def corr(arr1, arr2, method=None, stable=False, axis=0, par=False):
     pass
 
 
-@wrap("array_func")
+@impl_by_lazy()
 def rank(arr, pct=False, axis=0, par=False, rev=False):
     pass
 
 
 @wrap("array_func", inplace=True)
 def clip(arr, min, max, axis=0, par=False):
     pass
 
 
 @wrap("base")
+# @impl_by_lazy()
 def remove_nan(arr):
     pass
 
 
-@wrap("array_func")
+# @wrap("array_func")
+@impl_by_lazy()
 def split_group(arr, axis=0, par=False):
     pass
 
 
 @wrap("array_agg_func", inplace=True)
+# @impl_by_lazy()
 def fillna(arr, method=None, value=None, axis=0, par=False, inplace=False):
     pass
 
 
 @wrap("array_func", use=True)
 def zscore(arr, stable=False, axis=0, par=False, inplace=False):
     if inplace:
@@ -210,7 +218,12 @@
         warn("the dtype of arr is not float, so note that the result is not float too")
     if inplace:
         return _tp.winsorize_inplace(
             arr, method, method_params, stable, axis=axis, par=par
         )
     else:
         return _tp.winsorize(arr, method, method_params, stable, axis=axis, par=par)
+
+
+@impl_by_lazy()
+def shift(arr, n=1, fill=None, axis=0, par=False):
+    pass
```

### Comparing `teapy-0.1.2/teapy/converter.py` & `teapy-0.1.3/teapy/converter.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/teapy/datadict.py` & `teapy-0.1.3/teapy/datadict.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from .teapy import PyDataDict as _DataDict
 from .teapy import from_pandas
 
 
 def _new_with_dd(dd=None):
     if dd is None:
+        # for inplace functions
         return None
     out = DataDict()
     out._dd = dd
     return out
 
 
 def construct(func):
+    """For functions that return a DataDict"""
+
     def inner(*args, **kwargs):
         dd = func(*args, **kwargs)
         return _new_with_dd(dd)
 
     return inner
 
 
@@ -91,15 +94,15 @@
 
 
 class DataDict:
     def __init__(self, *args, **kwargs):
         if len(args) or len(kwargs):
             self._dd = _DataDict(*args, **kwargs)
         else:
-            self._dd = None
+            self._dd = _DataDict([])
 
     def __getitem__(self, key):
         return self._dd[key]
 
     def __setitem__(self, item, value):
         self._dd.__setitem__(item, value)
```

### Comparing `teapy-0.1.2/teapy/regression.py` & `teapy-0.1.3/teapy/regression.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/teapy/testing.py` & `teapy-0.1.3/teapy/testing.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,26 +13,41 @@
 atol = 1e-3
 
 settings.register_profile("test", suppress_health_check=[HealthCheck(3)])
 settings.load_profile("test")
 
 isclose = partial(isclose, rel_tol=rtol, abs_tol=atol)
 
+
+def assert_isclose3(a, b, c, *args):
+    assert isclose(a, b)
+    assert isclose(b, c)
+    for v in args:
+        assert isclose(a, v)
+
+
 assert_series_equal = partial(
     assert_series_equal,
     rtol=rtol,
     atol=atol,
     check_index=False,
     check_dtype=False,
     check_names=False,
 )
 
 assert_allclose = partial(assert_allclose, rtol=rtol, atol=atol)
 
 
+def assert_allclose3(a, b, c, *args):
+    assert_allclose(a, b)
+    assert_allclose(b, c)
+    for v in args:
+        assert_allclose(a, v)
+
+
 # 同个数组中的数如果差距过大，在计算时太小的数会被忽略
 STABLE_FLOAT_MIN, STABLE_FLOAT_MAX = -10, 10
 STABLE_INT_MIN, STABLE_INT_MAX = int(-1e3), int(1e3)
 dtype_list = [np.float64, np.float32, np.int32, np.int64]
 dtype_element_map_stable = {
     np.float64: st.floats(
         width=16, min_value=STABLE_FLOAT_MIN, max_value=STABLE_FLOAT_MAX
```

### Comparing `teapy-0.1.2/teapy/tests/test_array_func.py` & `teapy-0.1.3/teapy/tests/test_array_func.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,59 @@
 import numpy as np
 import pandas as pd
 from hypothesis import given
 from hypothesis import strategies as st
 
 import teapy as tp
 from teapy import Expr
-from teapy.testing import assert_allclose, assert_series_equal, isclose, make_arr
+from teapy.testing import (
+    assert_allclose,
+    assert_allclose3,
+    assert_isclose3,
+    assert_series_equal,
+    make_arr,
+)
 
 
 @given(make_arr(30, unique=True, nan_p=0))
 def test_argsort(arr):
     res1 = tp.argsort(arr)
-    res2 = arr.argsort()
-    assert_allclose(res1, res2)
+    res2 = Expr(arr).argsort().eview()
+    res3 = arr.argsort()
+    assert_allclose3(res1, res2, res3)
     res1 = tp.argsort(arr, rev=True)
-    res2 = arr.argsort()[::-1]
-    assert_allclose(res1, res2)
+    res2 = Expr(arr).argsort(rev=True).eview()
+    res3 = arr.argsort()[::-1]
+    assert_allclose3(res1, res2, res3)
 
 
 @given(make_arr(30))
 def test_rank(arr):
     res1 = tp.rank(arr)
-    res2 = pd.Series(arr).rank()
-    assert_series_equal(pd.Series(res1), res2)
-
-    res3 = tp.rank(arr, rev=True)
-    res4 = pd.Series(arr).rank(ascending=False)
-    assert_series_equal(pd.Series(res3), res4)
-
-    res5 = tp.rank(arr, pct=True)
-    res6 = pd.Series(arr).rank(pct=True)
-    assert_series_equal(pd.Series(res5), res6)
+    res2 = Expr(arr).rank().eview()
+    res3 = pd.Series(arr).rank().values
+    assert_allclose3(res1, res2, res3)
+
+    res4 = tp.rank(arr, rev=True)
+    res5 = Expr(arr).rank(rev=True).eview()
+    res6 = pd.Series(arr).rank(ascending=False).values
+    assert_allclose3(res4, res5, res6)
+
+    res7 = tp.rank(arr, pct=True)
+    res8 = Expr(arr).rank(pct=True).eview()
+    res9 = pd.Series(arr).rank(pct=True).values
+    assert_allclose3(res7, res8, res9)
 
 
 @given(make_arr((10, 10)), st.integers(0, 1))
 def test_max(arr, axis):
     res1 = tp.max(arr, axis=axis)
-    res2 = np.nanmax(arr, axis=axis)
-    assert_allclose(res1, res2)
+    res2 = Expr(arr).max(axis=axis).eview()
+    res3 = np.nanmax(arr, axis=axis)
+    assert_allclose3(res1, res2, res3)
 
 
 def test_arg_partition():
     arr = np.array(
         [
             [6, 0, -2, 8, -7],
             [-2, 3, -10, 2, 9],
@@ -59,203 +71,232 @@
     arr = Expr([1, np.nan, 3, np.nan, np.nan])
     assert_allclose(arr.arg_partition(2, rev=True).eview(), np.array([2, 0, -1]))
 
 
 @given(make_arr((10, 10)), st.integers(0, 1))
 def test_min(arr, axis):
     res1 = tp.min(arr, axis=axis)
-    res2 = np.nanmin(arr, axis=axis)
-    assert_allclose(res1, res2)
+    res2 = Expr(arr).min(axis=axis).eview()
+    res3 = np.nanmin(arr, axis=axis)
+    assert_allclose3(res1, res2, res3)
 
 
 @given(make_arr((10, 10)), st.integers(0, 1))
 def test_sum(arr, axis):
     res1 = tp.sum(arr, axis=axis)
-    res2 = np.nansum(arr, axis=axis)
-    assert_allclose(res1, res2)
+    res2 = Expr(arr).sum(axis=axis).eview()
+    res3 = np.nansum(arr, axis=axis)
+    assert_allclose3(res1, res2, res3)
 
 
 @given(make_arr((10, 10)), st.integers(0, 1))
 def test_median(arr, axis):
     res1 = tp.median(arr, axis=axis)
-    res2 = np.nanmedian(arr, axis=axis)
-    assert_allclose(res1, res2)
+    res2 = Expr(arr).median(axis=axis).eview()
+    res3 = np.nanmedian(arr, axis=axis)
+    assert_allclose3(res1, res2, res3)
 
 
 @given(make_arr((10, 10)), st.floats(0, 1), st.integers(0, 1))
 def test_quantile(arr, q, axis):
     res1 = tp.quantile(arr, q, axis=axis)
-    res2 = np.nanquantile(arr, q, axis=axis)
-    assert_allclose(res1, res2)
+    res2 = Expr(arr).quantile(q, axis=axis).eview()
+    res3 = np.nanquantile(arr, q, axis=axis)
+    assert_allclose3(res1, res2, res3)
 
 
 @given(make_arr((10, 10), nan_p=0.5), st.integers(0, 1))
 def test_count_nan(arr, axis):
     res1 = np.count_nonzero(np.isnan(arr), axis=axis)
     res2 = tp.count_nan(arr, axis=axis)
-    assert_allclose(res1, res2)
-    res3 = np.count_nonzero(~np.isnan(arr), axis=axis)
-    res4 = tp.count_notnan(arr, axis=axis)
-    assert_allclose(res3, res4)
+    res3 = Expr(arr).count_nan(axis=axis).eview()
+    assert_allclose3(res1, res2, res3)
+    res4 = np.count_nonzero(~np.isnan(arr), axis=axis)
+    res5 = tp.count_notnan(arr, axis=axis)
+    res6 = Expr(arr).count_notnan(axis=axis).eview()
+    assert_allclose3(res4, res5, res6)
 
 
 @given(make_arr((10, 10)), st.integers(0, 1))
 def test_mean(arr, axis):
-    arr = pd.DataFrame(arr)
-    res1 = arr.mean(axis=axis)
+    res1 = pd.DataFrame(arr).mean(axis=axis).values
     res2 = tp.mean(arr, axis=axis)
     res3 = tp.mean(arr, axis=axis, stable=True)
-    assert_series_equal(res1, res2)
-    assert_series_equal(res1, res3)
+    res4 = Expr(arr).mean(axis=axis, stable=True).eview()
+    assert_allclose3(res1, res2, res3, res4)
 
 
 @given(make_arr((10, 10)), st.integers(0, 1))
 def test_std(arr, axis):
-    arr = pd.DataFrame(arr)
-    res1 = arr.std(axis=axis)
+    res1 = pd.DataFrame(arr).std(axis=axis).values
     res2 = tp.std(arr, axis=axis)
     res3 = tp.std(arr, axis=axis, stable=True)
-    assert_series_equal(res1, res2)
-    assert_series_equal(res1, res3)
+    res4 = Expr(arr).std(axis=axis, stable=True).eview()
+    assert_allclose3(res1, res2, res3, res4)
 
 
 @given(make_arr((10, 10)), st.integers(0, 1))
 def test_var(arr, axis):
-    arr = pd.DataFrame(arr)
-    res1 = arr.var(axis=axis)
+    res1 = pd.DataFrame(arr).var(axis=axis).values
     res2 = tp.var(arr, axis=axis)
     res3 = tp.var(arr, axis=axis, stable=True)
-    assert_series_equal(res1, res2)
-    assert_series_equal(res1, res3)
+    res4 = Expr(arr).var(axis=axis, stable=True).eview()
+    assert_allclose3(res1, res2, res3, res4)
 
 
 @given(make_arr((10, 10), unique=True), st.integers(0, 1))
 def test_skew(arr, axis):
-    arr = pd.DataFrame(arr)
-    res1 = arr.skew(axis=axis)
+    res1 = pd.DataFrame(arr).skew(axis=axis).values
     res2 = tp.skew(arr, axis=axis)
     res3 = tp.skew(arr, axis=axis, stable=True)
-    assert_series_equal(res1, res2)
-    assert_series_equal(res1, res3)
+    res4 = Expr(arr).skew(axis=axis, stable=True).eview()
+    assert_allclose3(res1, res2, res3, res4)
 
 
 @given(make_arr((10, 10), unique=True), st.integers(0, 1))
 def test_kurt(arr, axis):
-    arr = pd.DataFrame(arr)
-    res1 = arr.kurt(axis=axis)
+    res1 = pd.DataFrame(arr).kurt(axis=axis).values
     res2 = tp.kurt(arr, axis=axis)
     res3 = tp.kurt(arr, axis=axis, stable=True)
-    assert_series_equal(res1, res2)
-    assert_series_equal(res1, res3)
+    res4 = Expr(arr).kurt(axis=axis, stable=True).eview()
+    assert_allclose3(res1, res2, res3, res4)
 
 
 @given(make_arr((10, 2)))
 def test_cov(arr):
     cov_pd = pd.DataFrame(arr).cov().iloc[0, 1]
     arr1, arr2 = np.array_split(arr, 2, axis=1)
     cov1 = tp.cov(arr1, arr2, axis=0)[0]
     cov2 = tp.cov(arr1, arr2, axis=0, stable=True)[0]
-    assert isclose(cov_pd, cov1) & isclose(cov_pd, cov2)
+    cov3 = Expr(arr1).cov(Expr(arr2), axis=0)[0].eview()
+    cov4 = Expr(arr1).cov(Expr(arr2), axis=0, stable=True)[0].eview()
+    assert_isclose3(cov_pd, cov1, cov2, cov3, cov4)
 
 
 @given(make_arr((10, 2)))
 def test_corr(arr):
     for method in ["pearson", "spearman"]:
         corr_pd = pd.DataFrame(arr).corr(method).iloc[0, 1]
         arr1, arr2 = np.array_split(arr, 2, axis=1)
-        tp.corr(tp.rank(arr1), tp.rank(arr2))
         corr1 = tp.corr(arr1, arr2, axis=0, method=method)[0]
         corr2 = tp.corr(arr1, arr2, axis=0, method=method, stable=True)[0]
+        corr3 = Expr(arr1).corr(Expr(arr2), axis=0, method=method)[0].eview()
+        corr4 = (
+            Expr(arr1).corr(Expr(arr2), axis=0, method=method, stable=True)[0].eview()
+        )
         if np.isnan(corr_pd):
-            assert np.isnan(corr1) & np.isnan(corr2)
+            assert np.isnan(corr1) & np.isnan(corr2) & np.isnan(corr3) & np.isnan(corr4)
         else:
-            assert isclose(corr_pd, corr1) & isclose(corr_pd, corr2)
+            assert_isclose3(corr_pd, corr1, corr2, corr3, corr4)
 
 
 def test_array_func_2d():
     arr = np.random.randn(20, 20)
-    res1 = tp.rank(arr, axis=0)
-    res2 = pd.DataFrame(arr).rank(axis=0).values
-    assert_allclose(res1, res2)
+    res1 = tp.rank(arr, axis=1)
+    res2 = Expr(arr).rank(axis=1).eview()
+    res3 = pd.DataFrame(arr).rank(axis=1).values
+    assert_allclose3(res1, res2, res3)
 
 
 def test_fillna():
     s = pd.Series([np.nan, 5, 6, 733, np.nan, 34, np.nan, np.nan])
     for method in ["ffill", "bfill"]:
         assert_series_equal(tp.fillna(s, method), s.fillna(method=method))
+        assert_allclose(
+            Expr(s, copy=True).fillna(method).eview(), s.fillna(method=method).values
+        )
         # test inplace
         s1 = s.copy()
         tp.fillna(s1, method, inplace=True)
         assert_series_equal(s1, s.fillna(method=method))
+
     # test fill value directly
     fill_value = 101
     assert_series_equal(tp.fillna(s, value=fill_value), s.fillna(fill_value))
+    assert_allclose(
+        Expr(s, copy=True).fillna(value=fill_value).eview(), s.fillna(fill_value).values
+    )
+    # test inplace
     tp.fillna(s, value=fill_value, inplace=True)
     assert_series_equal(s, pd.Series([101, 5, 6, 733, 101, 34, 101, 101]))
 
 
 def test_clip():
     s = pd.Series([np.nan, 5, 6, 733, np.nan, 34, 456, np.nan])
     assert_series_equal(tp.clip(s, 5, 100), s.clip(5, 100))
+    assert_allclose(Expr(s).clip(5, 100).eview(), s.clip(5, 100))
     s1 = s.copy()
     tp.clip(s1, 5, 100, inplace=True)
     assert_series_equal(s1, s.clip(5, 100))
 
 
-def test_remove_nan():
+@given(make_arr((10, 2), nan_p=0.2), st.integers(0, 1))
+def test_dropna(arr, axis):
+    # test dropna 1d
     s = pd.Series([np.nan, 5, 6, 12, np.nan, 1, np.nan, np.nan])
     assert_series_equal(tp.remove_nan(s), s.dropna())
+    assert_allclose(Expr(s).dropna().eview(), s.dropna())
+    # test dropna 2d
+    assert_allclose(
+        Expr(arr).dropna(axis=axis).eview(), pd.DataFrame(arr).dropna(axis=axis)
+    )
 
 
 def test_zscore():
     s = pd.Series(np.arange(12).astype(float))
     for stable in False, True:
-        s1 = tp.zscore(s, stable)
-        s2 = (s - s.mean()) / s.std()
-        assert_series_equal(s1, s2)
+        s1 = tp.zscore(s, stable)  # eager
+        s2 = Expr(s).zscore(stable).eview()  # lazy
+        s3 = (s - s.mean()) / s.std()  # expect
+        assert_allclose3(s1, s2, s3)
+        # test inplace
         s_copy = s.copy()
         tp.zscore(s_copy, stable, inplace=True)
-        assert_series_equal(s_copy, s2)
+        assert_series_equal(s_copy, s3)
 
 
 def test_winsorize():
     s = pd.Series(np.arange(12).astype(float))
 
     # quantile method
     q = 0.05
     s1 = tp.winsorize(s, "quantile", q)
+    s2 = Expr(s, copy=True).winsorize("quantile", q).eview()
     lower, upper = np.nanquantile(s, [q, 1 - q])
-    s2 = s.clip(lower, upper)
-    assert_series_equal(s1, s2)
+    s3 = s.clip(lower, upper)
+    assert_allclose3(s1, s2, s3)
     # test quantile inplace
     s_copy = s.copy()
     tp.winsorize(s_copy, "quantile", q, inplace=True)
-    assert_series_equal(s_copy, s2)
+    assert_series_equal(s_copy, s3)
 
     # median method
     q = 1
     s1 = tp.winsorize(s, "median", q)
+    s2 = Expr(s, copy=True).winsorize("median", q).eview()
     median = s.median()
     mad = (s - median).abs().median()
-    s2 = s.clip(median - q * mad, median + q * mad)
-    assert_series_equal(s1, s2)
+    s3 = s.clip(median - q * mad, median + q * mad)
+    assert_allclose3(s1, s2, s3)
 
     # sigma method
     q = 1.2
     s1 = tp.winsorize(s, "sigma", q)
+    s2 = Expr(s, copy=True).winsorize("sigma", q).eview()
     mean = s.mean()
     std = s.std()
-    s2 = s.clip(mean - q * std, mean + q * std)
-    assert_series_equal(s1, s2)
+    s3 = s.clip(mean - q * std, mean + q * std)
+    assert_allclose3(s1, s2, s3)
 
 
 @given(make_arr(20), st.integers(1, 10))
 def test_split_group(arr, group):
     def split_group_py(x: pd.Series, group=10, method="average"):
         size = x.size - np.count_nonzero(np.isnan(x))
         out = np.ceil(x.rank(method=method) / (size / group))
         return out.fillna(0)
 
     arr = pd.Series(arr)
-    out1 = tp.split_group(arr, group)
-    out2 = split_group_py(arr, group)
-    assert_series_equal(out1, out2)
+    s1 = tp.split_group(arr, group)
+    s2 = Expr(arr).split_group(group).eview()
+    s3 = split_group_py(arr, group)
+    assert_allclose3(s1, s2, s3)
```

### Comparing `teapy-0.1.2/teapy/tests/test_common.py` & `teapy-0.1.3/teapy/tests/test_common.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,45 +53,46 @@
     # test rank a array with 0 element
     assert tp.rank(np.array([])).tolist() == []
     assert tp.rank(np.array([2]))[0] == 1  # test rank a array with 1 element
     # test rank all nan array
     assert_allclose(tp.rank(np.array([np.nan, np.nan])), np.array([np.nan, np.nan]))
 
 
-def test_array_func_input():
-    from pandas.testing import assert_frame_equal, assert_series_equal
-
-    value, expect = [3, 2, 1], [2, 1, 0]
-    # List input
-    assert tp.argsort(value).tolist() == expect
-    # Series input
-    sr = pd.Series(value, name="aa")
-    assert_series_equal(tp.argsort(sr), pd.Series(expect, name="aa"), check_dtype=False)
-    # DataFrame input
-    df = pd.DataFrame({"a": value})
-    assert_frame_equal(
-        tp.argsort(df, axis=0), pd.DataFrame({"a": expect}), check_dtype=False
-    )
-
-
-def test_ts_func_input():
-    from pandas.testing import assert_frame_equal, assert_series_equal
-
-    value, expect = [1, 1, 1], [1.0, 2, 3]
-    # list input
-    assert tp.ts_sum(value, 3).tolist() == expect
-    # series input
-    sr = pd.Series(value, name="aa")
-    assert_series_equal(tp.ts_sum(sr, 3), pd.Series(expect, name="aa"))
-    df = pd.DataFrame({"a": value})
-    assert_frame_equal(tp.ts_sum(df, 3, axis=0), pd.DataFrame({"a": expect}))
-
-
-def test_ts_func2_input():
-    from pandas.testing import assert_series_equal
-
-    value1, value2, expect = [1, 2, 3], [1, 2, 3], [np.nan, 1.0, 1.0]
-    # list input
-    assert_allclose(tp.ts_corr(value1, value2, 3), np.array(expect))
-    # series input
-    sr1, sr2 = pd.Series(value1, name="aa"), pd.Series(value1, name="bb")
-    assert_series_equal(tp.ts_corr(sr1, sr2, 3), pd.Series(expect, name="aa"))
+# # currently only numpy array output is supported
+# def test_array_func_input():
+#     from pandas.testing import assert_frame_equal, assert_series_equal
+
+#     value, expect = [3, 2, 1], [2, 1, 0]
+#     # List input
+#     assert tp.argsort(value).tolist() == expect
+#     # Series input
+#     sr = pd.Series(value, name="aa")
+#     assert_series_equal(tp.argsort(sr), pd.Series(expect, name="aa"), check_dtype=False)
+#     # DataFrame input
+#     df = pd.DataFrame({"a": value})
+#     assert_frame_equal(
+#         tp.argsort(df, axis=0), pd.DataFrame({"a": expect}), check_dtype=False
+#     )
+
+# # currently only numpy array output is supported
+# def test_ts_func_input():
+#     from pandas.testing import assert_frame_equal, assert_series_equal
+
+#     value, expect = [1, 1, 1], [1.0, 2, 3]
+#     # list input
+#     assert tp.ts_sum(value, 3).tolist() == expect
+#     # series input
+#     sr = pd.Series(value, name="aa")
+#     assert_series_equal(tp.ts_sum(sr, 3), pd.Series(expect, name="aa"))
+#     df = pd.DataFrame({"a": value})
+#     assert_frame_equal(tp.ts_sum(df, 3, axis=0), pd.DataFrame({"a": expect}))
+
+# # currently only numpy array output is supported
+# def test_ts_func2_input():
+#     from pandas.testing import assert_series_equal
+
+#     value1, value2, expect = [1, 2, 3], [1, 2, 3], [np.nan, 1.0, 1.0]
+#     # list input
+#     assert_allclose(tp.ts_corr(value1, value2, 3), np.array(expect))
+#     # series input
+#     sr1, sr2 = pd.Series(value1, name="aa"), pd.Series(value1, name="bb")
+#     assert_series_equal(tp.ts_corr(sr1, sr2, 3), pd.Series(expect, name="aa"))
```

### Comparing `teapy-0.1.2/teapy/tests/window/test_compare.py` & `teapy-0.1.3/teapy/tests/window/test_reg.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,91 @@
 import numpy as np
 import pandas as pd
+import statsmodels.api as sm
 from hypothesis import given
 from hypothesis import strategies as st
 
 import teapy as tp
-from teapy.testing import assert_series_equal, make_arr
+from teapy import Expr
+from teapy.testing import assert_allclose3, make_arr
 
 
-@given(make_arr(30), st.integers(1, 5))
-def test_ts_max(arr, window):
-    # 测试移动最大值
-    arr = pd.Series(arr, copy=False)
-    min_periods = np.random.randint(1, window + 1)
-    res1 = tp.ts_max(arr, window, min_periods=min_periods)
-    res2 = arr.rolling(window, min_periods=min_periods).max()
-    assert_series_equal(res1, res2)
-
+@given(make_arr(30), st.integers(1, 5), st.booleans())
+def test_ts_reg(arr, window, stable):
+    # test moving regression
+    def ts_reg(s):
+        s = s.dropna()
+        if s.size > 1:
+            reg = sm.OLS(s, sm.add_constant(np.arange(s.size) + 1)).fit()
+            return reg.params[0] + reg.params[1] * s.size
+        else:
+            return np.nan
 
-@given(make_arr(30), st.integers(1, 5))
-def test_ts_min(arr, window):
-    # 测试移动最小值
-    arr = pd.Series(arr, copy=False)
+    arr = pd.Series(arr)
     min_periods = np.random.randint(1, window + 1)
-    res1 = tp.ts_min(arr, window, min_periods=min_periods)
-    res2 = arr.rolling(window, min_periods=min_periods).min()
-    assert_series_equal(res1, res2)
+    res1 = tp.ts_reg(arr, window, min_periods=min_periods, stable=stable)
+    res2 = Expr(arr).ts_reg(window, min_periods=min_periods, stable=stable).eview()
+    res3 = arr.rolling(window, min_periods=min_periods).apply(ts_reg)
+    assert_allclose3(res1, res2, res3)
+
+
+@given(make_arr(30), st.integers(1, 5), st.booleans())
+def test_ts_reg_intercept(arr, window, stable):
+    # test moving regression intercept
+    def ts_reg_intercept(s):
+        s = s.dropna()
+        if s.size > 1:
+            reg = sm.OLS(s, sm.add_constant(np.arange(s.size) + 1)).fit()
+            return reg.params[0]
+        else:
+            return np.nan
 
-
-@given(make_arr(30, nan_p=0, unique=True), st.integers(1, 5))
-def test_ts_argmax(arr, window):
-    # 测试移动最大值索引
-    # 对于重复值teapy总是取最后一个，而pandas取的是第一个，因此在无重复值的测试下进行
-    arr = pd.Series(arr, copy=False)
+    arr = pd.Series(arr)
     min_periods = np.random.randint(1, window + 1)
-    res1 = tp.ts_argmax(arr, window, min_periods=min_periods)
-    res2 = arr.rolling(window, min_periods=min_periods).apply(
-        lambda x: x.idxmax() - x.index[0] + 1
+    res1 = tp.ts_reg_intercept(arr, window, min_periods=min_periods, stable=stable)
+    res2 = (
+        Expr(arr)
+        .ts_reg_intercept(window, min_periods=min_periods, stable=stable)
+        .eview()
     )
-    assert_series_equal(res1, res2)
+    res3 = arr.rolling(window, min_periods=min_periods).apply(ts_reg_intercept)
+    assert_allclose3(res1, res2, res3)
+
 
+@given(make_arr(30), st.integers(1, 5), st.booleans())
+def test_ts_reg_slope(arr, window, stable):
+    # test moving regression slope
+    def ts_reg_slope(s):
+        s = s.dropna()
+        if s.size > 1:
+            reg = sm.OLS(s, sm.add_constant(np.arange(s.size) + 1)).fit()
+            return reg.params[1]
+        else:
+            return np.nan
 
-@given(make_arr(30, nan_p=0, unique=True), st.integers(1, 5))
-def test_ts_argmin(arr, window):
-    # 测试移动最小值索引
-    # 对于重复值teapy总是取最后一个，而pandas取的是第一个，在无重复值的测试下进行
-    arr = pd.Series(arr, copy=False)
+    arr = pd.Series(arr)
     min_periods = np.random.randint(1, window + 1)
-    res1 = tp.ts_argmin(arr, window, min_periods=min_periods)
-    res2 = arr.rolling(window, min_periods=min_periods).apply(
-        lambda x: x.idxmin() - x.index[0] + 1
+    res1 = tp.ts_reg_slope(arr, window, min_periods=min_periods, stable=stable)
+    res2 = (
+        Expr(arr).ts_reg_slope(window, min_periods=min_periods, stable=stable).eview()
     )
-    assert_series_equal(res1, res2)
+    res3 = arr.rolling(window, min_periods=min_periods).apply(ts_reg_slope)
+    assert_allclose3(res1, res2, res3)
 
 
-@given(make_arr(30, nan_p=0, unique=True), st.integers(1, 5))
-def test_ts_rank(arr, window):
-    # 测试移动排名
-    # 对于重复值teapy总是取最后一个，而pandas取的是第一个，在无重复值的测试下进行
-    arr = pd.Series(arr, copy=False)
-    min_periods = np.random.randint(1, window + 1)
-    res1 = tp.ts_rank(arr, window, min_periods=min_periods)
-    res2 = arr.rolling(window, min_periods=min_periods).apply(
-        lambda x: x.rank().iloc[-1]
-    )
-    assert_series_equal(res1, res2)
+@given(make_arr(30), st.integers(1, 5), st.booleans())
+def test_ts_tsf(arr, window, stable):
+    # test moving time series forecast
+    def ts_tsf(s):
+        s = s.dropna()
+        if s.size > 1:
+            reg = sm.OLS(s, sm.add_constant(np.arange(s.size) + 1)).fit()
+            return reg.params[0] + reg.params[1] * (s.size + 1)
+        else:
+            return np.nan
 
-    # rank pct
-    res3 = tp.ts_rank(arr, window, pct=True, min_periods=min_periods)
-    res4 = arr.rolling(window, min_periods=min_periods).apply(
-        lambda x: x.rank(pct=True).iloc[-1]
-    )
-    assert_series_equal(res3, res4)
+    arr = pd.Series(arr)
+    min_periods = np.random.randint(1, window + 1)
+    res1 = tp.ts_tsf(arr, window, min_periods=min_periods, stable=stable)
+    res2 = Expr(arr).ts_tsf(window, min_periods=min_periods, stable=stable).eview()
+    res3 = arr.rolling(window, min_periods=min_periods).apply(ts_tsf)
+    assert_allclose3(res1, res2, res3)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `teapy-0.1.2/teapy/tests/window/test_norm.py` & `teapy-0.1.3/teapy/tests/window/test_norm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 import numpy as np
 import pandas as pd
 from hypothesis import given
 from hypothesis import strategies as st
 
 import teapy as tp
-from teapy.testing import assert_series_equal, make_arr
+from teapy import Expr
+from teapy.testing import assert_allclose3, make_arr
 
 
 @given(make_arr(30, unique=True, stable=True), st.integers(1, 5), st.booleans())
 def test_ts_stable(arr, window, stable):
-    # 测试移动stable标准化
+    # test moving stable
     arr = pd.Series(arr, copy=False)
     min_periods = np.random.randint(1, window + 1)
     res1 = tp.ts_stable(arr, window, min_periods=min_periods, stable=stable)
-    res2 = arr.rolling(window, min_periods=min_periods).apply(
+    res2 = Expr(arr).ts_stable(window, min_periods=min_periods, stable=stable).eview()
+    res3 = arr.rolling(window, min_periods=min_periods).apply(
         lambda x: x.mean() / x.std() if x.std() != 0 else np.nan
     )
-    assert_series_equal(res1, res2)
+    assert_allclose3(res1, res2, res3)
 
 
 @given(make_arr(30, unique=True, stable=True), st.integers(1, 5), st.booleans())
 def test_ts_meanstdnorm(arr, window, stable):
-    # 测试移动meanstd标准化
+    # test moving meanstd normalization
     arr = pd.Series(arr, copy=False)
     min_periods = np.random.randint(1, window + 1)
     res1 = tp.ts_meanstdnorm(arr, window, min_periods=min_periods, stable=stable)
-    res2 = arr.rolling(window, min_periods=min_periods).apply(
+    res2 = (
+        Expr(arr).ts_meanstdnorm(window, min_periods=min_periods, stable=stable).eview()
+    )
+    res3 = arr.rolling(window, min_periods=min_periods).apply(
         lambda x: (x.iloc[-1] - x.mean()) / x.std() if x.std() != 0 else np.nan
     )
-    assert_series_equal(res1, res2)
+    assert_allclose3(res1, res2, res3)
 
 
 @given(make_arr(50, unique=True), st.integers(1, 5))
 def test_ts_minmaxnorm(arr, window):
-    # 测试移动minmax标准化
+    # test moving minmax normalization
     arr = pd.Series(arr, copy=False)
     min_periods = np.random.randint(1, window + 1)
     res1 = tp.ts_minmaxnorm(arr, window, min_periods=min_periods)
-    res2 = arr.rolling(window, min_periods=min_periods).apply(
+    res2 = Expr(arr).ts_minmaxnorm(window, min_periods=min_periods).eview()
+    res3 = arr.rolling(window, min_periods=min_periods).apply(
         lambda x: (x.iloc[-1] - x.min()) / (x.max() - x.min())
         if x.max() != x.min()
         else np.nan
     )
-    assert_series_equal(res1, res2)
+    assert_allclose3(res1, res2, res3)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `teapy-0.1.2/teapy/window_func.py` & `teapy-0.1.3/teapy/window_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.2/teapy/wrapper.py` & `teapy-0.1.3/teapy/wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,43 @@
 
 from . import teapy as _tp
 from .converter import Converter
 
 __all__ = ["wrap"]
 
 
+def default_wrapper(func):
+    @wraps(func)
+    def _wrapper(arr, *args, **kwargs):
+        func_name = f"{func.__name__}"
+        return getattr(_tp.PyExpr(arr), func_name)(*args, **kwargs).value()
+
+    return _wrapper
+
+
+def default_wrapper2(func):
+    @wraps(func)
+    def _wrapper(arr1, arr2, *args, **kwargs):
+        func_name = f"{func.__name__}"
+        return getattr(_tp.PyExpr(arr1), func_name)(
+            _tp.PyExpr(arr2), *args, **kwargs
+        ).value()
+
+    return _wrapper
+
+
+def impl_by_lazy(func_type: str = "default"):
+    if func_type == "default":
+        return default_wrapper
+    elif func_type == "default2":
+        return default_wrapper2
+    else:
+        raise ValueError("Not support func_type: %s" % func_type)
+
+
 def inplace_wrapper(func):
     @wraps(func)
     def _wrapper(*args, inplace=False, **kwargs):
         func_name = f"{func.__name__}" + "_inplace" if inplace else f"{func.__name__}"
         return getattr(_tp, func_name)(*args, **kwargs)
 
     return _wrapper
```

### Comparing `teapy-0.1.2/Cargo.lock` & `teapy-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1410,15 +1410,15 @@
 name = "target-lexicon"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
 
 [[package]]
 name = "teapy"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "ahash",
  "chrono",
  "cxx",
  "lapack-sys",
  "ndarray",
  "ndarray-linalg",
```

### Comparing `teapy-0.1.2/PKG-INFO` & `teapy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teapy
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: numpy>=1.16.0
 License-File: LICENSE
 Summary: A blazingly fast datadict library
 Author-email: Teamon <teamon9161@163.com>
```

