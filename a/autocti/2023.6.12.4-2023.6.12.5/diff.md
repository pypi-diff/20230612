# Comparing `tmp/autocti-2023.6.12.4.tar.gz` & `tmp/autocti-2023.6.12.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocti-2023.6.12.4.tar", last modified: Mon Jun 12 13:49:12 2023, max compression
+gzip compressed data, was "autocti-2023.6.12.5.tar", last modified: Mon Jun 12 14:10:29 2023, max compression
```

## Comparing `autocti-2023.6.12.4.tar` & `autocti-2023.6.12.5.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.780870 autocti-2023.6.12.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/CITATIONS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-06-12 13:49:12.780870 autocti-2023.6.12.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.764870 autocti-2023.6.12.4/autocti/
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.768870 autocti-2023.6.12.4/autocti/aggregator/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/aggregator/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/aggregator/cti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/aggregator/dataset_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/aggregator/fit_dataset_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/aggregator/fit_imaging_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/aggregator/imaging_ci.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.768870 autocti-2023.6.12.4/autocti/charge_injection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/ci_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/hyper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.768870 autocti-2023.6.12.4/autocti/charge_injection/imaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/imaging/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/imaging/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/imaging/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17201 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/master.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.768870 autocti-2023.6.12.4/autocti/charge_injection/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/mock/mock_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.768870 autocti-2023.6.12.4/autocti/charge_injection/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/model/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/ou_sim_ci.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.768870 autocti-2023.6.12.4/autocti/charge_injection/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/plot/fit_ci_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14863 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/charge_injection/plot/imaging_ci_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.768870 autocti-2023.6.12.4/autocti/clocker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/clocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/clocker/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/clocker/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)    37568 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/clocker/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.768870 autocti-2023.6.12.4/autocti/config/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/config/general.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/config/notation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.768870 autocti-2023.6.12.4/autocti/config/priors/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/config/priors/ccd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/config/priors/hyper.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/config/priors/traps.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/config/visualize.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.768870 autocti-2023.6.12.4/autocti/cosmics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/cosmics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/cosmics/cosmics.py
--rw-r--r--   0 runner    (1001) docker     (123)    41101 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/cosmics/cr_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/cosmics/cr_lengths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.772870 autocti-2023.6.12.4/autocti/dataset_1d/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/dataset_1d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.772870 autocti-2023.6.12.4/autocti/dataset_1d/dataset_1d/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/dataset_1d/dataset_1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/dataset_1d/dataset_1d/dataset_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/dataset_1d/dataset_1d/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/dataset_1d/dataset_1d/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/dataset_1d/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.772870 autocti-2023.6.12.4/autocti/dataset_1d/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/dataset_1d/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/dataset_1d/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/dataset_1d/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/dataset_1d/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.772870 autocti-2023.6.12.4/autocti/dataset_1d/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/dataset_1d/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/dataset_1d/plot/dataset_1d_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/dataset_1d/plot/fit_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.772870 autocti-2023.6.12.4/autocti/extract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.772870 autocti-2023.6.12.4/autocti/extract/one_d/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/one_d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/one_d/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/one_d/eper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/one_d/fpr.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/one_d/master.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/one_d/overscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.772870 autocti-2023.6.12.4/autocti/extract/two_d/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/extract_2d_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    19949 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/master.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.772870 autocti-2023.6.12.4/autocti/extract/two_d/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/parallel/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/parallel/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/parallel/eper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/parallel/fpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/parallel/overscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/parallel/pedestal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.776870 autocti-2023.6.12.4/autocti/extract/two_d/serial/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/serial/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/serial/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/serial/eper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/serial/fpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/serial/overscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/serial/overscan_no_eper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/extract/two_d/serial/prescan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.776870 autocti-2023.6.12.4/autocti/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/instruments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.776870 autocti-2023.6.12.4/autocti/instruments/acs/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/instruments/acs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/instruments/acs/acs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/instruments/acs/array_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/instruments/acs/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/instruments/acs/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/instruments/acs/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.776870 autocti-2023.6.12.4/autocti/instruments/euclid/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/instruments/euclid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/instruments/euclid/array_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/instruments/euclid/euclid_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/instruments/euclid/header.py
--rw-r--r--   0 runner    (1001) docker     (123)    17129 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/instruments/euclid/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.776870 autocti-2023.6.12.4/autocti/layout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/layout/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/layout/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.776870 autocti-2023.6.12.4/autocti/mask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/mask/mask_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/mask/mask_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.776870 autocti-2023.6.12.4/autocti/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/model/model_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/model/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.776870 autocti-2023.6.12.4/autocti/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/plot/abstract_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.776870 autocti-2023.6.12.4/autocti/plot/get_visuals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/plot/get_visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/plot/get_visuals/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/plot/get_visuals/two_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/preloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.776870 autocti-2023.6.12.4/autocti/util/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/autocti/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:12.776870 autocti-2023.6.12.4/autocti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-12 13:49:12.000000 autocti-2023.6.12.4/autocti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:49:12.780870 autocti-2023.6.12.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-12 13:49:03.000000 autocti-2023.6.12.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.048838 autocti-2023.6.12.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/CITATIONS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-06-12 14:10:29.048838 autocti-2023.6.12.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.032838 autocti-2023.6.12.5/autocti/
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.036838 autocti-2023.6.12.5/autocti/aggregator/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/aggregator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/aggregator/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/aggregator/cti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/aggregator/dataset_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/aggregator/fit_dataset_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/aggregator/fit_imaging_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/aggregator/imaging_ci.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.036838 autocti-2023.6.12.5/autocti/charge_injection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/ci_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/hyper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.036838 autocti-2023.6.12.5/autocti/charge_injection/imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/imaging/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/imaging/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/imaging/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17201 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/master.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.036838 autocti-2023.6.12.5/autocti/charge_injection/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/mock/mock_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.036838 autocti-2023.6.12.5/autocti/charge_injection/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/model/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/ou_sim_ci.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.036838 autocti-2023.6.12.5/autocti/charge_injection/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/plot/fit_ci_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14863 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/charge_injection/plot/imaging_ci_plotters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.036838 autocti-2023.6.12.5/autocti/clocker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/clocker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/clocker/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/clocker/one_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37568 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/clocker/two_d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.040838 autocti-2023.6.12.5/autocti/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/config/general.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/config/notation.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.040838 autocti-2023.6.12.5/autocti/config/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/config/priors/ccd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/config/priors/hyper.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/config/priors/traps.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/config/visualize.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.040838 autocti-2023.6.12.5/autocti/cosmics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/cosmics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/cosmics/cosmics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41101 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/cosmics/cr_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/cosmics/cr_lengths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.040838 autocti-2023.6.12.5/autocti/dataset_1d/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/dataset_1d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.040838 autocti-2023.6.12.5/autocti/dataset_1d/dataset_1d/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/dataset_1d/dataset_1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/dataset_1d/dataset_1d/dataset_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/dataset_1d/dataset_1d/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/dataset_1d/dataset_1d/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/dataset_1d/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.040838 autocti-2023.6.12.5/autocti/dataset_1d/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/dataset_1d/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/dataset_1d/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/dataset_1d/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/dataset_1d/model/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.040838 autocti-2023.6.12.5/autocti/dataset_1d/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/dataset_1d/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/dataset_1d/plot/dataset_1d_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/dataset_1d/plot/fit_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.040838 autocti-2023.6.12.5/autocti/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.040838 autocti-2023.6.12.5/autocti/extract/one_d/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/one_d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/one_d/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/one_d/eper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/one_d/fpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/one_d/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/one_d/overscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.044838 autocti-2023.6.12.5/autocti/extract/two_d/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/extract_2d_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19949 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/master.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.044838 autocti-2023.6.12.5/autocti/extract/two_d/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/parallel/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/parallel/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/parallel/eper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/parallel/fpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/parallel/overscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/parallel/pedestal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.044838 autocti-2023.6.12.5/autocti/extract/two_d/serial/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/serial/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/serial/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/serial/eper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/serial/fpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/serial/overscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/serial/overscan_no_eper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/extract/two_d/serial/prescan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.044838 autocti-2023.6.12.5/autocti/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/instruments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.044838 autocti-2023.6.12.5/autocti/instruments/acs/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/instruments/acs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/instruments/acs/acs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/instruments/acs/array_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/instruments/acs/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/instruments/acs/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/instruments/acs/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.048838 autocti-2023.6.12.5/autocti/instruments/euclid/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/instruments/euclid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/instruments/euclid/array_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/instruments/euclid/euclid_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/instruments/euclid/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17129 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/instruments/euclid/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.048838 autocti-2023.6.12.5/autocti/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/layout/one_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/layout/two_d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.048838 autocti-2023.6.12.5/autocti/mask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/mask/mask_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/mask/mask_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.048838 autocti-2023.6.12.5/autocti/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/model/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/model/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/model/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.048838 autocti-2023.6.12.5/autocti/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/plot/abstract_plotters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.048838 autocti-2023.6.12.5/autocti/plot/get_visuals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/plot/get_visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/plot/get_visuals/one_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/plot/get_visuals/two_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/preloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.048838 autocti-2023.6.12.5/autocti/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/autocti/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:29.048838 autocti-2023.6.12.5/autocti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-12 14:10:29.000000 autocti-2023.6.12.5/autocti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:10:29.048838 autocti-2023.6.12.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-12 14:10:17.000000 autocti-2023.6.12.5/setup.py
```

### Comparing `autocti-2023.6.12.4/CITATIONS.rst` & `autocti-2023.6.12.5/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/LICENSE` & `autocti-2023.6.12.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/PKG-INFO` & `autocti-2023.6.12.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocti
-Version: 2023.6.12.4
+Version: 2023.6.12.5
 Summary: PyAutoCTI: Charge Transfer Inefficiency Modeling
 Home-page: https://github.com/jammy2211/PyAutoCTI
 Author: James Nightingale, Richard Massey, Jacob Kegerreis and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
```

### Comparing `autocti-2023.6.12.4/README.rst` & `autocti-2023.6.12.5/README.rst`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/__init__.py` & `autocti-2023.6.12.5/autocti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,8 @@
 from . import plot
 from . import mock as m  # noqa
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2023.6.12.4"
+__version__ = "2023.6.12.5"
```

### Comparing `autocti-2023.6.12.4/autocti/aggregator/abstract.py` & `autocti-2023.6.12.5/autocti/aggregator/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/aggregator/cti.py` & `autocti-2023.6.12.5/autocti/aggregator/cti.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/aggregator/dataset_1d.py` & `autocti-2023.6.12.5/autocti/aggregator/dataset_1d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/aggregator/fit_dataset_1d.py` & `autocti-2023.6.12.5/autocti/aggregator/fit_dataset_1d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/aggregator/fit_imaging_ci.py` & `autocti-2023.6.12.5/autocti/aggregator/fit_imaging_ci.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/aggregator/imaging_ci.py` & `autocti-2023.6.12.5/autocti/aggregator/imaging_ci.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/ci_util.py` & `autocti-2023.6.12.5/autocti/charge_injection/ci_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/fit.py` & `autocti-2023.6.12.5/autocti/charge_injection/fit.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/hyper.py` & `autocti-2023.6.12.5/autocti/charge_injection/hyper.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/imaging/imaging.py` & `autocti-2023.6.12.5/autocti/charge_injection/imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/imaging/settings.py` & `autocti-2023.6.12.5/autocti/charge_injection/imaging/settings.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/imaging/simulator.py` & `autocti-2023.6.12.5/autocti/charge_injection/imaging/simulator.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/layout.py` & `autocti-2023.6.12.5/autocti/charge_injection/layout.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/master.py` & `autocti-2023.6.12.5/autocti/charge_injection/master.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/mock/mock_result.py` & `autocti-2023.6.12.5/autocti/charge_injection/mock/mock_result.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/model/analysis.py` & `autocti-2023.6.12.5/autocti/charge_injection/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/model/result.py` & `autocti-2023.6.12.5/autocti/charge_injection/model/result.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/model/visualizer.py` & `autocti-2023.6.12.5/autocti/charge_injection/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/ou_sim_ci.py` & `autocti-2023.6.12.5/autocti/charge_injection/ou_sim_ci.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/plot/fit_ci_plotters.py` & `autocti-2023.6.12.5/autocti/charge_injection/plot/fit_ci_plotters.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/plot/imaging_ci_plotters.py` & `autocti-2023.6.12.5/autocti/charge_injection/plot/imaging_ci_plotters.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/clocker/abstract.py` & `autocti-2023.6.12.5/autocti/clocker/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/clocker/one_d.py` & `autocti-2023.6.12.5/autocti/clocker/one_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/clocker/two_d.py` & `autocti-2023.6.12.5/autocti/clocker/two_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/config/notation.yaml` & `autocti-2023.6.12.5/autocti/config/notation.yaml`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/config/priors/ccd.yaml` & `autocti-2023.6.12.5/autocti/config/priors/ccd.yaml`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/config/priors/traps.yaml` & `autocti-2023.6.12.5/autocti/config/priors/traps.yaml`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/cosmics/cosmics.py` & `autocti-2023.6.12.5/autocti/cosmics/cosmics.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/cosmics/cr_distances.py` & `autocti-2023.6.12.5/autocti/cosmics/cr_distances.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/cosmics/cr_lengths.py` & `autocti-2023.6.12.5/autocti/cosmics/cr_lengths.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/dataset_1d/dataset_1d.py` & `autocti-2023.6.12.5/autocti/dataset_1d/dataset_1d/dataset_1d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/dataset_1d/simulator.py` & `autocti-2023.6.12.5/autocti/dataset_1d/dataset_1d/simulator.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/fit.py` & `autocti-2023.6.12.5/autocti/dataset_1d/fit.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/model/analysis.py` & `autocti-2023.6.12.5/autocti/dataset_1d/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/model/visualizer.py` & `autocti-2023.6.12.5/autocti/dataset_1d/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/plot/dataset_1d_plotters.py` & `autocti-2023.6.12.5/autocti/dataset_1d/plot/dataset_1d_plotters.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/plot/fit_plotters.py` & `autocti-2023.6.12.5/autocti/dataset_1d/plot/fit_plotters.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/exc.py` & `autocti-2023.6.12.5/autocti/exc.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/one_d/abstract.py` & `autocti-2023.6.12.5/autocti/extract/one_d/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/one_d/eper.py` & `autocti-2023.6.12.5/autocti/extract/one_d/eper.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/one_d/fpr.py` & `autocti-2023.6.12.5/autocti/extract/one_d/fpr.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/one_d/master.py` & `autocti-2023.6.12.5/autocti/extract/one_d/master.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/one_d/overscan.py` & `autocti-2023.6.12.5/autocti/extract/one_d/overscan.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/settings.py` & `autocti-2023.6.12.5/autocti/extract/settings.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/abstract.py` & `autocti-2023.6.12.5/autocti/extract/two_d/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/extract_2d_util.py` & `autocti-2023.6.12.5/autocti/extract/two_d/extract_2d_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/master.py` & `autocti-2023.6.12.5/autocti/extract/two_d/master.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/parallel/abstract.py` & `autocti-2023.6.12.5/autocti/extract/two_d/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/parallel/calibration.py` & `autocti-2023.6.12.5/autocti/extract/two_d/parallel/calibration.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/parallel/eper.py` & `autocti-2023.6.12.5/autocti/extract/two_d/parallel/eper.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/parallel/fpr.py` & `autocti-2023.6.12.5/autocti/extract/two_d/parallel/fpr.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/parallel/overscan.py` & `autocti-2023.6.12.5/autocti/extract/two_d/parallel/overscan.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/parallel/pedestal.py` & `autocti-2023.6.12.5/autocti/extract/two_d/parallel/pedestal.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/abstract.py` & `autocti-2023.6.12.5/autocti/extract/two_d/serial/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/calibration.py` & `autocti-2023.6.12.5/autocti/extract/two_d/serial/calibration.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/eper.py` & `autocti-2023.6.12.5/autocti/extract/two_d/serial/eper.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/fpr.py` & `autocti-2023.6.12.5/autocti/extract/two_d/serial/fpr.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/overscan.py` & `autocti-2023.6.12.5/autocti/extract/two_d/serial/overscan.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/overscan_no_eper.py` & `autocti-2023.6.12.5/autocti/extract/two_d/serial/overscan_no_eper.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/prescan.py` & `autocti-2023.6.12.5/autocti/extract/two_d/serial/prescan.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/fixtures.py` & `autocti-2023.6.12.5/autocti/fixtures.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/acs/acs_util.py` & `autocti-2023.6.12.5/autocti/instruments/acs/acs_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/acs/array_2d.py` & `autocti-2023.6.12.5/autocti/instruments/acs/array_2d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/acs/header.py` & `autocti-2023.6.12.5/autocti/instruments/acs/header.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/acs/image.py` & `autocti-2023.6.12.5/autocti/instruments/acs/image.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/acs/layout.py` & `autocti-2023.6.12.5/autocti/instruments/acs/layout.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/euclid/array_2d.py` & `autocti-2023.6.12.5/autocti/instruments/euclid/array_2d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/euclid/euclid_util.py` & `autocti-2023.6.12.5/autocti/instruments/euclid/euclid_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/euclid/header.py` & `autocti-2023.6.12.5/autocti/instruments/euclid/header.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/euclid/layout.py` & `autocti-2023.6.12.5/autocti/instruments/euclid/layout.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/layout/one_d.py` & `autocti-2023.6.12.5/autocti/layout/one_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/layout/two_d.py` & `autocti-2023.6.12.5/autocti/layout/two_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/mask/mask_1d.py` & `autocti-2023.6.12.5/autocti/mask/mask_1d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/mask/mask_2d.py` & `autocti-2023.6.12.5/autocti/mask/mask_2d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/model/model_util.py` & `autocti-2023.6.12.5/autocti/model/model_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/model/result.py` & `autocti-2023.6.12.5/autocti/model/result.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/model/settings.py` & `autocti-2023.6.12.5/autocti/model/settings.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/model/visualizer.py` & `autocti-2023.6.12.5/autocti/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/plot/__init__.py` & `autocti-2023.6.12.5/autocti/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/plot/abstract_plotters.py` & `autocti-2023.6.12.5/autocti/plot/abstract_plotters.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/plot/get_visuals/one_d.py` & `autocti-2023.6.12.5/autocti/plot/get_visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/plot/get_visuals/two_d.py` & `autocti-2023.6.12.5/autocti/plot/get_visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/preloads.py` & `autocti-2023.6.12.5/autocti/preloads.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/util/__init__.py` & `autocti-2023.6.12.5/autocti/util/__init__.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti.egg-info/SOURCES.txt` & `autocti-2023.6.12.5/autocti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/setup.py` & `autocti-2023.6.12.5/setup.py`

 * *Files identical despite different names*

