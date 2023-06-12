# Comparing `tmp/autogalaxy-2023.7.7.1.tar.gz` & `tmp/autogalaxy-2023.7.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogalaxy-2023.7.7.1.tar", last modified: Wed Jun  7 09:47:58 2023, max compression
+gzip compressed data, was "autogalaxy-2023.7.7.2.tar", last modified: Wed Jun  7 09:59:01 2023, max compression
```

## Comparing `autogalaxy-2023.7.7.1.tar` & `autogalaxy-2023.7.7.2.tar`

### file list

```diff
@@ -1,498 +1,498 @@
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.915660 autogalaxy-2023.7.7.1/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:57.985857 autogalaxy-2023.7.7.1/.github/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.047725 autogalaxy-2023.7.7.1/.github/workflows/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      475 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/.github/workflows/draft-pdf.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3327 2022-12-19 16:37:19.000000 autogalaxy-2023.7.7.1/.github/workflows/main.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1135 2022-12-19 11:17:33.000000 autogalaxy-2023.7.7.1/CITATIONS.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18987 2022-12-20 20:59:49.000000 autogalaxy-2023.7.7.1/CODE_OF_CONDUCT.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2494 2022-12-20 20:59:49.000000 autogalaxy-2023.7.7.1/CONTRIBUTING.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1095 2020-11-16 19:58:12.000000 autogalaxy-2023.7.7.1/LICENSE
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      388 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/MANIFEST.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8400 2023-06-07 09:47:58.914628 autogalaxy-2023.7.7.1/PKG-INFO
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7567 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/README.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.057726 autogalaxy-2023.7.7.1/autogalaxy/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5518 2023-06-07 09:38:14.000000 autogalaxy-2023.7.7.1/autogalaxy/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7805 2023-06-03 11:22:20.000000 autogalaxy-2023.7.7.1/autogalaxy/abstract_fit.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.068740 autogalaxy-2023.7.7.1/autogalaxy/aggregator/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      308 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7129 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4541 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/fit_imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4523 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/fit_interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2653 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2844 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2746 2023-05-11 09:42:09.000000 autogalaxy-2023.7.7.1/autogalaxy/aggregator/plane.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.087762 autogalaxy-2023.7.7.1/autogalaxy/analysis/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-08-21 09:36:45.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18823 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10497 2023-06-05 13:31:36.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/chaining_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7567 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/clump_model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5029 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/maker.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.090765 autogalaxy-2023.7.7.1/autogalaxy/analysis/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3288 2023-06-05 20:15:34.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/mock/mock_result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9953 2023-06-06 14:36:29.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/model_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9842 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/preloads.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6634 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1157 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/setup.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19568 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/analysis/visualizer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.099761 autogalaxy-2023.7.7.1/autogalaxy/config/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2020-11-11 16:43:14.000000 autogalaxy-2023.7.7.1/autogalaxy/config/.gitignore
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      630 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.1/autogalaxy/config/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      493 2023-06-06 18:37:09.000000 autogalaxy-2023.7.7.1/autogalaxy/config/general.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1677 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/autogalaxy/config/grids.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3369 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/config/notation.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.108171 autogalaxy-2023.7.7.1/autogalaxy/config/priors/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1607 2022-12-16 19:52:14.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       10 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/basis.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      620 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/cosmology.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.112203 autogalaxy-2023.7.7.1/autogalaxy/config/priors/galaxy/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      253 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/galaxy/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      204 2022-12-21 16:13:37.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/galaxy/redshift.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.115116 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1012 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/README.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.138665 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2105 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/chameleon.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1739 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2097 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/eff.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1733 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/exponential.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2849 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/exponential_core.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1705 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/gaussian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2061 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/moffat.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2101 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/sersic.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3217 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/sersic_core.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.144647 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear_operated/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1271 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear_operated/gaussian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear_operated/moffat.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.152660 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1271 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/gaussian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1450 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/moffat.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1469 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/sersic.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.160864 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1815 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/cartesian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1819 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/exponential.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1807 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/polar.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.185674 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2503 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/chameleon.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2137 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2495 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/eff.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2131 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/exponential.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3241 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/exponential_core.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2103 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/gaussian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2459 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/moffat.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2499 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/sersic.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3609 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/sersic_core.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.188655 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      639 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/README.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.207151 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2457 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/gnfw.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1682 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2077 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3593 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1274 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1022 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3402 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.216761 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/point/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      640 2023-05-15 17:46:30.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/point/point.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1029 2023-05-15 17:46:30.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/point/smbh.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1604 2023-05-17 15:24:31.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/point/smbh_binary.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.222325 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/sheets/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      389 2023-01-14 17:31:13.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/sheets/external_shear.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      632 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.240286 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2921 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/chameleon.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2545 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2539 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/exponential.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1481 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/gaussian.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2907 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/sersic.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4027 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/sersic_core.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3337 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.255277 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1729 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/isothermal.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2113 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/isothermal_core.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2089 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2867 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law_broken.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2473 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law_core.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1333 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law_multipole.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.267350 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      225 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      989 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/delaunay.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      385 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/rectangular.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      987 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/voronoi.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      991 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/voronoi_nn.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1536 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/point_sources.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.282870 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      246 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/adaptive_brightness.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1087 2023-03-24 12:25:33.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      211 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/constant.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      216 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/constant_split.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      434 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/constant_zeroth.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      209 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/zeroth.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.294944 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      696 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      174 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/general.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2023-03-18 16:31:03.000000 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/include.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      259 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/mat_wrap_1d.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      947 2023-03-18 16:31:03.000000 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/mat_wrap_2d.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5385 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.1/autogalaxy/config/visualize/plots.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3774 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/convert.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.301984 autogalaxy-2023.7.7.1/autogalaxy/cosmology/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      150 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/cosmology/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13974 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.1/autogalaxy/cosmology/lensing.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      933 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/cosmology/model.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1431 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/cosmology/wrap.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3232 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/exc.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7213 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/fixtures.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.308879 autogalaxy-2023.7.7.1/autogalaxy/galaxy/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20983 2023-05-15 19:02:02.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/galaxy.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.312879 autogalaxy-2023.7.7.1/autogalaxy/galaxy/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      758 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/mock/mock_galaxy.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.317928 autogalaxy-2023.7.7.1/autogalaxy/galaxy/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4437 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/plot/adapt_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40501 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/plot/galaxy_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1002 2022-12-20 17:00:47.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/redshift.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1772 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/galaxy/stellar_dark_decomp.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.322913 autogalaxy-2023.7.7.1/autogalaxy/gui/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/gui/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2041 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/gui/clicker.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6977 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/gui/scribbler.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.327921 autogalaxy-2023.7.7.1/autogalaxy/imaging/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12738 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/fit_imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3868 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/imaging.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.335921 autogalaxy-2023.7.7.1/autogalaxy/imaging/model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16878 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/model/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3215 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/model/result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4285 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/model/visualizer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.338924 autogalaxy-2023.7.7.1/autogalaxy/imaging/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9632 2023-06-03 16:50:56.000000 autogalaxy-2023.7.7.1/autogalaxy/imaging/plot/fit_imaging_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.344759 autogalaxy-2023.7.7.1/autogalaxy/interferometer/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10643 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/fit_interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3368 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/interferometer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.352759 autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17326 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2960 2023-06-05 20:15:34.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5378 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/visualizer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.357791 autogalaxy-2023.7.7.1/autogalaxy/interferometer/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8265 2023-06-03 16:50:56.000000 autogalaxy-2023.7.7.1/autogalaxy/interferometer/plot/fit_interferometer_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      341 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/mock.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.362803 autogalaxy-2023.7.7.1/autogalaxy/operate/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/operate/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36267 2023-06-03 17:45:40.000000 autogalaxy-2023.7.7.1/autogalaxy/operate/deflections.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20198 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/operate/image.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.369913 autogalaxy-2023.7.7.1/autogalaxy/plane/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      686 2020-11-16 19:58:12.000000 autogalaxy-2023.7.7.1/autogalaxy/plane/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16202 2023-05-15 18:37:24.000000 autogalaxy-2023.7.7.1/autogalaxy/plane/plane.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8439 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plane/plane_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.372907 autogalaxy-2023.7.7.1/autogalaxy/plane/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/plane/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14120 2023-05-23 09:38:20.000000 autogalaxy-2023.7.7.1/autogalaxy/plane/plot/plane_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10432 2023-06-06 10:32:57.000000 autogalaxy-2023.7.7.1/autogalaxy/plane/to_inversion.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.380903 autogalaxy-2023.7.7.1/autogalaxy/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3398 2023-06-03 09:03:18.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      553 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/abstract_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.385903 autogalaxy-2023.7.7.1/autogalaxy/plot/get_visuals/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/get_visuals/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9924 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/get_visuals/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13590 2023-06-03 17:45:40.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/get_visuals/two_d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.391906 autogalaxy-2023.7.7.1/autogalaxy/plot/include/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/include/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1470 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/include/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2658 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/include/two_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4560 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/mass_plotter.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.397908 autogalaxy-2023.7.7.1/autogalaxy/plot/mat_plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/mat_plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6113 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/mat_plot/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10005 2023-03-18 16:31:03.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/mat_plot/two_d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.402902 autogalaxy-2023.7.7.1/autogalaxy/plot/visuals/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/visuals/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2123 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/visuals/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4140 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/visuals/two_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      646 2023-03-18 16:31:03.000000 autogalaxy-2023.7.7.1/autogalaxy/plot/wrap.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.410870 autogalaxy-2023.7.7.1/autogalaxy/profiles/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-11 16:43:14.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13967 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/geometry_profiles.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.419394 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5442 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1883 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/basis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2511 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/decorators.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.454033 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      401 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6951 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/chameleon.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1859 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/dev_vaucouleurs.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/eff.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1835 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/exponential.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1734 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/exponential_core.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1755 2023-03-16 18:34:52.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1749 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/moffat.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2223 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/sersic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2730 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/sersic_core.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.464044 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear_operated/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       99 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear_operated/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      207 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear_operated/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      203 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear_operated/moffat.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      203 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear_operated/sersic.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.468188 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1032 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/mock/mock_light_profile.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.481195 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/operated/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      143 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/operated/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       39 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/operated/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      200 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/operated/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      196 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/operated/moffat.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      196 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/operated/sersic.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.493270 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      247 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1202 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4264 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/cartesian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4501 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/exponential.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4330 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/polar.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.513288 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      371 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4007 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3255 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/chameleon.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2581 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/dev_vaucouleurs.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2782 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/eff.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2504 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/exponential.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2227 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2736 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/sersic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2338 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/sersic_core.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.537261 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      490 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5851 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/chameleon.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2351 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/dev_vaucouleurs.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4414 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/eff.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2316 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/exponential.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3188 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/exponential_core.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4052 2023-04-27 18:43:48.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4905 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/moffat.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7640 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/sersic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5734 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/sersic_core.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25207 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/light_and_mass_profiles.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.540219 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1020 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.548262 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10340 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7050 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/cse.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8675 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/mge.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.573428 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      440 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12379 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13480 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/gnfw.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1130 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/gnfw_mcr.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3352 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/mcr_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11547 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2532 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_mcr.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2090 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4410 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_truncated.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2089 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1161 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.577335 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      714 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/mock/mock_mass_profile.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.586402 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       91 2023-05-17 15:24:31.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1902 2023-05-15 17:46:30.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/point.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1653 2023-05-15 17:46:30.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/smbh.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4963 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/smbh_binary.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.596000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      127 2022-12-16 18:30:52.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2611 2023-06-06 12:57:36.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/external_shear.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4977 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/input_deflections.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1416 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/mass_sheet.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.616301 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      372 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8482 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/chameleon.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2478 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2472 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/exponential.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7629 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/gaussian.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16715 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/sersic.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7038 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/sersic_core.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9613 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.633501 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      337 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6348 2023-06-06 12:20:19.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/isothermal.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2109 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/isothermal_core.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5545 2023-06-06 12:57:36.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6460 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law_broken.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8476 2023-06-06 12:51:47.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law_core.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8585 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law_multipole.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.639502 autogalaxy-2023.7.7.1/autogalaxy/profiles/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12961 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/plot/light_profile_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14915 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/plot/mass_profile_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      467 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/point_sources.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1450 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/profiles/scaling_relations.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.645036 autogalaxy-2023.7.7.1/autogalaxy/quantity/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9901 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/dataset_quantity.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4646 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/fit_quantity.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.653791 autogalaxy-2023.7.7.1/autogalaxy/quantity/model/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/model/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10139 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/model/analysis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1747 2023-02-20 18:27:21.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/model/result.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3510 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/model/visualizer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.657797 autogalaxy-2023.7.7.1/autogalaxy/quantity/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8126 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/quantity/plot/fit_quantity_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.663799 autogalaxy-2023.7.7.1/autogalaxy/util/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1391 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/autogalaxy/util/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2572 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/util/error_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.668800 autogalaxy-2023.7.7.1/autogalaxy/util/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/autogalaxy/util/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1353 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/autogalaxy/util/mock/mock_cosmology.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3858 2023-01-13 16:57:54.000000 autogalaxy-2023.7.7.1/autogalaxy/util/shear_field.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.913466 autogalaxy-2023.7.7.1/autogalaxy.egg-info/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16633 2023-06-07 09:47:57.000000 autogalaxy-2023.7.7.1/autogalaxy.egg-info/SOURCES.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.676119 autogalaxy-2023.7.7.1/docs/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.679798 autogalaxy-2023.7.7.1/docs/_templates/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2022-12-21 16:35:52.000000 autogalaxy-2023.7.7.1/docs/_templates/custom-class-template.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/docs/_templates/custom_module_template.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.686797 autogalaxy-2023.7.7.1/docs/advanced/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      388 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/advanced/chaining.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6363 2022-12-20 22:05:13.000000 autogalaxy-2023.7.7.1/docs/advanced/database.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1374 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/docs/advanced/graphical.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.701810 autogalaxy-2023.7.7.1/docs/api/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1592 2023-01-13 16:57:54.000000 autogalaxy-2023.7.7.1/docs/api/data.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      330 2022-12-20 17:33:12.000000 autogalaxy-2023.7.7.1/docs/api/fitting.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      664 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/docs/api/galaxy.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.022475 autogalaxy-2023.7.7.1/docs/api/images/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.710809 autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41383 2022-12-21 12:27:28.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/data_image_plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34340 2022-12-21 12:27:28.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/grid_image_plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    49269 2022-12-21 12:27:49.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/image_plane_mesh.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.717924 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40349 2022-12-21 12:22:21.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/data_image_plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26453 2022-12-21 12:22:21.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/grid_image_plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48007 2022-12-21 12:28:33.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/image_plane_mesh.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.725737 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    56739 2022-12-21 13:10:07.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/data_image_plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27379 2022-12-21 13:10:07.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/grid_image_plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    77426 2022-12-21 13:10:07.000000 autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/source_plane_mesh.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      531 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/docs/api/light.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1343 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/docs/api/modeling.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1771 2022-12-21 15:51:37.000000 autogalaxy-2023.7.7.1/docs/api/pixelization.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3184 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/docs/api/plot.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2420 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.1/docs/api/source.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4631 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/docs/conf.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.738737 autogalaxy-2023.7.7.1/docs/general/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1593 2023-02-06 13:53:49.000000 autogalaxy-2023.7.7.1/docs/general/citations.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1035 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/docs/general/configs.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1315 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/general/credits.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      981 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/general/likelihood_function.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9728 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.1/docs/general/model_cookbook.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       92 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/general/papers.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2450 2023-05-12 11:43:15.000000 autogalaxy-2023.7.7.1/docs/general/workspace.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.750173 autogalaxy-2023.7.7.1/docs/howtogalaxy/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1827 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_1_introduction.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2244 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_2_modeling.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1038 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_3_search_chaining.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1396 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_4_pixelizations.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      960 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_optional.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3447 2023-05-12 10:01:56.000000 autogalaxy-2023.7.7.1/docs/howtogalaxy/howtogalaxy.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10537 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/index.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.761177 autogalaxy-2023.7.7.1/docs/installation/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4014 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/docs/installation/conda.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3519 2023-05-12 10:01:56.000000 autogalaxy-2023.7.7.1/docs/installation/numba.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2403 2023-05-12 10:10:15.000000 autogalaxy-2023.7.7.1/docs/installation/overview.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3442 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/docs/installation/pip.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4703 2023-05-12 10:10:15.000000 autogalaxy-2023.7.7.1/docs/installation/source.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4572 2023-01-14 16:37:15.000000 autogalaxy-2023.7.7.1/docs/installation/troubleshooting.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.775209 autogalaxy-2023.7.7.1/docs/overview/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.029699 autogalaxy-2023.7.7.1/docs/overview/images/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.804669 autogalaxy-2023.7.7.1/docs/overview/images/fitting/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37264 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/bad_chi_squared_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    63409 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/bad_normalized_residual_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    39647 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/bad_residual_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    51168 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/chi_squared_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35309 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37035 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/masked_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33220 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/model_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44440 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/noise_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    69331 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/normalized_residual_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30136 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/plane_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31550 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/psf.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    65595 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/fitting/residual_map.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.819713 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28953 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/galaxy.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21591 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/grid_2d.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29995 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/merging_galaxies.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29232 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/plane.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29344 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/sersic_light_profile.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35172 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/galaxies/subplot_galaxies.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.839804 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   107396 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/dirty_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   113651 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/dirty_signal_to_noise.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   390140 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/fit_dirty_images.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41276 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/image_pre_ft.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46706 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/model_visibilities.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45127 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/reconstruction.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29898 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/uv_wavelengths.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30950 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/interferometry/visibilities.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.847859 autogalaxy-2023.7.7.1/docs/overview/images/modeling/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1175623 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/modeling/cornerplot.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    39125 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/modeling/image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   231702 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/modeling/subplot_fit.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.860859 autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    73817 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/dirty_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    75926 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/g_decomposed_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   152814 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/g_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   141963 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/r_decomposed_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   140328 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/r_image.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.865883 autogalaxy-2023.7.7.1/docs/overview/images/pixelizations/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38896 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/pixelizations/image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40489 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/pixelizations/rectangular.png
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.882894 autogalaxy-2023.7.7.1/docs/overview/images/simulating/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   106644 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/ao.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37696 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/euclid.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    80336 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/hst.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35633 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43310 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/noise_map.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33339 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/psf.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    49620 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/docs/overview/images/simulating/vro.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8164 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/overview/overview_1_galaxies.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6608 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/overview/overview_2_fitting.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20432 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/overview/overview_3_modeling.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2948 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/overview/overview_4_simulate.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3483 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/overview/overview_5_pixelizations.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8857 2023-06-03 12:30:36.000000 autogalaxy-2023.7.7.1/docs/overview/overview_6_interferometry.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10664 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/docs/overview/overview_7_multi_wavelength.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/docs/requirements.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/eden.ini
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.897879 autogalaxy-2023.7.7.1/files/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21260 2023-02-21 10:35:21.000000 autogalaxy-2023.7.7.1/files/citations.bib
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1679 2023-02-06 13:53:49.000000 autogalaxy-2023.7.7.1/files/citations.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2267 2023-02-06 13:53:49.000000 autogalaxy-2023.7.7.1/files/citations.tex
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43549 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/files/dirty_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29819 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/files/model_dirty_image.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    67674 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/files/non_parametric.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   139037 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/files/observed.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43670 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/files/parametric.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   223339 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/files/visibilities.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      112 2023-06-03 19:29:54.000000 autogalaxy-2023.7.7.1/optional_requirements.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:47:58.911501 autogalaxy-2023.7.7.1/paper/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      190 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/paper/README.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   399405 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/paper/almacombined.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   342368 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/paper/hstcombined.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   122730 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/paper/observed.pdf
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45539 2023-02-21 10:35:21.000000 autogalaxy-2023.7.7.1/paper/paper.bib
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      830 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/paper/paper.json
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13514 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.1/paper/paper.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43670 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.1/paper/parametric.png
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      201 2022-12-19 13:59:53.000000 autogalaxy-2023.7.7.1/readthedocs.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       29 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.1/requirements.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-06-07 09:47:58.915660 autogalaxy-2023.7.7.1/setup.cfg
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2016 2023-06-07 09:47:40.000000 autogalaxy-2023.7.7.1/setup.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3012 2023-06-07 09:38:14.000000 autogalaxy-2023.7.7.1/zenodo.json
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.964586 autogalaxy-2023.7.7.2/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:00.932542 autogalaxy-2023.7.7.2/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.028728 autogalaxy-2023.7.7.2/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      475 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/.github/workflows/draft-pdf.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3327 2022-12-19 16:37:19.000000 autogalaxy-2023.7.7.2/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1135 2022-12-19 11:17:33.000000 autogalaxy-2023.7.7.2/CITATIONS.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18987 2022-12-20 20:59:49.000000 autogalaxy-2023.7.7.2/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2494 2022-12-20 20:59:49.000000 autogalaxy-2023.7.7.2/CONTRIBUTING.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1095 2020-11-16 19:58:12.000000 autogalaxy-2023.7.7.2/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      388 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8400 2023-06-07 09:59:01.963586 autogalaxy-2023.7.7.2/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7567 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.038300 autogalaxy-2023.7.7.2/autogalaxy/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5518 2023-06-07 09:57:30.000000 autogalaxy-2023.7.7.2/autogalaxy/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7805 2023-06-03 11:22:20.000000 autogalaxy-2023.7.7.2/autogalaxy/abstract_fit.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.051961 autogalaxy-2023.7.7.2/autogalaxy/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      308 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/autogalaxy/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7129 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.2/autogalaxy/aggregator/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4541 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/autogalaxy/aggregator/fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4523 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/autogalaxy/aggregator/fit_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2653 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/autogalaxy/aggregator/imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2844 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/autogalaxy/aggregator/interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2746 2023-05-11 09:42:09.000000 autogalaxy-2023.7.7.2/autogalaxy/aggregator/plane.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.069900 autogalaxy-2023.7.7.2/autogalaxy/analysis/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-08-21 09:36:45.000000 autogalaxy-2023.7.7.2/autogalaxy/analysis/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18823 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.2/autogalaxy/analysis/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10497 2023-06-05 13:31:36.000000 autogalaxy-2023.7.7.2/autogalaxy/analysis/chaining_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7567 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.2/autogalaxy/analysis/clump_model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5029 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/analysis/maker.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.073900 autogalaxy-2023.7.7.2/autogalaxy/analysis/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/autogalaxy/analysis/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3288 2023-06-05 20:15:34.000000 autogalaxy-2023.7.7.2/autogalaxy/analysis/mock/mock_result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9953 2023-06-06 14:36:29.000000 autogalaxy-2023.7.7.2/autogalaxy/analysis/model_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9842 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.2/autogalaxy/analysis/preloads.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6634 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.2/autogalaxy/analysis/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1157 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.2/autogalaxy/analysis/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19568 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.2/autogalaxy/analysis/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.082840 autogalaxy-2023.7.7.2/autogalaxy/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2020-11-11 16:43:14.000000 autogalaxy-2023.7.7.2/autogalaxy/config/.gitignore
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      630 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.2/autogalaxy/config/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      493 2023-06-06 18:37:09.000000 autogalaxy-2023.7.7.2/autogalaxy/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1677 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.2/autogalaxy/config/grids.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3369 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.2/autogalaxy/config/notation.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.091810 autogalaxy-2023.7.7.2/autogalaxy/config/priors/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1607 2022-12-16 19:52:14.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       10 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/basis.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      620 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/cosmology.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.095809 autogalaxy-2023.7.7.2/autogalaxy/config/priors/galaxy/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      253 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/galaxy/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      204 2022-12-21 16:13:37.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/galaxy/redshift.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.097810 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1012 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.121941 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2105 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/chameleon.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1739 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2097 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/eff.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1733 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2849 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/exponential_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1705 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2061 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/moffat.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2101 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/sersic.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3217 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/sersic_core.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.126731 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear_operated/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1271 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear_operated/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear_operated/moffat.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.134773 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/operated/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1271 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/operated/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1450 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/operated/moffat.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1469 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/operated/sersic.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.143966 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/shapelets/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1815 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/shapelets/cartesian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1819 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/shapelets/exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1807 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/shapelets/polar.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.168742 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2503 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/chameleon.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2137 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2495 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/eff.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2131 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3241 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/exponential_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2103 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2459 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/moffat.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2499 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/sersic.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3609 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/sersic_core.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.171743 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      639 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.191207 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2457 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/gnfw.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1682 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2077 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/nfw.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3593 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1274 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1022 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3402 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.198967 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/point/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      640 2023-05-15 17:46:30.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/point/point.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1029 2023-05-15 17:46:30.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/point/smbh.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1604 2023-05-17 15:24:31.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/point/smbh_binary.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.204968 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/sheets/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      389 2023-01-14 17:31:13.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/sheets/external_shear.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      632 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.224724 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2921 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/chameleon.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2545 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2539 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/exponential.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1481 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/gaussian.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2907 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/sersic.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4027 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/sersic_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3337 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.241465 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/total/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1729 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/total/isothermal.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2113 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/total/isothermal_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2089 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/total/power_law.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2867 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/total/power_law_broken.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2473 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/total/power_law_core.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1333 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/total/power_law_multipole.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.254136 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mesh/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      225 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mesh/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      989 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mesh/delaunay.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      385 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mesh/rectangular.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      987 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mesh/voronoi.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      991 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/mesh/voronoi_nn.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1536 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/point_sources.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.272135 autogalaxy-2023.7.7.2/autogalaxy/config/priors/regularization/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      246 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/regularization/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1251 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/regularization/adaptive_brightness.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1087 2023-03-24 12:25:33.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      211 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/regularization/constant.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      216 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/regularization/constant_split.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      434 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/regularization/constant_zeroth.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      209 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/priors/regularization/zeroth.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.286135 autogalaxy-2023.7.7.2/autogalaxy/config/visualize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      696 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/visualize/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      174 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/config/visualize/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2023-03-18 16:31:03.000000 autogalaxy-2023.7.7.2/autogalaxy/config/visualize/include.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      259 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/config/visualize/mat_wrap_1d.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      947 2023-03-18 16:31:03.000000 autogalaxy-2023.7.7.2/autogalaxy/config/visualize/mat_wrap_2d.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5385 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.2/autogalaxy/config/visualize/plots.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3774 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/convert.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.294135 autogalaxy-2023.7.7.2/autogalaxy/cosmology/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      150 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/autogalaxy/cosmology/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13974 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.2/autogalaxy/cosmology/lensing.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      933 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/cosmology/model.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1431 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/autogalaxy/cosmology/wrap.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3232 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/exc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7213 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.302135 autogalaxy-2023.7.7.2/autogalaxy/galaxy/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/autogalaxy/galaxy/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20983 2023-05-15 19:02:02.000000 autogalaxy-2023.7.7.2/autogalaxy/galaxy/galaxy.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.306135 autogalaxy-2023.7.7.2/autogalaxy/galaxy/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/autogalaxy/galaxy/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      758 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/autogalaxy/galaxy/mock/mock_galaxy.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.312136 autogalaxy-2023.7.7.2/autogalaxy/galaxy/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.2/autogalaxy/galaxy/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4437 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/galaxy/plot/adapt_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40501 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/galaxy/plot/galaxy_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1002 2022-12-20 17:00:47.000000 autogalaxy-2023.7.7.2/autogalaxy/galaxy/redshift.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1772 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/galaxy/stellar_dark_decomp.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.318136 autogalaxy-2023.7.7.2/autogalaxy/gui/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/autogalaxy/gui/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2041 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/gui/clicker.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6977 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/gui/scribbler.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.324135 autogalaxy-2023.7.7.2/autogalaxy/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.2/autogalaxy/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12738 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/autogalaxy/imaging/fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3868 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/autogalaxy/imaging/imaging.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.333136 autogalaxy-2023.7.7.2/autogalaxy/imaging/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.2/autogalaxy/imaging/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16878 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.2/autogalaxy/imaging/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3215 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/imaging/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4285 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/autogalaxy/imaging/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.337137 autogalaxy-2023.7.7.2/autogalaxy/imaging/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.2/autogalaxy/imaging/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9632 2023-06-03 16:50:56.000000 autogalaxy-2023.7.7.2/autogalaxy/imaging/plot/fit_imaging_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.344135 autogalaxy-2023.7.7.2/autogalaxy/interferometer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.2/autogalaxy/interferometer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10643 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/autogalaxy/interferometer/fit_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3368 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/interferometer/interferometer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.353137 autogalaxy-2023.7.7.2/autogalaxy/interferometer/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.2/autogalaxy/interferometer/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17326 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.2/autogalaxy/interferometer/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2960 2023-06-05 20:15:34.000000 autogalaxy-2023.7.7.2/autogalaxy/interferometer/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5378 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/autogalaxy/interferometer/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.357137 autogalaxy-2023.7.7.2/autogalaxy/interferometer/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.2/autogalaxy/interferometer/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8265 2023-06-03 16:50:56.000000 autogalaxy-2023.7.7.2/autogalaxy/interferometer/plot/fit_interferometer_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      341 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/mock.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.363137 autogalaxy-2023.7.7.2/autogalaxy/operate/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.2/autogalaxy/operate/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36267 2023-06-03 17:45:40.000000 autogalaxy-2023.7.7.2/autogalaxy/operate/deflections.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20198 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/operate/image.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.372166 autogalaxy-2023.7.7.2/autogalaxy/plane/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      686 2020-11-16 19:58:12.000000 autogalaxy-2023.7.7.2/autogalaxy/plane/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16202 2023-05-15 18:37:24.000000 autogalaxy-2023.7.7.2/autogalaxy/plane/plane.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8439 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/plane/plane_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.376135 autogalaxy-2023.7.7.2/autogalaxy/plane/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.2/autogalaxy/plane/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14120 2023-05-23 09:38:20.000000 autogalaxy-2023.7.7.2/autogalaxy/plane/plot/plane_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10432 2023-06-06 10:32:57.000000 autogalaxy-2023.7.7.2/autogalaxy/plane/to_inversion.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.384135 autogalaxy-2023.7.7.2/autogalaxy/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3398 2023-06-03 09:03:18.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      553 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/abstract_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.391136 autogalaxy-2023.7.7.2/autogalaxy/plot/get_visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/get_visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9924 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/get_visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13590 2023-06-03 17:45:40.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/get_visuals/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.397136 autogalaxy-2023.7.7.2/autogalaxy/plot/include/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/include/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1470 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/include/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2658 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/include/two_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4560 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/mass_plotter.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.404134 autogalaxy-2023.7.7.2/autogalaxy/plot/mat_plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/mat_plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6113 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/mat_plot/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10005 2023-03-18 16:31:03.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/mat_plot/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.410135 autogalaxy-2023.7.7.2/autogalaxy/plot/visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2123 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4140 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/visuals/two_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      646 2023-03-18 16:31:03.000000 autogalaxy-2023.7.7.2/autogalaxy/plot/wrap.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.421134 autogalaxy-2023.7.7.2/autogalaxy/profiles/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-11 16:43:14.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13967 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/geometry_profiles.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.430136 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5442 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1883 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/basis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2511 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/decorators.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.458136 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      401 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6951 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/chameleon.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1859 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/dev_vaucouleurs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/eff.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1835 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1734 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/exponential_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1755 2023-03-16 18:34:52.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1749 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/moffat.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2223 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/sersic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2730 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/sersic_core.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.469136 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear_operated/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       99 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear_operated/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      207 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear_operated/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      203 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear_operated/moffat.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      203 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear_operated/sersic.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.474136 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1032 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/mock/mock_light_profile.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.486135 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/operated/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      143 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/operated/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       39 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/operated/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      200 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/operated/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      196 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/operated/moffat.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      196 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/operated/sersic.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.501165 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/shapelets/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      247 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/shapelets/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1202 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/shapelets/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4264 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/shapelets/cartesian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4501 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/shapelets/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4330 2023-03-03 11:53:26.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/shapelets/polar.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.530134 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      371 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4007 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3255 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/chameleon.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2581 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/dev_vaucouleurs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2782 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/eff.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2504 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2227 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2736 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/sersic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2338 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/sersic_core.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.560134 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      490 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5851 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/chameleon.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2351 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/dev_vaucouleurs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4414 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/eff.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2316 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3188 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/exponential_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4052 2023-04-27 18:43:48.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4905 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/moffat.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7640 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/sersic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5734 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/sersic_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25207 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/light_and_mass_profiles.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.562250 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1020 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.573247 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/abstract/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/abstract/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10340 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/abstract/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7050 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/abstract/cse.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8675 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/abstract/mge.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.602866 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      440 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12379 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13480 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/gnfw.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1130 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/gnfw_mcr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3352 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/mcr_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11547 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/nfw.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2532 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/nfw_mcr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2090 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4410 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/nfw_truncated.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2089 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1161 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.607865 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      714 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/mock/mock_mass_profile.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.617865 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/point/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       91 2023-05-17 15:24:31.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/point/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1902 2023-05-15 17:46:30.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/point/point.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1653 2023-05-15 17:46:30.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/point/smbh.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4963 2023-05-31 16:46:27.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/point/smbh_binary.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.628865 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/sheets/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      127 2022-12-16 18:30:52.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/sheets/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2611 2023-06-06 12:57:36.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/sheets/external_shear.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4977 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/sheets/input_deflections.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1416 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/sheets/mass_sheet.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.651668 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      372 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8482 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/chameleon.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2478 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2472 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/exponential.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7629 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/gaussian.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16715 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/sersic.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7038 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/sersic_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9613 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.669705 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      337 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6348 2023-06-06 12:20:19.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/isothermal.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2109 2022-12-16 19:36:21.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/isothermal_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5545 2023-06-06 12:57:36.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/power_law.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6460 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/power_law_broken.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8476 2023-06-06 12:51:47.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/power_law_core.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8585 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/power_law_multipole.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.676705 autogalaxy-2023.7.7.2/autogalaxy/profiles/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12961 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/plot/light_profile_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14915 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/plot/mass_profile_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      467 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/point_sources.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1450 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/profiles/scaling_relations.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.683254 autogalaxy-2023.7.7.2/autogalaxy/quantity/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.2/autogalaxy/quantity/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9901 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/quantity/dataset_quantity.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4646 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/quantity/fit_quantity.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.691865 autogalaxy-2023.7.7.2/autogalaxy/quantity/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.2/autogalaxy/quantity/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10139 2023-05-10 17:34:39.000000 autogalaxy-2023.7.7.2/autogalaxy/quantity/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1747 2023-02-20 18:27:21.000000 autogalaxy-2023.7.7.2/autogalaxy/quantity/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3510 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/autogalaxy/quantity/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.696959 autogalaxy-2023.7.7.2/autogalaxy/quantity/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autogalaxy-2023.7.7.2/autogalaxy/quantity/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8126 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/quantity/plot/fit_quantity_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.702573 autogalaxy-2023.7.7.2/autogalaxy/util/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1391 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.2/autogalaxy/util/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2572 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/util/error_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.706572 autogalaxy-2023.7.7.2/autogalaxy/util/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/autogalaxy/util/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1353 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/autogalaxy/util/mock/mock_cosmology.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3858 2023-01-13 16:57:54.000000 autogalaxy-2023.7.7.2/autogalaxy/util/shear_field.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.962587 autogalaxy-2023.7.7.2/autogalaxy.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16633 2023-06-07 09:59:00.000000 autogalaxy-2023.7.7.2/autogalaxy.egg-info/SOURCES.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.712109 autogalaxy-2023.7.7.2/docs/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.716086 autogalaxy-2023.7.7.2/docs/_templates/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2022-12-21 16:35:52.000000 autogalaxy-2023.7.7.2/docs/_templates/custom-class-template.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/docs/_templates/custom_module_template.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.721843 autogalaxy-2023.7.7.2/docs/advanced/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      388 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/advanced/chaining.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6363 2022-12-20 22:05:13.000000 autogalaxy-2023.7.7.2/docs/advanced/database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1374 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/docs/advanced/graphical.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.736499 autogalaxy-2023.7.7.2/docs/api/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1592 2023-01-13 16:57:54.000000 autogalaxy-2023.7.7.2/docs/api/data.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      330 2022-12-20 17:33:12.000000 autogalaxy-2023.7.7.2/docs/api/fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      664 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.2/docs/api/galaxy.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.001892 autogalaxy-2023.7.7.2/docs/api/images/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.744499 autogalaxy-2023.7.7.2/docs/api/images/pixelization_image_plane/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41383 2022-12-21 12:27:28.000000 autogalaxy-2023.7.7.2/docs/api/images/pixelization_image_plane/data_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34340 2022-12-21 12:27:28.000000 autogalaxy-2023.7.7.2/docs/api/images/pixelization_image_plane/grid_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    49269 2022-12-21 12:27:49.000000 autogalaxy-2023.7.7.2/docs/api/images/pixelization_image_plane/image_plane_mesh.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.752533 autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_image_plane/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40349 2022-12-21 12:22:21.000000 autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_image_plane/data_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26453 2022-12-21 12:22:21.000000 autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_image_plane/grid_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48007 2022-12-21 12:28:33.000000 autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_image_plane/image_plane_mesh.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.760548 autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_source_plane/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    56739 2022-12-21 13:10:07.000000 autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_source_plane/data_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27379 2022-12-21 13:10:07.000000 autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_source_plane/grid_image_plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    77426 2022-12-21 13:10:07.000000 autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_source_plane/source_plane_mesh.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      531 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/docs/api/light.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1343 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.2/docs/api/modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1771 2022-12-21 15:51:37.000000 autogalaxy-2023.7.7.2/docs/api/pixelization.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3184 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/docs/api/plot.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2420 2023-05-31 17:24:34.000000 autogalaxy-2023.7.7.2/docs/api/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4631 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/docs/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.774549 autogalaxy-2023.7.7.2/docs/general/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1593 2023-02-06 13:53:49.000000 autogalaxy-2023.7.7.2/docs/general/citations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1035 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/docs/general/configs.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1315 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/general/credits.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      981 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/general/likelihood_function.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9728 2023-05-10 13:41:17.000000 autogalaxy-2023.7.7.2/docs/general/model_cookbook.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       92 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/general/papers.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2450 2023-05-12 11:43:15.000000 autogalaxy-2023.7.7.2/docs/general/workspace.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.787053 autogalaxy-2023.7.7.2/docs/howtogalaxy/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1827 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/howtogalaxy/chapter_1_introduction.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2244 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/howtogalaxy/chapter_2_modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1038 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/howtogalaxy/chapter_3_search_chaining.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1396 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/howtogalaxy/chapter_4_pixelizations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      960 2023-06-06 10:32:01.000000 autogalaxy-2023.7.7.2/docs/howtogalaxy/chapter_optional.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3447 2023-05-12 10:01:56.000000 autogalaxy-2023.7.7.2/docs/howtogalaxy/howtogalaxy.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10537 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/docs/index.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.799033 autogalaxy-2023.7.7.2/docs/installation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4014 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/docs/installation/conda.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3519 2023-05-12 10:01:56.000000 autogalaxy-2023.7.7.2/docs/installation/numba.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2403 2023-05-12 10:10:15.000000 autogalaxy-2023.7.7.2/docs/installation/overview.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3442 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/docs/installation/pip.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4703 2023-05-12 10:10:15.000000 autogalaxy-2023.7.7.2/docs/installation/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4572 2023-01-14 16:37:15.000000 autogalaxy-2023.7.7.2/docs/installation/troubleshooting.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.812674 autogalaxy-2023.7.7.2/docs/overview/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.008822 autogalaxy-2023.7.7.2/docs/overview/images/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.844988 autogalaxy-2023.7.7.2/docs/overview/images/fitting/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37264 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/fitting/bad_chi_squared_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    63409 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/fitting/bad_normalized_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    39647 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/fitting/bad_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    51168 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/fitting/chi_squared_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35309 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/fitting/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37035 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/fitting/masked_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33220 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/fitting/model_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44440 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/fitting/noise_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    69331 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/fitting/normalized_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30136 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/fitting/plane_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31550 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/fitting/psf.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    65595 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/fitting/residual_map.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.859988 autogalaxy-2023.7.7.2/docs/overview/images/galaxies/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28953 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/galaxies/galaxy.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21591 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/galaxies/grid_2d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29995 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/galaxies/merging_galaxies.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29232 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/galaxies/plane.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29344 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/galaxies/sersic_light_profile.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35172 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/galaxies/subplot_galaxies.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.882554 autogalaxy-2023.7.7.2/docs/overview/images/interferometry/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   107396 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/interferometry/dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   113651 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/interferometry/dirty_signal_to_noise.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   390140 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/interferometry/fit_dirty_images.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41276 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/interferometry/image_pre_ft.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46706 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/interferometry/model_visibilities.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45127 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/interferometry/reconstruction.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29898 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/interferometry/uv_wavelengths.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30950 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/interferometry/visibilities.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.891552 autogalaxy-2023.7.7.2/docs/overview/images/modeling/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1175623 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/modeling/cornerplot.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    39125 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/modeling/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   231702 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/modeling/subplot_fit.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.905889 autogalaxy-2023.7.7.2/docs/overview/images/multiwavelength/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    73817 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/multiwavelength/dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    75926 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/multiwavelength/g_decomposed_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   152814 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/multiwavelength/g_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   141963 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/multiwavelength/r_decomposed_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   140328 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/multiwavelength/r_image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.910890 autogalaxy-2023.7.7.2/docs/overview/images/pixelizations/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38896 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/pixelizations/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40489 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/pixelizations/rectangular.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.928815 autogalaxy-2023.7.7.2/docs/overview/images/simulating/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   106644 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/simulating/ao.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37696 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/simulating/euclid.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    80336 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/simulating/hst.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35633 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/simulating/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43310 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/simulating/noise_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33339 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/simulating/psf.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    49620 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/docs/overview/images/simulating/vro.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8164 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/docs/overview/overview_1_galaxies.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6608 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/docs/overview/overview_2_fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20432 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/docs/overview/overview_3_modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2948 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/docs/overview/overview_4_simulate.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3483 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/docs/overview/overview_5_pixelizations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8857 2023-06-03 12:30:36.000000 autogalaxy-2023.7.7.2/docs/overview/overview_6_interferometry.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10664 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/docs/overview/overview_7_multi_wavelength.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/docs/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/eden.ini
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.945067 autogalaxy-2023.7.7.2/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21260 2023-02-21 10:35:21.000000 autogalaxy-2023.7.7.2/files/citations.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1679 2023-02-06 13:53:49.000000 autogalaxy-2023.7.7.2/files/citations.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2267 2023-02-06 13:53:49.000000 autogalaxy-2023.7.7.2/files/citations.tex
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43549 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/files/dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29819 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/files/model_dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    67674 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/files/non_parametric.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   139037 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/files/observed.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43670 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/files/parametric.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   223339 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/files/visibilities.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      112 2023-06-03 19:29:54.000000 autogalaxy-2023.7.7.2/optional_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:01.960586 autogalaxy-2023.7.7.2/paper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      190 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/paper/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   399405 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/paper/almacombined.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   342368 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/paper/hstcombined.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   122730 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/paper/observed.pdf
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45539 2023-02-21 10:35:21.000000 autogalaxy-2023.7.7.2/paper/paper.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      830 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/paper/paper.json
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13514 2023-06-03 11:20:35.000000 autogalaxy-2023.7.7.2/paper/paper.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43670 2022-11-24 19:55:46.000000 autogalaxy-2023.7.7.2/paper/parametric.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      201 2022-12-19 13:59:53.000000 autogalaxy-2023.7.7.2/readthedocs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       29 2022-12-16 17:06:50.000000 autogalaxy-2023.7.7.2/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-06-07 09:59:01.964586 autogalaxy-2023.7.7.2/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2016 2023-06-07 09:57:48.000000 autogalaxy-2023.7.7.2/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3012 2023-06-07 09:57:30.000000 autogalaxy-2023.7.7.2/zenodo.json
```

### Comparing `autogalaxy-2023.7.7.1/.github/workflows/main.yml` & `autogalaxy-2023.7.7.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/CITATIONS.rst` & `autogalaxy-2023.7.7.2/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/CODE_OF_CONDUCT.md` & `autogalaxy-2023.7.7.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/CONTRIBUTING.md` & `autogalaxy-2023.7.7.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/LICENSE` & `autogalaxy-2023.7.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/PKG-INFO` & `autogalaxy-2023.7.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogalaxy
-Version: 2023.7.7.1
+Version: 2023.7.7.2
 Summary: Open-Source Multi Wavelength Galaxy Structure & Morphology
 Home-page: https://github.com/Jammy2211/PyAutoGalaxy
 Author: James Nightingale and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
```

### Comparing `autogalaxy-2023.7.7.1/README.rst` & `autogalaxy-2023.7.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/__init__.py` & `autogalaxy-2023.7.7.2/autogalaxy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,8 +105,8 @@
 
 from .analysis.clump_model import ClumpModel
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2023.7.7.1"
+__version__ = "2023.7.7.2"
```

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/abstract_fit.py` & `autogalaxy-2023.7.7.2/autogalaxy/abstract_fit.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/aggregator/abstract.py` & `autogalaxy-2023.7.7.2/autogalaxy/aggregator/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/aggregator/fit_imaging.py` & `autogalaxy-2023.7.7.2/autogalaxy/aggregator/fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/aggregator/fit_interferometer.py` & `autogalaxy-2023.7.7.2/autogalaxy/aggregator/fit_interferometer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/aggregator/imaging.py` & `autogalaxy-2023.7.7.2/autogalaxy/aggregator/imaging.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/aggregator/interferometer.py` & `autogalaxy-2023.7.7.2/autogalaxy/aggregator/interferometer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/aggregator/plane.py` & `autogalaxy-2023.7.7.2/autogalaxy/aggregator/plane.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/analysis/analysis.py` & `autogalaxy-2023.7.7.2/autogalaxy/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/analysis/chaining_util.py` & `autogalaxy-2023.7.7.2/autogalaxy/analysis/chaining_util.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/analysis/clump_model.py` & `autogalaxy-2023.7.7.2/autogalaxy/analysis/clump_model.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/analysis/maker.py` & `autogalaxy-2023.7.7.2/autogalaxy/analysis/maker.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/analysis/mock/mock_result.py` & `autogalaxy-2023.7.7.2/autogalaxy/analysis/mock/mock_result.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/analysis/model_util.py` & `autogalaxy-2023.7.7.2/autogalaxy/analysis/model_util.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/analysis/preloads.py` & `autogalaxy-2023.7.7.2/autogalaxy/analysis/preloads.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/analysis/result.py` & `autogalaxy-2023.7.7.2/autogalaxy/analysis/result.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/analysis/setup.py` & `autogalaxy-2023.7.7.2/autogalaxy/analysis/setup.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/analysis/visualizer.py` & `autogalaxy-2023.7.7.2/autogalaxy/analysis/visualizer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/README.rst` & `autogalaxy-2023.7.7.2/autogalaxy/config/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/grids.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/grids.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/notation.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/notation.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/README.rst` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/cosmology.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/cosmology.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/README.rst` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/chameleon.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/chameleon.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/dev_vaucouleurs.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/eff.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/eff.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/exponential.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/exponential_core.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/exponential_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/gaussian.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/moffat.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/sersic.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear/sersic_core.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear/sersic_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear_operated/gaussian.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear_operated/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/linear_operated/moffat.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/linear_operated/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/gaussian.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/operated/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/moffat.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/operated/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/operated/sersic.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/operated/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/cartesian.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/shapelets/cartesian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/exponential.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/shapelets/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/shapelets/polar.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/shapelets/polar.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/chameleon.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/chameleon.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/dev_vaucouleurs.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/eff.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/eff.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/exponential.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/exponential_core.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/exponential_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/gaussian.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/moffat.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/moffat.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/sersic.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/light/standard/sersic_core.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/light/standard/sersic_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/README.rst` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/gnfw.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/gnfw.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/gnfw_mcr.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/nfw.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/nfw_mcr.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/nfw_mcr_scatter.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/nfw_truncated.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/dark/nfw_truncated_mcr.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/point/point.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/point/point.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/point/smbh.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/point/smbh.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/point/smbh_binary.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/point/smbh_binary.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/sheets/mass_sheet.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/chameleon.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/chameleon.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/dev_vaucouleurs.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/exponential.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/exponential.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/gaussian.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/gaussian.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/sersic.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/sersic.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/sersic_core.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/sersic_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/stellar/sersic_radial_gradient.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/isothermal.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/total/isothermal.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/isothermal_core.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/total/isothermal_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/total/power_law.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law_broken.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/total/power_law_broken.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law_core.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/total/power_law_core.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mass/total/power_law_multipole.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mass/total/power_law_multipole.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/delaunay.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mesh/delaunay.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/voronoi.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mesh/voronoi.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/mesh/voronoi_nn.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/mesh/voronoi_nn.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/point_sources.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/point_sources.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/adaptive_brightness.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/regularization/adaptive_brightness.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/priors/regularization/adaptive_brightness_split_zeroth.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/visualize/README.rst` & `autogalaxy-2023.7.7.2/autogalaxy/config/visualize/README.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/visualize/mat_wrap_2d.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/visualize/mat_wrap_2d.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/config/visualize/plots.yaml` & `autogalaxy-2023.7.7.2/autogalaxy/config/visualize/plots.yaml`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/convert.py` & `autogalaxy-2023.7.7.2/autogalaxy/convert.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/cosmology/lensing.py` & `autogalaxy-2023.7.7.2/autogalaxy/cosmology/lensing.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/cosmology/model.py` & `autogalaxy-2023.7.7.2/autogalaxy/cosmology/model.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/cosmology/wrap.py` & `autogalaxy-2023.7.7.2/autogalaxy/cosmology/wrap.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/exc.py` & `autogalaxy-2023.7.7.2/autogalaxy/exc.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/fixtures.py` & `autogalaxy-2023.7.7.2/autogalaxy/fixtures.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/galaxy/galaxy.py` & `autogalaxy-2023.7.7.2/autogalaxy/galaxy/galaxy.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/galaxy/mock/mock_galaxy.py` & `autogalaxy-2023.7.7.2/autogalaxy/galaxy/mock/mock_galaxy.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/galaxy/plot/adapt_plotters.py` & `autogalaxy-2023.7.7.2/autogalaxy/galaxy/plot/adapt_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/galaxy/plot/galaxy_plotters.py` & `autogalaxy-2023.7.7.2/autogalaxy/galaxy/plot/galaxy_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/galaxy/redshift.py` & `autogalaxy-2023.7.7.2/autogalaxy/galaxy/redshift.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/galaxy/stellar_dark_decomp.py` & `autogalaxy-2023.7.7.2/autogalaxy/galaxy/stellar_dark_decomp.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/gui/clicker.py` & `autogalaxy-2023.7.7.2/autogalaxy/gui/clicker.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/gui/scribbler.py` & `autogalaxy-2023.7.7.2/autogalaxy/gui/scribbler.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/imaging/fit_imaging.py` & `autogalaxy-2023.7.7.2/autogalaxy/imaging/fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/imaging/imaging.py` & `autogalaxy-2023.7.7.2/autogalaxy/imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/imaging/model/analysis.py` & `autogalaxy-2023.7.7.2/autogalaxy/imaging/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/imaging/model/result.py` & `autogalaxy-2023.7.7.2/autogalaxy/imaging/model/result.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/imaging/model/visualizer.py` & `autogalaxy-2023.7.7.2/autogalaxy/imaging/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/imaging/plot/fit_imaging_plotters.py` & `autogalaxy-2023.7.7.2/autogalaxy/imaging/plot/fit_imaging_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/interferometer/fit_interferometer.py` & `autogalaxy-2023.7.7.2/autogalaxy/interferometer/fit_interferometer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/interferometer/interferometer.py` & `autogalaxy-2023.7.7.2/autogalaxy/interferometer/interferometer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/analysis.py` & `autogalaxy-2023.7.7.2/autogalaxy/interferometer/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/result.py` & `autogalaxy-2023.7.7.2/autogalaxy/interferometer/model/result.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/interferometer/model/visualizer.py` & `autogalaxy-2023.7.7.2/autogalaxy/interferometer/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/interferometer/plot/fit_interferometer_plotters.py` & `autogalaxy-2023.7.7.2/autogalaxy/interferometer/plot/fit_interferometer_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/operate/deflections.py` & `autogalaxy-2023.7.7.2/autogalaxy/operate/deflections.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/operate/image.py` & `autogalaxy-2023.7.7.2/autogalaxy/operate/image.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plane/__init__.py` & `autogalaxy-2023.7.7.2/autogalaxy/plane/__init__.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plane/plane.py` & `autogalaxy-2023.7.7.2/autogalaxy/plane/plane.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plane/plane_util.py` & `autogalaxy-2023.7.7.2/autogalaxy/plane/plane_util.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plane/plot/plane_plotters.py` & `autogalaxy-2023.7.7.2/autogalaxy/plane/plot/plane_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plane/to_inversion.py` & `autogalaxy-2023.7.7.2/autogalaxy/plane/to_inversion.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plot/__init__.py` & `autogalaxy-2023.7.7.2/autogalaxy/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plot/abstract_plotters.py` & `autogalaxy-2023.7.7.2/autogalaxy/plot/abstract_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plot/get_visuals/one_d.py` & `autogalaxy-2023.7.7.2/autogalaxy/plot/get_visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plot/get_visuals/two_d.py` & `autogalaxy-2023.7.7.2/autogalaxy/plot/get_visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plot/include/one_d.py` & `autogalaxy-2023.7.7.2/autogalaxy/plot/include/one_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plot/include/two_d.py` & `autogalaxy-2023.7.7.2/autogalaxy/plot/include/two_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plot/mass_plotter.py` & `autogalaxy-2023.7.7.2/autogalaxy/plot/mass_plotter.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plot/mat_plot/one_d.py` & `autogalaxy-2023.7.7.2/autogalaxy/plot/mat_plot/one_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plot/mat_plot/two_d.py` & `autogalaxy-2023.7.7.2/autogalaxy/plot/mat_plot/two_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plot/visuals/one_d.py` & `autogalaxy-2023.7.7.2/autogalaxy/plot/visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plot/visuals/two_d.py` & `autogalaxy-2023.7.7.2/autogalaxy/plot/visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/plot/wrap.py` & `autogalaxy-2023.7.7.2/autogalaxy/plot/wrap.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/geometry_profiles.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/geometry_profiles.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/abstract.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/basis.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/basis.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/decorators.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/decorators.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/abstract.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/dev_vaucouleurs.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/exponential.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/exponential_core.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/exponential_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/gaussian.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/gaussian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/moffat.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/moffat.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/sersic.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/sersic.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/linear/sersic_core.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/linear/sersic_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/mock/mock_light_profile.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/mock/mock_light_profile.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/abstract.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/shapelets/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/cartesian.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/shapelets/cartesian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/exponential.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/shapelets/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/shapelets/polar.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/shapelets/polar.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/abstract.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/chameleon.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/chameleon.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/dev_vaucouleurs.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/eff.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/eff.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/exponential.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/gaussian.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/gaussian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/sersic.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/sersic.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/snr/sersic_core.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/snr/sersic_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/chameleon.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/chameleon.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/dev_vaucouleurs.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/eff.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/eff.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/exponential.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/exponential_core.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/exponential_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/gaussian.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/gaussian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/moffat.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/moffat.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/sersic.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/sersic.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light/standard/sersic_core.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light/standard/sersic_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/light_and_mass_profiles.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/light_and_mass_profiles.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/__init__.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/__init__.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/abstract.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/abstract/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/cse.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/abstract/cse.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/abstract/mge.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/abstract/mge.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/abstract.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/abstract.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/gnfw.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/gnfw.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/gnfw_mcr.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/gnfw_mcr.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/mcr_util.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/mcr_util.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/nfw.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_mcr.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/nfw_mcr.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/nfw_mcr_scatter.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_truncated.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/nfw_truncated.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/nfw_truncated_mcr.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/dark/nfw_truncated_mcr_scatter.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/mock/mock_mass_profile.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/mock/mock_mass_profile.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/point.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/point/point.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/smbh.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/point/smbh.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/point/smbh_binary.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/point/smbh_binary.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/external_shear.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/sheets/external_shear.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/input_deflections.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/sheets/input_deflections.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/sheets/mass_sheet.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/sheets/mass_sheet.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/chameleon.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/chameleon.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/dev_vaucouleurs.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/exponential.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/exponential.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/gaussian.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/gaussian.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/sersic.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/sersic.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/sersic_core.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/sersic_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/stellar/sersic_radial_gradient.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/isothermal.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/isothermal.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/isothermal_core.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/isothermal_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/power_law.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law_broken.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/power_law_broken.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law_core.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/power_law_core.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/mass/total/power_law_multipole.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/mass/total/power_law_multipole.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/plot/light_profile_plotters.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/plot/light_profile_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/plot/mass_profile_plotters.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/plot/mass_profile_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/profiles/scaling_relations.py` & `autogalaxy-2023.7.7.2/autogalaxy/profiles/scaling_relations.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/quantity/dataset_quantity.py` & `autogalaxy-2023.7.7.2/autogalaxy/quantity/dataset_quantity.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/quantity/fit_quantity.py` & `autogalaxy-2023.7.7.2/autogalaxy/quantity/fit_quantity.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/quantity/model/analysis.py` & `autogalaxy-2023.7.7.2/autogalaxy/quantity/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/quantity/model/result.py` & `autogalaxy-2023.7.7.2/autogalaxy/quantity/model/result.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/quantity/model/visualizer.py` & `autogalaxy-2023.7.7.2/autogalaxy/quantity/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/quantity/plot/fit_quantity_plotters.py` & `autogalaxy-2023.7.7.2/autogalaxy/quantity/plot/fit_quantity_plotters.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/util/__init__.py` & `autogalaxy-2023.7.7.2/autogalaxy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/util/error_util.py` & `autogalaxy-2023.7.7.2/autogalaxy/util/error_util.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/util/mock/mock_cosmology.py` & `autogalaxy-2023.7.7.2/autogalaxy/util/mock/mock_cosmology.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy/util/shear_field.py` & `autogalaxy-2023.7.7.2/autogalaxy/util/shear_field.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/autogalaxy.egg-info/SOURCES.txt` & `autogalaxy-2023.7.7.2/autogalaxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/_templates/custom-class-template.rst` & `autogalaxy-2023.7.7.2/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/_templates/custom_module_template.rst` & `autogalaxy-2023.7.7.2/docs/_templates/custom_module_template.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/advanced/database.rst` & `autogalaxy-2023.7.7.2/docs/advanced/database.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/advanced/graphical.rst` & `autogalaxy-2023.7.7.2/docs/advanced/graphical.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/data.rst` & `autogalaxy-2023.7.7.2/docs/api/data.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/galaxy.rst` & `autogalaxy-2023.7.7.2/docs/api/galaxy.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/data_image_plane.png` & `autogalaxy-2023.7.7.2/docs/api/images/pixelization_image_plane/data_image_plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/grid_image_plane.png` & `autogalaxy-2023.7.7.2/docs/api/images/pixelization_image_plane/grid_image_plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/images/pixelization_image_plane/image_plane_mesh.png` & `autogalaxy-2023.7.7.2/docs/api/images/pixelization_image_plane/image_plane_mesh.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/data_image_plane.png` & `autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_image_plane/data_image_plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/grid_image_plane.png` & `autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_image_plane/grid_image_plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_image_plane/image_plane_mesh.png` & `autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_image_plane/image_plane_mesh.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/data_image_plane.png` & `autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_source_plane/data_image_plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/grid_image_plane.png` & `autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_source_plane/grid_image_plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/images/pixelization_masked_source_plane/source_plane_mesh.png` & `autogalaxy-2023.7.7.2/docs/api/images/pixelization_masked_source_plane/source_plane_mesh.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/light.rst` & `autogalaxy-2023.7.7.2/docs/api/light.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/modeling.rst` & `autogalaxy-2023.7.7.2/docs/api/modeling.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/pixelization.rst` & `autogalaxy-2023.7.7.2/docs/api/pixelization.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/plot.rst` & `autogalaxy-2023.7.7.2/docs/api/plot.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/api/source.rst` & `autogalaxy-2023.7.7.2/docs/api/source.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/conf.py` & `autogalaxy-2023.7.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/general/citations.rst` & `autogalaxy-2023.7.7.2/docs/general/citations.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/general/configs.rst` & `autogalaxy-2023.7.7.2/docs/general/configs.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/general/credits.rst` & `autogalaxy-2023.7.7.2/docs/general/credits.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/general/likelihood_function.rst` & `autogalaxy-2023.7.7.2/docs/general/likelihood_function.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/general/model_cookbook.rst` & `autogalaxy-2023.7.7.2/docs/general/model_cookbook.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/general/workspace.rst` & `autogalaxy-2023.7.7.2/docs/general/workspace.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_1_introduction.rst` & `autogalaxy-2023.7.7.2/docs/howtogalaxy/chapter_1_introduction.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_2_modeling.rst` & `autogalaxy-2023.7.7.2/docs/howtogalaxy/chapter_2_modeling.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_3_search_chaining.rst` & `autogalaxy-2023.7.7.2/docs/howtogalaxy/chapter_3_search_chaining.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_4_pixelizations.rst` & `autogalaxy-2023.7.7.2/docs/howtogalaxy/chapter_4_pixelizations.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/howtogalaxy/chapter_optional.rst` & `autogalaxy-2023.7.7.2/docs/howtogalaxy/chapter_optional.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/howtogalaxy/howtogalaxy.rst` & `autogalaxy-2023.7.7.2/docs/howtogalaxy/howtogalaxy.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/index.rst` & `autogalaxy-2023.7.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/installation/conda.rst` & `autogalaxy-2023.7.7.2/docs/installation/conda.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/installation/numba.rst` & `autogalaxy-2023.7.7.2/docs/installation/numba.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/installation/overview.rst` & `autogalaxy-2023.7.7.2/docs/installation/overview.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/installation/pip.rst` & `autogalaxy-2023.7.7.2/docs/installation/pip.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/installation/source.rst` & `autogalaxy-2023.7.7.2/docs/installation/source.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/installation/troubleshooting.rst` & `autogalaxy-2023.7.7.2/docs/installation/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/fitting/bad_chi_squared_map.png` & `autogalaxy-2023.7.7.2/docs/overview/images/fitting/bad_chi_squared_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/fitting/bad_normalized_residual_map.png` & `autogalaxy-2023.7.7.2/docs/overview/images/fitting/bad_normalized_residual_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/fitting/bad_residual_map.png` & `autogalaxy-2023.7.7.2/docs/overview/images/fitting/bad_residual_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/fitting/chi_squared_map.png` & `autogalaxy-2023.7.7.2/docs/overview/images/fitting/chi_squared_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/fitting/image.png` & `autogalaxy-2023.7.7.2/docs/overview/images/fitting/image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/fitting/masked_image.png` & `autogalaxy-2023.7.7.2/docs/overview/images/fitting/masked_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/fitting/model_image.png` & `autogalaxy-2023.7.7.2/docs/overview/images/fitting/model_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/fitting/noise_map.png` & `autogalaxy-2023.7.7.2/docs/overview/images/fitting/noise_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/fitting/normalized_residual_map.png` & `autogalaxy-2023.7.7.2/docs/overview/images/fitting/normalized_residual_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/fitting/plane_image.png` & `autogalaxy-2023.7.7.2/docs/overview/images/fitting/plane_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/fitting/psf.png` & `autogalaxy-2023.7.7.2/docs/overview/images/fitting/psf.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/fitting/residual_map.png` & `autogalaxy-2023.7.7.2/docs/overview/images/fitting/residual_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/galaxies/galaxy.png` & `autogalaxy-2023.7.7.2/docs/overview/images/galaxies/galaxy.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/galaxies/grid_2d.png` & `autogalaxy-2023.7.7.2/docs/overview/images/galaxies/grid_2d.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/galaxies/merging_galaxies.png` & `autogalaxy-2023.7.7.2/docs/overview/images/galaxies/merging_galaxies.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/galaxies/plane.png` & `autogalaxy-2023.7.7.2/docs/overview/images/galaxies/plane.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/galaxies/sersic_light_profile.png` & `autogalaxy-2023.7.7.2/docs/overview/images/galaxies/sersic_light_profile.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/galaxies/subplot_galaxies.png` & `autogalaxy-2023.7.7.2/docs/overview/images/galaxies/subplot_galaxies.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/dirty_image.png` & `autogalaxy-2023.7.7.2/docs/overview/images/interferometry/dirty_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/dirty_signal_to_noise.png` & `autogalaxy-2023.7.7.2/docs/overview/images/interferometry/dirty_signal_to_noise.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/fit_dirty_images.png` & `autogalaxy-2023.7.7.2/docs/overview/images/interferometry/fit_dirty_images.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/image_pre_ft.png` & `autogalaxy-2023.7.7.2/docs/overview/images/interferometry/image_pre_ft.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/model_visibilities.png` & `autogalaxy-2023.7.7.2/docs/overview/images/interferometry/model_visibilities.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/reconstruction.png` & `autogalaxy-2023.7.7.2/docs/overview/images/interferometry/reconstruction.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/uv_wavelengths.png` & `autogalaxy-2023.7.7.2/docs/overview/images/interferometry/uv_wavelengths.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/interferometry/visibilities.png` & `autogalaxy-2023.7.7.2/docs/overview/images/interferometry/visibilities.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/modeling/cornerplot.png` & `autogalaxy-2023.7.7.2/docs/overview/images/modeling/cornerplot.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/modeling/image.png` & `autogalaxy-2023.7.7.2/docs/overview/images/modeling/image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/modeling/subplot_fit.png` & `autogalaxy-2023.7.7.2/docs/overview/images/modeling/subplot_fit.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/dirty_image.png` & `autogalaxy-2023.7.7.2/docs/overview/images/multiwavelength/dirty_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/g_decomposed_image.png` & `autogalaxy-2023.7.7.2/docs/overview/images/multiwavelength/g_decomposed_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/g_image.png` & `autogalaxy-2023.7.7.2/docs/overview/images/multiwavelength/g_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/r_decomposed_image.png` & `autogalaxy-2023.7.7.2/docs/overview/images/multiwavelength/r_decomposed_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/multiwavelength/r_image.png` & `autogalaxy-2023.7.7.2/docs/overview/images/multiwavelength/r_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/pixelizations/image.png` & `autogalaxy-2023.7.7.2/docs/overview/images/pixelizations/image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/pixelizations/rectangular.png` & `autogalaxy-2023.7.7.2/docs/overview/images/pixelizations/rectangular.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/simulating/ao.png` & `autogalaxy-2023.7.7.2/docs/overview/images/simulating/ao.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/simulating/euclid.png` & `autogalaxy-2023.7.7.2/docs/overview/images/simulating/euclid.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/simulating/hst.png` & `autogalaxy-2023.7.7.2/docs/overview/images/simulating/hst.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/simulating/image.png` & `autogalaxy-2023.7.7.2/docs/overview/images/simulating/image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/simulating/noise_map.png` & `autogalaxy-2023.7.7.2/docs/overview/images/simulating/noise_map.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/simulating/psf.png` & `autogalaxy-2023.7.7.2/docs/overview/images/simulating/psf.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/images/simulating/vro.png` & `autogalaxy-2023.7.7.2/docs/overview/images/simulating/vro.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/overview_1_galaxies.rst` & `autogalaxy-2023.7.7.2/docs/overview/overview_1_galaxies.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/overview_2_fitting.rst` & `autogalaxy-2023.7.7.2/docs/overview/overview_2_fitting.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/overview_3_modeling.rst` & `autogalaxy-2023.7.7.2/docs/overview/overview_3_modeling.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/overview_4_simulate.rst` & `autogalaxy-2023.7.7.2/docs/overview/overview_4_simulate.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/overview_5_pixelizations.rst` & `autogalaxy-2023.7.7.2/docs/overview/overview_5_pixelizations.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/overview_6_interferometry.rst` & `autogalaxy-2023.7.7.2/docs/overview/overview_6_interferometry.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/docs/overview/overview_7_multi_wavelength.rst` & `autogalaxy-2023.7.7.2/docs/overview/overview_7_multi_wavelength.rst`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/files/citations.bib` & `autogalaxy-2023.7.7.2/files/citations.bib`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/files/citations.md` & `autogalaxy-2023.7.7.2/files/citations.md`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/files/citations.tex` & `autogalaxy-2023.7.7.2/files/citations.tex`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/files/dirty_image.png` & `autogalaxy-2023.7.7.2/files/dirty_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/files/model_dirty_image.png` & `autogalaxy-2023.7.7.2/files/model_dirty_image.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/files/non_parametric.png` & `autogalaxy-2023.7.7.2/files/non_parametric.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/files/observed.png` & `autogalaxy-2023.7.7.2/files/observed.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/files/parametric.png` & `autogalaxy-2023.7.7.2/files/parametric.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/files/visibilities.png` & `autogalaxy-2023.7.7.2/files/visibilities.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/paper/almacombined.png` & `autogalaxy-2023.7.7.2/paper/almacombined.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/paper/hstcombined.png` & `autogalaxy-2023.7.7.2/paper/hstcombined.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/paper/observed.pdf` & `autogalaxy-2023.7.7.2/paper/observed.pdf`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/paper/paper.bib` & `autogalaxy-2023.7.7.2/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/paper/paper.json` & `autogalaxy-2023.7.7.2/paper/paper.json`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/paper/paper.md` & `autogalaxy-2023.7.7.2/paper/paper.md`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/paper/parametric.png` & `autogalaxy-2023.7.7.2/paper/parametric.png`

 * *Files identical despite different names*

### Comparing `autogalaxy-2023.7.7.1/setup.py` & `autogalaxy-2023.7.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "2023.7.7.1")
+version = environ.get("VERSION", "2023.7.7.2")
 requirements.extend(
     [f"autoconf=={version}", f"autoarray=={version}", f"autofit=={version}"]
 )
 
 
 def config_packages(directory):
     paths = [directory.replace("/", ".")]
```

### Comparing `autogalaxy-2023.7.7.1/zenodo.json` & `autogalaxy-2023.7.7.2/zenodo.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9398148148148149%*

 * *Differences: {"'related_identifiers'": "{0: {'identifier': "*

 * *                          "'https://github.com/Jammy2211/PyAutoGalaxy/tree/2023.7.7.2'}}",*

 * * "'version'": "'2023.7.7.2'"}*

```diff
@@ -55,21 +55,21 @@
         }
     ],
     "description": "Release which is tied to the publication of PyAutoGalaxy in the Journal of Open Source software (JOSS).",
     "license": "other-open",
     "publication_date": "2023-01-19",
     "related_identifiers": [
         {
-            "identifier": "https://github.com/Jammy2211/PyAutoGalaxy/tree/2023.7.7.1",
+            "identifier": "https://github.com/Jammy2211/PyAutoGalaxy/tree/2023.7.7.2",
             "relation": "isSupplementTo",
             "scheme": "url"
         },
         {
             "identifier": "10.5281/zenodo.7546914",
             "relation": "isVersionOf",
             "scheme": "doi"
         }
     ],
     "title": "PyAutoGalaxy: Open-Source Multiwavelength Galaxy Structure & Morphology",
     "upload_type": "software",
-    "version": "2023.7.7.1"
+    "version": "2023.7.7.2"
 }
```

