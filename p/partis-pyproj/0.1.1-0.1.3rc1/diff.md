# Comparing `tmp/partis_pyproj-0.1.1.tar.gz` & `tmp/partis_pyproj-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Nov 15 22:18:25 2022, max compression
+gzip compressed data, last modified: Mon Jun 12 16:28:09 2023, max compression
```

## Comparing `partis_pyproj-0.1.1.tar` & `partis_pyproj-0.1.3rc1.tar`

### file list

```diff
@@ -1,116 +1,118 @@
--rw-r--r--   0        0        0     1418 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/__init__.py
--rw-r--r--   0        0        0    10862 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/norms.py
--rw-r--r--   0        0        0    32658 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/pep.py
--rw-r--r--   0        0        0       80 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/builder/__init__.py
--rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/builder/builder.py
--rw-r--r--   0        0        0     2387 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/builder/cmake.py
--rw-r--r--   0        0        0     2387 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/builder/meson.py
--rw-r--r--   0        0        0     4321 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/load_module.py
--rw-r--r--   0        0        0     5306 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/_legacy_setup.py
--rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/_nonprintable.py
--rw-r--r--   0        0        0      226 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/path/__init__.py
--rw-r--r--   0        0        0    11677 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/path/match.py
--rw-r--r--   0        0        0    15634 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/path/pattern.py
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/path/utils.py
--rw-r--r--   0        0        0    31148 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/validate.py
--rw-r--r--   0        0        0    15250 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/pkginfo.py
--rw-r--r--   0        0        0     3922 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/dist_file/dist_targz.py
--rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/dist_file/__init__.py
--rw-r--r--   0        0        0     3887 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/dist_file/dist_zip.py
--rw-r--r--   0        0        0     7816 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/dist_file/dist_binary.py
--rw-r--r--   0        0        0    12086 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/dist_file/dist_base.py
--rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/dist_file/dist_source.py
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/dist_file/dist_copy.py
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/legacy.py
--rw-r--r--   0        0        0     6686 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/backend.py
--rw-r--r--   0        0        0    11864 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/pyproj.py
--rw-r--r--   0        0        0    12612 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/src/pyproj/pptoml.py
--rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/conf.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/__init__.py
--rw-r--r--   0        0        0    21545 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/index.rst
--rw-r--r--   0        0        0      138 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/src/pptoml.rst
--rw-r--r--   0        0        0      172 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/src/index.rst
--rw-r--r--   0        0        0      133 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/src/backend.rst
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/src/builder.rst
--rw-r--r--   0        0        0      142 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/src/validate.rst
--rw-r--r--   0        0        0      341 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/src/pkginfo.rst
--rw-r--r--   0        0        0      116 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/src/pyproj.rst
--rw-r--r--   0        0        0      209 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/src/path.rst
--rw-r--r--   0        0        0      115 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/src/pep.rst
--rw-r--r--   0        0        0      150 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/src/load_module.rst
--rw-r--r--   0        0        0      131 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/src/norms.rst
--rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/src/dist_file.rst
--rw-r--r--   0        0        0      417 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/__main__.py
--rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/doc/glossary.rst
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_5/src/test_pkg/sub_mod/sub_sub_mod/good_file.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_5/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_5/src/test_pkg/pure_mod/pure_mod.py
--rw-r--r--   0        0        0      488 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_5/pkgaux/__init__.py
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_5/pyproject.toml
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/__init__.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_2/src/test_pkg/pure_mod.py
--rw-r--r--   0        0        0      111 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_2/src/test_pkg/plat_mod.pyx
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_2/meson.build
--rw-r--r--   0        0        0      161 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_2/meson_options.txt
--rw-r--r--   0        0        0     1672 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_2/pyproject.toml
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_2/src/test_pkg/sub_mod/sub_sub_mod/good_file.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_2/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_2/src/test_pkg/pure_mod/pure_mod.py
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_2/pkgaux/__init__.py
--rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_2/pyproject.toml
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/__main__.py
--rw-r--r--   0        0        0     7942 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/test_03_dist.py
--rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/sitecustom/partis-sitecustom.pth
--rw-r--r--   0        0        0      375 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/sitecustom/pyproject.toml
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_bad_1/bad_link/src/test_pkg/pure_mod.py
--rw-r--r--   0        0        0      111 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_bad_1/bad_link/src/test_pkg/plat_mod.pyx
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_bad_1/bad_link/meson.build
--rw-r--r--   0        0        0      161 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_bad_1/bad_link/meson_options.txt
--rw-r--r--   0        0        0     1652 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_bad_1/bad_link/pyproject.toml
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_bad_1/src/test_pkg/pure_mod.py
--rw-r--r--   0        0        0      111 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_bad_1/src/test_pkg/plat_mod.pyx
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_bad_1/meson.build
--rw-r--r--   0        0        0      161 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_bad_1/meson_options.txt
--rw-r--r--   0        0        0     1676 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_bad_1/pyproject.toml
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_min/pure_mod.py
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_min/pyproject.toml
--rw-r--r--   0        0        0     3266 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/noxfile.py
--rw-r--r--   0        0        0     9605 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/test_00_validate.py
--rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/test_04_load_module.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_cmake_1/src/test_pkg/pure_mod.py
--rw-r--r--   0        0        0      111 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_cmake_1/src/test_pkg/plat_mod.pyx
--rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_cmake_1/src/test_pkg/CMakeLists.txt
--rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_cmake_1/CMakeLists.txt
--rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_cmake_1/pyproject.toml
--rw-r--r--   0        0        0    12276 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/test_01_norms.py
--rw-r--r--   0        0        0     5163 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/test_05_pkginfo.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_base/src/test_pkg/sub_mod/sub_sub_mod/good_file.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_base/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_base/src/test_pkg/sub_mod/good_file.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_base/src/test_pkg/sub_mod/bad_file.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_base/src/test_pkg/pure_mod/pure_mod.py
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_base/pkgaux/__init__.py
--rw-r--r--   0        0        0     1970 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_base/pyproject.toml
--rw-r--r--   0        0        0     6769 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/test_06_pyproj.py
--rw-r--r--   0        0        0     7554 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/test_02_path.py
--rw-r--r--   0        0        0      764 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_3/pyproject.toml
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_1/src/test_pkg/pure_mod.py
--rw-r--r--   0        0        0      111 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_1/src/test_pkg/plat_mod.pyx
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_1/meson.build
--rw-r--r--   0        0        0      161 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_1/meson_options.txt
--rw-r--r--   0        0        0     1652 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_meson_1/pyproject.toml
--rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/test_07_backend.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_4/src/test_pkg/sub_mod/sub_sub_mod/good_file.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_4/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_4/src/test_pkg/pure_mod/pure_mod.py
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_4/pkgaux/__init__.py
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_4/pyproject.toml
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_1/src/test_pkg/sub_mod/sub_sub_mod/good_file.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_1/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_1/src/test_pkg/pure_mod/pure_mod.py
--rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/test/pkg_bad_1/pyproject.toml
--rw-r--r--   0        0        0     6609 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      163 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/README.rst
--rw-r--r--   0        0        0    14341 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/setup.py
--rw-r--r--   0        0        0     2107 1970-01-01 00:00:00.000000 partis_pyproj-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/__init__.py
+-rw-r--r--   0        0        0    10862 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/norms.py
+-rw-r--r--   0        0        0    32658 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/pep.py
+-rw-r--r--   0        0        0      133 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/builder/__init__.py
+-rw-r--r--   0        0        0     4354 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/builder/builder.py
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/builder/cargo.py
+-rw-r--r--   0        0        0     2133 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/builder/cmake.py
+-rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/builder/meson.py
+-rw-r--r--   0        0        0     1878 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/builder/process.py
+-rw-r--r--   0        0        0     4305 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/load_module.py
+-rw-r--r--   0        0        0     5306 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/_legacy_setup.py
+-rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/_nonprintable.py
+-rw-r--r--   0        0        0      226 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/path/__init__.py
+-rw-r--r--   0        0        0    11677 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/path/match.py
+-rw-r--r--   0        0        0    15634 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/path/pattern.py
+-rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/path/utils.py
+-rw-r--r--   0        0        0    32324 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/validate.py
+-rw-r--r--   0        0        0    15250 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/pkginfo.py
+-rw-r--r--   0        0        0     3922 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_targz.py
+-rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/dist_file/__init__.py
+-rw-r--r--   0        0        0     3887 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_zip.py
+-rw-r--r--   0        0        0     7816 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_binary.py
+-rw-r--r--   0        0        0    12086 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_base.py
+-rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_source.py
+-rw-r--r--   0        0        0     3627 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_copy.py
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/legacy.py
+-rw-r--r--   0        0        0     6686 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/backend.py
+-rw-r--r--   0        0        0    12194 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/pyproj.py
+-rw-r--r--   0        0        0    13397 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/src/pyproj/pptoml.py
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/conf.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/__init__.py
+-rw-r--r--   0        0        0    21545 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/index.rst
+-rw-r--r--   0        0        0      138 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/src/pptoml.rst
+-rw-r--r--   0        0        0      172 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/src/index.rst
+-rw-r--r--   0        0        0      133 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/src/backend.rst
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/src/builder.rst
+-rw-r--r--   0        0        0      142 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/src/validate.rst
+-rw-r--r--   0        0        0      341 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/src/pkginfo.rst
+-rw-r--r--   0        0        0      116 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/src/pyproj.rst
+-rw-r--r--   0        0        0      209 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/src/path.rst
+-rw-r--r--   0        0        0      115 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/src/pep.rst
+-rw-r--r--   0        0        0      150 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/src/load_module.rst
+-rw-r--r--   0        0        0      131 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/src/norms.rst
+-rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/src/dist_file.rst
+-rw-r--r--   0        0        0      417 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/__main__.py
+-rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/doc/glossary.rst
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_5/src/test_pkg/sub_mod/sub_sub_mod/good_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_5/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_5/src/test_pkg/pure_mod/pure_mod.py
+-rw-r--r--   0        0        0      488 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_5/pkgaux/__init__.py
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_5/pyproject.toml
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/__init__.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_2/src/test_pkg/pure_mod.py
+-rw-r--r--   0        0        0      111 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_2/src/test_pkg/plat_mod.pyx
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_2/meson.build
+-rw-r--r--   0        0        0      161 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_2/meson_options.txt
+-rw-r--r--   0        0        0     1652 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_2/pyproject.toml
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_2/src/test_pkg/sub_mod/sub_sub_mod/good_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_2/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_2/src/test_pkg/pure_mod/pure_mod.py
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_2/pkgaux/__init__.py
+-rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_2/pyproject.toml
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/__main__.py
+-rw-r--r--   0        0        0     7942 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/test_03_dist.py
+-rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/sitecustom/partis-sitecustom.pth
+-rw-r--r--   0        0        0      375 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/sitecustom/pyproject.toml
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/bad_link/src/test_pkg/pure_mod.py
+-rw-r--r--   0        0        0      111 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/bad_link/src/test_pkg/plat_mod.pyx
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/bad_link/meson.build
+-rw-r--r--   0        0        0      161 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/bad_link/meson_options.txt
+-rw-r--r--   0        0        0     1652 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/bad_link/pyproject.toml
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/src/test_pkg/pure_mod.py
+-rw-r--r--   0        0        0      111 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/src/test_pkg/plat_mod.pyx
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/meson.build
+-rw-r--r--   0        0        0      161 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/meson_options.txt
+-rw-r--r--   0        0        0     1676 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/pyproject.toml
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_min/pure_mod.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_min/pyproject.toml
+-rw-r--r--   0        0        0     3266 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/noxfile.py
+-rw-r--r--   0        0        0    10191 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/test_00_validate.py
+-rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/test_04_load_module.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_cmake_1/src/test_pkg/pure_mod.py
+-rw-r--r--   0        0        0      111 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_cmake_1/src/test_pkg/plat_mod.pyx
+-rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_cmake_1/src/test_pkg/CMakeLists.txt
+-rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_cmake_1/CMakeLists.txt
+-rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_cmake_1/pyproject.toml
+-rw-r--r--   0        0        0    12276 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/test_01_norms.py
+-rw-r--r--   0        0        0     5163 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/test_05_pkginfo.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_base/src/test_pkg/sub_mod/sub_sub_mod/good_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_base/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_base/src/test_pkg/sub_mod/good_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_base/src/test_pkg/sub_mod/bad_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_base/src/test_pkg/pure_mod/pure_mod.py
+-rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_base/pkgaux/__init__.py
+-rw-r--r--   0        0        0     1970 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_base/pyproject.toml
+-rw-r--r--   0        0        0     6894 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/test_06_pyproj.py
+-rw-r--r--   0        0        0     7554 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/test_02_path.py
+-rw-r--r--   0        0        0      764 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_3/pyproject.toml
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_1/src/test_pkg/pure_mod.py
+-rw-r--r--   0        0        0      111 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_1/src/test_pkg/plat_mod.pyx
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_1/meson.build
+-rw-r--r--   0        0        0      161 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_1/meson_options.txt
+-rw-r--r--   0        0        0     1652 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_meson_1/pyproject.toml
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/test_07_backend.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_4/src/test_pkg/sub_mod/sub_sub_mod/good_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_4/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_4/src/test_pkg/pure_mod/pure_mod.py
+-rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_4/pkgaux/__init__.py
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_4/pyproject.toml
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_1/src/test_pkg/sub_mod/sub_sub_mod/good_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_1/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_1/src/test_pkg/pure_mod/pure_mod.py
+-rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/test/pkg_bad_1/pyproject.toml
+-rw-r--r--   0        0        0     6633 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/pyproject.toml
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/LICENSE.txt
+-rw-r--r--   0        0        0      163 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/README.rst
+-rw-r--r--   0        0        0    14798 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/setup.py
+-rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 partis_pyproj-0.1.3rc1/PKG-INFO
```

### Comparing `partis_pyproj-0.1.1/src/pyproj/__init__.py` & `partis_pyproj-0.1.3rc1/src/pyproj/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 from .validate import (
   ValidationError,
   ValidationWarning,
+  validating,
   valid_type,
   valid_keys,
   mapget,
   as_list )
 
 from .norms import (
   scalar,
```

### Comparing `partis_pyproj-0.1.1/src/pyproj/norms.py` & `partis_pyproj-0.1.3rc1/src/pyproj/norms.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/pep.py` & `partis_pyproj-0.1.3rc1/src/pyproj/pep.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/builder/builder.py` & `partis_pyproj-0.1.3rc1/src/pyproj/builder/builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,14 +78,21 @@
           if not src_dir.exists():
             raise ValidPathError(f"Source directory not found: {src_dir}")
 
         with validating(key = f"tool.pyproj.targets[{i}]"):
           if subdir(build_dir, prefix, check = False):
             raise ValidPathError(f"'prefix' cannot be inside 'build_dir': {build_dir}")
 
+        build_dirty = build_dir.exists() and any(build_dir.iterdir())
+
+        if target.build_clean and build_dirty:
+          raise ValidPathError(
+            f"'build_dir' is not empty, please remove manually."
+            f"If this was intended, set 'build_clean = false': {build_dir}")
+
         for k in ['build_dir', 'prefix']:
           with validating(key = f"tool.pyproj.targets[{i}].{k}"):
             dir = paths[k]
 
             if dir == self.root:
               raise ValidPathError(f"'{k}' cannot be root directory: {dir}")
 
@@ -107,15 +114,15 @@
           options = target.options,
           src_dir = src_dir,
           build_dir = build_dir,
           prefix = prefix,
           setup_args = target.setup_args,
           compile_args = target.compile_args,
           install_args = target.install_args,
-          build_clean = target.build_clean )
+          build_clean = not build_dirty )
 
     except:
       self.build_clean()
       raise
 
   #-----------------------------------------------------------------------------
   def __exit__(self, type, value, traceback):
```

### Comparing `partis_pyproj-0.1.1/src/pyproj/builder/cmake.py` & `partis_pyproj-0.1.3rc1/src/pyproj/builder/cmake.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,48 +50,43 @@
   if not shutil.which('cmake'):
     raise ValueError(f"The 'cmake' program not found.")
 
   if not shutil.which('ninja'):
     raise ValueError(f"The 'ninja' program not found.")
 
   # TODO: ensure any paths in setup_args are normalized
-  if not ( build_dir.exists() and any(build_dir.iterdir()) ):
+  if not build_clean:
+    # skip setup if the build directory
+    setup_args = list()
+  else:
     # only run setup if the build directory does not already exist (or is empty)
     setup_args = [
       'cmake',
       *setup_args,
       '-G',
       'Ninja',
       '--install-prefix',
-      os.fspath(prefix),
+      str(prefix),
       *[ cmake_option_arg(k,v) for k,v in options.items() ],
       '-B',
-      os.fspath(build_dir),
+      str(build_dir),
       '-S',
-      os.fspath(src_dir) ]
-
-  elif not build_clean:
-    # skip setup if the build directory should be 'clean'
-    setup_args = list()
-
-  else:
-    raise ValidPathError(
-      f"'build_dir' is not empty, remove manually if this is intended or set 'build_clean = false': {build_dir}")
+      str(src_dir) ]
 
   compile_args = [
     'cmake',
     *compile_args,
     '--build',
-    os.fspath(build_dir) ]
+    str(build_dir) ]
 
   install_args = [
     'cmake',
     *install_args,
     '--install',
-    os.fspath(build_dir) ]
+    str(build_dir) ]
 
 
   if setup_args:
     logger.debug(' '.join(setup_args))
     subprocess.check_call(setup_args)
 
   logger.debug(' '.join(compile_args))
```

### Comparing `partis_pyproj-0.1.1/src/pyproj/builder/meson.py` & `partis_pyproj-0.1.3rc1/src/pyproj/builder/meson.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,49 +49,46 @@
 
   if not shutil.which('meson'):
     raise ValueError(f"The 'meson' program not found.")
 
   if not shutil.which('ninja'):
     raise ValueError(f"The 'ninja' program not found.")
 
+  os.environ['MESON_FORCE_BACKTRACE'] = '1'
+
   # TODO: ensure any paths in setup_args are normalized
-  if not ( build_dir.exists() and any(build_dir.iterdir()) ):
+  if not build_clean:
+    # skip setup if the build directory already populated
+    setup_args = list()
+  else:
     # only run setup if the build directory does not already exist (or is empty)
     setup_args = [
       'meson',
       'setup',
       *setup_args,
       '--prefix',
-      os.fspath(prefix),
+      str(prefix),
       *[ meson_option_arg(k,v) for k,v in options.items() ],
-      os.fspath(build_dir),
-      os.fspath(src_dir) ]
-
-  elif not build_clean:
-    # skip setup if the build directory should be 'clean'
-    setup_args = list()
-
-  else:
-    raise ValidPathError(
-      f"'build_dir' is not empty, remove manually if this is intended or set 'build_clean = false': {build_dir}")
+      str(build_dir),
+      str(src_dir) ]
 
   compile_args = [
     'meson',
     'compile',
     *compile_args,
     '-C',
-    os.fspath(build_dir) ]
+    str(build_dir) ]
 
   install_args = [
     'meson',
     'install',
     *install_args,
     '--no-rebuild',
     '-C',
-    os.fspath(build_dir) ]
+    str(build_dir) ]
 
 
   if setup_args:
     logger.debug(' '.join(setup_args))
     subprocess.check_call(setup_args)
 
   logger.debug(' '.join(compile_args))
```

### Comparing `partis_pyproj-0.1.1/src/pyproj/load_module.py` & `partis_pyproj-0.1.3rc1/src/pyproj/load_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
   #-----------------------------------------------------------------------------
   def __call__(self, **kwargs):
 
     cwd = os.getcwd()
 
     try:
 
-      with validating( file = f"{self.name} -> {self.entry}(**{{{kwargs}}})" ):
+      with validating( file = f"{self.name} -> {self.entry}" ):
         self.func(
           self.pyproj,
           logger = self.logger,
           **kwargs )
 
     except Exception as e:
       raise EntryPointError(f"failed to run '{self.entry}'") from e
```

### Comparing `partis_pyproj-0.1.1/src/pyproj/_legacy_setup.py` & `partis_pyproj-0.1.3rc1/src/pyproj/_legacy_setup.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/_nonprintable.py` & `partis_pyproj-0.1.3rc1/src/pyproj/_nonprintable.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/path/match.py` & `partis_pyproj-0.1.3rc1/src/pyproj/path/match.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/path/pattern.py` & `partis_pyproj-0.1.3rc1/src/pyproj/path/pattern.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/path/utils.py` & `partis_pyproj-0.1.3rc1/src/pyproj/path/utils.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/validate.py` & `partis_pyproj-0.1.3rc1/src/pyproj/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,26 @@
 
     return msg
 
   #-----------------------------------------------------------------------------
   def __repr__(self):
     return str(self)
 
+  #-----------------------------------------------------------------------------
+  def model_hint(self):
+    from partis.utils import ModelHint, Loc
+
+    return ModelHint(
+      msg = type(self).__name__,
+      data = self.msg,
+      level = 'error',
+      loc = Loc(
+        filename = self.doc_file,
+        path = self.doc_path ))
+
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class RequiredValueError( ValidationError ):
   pass
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class ValidDefinitionError( ValidationError ):
   pass
@@ -216,38 +228,51 @@
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class Optional(Special):
   """Optional value
   """
   pass
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+class OptionalNone(Special):
+  """Optional value, but is set to None if not initially set
+  """
+  pass
+
+#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class Required(Special):
   """Required value
   """
   pass
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class NotSet(Special):
   """Special value indicating a value is not set
   """
   pass
 
 OPTIONAL = Optional()
+OPTIONAL_NONE = OptionalNone()
 REQUIRED = Required()
 NOTSET = NotSet()
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 def validate(val, default, validators):
   """Internal method to apply default value and validators
   """
-  if val is None:
-    if OPTIONAL == default:
-      return None
 
-    elif REQUIRED == default:
+  if val in [NOTSET, None]:
+    if default in [OPTIONAL, OPTIONAL_NONE]:
+      #               | NOTSET | None |
+      # --------------+--------+------+
+      # OPTIONAL      | NOTSET | None |
+      # --------------+--------+------+
+      # OPTIONAL_NONE | None   | None |
+      return None if default == OPTIONAL_NONE else val
+
+    elif default == REQUIRED:
       raise RequiredValueError(f"Value is required")
 
     else:
       val = default
 
   if not isinstance(validators, Sequence):
     validators = [validators]
@@ -336,22 +361,27 @@
   """
   #-----------------------------------------------------------------------------
   def __init__(self, *args, default = NOTSET):
 
     args = list(args)
 
     # TODO: change comparisons from 'is' to "==", reimplement Special __eq__
-    if NOTSET == default:
+    if default == NOTSET:
       default = REQUIRED
 
       if len(args):
         v = args.pop(0)
 
-        if OPTIONAL == v or v is None:
-          default = OPTIONAL
+        if v in [REQUIRED, OPTIONAL, OPTIONAL_NONE]:
+          # set from special value
+          default = v
+
+        elif v is None:
+          # set to fill in None if not given
+          default = OPTIONAL_NONE
 
         elif any(isinstance(v, t) for t in [bool, int, float, str, Sequence, Mapping]):
           default = v
 
         elif isinstance(v, type):
           # still used to validate the type
           args.insert(0, v)
@@ -365,20 +395,22 @@
           except Exception as e:
             # the type cannot be instantiated without arguments
             raise ValidDefinitionError(
               f"Default value must be specified, or explicitly set as optional or required") from e
 
         else:
           # cannot be used as default, put back to use as validator
+          # and a value is assumed to be required
           args.insert(0, v)
 
-    if default is None:
-      default = OPTIONAL
+    elif default is None:
+      # set to fill in None if not given
+      default = OPTIONAL_NONE
 
-    if len(args) == 0 and default not in [REQUIRED, OPTIONAL]:
+    if len(args) == 0 and default not in [REQUIRED, OPTIONAL, OPTIONAL_NONE]:
       # convenience method to used default value to derive type
       args.append(type(default))
 
     self._default = default
     self._validators = args
 
   #-----------------------------------------------------------------------------
@@ -392,15 +424,15 @@
     return f"{type(self).__name__}({args})"
 
   #-----------------------------------------------------------------------------
   def __repr__(self):
     return str(self)
 
   #-----------------------------------------------------------------------------
-  def __call__(self, val):
+  def __call__(self, val = NOTSET):
     return validate(val, self._default, self._validators)
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class Restricted(Validator):
   """Restricts a value to one of listed options
   """
   #-----------------------------------------------------------------------------
@@ -533,16 +565,16 @@
         raise ValidationError(f"Use of key '{k}' is not allowed")
 
   if deprecate_keys:
     for k_old, k_new in deprecate_keys:
       if k_old in out:
         out = copy_once(out)
 
-        if k_new and OPTIONAL != k_new:
-          if REQUIRED == k_new:
+        if k_new and k_new not in [OPTIONAL, OPTIONAL_NONE]:
+          if k_new == REQUIRED:
             # Use of REQUIRED indicates this is an error
             raise ValidationError(f"Use of key '{k_old}' is deprecated")
           else:
             warnings.warn(f"Use of key '{k_old}' is deprecated, replaced by '{k_new}'", DeprecationWarning)
 
           if k_new not in out:
             out[k_new] = out[k_old]
@@ -594,15 +626,15 @@
 
   if allow_keys is not None:
     allow_keys = copy(allow_keys)
     allow_keys.extend( require_keys or [] )
     allow_keys.extend( [
         k_new
         for k_old, k_new in deprecate_keys
-        if k_new not in [None, OPTIONAL, REQUIRED ] ]
+        if k_new not in [None, OPTIONAL, OPTIONAL_NONE, REQUIRED ] ]
       if deprecate_keys else [] )
 
     allow_keys.extend( default.keys() if default else [] )
 
     if proxy_keys:
       for keys in proxy_keys:
         allow_keys.extend(keys)
@@ -625,17 +657,18 @@
       if k not in allow_keys:
         raise ValidationError(
           f"Allowed keys {allow_keys}: '{k}'" )
 
   if default:
     for k, v in default.items():
       if not isinstance(v, Validator):
+        # convert literal value to a validator
         v = valid(v)
 
-      val = out.get(k, None)
+      val = out.get(k, NOTSET)
 
       with validating(key = k):
         _val = v( val )
 
       if _val is not val:
         out = copy_once(out)
         out[k] = _val
@@ -780,15 +813,15 @@
     if (
       len(kwargs) == 0
       and len(args) == 1
       and not isinstance(args[0], Mapping) ):
 
       v = args[0]
 
-      if v in [None, OPTIONAL]:
+      if v in [None, OPTIONAL, OPTIONAL_NONE]:
         args = [dict()]
       elif cls._proxy_key:
         args = [{ cls._proxy_key : v }]
 
     self._p_dict = dict(*args, **kwargs)
 
     with attrs_modify( self ):
@@ -803,15 +836,15 @@
     self._p_all_keys.extend( self._default.keys() )
 
     if self._deprecate_keys:
       for keys in self._deprecate_keys:
         self._p_all_keys.extend( [
             k_new
             for k_old, k_new in self._deprecate_keys
-            if k_new not in [None, OPTIONAL, REQUIRED] ] )
+            if k_new not in [None, OPTIONAL, OPTIONAL_NONE, REQUIRED] ] )
 
     if self._min_keys:
       for keys in self._min_keys:
         self._p_all_keys.extend(keys)
 
     if self._wedge_keys:
       for keys in self._wedge_keys:
@@ -1083,12 +1116,12 @@
     _default = default if i == last_i else dict()
 
     _obj = _obj.get( part, _default )
 
   return _obj
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-def as_list( obj ):
-  if isinstance( obj, str ) or isinstance(obj, Mapping) or not isinstance(obj, Iterable):
-    return [ obj ]
+def as_list(obj):
+  if isinstance(obj, (str, Mapping)) or not isinstance(obj, Iterable):
+    return [obj]
 
   return list(obj)
```

### Comparing `partis_pyproj-0.1.1/src/pyproj/pkginfo.py` & `partis_pyproj-0.1.3rc1/src/pyproj/pkginfo.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/dist_file/dist_targz.py` & `partis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_targz.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/dist_file/dist_zip.py` & `partis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_zip.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/dist_file/dist_binary.py` & `partis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_binary.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/dist_file/dist_base.py` & `partis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_base.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/dist_file/dist_source.py` & `partis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_source.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/legacy.py` & `partis_pyproj-0.1.3rc1/src/pyproj/legacy.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/backend.py` & `partis_pyproj-0.1.3rc1/src/pyproj/backend.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/src/pyproj/pyproj.py` & `partis_pyproj-0.1.3rc1/src/pyproj/pyproj.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,14 +98,25 @@
       src = fp.read()
       src = src.decode( 'utf-8', errors = 'replace' )
       self._pptoml = tomli.loads( src )
 
     with validating(root = self._pptoml, file = self.pptoml_file):
       self._pptoml = pptoml(self._pptoml)
 
+      with validating(key = 'tool'):
+        if 'tool' not in self.pptoml:
+          raise RequiredValueError(f"tool.pyproj is required for backend")
+
+        with validating(key = 'pyproj'):
+          if 'pyproj' not in self.pptoml.tool:
+            raise RequiredValueError(f"tool.pyproj is required for backend")
+
+      if self.project.dynamic and 'prep' not in self.pyproj:
+        raise ValidationError(f"tool.pyproj.prep is required to resolve project.dynamic")
+
     #...........................................................................
     # construct a validator from the tool.pyproj.config table
     config_default = dict()
 
     for k,v in self.pyproj.config.items():
       if isinstance(v, bool):
         config_default[k] = valid(v, norm_bool)
@@ -145,16 +156,16 @@
     if self.is_platlib:
       self.binary.compat_tags = platlib_compat_tags()
 
     #...........................................................................
     self.prep()
 
     with validating(
-      key = 'project', 
-      root = self._pptoml, 
+      key = 'project',
+      root = self._pptoml,
       file = self.pptoml_file):
 
       self.pkg_info = PkgInfo(
         project = self.project,
         root = self.root )
 
     # Update logger once package info is created
@@ -197,15 +208,15 @@
 
   #-----------------------------------------------------------------------------
   @property
   def meson(self):
     """:class:`partis.pyproj.pptoml.pyproj_meson`
 
     .. deprecated:: 0.1.0
-      Use :attr:`PyProjBase.targets` to access all build targets. 
+      Use :attr:`PyProjBase.targets` to access all build targets.
       These are no longer restricted to meson, but this attribute kept for backward
       compatability.
 
     """
     targets = self._pptoml.tool.pyproj.targets
 
     if not (len(targets) == 1 and targets[0].entry == 'partis.pyproj.builder:meson'):
@@ -278,18 +289,14 @@
   def prep( self ):
     """Prepares project metadata
     """
     # backup project to detect changes made by prep
     project = deepcopy(self.project)
     dynamic = project.dynamic
 
-
-    if dynamic and 'prep' not in self.pyproj:
-      raise ValidationError(f"tool.pyproj.prep is required to resolve project.dynamic")
-
     self.prep_entrypoint(
       name = f"tool.pyproj.prep",
       obj = self.pyproj,
       logger = self.logger.getChild( f"prep" ) )
 
     # NOTE: check that any dynamic meta-data is defined after prep
     for k in dynamic:
```

### Comparing `partis_pyproj-0.1.1/src/pyproj/pptoml.py` & `partis_pyproj-0.1.3rc1/src/pyproj/pptoml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-
+import re
 from packaging.requirements import Requirement
 from packaging.specifiers import SpecifierSet
 from pathlib import (
   Path,
   PurePath,
   PurePosixPath)
 
 from collections.abc import (
   Mapping,
   Sequence,
   Iterable )
 
 from .validate import (
   OPTIONAL,
+  OPTIONAL_NONE,
   REQUIRED,
   valid,
   union,
   restrict,
   valid_dict,
   valid_list,
   ValidationError,
@@ -211,15 +212,15 @@
 class build_system(valid_dict):
   _allow_keys = list()
   _require_keys = [
     'build-backend']
   _default = {
     'requires': build_requires,
     'build-backend': norm_entry_point_ref,
-    'backend-path': valid(OPTIONAL, path_parts) }
+    'backend-path': valid(OPTIONAL_NONE, path_parts) }
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 def compat_tag(v):
   return CompatibilityTags(*v)
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class compat_tags(valid_list):
@@ -294,30 +295,51 @@
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class ignore_list(valid_list):
   _as_list = valid(as_list)
   _value_valid = valid(nonempty_str)
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+class glob_list(valid_list):
+  _as_list = valid(as_list)
+  _value_valid = valid(nonempty_str)
+
+#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+class include(valid_dict):
+  _allow_keys = list()
+  # a string at top-level interpreted as 'match'
+  _proxy_key = 'glob'
+  # TODO: how to normalize patterns?
+  _default = {
+    'glob': valid(nonempty_str),
+    'rematch': valid(r'.*', nonempty_str, re.compile),
+    'replace': valid('{0}', nonempty_str)}
+
+#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+class include_list(valid_list):
+  _as_list = valid(as_list)
+  _value_valid = valid(include)
+
+#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class pyproj_dist_copy(valid_dict):
   # a string at top-level interpreted as 'src'
   _proxy_key = 'src'
   # take 'dst' from 'src' if not set
   _proxy_keys = [('dst', 'src')]
+  _deprecate_keys = [('glob', 'include')]
   _allow_keys = list()
   _min_keys = [
     ('src', 'glob') ]
   _default = {
     # NOTE: file paths should initially be given as a POSIX path,
     # but converted to current OS path so it may be read.
     'src': valid(REQUIRED, PurePosixPath, Path),
     # the destination path in the archive should remain as a POSIX path
     'dst': valid(REQUIRED, PurePosixPath),
-    # TODO; how to normalize patterns?
-    'glob': str,
+    'include': include_list,
     'ignore': ignore_list }
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class pyproj_dist_copy_list(valid_list):
   _value_valid = valid(pyproj_dist_copy)
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
@@ -327,18 +349,18 @@
     'ignore': ignore_list,
     'copy': pyproj_dist_copy_list }
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class pyproj_dist_binary(valid_dict):
   _allow_keys = list()
   _default = {
-    'build_number': valid(OPTIONAL, int),
-    'build_suffix': valid(OPTIONAL, str),
+    'build_number': valid(OPTIONAL_NONE, int),
+    'build_suffix': valid(OPTIONAL_NONE, str),
     'compat_tags': valid(purelib_compat_tags(), compat_tags),
-    'prep': valid(OPTIONAL, pyproj_dist_binary_prep),
+    'prep': valid(OPTIONAL_NONE, pyproj_dist_binary_prep),
     'ignore': ignore_list,
     'copy': pyproj_dist_copy_list,
     'data': pyproj_dist_scheme,
     'headers': pyproj_dist_scheme,
     'scripts': pyproj_dist_scheme,
     'purelib': pyproj_dist_scheme,
     'platlib': pyproj_dist_scheme }
@@ -383,13 +405,12 @@
     'pyproj': pyproj }
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class pptoml(valid_dict):
   _allow_keys = list()
   _require_keys = [
     'project',
-    'tool',
     'build-system']
   _default = {
     'project': valid(REQUIRED, project),
-    'tool': valid(REQUIRED, tool),
-    'build-system': valid(REQUIRED, build_system) }
+    'build-system': valid(REQUIRED, build_system),
+    'tool': valid(OPTIONAL, tool) }
```

### Comparing `partis_pyproj-0.1.1/doc/index.rst` & `partis_pyproj-0.1.3rc1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_bad_5/pyproject.toml` & `partis_pyproj-0.1.3rc1/test/pkg_bad_5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_meson_2/meson.build` & `partis_pyproj-0.1.3rc1/test/pkg_meson_2/meson.build`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_meson_2/pyproject.toml` & `partis_pyproj-0.1.3rc1/test/pkg_meson_2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
   'pyproject.toml' ]
 
 #...............................................................................
 # Configuration of the meson build system
 [[tool.pyproj.targets]]
 entry = 'partis.pyproj.builder:meson'
 
-build_clean = false
 compile_args = [
   '-j', '1' ]
 
 prefix = 'build'
 build_dir = 'build/meson'
 
 [tool.pyproj.targets.options]
```

### Comparing `partis_pyproj-0.1.1/test/pkg_bad_2/pkgaux/__init__.py` & `partis_pyproj-0.1.3rc1/test/pkg_bad_2/pkgaux/__init__.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_bad_2/pyproject.toml` & `partis_pyproj-0.1.3rc1/test/pkg_bad_2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/__main__.py` & `partis_pyproj-0.1.3rc1/test/__main__.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/test_03_dist.py` & `partis_pyproj-0.1.3rc1/test/test_03_dist.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_meson_bad_1/bad_link/meson.build` & `partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/bad_link/meson.build`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_meson_bad_1/bad_link/pyproject.toml` & `partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/bad_link/pyproject.toml`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_meson_bad_1/meson.build` & `partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/meson.build`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_meson_bad_1/pyproject.toml` & `partis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_min/pyproject.toml` & `partis_pyproj-0.1.3rc1/test/pkg_min/pyproject.toml`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/noxfile.py` & `partis_pyproj-0.1.3rc1/test/noxfile.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/test_00_validate.py` & `partis_pyproj-0.1.3rc1/test/test_00_validate.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,19 @@
   raises )
 
 from partis.pyproj.validate import (
   ValidationError,
   ValidDefinitionError,
   validating,
   validate,
+  NOTSET,
   Optional,
   OPTIONAL,
+  OptionalNone,
+  OPTIONAL_NONE,
   Required,
   REQUIRED,
   fmt_validator,
   Validator,
   Restricted,
   valid,
   union,
@@ -35,14 +38,16 @@
   print(hash(OPTIONAL))
 
   assert REQUIRED == Required()
   print(hash(REQUIRED))
 
   assert OPTIONAL != REQUIRED
   assert OPTIONAL != None
+  assert OPTIONAL_NONE != None
+  assert OPTIONAL_NONE != OPTIONAL
   assert REQUIRED != None
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 def test_validating():
 
   def f():
     assert False
@@ -124,36 +129,58 @@
 
   m = Validator()
   print(str(m))
   print(repr(m))
   assert m._default == REQUIRED
   assert m._validators == []
 
+  m = Validator(default = REQUIRED)
+  assert m._default == REQUIRED
+  assert m._validators == []
+
+  with raises(ValidationError):
+    m()
+
   m = Validator(default = None)
-  assert m._default == OPTIONAL
+  assert m._default == OPTIONAL_NONE
   assert m._validators == []
+  assert m() == None
 
   m = Validator(None)
+  assert m._default == OPTIONAL_NONE
+  assert m._validators == []
+  assert m() == None
+
+  m = Validator(default = OPTIONAL)
+  assert m._default == OPTIONAL
+  assert m._validators == []
+  assert m() == NOTSET
+
+  m = Validator(OPTIONAL)
   assert m._default == OPTIONAL
   assert m._validators == []
+  assert m() == NOTSET
 
   a = Validator(1)
   print(str(a))
   assert a._default == 1
   assert a._validators == [int]
+  assert a() == 1
 
   b = Validator(int)
   print(str(b))
   assert b._default == 0
   assert b._validators == [int]
+  assert b() == 0
 
   c = Validator(int, default = 2)
   print(str(c))
   assert c._default == 2
   assert c._validators == [int]
+  assert c() == 2
 
   class Test:
     def __init__(self, x):
       self._x = x
 
     def __eq__(self, other):
       if isinstance(other, Test):
```

### Comparing `partis_pyproj-0.1.1/test/test_04_load_module.py` & `partis_pyproj-0.1.3rc1/test/test_04_load_module.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_cmake_1/pyproject.toml` & `partis_pyproj-0.1.3rc1/test/pkg_cmake_1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 email = "software.support@nanohmics.com"
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 # Build and distribution configuration
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 [build-system]
 requires = [
-  "partis-pyproj[meson] >= 0.0.1",
+  "partis-pyproj[cmake] >= 0.0.1",
   "Cython>=0.29.18" ]
 
 build-backend = "partis.pyproj.backend"
 
 #...............................................................................
 [tool.pyproj.dist.source]
 
@@ -31,27 +31,26 @@
   'pyproject.toml' ]
 
 #...............................................................................
 # Configuration of the meson build system
 [[tool.pyproj.targets]]
 entry = 'partis.pyproj.builder:cmake'
 prefix = 'build'
-build_clean = false
 
 [tool.pyproj.targets.options]
 opt_a = true
 
 #...............................................................................
 [tool.pyproj.dist.binary]
 ignore = [
   '*.pyx' ]
 
 #...............................................................................
 [tool.pyproj.dist.binary.purelib]
 
 copy = [
-  { src = 'src/test_pkg', dst = 'test_pkg_meson_1' } ]
+  { src = 'src/test_pkg', dst = 'test_pkg_cmake_1' } ]
 
 #...............................................................................
 [tool.pyproj.dist.binary.platlib]
 copy = [
-  { src = 'build/lib', dst = 'test_pkg_meson_1' } ]
+  { src = 'build/lib', dst = 'test_pkg_cmake_1' } ]
```

### Comparing `partis_pyproj-0.1.1/test/test_01_norms.py` & `partis_pyproj-0.1.3rc1/test/test_01_norms.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/test_05_pkginfo.py` & `partis_pyproj-0.1.3rc1/test/test_05_pkginfo.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_base/pkgaux/__init__.py` & `partis_pyproj-0.1.3rc1/test/pkg_base/pkgaux/__init__.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_base/pyproject.toml` & `partis_pyproj-0.1.3rc1/test/pkg_base/pyproject.toml`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/test_06_pyproj.py` & `partis_pyproj-0.1.3rc1/test/test_06_pyproj.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,7 +274,11 @@
       source = False,
       binary = True )
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 @mark.skipif(SKIP_CMAKE, reason="")
 def test_cmake_1():
   run_pyproj('pkg_cmake_1')
+
+#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+if __name__ == '__main__':
+  test_cmake_1()
```

### Comparing `partis_pyproj-0.1.1/test/test_02_path.py` & `partis_pyproj-0.1.3rc1/test/test_02_path.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_bad_3/pyproject.toml` & `partis_pyproj-0.1.3rc1/test/pkg_bad_3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_meson_1/meson.build` & `partis_pyproj-0.1.3rc1/test/pkg_meson_1/meson.build`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_meson_1/pyproject.toml` & `partis_pyproj-0.1.3rc1/test/pkg_meson_1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/test_07_backend.py` & `partis_pyproj-0.1.3rc1/test/test_07_backend.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_bad_4/pkgaux/__init__.py` & `partis_pyproj-0.1.3rc1/test/pkg_bad_4/pkgaux/__init__.py`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_bad_4/pyproject.toml` & `partis_pyproj-0.1.3rc1/test/pkg_bad_4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/test/pkg_bad_1/pyproject.toml` & `partis_pyproj-0.1.3rc1/test/pkg_bad_1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/pyproject.toml` & `partis_pyproj-0.1.3rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 # Meta-data and dependencies
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 [project]
 name = "partis-pyproj"
-version = "0.1.1"
+version = "0.1.3rc1"
 description = "Minimal set of Python project utilities (PEP-517/621)"
 maintainers = [
   { name = "Nanohmics Inc.", email = "software.support@nanohmics.com" } ]
 license = { file = "LICENSE.txt" }
 readme = { file = "README.rst" }
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -57,15 +57,15 @@
   "ninja >= 1.10.2.3" ]
 
 cmake = [
   "cmake >= 3.24.3",
   "ninja >= 1.10.2.3" ]
 
 doc = [
-  'partis-utils[sphinx] >= 0.1.0' ]
+  'partis-utils[sphinx] >= 0.1.3rc1' ]
 
 #...............................................................................
 test = [
   "pip >= 18.1",
   "nox >= 2021.10.1",
   "build >= 0.7.0",
   # numpy needed to run some of the tests where the source code does not need it
@@ -119,15 +119,16 @@
   '.nox',
   '.pytest_cache',
   '.coverage',
   'tmp',
   'dist',
   'build',
   'doc/_build',
-  'doc/.nox' ]
+  'doc/.nox',
+  'test/*/build' ]
 
 #...............................................................................
 [tool.pyproj.dist.source]
 
 copy = [
   'src',
   'doc',
```

### Comparing `partis_pyproj-0.1.1/LICENSE.txt` & `partis_pyproj-0.1.3rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `partis_pyproj-0.1.1/setup.py` & `partis_pyproj-0.1.3rc1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -187,23 +187,23 @@
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 # NOTE: these are templated literal values substituded by the backend when
 # building the source distribution
 
 build_backend = 'pyproj.backend'
 backend_path = ['src']
-build_requires = ['importlib_metadata; python_version < "3.8"', 'tomli>=1.2.3', 'wheel', 'packaging==21.3']
+build_requires = ['wheel', 'tomli>=1.2.3', 'packaging==21.3', 'importlib_metadata; python_version < "3.8"']
 
 EGG_INFO_NAME = 'partis-pyproj.egg-info'
 
-PKG_INFO = b'Metadata-Version: 2.1\nName: partis-pyproj\nVersion: 0.1.1\nRequires-Python: >=3.6.2\nAuthor-email: "Nanohmics Inc." <software.support@nanohmics.com>\nMaintainer-email: "Nanohmics Inc." <software.support@nanohmics.com>\nSummary: Minimal set of Python project utilities (PEP-517/621)\nLicense-File: LICENSE.txt\nClassifier: Programming Language :: Python\nClassifier: License :: OSI Approved :: BSD License\nClassifier: Operating System :: POSIX :: Linux\nClassifier: Operating System :: Microsoft :: Windows\nClassifier: Programming Language :: Python :: 3\nClassifier: Topic :: Software Development :: Build Tools\nClassifier: Intended Audience :: Developers\nClassifier: Development Status :: 4 - Beta\nProvides-Extra: meson\nProvides-Extra: cmake\nProvides-Extra: doc\nProvides-Extra: test\nProvides-Extra: cov\nProvides-Extra: lint\nRequires-Dist: importlib_metadata; python_version < "3.8"\nRequires-Dist: packaging==21.3\nRequires-Dist: wheel\nRequires-Dist: tomli>=1.2.3\nRequires-Dist: meson>=0.61.3; extra == "meson"\nRequires-Dist: ninja>=1.10.2.3; extra == "meson"\nRequires-Dist: cmake>=3.24.3; extra == "cmake"\nRequires-Dist: ninja>=1.10.2.3; extra == "cmake"\nRequires-Dist: partis-utils[sphinx]>=0.1.0; extra == "doc"\nRequires-Dist: build>=0.7.0; extra == "test"\nRequires-Dist: ninja>=1.10.2.3; extra == "test"\nRequires-Dist: tomli>=1.2.3; extra == "test"\nRequires-Dist: coverage[toml]>=6.2; extra == "test"\nRequires-Dist: pip>=18.1; extra == "test"\nRequires-Dist: pytest-cov>=3.0.0; extra == "test"\nRequires-Dist: numpy; extra == "test"\nRequires-Dist: pytest_mock>=3.6.1; extra == "test"\nRequires-Dist: cmake>=3.24.3; extra == "test"\nRequires-Dist: Cython>=0.29.18; extra == "test"\nRequires-Dist: meson>=0.61.3; extra == "test"\nRequires-Dist: pytest>=6.2.5; extra == "test"\nRequires-Dist: nox>=2021.10.1; extra == "test"\nRequires-Dist: coverage[toml]>=6.2; extra == "cov"\nRequires-Dist: pyflakes==2.4.0; extra == "lint"\nDescription-Content-Type: text/x-rst\n\nThe ``partis.pyproj`` package aims to be very simple and\ntransparent implementation of a PEP-517 build back-end.\n\nhttps://nanohmics.bitbucket.io/doc/partis/pyproj'
+PKG_INFO = b'Metadata-Version: 2.1\nName: partis-pyproj\nVersion: 0.1.3rc1\nRequires-Python: >=3.6.2\nAuthor-email: "Nanohmics Inc." <software.support@nanohmics.com>\nMaintainer-email: "Nanohmics Inc." <software.support@nanohmics.com>\nSummary: Minimal set of Python project utilities (PEP-517/621)\nLicense-File: LICENSE.txt\nClassifier: Topic :: Software Development :: Build Tools\nClassifier: License :: OSI Approved :: BSD License\nClassifier: Programming Language :: Python\nClassifier: Operating System :: POSIX :: Linux\nClassifier: Development Status :: 4 - Beta\nClassifier: Intended Audience :: Developers\nClassifier: Programming Language :: Python :: 3\nClassifier: Operating System :: Microsoft :: Windows\nProvides-Extra: meson\nProvides-Extra: cmake\nProvides-Extra: doc\nProvides-Extra: test\nProvides-Extra: cov\nProvides-Extra: lint\nRequires-Dist: tomli>=1.2.3\nRequires-Dist: packaging==21.3\nRequires-Dist: importlib_metadata; python_version < "3.8"\nRequires-Dist: wheel\nRequires-Dist: meson>=0.61.3; extra == "meson"\nRequires-Dist: ninja>=1.10.2.3; extra == "meson"\nRequires-Dist: ninja>=1.10.2.3; extra == "cmake"\nRequires-Dist: cmake>=3.24.3; extra == "cmake"\nRequires-Dist: partis-utils[sphinx]>=0.1.3rc1; extra == "doc"\nRequires-Dist: meson>=0.61.3; extra == "test"\nRequires-Dist: numpy; extra == "test"\nRequires-Dist: pip>=18.1; extra == "test"\nRequires-Dist: coverage[toml]>=6.2; extra == "test"\nRequires-Dist: nox>=2021.10.1; extra == "test"\nRequires-Dist: tomli>=1.2.3; extra == "test"\nRequires-Dist: cmake>=3.24.3; extra == "test"\nRequires-Dist: Cython>=0.29.18; extra == "test"\nRequires-Dist: ninja>=1.10.2.3; extra == "test"\nRequires-Dist: pytest_mock>=3.6.1; extra == "test"\nRequires-Dist: build>=0.7.0; extra == "test"\nRequires-Dist: pytest>=6.2.5; extra == "test"\nRequires-Dist: pytest-cov>=3.0.0; extra == "test"\nRequires-Dist: coverage[toml]>=6.2; extra == "cov"\nRequires-Dist: pyflakes==2.4.0; extra == "lint"\nDescription-Content-Type: text/x-rst\n\nThe ``partis.pyproj`` package aims to be very simple and\ntransparent implementation of a PEP-517 build back-end.\n\nhttps://nanohmics.bitbucket.io/doc/partis/pyproj'
 
-REQUIRES = b'importlib_metadata; python_version < "3.8"\npackaging==21.3\nwheel\ntomli>=1.2.3\nmeson>=0.61.3; extra == "meson"\nninja>=1.10.2.3; extra == "meson"\ncmake>=3.24.3; extra == "cmake"\nninja>=1.10.2.3; extra == "cmake"\npartis-utils[sphinx]>=0.1.0; extra == "doc"\nbuild>=0.7.0; extra == "test"\nninja>=1.10.2.3; extra == "test"\ntomli>=1.2.3; extra == "test"\ncoverage[toml]>=6.2; extra == "test"\npip>=18.1; extra == "test"\npytest-cov>=3.0.0; extra == "test"\nnumpy; extra == "test"\npytest_mock>=3.6.1; extra == "test"\ncmake>=3.24.3; extra == "test"\nCython>=0.29.18; extra == "test"\nmeson>=0.61.3; extra == "test"\npytest>=6.2.5; extra == "test"\nnox>=2021.10.1; extra == "test"\ncoverage[toml]>=6.2; extra == "cov"\npyflakes==2.4.0; extra == "lint"'
+REQUIRES = b'tomli>=1.2.3\npackaging==21.3\nimportlib_metadata; python_version < "3.8"\nwheel\nmeson>=0.61.3; extra == "meson"\nninja>=1.10.2.3; extra == "meson"\nninja>=1.10.2.3; extra == "cmake"\ncmake>=3.24.3; extra == "cmake"\npartis-utils[sphinx]>=0.1.3rc1; extra == "doc"\nmeson>=0.61.3; extra == "test"\nnumpy; extra == "test"\npip>=18.1; extra == "test"\ncoverage[toml]>=6.2; extra == "test"\nnox>=2021.10.1; extra == "test"\ntomli>=1.2.3; extra == "test"\ncmake>=3.24.3; extra == "test"\nCython>=0.29.18; extra == "test"\nninja>=1.10.2.3; extra == "test"\npytest_mock>=3.6.1; extra == "test"\nbuild>=0.7.0; extra == "test"\npytest>=6.2.5; extra == "test"\npytest-cov>=3.0.0; extra == "test"\ncoverage[toml]>=6.2; extra == "cov"\npyflakes==2.4.0; extra == "lint"'
 
-SOURCES = b'partis_pyproj-0.1.1/src/pyproj/__init__.py\npartis_pyproj-0.1.1/src/pyproj/norms.py\npartis_pyproj-0.1.1/src/pyproj/pep.py\npartis_pyproj-0.1.1/src/pyproj/builder/__init__.py\npartis_pyproj-0.1.1/src/pyproj/builder/builder.py\npartis_pyproj-0.1.1/src/pyproj/builder/cmake.py\npartis_pyproj-0.1.1/src/pyproj/builder/meson.py\npartis_pyproj-0.1.1/src/pyproj/load_module.py\npartis_pyproj-0.1.1/src/pyproj/_legacy_setup.py\npartis_pyproj-0.1.1/src/pyproj/_nonprintable.py\npartis_pyproj-0.1.1/src/pyproj/path/__init__.py\npartis_pyproj-0.1.1/src/pyproj/path/match.py\npartis_pyproj-0.1.1/src/pyproj/path/pattern.py\npartis_pyproj-0.1.1/src/pyproj/path/utils.py\npartis_pyproj-0.1.1/src/pyproj/validate.py\npartis_pyproj-0.1.1/src/pyproj/pkginfo.py\npartis_pyproj-0.1.1/src/pyproj/dist_file/dist_targz.py\npartis_pyproj-0.1.1/src/pyproj/dist_file/__init__.py\npartis_pyproj-0.1.1/src/pyproj/dist_file/dist_zip.py\npartis_pyproj-0.1.1/src/pyproj/dist_file/dist_binary.py\npartis_pyproj-0.1.1/src/pyproj/dist_file/dist_base.py\npartis_pyproj-0.1.1/src/pyproj/dist_file/dist_source.py\npartis_pyproj-0.1.1/src/pyproj/dist_file/dist_copy.py\npartis_pyproj-0.1.1/src/pyproj/legacy.py\npartis_pyproj-0.1.1/src/pyproj/backend.py\npartis_pyproj-0.1.1/src/pyproj/pyproj.py\npartis_pyproj-0.1.1/src/pyproj/pptoml.py\npartis_pyproj-0.1.1/doc/conf.py\npartis_pyproj-0.1.1/doc/__init__.py\npartis_pyproj-0.1.1/doc/index.rst\npartis_pyproj-0.1.1/doc/src/pptoml.rst\npartis_pyproj-0.1.1/doc/src/index.rst\npartis_pyproj-0.1.1/doc/src/backend.rst\npartis_pyproj-0.1.1/doc/src/builder.rst\npartis_pyproj-0.1.1/doc/src/validate.rst\npartis_pyproj-0.1.1/doc/src/pkginfo.rst\npartis_pyproj-0.1.1/doc/src/pyproj.rst\npartis_pyproj-0.1.1/doc/src/path.rst\npartis_pyproj-0.1.1/doc/src/pep.rst\npartis_pyproj-0.1.1/doc/src/load_module.rst\npartis_pyproj-0.1.1/doc/src/norms.rst\npartis_pyproj-0.1.1/doc/src/dist_file.rst\npartis_pyproj-0.1.1/doc/__main__.py\npartis_pyproj-0.1.1/doc/glossary.rst\npartis_pyproj-0.1.1/test/pkg_bad_5/src/test_pkg/sub_mod/sub_sub_mod/good_file.py\npartis_pyproj-0.1.1/test/pkg_bad_5/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py\npartis_pyproj-0.1.1/test/pkg_bad_5/src/test_pkg/pure_mod/pure_mod.py\npartis_pyproj-0.1.1/test/pkg_bad_5/pkgaux/__init__.py\npartis_pyproj-0.1.1/test/pkg_bad_5/pyproject.toml\npartis_pyproj-0.1.1/test/__init__.py\npartis_pyproj-0.1.1/test/pkg_meson_2/src/test_pkg/pure_mod.py\npartis_pyproj-0.1.1/test/pkg_meson_2/src/test_pkg/plat_mod.pyx\npartis_pyproj-0.1.1/test/pkg_meson_2/meson.build\npartis_pyproj-0.1.1/test/pkg_meson_2/meson_options.txt\npartis_pyproj-0.1.1/test/pkg_meson_2/pyproject.toml\npartis_pyproj-0.1.1/test/pkg_bad_2/src/test_pkg/sub_mod/sub_sub_mod/good_file.py\npartis_pyproj-0.1.1/test/pkg_bad_2/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py\npartis_pyproj-0.1.1/test/pkg_bad_2/src/test_pkg/pure_mod/pure_mod.py\npartis_pyproj-0.1.1/test/pkg_bad_2/pkgaux/__init__.py\npartis_pyproj-0.1.1/test/pkg_bad_2/pyproject.toml\npartis_pyproj-0.1.1/test/__main__.py\npartis_pyproj-0.1.1/test/test_03_dist.py\npartis_pyproj-0.1.1/test/sitecustom/partis-sitecustom.pth\npartis_pyproj-0.1.1/test/sitecustom/pyproject.toml\npartis_pyproj-0.1.1/test/pkg_meson_bad_1/bad_link/src/test_pkg/pure_mod.py\npartis_pyproj-0.1.1/test/pkg_meson_bad_1/bad_link/src/test_pkg/plat_mod.pyx\npartis_pyproj-0.1.1/test/pkg_meson_bad_1/bad_link/meson.build\npartis_pyproj-0.1.1/test/pkg_meson_bad_1/bad_link/meson_options.txt\npartis_pyproj-0.1.1/test/pkg_meson_bad_1/bad_link/pyproject.toml\npartis_pyproj-0.1.1/test/pkg_meson_bad_1/src/test_pkg/pure_mod.py\npartis_pyproj-0.1.1/test/pkg_meson_bad_1/src/test_pkg/plat_mod.pyx\npartis_pyproj-0.1.1/test/pkg_meson_bad_1/meson.build\npartis_pyproj-0.1.1/test/pkg_meson_bad_1/meson_options.txt\npartis_pyproj-0.1.1/test/pkg_meson_bad_1/pyproject.toml\npartis_pyproj-0.1.1/test/pkg_min/pure_mod.py\npartis_pyproj-0.1.1/test/pkg_min/pyproject.toml\npartis_pyproj-0.1.1/test/noxfile.py\npartis_pyproj-0.1.1/test/test_00_validate.py\npartis_pyproj-0.1.1/test/test_04_load_module.py\npartis_pyproj-0.1.1/test/pkg_cmake_1/src/test_pkg/pure_mod.py\npartis_pyproj-0.1.1/test/pkg_cmake_1/src/test_pkg/plat_mod.pyx\npartis_pyproj-0.1.1/test/pkg_cmake_1/src/test_pkg/CMakeLists.txt\npartis_pyproj-0.1.1/test/pkg_cmake_1/CMakeLists.txt\npartis_pyproj-0.1.1/test/pkg_cmake_1/pyproject.toml\npartis_pyproj-0.1.1/test/test_01_norms.py\npartis_pyproj-0.1.1/test/test_05_pkginfo.py\npartis_pyproj-0.1.1/test/pkg_base/src/test_pkg/sub_mod/sub_sub_mod/good_file.py\npartis_pyproj-0.1.1/test/pkg_base/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py\npartis_pyproj-0.1.1/test/pkg_base/src/test_pkg/sub_mod/good_file.py\npartis_pyproj-0.1.1/test/pkg_base/src/test_pkg/sub_mod/bad_file.py\npartis_pyproj-0.1.1/test/pkg_base/src/test_pkg/pure_mod/pure_mod.py\npartis_pyproj-0.1.1/test/pkg_base/pkgaux/__init__.py\npartis_pyproj-0.1.1/test/pkg_base/pyproject.toml\npartis_pyproj-0.1.1/test/test_06_pyproj.py\npartis_pyproj-0.1.1/test/test_02_path.py\npartis_pyproj-0.1.1/test/pkg_bad_3/pyproject.toml\npartis_pyproj-0.1.1/test/pkg_meson_1/src/test_pkg/pure_mod.py\npartis_pyproj-0.1.1/test/pkg_meson_1/src/test_pkg/plat_mod.pyx\npartis_pyproj-0.1.1/test/pkg_meson_1/meson.build\npartis_pyproj-0.1.1/test/pkg_meson_1/meson_options.txt\npartis_pyproj-0.1.1/test/pkg_meson_1/pyproject.toml\npartis_pyproj-0.1.1/test/test_07_backend.py\npartis_pyproj-0.1.1/test/pkg_bad_4/src/test_pkg/sub_mod/sub_sub_mod/good_file.py\npartis_pyproj-0.1.1/test/pkg_bad_4/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py\npartis_pyproj-0.1.1/test/pkg_bad_4/src/test_pkg/pure_mod/pure_mod.py\npartis_pyproj-0.1.1/test/pkg_bad_4/pkgaux/__init__.py\npartis_pyproj-0.1.1/test/pkg_bad_4/pyproject.toml\npartis_pyproj-0.1.1/test/pkg_bad_1/src/test_pkg/sub_mod/sub_sub_mod/good_file.py\npartis_pyproj-0.1.1/test/pkg_bad_1/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py\npartis_pyproj-0.1.1/test/pkg_bad_1/src/test_pkg/pure_mod/pure_mod.py\npartis_pyproj-0.1.1/test/pkg_bad_1/pyproject.toml\npartis_pyproj-0.1.1/pyproject.toml\npartis_pyproj-0.1.1/LICENSE.txt\npartis_pyproj-0.1.1/README.rst'
+SOURCES = b'partis_pyproj-0.1.3rc1/src/pyproj/__init__.py\npartis_pyproj-0.1.3rc1/src/pyproj/norms.py\npartis_pyproj-0.1.3rc1/src/pyproj/pep.py\npartis_pyproj-0.1.3rc1/src/pyproj/builder/__init__.py\npartis_pyproj-0.1.3rc1/src/pyproj/builder/builder.py\npartis_pyproj-0.1.3rc1/src/pyproj/builder/cargo.py\npartis_pyproj-0.1.3rc1/src/pyproj/builder/cmake.py\npartis_pyproj-0.1.3rc1/src/pyproj/builder/meson.py\npartis_pyproj-0.1.3rc1/src/pyproj/builder/process.py\npartis_pyproj-0.1.3rc1/src/pyproj/load_module.py\npartis_pyproj-0.1.3rc1/src/pyproj/_legacy_setup.py\npartis_pyproj-0.1.3rc1/src/pyproj/_nonprintable.py\npartis_pyproj-0.1.3rc1/src/pyproj/path/__init__.py\npartis_pyproj-0.1.3rc1/src/pyproj/path/match.py\npartis_pyproj-0.1.3rc1/src/pyproj/path/pattern.py\npartis_pyproj-0.1.3rc1/src/pyproj/path/utils.py\npartis_pyproj-0.1.3rc1/src/pyproj/validate.py\npartis_pyproj-0.1.3rc1/src/pyproj/pkginfo.py\npartis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_targz.py\npartis_pyproj-0.1.3rc1/src/pyproj/dist_file/__init__.py\npartis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_zip.py\npartis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_binary.py\npartis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_base.py\npartis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_source.py\npartis_pyproj-0.1.3rc1/src/pyproj/dist_file/dist_copy.py\npartis_pyproj-0.1.3rc1/src/pyproj/legacy.py\npartis_pyproj-0.1.3rc1/src/pyproj/backend.py\npartis_pyproj-0.1.3rc1/src/pyproj/pyproj.py\npartis_pyproj-0.1.3rc1/src/pyproj/pptoml.py\npartis_pyproj-0.1.3rc1/doc/conf.py\npartis_pyproj-0.1.3rc1/doc/__init__.py\npartis_pyproj-0.1.3rc1/doc/index.rst\npartis_pyproj-0.1.3rc1/doc/src/pptoml.rst\npartis_pyproj-0.1.3rc1/doc/src/index.rst\npartis_pyproj-0.1.3rc1/doc/src/backend.rst\npartis_pyproj-0.1.3rc1/doc/src/builder.rst\npartis_pyproj-0.1.3rc1/doc/src/validate.rst\npartis_pyproj-0.1.3rc1/doc/src/pkginfo.rst\npartis_pyproj-0.1.3rc1/doc/src/pyproj.rst\npartis_pyproj-0.1.3rc1/doc/src/path.rst\npartis_pyproj-0.1.3rc1/doc/src/pep.rst\npartis_pyproj-0.1.3rc1/doc/src/load_module.rst\npartis_pyproj-0.1.3rc1/doc/src/norms.rst\npartis_pyproj-0.1.3rc1/doc/src/dist_file.rst\npartis_pyproj-0.1.3rc1/doc/__main__.py\npartis_pyproj-0.1.3rc1/doc/glossary.rst\npartis_pyproj-0.1.3rc1/test/pkg_bad_5/src/test_pkg/sub_mod/sub_sub_mod/good_file.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_5/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_5/src/test_pkg/pure_mod/pure_mod.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_5/pkgaux/__init__.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_5/pyproject.toml\npartis_pyproj-0.1.3rc1/test/__init__.py\npartis_pyproj-0.1.3rc1/test/pkg_meson_2/src/test_pkg/pure_mod.py\npartis_pyproj-0.1.3rc1/test/pkg_meson_2/src/test_pkg/plat_mod.pyx\npartis_pyproj-0.1.3rc1/test/pkg_meson_2/meson.build\npartis_pyproj-0.1.3rc1/test/pkg_meson_2/meson_options.txt\npartis_pyproj-0.1.3rc1/test/pkg_meson_2/pyproject.toml\npartis_pyproj-0.1.3rc1/test/pkg_bad_2/src/test_pkg/sub_mod/sub_sub_mod/good_file.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_2/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_2/src/test_pkg/pure_mod/pure_mod.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_2/pkgaux/__init__.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_2/pyproject.toml\npartis_pyproj-0.1.3rc1/test/__main__.py\npartis_pyproj-0.1.3rc1/test/test_03_dist.py\npartis_pyproj-0.1.3rc1/test/sitecustom/partis-sitecustom.pth\npartis_pyproj-0.1.3rc1/test/sitecustom/pyproject.toml\npartis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/bad_link/src/test_pkg/pure_mod.py\npartis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/bad_link/src/test_pkg/plat_mod.pyx\npartis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/bad_link/meson.build\npartis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/bad_link/meson_options.txt\npartis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/bad_link/pyproject.toml\npartis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/src/test_pkg/pure_mod.py\npartis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/src/test_pkg/plat_mod.pyx\npartis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/meson.build\npartis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/meson_options.txt\npartis_pyproj-0.1.3rc1/test/pkg_meson_bad_1/pyproject.toml\npartis_pyproj-0.1.3rc1/test/pkg_min/pure_mod.py\npartis_pyproj-0.1.3rc1/test/pkg_min/pyproject.toml\npartis_pyproj-0.1.3rc1/test/noxfile.py\npartis_pyproj-0.1.3rc1/test/test_00_validate.py\npartis_pyproj-0.1.3rc1/test/test_04_load_module.py\npartis_pyproj-0.1.3rc1/test/pkg_cmake_1/src/test_pkg/pure_mod.py\npartis_pyproj-0.1.3rc1/test/pkg_cmake_1/src/test_pkg/plat_mod.pyx\npartis_pyproj-0.1.3rc1/test/pkg_cmake_1/src/test_pkg/CMakeLists.txt\npartis_pyproj-0.1.3rc1/test/pkg_cmake_1/CMakeLists.txt\npartis_pyproj-0.1.3rc1/test/pkg_cmake_1/pyproject.toml\npartis_pyproj-0.1.3rc1/test/test_01_norms.py\npartis_pyproj-0.1.3rc1/test/test_05_pkginfo.py\npartis_pyproj-0.1.3rc1/test/pkg_base/src/test_pkg/sub_mod/sub_sub_mod/good_file.py\npartis_pyproj-0.1.3rc1/test/pkg_base/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py\npartis_pyproj-0.1.3rc1/test/pkg_base/src/test_pkg/sub_mod/good_file.py\npartis_pyproj-0.1.3rc1/test/pkg_base/src/test_pkg/sub_mod/bad_file.py\npartis_pyproj-0.1.3rc1/test/pkg_base/src/test_pkg/pure_mod/pure_mod.py\npartis_pyproj-0.1.3rc1/test/pkg_base/pkgaux/__init__.py\npartis_pyproj-0.1.3rc1/test/pkg_base/pyproject.toml\npartis_pyproj-0.1.3rc1/test/test_06_pyproj.py\npartis_pyproj-0.1.3rc1/test/test_02_path.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_3/pyproject.toml\npartis_pyproj-0.1.3rc1/test/pkg_meson_1/src/test_pkg/pure_mod.py\npartis_pyproj-0.1.3rc1/test/pkg_meson_1/src/test_pkg/plat_mod.pyx\npartis_pyproj-0.1.3rc1/test/pkg_meson_1/meson.build\npartis_pyproj-0.1.3rc1/test/pkg_meson_1/meson_options.txt\npartis_pyproj-0.1.3rc1/test/pkg_meson_1/pyproject.toml\npartis_pyproj-0.1.3rc1/test/test_07_backend.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_4/src/test_pkg/sub_mod/sub_sub_mod/good_file.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_4/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_4/src/test_pkg/pure_mod/pure_mod.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_4/pkgaux/__init__.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_4/pyproject.toml\npartis_pyproj-0.1.3rc1/test/pkg_bad_1/src/test_pkg/sub_mod/sub_sub_mod/good_file.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_1/src/test_pkg/sub_mod/sub_sub_mod/bad_file.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_1/src/test_pkg/pure_mod/pure_mod.py\npartis_pyproj-0.1.3rc1/test/pkg_bad_1/pyproject.toml\npartis_pyproj-0.1.3rc1/pyproject.toml\npartis_pyproj-0.1.3rc1/LICENSE.txt\npartis_pyproj-0.1.3rc1/README.rst'
 
 TOP_LEVEL = b''
 
 ENTRY_POINTS = b''
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
```

### Comparing `partis_pyproj-0.1.1/PKG-INFO` & `partis_pyproj-0.1.3rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 Metadata-Version: 2.1
 Name: partis-pyproj
-Version: 0.1.1
+Version: 0.1.3rc1
 Requires-Python: >=3.6.2
 Author-email: "Nanohmics Inc." <software.support@nanohmics.com>
 Maintainer-email: "Nanohmics Inc." <software.support@nanohmics.com>
 Summary: Minimal set of Python project utilities (PEP-517/621)
 License-File: LICENSE.txt
-Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Microsoft :: Windows
 Provides-Extra: meson
 Provides-Extra: cmake
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: cov
 Provides-Extra: lint
-Requires-Dist: importlib_metadata; python_version < "3.8"
+Requires-Dist: tomli>=1.2.3
 Requires-Dist: packaging==21.3
+Requires-Dist: importlib_metadata; python_version < "3.8"
 Requires-Dist: wheel
-Requires-Dist: tomli>=1.2.3
 Requires-Dist: meson>=0.61.3; extra == "meson"
 Requires-Dist: ninja>=1.10.2.3; extra == "meson"
-Requires-Dist: cmake>=3.24.3; extra == "cmake"
 Requires-Dist: ninja>=1.10.2.3; extra == "cmake"
-Requires-Dist: partis-utils[sphinx]>=0.1.0; extra == "doc"
-Requires-Dist: build>=0.7.0; extra == "test"
-Requires-Dist: ninja>=1.10.2.3; extra == "test"
-Requires-Dist: tomli>=1.2.3; extra == "test"
-Requires-Dist: coverage[toml]>=6.2; extra == "test"
-Requires-Dist: pip>=18.1; extra == "test"
-Requires-Dist: pytest-cov>=3.0.0; extra == "test"
+Requires-Dist: cmake>=3.24.3; extra == "cmake"
+Requires-Dist: partis-utils[sphinx]>=0.1.3rc1; extra == "doc"
+Requires-Dist: meson>=0.61.3; extra == "test"
 Requires-Dist: numpy; extra == "test"
-Requires-Dist: pytest_mock>=3.6.1; extra == "test"
+Requires-Dist: pip>=18.1; extra == "test"
+Requires-Dist: coverage[toml]>=6.2; extra == "test"
+Requires-Dist: nox>=2021.10.1; extra == "test"
+Requires-Dist: tomli>=1.2.3; extra == "test"
 Requires-Dist: cmake>=3.24.3; extra == "test"
 Requires-Dist: Cython>=0.29.18; extra == "test"
-Requires-Dist: meson>=0.61.3; extra == "test"
+Requires-Dist: ninja>=1.10.2.3; extra == "test"
+Requires-Dist: pytest_mock>=3.6.1; extra == "test"
+Requires-Dist: build>=0.7.0; extra == "test"
 Requires-Dist: pytest>=6.2.5; extra == "test"
-Requires-Dist: nox>=2021.10.1; extra == "test"
+Requires-Dist: pytest-cov>=3.0.0; extra == "test"
 Requires-Dist: coverage[toml]>=6.2; extra == "cov"
 Requires-Dist: pyflakes==2.4.0; extra == "lint"
 Description-Content-Type: text/x-rst
 
 The ``partis.pyproj`` package aims to be very simple and
 transparent implementation of a PEP-517 build back-end.
```

