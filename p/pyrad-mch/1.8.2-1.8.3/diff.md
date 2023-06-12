# Comparing `tmp/pyrad_mch-1.8.2.tar.gz` & `tmp/pyrad_mch-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrad_mch-1.8.2.tar", last modified: Thu Jun  8 11:10:35 2023, max compression
+gzip compressed data, was "pyrad_mch-1.8.3.tar", last modified: Mon Jun 12 12:48:40 2023, max compression
```

## Comparing `pyrad_mch-1.8.2.tar` & `pyrad_mch-1.8.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:10:35.889331 pyrad_mch-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-08 11:10:35.889331 pyrad_mch-1.8.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:10:35.877331 pyrad_mch-1.8.2/pyrad/
--rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:10:35.877331 pyrad_mch-1.8.2/pyrad/flow/
--rwxr-xr-x   0 runner    (1001) docker     (123)      386 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/flow/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57500 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/flow/flow_aux.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35108 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/flow/flow_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:10:35.881331 pyrad_mch-1.8.2/pyrad/graph/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3205 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/graph/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54994 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/graph/plots.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13147 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/graph/plots_aux.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44989 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/graph/plots_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    52389 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/graph/plots_spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24330 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/graph/plots_timeseries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    70743 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/graph/plots_vol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:10:35.881331 pyrad_mch-1.8.2/pyrad/io/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7748 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9281 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   112893 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/io_aux.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3936 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/mxpol_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15513 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/read_data_cosmo.py
--rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/read_data_dem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9542 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/read_data_hzt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/read_data_iso0_mf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37831 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/read_data_mxpol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57335 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/read_data_other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   185643 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/read_data_radar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    78210 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/read_data_sensor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15042 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/read_data_sun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7684 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/trajectory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    97871 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/io/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:10:35.885331 pyrad_mch-1.8.2/pyrad/proc/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11666 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_Doppler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    93122 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_aux.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    92202 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_calib.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38434 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_cosmo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_dem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    94520 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_echoclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    59766 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    89471 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_intercomp.py
--rw-r--r--   0 runner    (1001) docker     (123)    26560 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_iq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    62664 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_monitoring.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44326 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_phase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58764 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)    66245 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)    47217 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_timeseries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    72382 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/proc/process_traj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:10:35.885331 pyrad_mch-1.8.2/pyrad/prod/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/prod/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38966 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/prod/process_grid_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13183 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/prod/process_intercomp_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31042 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/prod/process_monitoring_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    56567 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/prod/process_product.py
--rw-r--r--   0 runner    (1001) docker     (123)    47103 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/prod/process_spectra_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30674 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/prod/process_timeseries_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5606 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/prod/process_traj_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   154891 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/prod/process_vol_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4392 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/prod/product_aux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:10:35.889331 pyrad_mch-1.8.2/pyrad/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    61246 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/util/radar_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4908 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/pyrad/util/stat_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-08 11:10:35.000000 pyrad_mch-1.8.2/pyrad/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:10:35.889331 pyrad_mch-1.8.2/pyrad_mch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-08 11:10:35.000000 pyrad_mch-1.8.2/pyrad_mch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-08 11:10:35.000000 pyrad_mch-1.8.2/pyrad_mch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:10:35.000000 pyrad_mch-1.8.2/pyrad_mch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:10:35.000000 pyrad_mch-1.8.2/pyrad_mch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 11:10:35.000000 pyrad_mch-1.8.2/pyrad_mch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:10:35.889331 pyrad_mch-1.8.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5799 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/scripts/common_colocated_gates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4556 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/scripts/main_precipitation_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/scripts/main_process_cosmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/scripts/main_process_cosmo_rt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/scripts/main_process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/scripts/main_process_data_birds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6393 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/scripts/main_process_data_period.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4622 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/scripts/main_process_data_rt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16283 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/scripts/main_process_data_trt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/scripts/main_process_euclid_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5965 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/scripts/main_process_gecsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/scripts/movie_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/scripts/rewrite_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:10:35.889331 pyrad_mch-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-08 11:10:17.000000 pyrad_mch-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:48:40.441561 pyrad_mch-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-12 12:48:40.441561 pyrad_mch-1.8.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:48:40.429560 pyrad_mch-1.8.3/pyrad/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:48:40.429560 pyrad_mch-1.8.3/pyrad/flow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      386 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/flow/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57799 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/flow/flow_aux.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35108 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/flow/flow_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:48:40.429560 pyrad_mch-1.8.3/pyrad/graph/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3205 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/graph/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54994 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/graph/plots.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13147 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/graph/plots_aux.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44989 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/graph/plots_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52389 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/graph/plots_spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24330 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/graph/plots_timeseries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    70743 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/graph/plots_vol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:48:40.433561 pyrad_mch-1.8.3/pyrad/io/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7748 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9281 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113754 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/io_aux.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3936 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/mxpol_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15513 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/read_data_cosmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/read_data_dem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9542 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/read_data_hzt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/read_data_iso0_mf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37831 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/read_data_mxpol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57335 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/read_data_other.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   186635 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/read_data_radar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    78210 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/read_data_sensor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15042 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/read_data_sun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7684 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/trajectory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    97871 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/io/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:48:40.437561 pyrad_mch-1.8.3/pyrad/proc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11666 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_Doppler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    93122 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_aux.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    92202 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_calib.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38434 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_cosmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_dem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    94520 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_echoclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59766 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    89479 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_intercomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26560 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_iq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    62624 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_monitoring.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44326 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_phase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58764 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66245 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47217 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_timeseries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    72382 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/proc/process_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:48:40.437561 pyrad_mch-1.8.3/pyrad/prod/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/prod/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38966 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/prod/process_grid_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13183 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/prod/process_intercomp_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31042 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/prod/process_monitoring_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56567 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/prod/process_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47103 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/prod/process_spectra_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30674 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/prod/process_timeseries_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5606 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/prod/process_traj_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   154891 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/prod/process_vol_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4392 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/prod/product_aux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:48:40.437561 pyrad_mch-1.8.3/pyrad/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61246 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/util/radar_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4908 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/pyrad/util/stat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-12 12:48:40.000000 pyrad_mch-1.8.3/pyrad/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:48:40.441561 pyrad_mch-1.8.3/pyrad_mch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-12 12:48:40.000000 pyrad_mch-1.8.3/pyrad_mch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-12 12:48:40.000000 pyrad_mch-1.8.3/pyrad_mch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:48:40.000000 pyrad_mch-1.8.3/pyrad_mch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:48:40.000000 pyrad_mch-1.8.3/pyrad_mch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 12:48:40.000000 pyrad_mch-1.8.3/pyrad_mch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:48:40.441561 pyrad_mch-1.8.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5799 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/scripts/common_colocated_gates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4556 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/scripts/main_precipitation_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/scripts/main_process_cosmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/scripts/main_process_cosmo_rt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/scripts/main_process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/scripts/main_process_data_birds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6393 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/scripts/main_process_data_period.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4622 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/scripts/main_process_data_rt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16283 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/scripts/main_process_data_trt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/scripts/main_process_euclid_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5965 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/scripts/main_process_gecsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/scripts/movie_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/scripts/rewrite_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:48:40.441561 pyrad_mch-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-12 12:48:29.000000 pyrad_mch-1.8.3/setup.py
```

### Comparing `pyrad_mch-1.8.2/PKG-INFO` & `pyrad_mch-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrad_mch
-Version: 1.8.2
+Version: 1.8.3
 Summary:  Python Radar Toolkit
 Home-page: https://github.com/MeteoSwiss/pyrad.git
 Author: MeteoSwiss Pyrad Developers
 Author-email: daniel.wolfensberger@meteoswiss.ch
 Maintainer: MeteoSwiss Pyrad Developers
 Maintainer-email: daniel.wolfensberger@meteoswiss.ch
 License: BSD
```

### Comparing `pyrad_mch-1.8.2/pyrad/__init__.py` & `pyrad_mch-1.8.3/pyrad/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/flow/flow_aux.py` & `pyrad_mch-1.8.3/pyrad/flow/flow_aux.py`

 * *Files 2% similar despite different names*

```diff
@@ -983,14 +983,18 @@
         cfg.update({'solarfluxpath': None})
     if 'selfconsistencypath' not in cfg:
         cfg.update({'selfconsistencypath': None})
     if 'loadbasepath' not in cfg:
         cfg.update({'loadbasepath': None})
     if 'loadname' not in cfg:
         cfg.update({'loadname': None})
+    if 'gecsxbasepath' not in cfg:
+        cfg.update({'gecsxbasepath': None})
+    if 'gecsxname' not in cfg:
+        cfg.update({'gecsxname': None})
     if 'RadarName' not in cfg:
         cfg.update({'RadarName': None})
     if 'RadarRes' not in cfg:
         cfg.update({'RadarRes': None})
     if 'metranet_read_lib' not in cfg:
         cfg.update({'metranet_read_lib': 'C'})
     if 'ScanPeriod' not in cfg:
@@ -1027,20 +1031,20 @@
             'ltxh': 0.*np.ones(cfg['NumRadars'], dtype=np.float32)})
     if 'ltxv' not in cfg:
         cfg.update({
             'ltxv': 0.*np.ones(cfg['NumRadars'], dtype=np.float32)})
 
     # Convert the following strings to string arrays
     strarr_list = [
-        'datapath', 'cosmopath', 'dempath', 'loadbasepath', 'psrpath',
-        'iqpath', 'satpath', 'loadname', 'RadarName', 'RadarRes', 'ScanList',
-        'imgformat', 'frequency', 'radar_beam_width_h', 'radar_beam_width_v',
-        'pulse_width', 'nyquist_velocity', 'AntennaGainH', 'AntennaGainV',
-        'dBADUtodBmh', 'dBADUtodBmv', 'mflossh', 'mflossv', 'radconsth',
-        'radconstv', 'txpwrh', 'txpwrv', 'attg', 'path_convention']
+        'datapath', 'cosmopath', 'dempath', 'gecsxbasepath', 'gecsxname',
+        'loadbasepath', 'psrpath','iqpath', 'satpath', 'loadname', 'RadarName',
+        'RadarRes', 'ScanList','imgformat', 'frequency', 'radar_beam_width_h', 
+        'radar_beam_width_v','pulse_width', 'nyquist_velocity', 'AntennaGainH', 
+        'AntennaGainV', 'dBADUtodBmh', 'dBADUtodBmv', 'mflossh', 'mflossv',
+        'radconsth', 'radconstv', 'txpwrh', 'txpwrv', 'attg', 'path_convention']
     for param in strarr_list:
         if param in cfg and isinstance(cfg[param], str):
             cfg[param] = [cfg[param]]
 
     # Convert the following floats to float arrays
     fltarr_list = [
         'frequency', 'radar_beam_width_h', 'radar_beam_width_v',
@@ -1128,15 +1132,14 @@
         if 'datatype' not in cfg['BinFileParams']:
             warn('BinFileParams: datatype not specified. Assumed Raccu')
             cfg['BinFileParams'].update({'datatype': 'Raccu'})
 
         if isinstance(cfg['BinFileParams']['datatype'], str):
             cfg['BinFileParams']['datatype'] = [
                 cfg['BinFileParams']['datatype']]
-
     return cfg
 
 
 @profiler(level=3)
 def _create_datacfg_dict(cfg):
     """
     creates a data configuration dictionary from a config dictionary
@@ -1161,14 +1164,16 @@
     datacfg.update({'MasterScanTimeTol': cfg['MasterScanTimeTol']})
     datacfg.update({'TimeTol': cfg['TimeTol']})
     datacfg.update({'NumRadars': cfg['NumRadars']})
     datacfg.update({'cosmopath': cfg['cosmopath']})
     datacfg.update({'dempath': cfg['dempath']})
     datacfg.update({'loadbasepath': cfg['loadbasepath']})
     datacfg.update({'loadname': cfg['loadname']})
+    datacfg.update({'gecsxbasepath': cfg['gecsxbasepath']})
+    datacfg.update({'gecsxname': cfg['gecsxname']})
     datacfg.update({'RadarName': cfg['RadarName']})
     datacfg.update({'RadarRes': cfg['RadarRes']})
     datacfg.update({'ScanPeriod': cfg['ScanPeriod']})
     datacfg.update({'CosmoRunFreq': int(cfg['CosmoRunFreq'])})
     datacfg.update({'CosmoForecasted': int(cfg['CosmoForecasted'])})
     datacfg.update({'path_convention': cfg['path_convention']})
     datacfg.update({'metranet_read_lib': cfg['metranet_read_lib']})
@@ -1538,15 +1543,15 @@
     masterdatatypedescr = None
     masterscan = None
     for datatypedescr in datatypesdescr:
         radarnr, datagroup, _, _, _ = get_datatype_fields(datatypedescr)
         if (datagroup not in (
                 'COSMO', 'RAD4ALPCOSMO', 'CFRADIALCOSMO', 'DEM', 'RAD4ALPDEM',
                 'RAD4ALPHYDRO', 'RAD4ALPDOPPLER', 'RAD4ALPIQ', 'PSR',
-                'PSRSPECTRA')):
+                'PSRSPECTRA', 'GECSX')):
             masterdatatypedescr = datatypedescr
             if scan_list is not None:
                 masterscan = scan_list[int(radarnr[5:8])-1][0]
             break
 
     # if data type is not radar use dBZ as reference
     if masterdatatypedescr is None:
```

### Comparing `pyrad_mch-1.8.2/pyrad/flow/flow_control.py` & `pyrad_mch-1.8.3/pyrad/flow/flow_control.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/graph/__init__.py` & `pyrad_mch-1.8.3/pyrad/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/graph/plots.py` & `pyrad_mch-1.8.3/pyrad/graph/plots.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/graph/plots_aux.py` & `pyrad_mch-1.8.3/pyrad/graph/plots_aux.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/graph/plots_grid.py` & `pyrad_mch-1.8.3/pyrad/graph/plots_grid.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/graph/plots_spectra.py` & `pyrad_mch-1.8.3/pyrad/graph/plots_spectra.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/graph/plots_timeseries.py` & `pyrad_mch-1.8.3/pyrad/graph/plots_timeseries.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/graph/plots_vol.py` & `pyrad_mch-1.8.3/pyrad/graph/plots_vol.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/io/__init__.py` & `pyrad_mch-1.8.3/pyrad/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/io/config.py` & `pyrad_mch-1.8.3/pyrad/io/config.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/io/io_aux.py` & `pyrad_mch-1.8.3/pyrad/io/io_aux.py`

 * *Files 1% similar despite different names*

```diff
@@ -2231,16 +2231,16 @@
     -------
     filelist : list of strings
         list of files within the time period. If it could not find them
         returns an empty list
     """
     radarnr, datagroup, datatype, dataset, product = get_datatype_fields(
         datadescriptor)
-    ind_rad = int(radarnr[5:8])-1
 
+    ind_rad = int(radarnr[5:8])-1
     if datatype in ('Nh', 'Nv'):
         datatype = 'dBZ'
 
     filelist = []
     for starttime, endtime in zip(starttimes, endtimes):
         startdate = starttime.replace(
             hour=0, minute=0, second=0, microsecond=0)
@@ -2411,14 +2411,28 @@
                 if not os.path.isdir(datapath):
                     warn("WARNING: Unknown datapath '%s'" % datapath)
                     continue
                 pattern = datapath+dayinfo+'*'+datatype+termination
                 dayfilelist = glob.glob(pattern)
                 for filename in dayfilelist:
                     t_filelist.append(filename)
+            elif datagroup in ('GECSX'):
+                termination = '.nc'
+                # Choose any date 
+                import pdb; pdb.set_trace()
+                datapath = (cfg['gecsxbasepath'][ind_rad] + 
+                            cfg['gecsxname'][ind_rad] + '/' + 
+                            dataset +'/' + product+'/')
+                if not os.path.isdir(datapath):
+                    warn("WARNING: Unknown datapath '%s'" % datapath)
+                    continue
+                pattern = datapath+'*'+datatype+termination
+                dayfilelist = glob.glob(pattern)
+                for filename in dayfilelist:
+                    t_filelist.append(filename)
             elif datagroup in ('MFCFRADIAL', 'MFBIN', 'MFPNG', 'MFGRIB',
                                'MFDAT', 'MFCF'):
                 try:
                     fpath_strf = dataset[
                         dataset.find("D")+2:dataset.find("F")-2]
                 except AttributeError:
                     warn('Unknown directory and/or date ' +
@@ -2483,22 +2497,25 @@
                     warn("WARNING: Unknown datapath '%s'" % datapath)
                     continue
                 pattern = datapath+'*'+dayinfo+'*.nc'
                 dayfilelist = glob.glob(pattern)
                 for filename in dayfilelist:
                     t_filelist.append(filename)
 
-        for filename in t_filelist:
-            filenamestr = str(filename)
-            fdatetime = get_datetime(filenamestr, datadescriptor)
-            if fdatetime is not None:
-                if starttime <= fdatetime <= endtime:
-                    if filenamestr not in filelist:
-                        filelist.append(filenamestr)
-    
+        if datagroup != 'GECSX':
+            for filename in t_filelist:
+                filenamestr = str(filename)
+                fdatetime = get_datetime(filenamestr, datadescriptor)
+                if fdatetime is not None:
+                    if starttime <= fdatetime <= endtime:
+                        if filenamestr not in filelist:
+                            filelist.append(filenamestr)
+        else: # For GECSX we ignore time, since the visibility is static
+            filelist = t_filelist
+            
         if not filelist:
             if pattern != None:
                 warn("WARNING: No file with pattern {:s} could be found between ".format(pattern)+\
                     "starttime {:s} and endtime {:s}".format(str(starttime),
                                                                 str(endtime)))
     return sorted(filelist)
```

### Comparing `pyrad_mch-1.8.2/pyrad/io/mxpol_config.py` & `pyrad_mch-1.8.3/pyrad/io/mxpol_config.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/io/read_data_cosmo.py` & `pyrad_mch-1.8.3/pyrad/io/read_data_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/io/read_data_dem.py` & `pyrad_mch-1.8.3/pyrad/io/read_data_dem.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,14 @@
         raster = gdal.Open(fname)
 
         prj = raster.GetProjection()
         srs = osr.SpatialReference(wkt=prj)
         projparams = _proj4_str_to_dict(srs.ExportToProj4())
         if not len(projparams): # gdal could not read proj
             projparams = None
-        import pdb; pdb.set_trace()
         width = raster.RasterXSize
         height = raster.RasterYSize
         gt = raster.GetGeoTransform()
         minx = gt[0]
         miny = gt[3] + width*gt[4] + height*gt[5]
 
         metadata = {}
```

### Comparing `pyrad_mch-1.8.2/pyrad/io/read_data_hzt.py` & `pyrad_mch-1.8.3/pyrad/io/read_data_hzt.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/io/read_data_iso0_mf.py` & `pyrad_mch-1.8.3/pyrad/io/read_data_iso0_mf.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/io/read_data_mxpol.py` & `pyrad_mch-1.8.3/pyrad/io/read_data_mxpol.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/io/read_data_other.py` & `pyrad_mch-1.8.3/pyrad/io/read_data_other.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/io/read_data_radar.py` & `pyrad_mch-1.8.3/pyrad/io/read_data_radar.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,15 +607,15 @@
             datatype_odimpyrad, dataset_odimpyrad, product_odimpyrad,
             rng_min=rmin, rng_max=rmax, ele_min=elmin, ele_max=elmax,
             azi_min=azmin, azi_max=azmax, termination='.h*')
         radar = add_field(radar, radar_aux)
 
     if ndatatypes_gecsx > 0:
         radar_aux = merge_fields_gecsx(
-            cfg['loadbasepath'][ind_rad], cfg['loadname'][ind_rad],
+            cfg['gecsxbasepath'][ind_rad], cfg['gecsxname'][ind_rad],
             datatype_gecsx, dataset_gecsx, product_gecsx,
             rng_min=rmin, rng_max=rmax, ele_min=elmin, ele_max=elmax,
             azi_min=azmin, azi_max=azmax)
         radar = add_field(radar, radar_aux)
         
     if ndatatypes_cfradialcosmo > 0:
         radar_aux = merge_fields_pyradcosmo(
@@ -2500,19 +2500,21 @@
         filename = []
         for filename_aux in filenames:
             fdatetime = find_date_in_file_name(
                 filename_aux, date_format=fdate_strf)
             if fdatetime == voltime:
                 filename = [filename_aux]
     elif cfg['path_convention'][ind_rad] == 'RADARV':
+        datapath = basepath+scan_list[0]
+        basename = '*'
         fpath_strf = (
             dataset_list[0][
                 dataset_list[0].find("D")+2:dataset_list[0].find("F")-2])
         fdate_strf = dataset_list[0][dataset_list[0].find("F")+2:-1]
-        filenames = glob.glob(basepath+scan_list[0]+'/'+'/'+
+        filenames = glob.glob(basepath+scan_list[0]+'/'+
                               voltime.strftime(fpath_strf)+'/*')
         filename = []
         for filename_aux in filenames:
             fdatetime = find_date_in_file_name(
                 filename_aux, date_format=fdate_strf)
             if fdatetime == voltime:
                 filename = [filename_aux]
@@ -2565,25 +2567,44 @@
             for filename_aux in filenames:
                 fdatetime = find_date_in_file_name(
                     filename_aux, date_format=fdate_strf)
                 if fdatetime == voltime:
                     filename = [filename_aux]
                     break
         elif cfg['path_convention'][ind_rad] == 'RADARV':
-            filename = glob.glob(basepath+scan+'/'+'/'+
+            filenames = glob.glob(basepath+scan+'/'+'/'+
                               voltime.strftime(fpath_strf)+'/*')
+            filename = []
+            for filename_aux in filenames:
+                fdatetime = find_date_in_file_name(
+                    filename_aux, date_format=fdate_strf)
+                if cfg['MasterScanTimeTol'][ind_rad] == 0:
+                    if fdatetime == voltime:
+                        filename = [filename_aux]
+                        break
+                elif cfg['MasterScanTimeTol'][ind_rad] == 1:
+                    if (voltime <= fdatetime < voltime
+                            + datetime.timedelta(
+                                minutes=cfg['ScanPeriod'])):
+                        filename = [filename_aux]
+                        break
+                else:
+                    if (voltime
+                        - datetime.timedelta(minutes=cfg['ScanPeriod'])
+                            < fdatetime <= voltime):
+                        filename = [filename_aux]
+                        break
         else:
             filename = glob.glob(datapath+basename+timeinfo+'*'+scan+'*')
         if not filename:
             warn('No file found in '+datapath+basename+timeinfo+'*.'+scan)
         else:
             radar_aux = pyart.io.read_cfradial2(filename[0], field_names=field_names)
             if radar_aux is None:
                 continue
-
             if radar is None:
                 radar = radar_aux
             else:
                 radar = pyart.util.radar_utils.join_radar(radar, radar_aux)
 
     if radar is None:
         return radar
@@ -4001,20 +4022,19 @@
     """
     radar = None
     for i, dataset in enumerate(dataset_list):
         datapath = (
             basepath+loadname+'/' +
             dataset+'/'+product_list[i]+'/')
         filename = glob.glob(
-            datapath+'*'+datatype_list[i]+'.nc')
+            datapath+'*'+datatype_list[i]+'*.nc')
         if not filename:
             warn('No file found in '+datapath+'*' +
-                 datatype_list[i]+'.nc')
+                 datatype_list[i]+'*.nc')
             continue
-
         try:
             radar_aux = pyart.io.read_cfradial(filename[0])
         except (OSError, KeyError) as ee:
             warn(str(ee))
             warn('Unable to read file '+filename[0])
             radar_aux = None
```

### Comparing `pyrad_mch-1.8.2/pyrad/io/read_data_sensor.py` & `pyrad_mch-1.8.3/pyrad/io/read_data_sensor.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/io/read_data_sun.py` & `pyrad_mch-1.8.3/pyrad/io/read_data_sun.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/io/timeseries.py` & `pyrad_mch-1.8.3/pyrad/io/timeseries.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/io/trajectory.py` & `pyrad_mch-1.8.3/pyrad/io/trajectory.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/io/write_data.py` & `pyrad_mch-1.8.3/pyrad/io/write_data.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/__init__.py` & `pyrad_mch-1.8.3/pyrad/proc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_Doppler.py` & `pyrad_mch-1.8.3/pyrad/proc/process_Doppler.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_aux.py` & `pyrad_mch-1.8.3/pyrad/proc/process_aux.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_calib.py` & `pyrad_mch-1.8.3/pyrad/proc/process_calib.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_cosmo.py` & `pyrad_mch-1.8.3/pyrad/proc/process_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_dem.py` & `pyrad_mch-1.8.3/pyrad/proc/process_dem.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_echoclass.py` & `pyrad_mch-1.8.3/pyrad/proc/process_echoclass.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_grid.py` & `pyrad_mch-1.8.3/pyrad/proc/process_grid.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_intercomp.py` & `pyrad_mch-1.8.3/pyrad/proc/process_intercomp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1240,21 +1240,21 @@
         ind_radar_list.add(int(radarnr[5:8])-1)
 
     ind_radar_list = list(ind_radar_list)
 
     if (len(radarnr_dict) != 2) or (len(radar_list) < 2):
         warn('Intercomparison requires data from two different radars')
         return None, None
-
+    
     # create the list of data types for each radar
     for datatypedescr in dscfg['datatype']:
         radarnr, _, datatype, _, _ = get_datatype_fields(datatypedescr)
         if radarnr in radarnr_dict:
             radarnr_dict[radarnr].append(get_fieldname_pyart(datatype))
-
+    
     radar1 = radar_list[ind_radar_list[0]]
     radar2 = radar_list[ind_radar_list[1]]
 
     if radar1 is None or radar2 is None:
         warn('Unable to inter-compare radars. Missing radar')
 
     if 'instrument_name' in radar1.metadata:
```

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_iq.py` & `pyrad_mch-1.8.3/pyrad/proc/process_iq.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_monitoring.py` & `pyrad_mch-1.8.3/pyrad/proc/process_monitoring.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,14 @@
                     zdr_kdpzh_list.append(zdr_kdpzh_table)
                     el_list.append((el/10.).astype(int))
             if not el_list:
                 warn('Unable to retrieve PhiDP and KDP using self-consistency. ' +
                      'No selfconsistency files for the radar elevations.')
 
                 return None, None
-            import pdb; pdb.set_trace()
             zdr_kdpzh_dict = {'zdr_kdpzh': zdr_kdpzh_list,
                               'elev': el_list,
                               'freq_band': freq_band}
         else:
             zdr_kdpzh_dict = {'zdr_kdpzh': None,
                               'elev': None,
                               'freq_band': freq_band}
```

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_phase.py` & `pyrad_mch-1.8.3/pyrad/proc/process_phase.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_retrieve.py` & `pyrad_mch-1.8.3/pyrad/proc/process_retrieve.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_spectra.py` & `pyrad_mch-1.8.3/pyrad/proc/process_spectra.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_timeseries.py` & `pyrad_mch-1.8.3/pyrad/proc/process_timeseries.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/proc/process_traj.py` & `pyrad_mch-1.8.3/pyrad/proc/process_traj.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/prod/__init__.py` & `pyrad_mch-1.8.3/pyrad/prod/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/prod/process_grid_products.py` & `pyrad_mch-1.8.3/pyrad/prod/process_grid_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/prod/process_intercomp_products.py` & `pyrad_mch-1.8.3/pyrad/prod/process_intercomp_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/prod/process_monitoring_products.py` & `pyrad_mch-1.8.3/pyrad/prod/process_monitoring_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/prod/process_product.py` & `pyrad_mch-1.8.3/pyrad/prod/process_product.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/prod/process_spectra_products.py` & `pyrad_mch-1.8.3/pyrad/prod/process_spectra_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/prod/process_timeseries_products.py` & `pyrad_mch-1.8.3/pyrad/prod/process_timeseries_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/prod/process_traj_products.py` & `pyrad_mch-1.8.3/pyrad/prod/process_traj_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/prod/process_vol_products.py` & `pyrad_mch-1.8.3/pyrad/prod/process_vol_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/prod/product_aux.py` & `pyrad_mch-1.8.3/pyrad/prod/product_aux.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/util/__init__.py` & `pyrad_mch-1.8.3/pyrad/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/util/radar_utils.py` & `pyrad_mch-1.8.3/pyrad/util/radar_utils.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad/util/stat_utils.py` & `pyrad_mch-1.8.3/pyrad/util/stat_utils.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/pyrad_mch.egg-info/PKG-INFO` & `pyrad_mch-1.8.3/pyrad_mch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrad-mch
-Version: 1.8.2
+Version: 1.8.3
 Summary:  Python Radar Toolkit
 Home-page: https://github.com/MeteoSwiss/pyrad.git
 Author: MeteoSwiss Pyrad Developers
 Author-email: daniel.wolfensberger@meteoswiss.ch
 Maintainer: MeteoSwiss Pyrad Developers
 Maintainer-email: daniel.wolfensberger@meteoswiss.ch
 License: BSD
```

### Comparing `pyrad_mch-1.8.2/pyrad_mch.egg-info/SOURCES.txt` & `pyrad_mch-1.8.3/pyrad_mch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/scripts/common_colocated_gates.py` & `pyrad_mch-1.8.3/scripts/common_colocated_gates.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/scripts/main_precipitation_comparison.py` & `pyrad_mch-1.8.3/scripts/main_precipitation_comparison.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/scripts/main_process_cosmo.py` & `pyrad_mch-1.8.3/scripts/main_process_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/scripts/main_process_cosmo_rt.py` & `pyrad_mch-1.8.3/scripts/main_process_cosmo_rt.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/scripts/main_process_data.py` & `pyrad_mch-1.8.3/scripts/main_process_data.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/scripts/main_process_data_birds.py` & `pyrad_mch-1.8.3/scripts/main_process_data_birds.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/scripts/main_process_data_period.py` & `pyrad_mch-1.8.3/scripts/main_process_data_period.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/scripts/main_process_data_rt.py` & `pyrad_mch-1.8.3/scripts/main_process_data_rt.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/scripts/main_process_data_trt.py` & `pyrad_mch-1.8.3/scripts/main_process_data_trt.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/scripts/main_process_euclid_data.py` & `pyrad_mch-1.8.3/scripts/main_process_euclid_data.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/scripts/main_process_gecsx.py` & `pyrad_mch-1.8.3/scripts/main_process_gecsx.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/scripts/movie_maker.py` & `pyrad_mch-1.8.3/scripts/movie_maker.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/scripts/rewrite_monitoring.py` & `pyrad_mch-1.8.3/scripts/rewrite_monitoring.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.2/setup.py` & `pyrad_mch-1.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 URL = "https://github.com/MeteoSwiss/pyrad.git"
 DOWNLOAD_URL = "https://github.com/MeteoSwiss/pyrad.git"
 LICENSE = 'BSD'
 CLASSIFIERS = list(filter(None, CLASSIFIERS.split('\n')))
 PLATFORMS = ["Linux"]
 MAJOR = 1
 MINOR = 8
-MICRO = 2
+MICRO = 3
 ISRELEASED = True
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 SCRIPTS = glob.glob('scripts/*')
 COMPILE_DATE_TIME = datetime.utcnow().strftime("%Y-%m-%d %H:%M")
 USERNAME = getpass.getuser()
```

