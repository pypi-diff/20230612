# Comparing `tmp/autocti-2023.6.12.4.tar.gz` & `tmp/autocti-2023.7.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocti-2023.6.12.4.tar", last modified: Mon Jun 12 13:49:12 2023, max compression
+gzip compressed data, was "autocti-2023.7.7.3.tar", last modified: Wed Jun  7 11:31:46 2023, max compression
```

## Comparing `autocti-2023.6.12.4.tar` & `autocti-2023.7.7.3.tar`

### file list

```diff
@@ -1,156 +1,271 @@
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
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.344378 autocti-2023.7.7.3/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.744441 autocti-2023.7.7.3/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.795336 autocti-2023.7.7.3/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      475 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/.github/workflows/draft-pdf.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2608 2023-06-03 12:16:24.000000 autocti-2023.7.7.3/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1111 2022-12-19 11:17:33.000000 autocti-2023.7.7.3/CITATIONS.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18831 2022-12-19 11:17:33.000000 autocti-2023.7.7.3/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2470 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/CONTRIBUTING.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1095 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      379 2022-11-28 11:07:42.000000 autocti-2023.7.7.3/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9800 2023-06-07 11:31:46.343378 autocti-2023.7.7.3/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8950 2023-06-03 09:39:55.000000 autocti-2023.7.7.3/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.804283 autocti-2023.7.7.3/autocti/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3411 2023-06-07 11:30:17.000000 autocti-2023.7.7.3/autocti/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.819299 autocti-2023.7.7.3/autocti/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      281 2023-05-15 17:43:12.000000 autocti-2023.7.7.3/autocti/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7455 2023-05-25 17:24:17.000000 autocti-2023.7.7.3/autocti/aggregator/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1839 2023-05-15 17:43:12.000000 autocti-2023.7.7.3/autocti/aggregator/cti.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2276 2023-05-25 17:24:17.000000 autocti-2023.7.7.3/autocti/aggregator/dataset_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3925 2023-06-03 10:36:19.000000 autocti-2023.7.7.3/autocti/aggregator/fit_dataset_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3578 2023-06-03 09:42:32.000000 autocti-2023.7.7.3/autocti/aggregator/fit_imaging_ci.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2277 2023-05-25 17:24:17.000000 autocti-2023.7.7.3/autocti/aggregator/imaging_ci.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.834294 autocti-2023.7.7.3/autocti/charge_injection/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/charge_injection/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2899 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/charge_injection/ci_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4971 2023-06-03 09:58:57.000000 autocti-2023.7.7.3/autocti/charge_injection/fit.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1500 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/charge_injection/hyper.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.843536 autocti-2023.7.7.3/autocti/charge_injection/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/charge_injection/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8478 2023-06-03 10:26:41.000000 autocti-2023.7.7.3/autocti/charge_injection/imaging/imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1833 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/charge_injection/imaging/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10080 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/charge_injection/imaging/simulator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17201 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/charge_injection/layout.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1174 2023-01-13 16:58:40.000000 autocti-2023.7.7.3/autocti/charge_injection/master.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.847537 autocti-2023.7.7.3/autocti/charge_injection/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/charge_injection/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3790 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/charge_injection/mock/mock_result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.857535 autocti-2023.7.7.3/autocti/charge_injection/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/charge_injection/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13653 2023-06-03 10:26:41.000000 autocti-2023.7.7.3/autocti/charge_injection/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1132 2023-06-03 10:26:26.000000 autocti-2023.7.7.3/autocti/charge_injection/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12970 2023-06-03 09:42:58.000000 autocti-2023.7.7.3/autocti/charge_injection/model/visualizer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9610 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/charge_injection/ou_sim_ci.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.865535 autocti-2023.7.7.3/autocti/charge_injection/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/charge_injection/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20366 2023-06-03 09:58:40.000000 autocti-2023.7.7.3/autocti/charge_injection/plot/fit_ci_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14182 2023-06-03 09:50:54.000000 autocti-2023.7.7.3/autocti/charge_injection/plot/imaging_ci_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.873535 autocti-2023.7.7.3/autocti/clocker/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/clocker/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2667 2022-12-20 20:16:56.000000 autocti-2023.7.7.3/autocti/clocker/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8978 2023-06-07 11:23:21.000000 autocti-2023.7.7.3/autocti/clocker/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    37570 2023-06-07 11:23:21.000000 autocti-2023.7.7.3/autocti/clocker/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.880536 autocti-2023.7.7.3/autocti/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      367 2023-01-15 20:17:47.000000 autocti-2023.7.7.3/autocti/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      688 2022-12-02 15:59:51.000000 autocti-2023.7.7.3/autocti/config/notation.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.887535 autocti-2023.7.7.3/autocti/config/priors/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      648 2023-02-27 14:53:06.000000 autocti-2023.7.7.3/autocti/config/priors/ccd.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      210 2022-12-02 15:59:51.000000 autocti-2023.7.7.3/autocti/config/priors/hyper.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1145 2022-12-05 10:42:13.000000 autocti-2023.7.7.3/autocti/config/priors/traps.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      369 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/config/visualize.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.897535 autocti-2023.7.7.3/autocti/cosmics/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/cosmics/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11375 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/cosmics/cosmics.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41101 2022-12-17 13:44:39.000000 autocti-2023.7.7.3/autocti/cosmics/cr_distances.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13590 2022-12-17 13:44:38.000000 autocti-2023.7.7.3/autocti/cosmics/cr_lengths.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.901535 autocti-2023.7.7.3/autocti/dataset_1d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/dataset_1d/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.912536 autocti-2023.7.7.3/autocti/dataset_1d/dataset_1d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/dataset_1d/dataset_1d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6766 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/dataset_1d/dataset_1d/dataset_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       92 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/dataset_1d/dataset_1d/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5606 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/dataset_1d/dataset_1d/simulator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      970 2022-12-13 16:21:22.000000 autocti-2023.7.7.3/autocti/dataset_1d/fit.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.922537 autocti-2023.7.7.3/autocti/dataset_1d/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/dataset_1d/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9268 2023-05-15 17:43:12.000000 autocti-2023.7.7.3/autocti/dataset_1d/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      101 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/dataset_1d/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12051 2023-06-03 10:17:27.000000 autocti-2023.7.7.3/autocti/dataset_1d/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.929536 autocti-2023.7.7.3/autocti/dataset_1d/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/dataset_1d/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9670 2023-06-03 09:50:54.000000 autocti-2023.7.7.3/autocti/dataset_1d/plot/dataset_1d_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13682 2023-06-03 10:16:35.000000 autocti-2023.7.7.3/autocti/dataset_1d/plot/fit_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      560 2023-02-14 15:40:54.000000 autocti-2023.7.7.3/autocti/exc.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.934537 autocti-2023.7.7.3/autocti/extract/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/extract/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.950536 autocti-2023.7.7.3/autocti/extract/one_d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/extract/one_d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7551 2023-05-16 14:13:25.000000 autocti-2023.7.7.3/autocti/extract/one_d/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2113 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/extract/one_d/eper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1059 2023-03-21 12:51:53.000000 autocti-2023.7.7.3/autocti/extract/one_d/fpr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10366 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/extract/one_d/master.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1227 2023-03-21 12:51:53.000000 autocti-2023.7.7.3/autocti/extract/one_d/overscan.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2146 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/extract/settings.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.960537 autocti-2023.7.7.3/autocti/extract/two_d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/extract/two_d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16148 2023-05-16 14:13:12.000000 autocti-2023.7.7.3/autocti/extract/two_d/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2356 2023-03-21 12:51:53.000000 autocti-2023.7.7.3/autocti/extract/two_d/extract_2d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19949 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/extract/two_d/master.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:45.982869 autocti-2023.7.7.3/autocti/extract/two_d/parallel/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/extract/two_d/parallel/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13507 2023-05-25 17:24:09.000000 autocti-2023.7.7.3/autocti/extract/two_d/parallel/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11608 2023-06-03 10:32:33.000000 autocti-2023.7.7.3/autocti/extract/two_d/parallel/calibration.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7164 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/extract/two_d/parallel/eper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4280 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/extract/two_d/parallel/fpr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4619 2023-03-21 12:51:53.000000 autocti-2023.7.7.3/autocti/extract/two_d/parallel/overscan.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5472 2023-03-21 12:51:53.000000 autocti-2023.7.7.3/autocti/extract/two_d/parallel/pedestal.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.007563 autocti-2023.7.7.3/autocti/extract/two_d/serial/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:03.000000 autocti-2023.7.7.3/autocti/extract/two_d/serial/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5951 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/extract/two_d/serial/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10782 2023-06-03 10:32:33.000000 autocti-2023.7.7.3/autocti/extract/two_d/serial/calibration.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6160 2023-03-21 12:51:53.000000 autocti-2023.7.7.3/autocti/extract/two_d/serial/eper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3793 2023-03-21 12:51:53.000000 autocti-2023.7.7.3/autocti/extract/two_d/serial/fpr.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4595 2023-03-21 12:51:53.000000 autocti-2023.7.7.3/autocti/extract/two_d/serial/overscan.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3790 2023-05-15 17:37:57.000000 autocti-2023.7.7.3/autocti/extract/two_d/serial/overscan_no_eper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3110 2023-03-21 12:51:53.000000 autocti-2023.7.7.3/autocti/extract/two_d/serial/prescan.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5622 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/autocti/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.010564 autocti-2023.7.7.3/autocti/instruments/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      122 2022-10-21 09:42:48.000000 autocti-2023.7.7.3/autocti/instruments/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.025563 autocti-2023.7.7.3/autocti/instruments/acs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      151 2022-10-24 13:23:41.000000 autocti-2023.7.7.3/autocti/instruments/acs/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6053 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/autocti/instruments/acs/acs_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11226 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/autocti/instruments/acs/array_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3037 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/autocti/instruments/acs/header.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4794 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/autocti/instruments/acs/image.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1061 2022-10-21 13:55:34.000000 autocti-2023.7.7.3/autocti/instruments/acs/layout.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.039233 autocti-2023.7.7.3/autocti/instruments/euclid/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      107 2022-10-21 13:47:30.000000 autocti-2023.7.7.3/autocti/instruments/euclid/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12883 2023-01-13 16:58:40.000000 autocti-2023.7.7.3/autocti/instruments/euclid/array_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      711 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/autocti/instruments/euclid/euclid_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      851 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/autocti/instruments/euclid/header.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    17129 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/autocti/instruments/euclid/layout.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.046233 autocti-2023.7.7.3/autocti/layout/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/autocti/layout/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2819 2023-05-30 13:00:37.000000 autocti-2023.7.7.3/autocti/layout/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11677 2023-05-25 17:24:17.000000 autocti-2023.7.7.3/autocti/layout/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.053694 autocti-2023.7.7.3/autocti/mask/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/autocti/mask/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2447 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/autocti/mask/mask_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11085 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/autocti/mask/mask_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      193 2023-02-08 17:48:18.000000 autocti-2023.7.7.3/autocti/mock.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.065694 autocti-2023.7.7.3/autocti/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/autocti/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3711 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/autocti/model/model_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      603 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/autocti/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1632 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/autocti/model/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1106 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/autocti/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.069693 autocti-2023.7.7.3/autocti/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2811 2023-06-03 09:48:03.000000 autocti-2023.7.7.3/autocti/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2752 2023-06-03 10:38:40.000000 autocti-2023.7.7.3/autocti/plot/abstract_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.077638 autocti-2023.7.7.3/autocti/plot/get_visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 16:14:32.000000 autocti-2023.7.7.3/autocti/plot/get_visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1215 2022-11-11 16:14:32.000000 autocti-2023.7.7.3/autocti/plot/get_visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3107 2023-06-03 09:58:40.000000 autocti-2023.7.7.3/autocti/plot/get_visuals/two_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2885 2022-12-18 14:37:25.000000 autocti-2023.7.7.3/autocti/preloads.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.079703 autocti-2023.7.7.3/autocti/util/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      829 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/autocti/util/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.341515 autocti-2023.7.7.3/autocti.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7804 2023-06-07 11:31:45.000000 autocti-2023.7.7.3/autocti.egg-info/SOURCES.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.086778 autocti-2023.7.7.3/docs/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.088791 autocti-2023.7.7.3/docs/_static/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/_static/.gitignore
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.093786 autocti-2023.7.7.3/docs/_templates/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2022-12-21 16:35:52.000000 autocti-2023.7.7.3/docs/_templates/custom-class-template.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2022-12-16 17:06:50.000000 autocti-2023.7.7.3/docs/_templates/custom_module_template.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.096302 autocti-2023.7.7.3/docs/advanced/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6858 2022-11-25 11:55:02.000000 autocti-2023.7.7.3/docs/advanced/database.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.110104 autocti-2023.7.7.3/docs/api/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      809 2022-12-20 20:00:42.000000 autocti-2023.7.7.3/docs/api/arctic.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      545 2022-12-20 20:00:42.000000 autocti-2023.7.7.3/docs/api/clocking.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1208 2023-01-13 16:58:40.000000 autocti-2023.7.7.3/docs/api/data.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      303 2022-12-20 20:00:42.000000 autocti-2023.7.7.3/docs/api/fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1480 2022-12-20 20:00:42.000000 autocti-2023.7.7.3/docs/api/modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2944 2022-12-20 20:00:42.000000 autocti-2023.7.7.3/docs/api/plot.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4623 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/docs/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.120266 autocti-2023.7.7.3/docs/general/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1111 2022-12-19 11:17:33.000000 autocti-2023.7.7.3/docs/general/citations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1015 2022-11-27 17:21:24.000000 autocti-2023.7.7.3/docs/general/configs.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      360 2022-11-27 17:21:24.000000 autocti-2023.7.7.3/docs/general/credits.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2256 2023-05-15 17:43:12.000000 autocti-2023.7.7.3/docs/general/workspace.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5281 2022-12-20 20:00:42.000000 autocti-2023.7.7.3/docs/index.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.137164 autocti-2023.7.7.3/docs/installation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1381 2022-12-06 16:43:06.000000 autocti-2023.7.7.3/docs/installation/arctic.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3203 2022-12-06 16:40:25.000000 autocti-2023.7.7.3/docs/installation/conda.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3360 2023-05-15 17:43:12.000000 autocti-2023.7.7.3/docs/installation/numba.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2450 2023-05-15 17:43:12.000000 autocti-2023.7.7.3/docs/installation/overview.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2783 2023-06-07 11:25:53.000000 autocti-2023.7.7.3/docs/installation/pip.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4642 2023-05-15 17:43:12.000000 autocti-2023.7.7.3/docs/installation/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5204 2023-05-15 17:43:12.000000 autocti-2023.7.7.3/docs/installation/troubleshooting.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.152609 autocti-2023.7.7.3/docs/overview/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.169638 autocti-2023.7.7.3/docs/overview/images/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   397515 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/ccd.gif
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   281375 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/ccd_schematic.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   514636 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/cti.gif
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   132888 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/cti_time_evolution.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.179660 autocti-2023.7.7.3/docs/overview/images/overview_1/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21797 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_1/array_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23382 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_1/array_1d_cti_corrected.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22695 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_1/array_1d_with_cti.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.196688 autocti-2023.7.7.3/docs/overview/images/overview_2/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22121 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_2/array_2d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23664 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_2/array_2d_cti_corrected.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22519 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_2/array_2d_parallel_cti.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24358 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_2/array_2d_parallel_serial_cti.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22449 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_2/array_2d_serial_cti.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.215228 autocti-2023.7.7.3/docs/overview/images/overview_3/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24750 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_3/density_1.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24719 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_3/density_2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26412 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_3/timescale_1.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25030 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_3/timescale_2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26471 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_3/volume_1.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26695 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_3/volume_2.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.245198 autocti-2023.7.7.3/docs/overview/images/overview_4/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34116 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_4/binned_parallel_eper.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    25079 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_4/binned_parallel_fpr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32451 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_4/binned_serial_eper.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31453 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_4/binned_serial_fpr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    79377 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_4/imaging_ci.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    47970 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_4/imaging_ci_eper.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44395 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_4/imaging_ci_fpr.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   351059 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_4/imaging_ci_non_uniform_cosmic_rays.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32372 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_4/pre_cti_image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.291046 autocti-2023.7.7.3/docs/overview/images/overview_5/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28538 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/chi_squared_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36932 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/chi_squared_map_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29730 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/chi_squared_map_good.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31056 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/chi_squared_map_masked.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35482 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/ci_image_masked.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    51137 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/dataset_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31199 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/normalized_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45032 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/normalized_residual_map_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31927 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/normalized_residual_map_good.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33155 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/normalized_residual_map_masked.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31172 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    47426 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/residual_map_1d.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30360 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/residual_map_good.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34986 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_5/residual_map_masked.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.320102 autocti-2023.7.7.3/docs/overview/images/overview_6/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   107188 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_6/fit_1d_100.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   120106 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_6/fit_1d_200000.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   102590 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_6/fit_1d_25000.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   105434 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_6/fit_1d_5000.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    80847 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_6/fit_2d_100.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    86775 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_6/fit_2d_200000.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    80846 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_6/fit_2d_25000.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    76721 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/overview_6/fit_2d_5000.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   542080 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/docs/overview/images/what_is_cti.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12544 2023-05-15 17:43:12.000000 autocti-2023.7.7.3/docs/overview/overview_1_what_is_cti.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10805 2023-05-15 17:43:12.000000 autocti-2023.7.7.3/docs/overview/overview_2_parallel_and_serial.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10013 2023-01-13 16:58:40.000000 autocti-2023.7.7.3/docs/overview/overview_3_cti_features.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11491 2023-06-03 09:42:32.000000 autocti-2023.7.7.3/docs/overview/overview_4_charge_injection_data.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14975 2023-06-03 10:29:07.000000 autocti-2023.7.7.3/docs/overview/overview_5_fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14938 2023-06-03 10:36:19.000000 autocti-2023.7.7.3/docs/overview/overview_6_cti_calibration.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      162 2023-06-07 11:25:53.000000 autocti-2023.7.7.3/docs/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       30 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/eden.ini
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.327103 autocti-2023.7.7.3/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14795 2022-11-27 17:05:27.000000 autocti-2023.7.7.3/files/citations.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1436 2022-11-27 17:05:27.000000 autocti-2023.7.7.3/files/citations.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2049 2022-11-27 17:10:36.000000 autocti-2023.7.7.3/files/citations.tex
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       13 2023-06-03 12:21:40.000000 autocti-2023.7.7.3/optional_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 11:31:46.339379 autocti-2023.7.7.3/paper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      180 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/paper/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   881609 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/paper/cti_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    98062 2023-05-15 17:37:58.000000 autocti-2023.7.7.3/paper/paper.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      829 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/paper/paper.json
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9817 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/paper/paper.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      917 2022-11-23 10:12:20.000000 autocti-2023.7.7.3/profiling
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      210 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/readthedocs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       13 2023-03-21 12:51:53.000000 autocti-2023.7.7.3/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-06-07 11:31:46.344378 autocti-2023.7.7.3/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1708 2023-06-07 11:31:41.000000 autocti-2023.7.7.3/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1875 2022-10-20 11:42:04.000000 autocti-2023.7.7.3/to_do_list
```

### Comparing `autocti-2023.6.12.4/CITATIONS.rst` & `autocti-2023.7.7.3/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/LICENSE` & `autocti-2023.7.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/PKG-INFO` & `autocti-2023.7.7.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocti
-Version: 2023.6.12.4
+Version: 2023.7.7.3
 Summary: PyAutoCTI: Charge Transfer Inefficiency Modeling
 Home-page: https://github.com/jammy2211/PyAutoCTI
 Author: James Nightingale, Richard Massey, Jacob Kegerreis and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
@@ -22,14 +22,17 @@
 
 PyAutoCTI: Charge Transfer Inefficiency Modeling
 ================================================
 
 .. |nbsp| unicode:: 0xA0
     :trim:
 
+.. |binder| image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/Jammy2211/autocti_workspace/HEAD
+
 .. |RTD| image:: https://readthedocs.org/projects/pyautocti/badge/?version=latest
     :target: https://pyautocti.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. |Tests| image:: https://github.com/Jammy2211/PyAutoCTI/actions/workflows/main.yml/badge.svg
    :target: https://github.com/Jammy2211/PyAutoCTI/actions
 
@@ -38,18 +41,19 @@
 
 .. |code-style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 .. |arXiv| image:: https://img.shields.io/badge/arXiv-1708.07377-blue
     :target: https://arxiv.org/abs/0909.0507
 
-|RTD| |Tests| |Build| |code-style| |arXiv|
+|binder| |RTD| |Tests| |Build| |code-style| |arXiv|
 
 `Installation Guide <https://pyautocti.readthedocs.io/en/latest/installation/overview.html>`_ |
 `readthedocs <https://pyautocti.readthedocs.io/en/latest/index.html>`_ |
+`Introduction on Binder <https://mybinder.org/v2/gh/Jammy2211/autocti_workspace/release?filepath=introduction.ipynb>`_ |
 `What is CTI? <https://pyautocti.readthedocs.io/en/latest/overview/overview_1_what_is_cti.html>`_
 
 Charge Transfer Inefficiency, or CTI for short, is an effect that occurs when acquiring imaging data from
 Charge Coupled Devices (CCDs). Due to radiation damage to the CCD's silicon lattice electrons are read-out inefficiently,
 creating a characteristic trailing or smearing effect.
 
 Here is an example of CTI in the Hubble space telescope, after decades of radiation damage:
@@ -66,17 +70,19 @@
 phenomena called weak gravitational lensing.
 
 Getting Started
 ---------------
 
 The following links are useful for new starters:
 
+- `The introduction Jupyter Notebook on Binder <https://mybinder.org/v2/gh/Jammy2211/autocti_workspace/release?filepath=introduction.ipynb>`_, where you can try **PyAutoCTI** in a web browser (without installation).
+
 - `The PyAutoCTI readthedocs <https://pyautocti.readthedocs.io/en/latest>`_, which includes `an installation guide <https://pyautocti.readthedocs.io/en/latest/installation/overview.html>`_ and an overview of **PyAutoCTI**'s core features.
 
-- `The autocti_workspace GitHub repository <https://github.com/Jammy2211/autocti_workspace>`_, which includes example scripts.
+- `The autocti_workspace GitHub repository <https://github.com/Jammy2211/autocti_workspace>`_, which includes example scripts and the `HowToCTI Jupyter notebook tutorials <https://github.com/Jammy2211/autocti_workspace/tree/master/notebooks/howtocti>`_ which give new users a step-by-step introduction to **PyAutoCTI**.
 
 API Overview
 ------------
 
 To model CTI, **PyAutoCTI** wraps the library **arCTIc** (https://github.com/jkeger/arctic).
 
 CTI can be added to an image as follows:
```

### Comparing `autocti-2023.6.12.4/README.rst` & `autocti-2023.7.7.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 PyAutoCTI: Charge Transfer Inefficiency Modeling
 ================================================
 
 .. |nbsp| unicode:: 0xA0
     :trim:
 
+.. |binder| image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/Jammy2211/autocti_workspace/HEAD
+
 .. |RTD| image:: https://readthedocs.org/projects/pyautocti/badge/?version=latest
     :target: https://pyautocti.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. |Tests| image:: https://github.com/Jammy2211/PyAutoCTI/actions/workflows/main.yml/badge.svg
    :target: https://github.com/Jammy2211/PyAutoCTI/actions
 
@@ -16,18 +19,19 @@
 
 .. |code-style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 .. |arXiv| image:: https://img.shields.io/badge/arXiv-1708.07377-blue
     :target: https://arxiv.org/abs/0909.0507
 
-|RTD| |Tests| |Build| |code-style| |arXiv|
+|binder| |RTD| |Tests| |Build| |code-style| |arXiv|
 
 `Installation Guide <https://pyautocti.readthedocs.io/en/latest/installation/overview.html>`_ |
 `readthedocs <https://pyautocti.readthedocs.io/en/latest/index.html>`_ |
+`Introduction on Binder <https://mybinder.org/v2/gh/Jammy2211/autocti_workspace/release?filepath=introduction.ipynb>`_ |
 `What is CTI? <https://pyautocti.readthedocs.io/en/latest/overview/overview_1_what_is_cti.html>`_
 
 Charge Transfer Inefficiency, or CTI for short, is an effect that occurs when acquiring imaging data from
 Charge Coupled Devices (CCDs). Due to radiation damage to the CCD's silicon lattice electrons are read-out inefficiently,
 creating a characteristic trailing or smearing effect.
 
 Here is an example of CTI in the Hubble space telescope, after decades of radiation damage:
@@ -44,17 +48,19 @@
 phenomena called weak gravitational lensing.
 
 Getting Started
 ---------------
 
 The following links are useful for new starters:
 
+- `The introduction Jupyter Notebook on Binder <https://mybinder.org/v2/gh/Jammy2211/autocti_workspace/release?filepath=introduction.ipynb>`_, where you can try **PyAutoCTI** in a web browser (without installation).
+
 - `The PyAutoCTI readthedocs <https://pyautocti.readthedocs.io/en/latest>`_, which includes `an installation guide <https://pyautocti.readthedocs.io/en/latest/installation/overview.html>`_ and an overview of **PyAutoCTI**'s core features.
 
-- `The autocti_workspace GitHub repository <https://github.com/Jammy2211/autocti_workspace>`_, which includes example scripts.
+- `The autocti_workspace GitHub repository <https://github.com/Jammy2211/autocti_workspace>`_, which includes example scripts and the `HowToCTI Jupyter notebook tutorials <https://github.com/Jammy2211/autocti_workspace/tree/master/notebooks/howtocti>`_ which give new users a step-by-step introduction to **PyAutoCTI**.
 
 API Overview
 ------------
 
 To model CTI, **PyAutoCTI** wraps the library **arCTIc** (https://github.com/jkeger/arctic).
 
 CTI can be added to an image as follows:
```

### Comparing `autocti-2023.6.12.4/autocti/__init__.py` & `autocti-2023.7.7.3/autocti/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,8 +68,8 @@
 from . import plot
 from . import mock as m  # noqa
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2023.6.12.4"
+__version__ = "2023.7.7.3"
```

### Comparing `autocti-2023.6.12.4/autocti/aggregator/abstract.py` & `autocti-2023.7.7.3/autocti/aggregator/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/aggregator/cti.py` & `autocti-2023.7.7.3/autocti/aggregator/cti.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/aggregator/dataset_1d.py` & `autocti-2023.7.7.3/autocti/aggregator/dataset_1d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/aggregator/fit_dataset_1d.py` & `autocti-2023.7.7.3/autocti/aggregator/fit_dataset_1d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/aggregator/fit_imaging_ci.py` & `autocti-2023.7.7.3/autocti/aggregator/fit_imaging_ci.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/aggregator/imaging_ci.py` & `autocti-2023.7.7.3/autocti/aggregator/imaging_ci.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/ci_util.py` & `autocti-2023.7.7.3/autocti/charge_injection/ci_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/fit.py` & `autocti-2023.7.7.3/autocti/charge_injection/fit.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/hyper.py` & `autocti-2023.7.7.3/autocti/charge_injection/hyper.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/imaging/imaging.py` & `autocti-2023.7.7.3/autocti/charge_injection/imaging/imaging.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,28 +88,14 @@
 
         return [
             np.ma.median(masked_image[region.y0 : region.y1, column_index])
             for region in self.region_list
             for column_index in range(region.x0, region.x1)
         ]
 
-    @property
-    def pre_cti_data_residual_map(self) -> aa.Array2D:
-        """
-        The residuals of the data and the pre CTI data.
-
-        This is used to assess whether the pre CTI data has been estimated accurately (e.g. from the FPR of the
-        data) and includes e specific set of visualization functions.
-
-        Returns
-        -------
-        The residual map of the data and pre CTI data.
-        """
-        return self.data - self.pre_cti_data
-
     def apply_mask(self, mask: mask_2d.Mask2D) -> "ImagingCI":
         image = aa.Array2D(values=self.image.native, mask=mask)
         noise_map = aa.Array2D(values=self.noise_map.native, mask=mask)
 
         if self.cosmic_ray_map is not None:
             cosmic_ray_map = aa.Array2D(values=self.cosmic_ray_map.native, mask=mask)
```

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/imaging/settings.py` & `autocti-2023.7.7.3/autocti/charge_injection/imaging/settings.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/imaging/simulator.py` & `autocti-2023.7.7.3/autocti/charge_injection/imaging/simulator.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/layout.py` & `autocti-2023.7.7.3/autocti/charge_injection/layout.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/master.py` & `autocti-2023.7.7.3/autocti/charge_injection/master.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/mock/mock_result.py` & `autocti-2023.7.7.3/autocti/charge_injection/mock/mock_result.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/model/analysis.py` & `autocti-2023.7.7.3/autocti/charge_injection/model/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,32 +262,28 @@
             region_list += ["fpr_non_uniformity"]
 
         dataset_list = [analysis.dataset for analysis in analyses]
 
         visualizer.visualize_dataset_combined(
             dataset_list=dataset_list,
         )
-
         visualizer.visualize_dataset_regions_combined(
             dataset_list=dataset_list,
             region_list=region_list,
         )
         if self.dataset_full is not None:
             dataset_full_list = [analysis.dataset_full for analysis in analyses]
 
             visualizer.visualize_dataset_combined(
-                dataset_list=dataset_full_list,
-                folder_suffix="_full",
-                filename_suffix="_full",
+                dataset_list=dataset_full_list, folder_suffix="_full"
             )
             visualizer.visualize_dataset_regions_combined(
                 dataset_list=dataset_full_list,
                 region_list=region_list,
                 folder_suffix="_full",
-                filename_suffix="_full",
             )
 
     def visualize(
         self,
         paths: af.DirectoryPaths,
         instance: af.ModelInstance,
         during_analysis: bool,
```

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/model/result.py` & `autocti-2023.7.7.3/autocti/charge_injection/model/result.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/model/visualizer.py` & `autocti-2023.7.7.3/autocti/charge_injection/model/visualizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
 
 class VisualizerImagingCI(Visualizer):
     def visualize_dataset(self, dataset, folder_suffix: str = ""):
         def should_plot(name):
             return plot_setting(section="dataset", name=name)
 
-        mat_plot = self.mat_plot_2d_from(subfolders=f"dataset{folder_suffix}")
+        mat_plot_2d = self.mat_plot_2d_from(subfolders=f"dataset{folder_suffix}")
 
         dataset_plotter = aplt.ImagingCIPlotter(
-            dataset=dataset, mat_plot_2d=mat_plot, include_2d=self.include_2d
+            dataset=dataset, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
         )
 
         if should_plot("subplot_dataset"):
             dataset_plotter.subplot_dataset()
 
         dataset_plotter.figures_2d(
             data=should_plot("data"),
@@ -36,18 +36,18 @@
             cosmic_ray_map=should_plot("cosmic_ray_map"),
         )
 
     def visualize_dataset_regions(self, dataset, region_list, folder_suffix: str = ""):
         def should_plot(name):
             return plot_setting(section="dataset", name=name)
 
-        mat_plot = self.mat_plot_1d_from(subfolders=f"dataset{folder_suffix}")
+        mat_plot_1d = self.mat_plot_1d_from(subfolders=f"dataset{folder_suffix}")
 
         dataset_plotter = aplt.ImagingCIPlotter(
-            dataset=dataset, mat_plot_1d=mat_plot, include_2d=self.include_2d
+            dataset=dataset, mat_plot_1d=mat_plot_1d, include_2d=self.include_2d
         )
 
         for region in region_list:
             try:
                 if should_plot("subplot_dataset"):
                     dataset_plotter.subplot_1d(region=region)
 
@@ -61,68 +61,35 @@
                 )
 
             except (exc.RegionException, TypeError, ValueError):
                 logger.info(
                     f"VISUALIZATION - Could not visualize the ImagingCI 1D {region}"
                 )
 
-    def visualize_dataset_combined(
-        self, dataset_list, folder_suffix: str = "", filename_suffix: str = ""
-    ):
+    def visualize_dataset_combined(self, dataset_list, folder_suffix: str = ""):
         def should_plot(name):
             return plot_setting(section="dataset", name=name)
 
-        mat_plot = self.mat_plot_2d_from(subfolders=f"dataset_combined{folder_suffix}")
+        mat_plot_2d = self.mat_plot_2d_from(
+            subfolders=f"dataset_combined{folder_suffix}"
+        )
 
         dataset_plotter_list = [
             aplt.ImagingCIPlotter(
-                dataset=dataset, mat_plot_2d=mat_plot, include_2d=self.include_2d
+                dataset=dataset, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
             )
             for dataset in dataset_list
         ]
         multi_plotter = aplt.MultiFigurePlotter(plotter_list=dataset_plotter_list)
 
         if should_plot("subplot_dataset"):
-            multi_plotter.subplot_of_figure(
-                func_name="figures_2d",
-                figure_name="data",
-                filename_suffix=filename_suffix,
-            )
-            multi_plotter.subplot_of_figure(
-                func_name="figures_2d",
-                figure_name="noise_map",
-                filename_suffix=filename_suffix,
-            )
-            multi_plotter.subplot_of_figure(
-                func_name="figures_2d",
-                figure_name="signal_to_noise_map",
-                filename_suffix=filename_suffix,
-            )
-            multi_plotter.subplot_of_figure(
-                func_name="figures_2d",
-                figure_name="pre_cti_data",
-                filename_suffix=filename_suffix,
-            )
-            multi_plotter.subplot_of_figure(
-                func_name="figures_2d",
-                figure_name="pre_cti_data_residual_map",
-                filename_suffix=filename_suffix,
-            )
-            multi_plotter.subplot_of_figure(
-                func_name="figures_2d",
-                figure_name="cosmic_ray_map",
-                filename_suffix=filename_suffix,
-            )
+            multi_plotter.subplot_of_figure(func_name="figures_2d", figure_name="data")
 
     def visualize_dataset_regions_combined(
-        self,
-        dataset_list,
-        region_list,
-        folder_suffix: str = "",
-        filename_suffix: str = "",
+        self, dataset_list, region_list, folder_suffix: str = ""
     ):
         def should_plot(name):
             return plot_setting(section="dataset", name=name)
 
         mat_plot_1d = self.mat_plot_1d_from(
             subfolders=f"dataset_combined{folder_suffix}"
         )
@@ -138,38 +105,38 @@
         for region in region_list:
             try:
                 if should_plot("data"):
                     multi_plotter.subplot_of_figure(
                         func_name="figures_1d",
                         figure_name="data",
                         region=region,
-                        filename_suffix=f"{filename_suffix}_{region}",
+                        filename_suffix=f"_{region}",
                     )
 
                 if should_plot("data_logy"):
                     multi_plotter.subplot_of_figure(
                         func_name="figures_1d",
                         figure_name="data_logy",
                         region=region,
-                        filename_suffix=f"{filename_suffix}_{region}",
+                        filename_suffix=f"_{region}",
                     )
 
             except (exc.RegionException, TypeError, ValueError):
                 logger.info(
                     f"VISUALIZATION - Could not visualize the ImagingCI 1D {region}"
                 )
 
     def visualize_fit(self, fit, during_analysis, folder_suffix: str = ""):
         def should_plot(name):
             return plot_setting(section="fit", name=name)
 
-        mat_plot = self.mat_plot_2d_from(subfolders=f"fit_dataset{folder_suffix}")
+        mat_plot_2d = self.mat_plot_2d_from(subfolders=f"fit_dataset{folder_suffix}")
 
         fit_plotter = aplt.FitImagingCIPlotter(
-            fit=fit, mat_plot_2d=mat_plot, include_2d=self.include_2d
+            fit=fit, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
         )
 
         fit_plotter.figures_2d(
             data=should_plot("data"),
             noise_map=should_plot("noise_map"),
             signal_to_noise_map=should_plot("signal_to_noise_map"),
             pre_cti_data=should_plot("pre_cti_data"),
@@ -200,18 +167,18 @@
 
     def visualize_fit_1d_regions(
         self, fit, region_list, during_analysis, folder_suffix: str = ""
     ):
         def should_plot(name):
             return plot_setting(section="fit", name=name)
 
-        mat_plot = self.mat_plot_1d_from(subfolders=f"fit_dataset{folder_suffix}")
+        mat_plot_1d = self.mat_plot_1d_from(subfolders=f"fit_dataset{folder_suffix}")
 
         fit_plotter = aplt.FitImagingCIPlotter(
-            fit=fit, mat_plot_1d=mat_plot, include_1d=self.include_1d
+            fit=fit, mat_plot_1d=mat_plot_1d, include_1d=self.include_1d
         )
 
         for region in region_list:
             try:
                 if should_plot("subplot_fit"):
                     fit_plotter.subplot_1d(region=region)
 
@@ -251,21 +218,21 @@
 
     def visualize_fit_combined(
         self, fit_list, during_analysis, folder_suffix: str = ""
     ):
         def should_plot(name):
             return plot_setting(section="fit", name=name)
 
-        mat_plot = self.mat_plot_2d_from(
+        mat_plot_2d = self.mat_plot_2d_from(
             subfolders=f"fit_dataset_combined{folder_suffix}"
         )
 
         fit_plotter_list = [
             aplt.FitImagingCIPlotter(
-                fit=fit, mat_plot_2d=mat_plot, include_2d=self.include_2d
+                fit=fit, mat_plot_2d=mat_plot_2d, include_2d=self.include_2d
             )
             for fit in fit_list
         ]
         multi_plotter = aplt.MultiFigurePlotter(plotter_list=fit_plotter_list)
 
         if should_plot("residual_map"):
             multi_plotter.subplot_of_figure(
@@ -284,21 +251,21 @@
 
     def visualize_fit_1d_regions_combined(
         self, fit_list, region_list, during_analysis, folder_suffix: str = ""
     ):
         def should_plot(name):
             return plot_setting(section="fit", name=name)
 
-        mat_plot = self.mat_plot_1d_from(
+        mat_plot_1d = self.mat_plot_1d_from(
             subfolders=f"fit_dataset_combined{folder_suffix}"
         )
 
         fit_plotter_list = [
             aplt.FitImagingCIPlotter(
-                fit=fit, mat_plot_1d=mat_plot, include_1d=self.include_1d
+                fit=fit, mat_plot_1d=mat_plot_1d, include_1d=self.include_1d
             )
             for fit in fit_list
         ]
         multi_plotter = aplt.MultiFigurePlotter(plotter_list=fit_plotter_list)
 
         for region in region_list:
             try:
```

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/ou_sim_ci.py` & `autocti-2023.7.7.3/autocti/charge_injection/ou_sim_ci.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/plot/fit_ci_plotters.py` & `autocti-2023.7.7.3/autocti/charge_injection/plot/fit_ci_plotters.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,17 @@
             chi_squared_map=chi_squared_map,
         )
 
         if pre_cti_data:
             self.mat_plot_2d.plot_array(
                 array=self.fit.pre_cti_data,
                 visuals_2d=self.get_visuals_2d(),
-                auto_labels=AutoLabels(title="Pre CTI Data", filename="pre_cti_data"),
+                auto_labels=AutoLabels(
+                    title="CI Pre CTI Image", filename="pre_cti_data"
+                ),
             )
 
         if post_cti_data:
             self.mat_plot_2d.plot_array(
                 array=self.fit.post_cti_data,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=AutoLabels(
```

### Comparing `autocti-2023.6.12.4/autocti/charge_injection/plot/imaging_ci_plotters.py` & `autocti-2023.7.7.3/autocti/charge_injection/plot/imaging_ci_plotters.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 
     def figures_2d(
         self,
         data: bool = False,
         noise_map: bool = False,
         signal_to_noise_map: bool = False,
         pre_cti_data: bool = False,
-        pre_cti_data_residual_map: bool = False,
         cosmic_ray_map: bool = False,
     ):
         """
         Plots the individual attributes of the plotter's `ImagingCI` object in 2D.
 
         The API is such that every plottable attribute of the `Imaging` object is an input parameter of type bool of
         the function, which if switched to `True` means that it is plotted.
@@ -103,54 +102,39 @@
             Whether to make a 2D plot (via `imshow`) of the image data.
         noise_map
             Whether to make a 2D plot (via `imshow`) of the noise map.
         signal_to_noise_map
             Whether to make a 2D plot (via `imshow`) of the signal-to-noise map.
         pre_cti_data
             Whether to make a 2D plot (via `imshow`) of the pre-cti data.
-        pre_cti_data_residual_map
-            Whether to make a 2D plot (via `imshow`) of the pre-cti data residual-map.
         cosmic_ray_map
             Whether to make a 2D plot (via `imshow`) of the cosmic ray map.
         """
 
-        title_str = self.title_str_2d_from()
-
         self._imaging_meta_plotter.figures_2d(
             data=data,
             noise_map=noise_map,
             signal_to_noise_map=signal_to_noise_map,
-            title_str=title_str,
         )
 
         if pre_cti_data:
             self.mat_plot_2d.plot_array(
                 array=self.dataset.pre_cti_data,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=AutoLabels(
-                    title=title_str or f"Pre CTI Data", filename="pre_cti_data"
-                ),
-            )
-
-        if pre_cti_data_residual_map:
-            self.mat_plot_2d.plot_array(
-                array=self.dataset.pre_cti_data_residual_map,
-                visuals_2d=self.get_visuals_2d(),
-                auto_labels=AutoLabels(
-                    title=title_str or f"Pre CTI Data Residual Map",
-                    filename="pre_cti_data_residual_map",
+                    title="CI Pre CTI Image", filename="pre_cti_data"
                 ),
             )
 
         if cosmic_ray_map:
             self.mat_plot_2d.plot_array(
                 array=self.dataset.cosmic_ray_map,
                 visuals_2d=self.get_visuals_2d(),
                 auto_labels=AutoLabels(
-                    title=title_str or f"Cosmic Ray Map", filename="cosmic_ray_map"
+                    title="Cosmic Ray Map", filename="cosmic_ray_map"
                 ),
             )
 
     def figures_1d(
         self,
         region: str,
         data: bool = False,
```

### Comparing `autocti-2023.6.12.4/autocti/clocker/abstract.py` & `autocti-2023.7.7.3/autocti/clocker/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/clocker/one_d.py` & `autocti-2023.7.7.3/autocti/clocker/one_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/clocker/two_d.py` & `autocti-2023.7.7.3/autocti/clocker/two_d.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,14 +260,15 @@
                 serial_time_stop=self.serial_time_stop,
                 serial_prune_n_electrons=self.serial_prune_n_electrons,
                 serial_prune_frequency=self.serial_prune_frequency,
                 pixel_bounce=self.pixel_bounce,
                 verbosity=self.verbosity,
             )
 
+
         try:
             return aa.Array2D(
                 values=image_post_cti, mask=data.mask, store_native=True, skip_mask=True
             )
         except AttributeError:
             return image_post_cti
```

### Comparing `autocti-2023.6.12.4/autocti/config/notation.yaml` & `autocti-2023.7.7.3/autocti/config/notation.yaml`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/config/priors/ccd.yaml` & `autocti-2023.7.7.3/autocti/config/priors/ccd.yaml`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/config/priors/traps.yaml` & `autocti-2023.7.7.3/autocti/config/priors/traps.yaml`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/cosmics/cosmics.py` & `autocti-2023.7.7.3/autocti/cosmics/cosmics.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/cosmics/cr_distances.py` & `autocti-2023.7.7.3/autocti/cosmics/cr_distances.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/cosmics/cr_lengths.py` & `autocti-2023.7.7.3/autocti/cosmics/cr_lengths.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/dataset_1d/dataset_1d.py` & `autocti-2023.7.7.3/autocti/dataset_1d/dataset_1d/dataset_1d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/dataset_1d/simulator.py` & `autocti-2023.7.7.3/autocti/dataset_1d/dataset_1d/simulator.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/fit.py` & `autocti-2023.7.7.3/autocti/dataset_1d/fit.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/model/analysis.py` & `autocti-2023.7.7.3/autocti/dataset_1d/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/model/visualizer.py` & `autocti-2023.7.7.3/autocti/dataset_1d/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/plot/dataset_1d_plotters.py` & `autocti-2023.7.7.3/autocti/dataset_1d/plot/dataset_1d_plotters.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/dataset_1d/plot/fit_plotters.py` & `autocti-2023.7.7.3/autocti/dataset_1d/plot/fit_plotters.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
             y = self.extract_region_from(array=self.fit.pre_cti_data, region=region)
 
             self.mat_plot_1d.plot_yx(
                 y=y,
                 x=range(len(y)),
                 visuals_1d=self.get_visuals_1d(),
                 auto_labels=AutoLabels(
-                    title="Pre CTI Data",
+                    title="CI Pre CTI Image",
                     yunit="e-",
                     filename=f"pre_cti_data{suffix}",
                 ),
             )
 
         if post_cti_data:
             y = self.extract_region_from(array=self.fit.post_cti_data, region=region)
```

### Comparing `autocti-2023.6.12.4/autocti/exc.py` & `autocti-2023.7.7.3/autocti/exc.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/one_d/abstract.py` & `autocti-2023.7.7.3/autocti/extract/one_d/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/one_d/eper.py` & `autocti-2023.7.7.3/autocti/extract/one_d/eper.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/one_d/fpr.py` & `autocti-2023.7.7.3/autocti/extract/one_d/fpr.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/one_d/master.py` & `autocti-2023.7.7.3/autocti/extract/one_d/master.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/one_d/overscan.py` & `autocti-2023.7.7.3/autocti/extract/one_d/overscan.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/settings.py` & `autocti-2023.7.7.3/autocti/extract/settings.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/abstract.py` & `autocti-2023.7.7.3/autocti/extract/two_d/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/extract_2d_util.py` & `autocti-2023.7.7.3/autocti/extract/two_d/extract_2d_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/master.py` & `autocti-2023.7.7.3/autocti/extract/two_d/master.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/parallel/abstract.py` & `autocti-2023.7.7.3/autocti/extract/two_d/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/parallel/calibration.py` & `autocti-2023.7.7.3/autocti/extract/two_d/parallel/calibration.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/parallel/eper.py` & `autocti-2023.7.7.3/autocti/extract/two_d/parallel/eper.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/parallel/fpr.py` & `autocti-2023.7.7.3/autocti/extract/two_d/parallel/fpr.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/parallel/overscan.py` & `autocti-2023.7.7.3/autocti/extract/two_d/parallel/overscan.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/parallel/pedestal.py` & `autocti-2023.7.7.3/autocti/extract/two_d/parallel/pedestal.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/abstract.py` & `autocti-2023.7.7.3/autocti/extract/two_d/serial/abstract.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/calibration.py` & `autocti-2023.7.7.3/autocti/extract/two_d/serial/calibration.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/eper.py` & `autocti-2023.7.7.3/autocti/extract/two_d/serial/eper.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/fpr.py` & `autocti-2023.7.7.3/autocti/extract/two_d/serial/fpr.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/overscan.py` & `autocti-2023.7.7.3/autocti/extract/two_d/serial/overscan.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/overscan_no_eper.py` & `autocti-2023.7.7.3/autocti/extract/two_d/serial/overscan_no_eper.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/extract/two_d/serial/prescan.py` & `autocti-2023.7.7.3/autocti/extract/two_d/serial/prescan.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/fixtures.py` & `autocti-2023.7.7.3/autocti/fixtures.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/acs/acs_util.py` & `autocti-2023.7.7.3/autocti/instruments/acs/acs_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/acs/array_2d.py` & `autocti-2023.7.7.3/autocti/instruments/acs/array_2d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/acs/header.py` & `autocti-2023.7.7.3/autocti/instruments/acs/header.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/acs/image.py` & `autocti-2023.7.7.3/autocti/instruments/acs/image.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/acs/layout.py` & `autocti-2023.7.7.3/autocti/instruments/acs/layout.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/euclid/array_2d.py` & `autocti-2023.7.7.3/autocti/instruments/euclid/array_2d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/euclid/euclid_util.py` & `autocti-2023.7.7.3/autocti/instruments/euclid/euclid_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/euclid/header.py` & `autocti-2023.7.7.3/autocti/instruments/euclid/header.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/instruments/euclid/layout.py` & `autocti-2023.7.7.3/autocti/instruments/euclid/layout.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/layout/one_d.py` & `autocti-2023.7.7.3/autocti/layout/one_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/layout/two_d.py` & `autocti-2023.7.7.3/autocti/layout/two_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/mask/mask_1d.py` & `autocti-2023.7.7.3/autocti/mask/mask_1d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/mask/mask_2d.py` & `autocti-2023.7.7.3/autocti/mask/mask_2d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/model/model_util.py` & `autocti-2023.7.7.3/autocti/model/model_util.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/model/result.py` & `autocti-2023.7.7.3/autocti/model/result.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/model/settings.py` & `autocti-2023.7.7.3/autocti/model/settings.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/model/visualizer.py` & `autocti-2023.7.7.3/autocti/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/plot/__init__.py` & `autocti-2023.7.7.3/autocti/plot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,13 @@
 from autoarray.plot.mat_plot.two_d import MatPlot2D
 from autoarray.plot.include.two_d import Include2D
 from autoarray.plot.visuals.two_d import Visuals2D
 
 from autoarray.structures.plot.structure_plotters import YX1DPlotter
 from autoarray.structures.plot.structure_plotters import YX1DPlotter as Array1DPlotter
 from autoarray.structures.plot.structure_plotters import Array2DPlotter
-
 from autoarray.plot.multi_plotters import MultiFigurePlotter
-from autoarray.plot.multi_plotters import MultiYX1DPlotter
 
 from autocti.dataset_1d.plot.dataset_1d_plotters import Dataset1DPlotter
 from autocti.dataset_1d.plot.fit_plotters import FitDataset1DPlotter
 from autocti.charge_injection.plot.imaging_ci_plotters import ImagingCIPlotter
 from autocti.charge_injection.plot.fit_ci_plotters import FitImagingCIPlotter
```

### Comparing `autocti-2023.6.12.4/autocti/plot/abstract_plotters.py` & `autocti-2023.7.7.3/autocti/plot/abstract_plotters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Optional
-
 from autoarray.plot.wrap.base.abstract import set_backend
 
 set_backend()
 
 import autoarray.plot as aplt
 
 from autoarray.plot.abstract_plotters import AbstractPlotter
@@ -38,15 +36,15 @@
     def get_1d(self):
         return GetVisuals1D(visuals=self.visuals_1d, include=self.include_1d)
 
     @property
     def get_2d(self):
         return GetVisuals2D(visuals=self.visuals_2d, include=self.include_2d)
 
-    def title_str_from(self, region: Optional[str]) -> str:
+    def title_str_from(self, region: str) -> str:
         if self.dataset.settings_dict is not None:
             ccd_str = self.dataset.settings_dict.get("CCD")
         else:
             ccd_str = None
 
         if region is None:
             title_str = ""
@@ -63,23 +61,14 @@
         elif region == "serial_eper":
             title_str = "Serial EPER"
 
         if ccd_str is None:
             return title_str
         return f"{ccd_str} {title_str}"
 
-    def title_str_2d_from(self) -> Optional[str]:
-        if self.dataset.settings_dict is not None:
-            ccd_str = self.dataset.settings_dict.get("CCD")
-            ig1_str = self.dataset.settings_dict.get("CI_IG1")
-            ig2_str = self.dataset.settings_dict.get("CI_IG2")
-            id_delay_str = self.dataset.settings_dict.get("CI_IDDLY")
-
-            return f"{ccd_str} IG1={ig1_str} IG2={ig2_str} IDD={id_delay_str}"
-
     def text_manual_dict_from(self, region: str):
         try:
             fpr_value = self.dataset.fpr_value
         except AttributeError:
             fpr_value = None
 
         text_manual_dict = {}
```

### Comparing `autocti-2023.6.12.4/autocti/plot/get_visuals/one_d.py` & `autocti-2023.7.7.3/autocti/plot/get_visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/plot/get_visuals/two_d.py` & `autocti-2023.7.7.3/autocti/plot/get_visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/preloads.py` & `autocti-2023.7.7.3/autocti/preloads.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/autocti/util/__init__.py` & `autocti-2023.7.7.3/autocti/util/__init__.py`

 * *Files identical despite different names*

### Comparing `autocti-2023.6.12.4/setup.py` & `autocti-2023.7.7.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "1.0.dev0")
+version = environ.get("VERSION", "2023.7.7.3")
 requirements.extend(
-    [f"autoconf=={version}", f"autofit=={version}", f"autoarray=={version}"]
+    [f"autoconf==2023.7.7.2", f"autofit==2023.7.7.2", f"autoarray==2023.7.7.2"]
 )
 
 setup(
     name="autocti",
     version=version,
     description="PyAutoCTI: Charge Transfer Inefficiency Modeling",
     long_description=long_description,
```

