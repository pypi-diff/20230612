# Comparing `tmp/autogalaxy-2023.6.12.4.tar.gz` & `tmp/autogalaxy-2023.6.12.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogalaxy-2023.6.12.4.tar", last modified: Mon Jun 12 13:49:04 2023, max compression
+gzip compressed data, was "autogalaxy-2023.6.12.5.tar", last modified: Mon Jun 12 14:10:16 2023, max compression
```

## Comparing `autogalaxy-2023.6.12.4.tar` & `autogalaxy-2023.6.12.5.tar`

### file list

```diff
@@ -1,356 +1,356 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.238565 autogalaxy-2023.6.12.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/CITATIONS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-06-12 13:49:04.238565 autogalaxy-2023.6.12.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.194564 autogalaxy-2023.6.12.4/autogalaxy/
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-06-12 13:48:55.000000 autogalaxy-2023.6.12.4/autogalaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/abstract_fit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.198564 autogalaxy-2023.6.12.4/autogalaxy/aggregator/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/aggregator/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/aggregator/fit_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/aggregator/fit_interferometer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/aggregator/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/aggregator/interferometer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/aggregator/plane.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.198564 autogalaxy-2023.6.12.4/autogalaxy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/analysis/chaining_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/analysis/clump_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/analysis/maker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.198564 autogalaxy-2023.6.12.4/autogalaxy/analysis/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/analysis/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/analysis/mock/mock_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/analysis/model_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/analysis/preloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/analysis/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/analysis/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19568 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/analysis/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.198564 autogalaxy-2023.6.12.4/autogalaxy/config/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/general.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/grids.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/notation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.202564 autogalaxy-2023.6.12.4/autogalaxy/config/priors/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/basis.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/cosmology.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.202564 autogalaxy-2023.6.12.4/autogalaxy/config/priors/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/galaxy/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/galaxy/redshift.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.202564 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.202564 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/chameleon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/eff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/exponential_core.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/moffat.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/sersic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/sersic_core.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.202564 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear_operated/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear_operated/gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear_operated/moffat.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.202564 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/operated/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/operated/gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/operated/moffat.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/operated/sersic.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.202564 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/shapelets/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/shapelets/cartesian.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/shapelets/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/shapelets/polar.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.202564 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/chameleon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/eff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/exponential_core.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/moffat.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/sersic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/sersic_core.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.206565 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.206565 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/gnfw.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/nfw.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.206565 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/point/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/point/point.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/point/smbh.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/point/smbh_binary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.206565 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/sheets/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/sheets/external_shear.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.206565 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/chameleon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/sersic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/sersic_core.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.206565 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/total/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/total/isothermal.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/total/isothermal_core.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/total/power_law.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/total/power_law_broken.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/total/power_law_core.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/total/power_law_multipole.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.206565 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mesh/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mesh/delaunay.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mesh/rectangular.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mesh/voronoi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/mesh/voronoi_nn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/point_sources.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.214564 autogalaxy-2023.6.12.4/autogalaxy/config/priors/regularization/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/regularization/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/regularization/adaptive_brightness.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/regularization/constant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/regularization/constant_split.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/regularization/constant_zeroth.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/priors/regularization/zeroth.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.214564 autogalaxy-2023.6.12.4/autogalaxy/config/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/visualize/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/visualize/general.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/visualize/include.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/visualize/mat_wrap_1d.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/visualize/mat_wrap_2d.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/config/visualize/plots.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.214564 autogalaxy-2023.6.12.4/autogalaxy/cosmology/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/cosmology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13974 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/cosmology/lensing.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/cosmology/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/cosmology/wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.214564 autogalaxy-2023.6.12.4/autogalaxy/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/galaxy/galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.214564 autogalaxy-2023.6.12.4/autogalaxy/galaxy/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/galaxy/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/galaxy/mock/mock_galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.214564 autogalaxy-2023.6.12.4/autogalaxy/galaxy/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/galaxy/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/galaxy/plot/adapt_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    40501 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/galaxy/plot/galaxy_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/galaxy/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/galaxy/stellar_dark_decomp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.214564 autogalaxy-2023.6.12.4/autogalaxy/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/gui/clicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/gui/scribbler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.214564 autogalaxy-2023.6.12.4/autogalaxy/imaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/imaging/fit_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/imaging/imaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.214564 autogalaxy-2023.6.12.4/autogalaxy/imaging/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/imaging/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18865 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/imaging/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/imaging/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/imaging/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.214564 autogalaxy-2023.6.12.4/autogalaxy/imaging/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/imaging/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/imaging/plot/fit_imaging_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.218565 autogalaxy-2023.6.12.4/autogalaxy/interferometer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/interferometer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/interferometer/fit_interferometer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/interferometer/interferometer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.218565 autogalaxy-2023.6.12.4/autogalaxy/interferometer/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/interferometer/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/interferometer/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/interferometer/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/interferometer/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.222565 autogalaxy-2023.6.12.4/autogalaxy/interferometer/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/interferometer/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/interferometer/plot/fit_interferometer_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.222565 autogalaxy-2023.6.12.4/autogalaxy/operate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/operate/deflections.py
--rw-r--r--   0 runner    (1001) docker     (123)    20242 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/operate/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.222565 autogalaxy-2023.6.12.4/autogalaxy/plane/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plane/plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plane/plane_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.222565 autogalaxy-2023.6.12.4/autogalaxy/plane/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plane/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plane/plot/plane_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plane/to_inversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.222565 autogalaxy-2023.6.12.4/autogalaxy/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/abstract_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.222565 autogalaxy-2023.6.12.4/autogalaxy/plot/get_visuals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/get_visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/get_visuals/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/get_visuals/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.222565 autogalaxy-2023.6.12.4/autogalaxy/plot/include/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/include/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/include/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/include/two_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/mass_plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.222565 autogalaxy-2023.6.12.4/autogalaxy/plot/mat_plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/mat_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/mat_plot/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/mat_plot/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.226565 autogalaxy-2023.6.12.4/autogalaxy/plot/visuals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/visuals/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/visuals/two_d.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/plot/wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.226565 autogalaxy-2023.6.12.4/autogalaxy/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/geometry_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.226565 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.226565 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/chameleon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/dev_vaucouleurs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/eff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/exponential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/exponential_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/moffat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/sersic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/sersic_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.226565 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear_operated/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear_operated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear_operated/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear_operated/moffat.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear_operated/sersic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.226565 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/mock/mock_light_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.230565 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/operated/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/operated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/operated/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/operated/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/operated/moffat.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/operated/sersic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.230565 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/shapelets/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/shapelets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/shapelets/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/shapelets/cartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/shapelets/exponential.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/shapelets/polar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.230565 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/chameleon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/dev_vaucouleurs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/eff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/exponential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/sersic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/sersic_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.230565 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/chameleon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/dev_vaucouleurs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/eff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/exponential.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/exponential_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/moffat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/sersic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/sersic_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    25207 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/light_and_mass_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.230565 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.230565 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/abstract/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/abstract/cse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/abstract/mge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.234565 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/gnfw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/gnfw_mcr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/mcr_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/nfw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/nfw_mcr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/nfw_truncated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.234565 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/mock/mock_mass_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.234565 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/point/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/point/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/point/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/point/smbh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/point/smbh_binary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.234565 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/sheets/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/sheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/sheets/external_shear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/sheets/input_deflections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/sheets/mass_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.234565 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/chameleon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/exponential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    16715 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/sersic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/sersic_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.238565 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/isothermal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/isothermal_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/power_law.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/power_law_broken.py
--rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/power_law_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/power_law_multipole.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.238565 autogalaxy-2023.6.12.4/autogalaxy/profiles/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/plot/light_profile_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/plot/mass_profile_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/point_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/profiles/scaling_relations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.238565 autogalaxy-2023.6.12.4/autogalaxy/quantity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/quantity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/quantity/dataset_quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/quantity/fit_quantity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.238565 autogalaxy-2023.6.12.4/autogalaxy/quantity/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/quantity/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/quantity/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/quantity/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/quantity/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.238565 autogalaxy-2023.6.12.4/autogalaxy/quantity/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/quantity/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/quantity/plot/fit_quantity_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.238565 autogalaxy-2023.6.12.4/autogalaxy/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/util/error_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.238565 autogalaxy-2023.6.12.4/autogalaxy/util/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/util/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/util/mock/mock_cosmology.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-12 13:48:54.000000 autogalaxy-2023.6.12.4/autogalaxy/util/shear_field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.238565 autogalaxy-2023.6.12.4/autogalaxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-12 13:49:04.000000 autogalaxy-2023.6.12.4/autogalaxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 13:48:55.000000 autogalaxy-2023.6.12.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 13:48:55.000000 autogalaxy-2023.6.12.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:49:04.238565 autogalaxy-2023.6.12.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-12 13:48:55.000000 autogalaxy-2023.6.12.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.310654 autogalaxy-2023.6.12.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/CITATIONS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-06-12 14:10:16.310654 autogalaxy-2023.6.12.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.278654 autogalaxy-2023.6.12.5/autogalaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/abstract_fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.282654 autogalaxy-2023.6.12.5/autogalaxy/aggregator/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/aggregator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/aggregator/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/aggregator/fit_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/aggregator/fit_interferometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/aggregator/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/aggregator/interferometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/aggregator/plane.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.282654 autogalaxy-2023.6.12.5/autogalaxy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/analysis/chaining_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/analysis/clump_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/analysis/maker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.282654 autogalaxy-2023.6.12.5/autogalaxy/analysis/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/analysis/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/analysis/mock/mock_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/analysis/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/analysis/preloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/analysis/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/analysis/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19568 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/analysis/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.282654 autogalaxy-2023.6.12.5/autogalaxy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/general.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/grids.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/notation.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.282654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/basis.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/cosmology.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.282654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/galaxy/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/galaxy/redshift.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.282654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.286654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/chameleon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/eff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/exponential_core.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/gaussian.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/moffat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/sersic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/sersic_core.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.286654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear_operated/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear_operated/gaussian.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear_operated/moffat.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.286654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/operated/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/operated/gaussian.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/operated/moffat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/operated/sersic.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.286654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/shapelets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/shapelets/cartesian.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/shapelets/exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/shapelets/polar.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.286654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/chameleon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/eff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/exponential_core.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/gaussian.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/moffat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/sersic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/sersic_core.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.286654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.286654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/gnfw.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/nfw.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.286654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/point/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/point/point.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/point/smbh.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/point/smbh_binary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.286654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/sheets/external_shear.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.286654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/chameleon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/gaussian.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/sersic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/sersic_core.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.290654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/total/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/total/isothermal.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/total/isothermal_core.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/total/power_law.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/total/power_law_broken.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/total/power_law_core.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/total/power_law_multipole.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.290654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mesh/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mesh/delaunay.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mesh/rectangular.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mesh/voronoi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/mesh/voronoi_nn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/point_sources.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.290654 autogalaxy-2023.6.12.5/autogalaxy/config/priors/regularization/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/regularization/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/regularization/adaptive_brightness.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/regularization/constant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/regularization/constant_split.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/regularization/constant_zeroth.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/priors/regularization/zeroth.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.290654 autogalaxy-2023.6.12.5/autogalaxy/config/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/visualize/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/visualize/general.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/visualize/include.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/visualize/mat_wrap_1d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/visualize/mat_wrap_2d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/config/visualize/plots.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.290654 autogalaxy-2023.6.12.5/autogalaxy/cosmology/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/cosmology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13974 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/cosmology/lensing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/cosmology/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/cosmology/wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.290654 autogalaxy-2023.6.12.5/autogalaxy/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/galaxy/galaxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.290654 autogalaxy-2023.6.12.5/autogalaxy/galaxy/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/galaxy/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/galaxy/mock/mock_galaxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.290654 autogalaxy-2023.6.12.5/autogalaxy/galaxy/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/galaxy/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/galaxy/plot/adapt_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40501 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/galaxy/plot/galaxy_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/galaxy/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/galaxy/stellar_dark_decomp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.294654 autogalaxy-2023.6.12.5/autogalaxy/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/gui/clicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/gui/scribbler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.294654 autogalaxy-2023.6.12.5/autogalaxy/imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/imaging/fit_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/imaging/imaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.294654 autogalaxy-2023.6.12.5/autogalaxy/imaging/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/imaging/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18865 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/imaging/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/imaging/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/imaging/model/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.294654 autogalaxy-2023.6.12.5/autogalaxy/imaging/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/imaging/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/imaging/plot/fit_imaging_plotters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.294654 autogalaxy-2023.6.12.5/autogalaxy/interferometer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/interferometer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/interferometer/fit_interferometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/interferometer/interferometer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.294654 autogalaxy-2023.6.12.5/autogalaxy/interferometer/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/interferometer/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/interferometer/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/interferometer/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/interferometer/model/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.294654 autogalaxy-2023.6.12.5/autogalaxy/interferometer/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/interferometer/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/interferometer/plot/fit_interferometer_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.294654 autogalaxy-2023.6.12.5/autogalaxy/operate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/operate/deflections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20242 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/operate/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.294654 autogalaxy-2023.6.12.5/autogalaxy/plane/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plane/plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plane/plane_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.294654 autogalaxy-2023.6.12.5/autogalaxy/plane/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plane/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plane/plot/plane_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plane/to_inversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.294654 autogalaxy-2023.6.12.5/autogalaxy/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/abstract_plotters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.294654 autogalaxy-2023.6.12.5/autogalaxy/plot/get_visuals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/get_visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/get_visuals/one_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/get_visuals/two_d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.294654 autogalaxy-2023.6.12.5/autogalaxy/plot/include/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/include/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/include/one_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/include/two_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/mass_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.298654 autogalaxy-2023.6.12.5/autogalaxy/plot/mat_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/mat_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/mat_plot/one_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/mat_plot/two_d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.298654 autogalaxy-2023.6.12.5/autogalaxy/plot/visuals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/visuals/one_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/visuals/two_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/plot/wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.298654 autogalaxy-2023.6.12.5/autogalaxy/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/geometry_profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.298654 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.298654 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/chameleon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/dev_vaucouleurs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/eff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/exponential_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/moffat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/sersic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/sersic_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.298654 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear_operated/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear_operated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear_operated/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear_operated/moffat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear_operated/sersic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.298654 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/mock/mock_light_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.298654 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/operated/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/operated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/operated/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/operated/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/operated/moffat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/operated/sersic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.302654 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/shapelets/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/shapelets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/shapelets/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/shapelets/cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/shapelets/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/shapelets/polar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.302654 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/chameleon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/dev_vaucouleurs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/eff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/sersic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/sersic_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.302654 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/chameleon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/dev_vaucouleurs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/eff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/exponential_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/moffat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/sersic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/sersic_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25207 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/light_and_mass_profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.302654 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.302654 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/abstract/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/abstract/cse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/abstract/mge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.302654 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/gnfw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/gnfw_mcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/mcr_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/nfw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/nfw_mcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/nfw_truncated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.306654 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/mock/mock_mass_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.306654 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/point/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/point/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/point/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/point/smbh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/point/smbh_binary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.306654 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/sheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/sheets/external_shear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/sheets/input_deflections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/sheets/mass_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.306654 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/chameleon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16715 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/sersic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/sersic_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.306654 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/isothermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/isothermal_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/power_law.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/power_law_broken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/power_law_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/power_law_multipole.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.306654 autogalaxy-2023.6.12.5/autogalaxy/profiles/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/plot/light_profile_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/plot/mass_profile_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/point_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/profiles/scaling_relations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.306654 autogalaxy-2023.6.12.5/autogalaxy/quantity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/quantity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/quantity/dataset_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/quantity/fit_quantity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.306654 autogalaxy-2023.6.12.5/autogalaxy/quantity/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/quantity/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/quantity/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/quantity/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/quantity/model/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.306654 autogalaxy-2023.6.12.5/autogalaxy/quantity/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/quantity/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/quantity/plot/fit_quantity_plotters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.310654 autogalaxy-2023.6.12.5/autogalaxy/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/util/error_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.310654 autogalaxy-2023.6.12.5/autogalaxy/util/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/util/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/util/mock/mock_cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/autogalaxy/util/shear_field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:16.310654 autogalaxy-2023.6.12.5/autogalaxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-12 14:10:16.000000 autogalaxy-2023.6.12.5/autogalaxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:10:16.310654 autogalaxy-2023.6.12.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-12 14:10:05.000000 autogalaxy-2023.6.12.5/setup.py
```

### Comparing `autogalaxy-2023.6.12.4/CITATIONS.rst` & `autogalaxy-2023.6.12.5/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/LICENSE` & `autogalaxy-2023.6.12.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/PKG-INFO` & `autogalaxy-2023.6.12.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogalaxy
-Version: 2023.6.12.4
+Version: 2023.6.12.5
 Summary: Open-Source Multi Wavelength Galaxy Structure & Morphology
 Home-page: https://github.com/Jammy2211/PyAutoGalaxy
 Author: James Nightingale and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
```

### Comparing `autogalaxy-2023.6.12.4/README.rst` & `autogalaxy-2023.6.12.5/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/__init__.py` & `autogalaxy-2023.6.12.5/autogalaxy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,8 +105,8 @@
 
 from .analysis.clump_model import ClumpModel
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2023.6.12.4"
+__version__ = "2023.6.12.5"
```

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/abstract_fit.py` & `autogalaxy-2023.6.12.5/autogalaxy/abstract_fit.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/aggregator/abstract.py` & `autogalaxy-2023.6.12.5/autogalaxy/aggregator/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/aggregator/fit_imaging.py` & `autogalaxy-2023.6.12.5/autogalaxy/aggregator/fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/aggregator/fit_interferometer.py` & `autogalaxy-2023.6.12.5/autogalaxy/aggregator/fit_interferometer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/aggregator/imaging.py` & `autogalaxy-2023.6.12.5/autogalaxy/aggregator/imaging.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/aggregator/interferometer.py` & `autogalaxy-2023.6.12.5/autogalaxy/aggregator/interferometer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/aggregator/plane.py` & `autogalaxy-2023.6.12.5/autogalaxy/aggregator/plane.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/analysis/analysis.py` & `autogalaxy-2023.6.12.5/autogalaxy/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/analysis/chaining_util.py` & `autogalaxy-2023.6.12.5/autogalaxy/analysis/chaining_util.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/analysis/clump_model.py` & `autogalaxy-2023.6.12.5/autogalaxy/analysis/clump_model.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/analysis/maker.py` & `autogalaxy-2023.6.12.5/autogalaxy/analysis/maker.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/analysis/mock/mock_result.py` & `autogalaxy-2023.6.12.5/autogalaxy/analysis/mock/mock_result.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/analysis/model_util.py` & `autogalaxy-2023.6.12.5/autogalaxy/analysis/model_util.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/analysis/preloads.py` & `autogalaxy-2023.6.12.5/autogalaxy/analysis/preloads.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/analysis/result.py` & `autogalaxy-2023.6.12.5/autogalaxy/analysis/result.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/analysis/setup.py` & `autogalaxy-2023.6.12.5/autogalaxy/analysis/setup.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/analysis/visualizer.py` & `autogalaxy-2023.6.12.5/autogalaxy/analysis/visualizer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/README.rst` & `autogalaxy-2023.6.12.5/autogalaxy/config/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/grids.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/grids.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/notation.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/notation.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/README.rst` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/cosmology.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/cosmology.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/README.rst` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/chameleon.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/chameleon.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/eff.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/eff.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/exponential.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/exponential_core.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/exponential_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/gaussian.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/moffat.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/sersic.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear/sersic_core.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear/sersic_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear_operated/gaussian.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear_operated/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/linear_operated/moffat.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/linear_operated/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/operated/gaussian.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/operated/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/operated/moffat.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/operated/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/operated/sersic.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/operated/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/shapelets/cartesian.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/shapelets/cartesian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/shapelets/exponential.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/shapelets/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/shapelets/polar.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/shapelets/polar.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/chameleon.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/chameleon.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/eff.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/eff.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/exponential.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/exponential_core.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/exponential_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/gaussian.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/moffat.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/sersic.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/light/standard/sersic_core.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/light/standard/sersic_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/README.rst` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/gnfw.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/gnfw.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/nfw.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/nfw.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/point/point.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/point/point.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/point/smbh.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/point/smbh.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/point/smbh_binary.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/point/smbh_binary.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/chameleon.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/chameleon.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/exponential.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/gaussian.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/sersic.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/sersic_core.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/sersic_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/total/isothermal.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/total/isothermal.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/total/isothermal_core.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/total/isothermal_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/total/power_law.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/total/power_law.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/total/power_law_broken.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/total/power_law_broken.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/total/power_law_core.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/total/power_law_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mass/total/power_law_multipole.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mass/total/power_law_multipole.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mesh/delaunay.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mesh/delaunay.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mesh/voronoi.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mesh/voronoi.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/mesh/voronoi_nn.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/mesh/voronoi_nn.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/point_sources.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/point_sources.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/regularization/adaptive_brightness.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/regularization/adaptive_brightness.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/visualize/README.rst` & `autogalaxy-2023.6.12.5/autogalaxy/config/visualize/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/visualize/mat_wrap_2d.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/visualize/mat_wrap_2d.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/config/visualize/plots.yaml` & `autogalaxy-2023.6.12.5/autogalaxy/config/visualize/plots.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/convert.py` & `autogalaxy-2023.6.12.5/autogalaxy/convert.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/cosmology/lensing.py` & `autogalaxy-2023.6.12.5/autogalaxy/cosmology/lensing.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/cosmology/model.py` & `autogalaxy-2023.6.12.5/autogalaxy/cosmology/model.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/cosmology/wrap.py` & `autogalaxy-2023.6.12.5/autogalaxy/cosmology/wrap.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/exc.py` & `autogalaxy-2023.6.12.5/autogalaxy/exc.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/fixtures.py` & `autogalaxy-2023.6.12.5/autogalaxy/fixtures.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/galaxy/galaxy.py` & `autogalaxy-2023.6.12.5/autogalaxy/galaxy/galaxy.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/galaxy/mock/mock_galaxy.py` & `autogalaxy-2023.6.12.5/autogalaxy/galaxy/mock/mock_galaxy.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/galaxy/plot/adapt_plotters.py` & `autogalaxy-2023.6.12.5/autogalaxy/galaxy/plot/adapt_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/galaxy/plot/galaxy_plotters.py` & `autogalaxy-2023.6.12.5/autogalaxy/galaxy/plot/galaxy_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/galaxy/redshift.py` & `autogalaxy-2023.6.12.5/autogalaxy/galaxy/redshift.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/galaxy/stellar_dark_decomp.py` & `autogalaxy-2023.6.12.5/autogalaxy/galaxy/stellar_dark_decomp.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/gui/clicker.py` & `autogalaxy-2023.6.12.5/autogalaxy/gui/clicker.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/gui/scribbler.py` & `autogalaxy-2023.6.12.5/autogalaxy/gui/scribbler.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/imaging/fit_imaging.py` & `autogalaxy-2023.6.12.5/autogalaxy/imaging/fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/imaging/imaging.py` & `autogalaxy-2023.6.12.5/autogalaxy/imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/imaging/model/analysis.py` & `autogalaxy-2023.6.12.5/autogalaxy/imaging/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/imaging/model/result.py` & `autogalaxy-2023.6.12.5/autogalaxy/imaging/model/result.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/imaging/model/visualizer.py` & `autogalaxy-2023.6.12.5/autogalaxy/imaging/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/imaging/plot/fit_imaging_plotters.py` & `autogalaxy-2023.6.12.5/autogalaxy/imaging/plot/fit_imaging_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/interferometer/fit_interferometer.py` & `autogalaxy-2023.6.12.5/autogalaxy/interferometer/fit_interferometer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/interferometer/interferometer.py` & `autogalaxy-2023.6.12.5/autogalaxy/interferometer/interferometer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/interferometer/model/analysis.py` & `autogalaxy-2023.6.12.5/autogalaxy/interferometer/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/interferometer/model/result.py` & `autogalaxy-2023.6.12.5/autogalaxy/interferometer/model/result.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/interferometer/model/visualizer.py` & `autogalaxy-2023.6.12.5/autogalaxy/interferometer/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/interferometer/plot/fit_interferometer_plotters.py` & `autogalaxy-2023.6.12.5/autogalaxy/interferometer/plot/fit_interferometer_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/operate/deflections.py` & `autogalaxy-2023.6.12.5/autogalaxy/operate/deflections.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/operate/image.py` & `autogalaxy-2023.6.12.5/autogalaxy/operate/image.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plane/__init__.py` & `autogalaxy-2023.6.12.5/autogalaxy/plane/__init__.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plane/plane.py` & `autogalaxy-2023.6.12.5/autogalaxy/plane/plane.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plane/plane_util.py` & `autogalaxy-2023.6.12.5/autogalaxy/plane/plane_util.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plane/plot/plane_plotters.py` & `autogalaxy-2023.6.12.5/autogalaxy/plane/plot/plane_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plane/to_inversion.py` & `autogalaxy-2023.6.12.5/autogalaxy/plane/to_inversion.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plot/__init__.py` & `autogalaxy-2023.6.12.5/autogalaxy/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plot/abstract_plotters.py` & `autogalaxy-2023.6.12.5/autogalaxy/plot/abstract_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plot/get_visuals/one_d.py` & `autogalaxy-2023.6.12.5/autogalaxy/plot/get_visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plot/get_visuals/two_d.py` & `autogalaxy-2023.6.12.5/autogalaxy/plot/get_visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plot/include/one_d.py` & `autogalaxy-2023.6.12.5/autogalaxy/plot/include/one_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plot/include/two_d.py` & `autogalaxy-2023.6.12.5/autogalaxy/plot/include/two_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plot/mass_plotter.py` & `autogalaxy-2023.6.12.5/autogalaxy/plot/mass_plotter.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plot/mat_plot/one_d.py` & `autogalaxy-2023.6.12.5/autogalaxy/plot/mat_plot/one_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plot/mat_plot/two_d.py` & `autogalaxy-2023.6.12.5/autogalaxy/plot/mat_plot/two_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plot/visuals/one_d.py` & `autogalaxy-2023.6.12.5/autogalaxy/plot/visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plot/visuals/two_d.py` & `autogalaxy-2023.6.12.5/autogalaxy/plot/visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/plot/wrap.py` & `autogalaxy-2023.6.12.5/autogalaxy/plot/wrap.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/geometry_profiles.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/geometry_profiles.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/abstract.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/basis.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/basis.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/decorators.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/decorators.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/abstract.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/dev_vaucouleurs.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/exponential.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/exponential_core.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/exponential_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/gaussian.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/gaussian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/moffat.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/moffat.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/sersic.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/sersic.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/linear/sersic_core.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/linear/sersic_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/mock/mock_light_profile.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/mock/mock_light_profile.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/shapelets/abstract.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/shapelets/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/shapelets/cartesian.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/shapelets/cartesian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/shapelets/exponential.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/shapelets/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/shapelets/polar.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/shapelets/polar.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/abstract.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/chameleon.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/chameleon.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/dev_vaucouleurs.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/eff.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/eff.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/exponential.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/gaussian.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/gaussian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/sersic.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/sersic.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/snr/sersic_core.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/snr/sersic_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/chameleon.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/chameleon.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/dev_vaucouleurs.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/eff.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/eff.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/exponential.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/exponential_core.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/exponential_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/gaussian.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/gaussian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/moffat.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/moffat.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/sersic.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/sersic.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light/standard/sersic_core.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light/standard/sersic_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/light_and_mass_profiles.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/light_and_mass_profiles.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/__init__.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/__init__.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/abstract/abstract.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/abstract/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/abstract/cse.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/abstract/cse.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/abstract/mge.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/abstract/mge.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/abstract.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/gnfw.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/gnfw.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/gnfw_mcr.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/gnfw_mcr.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/mcr_util.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/mcr_util.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/nfw.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/nfw.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/nfw_mcr.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/nfw_mcr.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/nfw_truncated.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/nfw_truncated.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/mock/mock_mass_profile.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/mock/mock_mass_profile.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/point/point.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/point/point.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/point/smbh.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/point/smbh.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/point/smbh_binary.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/point/smbh_binary.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/sheets/external_shear.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/sheets/external_shear.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/sheets/input_deflections.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/sheets/input_deflections.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/sheets/mass_sheet.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/sheets/mass_sheet.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/chameleon.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/chameleon.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/exponential.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/gaussian.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/gaussian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/sersic.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/sersic.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/sersic_core.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/sersic_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/isothermal.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/isothermal.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/isothermal_core.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/isothermal_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/power_law.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/power_law.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/power_law_broken.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/power_law_broken.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/power_law_core.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/power_law_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/mass/total/power_law_multipole.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/mass/total/power_law_multipole.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/plot/light_profile_plotters.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/plot/light_profile_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/plot/mass_profile_plotters.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/plot/mass_profile_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/profiles/scaling_relations.py` & `autogalaxy-2023.6.12.5/autogalaxy/profiles/scaling_relations.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/quantity/dataset_quantity.py` & `autogalaxy-2023.6.12.5/autogalaxy/quantity/dataset_quantity.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/quantity/fit_quantity.py` & `autogalaxy-2023.6.12.5/autogalaxy/quantity/fit_quantity.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/quantity/model/analysis.py` & `autogalaxy-2023.6.12.5/autogalaxy/quantity/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/quantity/model/result.py` & `autogalaxy-2023.6.12.5/autogalaxy/quantity/model/result.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/quantity/model/visualizer.py` & `autogalaxy-2023.6.12.5/autogalaxy/quantity/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/quantity/plot/fit_quantity_plotters.py` & `autogalaxy-2023.6.12.5/autogalaxy/quantity/plot/fit_quantity_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/util/__init__.py` & `autogalaxy-2023.6.12.5/autogalaxy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/util/error_util.py` & `autogalaxy-2023.6.12.5/autogalaxy/util/error_util.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/util/mock/mock_cosmology.py` & `autogalaxy-2023.6.12.5/autogalaxy/util/mock/mock_cosmology.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy/util/shear_field.py` & `autogalaxy-2023.6.12.5/autogalaxy/util/shear_field.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/autogalaxy.egg-info/SOURCES.txt` & `autogalaxy-2023.6.12.5/autogalaxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.6.12.4/setup.py` & `autogalaxy-2023.6.12.5/setup.py`

 * *Files identical despite different names*

