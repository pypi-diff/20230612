# Comparing `tmp/teapy-0.1.3.tar.gz` & `tmp/teapy-0.1.4.tar.gz`

## Comparing `teapy-0.1.3.tar` & `teapy-0.1.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 teapy-0.1.3/Cargo.toml
--rw-r--r--   0     1001      123      891 2023-06-12 04:50:58.000000 teapy-0.1.3/.github/workflows/build.yaml
--rw-r--r--   0     1001      123     1097 2023-06-12 04:50:58.000000 teapy-0.1.3/.github/workflows/coverage.yaml
--rw-r--r--   0     1001      123     3240 2023-06-12 04:50:58.000000 teapy-0.1.3/.github/workflows/release_python.yaml
--rw-r--r--   0     1001      123     1280 2023-06-12 04:50:58.000000 teapy-0.1.3/.github/workflows/test_python.yaml
--rw-r--r--   0     1001      123      105 2023-06-12 04:50:58.000000 teapy-0.1.3/.gitignore
--rw-r--r--   0     1001      123     1049 2023-06-12 04:50:58.000000 teapy-0.1.3/LICENSE
--rw-r--r--   0     1001      123     1272 2023-06-12 04:50:58.000000 teapy-0.1.3/Makefile
--rw-r--r--   0     1001      123      441 2023-06-12 04:50:58.000000 teapy-0.1.3/README.md
--rw-r--r--   0     1001      123      195 2023-06-12 04:50:58.000000 teapy-0.1.3/build.requirements.txt
--rw-r--r--   0     1001      123      462 2023-06-12 04:50:58.000000 teapy-0.1.3/pyproject.toml
--rwxr-xr-x   0     1001      123      850 2023-06-12 04:51:27.000000 teapy-0.1.3/run-maturin-action.sh
--rw-r--r--   0     1001      123    13986 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/agg.rs
--rw-r--r--   0     1001      123    31986 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/arr_func.rs
--rw-r--r--   0     1001      123     4672 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/corr.rs
--rw-r--r--   0     1001      123     8363 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/datatype.rs
--rw-r--r--   0     1001      123      548 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/export.rs
--rw-r--r--   0     1001      123     9128 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/groupby.rs
--rw-r--r--   0     1001      123    15524 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/impls/impl_1d_method.rs
--rw-r--r--   0     1001      123     5221 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/impls/impl_linalg.rs
--rw-r--r--   0     1001      123    10397 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/impls/impl_method.rs
--rw-r--r--   0     1001      123     6606 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/impls/impl_numeric.rs
--rw-r--r--   0     1001      123     3399 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/impls/impl_traits.rs
--rw-r--r--   0     1001      123      114 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/impls/mod.rs
--rw-r--r--   0     1001      123    10337 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/iterators.rs
--rw-r--r--   0     1001      123     2886 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/join.rs
--rw-r--r--   0     1001      123     4835 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/auto_impl_own.rs
--rw-r--r--   0     1001      123     3247 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/expr_view.rs
--rw-r--r--   0     1001      123    14759 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/exprs.rs
--rw-r--r--   0     1001      123     1570 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/impl_cmp.rs
--rw-r--r--   0     1001      123      397 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/impl_mut.rs
--rw-r--r--   0     1001      123     2800 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/impl_ops.rs
--rw-r--r--   0     1001      123    25019 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/impl_own.rs
--rw-r--r--   0     1001      123    10697 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/impl_view.rs
--rw-r--r--   0     1001      123     8918 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/linalg.rs
--rw-r--r--   0     1001      123    41157 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/mod.rs
--rw-r--r--   0     1001      123    40512 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/lazy/mod_test.rs
--rw-r--r--   0     1001      123    11490 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/macros.rs
--rw-r--r--   0     1001      123    21693 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/mod.rs
--rw-r--r--   0     1001      123      451 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/option_datetype.rs
--rw-r--r--   0     1001      123    11108 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/time.rs
--rw-r--r--   0     1001      123     1618 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/util_trait.rs
--rw-r--r--   0     1001      123     3680 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/utils/algos.rs
--rw-r--r--   0     1001      123     1746 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/utils/alloc.rs
--rw-r--r--   0     1001      123      195 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/utils/default_new.rs
--rw-r--r--   0     1001      123      185 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/utils/mod.rs
--rw-r--r--   0     1001      123    13468 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/window/compare.rs
--rw-r--r--   0     1001      123     6390 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/window/corr.rs
--rw-r--r--   0     1001      123    24023 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/window/feature.rs
--rw-r--r--   0     1001      123       75 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/window/mod.rs
--rw-r--r--   0     1001      123     9226 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/window/norm.rs
--rw-r--r--   0     1001      123    12965 2023-06-12 04:50:58.000000 teapy-0.1.3/src/arr/window/reg.rs
--rw-r--r--   0     1001      123     4974 2023-06-12 04:50:58.000000 teapy-0.1.3/src/eager_api.rs
--rw-r--r--   0     1001      123     2769 2023-06-12 04:50:58.000000 teapy-0.1.3/src/eager_macros.rs
--rw-r--r--   0     1001      123     9340 2023-06-12 04:50:58.000000 teapy-0.1.3/src/equity.rs
--rw-r--r--   0     1001      123     8298 2023-06-12 04:50:58.000000 teapy-0.1.3/src/from_py.rs
--rw-r--r--   0     1001      123     1113 2023-06-12 04:50:58.000000 teapy-0.1.3/src/lib.rs
--rw-r--r--   0     1001      123    37387 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/datadict.rs
--rw-r--r--   0     1001      123      530 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/export.rs
--rw-r--r--   0     1001      123     2628 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/groupby.rs
--rw-r--r--   0     1001      123    85968 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/impl_pyexpr.rs
--rw-r--r--   0     1001      123     1200 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/mod.rs
--rw-r--r--   0     1001      123    19759 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/pyexpr.rs
--rw-r--r--   0     1001      123    15098 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/pyfunc.rs
--rw-r--r--   0     1001      123      454 2023-06-12 04:50:58.000000 teapy-0.1.3/src/pylazy/time.rs
--rw-r--r--   0     1001      123      388 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/__init__.py
--rw-r--r--   0     1001      123     5452 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/array_func.py
--rw-r--r--   0     1001      123     3184 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/converter.py
--rw-r--r--   0     1001      123     4264 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/datadict.py
--rw-r--r--   0     1001      123     6985 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/regression.py
--rw-r--r--   0     1001      123     3440 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/testing.py
--rw-r--r--   0     1001      123     9870 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/test_array_func.py
--rw-r--r--   0     1001      123     3380 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/test_common.py
--rw-r--r--   0     1001      123     3211 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/window/test_compare.py
--rw-r--r--   0     1001      123     1418 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/window/test_corr.py
--rw-r--r--   0     1001      123     5772 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/window/test_feature.py
--rw-r--r--   0     1001      123     1995 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/window/test_norm.py
--rw-r--r--   0     1001      123     3165 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/tests/window/test_reg.py
--rw-r--r--   0     1001      123     3660 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/window_func.py
--rw-r--r--   0     1001      123     5751 2023-06-12 04:50:58.000000 teapy-0.1.3/teapy/wrapper.py
--rw-r--r--   0     1001      123    44634 2023-06-12 04:50:58.000000 teapy-0.1.3/Cargo.lock
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 teapy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 teapy-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      123      891 2023-06-12 05:39:07.000000 teapy-0.1.4/.github/workflows/build.yaml
+-rw-r--r--   0     1001      123     1097 2023-06-12 05:39:07.000000 teapy-0.1.4/.github/workflows/coverage.yaml
+-rw-r--r--   0     1001      123     3284 2023-06-12 05:39:07.000000 teapy-0.1.4/.github/workflows/release_python.yaml
+-rw-r--r--   0     1001      123     1280 2023-06-12 05:39:07.000000 teapy-0.1.4/.github/workflows/test_python.yaml
+-rw-r--r--   0     1001      123      105 2023-06-12 05:39:07.000000 teapy-0.1.4/.gitignore
+-rw-r--r--   0     1001      123     1049 2023-06-12 05:39:07.000000 teapy-0.1.4/LICENSE
+-rw-r--r--   0     1001      123     1272 2023-06-12 05:39:07.000000 teapy-0.1.4/Makefile
+-rw-r--r--   0     1001      123      441 2023-06-12 05:39:07.000000 teapy-0.1.4/README.md
+-rw-r--r--   0     1001      123      195 2023-06-12 05:39:07.000000 teapy-0.1.4/build.requirements.txt
+-rw-r--r--   0     1001      123      462 2023-06-12 05:39:07.000000 teapy-0.1.4/pyproject.toml
+-rwxr-xr-x   0     1001      123      850 2023-06-12 05:39:36.000000 teapy-0.1.4/run-maturin-action.sh
+-rw-r--r--   0     1001      123    13986 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/agg.rs
+-rw-r--r--   0     1001      123    31986 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/arr_func.rs
+-rw-r--r--   0     1001      123     4672 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/corr.rs
+-rw-r--r--   0     1001      123     8363 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/datatype.rs
+-rw-r--r--   0     1001      123      548 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/export.rs
+-rw-r--r--   0     1001      123     9128 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/groupby.rs
+-rw-r--r--   0     1001      123    15524 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/impls/impl_1d_method.rs
+-rw-r--r--   0     1001      123     5221 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/impls/impl_linalg.rs
+-rw-r--r--   0     1001      123    10397 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/impls/impl_method.rs
+-rw-r--r--   0     1001      123     6606 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/impls/impl_numeric.rs
+-rw-r--r--   0     1001      123     3399 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/impls/impl_traits.rs
+-rw-r--r--   0     1001      123      114 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/impls/mod.rs
+-rw-r--r--   0     1001      123    10337 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/iterators.rs
+-rw-r--r--   0     1001      123     2886 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/join.rs
+-rw-r--r--   0     1001      123     4835 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/auto_impl_own.rs
+-rw-r--r--   0     1001      123     3247 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/expr_view.rs
+-rw-r--r--   0     1001      123    14759 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/exprs.rs
+-rw-r--r--   0     1001      123     1570 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/impl_cmp.rs
+-rw-r--r--   0     1001      123      397 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/impl_mut.rs
+-rw-r--r--   0     1001      123     2800 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/impl_ops.rs
+-rw-r--r--   0     1001      123    25019 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/impl_own.rs
+-rw-r--r--   0     1001      123    10697 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/impl_view.rs
+-rw-r--r--   0     1001      123     8918 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/linalg.rs
+-rw-r--r--   0     1001      123    41157 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/mod.rs
+-rw-r--r--   0     1001      123    40512 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/mod_test.rs
+-rw-r--r--   0     1001      123    11490 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/macros.rs
+-rw-r--r--   0     1001      123    21693 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/mod.rs
+-rw-r--r--   0     1001      123      451 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/option_datetype.rs
+-rw-r--r--   0     1001      123    11108 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/time.rs
+-rw-r--r--   0     1001      123     1618 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/util_trait.rs
+-rw-r--r--   0     1001      123     3680 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/utils/algos.rs
+-rw-r--r--   0     1001      123     1746 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/utils/alloc.rs
+-rw-r--r--   0     1001      123      195 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/utils/default_new.rs
+-rw-r--r--   0     1001      123      185 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/utils/mod.rs
+-rw-r--r--   0     1001      123    13468 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/window/compare.rs
+-rw-r--r--   0     1001      123     6390 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/window/corr.rs
+-rw-r--r--   0     1001      123    24023 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/window/feature.rs
+-rw-r--r--   0     1001      123       75 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/window/mod.rs
+-rw-r--r--   0     1001      123     9226 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/window/norm.rs
+-rw-r--r--   0     1001      123    12965 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/window/reg.rs
+-rw-r--r--   0     1001      123     4974 2023-06-12 05:39:07.000000 teapy-0.1.4/src/eager_api.rs
+-rw-r--r--   0     1001      123     2769 2023-06-12 05:39:07.000000 teapy-0.1.4/src/eager_macros.rs
+-rw-r--r--   0     1001      123     9340 2023-06-12 05:39:07.000000 teapy-0.1.4/src/equity.rs
+-rw-r--r--   0     1001      123     8298 2023-06-12 05:39:07.000000 teapy-0.1.4/src/from_py.rs
+-rw-r--r--   0     1001      123     1113 2023-06-12 05:39:07.000000 teapy-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      123    37387 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/datadict.rs
+-rw-r--r--   0     1001      123      530 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/export.rs
+-rw-r--r--   0     1001      123     2628 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/groupby.rs
+-rw-r--r--   0     1001      123    85968 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/impl_pyexpr.rs
+-rw-r--r--   0     1001      123     1200 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/mod.rs
+-rw-r--r--   0     1001      123    19759 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/pyexpr.rs
+-rw-r--r--   0     1001      123    15098 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/pyfunc.rs
+-rw-r--r--   0     1001      123      454 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/time.rs
+-rw-r--r--   0     1001      123      388 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/__init__.py
+-rw-r--r--   0     1001      123     5452 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/array_func.py
+-rw-r--r--   0     1001      123     3184 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/converter.py
+-rw-r--r--   0     1001      123     4264 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/datadict.py
+-rw-r--r--   0     1001      123     6985 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/regression.py
+-rw-r--r--   0     1001      123     3440 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/testing.py
+-rw-r--r--   0     1001      123     9870 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      123     3380 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/test_common.py
+-rw-r--r--   0     1001      123     3211 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      123     1418 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      123     5772 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      123     1995 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      123     3165 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      123     3660 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/window_func.py
+-rw-r--r--   0     1001      123     5751 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/wrapper.py
+-rw-r--r--   0     1001      123    44634 2023-06-12 05:39:07.000000 teapy-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 teapy-0.1.4/PKG-INFO
```

### Comparing `teapy-0.1.3/Cargo.toml` & `teapy-0.1.4/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "teapy"
-version = "0.1.3"
+version = "0.1.4"
 edition = "2021"
 
 [lib]
 name = "teapy"
 crate-type = ["cdylib", "rlib"]
 
 [features]
```

### Comparing `teapy-0.1.3/.github/workflows/build.yaml` & `teapy-0.1.4/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/.github/workflows/coverage.yaml` & `teapy-0.1.4/.github/workflows/coverage.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/.github/workflows/release_python.yaml` & `teapy-0.1.4/.github/workflows/release_python.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -71,23 +71,23 @@
     runs-on: macos-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.8'
 
-
       - name: Set up Rust targets
         run: rustup target add aarch64-apple-darwin
 
       - name: Publish wheel
         uses: messense/maturin-action@v1
         env:
           MATURIN_PASSWORD: ${{ secrets.PYPI_SECRET }}
         with:
+          rust-toolchain: nightly-2023-01-19
           maturin-version: '0.14.10'
           command: publish
           args: --target aarch64-apple-darwin --skip-existing --no-sdist -o wheels -i python -u teamon
 
 
   # # the dependency of ndarry-linalg crate can not be build on manylinux-arrch64 currently
```

### Comparing `teapy-0.1.3/.github/workflows/test_python.yaml` & `teapy-0.1.4/.github/workflows/test_python.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/LICENSE` & `teapy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/Makefile` & `teapy-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/run-maturin-action.sh` & `teapy-0.1.4/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/agg.rs` & `teapy-0.1.4/src/arr/agg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/arr_func.rs` & `teapy-0.1.4/src/arr/arr_func.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/corr.rs` & `teapy-0.1.4/src/arr/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/datatype.rs` & `teapy-0.1.4/src/arr/datatype.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/export.rs` & `teapy-0.1.4/src/arr/export.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/groupby.rs` & `teapy-0.1.4/src/arr/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/impls/impl_1d_method.rs` & `teapy-0.1.4/src/arr/impls/impl_1d_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/impls/impl_linalg.rs` & `teapy-0.1.4/src/arr/impls/impl_linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/impls/impl_method.rs` & `teapy-0.1.4/src/arr/impls/impl_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/impls/impl_numeric.rs` & `teapy-0.1.4/src/arr/impls/impl_numeric.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/impls/impl_traits.rs` & `teapy-0.1.4/src/arr/impls/impl_traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/iterators.rs` & `teapy-0.1.4/src/arr/iterators.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/join.rs` & `teapy-0.1.4/src/arr/join.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/lazy/auto_impl_own.rs` & `teapy-0.1.4/src/arr/lazy/auto_impl_own.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/lazy/expr_view.rs` & `teapy-0.1.4/src/arr/lazy/expr_view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/lazy/exprs.rs` & `teapy-0.1.4/src/arr/lazy/exprs.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/lazy/impl_cmp.rs` & `teapy-0.1.4/src/arr/lazy/impl_cmp.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/lazy/impl_ops.rs` & `teapy-0.1.4/src/arr/lazy/impl_ops.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/lazy/impl_own.rs` & `teapy-0.1.4/src/arr/lazy/impl_own.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/lazy/impl_view.rs` & `teapy-0.1.4/src/arr/lazy/impl_view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/lazy/linalg.rs` & `teapy-0.1.4/src/arr/lazy/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/lazy/mod.rs` & `teapy-0.1.4/src/arr/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/lazy/mod_test.rs` & `teapy-0.1.4/src/arr/lazy/mod_test.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/macros.rs` & `teapy-0.1.4/src/arr/macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/mod.rs` & `teapy-0.1.4/src/arr/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/time.rs` & `teapy-0.1.4/src/arr/time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/util_trait.rs` & `teapy-0.1.4/src/arr/util_trait.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/utils/algos.rs` & `teapy-0.1.4/src/arr/utils/algos.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/utils/alloc.rs` & `teapy-0.1.4/src/arr/utils/alloc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/window/compare.rs` & `teapy-0.1.4/src/arr/window/compare.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/window/corr.rs` & `teapy-0.1.4/src/arr/window/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/window/feature.rs` & `teapy-0.1.4/src/arr/window/feature.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/window/norm.rs` & `teapy-0.1.4/src/arr/window/norm.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/arr/window/reg.rs` & `teapy-0.1.4/src/arr/window/reg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/eager_api.rs` & `teapy-0.1.4/src/eager_api.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/eager_macros.rs` & `teapy-0.1.4/src/eager_macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/equity.rs` & `teapy-0.1.4/src/equity.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/from_py.rs` & `teapy-0.1.4/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/lib.rs` & `teapy-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/pylazy/datadict.rs` & `teapy-0.1.4/src/pylazy/datadict.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/pylazy/export.rs` & `teapy-0.1.4/src/pylazy/export.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/pylazy/groupby.rs` & `teapy-0.1.4/src/pylazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/pylazy/impl_pyexpr.rs` & `teapy-0.1.4/src/pylazy/impl_pyexpr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/pylazy/mod.rs` & `teapy-0.1.4/src/pylazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/pylazy/pyexpr.rs` & `teapy-0.1.4/src/pylazy/pyexpr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/src/pylazy/pyfunc.rs` & `teapy-0.1.4/src/pylazy/pyfunc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/array_func.py` & `teapy-0.1.4/teapy/array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/converter.py` & `teapy-0.1.4/teapy/converter.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/datadict.py` & `teapy-0.1.4/teapy/datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/regression.py` & `teapy-0.1.4/teapy/regression.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/testing.py` & `teapy-0.1.4/teapy/testing.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/tests/test_array_func.py` & `teapy-0.1.4/teapy/tests/test_array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/tests/test_common.py` & `teapy-0.1.4/teapy/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/tests/window/test_compare.py` & `teapy-0.1.4/teapy/tests/window/test_compare.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/tests/window/test_corr.py` & `teapy-0.1.4/teapy/tests/window/test_corr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/tests/window/test_feature.py` & `teapy-0.1.4/teapy/tests/window/test_feature.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/tests/window/test_norm.py` & `teapy-0.1.4/teapy/tests/window/test_norm.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/tests/window/test_reg.py` & `teapy-0.1.4/teapy/tests/window/test_reg.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/window_func.py` & `teapy-0.1.4/teapy/window_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/teapy/wrapper.py` & `teapy-0.1.4/teapy/wrapper.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.3/Cargo.lock` & `teapy-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1410,15 +1410,15 @@
 name = "target-lexicon"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
 
 [[package]]
 name = "teapy"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "ahash",
  "chrono",
  "cxx",
  "lapack-sys",
  "ndarray",
  "ndarray-linalg",
```

### Comparing `teapy-0.1.3/PKG-INFO` & `teapy-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teapy
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: numpy>=1.16.0
 License-File: LICENSE
 Summary: A blazingly fast datadict library
 Author-email: Teamon <teamon9161@163.com>
```

