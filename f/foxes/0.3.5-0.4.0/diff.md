# Comparing `tmp/foxes-0.3.5.tar.gz` & `tmp/foxes-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxes-0.3.5.tar", last modified: Fri Jun  2 09:25:48 2023, max compression
+gzip compressed data, was "foxes-0.4.0.tar", last modified: Mon Jun 12 12:59:15 2023, max compression
```

## Comparing `foxes-0.3.5.tar` & `foxes-0.4.0.tar`

### file list

```diff
@@ -1,261 +1,262 @@
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1071 2023-06-02 08:05:39.000000 foxes-0.3.5/LICENSE
--rw-r--r--   0 jonas     (1000) jonas     (1000)    40774 2023-06-02 08:05:43.000000 foxes-0.3.5/Logo_FOXES.svg
--rw-r--r--   0 jonas     (1000) jonas     (1000)      215 2023-06-02 08:05:43.000000 foxes-0.3.5/MANIFEST.in
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6589 2023-06-02 09:25:48.016762 foxes-0.3.5/PKG-INFO
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5769 2023-06-02 08:05:39.000000 foxes-0.3.5/README.md
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/
--rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/VERSION
--rw-r--r--   0 jonas     (1000) jonas     (1000)      717 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/algorithms/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      188 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/algorithms/downwind/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       53 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/algorithms/downwind/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    17305 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/downwind/downwind.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/algorithms/downwind/models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      242 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/algorithms/downwind/models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2292 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/algorithms/downwind/models/calc_order.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3329 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/downwind/models/farm_wakes_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4391 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/downwind/models/point_wakes_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1876 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/algorithms/downwind/models/set_amb_farm_results.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1500 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/downwind/models/set_amb_point_results.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/algorithms/iterative/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       55 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/algorithms/iterative/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2016 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/iterative/iterative.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/algorithms/iterative/models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      161 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/algorithms/iterative/models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5050 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/iterative/models/convergence.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3266 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/iterative/models/farm_wakes_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4064 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/algorithms/iterative/models/loop_runner.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1568 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/constants.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/core/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      811 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    16434 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/algorithm.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2834 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/data.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7848 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/data_calc_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12026 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/farm_controller.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7098 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/farm_data_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      246 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/farm_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5498 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5054 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/partial_wakes_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6951 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/point_data_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12678 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/rotor_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8029 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/states.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2929 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/turbine.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1058 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/turbine_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1304 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/turbine_type.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1619 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/vertical_profile.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6499 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/core/wake_frame.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2901 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/wake_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2540 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/wake_superposition.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1636 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/core/wind_farm.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/data/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/data/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/data/farms/
--rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/farms/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1872 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/farms/test_farm_67.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2916 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/data/parse.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/data/power_ct_curves/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      410 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)      300 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)      851 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)      401 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/power_ct_curves/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/data/states/
--rw-r--r--   0 jonas     (1000) jonas     (1000)   427815 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/WRF-Timeseries-4464.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)   126124 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/abl_states_6000.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)    29085 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/timeseries_3000.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)    78694 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/timeseries_8000.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4943 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/wind_rose_bremen.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10990 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/states/wind_rotation.nc
--rw-r--r--   0 jonas     (1000) jonas     (1000)      519 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/data/static_data.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/input/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      125 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/input/farm_layout/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      250 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3169 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/from_csv.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      547 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/from_df.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1553 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/from_file.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1618 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/from_json.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1444 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/grid.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1175 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/farm_layout/row.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/input/states/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      278 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/input/states/create/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       81 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/input/states/create/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3247 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/create/random_abl_states.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    15926 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/field_data_nc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12343 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/multi_height.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4362 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/scan_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5734 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/single.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10481 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/states/states_table.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/input/windio/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       88 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/windio/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8679 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/input/windio/windio.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      375 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/models/farm_controllers/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       71 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/farm_controllers/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      211 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/farm_controllers/basic.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/models/farm_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       65 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/farm_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3347 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/farm_models/turbine2farm.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    13156 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/model_book.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes/models/partial_wakes/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      241 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/partial_wakes/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10383 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/partial_wakes/axiwake.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10685 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/partial_wakes/distsliced.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2571 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/partial_wakes/grid.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7397 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/partial_wakes/mapped.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6126 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/partial_wakes/rotor_points.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9578 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/partial_wakes/top_hat.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/point_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      130 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/point_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4430 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/point_models/set_uniform_data.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1372 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/point_models/tke2ti.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1935 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/point_models/wake_deltas.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/rotor_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       82 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/rotor_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5587 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/rotor_models/centre.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4840 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/rotor_models/grid.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/turbine_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      419 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2531 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/calculator.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2757 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/kTI_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5410 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/power_mask.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4415 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/rotor_centre_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7541 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/sector_management.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3392 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/set_XYHD.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3846 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_models/set_farm_vars.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5120 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/turbine_models/table_factors.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2060 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/turbine_models/thrust2ct.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1580 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/turbine_models/yaw2yawm.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1551 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/turbine_models/yawm2yaw.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/turbine_types/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1429 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_types/CpCt_file.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2131 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_types/CpCt_from_two.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7723 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_types/PCt_file.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8853 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_types/PCt_from_two.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      250 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_types/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1284 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/turbine_types/null_type.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11067 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/turbine_types/wsrho2PCt_two_files.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/vertical_profiles/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       93 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/vertical_profiles/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      289 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1082 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_neutral_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1161 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_stable_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1173 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_unstable_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2495 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1148 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/vertical_profiles/abl_log/sheared_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      375 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/vertical_profiles/uniform.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/wake_frames/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      164 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_frames/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4675 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_frames/farm_order.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3732 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_frames/rotor_wd.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11876 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_frames/streamlines.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8181 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_frames/yawed_wakes.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/wake_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      228 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2672 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/wake_models/axisymmetric.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6506 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/dist_sliced.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2637 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/models/wake_models/gaussian.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/wake_models/ti/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      124 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/ti/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8307 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/ti/crespo_hernandez.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6126 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/ti/iec_ti.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5037 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/top_hat.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/wake_models/wind/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      212 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/wind/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5463 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/wind/bastankhah.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4954 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/wind/jensen.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    14670 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/wind/porte_agel.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11887 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_models/wind/turbopark.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/models/wake_superpositions/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      236 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_superpositions/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5888 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_superpositions/linear.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6676 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_superpositions/max.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3783 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_superpositions/product.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6469 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_superpositions/quadratic.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4756 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/models/wake_superpositions/ti_superp.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      171 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/constraints/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      158 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/constraints/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5927 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/constraints/area_geometry.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7419 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/constraints/min_dist.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/core/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      288 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/core/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1937 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/core/farm_constraint.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1936 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/core/farm_objective.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9497 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/core/farm_opt_problem.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7766 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/core/farm_vars_problem.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5600 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/core/pop_states.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/objectives/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/objectives/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8807 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/objectives/farm_vars.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4050 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/objectives/max_n_turbines.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/problems/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      102 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/problems/layout/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      228 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5753 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/farm_layout.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      385 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8090 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/constraints.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8052 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7474 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9992 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    14102 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6271 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/objectives.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11691 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/reggrids_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10534 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/layout/regular_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    19545 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/opt/problems/opt_farm_vars.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/output/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      391 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10553 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/farm_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    15706 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/farm_results_eval.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    45193 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/flow_plots_2d.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2189 2023-06-02 08:05:43.000000 foxes-0.3.5/foxes/output/output.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2580 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/results_writer.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9997 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/rose_plot.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2347 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/state_turbine_map.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5450 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/output/turbine_type_curves.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/utils/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      480 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/utils/abl/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      134 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/abl/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1278 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/abl/neutral.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      442 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/abl/sheared.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1728 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/abl/stable.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1530 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/abl/unstable.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3308 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/cubic_roots.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5141 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/data_book.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      793 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/dict.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.016762 foxes-0.3.5/foxes/utils/geom2d/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      217 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    18791 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/area_geometry.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4450 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/circle.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1626 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/example_intersection.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1750 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/example_union.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6090 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/half_plane.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5462 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geom2d/polygon.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7842 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/geopandas_helpers.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4618 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/pandas_helpers.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      350 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/plotly_helpers.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5792 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/runners.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      362 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/subclasses.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2758 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/utils/two_circles.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2746 2023-06-02 08:05:44.000000 foxes-0.3.5/foxes/utils/wind_dir.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3401 2023-06-02 09:24:47.000000 foxes-0.3.5/foxes/variables.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-02 09:25:48.006762 foxes-0.3.5/foxes.egg-info/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6589 2023-06-02 09:25:47.000000 foxes-0.3.5/foxes.egg-info/PKG-INFO
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7742 2023-06-02 09:25:47.000000 foxes-0.3.5/foxes.egg-info/SOURCES.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-06-02 09:25:47.000000 foxes-0.3.5/foxes.egg-info/dependency_links.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)      195 2023-06-02 09:25:47.000000 foxes-0.3.5/foxes.egg-info/requires.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-06-02 09:25:47.000000 foxes-0.3.5/foxes.egg-info/top_level.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-06-02 09:25:47.000000 foxes-0.3.5/foxes.egg-info/zip-safe
--rw-r--r--   0 jonas     (1000) jonas     (1000)      185 2023-06-02 08:05:39.000000 foxes-0.3.5/pyproject.toml
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1131 2023-06-02 09:25:48.016762 foxes-0.3.5/setup.cfg
--rw-r--r--   0 jonas     (1000) jonas     (1000)       69 2023-06-02 08:05:43.000000 foxes-0.3.5/setup.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1071 2023-06-02 08:05:39.000000 foxes-0.4.0/LICENSE
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    40774 2023-06-02 08:05:43.000000 foxes-0.4.0/Logo_FOXES.svg
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      215 2023-06-02 08:05:43.000000 foxes-0.4.0/MANIFEST.in
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6589 2023-06-12 12:59:15.634295 foxes-0.4.0/PKG-INFO
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5769 2023-06-12 12:58:21.000000 foxes-0.4.0/README.md
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/VERSION
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      717 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/algorithms/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      188 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/algorithms/downwind/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       53 2023-06-02 08:05:44.000000 foxes-0.4.0/foxes/algorithms/downwind/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    17305 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/downwind/downwind.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/algorithms/downwind/models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      242 2023-06-02 08:05:44.000000 foxes-0.4.0/foxes/algorithms/downwind/models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2292 2023-06-06 06:30:42.000000 foxes-0.4.0/foxes/algorithms/downwind/models/calc_order.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3329 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/downwind/models/farm_wakes_calc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4391 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/downwind/models/point_wakes_calc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1876 2023-06-02 08:05:44.000000 foxes-0.4.0/foxes/algorithms/downwind/models/set_amb_farm_results.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1500 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/downwind/models/set_amb_point_results.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/algorithms/iterative/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       55 2023-06-06 06:30:42.000000 foxes-0.4.0/foxes/algorithms/iterative/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2016 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/iterative/iterative.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/algorithms/iterative/models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      161 2023-06-06 06:30:42.000000 foxes-0.4.0/foxes/algorithms/iterative/models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5050 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/iterative/models/convergence.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3266 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/iterative/models/farm_wakes_calc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4064 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/iterative/models/loop_runner.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1568 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/constants.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/core/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      811 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/core/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    16552 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/algorithm.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2951 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/data.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7859 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/data_calc_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12097 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/farm_controller.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7251 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/farm_data_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      269 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/farm_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5554 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5135 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/partial_wakes_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6923 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/point_data_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12744 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/rotor_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8120 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/states.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3059 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/turbine.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1069 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/turbine_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1418 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/turbine_type.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1637 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/vertical_profile.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6492 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/wake_frame.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2908 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/wake_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2547 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/wake_superposition.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1713 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/wind_farm.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/data/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/data/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/data/farms/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/farms/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1872 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/farms/test_farm_67.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2957 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/data/parse.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/data/power_ct_curves/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      410 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      300 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      851 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      401 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/power_ct_curves/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/data/states/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)   427815 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/WRF-Timeseries-4464.csv.gz
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)   126124 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/abl_states_6000.csv.gz
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    29085 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/timeseries_3000.csv.gz
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    78694 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/timeseries_8000.csv.gz
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4943 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/wind_rose_bremen.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10990 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/wind_rotation.nc
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      543 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/data/static_data.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/input/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      125 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/input/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/input/farm_layout/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      250 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/input/farm_layout/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3189 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/farm_layout/from_csv.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      578 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/farm_layout/from_df.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1578 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/farm_layout/from_file.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1646 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/farm_layout/from_json.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1469 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/farm_layout/grid.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1196 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/farm_layout/row.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/input/states/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      302 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/input/states/create/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       81 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/input/states/create/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3270 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/create/random_abl_states.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    16107 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/field_data_nc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12501 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/multi_height.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4459 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/scan_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5850 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/single.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10640 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/states_table.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/input/windio/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       88 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/input/windio/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8680 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/windio/windio.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      375 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/farm_controllers/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       71 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/farm_controllers/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      253 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/farm_controllers/basic.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/farm_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       65 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/farm_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3439 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/farm_models/turbine2farm.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    13207 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/model_book.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/partial_wakes/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      241 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/partial_wakes/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10485 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/partial_wakes/axiwake.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10792 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/partial_wakes/distsliced.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2695 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/partial_wakes/grid.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7519 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/partial_wakes/mapped.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6214 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/partial_wakes/rotor_points.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     9670 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/partial_wakes/top_hat.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/point_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      130 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/point_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4548 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/point_models/set_uniform_data.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1403 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/point_models/tke2ti.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2027 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/point_models/wake_deltas.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/rotor_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       82 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/rotor_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5607 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/rotor_models/centre.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4993 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/rotor_models/grid.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/turbine_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      457 2023-06-12 12:58:21.000000 foxes-0.4.0/foxes/models/turbine_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2658 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/calculator.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2892 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/kTI_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5888 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/lookup_table.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5509 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/power_mask.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4510 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/rotor_centre_calc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7695 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/sector_management.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3500 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/set_XYHD.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4533 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/set_farm_vars.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5247 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/table_factors.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2162 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/thrust2ct.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1613 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/yaw2yawm.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1584 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/yawm2yaw.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/turbine_types/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1567 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/CpCt_file.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2285 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/CpCt_from_two.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7884 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/PCt_file.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     9027 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/PCt_from_two.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      248 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1316 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/null_type.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    11215 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/wsrho2PCt_from_two.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/models/vertical_profiles/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      314 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1121 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/abl_log_neutral_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1200 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/abl_log_stable_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1212 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/abl_log_unstable_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2534 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/abl_log_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1245 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/sheared_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1202 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/uniform.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/models/wake_frames/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      164 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/wake_frames/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4754 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_frames/farm_order.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3816 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_frames/rotor_wd.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    11983 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_frames/streamlines.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8304 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_frames/yawed_wakes.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/models/wake_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      228 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/wake_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2693 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/axisymmetric.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6589 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/dist_sliced.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2659 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/gaussian.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/models/wake_models/ti/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      124 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/wake_models/ti/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8485 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/ti/crespo_hernandez.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6242 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/ti/iec_ti.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5136 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/top_hat.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/models/wake_models/wind/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      212 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/wake_models/wind/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5597 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/wind/bastankhah.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5073 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/wind/jensen.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    15626 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/wind/porte_agel.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12164 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/wind/turbopark.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/models/wake_superpositions/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      236 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/wake_superpositions/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6016 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_superpositions/linear.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6781 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_superpositions/max.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3889 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_superpositions/product.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6574 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_superpositions/quadratic.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4858 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_superpositions/ti_superp.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      171 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/opt/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/constraints/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      158 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/opt/constraints/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6176 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/constraints/area_geometry.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7538 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/constraints/min_dist.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/core/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      288 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/opt/core/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2017 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/core/farm_constraint.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2047 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/core/farm_objective.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10624 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/core/farm_opt_problem.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7778 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/core/farm_vars_problem.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5684 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/core/pop_states.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/objectives/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/opt/objectives/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8998 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/objectives/farm_vars.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4156 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/objectives/max_n_turbines.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/problems/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      103 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/problems/layout/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      228 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/opt/problems/layout/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5772 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/farm_layout.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      385 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    22671 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/constraints.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8176 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_layout.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7598 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10115 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    14234 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    17906 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/objectives.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    11816 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/reggrids_layout.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10637 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/regular_layout.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    19431 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/opt_farm_vars.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/output/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      391 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/output/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10647 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/farm_layout.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    15752 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/farm_results_eval.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    45090 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/flow_plots_2d.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2204 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/output.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2670 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/results_writer.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10073 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/rose_plot.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2425 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/state_turbine_map.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5526 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/turbine_type_curves.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/utils/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      480 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/utils/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/utils/abl/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      134 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/utils/abl/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1370 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/abl/neutral.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      451 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/abl/sheared.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1834 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/abl/stable.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1611 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/abl/unstable.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3321 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/cubic_roots.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5306 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/data_book.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      898 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/dict.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/utils/geom2d/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      251 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/geom2d/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    19159 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/geom2d/area_geometry.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4538 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/geom2d/circle.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1626 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/utils/geom2d/example_intersection.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1750 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/utils/geom2d/example_union.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6175 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/geom2d/half_plane.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5542 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/geom2d/polygon.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7915 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/geopandas_helpers.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4631 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/pandas_helpers.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      373 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/plotly_helpers.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/utils/runners/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       55 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/runners/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6523 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/runners/runners.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      384 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/subclasses.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2818 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/two_circles.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2829 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/wind_dir.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3576 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/variables.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes.egg-info/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6589 2023-06-12 12:59:15.000000 foxes-0.4.0/foxes.egg-info/PKG-INFO
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7734 2023-06-12 12:59:15.000000 foxes-0.4.0/foxes.egg-info/SOURCES.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-06-12 12:59:15.000000 foxes-0.4.0/foxes.egg-info/dependency_links.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      195 2023-06-12 12:59:15.000000 foxes-0.4.0/foxes.egg-info/requires.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-06-12 12:59:15.000000 foxes-0.4.0/foxes.egg-info/top_level.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-06-12 12:59:15.000000 foxes-0.4.0/foxes.egg-info/zip-safe
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      185 2023-06-02 08:05:39.000000 foxes-0.4.0/pyproject.toml
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1131 2023-06-12 12:59:15.634295 foxes-0.4.0/setup.cfg
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       69 2023-06-02 08:05:43.000000 foxes-0.4.0/setup.py
```

### Comparing `foxes-0.3.5/LICENSE` & `foxes-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/Logo_FOXES.svg` & `foxes-0.4.0/Logo_FOXES.svg`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/PKG-INFO` & `foxes-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.3.5
+Version: 0.4.0
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
@@ -53,105 +53,105 @@
 
 - `Python 3.7`
 - `Python 3.8`
 - `Python 3.9`
 - `Python 3.10`
 - `Python 3.11`
 
-## Installation via conda
+## Installation via pip
 
 ### Virtual Python environment
 
-First create a new `conda` environment, for example called `foxes`, by
+First create a new `venv` environment, for example called `foxes` and located at `~/venv/foxes` (choose any other convenient name and location in your file system if you prefer), by
 
 ```console
-conda create -c conda-forge --name foxes
+python3 -m venv ~/venv/foxes
 ```
 
 Then activate the environment every time you work with `foxes`, by
 
 ```console
-conda activate foxes
+source ~/venv/foxes/bin/activate
 ```
 
 You can leave the environment by
 
 ```console
-conda deactivate
+deactivate
 ```
 
-The `conda` installation commands below should be executed within the active `foxes` environment.
+The `pip` installation commands below should be executed within the active `foxes` environment.
 
 ### Standard users
 
-The `foxes` package is available on the channel [conda-forge](https://anaconda.org/conda-forge/foxes). You can install the latest version by
+As a standard user, you can install the latest release via [pip](https://pypi.org/project/foxes/) by
 
 ```console
-conda install -c conda-forge foxes
+pip install foxes
+```
+
+This commands installs the version that correspond to the `main` branch at [github](https://github.com/FraunhoferIWES/foxes). Alternatively, you can decide to install the latest pre-release developments (non-stable) by
+
+```console
+pip install git+https://github.com/FraunhoferIWES/foxes@dev#egg=foxes
 ```
 
 ### Developers
 
-For developers using `conda`, we recommend first installing foxes, then removing only the `foxes` package while keeping the dependencies, and then adding `foxes` again from a git using `conda develop`:
+For developers using `pip`, simply invoke the `-e` flag in the installation command in your local clone:
 
 ```console
-conda install -c conda-forge foxes conda-build
-conda remove foxes --force
 git clone https://github.com/FraunhoferIWES/foxes.git
 cd foxes
-conda develop .
+pip install -e .
 ```
 The last line makes sure that all your code changes are included whenever importing `foxes`. Concerning the `git clone` line, we actually recommend that you fork `foxes` on GitHub and then replace that command by cloning your fork instead.
 
-## Installation via pip
+## Installation via conda
 
 ### Virtual Python environment
 
-First create a new `venv` environment, for example called `foxes` and located at `~/venv/foxes` (choose any other convenient name and location in your file system if you prefer), by
+First create a new `conda` environment, for example called `foxes`, by
 
 ```console
-python3 -m venv ~/venv/foxes
+conda create -c conda-forge --name foxes
 ```
 
 Then activate the environment every time you work with `foxes`, by
 
 ```console
-source ~/venv/foxes/bin/activate
+conda activate foxes
 ```
 
 You can leave the environment by
 
 ```console
-deactivate
+conda deactivate
 ```
 
-The `pip` installation commands below should be executed within the active `foxes` environment.
+The `conda` installation commands below should be executed within the active `foxes` environment.
 
 ### Standard users
 
-As a standard user, you can install the latest release via [pip](https://pypi.org/project/foxes/) by
-
-```console
-pip install foxes
-```
-
-This commands installs the version that correspond to the `main` branch at [github](https://github.com/FraunhoferIWES/foxes). Alternatively, you can decide to install the latest pre-release developments (non-stable) by
+The `foxes` package is available on the channel [conda-forge](https://anaconda.org/conda-forge/foxes). You can install the latest version by
 
 ```console
-pip install git+https://github.com/FraunhoferIWES/foxes@dev#egg=foxes
+conda install -c conda-forge foxes
 ```
 
 ### Developers
 
-For developers using `pip`, simply invoke the `-e` flag in the installation command in your local clone:
+For developers using `conda`, we recommend first installing foxes, then removing only the `foxes` package while keeping the dependencies, and then adding `foxes` again from a git using `conda develop`:
 
 ```console
+conda install -c conda-forge foxes conda-build
+conda remove foxes --force
 git clone https://github.com/FraunhoferIWES/foxes.git
 cd foxes
-pip install -e .
+conda develop .
 ```
 The last line makes sure that all your code changes are included whenever importing `foxes`. Concerning the `git clone` line, we actually recommend that you fork `foxes` on GitHub and then replace that command by cloning your fork instead.
 
 ## Usage
 
 For detailed examples of how to run _foxes_, check the `examples` and `notebooks` folders in this repository. A minimal running example is the following, based on provided static `csv` data files:
```

### Comparing `foxes-0.3.5/README.md` & `foxes-0.4.0/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -31,105 +31,105 @@
 
 - `Python 3.7`
 - `Python 3.8`
 - `Python 3.9`
 - `Python 3.10`
 - `Python 3.11`
 
-## Installation via conda
+## Installation via pip
 
 ### Virtual Python environment
 
-First create a new `conda` environment, for example called `foxes`, by
+First create a new `venv` environment, for example called `foxes` and located at `~/venv/foxes` (choose any other convenient name and location in your file system if you prefer), by
 
 ```console
-conda create -c conda-forge --name foxes
+python3 -m venv ~/venv/foxes
 ```
 
 Then activate the environment every time you work with `foxes`, by
 
 ```console
-conda activate foxes
+source ~/venv/foxes/bin/activate
 ```
 
 You can leave the environment by
 
 ```console
-conda deactivate
+deactivate
 ```
 
-The `conda` installation commands below should be executed within the active `foxes` environment.
+The `pip` installation commands below should be executed within the active `foxes` environment.
 
 ### Standard users
 
-The `foxes` package is available on the channel [conda-forge](https://anaconda.org/conda-forge/foxes). You can install the latest version by
+As a standard user, you can install the latest release via [pip](https://pypi.org/project/foxes/) by
 
 ```console
-conda install -c conda-forge foxes
+pip install foxes
+```
+
+This commands installs the version that correspond to the `main` branch at [github](https://github.com/FraunhoferIWES/foxes). Alternatively, you can decide to install the latest pre-release developments (non-stable) by
+
+```console
+pip install git+https://github.com/FraunhoferIWES/foxes@dev#egg=foxes
 ```
 
 ### Developers
 
-For developers using `conda`, we recommend first installing foxes, then removing only the `foxes` package while keeping the dependencies, and then adding `foxes` again from a git using `conda develop`:
+For developers using `pip`, simply invoke the `-e` flag in the installation command in your local clone:
 
 ```console
-conda install -c conda-forge foxes conda-build
-conda remove foxes --force
 git clone https://github.com/FraunhoferIWES/foxes.git
 cd foxes
-conda develop .
+pip install -e .
 ```
 The last line makes sure that all your code changes are included whenever importing `foxes`. Concerning the `git clone` line, we actually recommend that you fork `foxes` on GitHub and then replace that command by cloning your fork instead.
 
-## Installation via pip
+## Installation via conda
 
 ### Virtual Python environment
 
-First create a new `venv` environment, for example called `foxes` and located at `~/venv/foxes` (choose any other convenient name and location in your file system if you prefer), by
+First create a new `conda` environment, for example called `foxes`, by
 
 ```console
-python3 -m venv ~/venv/foxes
+conda create -c conda-forge --name foxes
 ```
 
 Then activate the environment every time you work with `foxes`, by
 
 ```console
-source ~/venv/foxes/bin/activate
+conda activate foxes
 ```
 
 You can leave the environment by
 
 ```console
-deactivate
+conda deactivate
 ```
 
-The `pip` installation commands below should be executed within the active `foxes` environment.
+The `conda` installation commands below should be executed within the active `foxes` environment.
 
 ### Standard users
 
-As a standard user, you can install the latest release via [pip](https://pypi.org/project/foxes/) by
-
-```console
-pip install foxes
-```
-
-This commands installs the version that correspond to the `main` branch at [github](https://github.com/FraunhoferIWES/foxes). Alternatively, you can decide to install the latest pre-release developments (non-stable) by
+The `foxes` package is available on the channel [conda-forge](https://anaconda.org/conda-forge/foxes). You can install the latest version by
 
 ```console
-pip install git+https://github.com/FraunhoferIWES/foxes@dev#egg=foxes
+conda install -c conda-forge foxes
 ```
 
 ### Developers
 
-For developers using `pip`, simply invoke the `-e` flag in the installation command in your local clone:
+For developers using `conda`, we recommend first installing foxes, then removing only the `foxes` package while keeping the dependencies, and then adding `foxes` again from a git using `conda develop`:
 
 ```console
+conda install -c conda-forge foxes conda-build
+conda remove foxes --force
 git clone https://github.com/FraunhoferIWES/foxes.git
 cd foxes
-pip install -e .
+conda develop .
 ```
 The last line makes sure that all your code changes are included whenever importing `foxes`. Concerning the `git clone` line, we actually recommend that you fork `foxes` on GitHub and then replace that command by cloning your fork instead.
 
 ## Usage
 
 For detailed examples of how to run _foxes_, check the `examples` and `notebooks` folders in this repository. A minimal running example is the following, based on provided static `csv` data files:
```

### Comparing `foxes-0.3.5/foxes/__init__.py` & `foxes-0.4.0/foxes/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/algorithms/downwind/downwind.py` & `foxes-0.4.0/foxes/algorithms/downwind/downwind.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/algorithms/downwind/models/calc_order.py` & `foxes-0.4.0/foxes/algorithms/downwind/models/calc_order.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/algorithms/downwind/models/farm_wakes_calc.py` & `foxes-0.4.0/foxes/algorithms/downwind/models/farm_wakes_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/algorithms/downwind/models/point_wakes_calc.py` & `foxes-0.4.0/foxes/algorithms/downwind/models/point_wakes_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/algorithms/downwind/models/set_amb_farm_results.py` & `foxes-0.4.0/foxes/algorithms/downwind/models/set_amb_farm_results.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/algorithms/downwind/models/set_amb_point_results.py` & `foxes-0.4.0/foxes/algorithms/downwind/models/set_amb_point_results.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/algorithms/iterative/iterative.py` & `foxes-0.4.0/foxes/algorithms/iterative/iterative.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/algorithms/iterative/models/convergence.py` & `foxes-0.4.0/foxes/algorithms/iterative/models/convergence.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/algorithms/iterative/models/farm_wakes_calc.py` & `foxes-0.4.0/foxes/algorithms/iterative/models/farm_wakes_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/algorithms/iterative/models/loop_runner.py` & `foxes-0.4.0/foxes/algorithms/iterative/models/loop_runner.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/constants.py` & `foxes-0.4.0/foxes/constants.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/core/__init__.py` & `foxes-0.4.0/foxes/core/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/core/algorithm.py` & `foxes-0.4.0/foxes/core/algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,49 +15,55 @@
     """
     Abstract base class for algorithms.
 
     Algorithms collect required objects for running
     calculations, and contain the calculation functions
     which are meant to be called from top level code.
 
-    Parameters
-    ----------
-    mbook : foxes.ModelBook
-        The model book
-    farm : foxes.WindFarm
-        The wind farm
-    chunks : dict
-        The chunks choice for running in parallel with dask,
-        e.g. `{"state": 1000}` for chunks of 1000 states
-    verbosity : int
-        The verbosity level, 0 means silent
-    dbook : foxes.DataBook, optional
-        The data book, or None for default
-    keep_models : list of str
-        Keep these models data in memory and do not finalize them
-
     Attributes
     ----------
-    mbook : foxes.ModelBook
+    mbook: foxes.models.ModelBook
         The model book
-    farm : foxes.WindFarm
+    farm: foxes.WindFarm
         The wind farm
-    chunks : dict
+    chunks: dict
         The chunks choice for running in parallel with dask,
         e.g. `{"state": 1000}` for chunks of 1000 states
-    verbosity : int
+    verbosity: int
         The verbosity level, 0 means silent
-    dbook : foxes.DataBook
+    dbook: foxes.DataBook
         The data book, or None for default
-    keep_models : list of str
+    keep_models: list of str
         Keep these models data in memory and do not finalize them
+    
+    :group: core
 
     """
 
     def __init__(self, mbook, farm, chunks, verbosity, dbook=None, keep_models=[]):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        mbook: foxes.models.ModelBook
+            The model book
+        farm: foxes.WindFarm
+            The wind farm
+        chunks: dict
+            The chunks choice for running in parallel with dask,
+            e.g. `{"state": 1000}` for chunks of 1000 states
+        verbosity: int
+            The verbosity level, 0 means silent
+        dbook: foxes.DataBook, optional
+            The data book, or None for default
+        keep_models: list of str
+            Keep these models data in memory and do not finalize them
+
+        """
         super().__init__()
 
         self.name = type(self).__name__
         self.mbook = mbook
         self.farm = farm
         self.chunks = chunks
         self.verbosity = verbosity
@@ -163,20 +169,20 @@
 
     def update_idata(self, models, idata=None, verbosity=None):
         """
         Add to idata memory, optionally update and return idata object.
 
         Parameters
         ----------
-        models : foxes.core.Model or list of foxes.core.Model
+        models: foxes.core.Model or list of foxes.core.Model
             The models to initialize
-        idata : dict, optional
+        idata: dict, optional
             The idata dictionary to be updated, else only add
             to idata memory
-        verbosity : int, optional
+        verbosity: int, optional
             The verbosity level, 0 = silent
 
         """
         if idata is None and not self.initialized:
             raise ValueError(
                 f"Algorithm '{self.name}': update_idata called before initialization"
             )
@@ -294,15 +300,15 @@
 
     def get_models_data(self, idata=None):
         """
         Creates xarray from model input data.
 
         Parameters
         ----------
-        idata : dict, optional
+        idata: dict, optional
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`.
             Take algorithm's idata object by default.
 
         Returns
         -------
@@ -330,17 +336,17 @@
 
     def new_point_data(self, points, states_indices=None):
         """
         Creates a point data xarray object, containing only points.
 
         Parameters
         ----------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The points, shape: (n_states, n_points, 3)
-        states_indices : array_like, optional
+        states_indices: array_like, optional
             The indices of the states dimension
 
         Returns
         -------
         xarray.Dataset
             A dataset containing the points data
 
@@ -367,18 +373,18 @@
     def finalize_model(self, model, verbosity=None):
         """
         Call the finalization routine of the model,
         if not to be kept.
 
         Parameters
         ----------
-        model : foxes.core.Model
+        model: foxes.core.Model
             The model to be finalized, if not in the
             keep_models list
-        verbosity : int, optional
+        verbosity: int, optional
             The verbosity level, 0 = silent
 
         """
         verbosity = self.verbosity if verbosity is None else verbosity
 
         pr = False
         if isinstance(model, FarmController):
@@ -410,15 +416,15 @@
 
     def finalize(self, clear_mem=False):
         """
         Finalizes the algorithm.
 
         Parameters
         ----------
-        clear_mem : bool
+        clear_mem: bool
             Clear idata memory, including keep_models entries
 
         """
         if clear_mem:
             self._idata_mem = Dict()
         if self.initialized:
             super().finalize(self, self.verbosity)
@@ -426,19 +432,19 @@
     @classmethod
     def new(cls, algo_type, *args, **kwargs):
         """
         Run-time algorithm factory.
 
         Parameters
         ----------
-        algo_type : str
+        algo_type: str
             The selected derived class name
-        args : tuple, optional
+        args: tuple, optional
             Additional parameters for the constructor
-        kwargs : dict, optional
+        kwargs: dict, optional
             Additional parameters for the constructor
 
         """
 
         if algo_type is None:
             return None
```

### Comparing `foxes-0.3.5/foxes/core/data.py` & `foxes-0.4.0/foxes/core/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,42 +7,48 @@
 
 class Data(Dict):
     """
     Container for data and meta data.
 
     Used during the calculation of single chunks,
     usually for numpy data (not xarray data).
-
-    Parameters
-    ----------
-    data : dict
-        The initial data to be stored
-    dims : dict
-        The dimensions tuples, same or subset
-        of data keys
-    loop_dims : array_like of str
-        List of the loop dimensions during xarray's
-        `apply_ufunc` calculations
-    name : str
-        The data container name
         
     Attributes
     ----------
-    dims : dict
+    dims: dict
         The dimensions tuples, same or subset
         of data keys
-    loop_dims : array_like of str
+    loop_dims: array_like of str
         List of the loop dimensions during xarray's
         `apply_ufunc` calculations
-    sizes : dict
+    sizes: dict
         The dimension sizes
 
+    :group: core
+    
     """
 
     def __init__(self, data, dims, loop_dims, name="data"):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        data: dict
+            The initial data to be stored
+        dims: dict
+            The dimensions tuples, same or subset
+            of data keys
+        loop_dims: array_like of str
+            List of the loop dimensions during xarray's
+            `apply_ufunc` calculations
+        name: str
+            The data container name
+
+        """
         super().__init__(name="data")
 
         self.update(data)
         self.dims = dims
         self.loop_dims = loop_dims
 
         self.sizes = {}
```

### Comparing `foxes-0.3.5/foxes/core/data_calc_model.py` & `foxes-0.4.0/foxes/core/data_calc_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,36 +19,38 @@
     The calculations are run via xarray's
     `apply_ufunc` function, i.e., they run in
     parallel depending on the dask settings.
 
     For each individual data chunk the `calculate`
     function is called.
 
+    :group: core
+
     """
 
     @abstractmethod
     def calculate(self, algo, *data, **parameters):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        *data : foxes.core.Data
+        data: tuple of foxes.core.Data
             The input data
-        **parameters : dict, optional
+        parameters: dict, optional
             The calculation parameters
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray
 
         """
         pass
 
     def _wrap_calc(
@@ -143,32 +145,32 @@
         Starts the model calculation in parallel, via
         xarray's `apply_ufunc`.
 
         Typically this function is called by algorithms.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        *data : tuple of xarray.Dataset
+        data: tuple of xarray.Dataset
             The input data
         out_vars: list of str
             The calculation output variables
-        loop_dims : array_like of str
+        loop_dims: array_like of str
             List of the loop dimensions during xarray's
             `apply_ufunc` calculations
-        out_core_vars : list of str
+        out_core_vars: list of str
             The core dimensions of the output data, use
             `FC.VARS` for variables dimension (required)
-        **calc_pars : dict, optional
+        calc_pars: dict, optional
             Additional arguments for the `calculate` function
 
         Returns
         -------
-        results : xarray.Dataset
+        results: xarray.Dataset
             The calculation results
 
         """
         # check:
         if not self.initialized:
             raise ValueError(
                 f"DataCalcModel '{self.name}': run_calculation called for uninitialized model"
```

### Comparing `foxes-0.3.5/foxes/core/farm_controller.py` & `foxes-0.4.0/foxes/core/farm_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,40 +5,46 @@
 from .turbine_type import TurbineType
 import foxes.constants as FC
 
 class FarmController(FarmDataModel):
     """
     Analyses selected turbine models and handles their call.
 
-    Parameters
-    ----------
-    pars : dict
-        Parameters for the turbine models, stored
-        under their respective name
-
     Attributes
     ----------
-    turbine_types : list of foxes.core.TurbineType
+    turbine_types: list of foxes.core.TurbineType
         The turbine type of each turbine
-    turbine_model_names : list of str
+    turbine_model_names: list of str
         Names of all turbine models found in the farm
-    turbine_model_sels : numpy.ndarray of bool
+    turbine_model_sels: numpy.ndarray of bool
         Selection flags for all turbine models,
         shape: (n_states, n_turbines, n_models)
-    pre_rotor_models : foxes.core.FarmDataModelList
+    pre_rotor_models: foxes.core.FarmDataModelList
         The turbine models with pre-rotor flag
-    post_rotor_models : foxes.core.FarmDataModelList
+    post_rotor_models: foxes.core.FarmDataModelList
         The turbine models without pre-rotor flag
-    pars : dict
+    pars: dict
         Parameters for the turbine models, stored
         under their respecitve name
 
+    :group: core
+    
     """
 
     def __init__(self, pars={}):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        pars: dict
+            Parameters for the turbine models, stored
+            under their respective name
+
+        """
         super().__init__()
 
         self.turbine_types = None
         self.turbine_model_names = None
         self.turbine_model_sels = None
         self.pre_rotor_models = None
         self.post_rotor_models = None
@@ -47,21 +53,21 @@
 
     def set_pars(self, model_name, init_pars, calc_pars, final_pars):
         """
         Set parameters for a turbine model
 
         Parameters
         ----------
-        model_name : str
+        model_name: str
             Name of the model
-        init_pars : dict
+        init_pars: dict
             Parameters for initialization
-        calc_pars : dict
+        calc_pars: dict
             Parameters for calculation
-        final_pars : dict
+        final_pars: dict
             Parameters for finalization
 
         """
         self.pars[model_name] = {
             "init": init_pars,
             "calc": calc_pars,
             "final": final_pars,
@@ -129,15 +135,15 @@
     def collect_models(self, algo):
         """
         Analyze and gather turbine models, based on the
         turbines of the wind farm.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         """
 
         # check turbine models, and find turbine types and pre/post-rotor models:
         self.turbine_types = [None for t in algo.farm.turbines]
         prer_models = [[] for t in algo.farm.turbines]
@@ -235,22 +241,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
 
@@ -270,20 +276,20 @@
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return list(
             dict.fromkeys(
                 self.pre_rotor_models.output_farm_vars(algo)
                 + self.post_rotor_models.output_farm_vars(algo)
@@ -295,30 +301,30 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pre_rotor : bool
+        pre_rotor: bool
             Flag for running pre-rotor or post-rotor
             models
-        st_sel : numpy.ndarray of bool, optional
+        st_sel: numpy.ndarray of bool, optional
             Selection of states and turbines, shape:
             (n_states, n_turbines). None for all.
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         s = self.pre_rotor_models if pre_rotor else self.post_rotor_models
         pars = self.__get_pars(algo, s.models, "calc", mdata, st_sel, from_data=True)
         res = s.calculate(algo, mdata, fdata, parameters=pars)
@@ -327,17 +333,17 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 means silent
 
         """
         for s in [self.pre_rotor_models, self.post_rotor_models]:
             if s is not None and s.initialized:
                 algo.finalize_model(s, verbosity)
```

### Comparing `foxes-0.3.5/foxes/core/farm_data_model.py` & `foxes-0.4.0/foxes/core/farm_data_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,45 +4,51 @@
 import foxes.constants as FC
 
 class FarmDataModel(DataCalcModel):
     """
     Abstract base class for models that modify
     farm data.
 
-    Parameters
-    ----------
-    pre_rotor : bool
-        Flag for running this model before
-        running the rotor model.
-
     Attributes
     ----------
-    pre_rotor : bool
+    pre_rotor: bool
         Flag for running this model before
         running the rotor model.
 
+    :group: core
+    
     """
 
     def __init__(self, pre_rotor=False):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        pre_rotor: bool
+            Flag for running this model before
+            running the rotor model.
+
+        """
         super().__init__()
         self.pre_rotor = pre_rotor
 
     @abstractmethod
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return []
 
     @abstractmethod
     def calculate(self, algo, mdata, fdata):
@@ -50,24 +56,24 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         pass
 
     def run_calculation(self, algo, *data, out_vars, **calc_pars):
@@ -75,26 +81,26 @@
         Starts the model calculation in parallel, via
         xarray's `apply_ufunc`.
 
         Typically this function is called by algorithms.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        *data : tuple of xarray.Dataset
+        *data: tuple of xarray.Dataset
             The input data
         out_vars: list of str
             The calculation output variables
-        **calc_pars : dict, optional
+        **calc_pars: dict, optional
             Additional arguments for the `calculate` function
 
         Returns
         -------
-        results : xarray.Dataset
+        results: xarray.Dataset
             The calculation results
 
         """
         return super().run_calculation(
             algo,
             *data,
             out_vars=out_vars,
@@ -116,54 +122,60 @@
     """
     A list of farm data models.
 
     By using the FarmDataModelList the models'
     `calculate` functions are called together
     under one common call of xarray's `apply_ufunc`.
 
-    Parameters
-    ----------
-    models : list of foxes.core.FarmDataModel
-        The model list
-
     Attributes
     ----------
-    models : list of foxes.core.FarmDataModel
+    models: list of foxes.core.FarmDataModel
         The model list
+    
+    :group: core
 
     """
 
     def __init__(self, models=[]):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        models: list of foxes.core.FarmDataModel
+            The model list
+
+        """
         super().__init__()
         self.models = models
 
     def append(self, model):
         """
         Add a model to the list
 
         Parameters
         ----------
-        model : foxes.core.FarmDataModel
+        model: foxes.core.FarmDataModel
             The model to add
 
         """
         self.models.append(model)
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         ovars = []
         for m in self.models:
             ovars += m.output_farm_vars(algo)
         return list(dict.fromkeys(ovars))
@@ -176,22 +188,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
 
@@ -205,26 +217,26 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        parameters : list of dict, optional
+        parameters: list of dict, optional
             A list of parameter dicts, one for each model
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         if parameters is None:
             parameters = [{}] * len(self.models)
         elif not isinstance(parameters, list):
@@ -245,17 +257,17 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 means silent
 
         """
         for m in self.models:
             if m.initialized:
                 algo.finalize_model(m, verbosity)
```

### Comparing `foxes-0.3.5/foxes/core/model.py` & `foxes-0.4.0/foxes/core/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,27 @@
 
 class Model(metaclass=ABCMeta):
     """
     Base class for all models.
 
     Attributes
     ----------
-    name : str
+    name: str
         The model name
+    
+    :group: core
 
     """
 
     _ids = {}
 
     def __init__(self):
+        """
+        Constructor.
+        """
         t = type(self).__name__
         if t not in self._ids:
             self._ids[t] = count(0)
         self._id = next(self._ids[t])
 
         ext = "" if self._id == 0 else f"{self._id}"
         self.name = f"{type(self).__name__}{ext}"
@@ -46,15 +51,15 @@
 
     def var(self, v):
         """
         Creates a model specific variable name.
 
         Parameters
         ----------
-        v : str
+        v: str
             The variable name
 
         Returns
         -------
         str
             Model specific variable name
 
@@ -82,22 +87,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         if self.initialized:
             raise ValueError(
@@ -108,17 +113,17 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         if not self.initialized:
             raise ValueError(
                 f"Model '{self.name}': Finalization called for uninitialized object"
             )
@@ -135,21 +140,21 @@
     ):
         """
         Getter for a data entry in either the given
         data source, or the model object.
 
         Parameters
         ----------
-        variable : str
+        variable: str
             The variable, serves as data key
-        data : dict
+        data: dict
             The data source
-        st_sel : numpy.ndarray of bool, optional
+        st_sel: numpy.ndarray of bool, optional
             If given, get the specified state-turbine subset
-        upcast : str, optional
+        upcast: str, optional
             Either 'farm' or 'points', broadcasts potential
             scalar data to numpy.ndarray with dimensions
             (n_states, n_turbines) or (n_states, n_points),
             respectively
         data_prio: bool
             First search the data source, then the object
         accept_none: bool
```

### Comparing `foxes-0.3.5/foxes/core/partial_wakes_model.py` & `foxes-0.4.0/foxes/core/partial_wakes_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,32 +7,38 @@
 class PartialWakesModel(Model):
     """
     Abstract base class for partial wakes models.
 
     Partial wakes models compute wake effects
     for rotor effective quantities.
 
-    Parameters
-    ----------
-    wake_models : list of foxes.core.WakeModel
-        The wake model selection, None for all
-        from algorithm.
-    wake_frame : foxes.core.WakeFrame, optional
-        The wake frame, None takes from algorithm
-
     Attributes
     ----------
-    wake_models : list of foxes.core.WakeModel
+    wake_models: list of foxes.core.WakeModel
         The wake model selection
-    wake_frame : foxes.core.WakeFrame, optional
+    wake_frame: foxes.core.WakeFrame, optional
         The wake frame
+    
+    :group: core
 
     """
 
     def __init__(self, wake_models=None, wake_frame=None):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        wake_models: list of foxes.core.WakeModel
+            The wake model selection, None for all
+            from algorithm.
+        wake_frame: foxes.core.WakeFrame, optional
+            The wake frame, None takes from algorithm
+
+        """
         super().__init__()
 
         self._wmodels = wake_models
         self._wframe = wake_frame
 
     def initialize(self, algo, verbosity=0):
         """
@@ -42,22 +48,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.wake_models = algo.wake_models if self._wmodels is None else self._wmodels
         self.wake_frame = algo.wake_frame if self._wframe is None else self._wframe
@@ -71,24 +77,24 @@
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        wake_deltas : dict
+        wake_deltas: dict
             Keys: Variable name str, values: any
 
         """
         pass
 
     @abstractmethod
     def contribute_to_wake_deltas(
@@ -96,24 +102,24 @@
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray of int
+        states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
-        wake_deltas : Any
+        wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
         """
         pass
 
     @abstractmethod
@@ -122,43 +128,43 @@
     ):
         """
         Updates the farm data according to the wake
         deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
             Modified in-place by this function
-        wake_deltas : Any
+        wake_deltas: Any
             The wake deltas object, created by the
             `new_wake_deltas` function and filled
             by `contribute_to_wake_deltas`
-        states_turbine : numpy.ndarray of int
+        states_turbine: numpy.ndarray of int
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
-        update_amb_res : bool
+        update_amb_res: bool
             Flag for updating ambient results
 
         """
         pass
 
     @classmethod
     def new(cls, pwake_type, **kwargs):
         """
         Run-time partial wakes factory.
 
         Parameters
         ----------
-        pwake_type : str
+        pwake_type: str
             The selected derived class name
 
         """
 
         if pwake_type is None:
             return None
```

### Comparing `foxes-0.3.5/foxes/core/point_data_model.py` & `foxes-0.4.0/foxes/core/point_data_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,27 @@
 from .data_calc_model import DataCalcModel
 import foxes.constants as FC
 
 class PointDataModel(DataCalcModel):
     """
     Abstract base class for models that modify
     point based data.
+
+    :group: core
+    
     """
 
     @abstractmethod
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
-        Parameters
-        ----------
-        algo : foxes.core.Algorithm
-            The calculation algorithm
-
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return []
 
     @abstractmethod
     def calculate(self, algo, mdata, fdata, pdata):
@@ -33,26 +31,26 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pdata : foxes.core.Data
+        pdata: foxes.core.Data
             The point data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         pass
 
     def run_calculation(self, algo, *data, out_vars, **calc_pars):
@@ -60,26 +58,26 @@
         Starts the model calculation in parallel, via
         xarray's `apply_ufunc`.
 
         Typically this function is called by algorithms.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        *data : tuple of xarray.Dataset
+        *data: tuple of xarray.Dataset
             The input data
         out_vars: list of str
             The calculation output variables
-        **calc_pars : dict, optional
+        **calc_pars: dict, optional
             Additional arguments for the `calculate` function
 
         Returns
         -------
-        results : xarray.Dataset
+        results: xarray.Dataset
             The calculation results
 
         """
         return super().run_calculation(
             algo,
             *data,
             out_vars=out_vars,
@@ -101,54 +99,60 @@
     """
     A list of point data models.
 
     By using the PointDataModelList the models'
     `calculate` functions are called together
     under one common call of xarray's `apply_ufunc`.
 
-    Parameters
-    ----------
-    models : list of foxes.core.PointDataModel
-        The model list
-
     Attributes
     ----------
-    models : list of foxes.core.PointDataModel
+    models: list of foxes.core.PointDataModel
         The model list
 
+    :group: core
+
     """
 
     def __init__(self, models=[]):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        models: list of foxes.core.PointDataModel
+            The model list
+
+        """
         super().__init__()
         self.models = models
 
     def append(self, model):
         """
         Add a model to the list
 
         Parameters
         ----------
-        model : foxes.core.PointDataModel
+        model: foxes.core.PointDataModel
             The model to add
 
         """
         self.models.append(model)
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         ovars = []
         for m in self.models:
             ovars += m.output_point_vars(algo)
         return list(dict.fromkeys(ovars))
@@ -161,22 +165,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         if verbosity > 1:
             print(f"-- {self.name}: Starting initialization -- ")
@@ -194,28 +198,28 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pdata : foxes.core.Data
+        pdata: foxes.core.Data
             The point data
-        parameters : list of dict, optional
+        parameters: list of dict, optional
             A list of parameter dicts, one for each model
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         if parameters is None:
             parameters = [{}] * len(self.models)
         elif not isinstance(parameters, list):
@@ -235,17 +239,17 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 means silent
 
         """
         for m in self.models:
             if m.initialized:
                 algo.finalize_model(m, verbosity)
```

### Comparing `foxes-0.3.5/foxes/core/rotor_model.py` & `foxes-0.4.0/foxes/core/rotor_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,72 +11,78 @@
     """
     Abstract base class of rotor models.
 
     Rotor models calculate ambient farm data from
     states, and provide rotor points and weights
     for the calculation of rotor effective quantities.
 
-    Parameters
-    ----------
-    calc_vars : list of str
-        The variables that are calculated by the model
-        (Their ambients are added automatically)
-
     Attributes
     ----------
-    calc_vars : list of str
+    calc_vars: list of str
         The variables that are calculated by the model
         (Their ambients are added automatically)
 
+    :group: core
+
     """
 
     def __init__(self, calc_vars):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        calc_vars: list of str
+            The variables that are calculated by the model
+            (Their ambients are added automatically)
+
+        """
         super().__init__()
         self.calc_vars = calc_vars
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return self.calc_vars + [
             FV.var2amb[v] for v in self.calc_vars if v in FV.var2amb
         ]
 
     @abstractmethod
     def n_rotor_points(self):
         """
         The number of rotor points
 
         Returns
         -------
-        n_rpoints : int
+        n_rpoints: int
             The number of rotor points
 
         """
         pass
 
     @abstractmethod
     def rotor_point_weights(self):
         """
         The weights of the rotor points
 
         Returns
         -------
-        weights : numpy.ndarray
+        weights: numpy.ndarray
             The weights of the rotor points,
             add to one, shape: (n_rpoints,)
 
         """
         pass
 
     @abstractmethod
@@ -89,36 +95,36 @@
         - (0,0,0) is the centre point,
         - (1,0,0) is the point radius * n_rotor_axis
         - (0,1,0) is the point radius * n_rotor_side
         - (0,0,1) is the point radius * n_rotor_up
 
         Returns
         -------
-        dpoints : numpy.ndarray
+        dpoints: numpy.ndarray
             The design points, shape: (n_points, 3)
 
         """
         pass
 
     def get_rotor_points(self, algo, mdata, fdata):
         """
         Calculates rotor points from design points.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The rotor points, shape:
             (n_states, n_turbines, n_rpoints, 3)
 
         """
 
         n_states = mdata.n_states
         n_points = self.n_rotor_points()
@@ -171,30 +177,30 @@
         for all turbines or one turbine per state,
         depending on parameter `states_turbine`. In
         the latter case, the turbine dimension of the
         `rpoint_results` is expected to have size one.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        rpoint_results : dict
+        rpoint_results: dict
             The results at rotor points. Keys: variable str.
             Values: numpy.ndarray, shape if `states_turbine`
             is None: (n_states, n_turbines, n_rpoints).
             Else: (n_states, 1, n_rpoints)
-        weights : numpy.ndarray
+        weights: numpy.ndarray
             The rotor point weights, shape: (n_rpoints,)
         states_turbine: numpy.ndarray of int, optional
             The turbine indices, one per state. Shape: (n_states,)
-        copy_to_ambient : bool, optional
+        copy_to_ambient: bool, optional
             If `True`, the fdata results are copied to ambient
             variables after calculation
 
         """
 
         n_states = mdata.n_states
         n_turbines = algo.n_turbines
@@ -316,39 +322,39 @@
         states_turbine=None,
     ):
         """
         Calculate ambient rotor effective results.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        rpoints : numpy.ndarray, optional
+        rpoints: numpy.ndarray, optional
             The rotor points, or None for automatic for
             this rotor. Shape: (n_states, n_turbines, n_rpoints, 3)
-        weights : numpy.ndarray, optional
+        weights: numpy.ndarray, optional
             The rotor point weights, or None for automatic
             for this rotor. Shape: (n_rpoints,)
-        store_rpoints : bool, optional
+        store_rpoints: bool, optional
             Switch for storing rotor points to mdata
-        store_rweights : bool, optional
+        store_rweights: bool, optional
             Switch for storing rotor point weights to mdata
-        store_amb_res : bool, optional
+        store_amb_res: bool, optional
             Switch for storing ambient rotor point reults as they
             come from the states to mdata
         states_turbine: numpy.ndarray of int, optional
             The turbine indices, one per state. Shape: (n_states,)
 
         Returns
         -------
-        results : dict
+        results: dict
             results dict. Keys: Variable name str. Values:
             numpy.ndarray with results, shape: (n_states, n_turbines)
 
         """
 
         if rpoints is None:
             rpoints = mdata.get(FC.RPOINTS, self.get_rotor_points(algo, mdata, fdata))
```

### Comparing `foxes-0.3.5/foxes/core/states.py` & `foxes-0.4.0/foxes/core/states.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     """
     Abstract base class for states.
 
     States describe ambient meteorological data,
     typically wind speed, wind direction, turbulence
     intensity and air density.
 
+    :group: core
+
     """
 
     @abstractmethod
     def size(self):
         """
         The total number of states.
 
@@ -29,50 +31,50 @@
 
     def index(self):
         """
         The index list
 
         Returns
         -------
-        indices : array_like
+        indices: array_like
             The index labels of states, or None for default integers
 
         """
         return list(range(self.size()))
 
     @abstractmethod
     def weights(self, algo):
         """
         The statistical weights of all states.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        weights : numpy.ndarray
+        weights: numpy.ndarray
             The weights, shape: (n_states, n_turbines)
 
         """
         pass
 
     def _update_idata(self, algo, idata):
         """
         Add basic states data to idata.
 
         This function should be called within initialize,
         after loading the data.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         sinds = self.index()
         if sinds is not None:
@@ -93,20 +95,20 @@
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return [FV.WS, FV.WD, FV.TI, FV.RHO]
 
     def __add__(self, s):
         if isinstance(s, list):
@@ -121,42 +123,48 @@
             return ExtendedStates(self, [s])
 
 
 class ExtendedStates(States):
     """
     States extended by point data models.
 
-    Parameters
-    ----------
-    states : foxes.core.States
-        The base states to start from
-    point_models : list of foxes.core.PointDataModel, optional
-        The point models, executed after states
-
     Attributes
     ----------
-    states : foxes.core.States
+    states: foxes.core.States
         The base states to start from
-    pmodels : foxes.core.PointDataModelList
+    pmodels: foxes.core.PointDataModelList
         The point models, including states as first model
+    
+    :group: core
 
     """
 
     def __init__(self, states, point_models=[]):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        states: foxes.core.States
+            The base states to start from
+        point_models: list of foxes.core.PointDataModel, optional
+            The point models, executed after states
+
+        """
         super().__init__()
         self.states = states
         self.pmodels = PointDataModelList(models=[states] + point_models)
 
     def append(self, model):
         """
         Add a model to the list
 
         Parameters
         ----------
-        model : foxes.core.PointDataModel
+        model: foxes.core.PointDataModel
             The model to add
 
         """
         self.pmodels.append(model)
 
     def size(self):
         """
@@ -172,32 +180,32 @@
 
     def index(self):
         """
         The index list
 
         Returns
         -------
-        indices : array_like
+        indices: array_like
             The index labels of states, or None for default integers
 
         """
         return self.states.index()
 
     def weights(self, algo):
         """
         The statistical weights of all states.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        weights : numpy.ndarray
+        weights: numpy.ndarray
             The weights, shape: (n_states, n_turbines)
 
         """
         return self.states.weights(algo)
 
     def initialize(self, algo, verbosity=0):
         """
@@ -207,22 +215,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
         algo.update_idata(self.pmodels, idata=idata, verbosity=verbosity)
@@ -231,61 +239,61 @@
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return self.states.output_point_vars(algo)
 
     def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pdata : foxes.core.Data
+        pdata: foxes.core.Data
             The point data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         return self.pmodels.calculate(algo, mdata, fdata, pdata)
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level
 
         """
         self.pmodels.finalize(algo, verbosity)
         super().finalize(algo, verbosity)
 
     def __add__(self, m):
```

### Comparing `foxes-0.3.5/foxes/core/turbine.py` & `foxes-0.4.0/foxes/core/turbine.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,68 +4,74 @@
 class Turbine:
     """
     An individual wind turbine.
 
     The turbine is merely a defined by basic data
     entries and a choice of turbine models.
 
-    Parameters
-    ----------
-    xy : array_like
-        The turbine ground position, shape: (2,)
-    turbine_models : list of str
-        The turbine model names, as they appear
-        in the model book
-    index : int, optional
-        The index in the wind farm
-    name : str, optional
-        The turbine name/label
-    models_state_sel : list of numpy.ndarray, optional
-        For each turbine model, the state selection
-        boolean array with shape (n_states,)
-    D : float, optional
-        The rotor diameter. Overwrites turbine type
-        settings if given
-    H : float, optional
-        The hub height. Overwrites turbine type
-        settings if given
-
     Attributes
     ----------
-    xy : array_like
+    xy: array_like
         The turbine ground position, shape: (2,)
-    models : list of str
+    models: list of str
         The turbine model names, as they appear
         in the model book
-    index : int, optional
+    index: int, optional
         The index in the wind farm
-    name : str, optional
+    name: str, optional
         The turbine name/label
-    mstates_sel : list of numpy.ndarray, optional
+    mstates_sel: list of numpy.ndarray, optional
         For each turbine model, the state selection
         boolean array with shape (n_states,)
-    D : float, optional
+    D: float, optional
         The rotor diameter. Overwrites turbine type
         settings if given
-    H : float, optional
+    H: float, optional
         The hub height. Overwrites turbine type
         settings if given
 
+    :group: foxes
+    
     """
 
     def __init__(
         self,
         xy,
         turbine_models=[],
         index=None,
         name=None,
         models_state_sel=None,
         D=None,
         H=None,
     ):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        xy: array_like
+            The turbine ground position, shape: (2,)
+        turbine_models: list of str
+            The turbine model names, as they appear
+            in the model book
+        index: int, optional
+            The index in the wind farm
+        name: str, optional
+            The turbine name/label
+        models_state_sel: list of numpy.ndarray, optional
+            For each turbine model, the state selection
+            boolean array with shape (n_states,)
+        D: float, optional
+            The rotor diameter. Overwrites turbine type
+            settings if given
+        H: float, optional
+            The hub height. Overwrites turbine type
+            settings if given
+
+        """
         self.index = index
         self.name = name
         self.xy = np.array(xy)
         self.models = turbine_models
         self.D = D
         self.H = H
 
@@ -75,32 +81,32 @@
 
     def add_model(self, model, states_sel=None):
         """
         Add a turbine model to the list.
 
         Parameters
         ----------
-        model : foxes.core.TurbineModel
+        model: foxes.core.TurbineModel
             The model
-        states_sel : numpy.ndarray of bool, optional
+        states_sel: numpy.ndarray of bool, optional
             The states selection for the model, shape: (n_states,)
 
         """
         self.models.append(model)
         self.mstates_sel.append(states_sel)
 
     def insert_model(self, index, model, states_sel=None):
         """
         Insert a turbine model into the list of models.
 
         Parameters
         ----------
-        index : int
+        index: int
             The position in the model list
-        model : foxes.core.TurbineModel
+        model: foxes.core.TurbineModel
             The model
-        states_sel : numpy.ndarray of bool, optional
+        states_sel: numpy.ndarray of bool, optional
             The states selection for the model, shape: (n_states,)
 
         """
         self.models.insert(index, model)
         self.mstates_sel.insert(index, states_sel)
```

### Comparing `foxes-0.3.5/foxes/core/turbine_model.py` & `foxes-0.4.0/foxes/core/turbine_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,37 +6,39 @@
 class TurbineModel(FarmDataModel):
     """
     Abstract base class for turbine models.
 
     Turbine models are FarmDataModels that run
     on a selection of turbines.
 
+    :group: core
+
     """
 
     @abstractmethod
     def calculate(self, algo, mdata, fdata, st_sel):
-        """ "
+        """
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         pass
```

### Comparing `foxes-0.3.5/foxes/core/turbine_type.py` & `foxes-0.4.0/foxes/core/turbine_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,44 +5,50 @@
 class TurbineType(TurbineModel):
     """
     Abstract base class for turbine type models.
 
     Rotor diameter and hub height can be overwritten
     by individual settings in the Turbine object.
 
-    Parameters
-    ----------
-    name : str, optional
-        The model name
-    D : float, optional
-        The rotor diameter
-    H : float, optional
-        The hub height
-    P_nominal : float, optional
-        The nominal power in kW
-    P_unit : str
-        The unit of power, choices:
-        W, kW, MW, GW
-
     Attributes
     ----------
-    name : str
+    name: str
         The model name
-    D : float
+    D: float
         The rotor diameter
-    H : float
+    H: float
         The hub height
-    P_nominal : float
+    P_nominal: float
         The nominal power in kW
-    P_unit : str
+    P_unit: str
         The unit of power
 
+    :group: core
+
     """
 
     def __init__(self, name=None, D=None, H=None, P_nominal=None, P_unit="kW"):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        name: str, optional
+            The model name
+        D: float, optional
+            The rotor diameter
+        H: float, optional
+            The hub height
+        P_nominal: float, optional
+            The nominal power in kW
+        P_unit: str
+            The unit of power, choices:
+            W, kW, MW, GW
+
+        """
         super().__init__()
 
         self.name = name if name is not None else type(self).__name__
         self.D = D
         self.H = H
         self.P_nominal = P_nominal
         self.P_unit = P_unit
```

### Comparing `foxes-0.3.5/foxes/core/vertical_profile.py` & `foxes-0.4.0/foxes/core/vertical_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,59 +3,62 @@
 from .model import Model
 from foxes.utils import all_subclasses
 
 
 class VerticalProfile(Model):
     """
     Abstract base class for vertical profiles.
+
+    :group: core
+    
     """
 
     @abstractmethod
     def input_vars(self):
         """
         The input variables needed for the profile
         calculation.
 
         Returns
         -------
-        vars : list of str
+        vars: list of str
             The variable names
 
         """
         return []
 
     @abstractmethod
     def calculate(self, data, heights):
         """
         Run the profile calculation.
 
         Parameters
         ----------
-        data : dict
+        data: dict
             The input data
-        heights : numpy.ndarray
+        heights: numpy.ndarray
             The evaluation heights
 
         Returns
         -------
-        results : numpy.ndarray
+        results: numpy.ndarray
             The profile results, same
             shape as heights
 
         """
         pass
 
     @classmethod
     def new(cls, profile_type, **kwargs):
         """
         Run-time profile factory.
 
         Parameters
         ----------
-        profile_type : str
+        profile_type: str
             The selected derived class name
 
         """
 
         if profile_type is None:
             return None
```

### Comparing `foxes-0.3.5/foxes/core/wake_frame.py` & `foxes-0.4.0/foxes/core/wake_frame.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,91 +14,93 @@
     Wake frames translate global coordinates into
     wake frame coordinates, which are then evaluated
     by wake models.
 
     They are also responsible for the calculation of
     the turbine evaluation order.
 
+    :group: core
+
     """
 
     @abstractmethod
     def calc_order(self, algo, mdata, fdata):
         """ "
         Calculates the order of turbine evaluation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        order : numpy.ndarray
+        order: numpy.ndarray
             The turbine order, shape: (n_states, n_turbines)
 
         """
         pass
 
     @abstractmethod
     def get_wake_coos(self, algo, mdata, fdata, states_source_turbine, points):
         """
         Calculate wake coordinates.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        points : numpy.ndarray
+        points: numpy.ndarray
             The evaluation points, shape: (n_states, n_points, 3)
 
         Returns
         -------
-        wake_coos : numpy.ndarray
+        wake_coos: numpy.ndarray
             The wake frame coordinates of the evaluation
             points, shape: (n_states, n_points, 3)
 
         """
         pass
 
     def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
         """
         Gets the points along the centreline for given
         values of x.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
 
         Returns
         -------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
 
         """
         raise NotImplementedError(
             f"Wake frame '{self.name}': Centreline points requested but not implemented."
         )
 
@@ -114,36 +116,36 @@
         **ipars,
     ):
         """
         Integrates variables along the centreline.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        variables : list of str
+        variables: list of str
             The variables to be integrated
-        x : numpy.ndarray
+        x: numpy.ndarray
             The wake frame x coordinates of the upper integral bounds,
             shape: (n_states, n_points)
-        dx : float
+        dx: float
             The step size of the integral
-        ipars : dict, optional
+        ipars: dict, optional
             Additional interpolation parameters
 
         Returns
         -------
-        results : numpy.ndarray
+        results: numpy.ndarray
             The integration results, shape: (n_states, n_points, n_vars)
 
         """
         # prepare:
         n_states, n_points = x.shape
         vrs = [FV.amb2var.get(v, v) for v in variables]
         n_vars = len(vrs)
```

### Comparing `foxes-0.3.5/foxes/core/wake_superposition.py` & `foxes-0.4.0/foxes/core/wake_superposition.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     """
     Abstract base class for wake superposition models.
 
     Note that it is a matter of the wake model
     if superposition models are used, or if the
     wake model computes the total wake result by
     other means.
+
+    :group: core
+    
     """
 
     @abstractmethod
     def calc_wakes_plus_wake(
         self,
         algo,
         mdata,
@@ -26,36 +29,36 @@
         wake_model_result,
     ):
         """
         Add a wake delta to previous wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        sel_sp : numpy.ndarray of bool
+        sel_sp: numpy.ndarray of bool
             The selection of points, shape: (n_states, n_points)
-        variable : str
+        variable: str
             The variable name for which the wake deltas applies
-        wake_delta : numpy.ndarray
+        wake_delta: numpy.ndarray
             The original wake deltas, shape: (n_states, n_points)
-        wake_model_result : numpy.ndarray
+        wake_model_result: numpy.ndarray
             The new wake deltas of the selected points,
             shape: (n_sel_sp,)
 
         Returns
         -------
-        wdelta : numpy.ndarray
+        wdelta: numpy.ndarray
             The updated wake deltas, shape: (n_states, n_points)
 
         """
         pass
 
     @abstractmethod
     def calc_final_wake_delta(
@@ -63,28 +66,28 @@
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        variable : str
+        variable: str
             The variable name for which the wake deltas applies
-        amb_results : numpy.ndarray
+        amb_results: numpy.ndarray
             The ambient results, shape: (n_states, n_points)
-        wake_delta : numpy.ndarray
+        wake_delta: numpy.ndarray
             The wake deltas, shape: (n_states, n_points)
 
         Returns
         -------
-        final_wake_delta : numpy.ndarray
+        final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
             results by simple plus operation. Shape: (n_states, n_points)
 
         """
         pass
```

### Comparing `foxes-0.3.5/foxes/core/wind_farm.py` & `foxes-0.4.0/foxes/core/wind_farm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 class WindFarm:
     """
     The wind farm.
 
-    Parameters
-    ----------
-    name : str
-        The wind farm name
-
     Attributes
     ----------
-    name : str
+    name: str
         The wind farm name
-    turbines : list of foxes.core.Turbine
+    turbines: list of foxes.core.Turbine
         The wind turbines
-    boundary : foxes.utils.geom2d.AreaGeometry, optional
+    boundary: foxes.utils.geom2d.AreaGeometry, optional
         The wind farm boundary
+    
+    :group: foxes
 
     """
 
     def __init__(self, name="wind_farm", boundary=None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        name: str
+            The wind farm name
+
+        """
         self.name = name
         self.turbines = []
         self.boundary = boundary
 
     def add_turbine(self, turbine, verbosity=1):
         """
         Add a wind turbine to the list.
 
         Parameters
         ----------
-        turbine : foxes.core.Turbine
+        turbine: foxes.core.Turbine
             The wind turbine
-        verbosity : int
+        verbosity: int
             The output verbosity, 0 = silent
 
         """
         if turbine.index is None:
             turbine.index = len(self.turbines)
         if turbine.name is None:
             turbine.name = f"T{turbine.index}"
@@ -48,25 +54,25 @@
     @property
     def n_turbines(self):
         """
         The number of turbines in the wind farm
 
         Returns
         -------
-        n_turbines : int
+        n_turbines: int
             The total number of turbines
 
         """
         return len(self.turbines)
 
     @property
     def turbine_names(self):
         """
         The list of names of all turbines
 
         Returns
         -------
-        names : list of str
+        names: list of str
             The names of all turbines
 
         """
         return [t.name for t in self.turbines]
```

### Comparing `foxes-0.3.5/foxes/data/farms/test_farm_67.csv` & `foxes-0.4.0/foxes/data/farms/test_farm_67.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/data/parse.py` & `foxes-0.4.0/foxes/data/parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,23 @@
     """
     Parse basic turbine data from file name
 
     Expected format: `[name]-[...]MW-D[...]-H[...].csv`
 
     Parameters
     ----------
-    file_name : str or pathlib.Path
+    file_name: str or pathlib.Path
         Path to the file
 
     Returns
     -------
-    parsed_data : dict
+    parsed_data: dict
         dict with data parsed from file name
+    
+    :group: foxes
 
     """
     sname = Path(file_name).stem
     pars = {"name": sname.split(".")[0]}
 
     i = sname.find(".")
     if i >= 0:
@@ -69,23 +71,25 @@
     """
     Parse basic turbine data from file names
 
     Expected format: `[name]-[...]MW-D[...]-H[...].csv`
 
     Parameters
     ----------
-    file_name_A : str or pathlib.Path
+    file_name_A: str or pathlib.Path
         Path to the first file
-    file_name_B : str or pathlib.Path
+    file_name_B: str or pathlib.Path
         Path to the second file
 
     Returns
     -------
-    parsed_data : dict
+    parsed_data: dict
         dict with data parsed from file name
+    
+    :group: foxes
 
     """
     pars_A = parse_Pct_file_name(file_name_A)
     pars_B = parse_Pct_file_name(file_name_B)
     name = pars_A["name"]
     name_ct = pars_B["name"]
     i = 0
```

### Comparing `foxes-0.3.5/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv` & `foxes-0.4.0/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/data/states/WRF-Timeseries-4464.csv.gz` & `foxes-0.4.0/foxes/data/states/WRF-Timeseries-4464.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/data/states/abl_states_6000.csv.gz` & `foxes-0.4.0/foxes/data/states/abl_states_6000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/data/states/timeseries_3000.csv.gz` & `foxes-0.4.0/foxes/data/states/timeseries_3000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/data/states/timeseries_8000.csv.gz` & `foxes-0.4.0/foxes/data/states/timeseries_8000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/data/states/wind_rose_bremen.csv` & `foxes-0.4.0/foxes/data/states/wind_rose_bremen.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/data/states/wind_rotation.nc` & `foxes-0.4.0/foxes/data/states/wind_rotation.nc`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/data/static_data.py` & `foxes-0.4.0/foxes/data/static_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 PCTCURVE = "power_ct_curve"
 
 
 class StaticData(DataBook):
     """
     A DataBook filled with static data from
     this directory.
+
+    :group: foxes
+    
     """
 
     def __init__(self):
         super().__init__()
 
         self.add_data_package(FARM, farms, ".csv")
         self.add_data_package(STATES, states, [".csv", ".csv.gz", ".nc"])
```

### Comparing `foxes-0.3.5/foxes/input/farm_layout/from_csv.py` & `foxes-0.4.0/foxes/input/farm_layout/from_csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,50 +22,52 @@
     **turbine_parameters,
 ):
     """
     Add turbines to wind farm via csv input file.
 
     Parameters
     ----------
-    farm : foxes.WindFarm
+    farm: foxes.WindFarm
         The wind farm
-    data_source : str or pandas.DataFrame
+    data_source: str or pandas.DataFrame
         The input csv file or data source
-    col_index : str, optional
+    col_index: str, optional
         The index column, or None
-    col_name : str, optional
+    col_name: str, optional
         The name column, or None
-    col_x : str, optional
+    col_x: str, optional
         The x column
-    col_y : str, optional
+    col_y: str, optional
         The y column
     col_H: str, optional
         The hub height column
-    col_D : str, optional
+    col_D: str, optional
         The rotor diameter column
-    col_id : str, optional
+    col_id: str, optional
         The id column
-    cols_models_pre : list of str, optional
+    cols_models_pre: list of str, optional
         The turbine model columns, entered before
         turbine_models
-    cols_models_post : list of str, optional
+    cols_models_post: list of str, optional
         The turbine model columns, entered after
         turbine_models
-    turbine_base_name : str, optional
+    turbine_base_name: str, optional
         The turbine base name, only used
         if col_name is None
-    turbine_ids : list, optional
+    turbine_ids: list, optional
         The turbine ids, or None for
         index
-    turbine_base_name_count_shift : bool, optional
+    turbine_base_name_count_shift: bool, optional
         Start turbine names by 1 instead of 0
-    verbosity : int
+    verbosity: int
         The verbosity level, 0 = silent
-    turbine_parameters : dict, optional
+    turbine_parameters: dict, optional
         Additional parameters are forwarded to the WindFarm.add_turbine().
+    
+    :group: input.farm_layout
 
     """
 
     if isinstance(data_source, pd.DataFrame):
         data = data_source
     else:
         if verbosity:
```

### Comparing `foxes-0.3.5/foxes/input/farm_layout/from_df.py` & `foxes-0.4.0/foxes/input/farm_layout/from_df.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,18 +8,20 @@
     **kwargs,
 ):
     """
     Add turbines to wind farm via pandas DataFrame.
 
     Parameters
     ----------
-    farm : foxes.WindFarm
+    farm: foxes.WindFarm
         The wind farm
-    data_source : str or pandas.DataFrame
+    data_source: str or pandas.DataFrame
         The input csv file or data source
-    args : tuple, optional
+    args: tuple, optional
         Additional parameters for add_from_csv()
-    kwargs : dict, optional
+    kwargs: dict, optional
         Additional parameters for add_from_csv()
+    
+    :group: input.farm_layout
 
     """
     add_from_csv(farm, data_source, *args, **kwargs)
```

### Comparing `foxes-0.3.5/foxes/input/farm_layout/from_file.py` & `foxes-0.4.0/foxes/input/farm_layout/from_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,28 +9,30 @@
     """
     Add turbines from file.
 
     The method is inferred according to the file suffix.
 
     Parameters
     ----------
-    farm : foxes.WindFarm
+    farm: foxes.WindFarm
         The wind farm
-    file_path : str
+    file_path: str
         Path to the file
     verbosity
-    args : tuple, optional
+    args: tuple, optional
         Parameters forwarded to the method
-    verbosity : int
+    verbosity: int
         The verbosity level, 0 = silent
-    dbook : foxes.DataBook, optional
+    dbook: foxes.DataBook, optional
         The data book, or None for default
-    kwargs : dict, optional
+    kwargs: dict, optional
         Parameters forwarded to the method
 
+    :group: input.farm_layout
+
     """
 
     fpath = Path(file_path)
     dbook = StaticData() if dbook is None else dbook
 
     if not fpath.is_file():
         if verbosity:
```

### Comparing `foxes-0.3.5/foxes/input/farm_layout/from_json.py` & `foxes-0.4.0/foxes/input/farm_layout/from_json.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,24 +9,26 @@
     farm, file_path, set_farm_name=True, verbosity=1, **turbine_parameters
 ):
     """
     Add turbimes from a json file.
 
     Parameters
     ----------
-    farm : foxes.WindFarm
+    farm: foxes.WindFarm
         The wind farm
-    file_path : str
+    file_path: str
         Path to the file
-    set_farm_name : bool
+    set_farm_name: bool
         Flag for inferring wind farm name from data
-    verbosity : int
+    verbosity: int
         The verbosity level, 0 = silent
-    **turbine_parameters : dict, optional
+    turbine_parameters: dict, optional
         Parameters forwarded to `foxes.core.Turbine`
+    
+    :group: input.farm_layout
 
     """
 
     if verbosity:
         print("Reading file", file_path)
     with open(file_path) as f:
         dict = json.load(f)
```

### Comparing `foxes-0.3.5/foxes/input/farm_layout/grid.py` & `foxes-0.4.0/foxes/input/farm_layout/grid.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,31 +15,33 @@
     **turbine_parameters
 ):
     """
     Add a regular grid of turbines.
 
     Parameters
     ----------
-    farm : foxes.WindFarm
+    farm: foxes.WindFarm
         The wind farm
-    xy_base : numpy.ndarray
+    xy_base: numpy.ndarray
         The base point, shape: (2,)
-    step_vectors : numpy.ndarray
+    step_vectors: numpy.ndarray
         The two step vectors in x and y,
         respectively, shape: (2, 2)
-    steps : array_like of int
+    steps: array_like of int
         The steps in x, y. Length 2
-    indices : list of int, optional
+    indices: list of int, optional
         The turbine indices
-    names : list of str, optional
+    names: list of str, optional
         The turbine names
-    verbosity : int
+    verbosity: int
         The verbosity level, 0 = silent
-    **turbine_parameters : dict, optional
+    turbine_parameters: dict, optional
         Parameters forwarded to `foxes.core.Turbine`
+    
+    :group: input.farm_layout
 
     """
 
     inds = list(np.ndindex(*steps))
     n_turbines = len(inds)
 
     xy_base = np.array(xy_base, dtype=FC.DTYPE)
```

### Comparing `foxes-0.3.5/foxes/input/farm_layout/row.py` & `foxes-0.4.0/foxes/input/farm_layout/row.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,31 +14,33 @@
     **turbine_parameters
 ):
     """
     Add a single row of turbines.
 
     Parameters
     ----------
-    farm : foxes.WindFarm
+    farm: foxes.WindFarm
         The wind farm
-    xy_base : numpy.ndarray
+    xy_base: numpy.ndarray
         The base point, shape: (2,)
-    xy_step : numpy.ndarray
+    xy_step: numpy.ndarray
         The step vector, shape: (2,)
-    n_turbines : int
+    n_turbines: int
         The number of turbines
-    indices : list of int, optional
+    indices: list of int, optional
         The turbine indices
-    names : list of str, optional
+    names: list of str, optional
         The turbine names
-    verbosity : int
+    verbosity: int
         The verbosity level, 0 = silent
-    **turbine_parameters : dict, optional
+    turbine_parameters: dict, optional
         Parameters forwarded to `foxes.core.Turbine`
 
+    :group: input.farm_layout
+
     """
     p0 = np.array(xy_base)
     delta = np.array(xy_step)
 
     for i in range(n_turbines):
         farm.add_turbine(
             Turbine(
```

### Comparing `foxes-0.3.5/foxes/input/states/create/random_abl_states.py` & `foxes-0.4.0/foxes/input/states/create/random_abl_states.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,35 +7,37 @@
 
 def create_random_abl_states(
     n_states, cols_minmax, var2col={}, mol_abs_range=(50.0, 5000.0), normalize=True
 ):
     """
     Create random abl states.
 
-    Parameters
+        Parameters
     ----------
-    n_states : int
+    n_states: int
         The number of states
-    cols_minmax : dict
+    cols_minmax: dict
         For each variable the min and max values,
         keys: variable name str, values: array_like
         with length 2
-    var2col : dict, optional
+    var2col: dict, optional
         Mapping from variables to column names
-    mol_abs_range : tuple
+    mol_abs_range: tuple
         Min and max of allowed MOL values, set to
         nan if exceeded (i.e., neutral stratification)
-    normalize : bool
+    normalize: bool
         Normalize weights to 1
-
+        
     Returns
     -------
-    data : pandas.DataFrame
+    data: pandas.DataFrame
         The created states data
 
+    :group: input.states
+
     """
 
     data = pd.DataFrame(index=range(n_states))
     data.index.name = FC.STATE
 
     for v, mm in cols_minmax.items():
         data[v] = np.random.uniform(low=mm[0], high=mm[1], size=(n_states,)).astype(
@@ -64,34 +66,34 @@
     mol_abs_range=(50.0, 5000.0),
     normalize=True,
     verbosity=1,
     digits="auto",
     **kwargs
 ):
     """
-    file_path : str
+    file_path: str
         Path to the file
-    n_states : int
+    n_states: int
         The number of states
-    cols_minmax : dict
+    cols_minmax: dict
         For each variable the min and max values,
         keys: variable name str, values: array_like
         with length 2
-    var2col : dict, optional
+    var2col: dict, optional
         Mapping from variables to column names
-    mol_abs_range : tuple
+    mol_abs_range: tuple
         Min and max of allowed MOL values, set to
         nan if exceeded (i.e., neutral stratification)
-    normalize : bool
+    normalize: bool
         Normalize weights to 1
-    verbosity : int
+    verbosity: int
         The verbosity level, 0 = silent
-    digits : int or auto
+    digits: int or auto
         The number of digits to be written
-    kwargs : dict, optional
+    kwargs: dict, optional
         Parameters for `pandas.DataFrame.to_csv`
 
     """
 
     if verbosity:
         print("Writing file", file_path)
```

### Comparing `foxes-0.3.5/foxes/input/states/field_data_nc.py` & `foxes-0.4.0/foxes/input/states/field_data_nc.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,86 +13,51 @@
 
 
 class FieldDataNC(States):
     """
     Heterogeneous ambient states on a regular
     horizontal grid in NetCDF format.
 
-    Parameters
-    ----------
-    data_source : str or xarray.Dataset
-        The data or the file search pattern, should end with
-        suffix '.nc'. One or many files.
-    output_vars : list of str
-        The output variables
-    var2ncvar : dict, optional
-        Mapping from variable names to variable names
-        in the nc file
-    fixed_vars : dict, optional
-        Uniform values for output variables, instead
-        of reading from data
-    states_coord : str
-        The states coordinate name in the data
-    x_coord : str
-        The x coordinate name in the data
-    y_coord : str
-        The y coordinate name in the data
-    h_coord : str
-        The height coordinate name in the data
-    pre_load : bool
-        Flag for loading all data into memory during
-        initialization
-    weight_ncvar : str, optional
-        Name of the weight data variable in the nc file(s)
-    bounds_error : bool
-        Flag for raising errors if bounds are exceeded
-    fill_value : number, optional
-        Fill value in case of exceeding bounds, if no bounds error
-    time_format : str
-        The datetime parsing format string
-    sel : dict, optional
-        Subset selection via xr.Dataset.sel()
-    verbosity : int
-        Verbosity level for pre_load file reading
-
     Attributes
     ----------
-    data_source : str or xarray.Dataset
+    data_source: str or xarray.Dataset
         The data or the file search pattern, should end with
         suffix '.nc'. One or many files.
-    ovars : list of str
+    ovars: list of str
         The output variables
-    var2ncvar : dict
+    var2ncvar: dict
         Mapping from variable names to variable names
         in the nc file
-    fixed_vars : dict
+    fixed_vars: dict
         Uniform values for output variables, instead
         of reading from data
-    states_coord : str
+    states_coord: str
         The states coordinate name in the data
-    x_coord : str
+    x_coord: str
         The x coordinate name in the data
-    y_coord : str
+    y_coord: str
         The y coordinate name in the data
-    h_coord : str
+    h_coord: str
         The height coordinate name in the data
-    pre_load : bool
+    pre_load: bool
         Flag for loading all data into memory during
         initialization
-    weight_ncvar : str
+    weight_ncvar: str
         Name of the weight data variable in the nc file(s)
-    bounds_error : bool
+    bounds_error: bool
         Flag for raising errors if bounds are exceeded
-    fill_value : number
+    fill_value: number
         Fill value in case of exceeding bounds, if no bounds error
-    time_format : str
+    time_format: str
         The datetime parsing format string
-    sel : dict
+    sel: dict
         Subset selection via xr.Dataset.sel()
 
+    :group: input.states
+
     """
 
     def __init__(
         self,
         data_source,
         output_vars,
         var2ncvar={},
@@ -105,14 +70,55 @@
         weight_ncvar=None,
         bounds_error=True,
         fill_value=None,
         time_format="%Y-%m-%d_%H:%M:%S",
         sel=None,
         verbosity=1,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        data_source: str or xarray.Dataset
+            The data or the file search pattern, should end with
+            suffix '.nc'. One or many files.
+        output_vars: list of str
+            The output variables
+        var2ncvar: dict, optional
+            Mapping from variable names to variable names
+            in the nc file
+        fixed_vars: dict, optional
+            Uniform values for output variables, instead
+            of reading from data
+        states_coord: str
+            The states coordinate name in the data
+        x_coord: str
+            The x coordinate name in the data
+        y_coord: str
+            The y coordinate name in the data
+        h_coord: str
+            The height coordinate name in the data
+        pre_load: bool
+            Flag for loading all data into memory during
+            initialization
+        weight_ncvar: str, optional
+            Name of the weight data variable in the nc file(s)
+        bounds_error: bool
+            Flag for raising errors if bounds are exceeded
+        fill_value: number, optional
+            Fill value in case of exceeding bounds, if no bounds error
+        time_format: str
+            The datetime parsing format string
+        sel: dict, optional
+            Subset selection via xr.Dataset.sel()
+        verbosity: int
+            Verbosity level for pre_load file reading
+
+        """
         super().__init__()
 
         self.data_source = data_source
         self.states_coord = states_coord
         self.ovars = output_vars
         self.fixed_vars = fixed_vars
         self.x_coord = x_coord
@@ -266,22 +272,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
 
         if (FV.WS in self.ovars and FV.WD not in self.ovars) or (
@@ -349,75 +355,75 @@
 
     def index(self):
         """
         The index list
 
         Returns
         -------
-        indices : array_like
+        indices: array_like
             The index labels of states, or None for default integers
 
         """
         return self._inds
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return self.ovars
 
     def weights(self, algo):
         """
         The statistical weights of all states.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        weights : numpy.ndarray
+        weights: numpy.ndarray
             The weights, shape: (n_states, n_turbines)
 
         """
         return self._weights
 
     def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pdata : foxes.core.Data
+        pdata: foxes.core.Data
             The point data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         # prepare:
         points = pdata[FC.POINTS]
         n_pts = points.shape[1]
@@ -466,15 +472,15 @@
         iterp = RegularGridInterpolator(
             gvars, data, bounds_error=self.bounds_error, fill_value=self.fill_value
         )
         try:
             data = iterp(pts).reshape(n_states, n_pts, self._n_dvars)
         except ValueError as e:
             print(f"\n\nStates '{self.name}': Interpolation error")
-            print("INPUT VARS : (state, heights, y, x)")
+            print("INPUT VARS: (state, heights, y, x)")
             print(
                 "DATA BOUNDS:", [np.min(d) for d in gvars], [np.max(d) for d in gvars]
             )
             print(
                 "EVAL BOUNDS:", [np.min(p) for p in pts.T], [np.max(p) for p in pts.T]
             )
             raise e
```

### Comparing `foxes-0.3.5/foxes/input/states/multi_height.py` & `foxes-0.4.0/foxes/input/states/multi_height.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,57 +18,37 @@
     The input data is taken from a csv file or
     pandas data frame with columns. The format
     of the data columns is as in the following
     example for wind speed at heights 50, 60, 100 m:
 
     WS-50, WS-60, WS-100, ...
 
-    Parameters
-    ----------
-    data_source : str or pandas.DataFrame
-        Either path to a file or data
-    output_vars : list of str
-        The output variables
-    heights : list of float
-        The heights at which to search data
-    var2col : dict, optional
-        Mapping from variable names to data column names
-    fixed_vars : dict, optional
-        Fixed uniform variable values, instead of
-        reading from data
-    pd_read_pars : dict, optional
-        pandas file reading parameters
-    states_sel : slice or range or list of int, optional
-        States subset selection
-    states_loc : list, optional
-        State index selection via pandas loc function
-    ipars : dict, optional
-        Parameters for scipy.interpolate.interp1d
-
     Attributes
     ----------
-    data_source : str or pandas.DataFrame
+    data_source: str or pandas.DataFrame
         Either path to a file or data
-    ovars : list of str
+    ovars: list of str
         The output variables
-    heights : list of float
+    heights: list of float
         The heights at which to search data
-    var2col : dict, optional
+    var2col: dict, optional
         Mapping from variable names to data column names
-    fixed_vars : dict, optional
+    fixed_vars: dict, optional
         Fixed uniform variable values, instead of
         reading from data
-    pd_read_pars : dict, optional
+    pd_read_pars: dict, optional
         pandas file reading parameters
-    states_sel : slice or range or list of int
+    states_sel: slice or range or list of int
         States subset selection
-    states_loc : list
+    states_loc: list
         State index selection via pandas loc function
-    RDICT : dict
+    RDICT: dict
         Default pandas file reading parameters
+    
+    :group: input.states
 
     """
 
     RDICT = {"index_col": 0}
 
     def __init__(
         self,
@@ -78,14 +58,40 @@
         var2col={},
         fixed_vars={},
         pd_read_pars={},
         states_sel=None,
         states_loc=None,
         ipars={},
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        data_source: str or pandas.DataFrame
+            Either path to a file or data
+        output_vars: list of str
+            The output variables
+        heights: list of float
+            The heights at which to search data
+        var2col: dict, optional
+            Mapping from variable names to data column names
+        fixed_vars: dict, optional
+            Fixed uniform variable values, instead of
+            reading from data
+        pd_read_pars: dict, optional
+            pandas file reading parameters
+        states_sel: slice or range or list of int, optional
+            States subset selection
+        states_loc: list, optional
+            State index selection via pandas loc function
+        ipars: dict, optional
+            Parameters for scipy.interpolate.interp1d
+
+        """
         super().__init__()
 
         self.data_source = data_source
         self.ovars = output_vars
         self.heights = np.array(heights, dtype=FC.DTYPE)
         self.rpars = pd_read_pars
         self.var2col = var2col
@@ -101,19 +107,19 @@
 
     def reset(self, algo=None, states_sel=None, states_loc=None, verbosity=0):
         """
         Reset the states, optionally select states
 
         Parameters
         ----------
-        states_sel : slice or range or list of int, optional
+        states_sel: slice or range or list of int, optional
             States subset selection
-        states_loc : list, optional
+        states_loc: list, optional
             State index selection via pandas loc function
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         if self.initialized:
             if algo is None:
                 raise KeyError(f"{self.name}: Missing algo for reset")
             elif algo.states is not self:
@@ -153,22 +159,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         if not isinstance(self.data_source, pd.DataFrame):
             if not Path(self.data_source).is_file():
@@ -261,75 +267,75 @@
 
     def index(self):
         """
         The index list
 
         Returns
         -------
-        indices : array_like
+        indices: array_like
             The index labels of states, or None for default integers
 
         """
         return self._inds
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return self.ovars
 
     def weights(self, algo):
         """
         The statistical weights of all states.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        weights : numpy.ndarray
+        weights: numpy.ndarray
             The weights, shape: (n_states, n_turbines)
 
         """
         return self._weights
 
     def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pdata : foxes.core.Data
+        pdata: foxes.core.Data
             The point data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         h = mdata[self.H]
         z = pdata[FC.POINTS][:, :, 2]
         n_h = len(h)
@@ -384,26 +390,28 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level
 
         """
         self._cmap = None
         self._solo = None
         self._weights = None
         self._N = None
         super().finalize(algo, verbosity)
 
 
 class MultiHeightTimeseries(MultiHeightStates):
     """
     Multi-height timeseries states data.
-    """
 
+    :group: input.states
+
+    """
     RDICT = {"index_col": 0, "parse_dates": [0]}
```

### Comparing `foxes-0.3.5/foxes/input/states/scan_ws.py` & `foxes-0.4.0/foxes/input/states/scan_ws.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,35 +7,41 @@
 
 class ScanWS(States):
     """
     A given list of wind speeds, all other variables are fixed.
 
     Parameters
     ----------
-    ws_list : array_like
-        The wind speed values
-    wd : float
+    wd: float
         The wind direction
-    ti : float, optional
+    ti: float
         The TI value
-    rho : float, optional
-        The air density
-
-    Parameters
-    ----------
-    wd : float
-        The wind direction
-    ti : float
-        The TI value
-    rho : float
+    rho: float
         The air density
+    
+    :group: input.states
 
     """
 
     def __init__(self, ws_list, wd, ti=None, rho=None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        ws_list: array_like
+            The wind speed values
+        wd: float
+            The wind direction
+        ti: float, optional
+            The TI value
+        rho: float, optional
+            The air density
+
+        """
         super().__init__()
 
         self._wsl = np.array(ws_list)
         self.N = len(ws_list)
         self.wd = wd
         self.ti = ti
         self.rho = rho
@@ -48,22 +54,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.WS = self.var(FV.WS)
 
@@ -87,20 +93,20 @@
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         pvars = [FV.WS]
         if self.wd is not None:
             pvars.append(FV.WD)
         if self.ti is not None:
@@ -111,46 +117,46 @@
 
     def weights(self, algo):
         """
         The statistical weights of all states.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        weights : numpy.ndarray
+        weights: numpy.ndarray
             The weights, shape: (n_states, n_turbines)
 
         """
         return np.full((self.N, algo.n_turbines), 1.0 / self.N, dtype=FC.DTYPE)
 
     def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pdata : foxes.core.Data
+        pdata: foxes.core.Data
             The point data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         pdata[FV.WS][:] = mdata[self.WS][:, None]
 
         if self.wd is not None:
```

### Comparing `foxes-0.3.5/foxes/input/states/single.py` & `foxes-0.4.0/foxes/input/states/single.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,49 +5,55 @@
 import foxes.constants as FC
 
 
 class SingleStateStates(States):
     """
     A single uniform state.
 
-    Parameters
-    ----------
-    ws : float
-        The wind speed
-    wd : float
-        The wind direction
-    ti : float, optional
-        The TI value
-    rho : float, optional
-        The air density
-    profiles : dict, optional
-        Key: output variable name str, Value: str or dict
-        or `foxes.core.VerticalProfile`
-    profdata : dict, optional
-        Additional data for profiles
-
     Attributes
     ----------
-    ws : float
+    ws: float
         The wind speed
-    wd : float
+    wd: float
         The wind direction
-    ti : float
+    ti: float
         The TI value
-    rho : float
+    rho: float
         The air density
-    profdicts : dict
+    profdicts: dict
         Key: output variable name str, Value: str or dict
         or `foxes.core.VerticalProfile`
-    profdata : dict,
+    profdata: dict,
         Additional data for profiles
 
+    :group: input.states
+
     """
 
     def __init__(self, ws, wd, ti=None, rho=None, profiles={}, **profdata):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        ws: float
+            The wind speed
+        wd: float
+            The wind direction
+        ti: float, optional
+            The TI value
+        rho: float, optional
+            The air density
+        profiles: dict, optional
+            Key: output variable name str, Value: str or dict
+            or `foxes.core.VerticalProfile`
+        profdata: dict, optional
+            Additional data for profiles
+
+        """
         super().__init__()
         self.ws = ws
         self.wd = wd
         self.ti = ti
         self.rho = rho
         self.profdicts = profiles
         self.profdata = profdata
@@ -60,22 +66,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self._profiles = {}
         for v, d in self.profdicts.items():
@@ -110,20 +116,20 @@
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         out = []
         if self.ws is not None:
             out.append(FV.WS)
         if self.wd is not None:
@@ -136,46 +142,46 @@
 
     def weights(self, algo):
         """
         The statistical weights of all states.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        weights : numpy.ndarray
+        weights: numpy.ndarray
             The weights, shape: (n_states, n_turbines)
 
         """
         return np.ones((1, algo.n_turbines), dtype=FC.DTYPE)
 
     def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pdata : foxes.core.Data
+        pdata: foxes.core.Data
             The point data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
 
         if self.ws is not None:
             pdata[FV.WS] = np.full(
```

### Comparing `foxes-0.3.5/foxes/input/states/states_table.py` & `foxes-0.4.0/foxes/input/states/states_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,57 +9,38 @@
 import foxes.constants as FC
 
 
 class StatesTable(States):
     """
     States from a `pandas.DataFrame` or a pandas readable file.
 
-    Parameters
-    ----------
-    data_source : str or pandas.DataFrame
-        Either path to a file or data
-    output_vars : list of str
-        The output variables
-    var2col : dict
-        Mapping from variable names to data column names
-    fixed_vars : dict
-        Fixed uniform variable values, instead of
-        reading from data
-    profiles : dict
-        Key: output variable name str, Value: str or dict
-        or `foxes.core.VerticalProfile`
-    pd_read_pars : dict
-        pandas file reading parameters
-    states_sel : slice or range or list of int, optional
-        States subset selection
-    states_loc : list, optional
-        State index selection via pandas loc function
-
     Attributes
     ----------
-    data_source : str or pandas.DataFrame
+    data_source: str or pandas.DataFrame
         Either path to a file or data
-    ovars : list of str
+    ovars: list of str
         The output variables
-    var2col : dict
+    var2col: dict
         Mapping from variable names to data column names
-    fixed_vars : dict
+    fixed_vars: dict
         Fixed uniform variable values, instead of
         reading from data
-    profdicts : dict
+    profdicts: dict
         Key: output variable name str, Value: str or dict
         or `foxes.core.VerticalProfile`
-    rpars : dict
+    rpars: dict
         pandas file reading parameters
-    states_sel : slice or range or list of int
+    states_sel: slice or range or list of int
         States subset selection
-    states_loc : list
+    states_loc: list
         State index selection via pandas loc function
-    RDICT : dict
+    RDICT: dict
         Default pandas file reading parameters
+    
+    :group: input.states
 
     """
 
     RDICT = {"index_col": 0}
 
     def __init__(
         self,
@@ -68,14 +49,39 @@
         var2col={},
         fixed_vars={},
         profiles={},
         pd_read_pars={},
         states_sel=None,
         states_loc=None,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        data_source: str or pandas.DataFrame
+            Either path to a file or data
+        output_vars: list of str
+            The output variables
+        var2col: dict
+            Mapping from variable names to data column names
+        fixed_vars: dict
+            Fixed uniform variable values, instead of
+            reading from data
+        profiles: dict
+            Key: output variable name str, Value: str or dict
+            or `foxes.core.VerticalProfile`
+        pd_read_pars: dict
+            pandas file reading parameters
+        states_sel: slice or range or list of int, optional
+            States subset selection
+        states_loc: list, optional
+            State index selection via pandas loc function
+
+        """
         super().__init__()
 
         self.data_source = data_source
         self.ovars = output_vars
         self.rpars = pd_read_pars
         self.var2col = var2col
         self.fixed_vars = fixed_vars
@@ -94,19 +100,19 @@
 
     def reset(self, algo=None, states_sel=None, states_loc=None, verbosity=0):
         """
         Reset the states, optionally select states
 
         Parameters
         ----------
-        states_sel : slice or range or list of int, optional
+        states_sel: slice or range or list of int, optional
             States subset selection
-        states_loc : list, optional
+        states_loc: list, optional
             State index selection via pandas loc function
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         if self.initialized:
             if algo is None:
                 raise KeyError(f"{self.name}: Missing algo for reset")
             elif algo.states is not self:
@@ -123,22 +129,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.VARS = self.var("vars")
         self.DATA = self.var("data")
@@ -238,75 +244,75 @@
 
     def index(self):
         """
         The index list
 
         Returns
         -------
-        indices : array_like
+        indices: array_like
             The index labels of states, or None for default integers
 
         """
         return self._inds
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return self.ovars
 
     def weights(self, algo):
         """
         The statistical weights of all states.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        weights : numpy.ndarray
+        weights: numpy.ndarray
             The weights, shape: (n_states, n_turbines)
 
         """
         return self._weights
 
     def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pdata : foxes.core.Data
+        pdata: foxes.core.Data
             The point data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         z = pdata[FC.POINTS][:, :, 2]
 
         for i, v in enumerate(self._tvars):
@@ -323,26 +329,28 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level
 
         """
         self._weights = None
         self._N = None
         self._tvars = None
 
         super().finalize(algo, verbosity)
 
 
 class Timeseries(StatesTable):
     """
     Timeseries states data.
-    """
 
+    :group: input.states
+    
+    """
     RDICT = {"index_col": 0, "parse_dates": [0]}
```

### Comparing `foxes-0.3.5/foxes/input/windio/windio.py` & `foxes-0.4.0/foxes/input/windio/windio.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 
 def read_resource(res_yaml, fixed_vars={}, **kwargs):
     """
     Reads a WindIO energy resource
 
     Parameters
     ----------
-    res_yaml : str
+    res_yaml: str
         Path to the yaml file
-    fixed_vars : dict
+    fixed_vars: dict
         Additional fixes variables that do
         not occur in the yaml
-    kwargs : dict, optional
+    kwargs: dict, optional
         Additional arguments for StatesTable
 
     Returns
     -------
     states: foxes.states.StatesTable
         The uniform states
 
@@ -102,22 +102,22 @@
 
 def read_site(site_yaml, **kwargs):
     """
     Reads a WindIO site
 
     Parameters
     ----------
-    site_yaml : str
+    site_yaml: str
         Path to the yaml file
-    kwargs : dict, optional
+    kwargs: dict, optional
         Additional arguments for read_resource
 
     Returns
     -------
-    states : foxes.states.States
+    states: foxes.states.States
         The states object
 
     """
     site_yaml = Path(site_yaml)
 
     with open(site_yaml, "r") as file:
         site = yaml.load(file, Loader=yaml.loader.BaseLoader)
@@ -132,30 +132,30 @@
 
 def read_farm(farm_yaml, mbook=None, layout=-1, turbine_models=[], **kwargs):
     """
     Reads a WindIO wind farm
 
     Parameters
     ----------
-    farm_yaml : str
+    farm_yaml: str
         Path to the yaml file
-    mbook : foxes.ModelBook, optional
+    mbook: foxes.ModelBook, optional
         The model book to start from
-    layout : str or int
+    layout: str or int
         The layout choice
-    turbine_models : list of str
+    turbine_models: list of str
         Additional turbine models
-    kwargs : dict, optional
+    kwargs: dict, optional
         Additional parameters for add_from_df()
 
     Returns
     -------
-    mbook : foxes.ModelBook
+    mbook: foxes.ModelBook
         The model book
-    farm : foxes.WindFarm
+    farm: foxes.WindFarm
         The wind farm
 
     """
     mbook = ModelBook() if mbook is None else mbook
     farm_yaml = Path(farm_yaml)
 
     with open(farm_yaml, "r") as file:
@@ -217,33 +217,33 @@
     analyses, mbook, farm, states, keymap={}, algo_type="Downwind", **algo_pars
 ):
     """
     Reads a WindIO wind farm
 
     Parameters
     ----------
-    analyses : dict
+    analyses: dict
         The analyses sub-dict of the case
-    mbook : foxes.ModelBook
+    mbook: foxes.ModelBook
         The model book
-    farm : foxes.WindFarm
+    farm: foxes.WindFarm
         The wind farm
-    states : foxes.states.States
+    states: foxes.states.States
         The states object
-    keymap : dict
+    keymap: dict
         Translation from windio to foxes keywords
-    algo_type : str
+    algo_type: str
         The default algorithm class name
-    algo_pars : dict, optional
+    algo_pars: dict, optional
         Additional parameters for the algorithm
         constructor
 
     Returns
     -------
-    algo : foxes.core.Algorithm
+    algo: foxes.core.Algorithm
         The algorithm
 
     """
     wmodel = analyses["wake_model"]["name"]
     wmodels = [keymap.get(wmodel, wmodel)]
 
     return Algorithm.new(
@@ -253,33 +253,35 @@
 
 def read_case(case_yaml, site_pars={}, farm_pars={}, ana_pars={}):
     """
     Reads a WindIO case
 
     Parameters
     ----------
-    case_yaml : str
+    case_yaml: str
         Path to the yaml file
-    site_pars : dict
+    site_pars: dict
         Additional arguments for read_site
-    farm_pars : dict
+    farm_pars: dict
         Additional arguments for read_farm
-    ana_pars : dict
+    ana_pars: dict
         Additional arguments for read_analyses
 
     Returns
     -------
-    mbook : foxes.ModelBook
+    mbook: foxes.ModelBook
         The model book
-    farm : foxes.WindFarm
+    farm: foxes.WindFarm
         The wind farm
-    states : foxes.states.States
+    states: foxes.states.States
         The states object
-    algo : foxes.core.Algorithm
+    algo: foxes.core.Algorithm
         The algorithm
+    
+    :group: input.windio
 
     """
     case_yaml = Path(case_yaml)
 
     with open(case_yaml, "r") as file:
         case = yaml.load(file, Loader=yaml.loader.BaseLoader)
```

### Comparing `foxes-0.3.5/foxes/models/farm_models/turbine2farm.py` & `foxes-0.4.0/foxes/models/farm_models/turbine2farm.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,27 +5,33 @@
 
 class Turbine2FarmModel(FarmModel):
     """
     Wrapper that promotes turbine models
     into farm models, simply by selecting
     all turbines.
 
-    Parameters
-    ----------
-    turbine_model : foxes.core.TurbineModel
-        The turbine model
-
     Attributes
     ----------
-    turbine_model : foxes.core.TurbineModel
+    turbine_model: foxes.core.TurbineModel
         The turbine model
+    
+    :group: models.farm_models
 
     """
 
     def __init__(self, turbine_model):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        turbine_model: foxes.core.TurbineModel
+            The turbine model
+
+        """
         super().__init__()
         self.turbine_model = turbine_model
 
     def __repr__(self):
         return f"{type(self).__name__}({self.turbine_model})"
 
     def initialize(self, algo, verbosity=0):
@@ -36,22 +42,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
         algo.update_idata(self.turbine_model, idata=idata, verbosity=verbosity)
@@ -60,61 +66,61 @@
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return self.turbine_model.output_farm_vars(algo)
 
     def calculate(self, algo, mdata, fdata, **parameters):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        **parameters : dict, optional
+        **parameters: dict, optional
             Init parameters forwarded to the turbine model
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         s = np.ones((algo.n_states, algo.n_turbines), dtype=bool)
         return self.turbine_model.calculate(algo, mdata, fdata, st_sel=s, **parameters)
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level
 
         """
         if self.turbine_model.initialized:
             algo.finalize_model(self.turbine_model, verbosity)
         super().finalize(algo, verbosity)
```

### Comparing `foxes-0.3.5/foxes/models/model_book.py` & `foxes-0.4.0/foxes/models/model_book.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import numpy as np
-
 import foxes.models as fm
 import foxes.variables as FV
 from foxes.utils import Dict
 from foxes.core import (
     TurbineModel,
     RotorModel,
     FarmModel,
@@ -12,61 +10,66 @@
 )
 
 
 class ModelBook:
     """
     Container for all kinds of models.
 
-    Parameters
-    ----------
-    Pct_file : str, optional
-        Path to power/ct curve file, for creation
-        of default turbine type model
-
     Attributes
     ----------
-    point_models : foxes.utils.Dict
+    point_models: foxes.utils.Dict
         The point models. Keys: model name str,
         values: foxes.core.PointDataModel
-    rotor_models : foxes.utils.Dict
+    rotor_models: foxes.utils.Dict
         The rotor models. Keys: model name str,
         values: foxes.core.RotorModel
-    turbine_types : foxes.utils.Dict
+    turbine_types: foxes.utils.Dict
         The turbine type models. Keys: model name str,
         values: foxes.core.TurbineType
-    turbine_models : foxes.utils.Dict
+    turbine_models: foxes.utils.Dict
         The turbine models. Keys: model name str,
         values: foxes.core.TurbineModel
-    turbine_orders : foxes.utils.Dict
+    turbine_orders: foxes.utils.Dict
         The turbine orders. Keys: model name str,
         values: foxes.core.TurbineOrder
-    farm_models : foxes.utils.Dict
+    farm_models: foxes.utils.Dict
         The farm models. Keys: model name str,
         values: foxes.core.FarmModel
-    farm_controllers : foxes.utils.Dict
+    farm_controllers: foxes.utils.Dict
         The farm controllers. Keys: model name str,
         values: foxes.core.FarmController
-    partial_wakes : foxes.utils.Dict
+    partial_wakes: foxes.utils.Dict
         The partial wakes. Keys: model name str,
         values: foxes.core.PartialWakeModel
-    wake_frames : foxes.utils.Dict
+    wake_frames: foxes.utils.Dict
         The wake frames. Keys: model name str,
         values: foxes.core.WakeFrame
-    wake_superpositions : foxes.utils.Dict
+    wake_superpositions: foxes.utils.Dict
         The wake superposition models. Keys: model name str,
         values: foxes.core.WakeSuperposition
-    wake_models : foxes.utils.Dict
+    wake_models: foxes.utils.Dict
         The wake models. Keys: model name str,
         values: foxes.core.WakeModel
-    sources : foxes.utils.Dict
+    sources: foxes.utils.Dict
         All sources dict
+    
+    :group: foxes
 
     """
 
     def __init__(self, Pct_file=None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        Pct_file: str, optional
+            Path to power/ct curve file, for creation
+            of default turbine type model
+        """
         self.point_models = Dict(name="point_models")
         self.point_models["tke2ti"] = fm.point_models.TKE2TI()
 
         self.rotor_models = Dict(name="rotor_models")
         rvars = [FV.REWS, FV.REWS2, FV.REWS3, FV.TI, FV.RHO]
         self.rotor_models["centre"] = fm.rotor_models.CentreRotor(calc_vars=rvars)
         nlist = list(range(2, 11)) + [20]
@@ -312,17 +315,17 @@
 
     def print_toc(self, subset=None, search=None):
         """
         Print the contents.
 
         Parameters
         ----------
-        subset : list of str, optional
+        subset: list of str, optional
             Selection of model types
-        search :  str, optional
+        search:  str, optional
             String that has to be part of the model name
 
         """
         for k in sorted(list(self.sources.keys())):
             ms = self.sources[k]
             if subset is None or k in subset:
                 print(k)
@@ -337,17 +340,17 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         for ms in self.sources.values():
             if isinstance(ms, Dict):
                 for m in ms.values():
                     if m.initialized:
```

### Comparing `foxes-0.3.5/foxes/models/partial_wakes/axiwake.py` & `foxes-0.4.0/foxes/models/partial_wakes/axiwake.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,35 +14,41 @@
     The basic idea is that the x-dependent part of
     the wake model is evaluated only once, and the radial
     part then for `n` radii that cover the target rotor discs.
 
     The latter results are then weighted according to the overlap
     of radial wake circle area deltas and the target rotor disc area.
 
-    Parameters
-    ----------
-    n : int
-        The number of radial evaluation points
-    wake_models : list of foxes.core.WakeModel, optional
-        The wake models, default are the ones from the algorithm
-    wake_frame : foxes.core.WakeFrame, optional
-        The wake frame, default is the one from the algorithm
-    rotor_model : foxes.core.RotorModel, optional
-        The rotor model, default is the one from the algorithm
-
     Attributes
     ----------
-    n : int
+    n: int
         The number of radial evaluation points
-    rotor_model : foxes.core.RotorModel
+    rotor_model: foxes.core.RotorModel
         The rotor model, default is the one from the algorithm
 
+    :group: models.partial_wakes
+
     """
 
     def __init__(self, n, wake_models=None, wake_frame=None, rotor_model=None):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        n: int
+            The number of radial evaluation points
+        wake_models: list of foxes.core.WakeModel, optional
+            The wake models, default are the ones from the algorithm
+        wake_frame: foxes.core.WakeFrame, optional
+            The wake frame, default is the one from the algorithm
+        rotor_model: foxes.core.RotorModel, optional
+            The rotor model, default is the one from the algorithm
+
+        """
         super().__init__(wake_models, wake_frame)
 
         self.n = n
         self.rotor_model = rotor_model
 
     def __repr__(self):
         return super().__repr__() + f"(n={self.n})"
@@ -55,22 +61,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
 
@@ -90,24 +96,24 @@
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        wake_deltas : dict
+        wake_deltas: dict
             Keys: Variable name str, values: any
 
         """
         n_points = fdata.n_turbines
         wake_deltas = {}
         for w in self.wake_models:
             w.init_wake_deltas(algo, mdata, fdata, n_points, wake_deltas)
@@ -119,24 +125,24 @@
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray of int
+        states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
-        wake_deltas : Any
+        wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
         """
         # prepare:
         n_states = mdata.n_states
         n_turbines = algo.n_turbines
@@ -245,30 +251,30 @@
     ):
         """
         Updates the farm data according to the wake
         deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
             Modified in-place by this function
-        wake_deltas : Any
+        wake_deltas: Any
             The wake deltas object, created by the
             `new_wake_deltas` function and filled
             by `contribute_to_wake_deltas`
-        states_turbine : numpy.ndarray of int
+        states_turbine: numpy.ndarray of int
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
-        update_amb_res : bool
+        update_amb_res: bool
             Flag for updating ambient results
 
         """
         weights = self.get_data(FC.RWEIGHTS, mdata)
         amb_res = self.get_data(FC.AMB_RPOINT_RESULTS, mdata)
         rpoints = self.get_data(FC.RPOINTS, mdata)
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
@@ -298,16 +304,16 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level
 
         """
         if self.rotor_model.initialized:
             self.rotor_model.finalize(algo, verbosity)
         super().finalize(algo, verbosity)
```

### Comparing `foxes-0.3.5/foxes/models/partial_wakes/distsliced.py` & `foxes-0.4.0/foxes/models/partial_wakes/distsliced.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,39 +12,45 @@
     """
     Partial wakes for distance sliced wake models,
     making use of their structure.
 
     The evaluations are optinally done on a grid rotor
     that can differ from the algorithm's rotor model.
 
-    Parameters
-    ----------
-    n : int, optional
-        The `GridRotor`'s `n` parameter
-    wake_models : list of foxes.core.WakeModel, optional
-        The wake models, default are the ones from the algorithm
-    wake_frame : foxes.core.WakeFrame, optional
-        The wake frame, default is the one from the algorithm
-    rotor_model : foxes.core.RotorModel, optional
-        The rotor model, default is the one from the algorithm
-    **kwargs : dict, optional
-        Additional parameters for the `GridRotor`
-
     Attributes
     ----------
-    rotor_model : foxes.core.RotorModel
+    rotor_model: foxes.core.RotorModel
         The rotor model, default is the one from the algorithm
-    grotor : foxes.models.rotor_models.GridRotor
+    grotor: foxes.models.rotor_models.GridRotor
         The grid rotor model
 
+    :group: models.partial_wakes
+
     """
 
     def __init__(
         self, n=None, wake_models=None, wake_frame=None, rotor_model=None, **kwargs
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        n: int, optional
+            The `GridRotor`'s `n` parameter
+        wake_models: list of foxes.core.WakeModel, optional
+            The wake models, default are the ones from the algorithm
+        wake_frame: foxes.core.WakeFrame, optional
+            The wake frame, default is the one from the algorithm
+        rotor_model: foxes.core.RotorModel, optional
+            The rotor model, default is the one from the algorithm
+        kwargs: dict, optional
+            Additional parameters for the `GridRotor`
+
+        """
         super().__init__(wake_models, wake_frame)
 
         self.rotor_model = rotor_model
         self.grotor = None if n is None else GridRotor(n=n, calc_vars=[], **kwargs)
 
     def __repr__(self):
         if self.grotor is not None:
@@ -62,22 +68,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
 
@@ -104,24 +110,24 @@
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        wake_deltas : dict
+        wake_deltas: dict
             Keys: Variable name str, values: any
 
         """
         n_rpoints = self.grotor.n_rotor_points()
         n_points = fdata.n_turbines * n_rpoints
         wake_deltas = {}
         for w in self.wake_models:
@@ -134,24 +140,24 @@
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray of int
+        states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
-        wake_deltas : Any
+        wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
         """
         # calc coordinates to rotor centres:
         wcoos = self.wake_frame.get_wake_coos(
             algo, mdata, fdata, states_source_turbine, fdata[FV.TXYH]
@@ -213,30 +219,30 @@
     ):
         """
         Updates the farm data according to the wake
         deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
             Modified in-place by this function
-        wake_deltas : Any
+        wake_deltas: Any
             The wake deltas object, created by the
             `new_wake_deltas` function and filled
             by `contribute_to_wake_deltas`
-        states_turbine : numpy.ndarray of int
+        states_turbine: numpy.ndarray of int
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
-        update_amb_res : bool
+        update_amb_res: bool
             Flag for updating ambient results
 
         """
         amb_res = self.get_data(FC.AMB_RPOINT_RESULTS, mdata)
         rpoints = self.get_data(FC.RPOINTS, mdata)
         rweights = self.get_data(FC.RWEIGHTS, mdata)
         wweights = self.grotor.rotor_point_weights()
@@ -294,17 +300,17 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level
 
         """
         if self.rotor_model.initialized:
             self.rotor_model.finalize(algo, verbosity)
         if self.grotor is not None and self.grotor.initialized:
             self.grotor.finalize(algo, verbosity)
```

### Comparing `foxes-0.3.5/foxes/models/partial_wakes/grid.py` & `foxes-0.4.0/foxes/models/partial_wakes/grid.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,32 +3,38 @@
 
 
 class PartialGrid(PartialDistSlicedWake):
     """
     Partial wakes on a grid rotor that may
     differ from the one in the algorithm.
 
-    Parameters
-    ----------
-    n : int, optional
-        The `GridRotor`'s `n` parameter
-    wake_models : list of foxes.core.WakeModel, optional
-        The wake models, default are the ones from the algorithm
-    wake_frame : foxes.core.WakeFrame, optional
-        The wake frame, default is the one from the algorithm
-    rotor_model : foxes.core.RotorModel, optional
-        The rotor model, default is the one from the algorithm
-    **kwargs : dict, optional
-        Additional parameters for the `GridRotor`
+    :group: models.partial_wakes
 
     """
 
     def __init__(
         self, n, wake_models=None, wake_frame=None, rotor_model=None, **kwargs
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        n: int, optional
+            The `GridRotor`'s `n` parameter
+        wake_models: list of foxes.core.WakeModel, optional
+            The wake models, default are the ones from the algorithm
+        wake_frame: foxes.core.WakeFrame, optional
+            The wake frame, default is the one from the algorithm
+        rotor_model: foxes.core.RotorModel, optional
+            The rotor model, default is the one from the algorithm
+        kwargs: dict, optional
+            Additional parameters for the `GridRotor`
+
+        """
         super().__init__(n, wake_models, wake_frame, rotor_model, **kwargs)
 
         if not isinstance(self.grotor, GridRotor):
             raise ValueError(
                 f"Wrong grotor type, expecting {GridRotor.__name__}, got {type(self.grotor).__name__}"
             )
 
@@ -37,24 +43,24 @@
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray of int
+        states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
-        wake_deltas : Any
+        wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
         """
         # evaluate grid rotor:
         n_states = fdata.n_states
         n_turbines = fdata.n_turbines
```

### Comparing `foxes-0.3.5/foxes/models/partial_wakes/mapped.py` & `foxes-0.4.0/foxes/models/partial_wakes/mapped.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,45 +13,51 @@
 class Mapped(PartialWakesModel):
     """
     Partial wake models depending on the wake model (type).
 
     This is required if more than one wake models are
     used and different partial wake models should be invoked.
 
-    Parameters
-    ----------
-    wname2pwake : dict, optional
-        Mapping from wake model name to partial wakes.
-        Key: model name str, value: Tuple of length 2,
-        (Partial wake class name, parameter dict)
-    wtype2pwake : dict, optional
-        Mapping from wake model class name to partial wakes.
-        Key: wake model class name str, value: Tuple of length 2,
-        (Partial wake class name, parameter dict)
-    wake_models : list of foxes.core.WakeModel, optional
-        The wake models, default are the ones from the algorithm
-    wake_frame : foxes.core.WakeFrame, optional
-        The wake frame, default is the one from the algorithm
-
     Attributes
     ----------
-    wname2pwake : dict
+    wname2pwake: dict
         Mapping from wake model name to partial wakes.
         Key: model name str, value: Tuple of length 2,
         (Partial wake class name, parameter dict)
-    wtype2pwake : dict
+    wtype2pwake: dict
         Mapping from wake model class name to partial wakes.
         Key: wake model class name str, value: Tuple of length 2,
         (Partial wake class name, parameter dict)
+    
+    :group: models.partial_wakes
 
     """
 
     def __init__(
         self, wname2pwake={}, wtype2pwake=None, wake_models=None, wake_frame=None
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        wname2pwake: dict, optional
+            Mapping from wake model name to partial wakes.
+            Key: model name str, value: Tuple of length 2,
+            (Partial wake class name, parameter dict)
+        wtype2pwake: dict, optional
+            Mapping from wake model class name to partial wakes.
+            Key: wake model class name str, value: Tuple of length 2,
+            (Partial wake class name, parameter dict)
+        wake_models: list of foxes.core.WakeModel, optional
+            The wake models, default are the ones from the algorithm
+        wake_frame: foxes.core.WakeFrame, optional
+            The wake frame, default is the one from the algorithm
+
+        """
         super().__init__(wake_models, wake_frame)
 
         self.wname2pwake = wname2pwake
 
         if wtype2pwake is None:
             self.wtype2pwake = {
                 TopHatWakeModel: (PartialTopHat.__name__, {}),
@@ -71,22 +77,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
 
@@ -127,48 +133,48 @@
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        wake_deltas : dict
+        wake_deltas: dict
             Keys: Variable name str, values: any
 
         """
         return [pw.new_wake_deltas(algo, mdata, fdata) for pw in self._pwakes]
 
     def contribute_to_wake_deltas(
         self, algo, mdata, fdata, states_source_turbine, wake_deltas
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray of int
+        states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
-        wake_deltas : Any
+        wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
         """
         for pwi, pw in enumerate(self._pwakes):
             pw.contribute_to_wake_deltas(
                 algo, mdata, fdata, states_source_turbine, wake_deltas[pwi]
@@ -179,45 +185,45 @@
     ):
         """
         Updates the farm data according to the wake
         deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
             Modified in-place by this function
-        wake_deltas : Any
+        wake_deltas: Any
             The wake deltas object, created by the
             `new_wake_deltas` function and filled
             by `contribute_to_wake_deltas`
-        states_turbine : numpy.ndarray of int
+        states_turbine: numpy.ndarray of int
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
-        update_amb_res : bool
+        update_amb_res: bool
             Flag for updating ambient results
 
         """
         for pwi, pw in enumerate(self._pwakes):
             pw.evaluate_results(
                 algo, mdata, fdata, wake_deltas[pwi], states_turbine, update_amb_res
             )
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level
 
         """
         self._pwakes = None
         super().finalize(algo, verbosity)
```

### Comparing `foxes-0.3.5/foxes/models/partial_wakes/rotor_points.py` & `foxes-0.4.0/foxes/models/partial_wakes/rotor_points.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,46 +5,52 @@
 import foxes.constants as FC
 
 class RotorPoints(PartialWakesModel):
     """
     Partial wakes calculation directly by the
     rotor model.
 
-    Parameters
-    ----------
-    wake_models : list of foxes.core.WakeModel, optional
-        The wake models, default are the ones from the algorithm
-    wake_frame : foxes.core.WakeFrame, optional
-        The wake frame, default is the one from the algorithm
+    :group: models.partial_wakes
 
     """
 
     def __init__(self, wake_models=None, wake_frame=None):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        wake_models: list of foxes.core.WakeModel, optional
+            The wake models, default are the ones from the algorithm
+        wake_frame: foxes.core.WakeFrame, optional
+            The wake frame, default is the one from the algorithm
+
+        """
         super().__init__(wake_models, wake_frame)
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.WPOINTS = self.var("WPOINTS")
 
@@ -55,48 +61,48 @@
 
     def get_wake_points(self, algo, mdata, fdata):
         """
         Get the wake calculation points.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        rpoints : numpy.ndarray
+        rpoints: numpy.ndarray
             All rotor points, shape: (n_states, n_points, 3)
 
         """
         rpoints = self.get_data(FC.RPOINTS, mdata)
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
         return rpoints.reshape(n_states, n_turbines * n_rpoints, 3)
 
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        wake_deltas : dict
+        wake_deltas: dict
             Keys: Variable name str, values: any
 
         """
         mdata[self.WPOINTS] = self.get_wake_points(algo, mdata, fdata)
         n_points = mdata[self.WPOINTS].shape[1]
 
         wake_deltas = {}
@@ -110,24 +116,24 @@
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray of int
+        states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
-        wake_deltas : Any
+        wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
         """
         points = mdata[self.WPOINTS]
         wcoos = self.wake_frame.get_wake_coos(
             algo, mdata, fdata, states_source_turbine, points
@@ -143,30 +149,30 @@
     ):
         """
         Updates the farm data according to the wake
         deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
             Modified in-place by this function
-        wake_deltas : Any
+        wake_deltas: Any
             The wake deltas object, created by the
             `new_wake_deltas` function and filled
             by `contribute_to_wake_deltas`
-        states_turbine : numpy.ndarray of int
+        states_turbine: numpy.ndarray of int
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
-        update_amb_res : bool
+        update_amb_res: bool
             Flag for updating ambient results
 
         """
         weights = self.get_data(FC.RWEIGHTS, mdata)
         amb_res = self.get_data(FC.AMB_RPOINT_RESULTS, mdata)
         rpoints = self.get_data(FC.RPOINTS, mdata)
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
```

### Comparing `foxes-0.3.5/foxes/models/partial_wakes/top_hat.py` & `foxes-0.4.0/foxes/models/partial_wakes/top_hat.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,31 +10,37 @@
 class PartialTopHat(PartialWakesModel):
     """
     Partial wakes for top-hat models.
 
     The wake effect is weighted by the overlap of
     the wake circle and the rotor disc circle.
 
-    Parameters
-    ----------
-    wake_models : list of foxes.core.WakeModel, optional
-        The wake models, default are the ones from the algorithm
-    wake_frame : foxes.core.WakeFrame, optional
-        The wake frame, default is the one from the algorithm
-    rotor_model : foxes.core.RotorModel, optional
-        The rotor model, default is the one from the algorithm
-
     Attributes
     ----------
-    rotor_model : foxes.core.RotorModel
+    rotor_model: foxes.core.RotorModel
         The rotor model, default is the one from the algorithm
 
+    :group: models.partial_wakes
+
     """
 
     def __init__(self, wake_models=None, wake_frame=None, rotor_model=None):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        wake_models: list of foxes.core.WakeModel, optional
+            The wake models, default are the ones from the algorithm
+        wake_frame: foxes.core.WakeFrame, optional
+            The wake frame, default is the one from the algorithm
+        rotor_model: foxes.core.RotorModel, optional
+            The rotor model, default is the one from the algorithm
+
+        """
         super().__init__(wake_models, wake_frame)
         self.rotor_model = rotor_model
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
@@ -42,22 +48,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
 
@@ -80,46 +86,46 @@
 
     def get_wake_points(self, algo, mdata, fdata):
         """
         Get the wake calculation points.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        rpoints : numpy.ndarray
+        rpoints: numpy.ndarray
             All rotor points, shape: (n_states, n_points, 3)
 
         """
         return fdata[FV.TXYH]
 
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        wake_deltas : dict
+        wake_deltas: dict
             Keys: Variable name str, values: any
 
         """
         n_points = fdata.n_turbines
         wake_deltas = {}
         for w in self.wake_models:
             w.init_wake_deltas(algo, mdata, fdata, n_points, wake_deltas)
@@ -131,24 +137,24 @@
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray of int
+        states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
-        wake_deltas : Any
+        wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
         """
         n_states = mdata.n_states
         n_points = fdata.n_turbines
         stsel = (np.arange(n_states), states_source_turbine)
@@ -225,30 +231,30 @@
     ):
         """
         Updates the farm data according to the wake
         deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
             Modified in-place by this function
-        wake_deltas : Any
+        wake_deltas: Any
             The wake deltas object, created by the
             `new_wake_deltas` function and filled
             by `contribute_to_wake_deltas`
-        states_turbine : numpy.ndarray of int
+        states_turbine: numpy.ndarray of int
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
-        update_amb_res : bool
+        update_amb_res: bool
             Flag for updating ambient results
 
         """
         weights = self.get_data(FC.RWEIGHTS, mdata)
         amb_res = self.get_data(FC.AMB_RPOINT_RESULTS, mdata)
         rpoints = self.get_data(FC.RPOINTS, mdata)
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
@@ -278,16 +284,16 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level
 
         """
         if self.rotor_model.initialized:
             self.rotor_model.finalize(algo, verbosity)
         super().finalize(algo, verbosity)
```

### Comparing `foxes-0.3.5/foxes/models/point_models/set_uniform_data.py` & `foxes-0.4.0/foxes/models/point_models/set_uniform_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,47 +6,53 @@
 import foxes.variables as FV
 
 
 class SetUniformData(PointDataModel):
     """
     Set uniform data (can be state dependent)
 
-    Parameters
-    ----------
-    data_source : str or pandas.DataFrame or dict
-        Either a file name, or a data frame, both assuming
-        state dependent data. Or a dict for state independent
-        uniform data (i.e., scalars)
-    output_vars : list of str
-        The variables to be written
-    var2col : dict
-        Mapping from variable names to data column names
-    pd_read_pars : dict
-        pandas file reading parameters
-
     Attributes
     ----------
-    data_source : str or pandas.DataFrame or dict
+    data_source: str or pandas.DataFrame or dict
         Either a file name, or a data frame, both assuming
         state dependent data. Or a dict for state independent
         uniform data (i.e., scalars)
-    ovars : list of str
+    ovars: list of str
         The variables to be written
-    var2col : dict
+    var2col: dict
         Mapping from variable names to data column names
 
+    :group: models.point_models
+
     """
 
     def __init__(
         self,
         data_source,
         output_vars,
         var2col={},
         pd_read_pars={},
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        data_source: str or pandas.DataFrame or dict
+            Either a file name, or a data frame, both assuming
+            state dependent data. Or a dict for state independent
+            uniform data (i.e., scalars)
+        output_vars: list of str
+            The variables to be written
+        var2col: dict
+            Mapping from variable names to data column names
+        pd_read_pars: dict
+            pandas file reading parameters
+
+        """
         self.data_source = data_source
         self.ovars = output_vars
         self.var2col = var2col
 
         self._rpars = pd_read_pars
 
     def initialize(self, algo, verbosity=0):
@@ -57,22 +63,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.VARS = self.var("VARS")
         self.DATA = self.var("DATA")
@@ -99,46 +105,46 @@
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return self.ovars
 
     def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pdata : foxes.core.Data
+        pdata: foxes.core.Data
             The point data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         for v in self.ovars:
             if self.DATA in mdata:
                 pdata[v][:] = mdata[v][None, self.ovars.index(v)]
```

### Comparing `foxes-0.3.5/foxes/models/point_models/tke2ti.py` & `foxes-0.4.0/foxes/models/point_models/tke2ti.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,54 +3,57 @@
 from foxes.core import PointDataModel
 import foxes.variables as FV
 
 
 class TKE2TI(PointDataModel):
     """
     Calculates TI from TKE, using TI = sqrt( 3/2 * TKE) / WS
+
+    :group: models.point_models
+    
     """
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return [FV.TI]
 
     def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pdata : foxes.core.Data
+        pdata: foxes.core.Data
             The point data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         tke = pdata[FV.TKE]
         ws = pdata[FV.WS]
```

### Comparing `foxes-0.3.5/foxes/models/point_models/wake_deltas.py` & `foxes-0.4.0/foxes/models/point_models/wake_deltas.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,73 +3,79 @@
 
 
 class WakeDeltas(PointDataModel):
     """
     This point model simply subtracts ambient results
     from waked results.
 
-    Parameters
-    ----------
-    vars : list of str
-        The variables
-    normalize : bool
-        Divide resulting deltas by ambient values
-
     Attributes
     ----------
-    vars : list of str
+    vars: list of str
         The variables
-    normalize : bool
+    normalize: bool
         Divide resulting deltas by ambient values
 
+    :group: models.point_models
+
     """
 
     def __init__(self, vars, normalize=False):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        vars: list of str
+            The variables
+        normalize: bool
+            Divide resulting deltas by ambient values
+
+        """
         super().__init__()
         self.vars = vars
         self.normalize = normalize
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return [f"DELTA_{v}" for v in self.vars]
 
     def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pdata : foxes.core.Data
+        pdata: foxes.core.Data
             The point data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
 
         out = {f"DELTA_{v}": pdata[v] - pdata[FV.var2amb[v]] for v in self.vars}
```

### Comparing `foxes-0.3.5/foxes/models/rotor_models/centre.py` & `foxes-0.4.0/foxes/models/rotor_models/centre.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 class CentreRotor(RotorModel):
     """
     The centre rotor model.
 
     Evaluates states at a single point, located
     at the rotor centre.
 
+    :group: models.rotor_models
+
     """
 
     def n_rotor_points(self):
         """
         The number of rotor points
 
         Returns
         -------
-        n_rpoints : int
+        n_rpoints: int
             The number of rotor points
 
         """
         return 1
 
     def design_points(self):
         """
@@ -36,49 +38,49 @@
         - (0,0,0) is the centre point,
         - (1,0,0) is the point radius * n_rotor_axis
         - (0,1,0) is the point radius * n_rotor_side
         - (0,0,1) is the point radius * n_rotor_up
 
         Returns
         -------
-        dpoints : numpy.ndarray
+        dpoints: numpy.ndarray
             The design points, shape: (n_points, 3)
 
         """
         return np.array([[0.0, 0.0, 0.0]])
 
     def rotor_point_weights(self):
         """
         The weights of the rotor points
 
         Returns
         -------
-        weights : numpy.ndarray
+        weights: numpy.ndarray
             The weights of the rotor points,
             add to one, shape: (n_rpoints,)
 
         """
         return np.array([1.0])
 
     def get_rotor_points(self, algo, mdata, fdata):
         """
         Calculates rotor points from design points.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The rotor points, shape:
             (n_states, n_turbines, n_rpoints, 3)
 
         """
         return fdata[FV.TXYH][:, :, None, :]
 
     def eval_rpoint_results(
@@ -98,30 +100,30 @@
         for all turbines or one turbine per state,
         depending on parameter `states_turbine`. In
         the latter case, the turbine dimension of the
         `rpoint_results` is expected to have size one.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        rpoint_results : dict
+        rpoint_results: dict
             The results at rotor points. Keys: variable str.
             Values: numpy.ndarray, shape if `states_turbine`
             is None: (n_states, n_turbines, n_rpoints).
             Else: (n_states, 1, n_rpoints)
-        weights : numpy.ndarray
+        weights: numpy.ndarray
             The rotor point weights, shape: (n_rpoints,)
         states_turbine: numpy.ndarray of int, optional
             The turbine indices, one per state. Shape: (n_states,)
-        copy_to_ambient : bool, optional
+        copy_to_ambient: bool, optional
             If `True`, the fdata results are copied to ambient
             variables after calculation
 
         """
         if len(weights) > 1:
             return super().eval_rpoint_results(
                 algo, mdata, fdata, rpoint_results, weights, states_turbine
```

### Comparing `foxes-0.3.5/foxes/models/rotor_models/grid.py` & `foxes-0.4.0/foxes/models/rotor_models/grid.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,49 +2,55 @@
 
 from foxes.core import RotorModel
 import foxes.constants as FC
 
 
 class GridRotor(RotorModel):
     """
-    The regular grid rotor model, composed maximally
+    The weighted regular grid rotor model, composed maximally
     of n x n points, possibly kicking out the outside points.
 
-    Parameters
-    ----------
-    n: int
-        The number of points along one direction,
-        maximal number of points is N = n * n
-    calc_vars : list of str
-        The variables that are calculated by the model
-        (Their ambients are added automatically)
-    reduce: bool
-        Flag for reduction to points actually representing
-        an area with overlap with the circe, recalculating
-        the self.weights accordingly
-    nint: int
-        Integration steps per element
-    name: str, optional
-        The model name
-
     Attributes
     ----------
     n: int
         The number of points along one direction,
         maximal number of points is N = n * n
     reduce: bool
         Flag for reduction to points actually representing
         an area with overlap with the circe, recalculating
         the self.weights accordingly
     nint: int
         Integration steps per element
 
+    :group: models.rotor_models
+
     """
 
     def __init__(self, n, calc_vars, reduce=True, nint=200):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        n: int
+            The number of points along one direction,
+            maximal number of points is N = n * n
+        calc_vars: list of str
+            The variables that are calculated by the model
+            (Their ambients are added automatically)
+        reduce: bool
+            Flag for reduction to points actually representing
+            an area with overlap with the circe, recalculating
+            the self.weights accordingly
+        nint: int
+            Integration steps per element
+        name: str, optional
+            The model name
+
+        """
         super().__init__(calc_vars)
 
         self.n = n
         self.reduce = reduce
         self.nint = nint
 
     def __repr__(self):
@@ -58,22 +64,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         N = self.n * self.n
         delta = 2.0 / self.n
@@ -116,15 +122,15 @@
 
     def n_rotor_points(self):
         """
         The number of rotor points
 
         Returns
         -------
-        n_rpoints : int
+        n_rpoints: int
             The number of rotor points
 
         """
         return len(self.weights)
 
     def design_points(self):
         """
@@ -135,25 +141,25 @@
         - (0,0,0) is the centre point,
         - (1,0,0) is the point radius * n_rotor_axis
         - (0,1,0) is the point radius * n_rotor_side
         - (0,0,1) is the point radius * n_rotor_up
 
         Returns
         -------
-        dpoints : numpy.ndarray
+        dpoints: numpy.ndarray
             The design points, shape: (n_points, 3)
 
         """
         return self.dpoints
 
     def rotor_point_weights(self):
         """
         The weights of the rotor points
 
         Returns
         -------
-        weights : numpy.ndarray
+        weights: numpy.ndarray
             The weights of the rotor points,
             add to one, shape: (n_rpoints,)
 
         """
         return self.weights
```

### Comparing `foxes-0.3.5/foxes/models/turbine_models/calculator.py` & `foxes-0.4.0/foxes/models/turbine_models/calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,87 +3,93 @@
 from foxes.core import TurbineModel
 
 
 class Calculator(TurbineModel):
     """
     Calculates variables based on given functions.
 
-    Parameters
-    ----------
-    in_vars : list of str
-        The input farm vairables
-    out_vars : list of str
-        The output variables
-    func : Function
-        The function: f(in0, in1, ..., stsel) -> (out0, ou1, ...)
-        where inX and outY are numpy.ndarrays and
-        st_sel is the boolean state-turbine selection.
-        All arrays have shape (n_states, n_turbines).
-    kwargs : dict, optional
-        Additional arguments for TurbineModel
-
     Attributes
     ----------
-    in_vars : list of str
+    in_vars: list of str
         The input farm vairables
-    out_vars : list of str
+    out_vars: list of str
         The output variables
-    func : Function
+    func: Function
         The function: f(in0, in1, ..., stsel) -> (out0, ou1, ...)
         where inX and outY are numpy.ndarrays and
         st_sel is the boolean state-turbine selection.
         All arrays have shape (n_states, n_turbines).
 
+    :group: models.turbine_models
+
     """
 
     def __init__(self, in_vars, out_vars, func, **kwargs):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        in_vars: list of str
+            The input farm vairables
+        out_vars: list of str
+            The output variables
+        func: Function
+            The function: f(in0, in1, ..., stsel) -> (out0, ou1, ...)
+            where inX and outY are numpy.ndarrays and
+            st_sel is the boolean state-turbine selection.
+            All arrays have shape (n_states, n_turbines).
+        kwargs: dict, optional
+            Additional arguments for TurbineModel
+
+        """
         super().__init__(**kwargs)
         self.in_vars = in_vars
         self.out_vars = out_vars
         self.func = func
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return self.out_vars
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         ins = [fdata[v] if v in fdata else mdata[v] for v in self.in_vars]
         outs = self.func(*ins, st_sel=st_sel)
```

### Comparing `foxes-0.3.5/foxes/models/turbine_models/kTI_model.py` & `foxes-0.4.0/foxes/models/turbine_models/kTI_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,40 +6,46 @@
 
 
 class kTI(TurbineModel):
     """
     Calculates the wake model parameter `k`
     as a linear function of `TI`.
 
-    Parameters
-    ----------
-    kTI : float, optional
-        Uniform value for `kTI`. If not given it
-        will be searched in farm data
-    kb : float, optional
-        Uniform value for `kb`. If not given it
-        will be searched in farm data, and zero by default
-    ti_var : str
-        The `TI` variable name
-    ti_val : float, optional
-        The uniform value of `TI`. If not given it
-        will be searched in farm data
-    k_var : str
-        The variable name for k
-
     Attributes
     ----------
-    ti_var : str
+    ti_var: str
         The `TI` variable name
-    k_var : str
+    k_var: str
         The variable name for k
 
+    :group: models.turbine_models
+
     """
 
     def __init__(self, kTI=None, kb=None, ti_var=FV.TI, ti_val=None, k_var=FV.K):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        kTI: float, optional
+            Uniform value for `kTI`. If not given it
+            will be searched in farm data
+        kb: float, optional
+            Uniform value for `kb`. If not given it
+            will be searched in farm data, and zero by default
+        ti_var: str
+            The `TI` variable name
+        ti_val: float, optional
+            The uniform value of `TI`. If not given it
+            will be searched in farm data
+        k_var: str
+            The variable name for k
+
+        """
         super().__init__()
 
         self.ti_var = ti_var
         self.k_var = k_var
         setattr(self, ti_var, ti_val)
         setattr(self, FV.KTI, kTI)
         setattr(self, FV.KB, 0 if kb is None else kb)
@@ -49,47 +55,47 @@
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return [self.k_var]
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         kTI = self.get_data(FV.KTI, fdata, st_sel)
         kb = self.get_data(FV.KB, fdata, st_sel)
         ti = self.get_data(self.ti_var, fdata, st_sel)
```

### Comparing `foxes-0.3.5/foxes/models/turbine_models/power_mask.py` & `foxes-0.4.0/foxes/models/turbine_models/power_mask.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,48 +14,54 @@
     the maximal power value is below rated power.
     For higher values, a boost is introduced.
 
     The model updates the P and CT variables,
     so it is wise to use it after calling the
     turbine type model.
 
-    Parameters
-    ----------
-    var_ws_P : str
-        The wind speed variable for power lookup
-    factor_P : float
-        The power unit factor, e.g. 1000 for kW
-
     Attributes
     ----------
-    var_ws_P : str
+    var_ws_P: str
         The wind speed variable for power lookup
-    factor_P : float
+    factor_P: float
         The power unit factor, e.g. 1000 for kW
 
+    :group: models.turbine_models
+
     """
 
     def __init__(self, var_ws_P=FV.REWS3, factor_P=1.0e3):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        var_ws_P: str
+            The wind speed variable for power lookup
+        factor_P: float
+            The power unit factor, e.g. 1000 for kW
+
+        """
         super().__init__()
 
         self.var_ws_P = var_ws_P
         self.factor_P = factor_P
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return [FV.P, FV.CT]
 
     def initialize(self, algo, verbosity=0):
         """
@@ -65,22 +71,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self._P_rated = []
         for t in algo.farm_controller.turbine_types:
@@ -147,27 +153,27 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
 
         # prepare:
         max_P = fdata[FV.MAX_P]
```

### Comparing `foxes-0.3.5/foxes/models/turbine_models/rotor_centre_calc.py` & `foxes-0.4.0/foxes/models/turbine_models/rotor_centre_calc.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,35 @@
 import foxes.variables as FV
 import foxes.constants as FC
 
 class RotorCentreCalc(TurbineModel):
     """
     Calculates data at the rotor centre
 
-    Parameters
-    ----------
-    calc_vars : dict
-        The variables that are calculated by the model,
-        keys: var names, values: rotor var names
-
     Attributes
     ----------
-    calc_vars : dict
+    calc_vars: dict
         The variables that are calculated by the model,
         keys: var names, values: rotor var names
         
+    :group: models.turbine_models
+
     """
 
     def __init__(self, calc_vars):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        calc_vars: dict
+            The variables that are calculated by the model,
+            keys: var names, values: rotor var names
+
+        """
         super().__init__()
         
         if isinstance(calc_vars, dict):
             self.calc_vars = calc_vars
         else:
             self.calc_vars = {v: v for v in calc_vars}
 
@@ -38,22 +44,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         pvars = list(self.calc_vars.values())
         self._wcalc = algo.PointWakesCalculation(point_vars=pvars)
@@ -65,47 +71,47 @@
         
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return list(self.calc_vars.keys())
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         # prepare point data:
         pdata = {FC.POINTS: fdata[FV.TXYH]}
         dims = {FC.POINTS: (FC.STATE, FC.POINT, FV.XYH)}
@@ -139,16 +145,16 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         algo.finalize_model(self._wcalc, verbosity)
         super().finalize(algo, verbosity)
```

### Comparing `foxes-0.3.5/foxes/models/turbine_models/sector_management.py` & `foxes-0.4.0/foxes/models/turbine_models/sector_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,54 +6,60 @@
 import foxes.variables as FV
 import foxes.constants as FC
 
 class SectorManagement(TurbineModel):
     """
     Changes variables based on variable range conditions.
 
-    Parameters
-    ----------
-    data_source : str or pandas.DataFrame
-        The file path or data
-    range_vars : list of str
-        The variables for which (min, max) ranges
-        are specified in the data
-    target_vars : list of str
-        The variables that change if range variables
-        are within specified ranges
-    col_tinds : str, optional
-        The turbine index column name in the data
-    col_tnames : str, optional
-        The turbine name column name in the data
-    colmap : dict
-        Mapping from expected to existing
-        column names
-    var_periods : dict
-        Periods for periodic variables
-    pd_file_read_pars : dict
-        Parameters for pandas file reading
-
     Attributes
     ----------
-    source : str or pandas.DataFrame
+    source: str or pandas.DataFrame
         The file path or data
 
+    :group: models.turbine_models
+
     """
 
     def __init__(
         self,
         data_source,
         range_vars,
         target_vars,
         col_tinds=None,
         col_tnames=None,
         colmap={},
         var_periods={FV.WD: 360.0, FV.AMB_WD: 360.0},
         pd_file_read_pars={},
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        data_source: str or pandas.DataFrame
+            The file path or data
+        range_vars: list of str
+            The variables for which (min, max) ranges
+            are specified in the data
+        target_vars: list of str
+            The variables that change if range variables
+            are within specified ranges
+        col_tinds: str, optional
+            The turbine index column name in the data
+        col_tnames: str, optional
+            The turbine name column name in the data
+        colmap: dict
+            Mapping from expected to existing
+            column names
+        var_periods: dict
+            Periods for periodic variables
+        pd_file_read_pars: dict
+            Parameters for pandas file reading
+
+        """
         super().__init__()
 
         self.source = data_source
 
         self._col_i = col_tinds
         self._col_t = col_tnames
         self._rvars = range_vars
@@ -74,22 +80,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         if isinstance(self.source, pd.DataFrame):
             data = self.source
@@ -152,47 +158,47 @@
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return self._tvars
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
 
         # prepare:
         n_trbs = len(self._trbs)
```

### Comparing `foxes-0.3.5/foxes/models/turbine_models/set_XYHD.py` & `foxes-0.4.0/foxes/models/turbine_models/set_XYHD.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,53 +6,59 @@
 
 
 class SetXYHD(TurbineModel):
     """
     Sets basic turbine data, from
     turbine object to farm data.
 
-    Parameters
-    ----------
-    set_XY : bool
-        Flag for (x,y) data
-    set_H : bool
-        Flag for height data
-    set_D : bool
-        Flag for rotor diameter data
-
     Attributes
     ----------
-    set_XY : bool
+    set_XY: bool
         Flag for (x,y) data
-    set_H : bool
+    set_H: bool
         Flag for height data
-    set_D : bool
+    set_D: bool
         Flag for rotor diameter data
 
+    :group: models.turbine_models
+
     """
 
     def __init__(self, set_XY=True, set_H=True, set_D=True):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        set_XY: bool
+            Flag for (x,y) data
+        set_H: bool
+            Flag for height data
+        set_D: bool
+            Flag for rotor diameter data
+
+        """
         super().__init__()
 
         self.set_XY = set_XY
         self.set_H = set_H
         self.set_D = set_D
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         ovars = []
         if self.set_XY:
             ovars.append(FV.X)
             ovars.append(FV.Y)
@@ -67,27 +73,27 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         n_states = mdata.n_states
         n_turbines = algo.n_turbines
```

### Comparing `foxes-0.3.5/foxes/models/turbine_models/set_farm_vars.py` & `foxes-0.4.0/foxes/models/turbine_models/set_farm_vars.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,65 +3,71 @@
 from foxes.core import TurbineModel
 import foxes.constants as FC
 
 class SetFarmVars(TurbineModel):
     """
     Set farm data variables to given data.
 
-    Parameters
-    ----------
-    pre_rotor : bool
-        Flag for running this model before
-        running the rotor model.
-
     Attributes
     ----------
-    vars : list of str
+    vars: list of str
         The variables to be set
 
+    :group: models.turbine_models
+
     """
 
     def __init__(self, pre_rotor=False):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        pre_rotor: bool
+            Flag for running this model before
+            running the rotor model.
+
+        """
         super().__init__(pre_rotor=pre_rotor)
         self.reset()
 
     def add_var(self, var, data):
         """
         Add data for a variable.
 
         Parameters
         ----------
-        var : str
+        var: str
             The variable name
-        data : numpy.ndarray
+        data: numpy.ndarray
             The data, shape: (n_states, n_turbines)
 
         """
         self.vars.append(var)
-        self._vdata.append(data)
+        self._vdata.append(np.asarray(data, dtype=FC.DTYPE))
 
     def reset(self):
         """
         Remove all variables.
         """
         self.vars = []
         self._vdata = []
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return self.vars
 
     def initialize(self, algo, verbosity=0):
         """
@@ -71,59 +77,72 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
 
         for i, v in enumerate(self.vars):
             data = np.full((algo.n_states, algo.n_turbines), np.nan, dtype=FC.DTYPE)
-            data[:] = self._vdata[i]
+            vdata = self._vdata[i]
 
+            # handle special case of call during vectorized optimization:
+            if (np.ndim(vdata) and 
+                vdata.shape[0] != algo.n_states and 
+                hasattr(algo.states, "n_pop")):
+
+                n_pop = algo.states.n_pop
+                n_ost = algo.states.states.size()
+                n_trb = algo.n_turbines
+                vdata = np.zeros((n_pop, n_ost, n_trb), dtype=FC.DTYPE)
+                vdata[:] = self._vdata[i][None, :]
+                vdata = vdata.reshape(n_pop*n_ost, n_trb)
+            
+            data[:] = vdata
             idata["data_vars"][self.var(v)] = ((FC.STATE, FC.TURBINE), data)
 
         return idata
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         n_states = fdata.n_states
         n_turbines = fdata.n_turbines
         allt = np.all(st_sel)
```

### Comparing `foxes-0.3.5/foxes/models/turbine_models/table_factors.py` & `foxes-0.4.0/foxes/models/turbine_models/table_factors.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,53 +11,59 @@
     """
     Multiplies variables by factors from a
     two dimensional table.
 
     The column names are expected to be numbers
     that represent the col_var variable.
 
-    Parameters
-    ----------
-    data_source : str or pandas.DataFrame
-        Either path to a file or data
-    row_var : str
-        The row-wise variable
-    col_var : str
-        The column-wise variable
-    output_vars : list of str
-        The variables onto which the factors
-        are multiplied
-    pd_file_read_pars : dict
-        Parameters for pandas file reading
-    ipars : dict, optional
-        Parameters for scipy.interpolate.interpn
-
     Attributes
     ----------
-    data_source : str or pandas.DataFrame
+    data_source: str or pandas.DataFrame
         Either path to a file or data
-    row_var : str
+    row_var: str
         The row-wise variable
-    col_var : str
+    col_var: str
         The column-wise variable
-    ovars : list of str
+    ovars: list of str
         The variables onto which the factors
         are multiplied
 
+    :group: models.turbine_models
+
     """
 
     def __init__(
         self,
         data_source,
         row_var,
         col_var,
         output_vars,
         pd_file_read_pars={},
         **ipars,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        data_source: str or pandas.DataFrame
+            Either path to a file or data
+        row_var: str
+            The row-wise variable
+        col_var: str
+            The column-wise variable
+        output_vars: list of str
+            The variables onto which the factors
+            are multiplied
+        pd_file_read_pars: dict
+            Parameters for pandas file reading
+        ipars: dict, optional
+            Parameters for scipy.interpolate.interpn
+
+        """
         super().__init__()
 
         self.data_source = data_source
         self.row_var = row_var
         self.col_var = col_var
         self.ovars = output_vars
         self._rpars = pd_file_read_pars
@@ -68,20 +74,20 @@
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return self.ovars
 
     def initialize(self, algo, verbosity=0):
         """
@@ -91,22 +97,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         if isinstance(self.data_source, pd.DataFrame):
             self._data = self.data_source
@@ -128,44 +134,44 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         n_sel = np.sum(st_sel)
         qts = np.zeros((n_sel, 2), dtype=FC.DTYPE)
         qts[:, 0] = fdata[self.row_var][st_sel]
         qts[:, 1] = fdata[self.col_var][st_sel]
 
         try:
             factors = interpn(
                 (self._rvals, self._cvals), self._data, qts, **self._ipars
             )
         except ValueError as e:
-            print(f"\nDATA        : ({self.row_var}, {self.col_var})")
+            print(f"\nDATA       : ({self.row_var}, {self.col_var})")
             print(
-                f"DATA BOUNDS : ({np.min(self._rvals)}, {np.min(self._cvals)}) -- ({np.max(self._rvals)}, {np.max(self._cvals)})"
+                f"DATA BOUNDS: ({np.min(self._rvals)}, {np.min(self._cvals)}) -- ({np.max(self._rvals)}, {np.max(self._cvals)})"
             )
             print(
                 f"VALUE BOUNDS: ({np.min(qts[:, 0]):.4f}, {np.min(qts[:, 1]):.4f}) -- ({np.max(qts[:, 0]):.4f}, {np.max(qts[:, 1]):.4f})\n"
             )
             raise e
 
         for v in self.output_farm_vars(algo):
```

### Comparing `foxes-0.3.5/foxes/models/turbine_models/thrust2ct.py` & `foxes-0.4.0/foxes/models/turbine_models/thrust2ct.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,74 +4,80 @@
 import foxes.variables as FV
 
 
 class Thrust2Ct(TurbineModel):
     """
     Calculates ct from thrust force data.
 
-    Parameters
-    ----------
-    thrust_var : str
-        Name of the thrust variable
-    var_ws_ct : str
-        The wind speed variable for ct lookup
-
     Attributes
     ----------
-    thrust_var : str
+    thrust_var: str
         Name of the thrust variable
-    WSCT : str
+    WSCT: str
         The wind speed variable for ct lookup
 
+    :group: models.turbine_models
+
     """
 
     def __init__(self, thrust_var=FV.T, var_ws_ct=FV.REWS2):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        thrust_var: str
+            Name of the thrust variable
+        var_ws_ct: str
+            The wind speed variable for ct lookup
+
+        """
         super().__init__()
         self.thrust_var = thrust_var
         self.WSCT = var_ws_ct
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return [FV.CT]
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         ct = fdata[FV.CT]
 
         T = self.get_data(self.thrust_var, fdata, st_sel)
```

### Comparing `foxes-0.3.5/foxes/models/turbine_models/yaw2yawm.py` & `foxes-0.4.0/foxes/models/turbine_models/yaw2yawm.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,55 +5,58 @@
 from foxes.utils import delta_wd
 
 
 class YAW2YAWM(TurbineModel):
     """
     Calculates delta yaw (i.e. YAWM) from absolute
     yaw (i.e. YAW)
+
+    :group: models.turbine_models
+    
     """
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return [FV.YAWM]
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         yaw = self.get_data(FV.YAW, fdata, st_sel)
         wd = self.get_data(FV.WD, fdata, st_sel)
```

### Comparing `foxes-0.3.5/foxes/models/turbine_models/yawm2yaw.py` & `foxes-0.4.0/foxes/models/turbine_models/yawm2yaw.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,55 +4,58 @@
 import foxes.variables as FV
 
 
 class YAWM2YAW(TurbineModel):
     """
     Calculates absolute yaw (i.e. YAWM) from delta
     yaw (i.e. YAWM)
+
+    :group: models.turbine_models
+    
     """
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return [FV.YAW]
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         yawm = self.get_data(FV.YAWM, fdata, st_sel)
         wd = self.get_data(FV.WD, fdata, st_sel)
```

### Comparing `foxes-0.3.5/foxes/models/turbine_types/CpCt_file.py` & `foxes-0.4.0/foxes/models/turbine_types/CpCt_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,40 +7,46 @@
 
 
 class CpCtFile(PCtFile):
     """
     Calculate power and ct by interpolating
     from cp-ct-curve data file (or pandas DataFrame).
 
-    Parameters
-    ----------
-    data_source : str or pandas.DataFrame
-        The file path, static name, or data
-    col_ws : str
-        The wind speed column
-    col_cp : str
-        The cp column
-    rho : float
-        The air density for the curves
-    pd_file_read_pars : dict
-        Parameters for pandas file reading
-    paramerers : dict, optional
-        Additional parameters for PCtFile class
+    :group: models.turbine_types
 
     """
 
     def __init__(
         self,
         data_source,
         col_ws="ws",
         col_cp="cp",
         rho=1.225,
         pd_file_read_pars={},
         **parameters,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        data_source: str or pandas.DataFrame
+            The file path, static name, or data
+        col_ws: str
+            The wind speed column
+        col_cp: str
+            The cp column
+        rho: float
+            The air density for the curves
+        pd_file_read_pars: dict
+            Parameters for pandas file reading
+        paramerers: dict, optional
+            Additional parameters for PCtFile class
+
+        """
         if not isinstance(data_source, pd.DataFrame):
             pars = parse_Pct_file_name(data_source)
             pars.update(parameters)
             data = PandasFileHelper.read_file(data_source, **pd_file_read_pars)
         else:
             data = data_source
             pars = parameters
```

### Comparing `foxes-0.3.5/foxes/models/turbine_types/CpCt_from_two.py` & `foxes-0.4.0/foxes/models/turbine_types/CpCt_from_two.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,46 +9,52 @@
 
 class CpCtFromTwo(PCtFromTwo):
     """
     Calculate power and ct by interpolating
     cp and ct from two files (or two pandas
     DataFrames).
 
-    Parameters
-    ----------
-    data_source_cp : str or pandas.DataFrame
-        The file path, static name, or data
-    data_source_ct : str or pandas.DataFrame
-        The file path, static name, or data
-    col_ws_cp_file : str
-        The wind speed column in the file of the cp curve
-    col_cp : str
-        The cp column
-    rho : float
-        The air density for the curves
-    pd_file_read_pars_cp:  dict
-        Parameters for pandas cp file reading
-    pd_file_read_pars_ct:  dict
-        Parameters for pandas ct file reading
-    paramerers : dict, optional
-        Additional parameters for PCtFile class
+    :group: models.turbine_types
 
     """
 
     def __init__(
         self,
         data_source_cp,
         data_source_ct,
         col_ws_cp_file="ws",
         col_cp="cp",
         rho=1.225,
         pd_file_read_pars_cp={},
         pd_file_read_pars_ct={},
         **parameters,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        data_source_cp: str or pandas.DataFrame
+            The file path, static name, or data
+        data_source_ct: str or pandas.DataFrame
+            The file path, static name, or data
+        col_ws_cp_file: str
+            The wind speed column in the file of the cp curve
+        col_cp: str
+            The cp column
+        rho: float
+            The air density for the curves
+        pd_file_read_pars_cp:  dict
+            Parameters for pandas cp file reading
+        pd_file_read_pars_ct:  dict
+            Parameters for pandas ct file reading
+        parameters: dict, optional
+            Additional parameters for PCtFile class
+
+        """
         if not isinstance(data_source_cp, pd.DataFrame) or not isinstance(
             data_source_ct, pd.DataFrame
         ):
             pars = parse_Pct_two_files(data_source_cp, data_source_ct)
             data_cp = PandasFileHelper.read_file(data_source_cp, **pd_file_read_pars_cp)
             data_ct = PandasFileHelper.read_file(data_source_ct, **pd_file_read_pars_ct)
         else:
```

### Comparing `foxes-0.3.5/foxes/models/turbine_types/PCt_file.py` & `foxes-0.4.0/foxes/models/turbine_types/PCt_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,60 +10,36 @@
 
 
 class PCtFile(TurbineType):
     """
     Calculate power and ct by interpolating
     from power-ct-curve data file (or pandas DataFrame).
 
-    Parameters
-    ----------
-    data_source : str or pandas.DataFrame
-        The file path, static name, or data
-    col_ws : str
-        The wind speed column
-    col_P : str
-        The power column
-    col_ct : str
-        The ct column
-    rho: float, optional
-        The air densitiy for which the data is valid
-        or None for no correction
-    p_ct: float
-        The exponent for yaw dependency of ct
-    p_P: float
-        The exponent for yaw dependency of P
-    var_ws_ct : str
-        The wind speed variable for ct lookup
-    var_ws_P : str
-        The wind speed variable for power lookup
-    pd_file_read_pars : dict
-        Parameters for pandas file reading
-    paramerers : dict, optional
-        Additional parameters for TurbineType class
-
     Attributes
     ----------
-    source : str or pandas.DataFrame
+    source: str or pandas.DataFrame
         The file path, static name, or data
-    col_ws : str
+    col_ws: str
         The wind speed column
-    col_P : str
+    col_P: str
         The power column
-    col_ct : str
+    col_ct: str
         The ct column
     rho: float
         The air densitiy for which the data is valid
         or None for no correction
-    WSCT : str
+    WSCT: str
         The wind speed variable for ct lookup
-    WSP : str
+    WSP: str
         The wind speed variable for power lookup
-    rpars : dict, optional
+    rpars: dict, optional
         Parameters for pandas file reading
 
+    :group: models.turbine_types
+
     """
 
     def __init__(
         self,
         data_source,
         col_ws="ws",
         col_P="P",
@@ -72,14 +48,44 @@
         p_ct=1.0,
         p_P=1.88,
         var_ws_ct=FV.REWS2,
         var_ws_P=FV.REWS3,
         pd_file_read_pars={},
         **parameters,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        data_source: str or pandas.DataFrame
+            The file path, static name, or data
+        col_ws: str
+            The wind speed column
+        col_P: str
+            The power column
+        col_ct: str
+            The ct column
+        rho: float, optional
+            The air densitiy for which the data is valid
+            or None for no correction
+        p_ct: float
+            The exponent for yaw dependency of ct
+        p_P: float
+            The exponent for yaw dependency of P
+        var_ws_ct: str
+            The wind speed variable for ct lookup
+        var_ws_P: str
+            The wind speed variable for power lookup
+        pd_file_read_pars: dict
+            Parameters for pandas file reading
+        parameters: dict, optional
+            Additional parameters for TurbineType class
+
+        """
         if not isinstance(data_source, pd.DataFrame):
             pars = parse_Pct_file_name(data_source)
             pars.update(parameters)
         else:
             pars = parameters
 
         super().__init__(**pars)
@@ -97,20 +103,20 @@
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return [FV.P, FV.CT]
 
     def initialize(self, algo, verbosity=0):
         """
@@ -120,22 +126,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         if isinstance(self.source, pd.DataFrame):
             data = self.source
@@ -170,27 +176,27 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         rews2 = fdata[self.WSCT][st_sel]
         rews3 = fdata[self.WSP][st_sel]
 
@@ -237,15 +243,15 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level
 
         """
         del self.data_ws, self.data_P, self.data_ct
         super().finalize(algo, verbosity)
```

### Comparing `foxes-0.3.5/foxes/models/turbine_types/PCt_from_two.py` & `foxes-0.4.0/foxes/models/turbine_types/PCt_from_two.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,70 +9,40 @@
 
 
 class PCtFromTwo(TurbineType):
     """
     Calculate power and ct by interpolating
     from power curve and ct curve data files.
 
-    Parameters
-    ----------
-    data_source_P : str or pandas.DataFrame
-        The file path for the power curve, static name, or data
-    data_source_ct : str or pandas.DataFrame
-        The file path for the ct curve, static name, or data
-    col_ws_P_file : str
-        The wind speed column in the file of the power curve
-    col_ws_ct_file : str
-        The wind speed column in the file of the ct curve
-    col_P : str
-        The power column
-    col_ct : str
-        The ct column
-    rho: float, optional
-        The air densitiy for which the data is valid
-        or None for no correction
-    p_ct: float
-        The exponent for yaw dependency of ct
-    p_P: float
-        The exponent for yaw dependency of P
-    var_ws_ct : str
-        The wind speed variable for ct lookup
-    var_ws_P : str
-        The wind speed variable for power lookup
-    pd_file_read_pars_P:  dict
-        Parameters for pandas power file reading
-    pd_file_read_pars_ct:  dict
-        Parameters for pandas ct file reading
-    parameters : dict, optional
-        Additional parameters for TurbineType class
-
     Attributes
     ----------
-    source_P : str or pandas.DataFrame
+    source_P: str or pandas.DataFrame
         The file path for the power curve, static name, or data
-    source_ct : str or pandas.DataFrame
+    source_ct: str or pandas.DataFrame
         The file path for the ct curve, static name, or data
-    col_ws : str
+    col_ws: str
         The wind speed column
-    col_P : str
+    col_P: str
         The power column
-    col_ct : str
+    col_ct: str
         The ct column
     rho: float
         The air densitiy for which the data is valid
         or None for no correction
-    WSCT : str
+    WSCT: str
         The wind speed variable for ct lookup
-    WSP : str
+    WSP: str
         The wind speed variable for power lookup
-    rpars_P : dict, optional
+    rpars_P: dict, optional
         Parameters for pandas power file reading
-    rpars_ct : dict, optional
+    rpars_ct: dict, optional
         Parameters for pandas ct file reading
 
+    :group: models.turbine_types
+
     """
 
     def __init__(
         self,
         data_source_P,
         data_source_ct,
         col_ws_P_file="ws",
@@ -84,14 +54,50 @@
         p_P=1.88,
         var_ws_ct=FV.REWS2,
         var_ws_P=FV.REWS3,
         pd_file_read_pars_P={},
         pd_file_read_pars_ct={},
         **parameters,
     ):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        data_source_P: str or pandas.DataFrame
+            The file path for the power curve, static name, or data
+        data_source_ct: str or pandas.DataFrame
+            The file path for the ct curve, static name, or data
+        col_ws_P_file: str
+            The wind speed column in the file of the power curve
+        col_ws_ct_file: str
+            The wind speed column in the file of the ct curve
+        col_P: str
+            The power column
+        col_ct: str
+            The ct column
+        rho: float, optional
+            The air densitiy for which the data is valid
+            or None for no correction
+        p_ct: float
+            The exponent for yaw dependency of ct
+        p_P: float
+            The exponent for yaw dependency of P
+        var_ws_ct: str
+            The wind speed variable for ct lookup
+        var_ws_P: str
+            The wind speed variable for power lookup
+        pd_file_read_pars_P:  dict
+            Parameters for pandas power file reading
+        pd_file_read_pars_ct:  dict
+            Parameters for pandas ct file reading
+        parameters: dict, optional
+            Additional parameters for TurbineType class
+
+        """
         if not isinstance(data_source_P, pd.DataFrame) or not isinstance(
             data_source_ct, pd.DataFrame
         ):
             pars = parse_Pct_two_files(data_source_P, data_source_ct)
         else:
             pars = parameters
         super().__init__(**pars)
@@ -117,20 +123,20 @@
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return [FV.P, FV.CT]
 
     def initialize(self, algo, verbosity=0):
         """
@@ -140,22 +146,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         # read power curve:
         if isinstance(self.source_P, pd.DataFrame):
@@ -193,27 +199,27 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         rews2 = fdata[self.WSCT][st_sel]
         rews3 = fdata[self.WSP][st_sel]
 
@@ -259,15 +265,15 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level
 
         """
         del self._data_ws_P, self._data_ws_ct, self._data_P, self._data_ct
         super().finalize(algo, verbosity)
```

### Comparing `foxes-0.3.5/foxes/models/turbine_types/null_type.py` & `foxes-0.4.0/foxes/models/turbine_types/null_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 from foxes.core import TurbineType
 
 
 class NullType(TurbineType):
     """
     A turbine type that does not compute any data.
+
+    :group: models.turbine_types
+    
     """
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return []
 
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         return {}
```

### Comparing `foxes-0.3.5/foxes/models/turbine_types/wsrho2PCt_two_files.py` & `foxes-0.4.0/foxes/models/turbine_types/wsrho2PCt_from_two.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,71 +5,48 @@
 from foxes.core import TurbineType
 from foxes.utils import PandasFileHelper
 from foxes.data import PCTCURVE, parse_Pct_two_files
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class WsRho2PCtTwoFiles(TurbineType):
+class WsRho2PCtFromTwo(TurbineType):
     """
     Calculate air density dependent power
     and ct values, as given by two individual
     files.
 
     The structure of each file is:
     ws,1.225,0.950,0.975,...,1.275
 
     The first column represents wind speed in m/s
     and the subsequent columns are air density values
     (not neccessarily in order).
 
-    Parameters
-    ----------
-    data_source_P : str or pandas.DataFrame
-        The file path for the power curve, static name, or data
-    data_source_ct : str or pandas.DataFrame
-        The file path for the ct curve, static name, or data
-    p_ct: float
-        The exponent for yaw dependency of ct
-    p_P: float
-        The exponent for yaw dependency of P
-    var_ws_ct : str
-        The wind speed variable for ct lookup
-    var_ws_P : str
-        The wind speed variable for power lookup
-    pd_file_read_pars_P:  dict
-        Parameters for pandas power file reading
-    pd_file_read_pars_ct:  dict
-        Parameters for pandas ct file reading
-    interpn_pars_P : dict, optional
-        Parameters for scipy.interpolate.interpn()
-    interpn_pars_ct : dict, optional
-        Parameters for scipy.interpolate.interpn()
-    parameters : dict, optional
-        Additional parameters for TurbineType class
-
     Attributes
     ----------
-    source_P : str or pandas.DataFrame
+    source_P: str or pandas.DataFrame
         The file path for the power curve, static name, or data
-    source_ct : str or pandas.DataFrame
+    source_ct: str or pandas.DataFrame
         The file path for the ct curve, static name, or data
-    WSCT : str
+    WSCT: str
         The wind speed variable for ct lookup
-    WSP : str
+    WSP: str
         The wind speed variable for power lookup
-    rpars_P : dict, optional
+    rpars_P: dict, optional
         Parameters for pandas power file reading
-    rpars_ct : dict, optional
+    rpars_ct: dict, optional
         Parameters for pandas ct file reading
-    ipars_P : dict, optional
+    ipars_P: dict, optional
         Parameters for scipy.interpolate.interpn()
-    ipars_ct : dict, optional
+    ipars_ct: dict, optional
         Parameters for scipy.interpolate.interpn()
 
+    :group: models.turbine_types
+
     """
 
     def __init__(
         self,
         data_source_P,
         data_source_ct,
         p_ct=1.0,
@@ -78,14 +55,43 @@
         var_ws_P=FV.REWS3,
         pd_file_read_pars_P={},
         pd_file_read_pars_ct={},
         interpn_pars_P=None,
         interpn_pars_ct=None,
         **parameters,
     ):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        data_source_P: str or pandas.DataFrame
+            The file path for the power curve, static name, or data
+        data_source_ct: str or pandas.DataFrame
+            The file path for the ct curve, static name, or data
+        p_ct: float
+            The exponent for yaw dependency of ct
+        p_P: float
+            The exponent for yaw dependency of P
+        var_ws_ct: str
+            The wind speed variable for ct lookup
+        var_ws_P: str
+            The wind speed variable for power lookup
+        pd_file_read_pars_P:  dict
+            Parameters for pandas power file reading
+        pd_file_read_pars_ct:  dict
+            Parameters for pandas ct file reading
+        interpn_pars_P: dict, optional
+            Parameters for scipy.interpolate.interpn()
+        interpn_pars_ct: dict, optional
+            Parameters for scipy.interpolate.interpn()
+        parameters: dict, optional
+            Additional parameters for TurbineType class
+
+        """
         if not isinstance(data_source_P, pd.DataFrame) or not isinstance(
             data_source_ct, pd.DataFrame
         ):
             pars = parse_Pct_two_files(data_source_P, data_source_ct)
         else:
             pars = parameters
         super().__init__(**pars)
@@ -111,20 +117,20 @@
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return [FV.P, FV.CT]
 
     def initialize(self, algo, verbosity=0):
         """
@@ -134,22 +140,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         # read power curve:
         if isinstance(self.source_P, pd.DataFrame):
@@ -205,27 +211,27 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        st_sel : numpy.ndarray of bool
+        st_sel: numpy.ndarray of bool
             The state-turbine selection,
             shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
 
         # calculate P:
         st_sel_P = (
@@ -310,17 +316,17 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level
 
         """
         del self._ws_P, self._rho_P, self._ws_ct, self._rho_ct
         self._P = None
         self._ct = None
         super().finalize(algo, verbosity)
```

### Comparing `foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_neutral_ws.py` & `foxes-0.4.0/foxes/models/vertical_profiles/abl_log_unstable_ws.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 from foxes.core import VerticalProfile
-from foxes.utils.abl import neutral
+from foxes.utils.abl import unstable
 import foxes.constants as FC
 import foxes.variables as FV
 
 
-class ABLLogNeutralWsProfile(VerticalProfile):
+class ABLLogUnstableWsProfile(VerticalProfile):
     """
-    The neutral ABL wind speed log profile.
+    The unstable ABL wind speed log profile.
+
+    :group: models.vertical_profiles
+    
     """
 
     def input_vars(self):
         """
         The input variables needed for the profile
         calculation.
 
         Returns
         -------
-        vars : list of str
+        vars: list of str
             The variable names
 
         """
-        return [FV.WS, FV.H, FV.Z0]
+        return [FV.WS, FV.H, FV.Z0, FV.MOL]
 
     def calculate(self, data, heights):
         """
         Run the profile calculation.
 
         Parameters
         ----------
-        data : dict
+        data: dict
             The input data
-        heights : numpy.ndarray
+        heights: numpy.ndarray
             The evaluation heights
 
         Returns
         -------
-        results : numpy.ndarray
+        results: numpy.ndarray
             The profile results, same
             shape as heights
 
         """
-        z0 = data[FV.Z0]
-        h0 = data[FV.H]
         ws = data[FV.WS]
+        h0 = data[FV.H]
+        z0 = data[FV.Z0]
+        mol = data[FV.MOL]
 
-        ustar = neutral.ustar(ws, h0, z0, kappa=FC.KAPPA)
+        ustar = unstable.ustar(ws, h0, z0, mol, kappa=FC.KAPPA)
+        psi = unstable.psi(heights, mol)
 
-        return neutral.calc_ws(heights, z0, ustar, kappa=FC.KAPPA)
+        return unstable.calc_ws(heights, z0, ustar, psi, kappa=FC.KAPPA)
```

### Comparing `foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_stable_ws.py` & `foxes-0.4.0/foxes/models/vertical_profiles/abl_log_stable_ws.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,43 +3,46 @@
 import foxes.constants as FC
 import foxes.variables as FV
 
 
 class ABLLogStableWsProfile(VerticalProfile):
     """
     The stable ABL wind speed log profile.
+
+    :group: models.vertical_profiles
+    
     """
 
     def input_vars(self):
         """
         The input variables needed for the profile
         calculation.
 
         Returns
         -------
-        vars : list of str
+        vars: list of str
             The variable names
 
         """
         return [FV.WS, FV.H, FV.Z0, FV.MOL]
 
     def calculate(self, data, heights):
         """
         Run the profile calculation.
 
         Parameters
         ----------
-        data : dict
+        data: dict
             The input data
-        heights : numpy.ndarray
+        heights: numpy.ndarray
             The evaluation heights
 
         Returns
         -------
-        results : numpy.ndarray
+        results: numpy.ndarray
             The profile results, same
             shape as heights
 
         """
         ws = data[FV.WS]
         h0 = data[FV.H]
         z0 = data[FV.Z0]
```

### Comparing `foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_unstable_ws.py` & `foxes-0.4.0/foxes/models/vertical_profiles/sheared_ws.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,60 @@
+import numpy as np
+
 from foxes.core import VerticalProfile
-from foxes.utils.abl import unstable
-import foxes.constants as FC
+from foxes.utils import abl
 import foxes.variables as FV
 
 
-class ABLLogUnstableWsProfile(VerticalProfile):
+class ShearedProfile(VerticalProfile):
     """
-    The unstable ABL wind speed log profile.
+    A wind shear profile, based on a shear exponent.
+    
+    :group: models.vertical_profiles
+    
     """
 
     def input_vars(self):
         """
         The input variables needed for the profile
         calculation.
 
         Returns
         -------
-        vars : list of str
+        vars: list of str
             The variable names
-
+            
         """
-        return [FV.WS, FV.H, FV.Z0, FV.MOL]
+        return [FV.WS, FV.H, FV.SHEAR]
 
     def calculate(self, data, heights):
         """
         Run the profile calculation.
 
         Parameters
         ----------
-        data : dict
+        data: dict
             The input data
-        heights : numpy.ndarray
+        heights: numpy.ndarray
             The evaluation heights
 
         Returns
         -------
-        results : numpy.ndarray
+        results: numpy.ndarray
             The profile results, same
             shape as heights
 
         """
-        ws = data[FV.WS]
-        h0 = data[FV.H]
-        z0 = data[FV.Z0]
-        mol = data[FV.MOL]
 
-        ustar = unstable.ustar(ws, h0, z0, mol, kappa=FC.KAPPA)
-        psi = unstable.psi(heights, mol)
+        ws = np.zeros_like(heights)
+        ws[:] = data[FV.WS]
+
+        h0 = np.zeros_like(heights)
+        h0[:] = data[FV.H]
+
+        shear = np.zeros_like(heights)
+        shear[:] = data[FV.SHEAR]
+
+        out = np.zeros_like(heights)
+        out[:] = abl.sheared.calc_ws(heights, h0, ws, shear)
 
-        return unstable.calc_ws(heights, z0, ustar, psi, kappa=FC.KAPPA)
+        return out
```

### Comparing `foxes-0.3.5/foxes/models/vertical_profiles/abl_log/abl_log_ws.py` & `foxes-0.4.0/foxes/models/vertical_profiles/abl_log_ws.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,43 +8,46 @@
 
 class ABLLogWsProfile(VerticalProfile):
     """
     The neutral/stable/unstable ABL wind speed log profile.
 
     This profile picks the profile according to the mol value
     (neutral: mol = None or mol = 0)
+
+    :group: models.vertical_profiles
+    
     """
 
     def input_vars(self):
         """
         The input variables needed for the profile
         calculation.
 
         Returns
         -------
-        vars : list of str
+        vars: list of str
             The variable names
 
         """
         return [FV.WS, FV.H, FV.Z0, FV.MOL]
 
     def calculate(self, data, heights):
         """
         Run the profile calculation.
 
         Parameters
         ----------
-        data : dict
+        data: dict
             The input data
-        heights : numpy.ndarray
+        heights: numpy.ndarray
             The evaluation heights
 
         Returns
         -------
-        results : numpy.ndarray
+        results: numpy.ndarray
             The profile results, same
             shape as heights
 
         """
         ws = np.zeros_like(heights)
         ws[:] = data[FV.WS]
```

### Comparing `foxes-0.3.5/foxes/models/wake_frames/farm_order.py` & `foxes-0.4.0/foxes/models/wake_frames/farm_order.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,27 +10,33 @@
     Invokes turbine ordering as defined
     by the wind farm.
 
     Warning: This is for testing purposes only, and in general
     only gives correct calculation results when used
     in an iterative algorithm.
 
-    Parameters
-    ----------
-    base_frame : foxes.core.WakeFrame
-        The wake frame from which to start
-
     Attributes
     ----------
-    base_frame : foxes.core.WakeFrame
+    base_frame: foxes.core.WakeFrame
         The wake frame from which to start
 
+    :group: models.wake_frames
+
     """
 
     def __init__(self, base_frame=RotorWD()):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        base_frame: foxes.core.WakeFrame
+            The wake frame from which to start
+
+        """
         super().__init__()
         self.base_frame = base_frame
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
@@ -38,22 +44,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
         algo.update_idata(self.base_frame, idata=idata, verbosity=verbosity)
@@ -65,97 +71,97 @@
         Calculates the order of turbine evaluation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        order : numpy.ndarray
+        order: numpy.ndarray
             The turbine order, shape: (n_states, n_turbines)
 
         """
         order = np.zeros((fdata.n_states, fdata.n_turbines), dtype=FC.ITYPE)
         order[:] = np.arange(fdata.n_turbines)[None, :]
 
         return order
 
     def get_wake_coos(self, algo, mdata, fdata, states_source_turbine, points):
         """
         Calculate wake coordinates.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        points : numpy.ndarray
+        points: numpy.ndarray
             The evaluation points, shape: (n_states, n_points, 3)
 
         Returns
         -------
-        wake_coos : numpy.ndarray
+        wake_coos: numpy.ndarray
             The wake coordinates, shape: (n_states, n_points, 3)
 
         """
         return self.base_frame.get_wake_coos(
             algo, mdata, fdata, states_source_turbine, points
         )
 
     def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
         """
         Gets the points along the centreline for given
         values of x.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
 
         Returns
         -------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
 
         """
         return self.base_frame.get_centreline_points(
             algo, mdata, fdata, states_source_turbine, x
         )
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         if self.base_frame.initialized:
             self.base_frame.finalize(algo, verbosity)
         super().finalize(algo, verbosity)
```

### Comparing `foxes-0.3.5/foxes/models/wake_frames/rotor_wd.py` & `foxes-0.4.0/foxes/models/wake_frames/rotor_wd.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,49 +7,55 @@
 
 
 class RotorWD(WakeFrame):
     """
     Align the first axis for each rotor with the
     local normalized wind direction.
 
-    Parameters
-    ----------
-    var_wd : str
-        The wind direction variable
-
     Attributes
     ----------
-    var_wd : str
+    var_wd: str
         The wind direction variable
 
+    :group: models.wake_frames
+
     """
 
     def __init__(self, var_wd=FV.WD):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        var_wd: str
+            The wind direction variable
+
+        """
         super().__init__()
         self.var_wd = var_wd
 
     def calc_order(self, algo, mdata, fdata):
         """ "
         Calculates the order of turbine evaluation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        order : numpy.ndarray
+        order: numpy.ndarray
             The turbine order, shape: (n_states, n_turbines)
 
         """
         n = np.mean(wd2uv(fdata[self.var_wd], axis=1), axis=-1)
         xy = fdata[FV.TXYH][:, :, :2]
 
         order = np.argsort(np.einsum("std,sd->st", xy, n), axis=-1)
@@ -58,29 +64,29 @@
 
     def get_wake_coos(self, algo, mdata, fdata, states_source_turbine, points):
         """
         Calculate wake coordinates.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        points : numpy.ndarray
+        points: numpy.ndarray
             The evaluation points, shape: (n_states, n_points, 3)
 
         Returns
         -------
-        wake_coos : numpy.ndarray
+        wake_coos: numpy.ndarray
             The wake coordinates, shape: (n_states, n_points, 3)
 
         """
         n_states = mdata.n_states
         stsel = (np.arange(n_states), states_source_turbine)
 
         xyz = fdata[FV.TXYH][stsel]
@@ -104,29 +110,29 @@
     def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
         """
         Gets the points along the centreline for given
         values of x.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
 
         Returns
         -------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
 
         """
         n_states = mdata.n_states
         stsel = (np.arange(n_states), states_source_turbine)
 
         wd = fdata[self.var_wd][stsel]
```

### Comparing `foxes-0.3.5/foxes/models/wake_frames/streamlines.py` & `foxes-0.4.0/foxes/models/wake_frames/streamlines.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,41 +8,47 @@
 import foxes.constants as FC
 
 
 class Streamlines(WakeFrame):
     """
     Streamline following wakes
 
-    Parameters
-    ----------
-    step : float
-        The streamline step size in m
-    n_delstor : int
-        The streamline point storage increase
-    max_length : float
-        The maximal streamline length
-    cl_ipars : dict
-        Interpolation parameters for centre line
-        point interpolation
-
     Attributes
     ----------
-    step : float
+    step: float
         The streamline step size in m
-    n_delstor : int
+    n_delstor: int
         The streamline point storage increase
-    max_length : float
+    max_length: float
         The maximal streamline length
-    cl_ipars : dict
+    cl_ipars: dict
         Interpolation parameters for centre line
         point interpolation
+    
+    :group: models.wake_frames
 
     """
 
     def __init__(self, step, n_delstor=100, max_length=1e5, cl_ipars={}):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        step: float
+            The streamline step size in m
+        n_delstor: int
+            The streamline point storage increase
+        max_length: float
+            The maximal streamline length
+        cl_ipars: dict
+            Interpolation parameters for centre line
+            point interpolation
+
+        """
         super().__init__()
         self.step = step
         self.n_delstor = n_delstor
         self.max_length = max_length
         self.cl_ipars = cl_ipars
 
     def __repr__(self):
@@ -56,22 +62,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.DATA = self.var("DATA")
         self.CNTR = self.var("CNTR")
@@ -242,24 +248,24 @@
         Calculates the order of turbine evaluation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        order : numpy.ndarray
+        order: numpy.ndarray
             The turbine order, shape: (n_states, n_turbines)
 
         """
 
         # prepare:
         n_states = mdata.n_states
         n_turbines = mdata.n_turbines
@@ -282,29 +288,29 @@
 
     def get_wake_coos(self, algo, mdata, fdata, states_source_turbine, points):
         """
         Calculate wake coordinates.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        points : numpy.ndarray
+        points: numpy.ndarray
             The evaluation points, shape: (n_states, n_points, 3)
 
         Returns
         -------
-        wake_coos : numpy.ndarray
+        wake_coos: numpy.ndarray
             The wake coordinates, shape: (n_states, n_points, 3)
 
         """
 
         # prepare:
         n_states = mdata.n_states
         stsel = (np.arange(n_states), states_source_turbine)
@@ -325,29 +331,29 @@
     def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
         """
         Gets the points along the centreline for given
         values of x.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
 
         Returns
         -------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
 
         """
         # calculate long enough streamlines:
         xmax = np.max(x)
         self._ensure_min_length(algo, mdata, fdata, xmax)
```

### Comparing `foxes-0.3.5/foxes/models/wake_frames/yawed_wakes.py` & `foxes-0.4.0/foxes/models/wake_frames/yawed_wakes.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,57 +9,63 @@
 
 class YawedWakes(WakeFrame):
     """
     Bend the wakes for yawed turbines.
 
     Based on Bastankhah & Porte-Agel, 2016, https://doi.org/10.1017/jfm.2016.595
 
-    Parameters
-    ----------
-    k : float, optional
-        The wake growth parameter k. If not given here
-        it will be searched in the farm data, by default None
-    ct_max : float, optional
-        The maximal value for ct, values beyond will be limited
-        to this number, by default 0.9999
-    alpha : float, optional
-        model parameter used to determine onset of far wake region
-    beta : float, optional
-        model parameter used to determine onset of far wake region
-    base_frame : foxes.core.WakeFrame
-        The wake frame from which to start
-    k_var : str
-        The variable name for k
-
     Attributes
     ----------
-    model : PorteAgelModel
+    model: PorteAgelModel
         The model for computing common data
-    K : float
+    K: float
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
-    YAWM : float
+    YAWM: float
         The yaw misalignment YAWM. If not given here
         it will be searched in the farm data.
-    base_frame : foxes.core.WakeFrame
+    base_frame: foxes.core.WakeFrame
         The wake frame from which to start
-    k_var : str
+    k_var: str
         The variable name for k
+    
+    :group: models.wake_frames
 
     """
 
     def __init__(
         self,
         k=None,
         ct_max=0.9999,
-        alpha=0.58,
+        alpha=0.58, 
         beta=0.07,
         base_frame=RotorWD(),
         k_var=FV.K,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        k: float, optional
+            The wake growth parameter k. If not given here
+            it will be searched in the farm data, by default None
+        ct_max: float, optional
+            The maximal value for ct, values beyond will be limited
+            to this number, by default 0.9999
+        alpha: float, optional
+            model parameter used to determine onset of far wake region
+        beta: float, optional
+            model parameter used to determine onset of far wake region
+        base_frame: foxes.core.WakeFrame
+            The wake frame from which to start
+        k_var: str
+            The variable name for k
+
+        """
         super().__init__()
 
         self.base_frame = base_frame
         self.model = PorteAgelModel(ct_max, alpha, beta)
         self.k_var = k_var
 
         setattr(self, k_var, k)
@@ -73,22 +79,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
         algo.update_idata(self.base_frame, idata=idata, verbosity=verbosity)
@@ -100,24 +106,24 @@
         Calculates the order of turbine evaluation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        order : numpy.ndarray
+        order: numpy.ndarray
             The turbine order, shape: (n_states, n_turbines)
 
         """
         return self.base_frame.calc_order(algo, mdata, fdata)
 
     def _update_y(self, mdata, fdata, states_source_turbine, x, y):
         """
@@ -174,29 +180,29 @@
 
     def get_wake_coos(self, algo, mdata, fdata, states_source_turbine, points):
         """
         Calculate wake coordinates.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        points : numpy.ndarray
+        points: numpy.ndarray
             The evaluation points, shape: (n_states, n_points, 3)
 
         Returns
         -------
-        wake_coos : numpy.ndarray
+        wake_coos: numpy.ndarray
             The wake coordinates, shape: (n_states, n_points, 3)
 
         """
         # get unyawed results:
         xyz = self.base_frame.get_wake_coos(
             algo, mdata, fdata, states_source_turbine, points
         )
@@ -211,29 +217,29 @@
     def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
         """
         Gets the points along the centreline for given
         values of x.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The wake frame x coordinates, shape: (n_states, n_points)
 
         Returns
         -------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The centreline points, shape: (n_states, n_points, 3)
 
         """
         points = self.base_frame.get_centreline_points(
             algo, mdata, fdata, states_source_turbine, x
         )
 
@@ -259,16 +265,16 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         if self.base_frame.initialized:
             self.base_frame.finalize(algo, verbosity)
         super().finalize(algo, verbosity)
```

### Comparing `foxes-0.3.5/foxes/models/wake_models/axisymmetric.py` & `foxes-0.4.0/foxes/models/wake_models/axisymmetric.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,77 +7,80 @@
 class AxisymmetricWakeModel(DistSlicedWakeModel):
     """
     Abstract base class for wake models
     that depend on (x, r) separately.
 
     The ability to evaluate multiple r values per x
     is used by the `PartialAxiwake` partial wakes model.
+
+    :group: models.wake_models
+    
     """
 
     @abstractmethod
     def calc_wakes_spsel_x_r(self, algo, mdata, fdata, states_source_turbine, x, r):
         """
         Calculate wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
-        r : numpy.ndarray
+        r: numpy.ndarray
             The radial values for each x value, shape:
             (n_states, n_points, n_r_per_x, 2)
 
         Returns
         -------
-        wdeltas : dict
+        wdeltas: dict
             The wake deltas. Key: variable name str,
             value: numpy.ndarray, shape: (n_sp_sel, n_r_per_x)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
         pass
 
     def calc_wakes_spsel_x_yz(self, algo, mdata, fdata, states_source_turbine, x, yz):
         """
         Calculate wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
-        yz : numpy.ndarray
+        yz: numpy.ndarray
             The yz values for each x value, shape:
             (n_states, n_points, n_yz_per_x, 2)
 
         Returns
         -------
-        wdeltas : dict
+        wdeltas: dict
             The wake deltas. Key: variable name str,
             value: numpy.ndarray, shape: (n_sp_sel, n_yz_per_x)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
         r = np.linalg.norm(yz, axis=-1)
         return self.calc_wakes_spsel_x_r(
             algo, mdata, fdata, states_source_turbine, x, r
```

### Comparing `foxes-0.3.5/foxes/models/wake_models/dist_sliced.py` & `foxes-0.4.0/foxes/models/wake_models/dist_sliced.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,40 @@
     Abstract base class for wake models for which
     the x-denpendency can be separated from the
     yz-dependency.
 
     The multi-yz ability is used by the `PartialDistSlicedWake`
     partial wakes model.
 
-    Parameters
-    ----------
-    superpositions : dict
-        The superpositions. Key: variable name str,
-        value: The wake superposition model name,
-        will be looked up in model book
-
     Attributes
     ----------
-    superpositions : dict
+    superpositions: dict
         The superpositions. Key: variable name str,
         value: The wake superposition model name,
         will be looked up in model book
-    superp : dict
+    superp: dict
         The superposition dict, key: variable name str,
         value: `foxes.core.WakeSuperposition`
 
+    :group: models.wake_models
+
     """
 
     def __init__(self, superpositions):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        superpositions: dict
+            The superpositions. Key: variable name str,
+            value: The wake superposition model name,
+            will be looked up in model book
+
+        """
         super().__init__()
         self.superpositions = superpositions
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
@@ -43,22 +49,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.superp = {
             v: algo.mbook.wake_superpositions[s] for v, s in self.superpositions.items()
@@ -72,35 +78,35 @@
     @abstractmethod
     def calc_wakes_spsel_x_yz(self, algo, mdata, fdata, states_source_turbine, x, yz):
         """
         Calculate wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
-        yz : numpy.ndarray
+        yz: numpy.ndarray
             The yz values for each x value, shape:
             (n_states, n_points, n_yz_per_x, 2)
 
         Returns
         -------
-        wdeltas : dict
+        wdeltas: dict
             The wake deltas. Key: variable name str,
             value: numpy.ndarray, shape: (n_sp_sel, n_yz_per_x)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
         pass
 
     def contribute_to_wake_deltas(
@@ -110,27 +116,27 @@
         Calculate the contribution to the wake deltas
         by this wake model.
 
         Modifies wake_deltas on the fly.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        wake_coos : numpy.ndarray
+        wake_coos: numpy.ndarray
             The wake frame coordinates of the evaluation
             points, shape: (n_states, n_points, 3)
-        wake_deltas : dict
+        wake_deltas: dict
             The wake deltas, are being modified ob the fly.
             Key: Variable name str, for which the
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
         x = wake_coos[:, :, 0]
@@ -163,24 +169,24 @@
         """
         Finalize the wake calculation.
 
         Modifies wake_deltas on the fly.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        amb_results : dict
+        amb_results: dict
             The ambient results, key: variable name str,
             values: numpy.ndarray with shape (n_states, n_points)
-        wake_deltas : dict
+        wake_deltas: dict
             The wake deltas, are being modified ob the fly.
             Key: Variable name str, for which the wake delta
             applies, values: numpy.ndarray with shape
             (n_states, n_points, ...) before evaluation,
             numpy.ndarray with shape (n_states, n_points) afterwards
 
         """
@@ -191,16 +197,16 @@
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         for s in self.superp.values():
             s.finalize(algo, verbosity)
         super().finalize(algo, verbosity)
```

### Comparing `foxes-0.3.5/foxes/models/wake_models/gaussian.py` & `foxes-0.4.0/foxes/models/wake_models/gaussian.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,75 +3,78 @@
 
 from foxes.models.wake_models.axisymmetric import AxisymmetricWakeModel
 
 
 class GaussianWakeModel(AxisymmetricWakeModel):
     """
     Abstract base class for Gaussian wake models.
+
+    :group: models.wake_models
+    
     """
 
     @abstractmethod
     def calc_amplitude_sigma_spsel(self, algo, mdata, fdata, states_source_turbine, x):
         """
         Calculate the amplitude and the sigma,
         both depend only on x (not on r).
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
 
         Returns
         -------
-        amsi : tuple
+        amsi: tuple
             The amplitude and sigma, both numpy.ndarray
             with shape (n_sp_sel,)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
         pass
 
     def calc_wakes_spsel_x_r(self, algo, mdata, fdata, states_source_turbine, x, r):
         """
         Calculate wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
-        r : numpy.ndarray
+        r: numpy.ndarray
             The radial values for each x value, shape:
             (n_states, n_points, n_r_per_x)
 
         Returns
         -------
-        wdeltas : dict
+        wdeltas: dict
             The wake deltas. Key: variable name str,
             value: numpy.ndarray, shape: (n_sp_sel, n_r_per_x)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
         amsi, sp_sel = self.calc_amplitude_sigma_spsel(
             algo, mdata, fdata, states_source_turbine, x
         )
```

### Comparing `foxes-0.3.5/foxes/models/wake_models/ti/crespo_hernandez.py` & `foxes-0.4.0/foxes/models/wake_models/ti/crespo_hernandez.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,78 +4,48 @@
 import foxes.variables as FV
 import foxes.constants as FC
 
 
 class CrespoHernandezTIWake(TopHatWakeModel):
     """
     The Crespo and Hernandez TI empirical correlation
+    
     Source: https://doi.org/10.1016/0167-6105(95)00033-X
 
     For the wake diameter we use Eqns. (17), (15), (4), (5) from
             doi:10.1088/1742-6596/625/1/012039
 
-    Parameters
-    ----------
-    superpositions : dict
-        The superpositions. Key: variable name str,
-        value: The wake superposition model name,
-        will be looked up in model book
-    k : float, optional
-        The wake growth parameter k. If not given here
-        it will be searched in the farm data.
-    use_ambti : bool
-        Flag for using ambient TI instead of local
-        wake corrected TI
-    sbeta_factor : float
-        Factor multiplying sbeta
-    near_wake_D : float, optional
-        The near wake distance in units of D,
-        calculated from TI and ct if not given here
-    ct_max : float
-        The maximal value for ct, values beyond will be limited
-        to this number
-    a_near : float
-        Model parameter
-    a_far : float
-        Model parameter
-    e1 : float
-        Model parameter
-    e2 : float
-        Model parameter
-    e3 : float
-        Model parameter
-    k_var : str
-        The variable name for k
-
     Attributes
     ----------
-    k : float
+    k: float
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
-    a_near : float
+    a_near: float
         Model parameter
-    a_far : float
+    a_far: float
         Model parameter
-    e1 : float
+    e1: float
         Model parameter
-    e2 : float
+    e2: float
         Model parameter
-    e3 : float
+    e3: float
         Model parameter
-    use_ambti : bool
+    use_ambti: bool
         Flag for using ambient TI instead of local
         wake corrected TI
-    sbeta_factor : float
+    sbeta_factor: float
         Factor multiplying sbeta
-    near_wake_D : float
+    near_wake_D: float
         The near wake distance in units of D,
         calculated from TI and ct if None
-    k_var : str
+    k_var: str
         The variable name for k
 
+    :group: models.wake_models.ti
+
     """
 
     def __init__(
         self,
         superposition,
         k=None,
         use_ambti=False,
@@ -85,14 +55,51 @@
         a_near=0.362,
         a_far=0.73,
         e1=0.83,
         e2=-0.0325,
         e3=-0.32,
         k_var=FV.K
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        superpositions: dict
+            The superpositions. Key: variable name str,
+            value: The wake superposition model name,
+            will be looked up in model book
+        k: float, optional
+            The wake growth parameter k. If not given here
+            it will be searched in the farm data.
+        use_ambti: bool
+            Flag for using ambient TI instead of local
+            wake corrected TI
+        sbeta_factor: float
+            Factor multiplying sbeta
+        near_wake_D: float, optional
+            The near wake distance in units of D,
+            calculated from TI and ct if not given here
+        ct_max: float
+            The maximal value for ct, values beyond will be limited
+            to this number
+        a_near: float
+            Model parameter
+        a_far: float
+            Model parameter
+        e1: float
+            Model parameter
+        e2: float
+            Model parameter
+        e3: float
+            Model parameter
+        k_var: str
+            The variable name for k
+
+        """
         super().__init__(superpositions={FV.TI: superposition}, ct_max=ct_max)
 
         self.a_near = a_near
         self.a_far = a_far
         self.e1 = e1
         self.e2 = e2
         self.e3 = e3
@@ -113,23 +120,23 @@
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        n_points : int
+        n_points: int
             The number of wake evaluation points
-        wake_deltas : dict
+        wake_deltas: dict
             The wake deltas storage, add wake deltas
             on the fly. Keys: Variable name str, for which the
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
         n_states = mdata.n_states
@@ -137,35 +144,35 @@
 
     def calc_wake_radius(self, algo, mdata, fdata, states_source_turbine, x, ct):
         """
         Calculate the wake radius, depending on x only (not r).
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
-        r : numpy.ndarray
+        r: numpy.ndarray
             The radial values for each x value, shape:
             (n_states, n_points, n_r_per_x, 2)
-        ct : numpy.ndarray
+        ct: numpy.ndarray
             The ct values of the wake-causing turbines,
             shape: (n_states, n_points)
 
         Returns
         -------
-        wake_r : numpy.ndarray
+        wake_r: numpy.ndarray
             The wake radii, shape: (n_states, n_points)
 
         """
         # prepare:
         n_states = fdata.n_states
         st_sel = (np.arange(n_states), states_source_turbine)
 
@@ -187,37 +194,37 @@
         self, algo, mdata, fdata, states_source_turbine, sp_sel, x, wake_r, ct
     ):
         """
         Calculate centre line results of wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_sp_sel,)
-        wake_r : numpy.ndarray
+        wake_r: numpy.ndarray
             The wake radii, shape: (n_sp_sel,)
-        ct : numpy.ndarray
+        ct: numpy.ndarray
             The ct values of the wake-causing turbines,
             shape: (n_sp_sel,)
 
         Returns
         -------
-        cl_del : dict
+        cl_del: dict
             The centre line wake deltas. Key: variable name str,
             varlue: numpy.ndarray, shape: (n_sp_sel,)
 
         """
         # prepare:
         n_states = fdata.n_states
         n_points = sp_sel.shape[1]
```

### Comparing `foxes-0.3.5/foxes/models/wake_models/ti/iec_ti.py` & `foxes-0.4.0/foxes/models/wake_models/ti/iec_ti.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,48 +13,53 @@
     v2: VolLuk: corrected implementation following: IEC-64100-1-2005-8
     (Appearently an error in the document by DTU)
 
     and the Frandsen wake TI model, from IEC-64100 (2019):
 
     Source: http://orbit.dtu.dk/files/3750291/2009_31.pdf
 
-
-    Parameters
-    ----------
-    superpositions : dict
-        The superpositions. Key: variable name str,
-        value: The wake superposition model name,
-        will be looked up in model book
-    opening_angle : float
-        The wake opening angle. The wake growth parameter k is calculated
-        based on the wake opening angle.
-    ct_max : float
-        The maximal value for ct, values beyond will be limited
-        to this number
-    k_var : str
-        The variable name for k
-
     Attributes
     ----------
-    opening_angle : float
+    opening_angle: float
         The wake opening angle. The wake growth parameter k is calculated
         based on the wake opening angle.
-    k_var : str
+    k_var: str
         The variable name for k
 
+    :group: models.wake_models.ti
+
     """
 
     def __init__(
         self,
         superposition,
         opening_angle=21.6,
         ct_max=0.9999,
         iec_type="2019",
         k_var=FV.K
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        superpositions: dict
+            The superpositions. Key: variable name str,
+            value: The wake superposition model name,
+            will be looked up in model book
+        opening_angle: float
+            The wake opening angle. The wake growth parameter k is calculated
+            based on the wake opening angle.
+        ct_max: float
+            The maximal value for ct, values beyond will be limited
+            to this number
+        k_var: str
+            The variable name for k
+
+        """
         super().__init__(superpositions={FV.TI: superposition}, ct_max=ct_max)
 
         k = float(np.tan(np.deg2rad(opening_angle / 2.0)))
 
         self.iec_type = iec_type
         self.k_var = k_var
         setattr(self, k_var, k)
@@ -69,23 +74,23 @@
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        n_points : int
+        n_points: int
             The number of wake evaluation points
-        wake_deltas : dict
+        wake_deltas: dict
             The wake deltas storage, add wake deltas
             on the fly. Keys: Variable name str, for which the
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
         n_states = mdata.n_states
@@ -93,35 +98,35 @@
 
     def calc_wake_radius(self, algo, mdata, fdata, states_source_turbine, x, ct):
         """
         Calculate the wake radius, depending on x only (not r).
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
-        r : numpy.ndarray
+        r: numpy.ndarray
             The radial values for each x value, shape:
             (n_states, n_points, n_r_per_x, 2)
-        ct : numpy.ndarray
+        ct: numpy.ndarray
             The ct values of the wake-causing turbines,
             shape: (n_states, n_points)
 
         Returns
         -------
-        wake_r : numpy.ndarray
+        wake_r: numpy.ndarray
             The wake radii, shape: (n_states, n_points)
 
         """
         # prepare:
         n_states = fdata.n_states
         st_sel = (np.arange(n_states), states_source_turbine)
 
@@ -139,37 +144,37 @@
         self, algo, mdata, fdata, states_source_turbine, sp_sel, x, wake_r, ct
     ):
         """
         Calculate centre line results of wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_sp_sel,)
-        wake_r : numpy.ndarray
+        wake_r: numpy.ndarray
             The wake radii, shape: (n_sp_sel,)
-        ct : numpy.ndarray
+        ct: numpy.ndarray
             The ct values of the wake-causing turbines,
             shape: (n_sp_sel,)
 
         Returns
         -------
-        cl_del : dict
+        cl_del: dict
             The centre line wake deltas. Key: variable name str,
             varlue: numpy.ndarray, shape: (n_sp_sel,)
 
         """
         # prepare:
         n_states = fdata.n_states
         n_points = sp_sel.shape[1]
```

### Comparing `foxes-0.3.5/foxes/models/wake_models/top_hat.py` & `foxes-0.4.0/foxes/models/wake_models/top_hat.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,129 +5,135 @@
 import foxes.variables as FV
 import foxes.constants as FC
 
 
 class TopHatWakeModel(AxisymmetricWakeModel):
     """
     Abstract base class for top-hat wake models.
-
-    Parameters
-    ----------
-    superpositions : dict
-        The superpositions. Key: variable name str,
-        value: The wake superposition model name,
-        will be looked up in model book
-    ct_max : float
-        The maximal value for ct, values beyond will be limited
-        to this number
+    
+    :group: models.wake_models
 
     """
 
     def __init__(self, superpositions, ct_max=0.9999):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        superpositions: dict
+            The superpositions. Key: variable name str,
+            value: The wake superposition model name,
+            will be looked up in model book
+        ct_max: float
+            The maximal value for ct, values beyond will be limited
+            to this number
+
+        """
         super().__init__(superpositions)
         self.ct_max = ct_max
 
     @abstractmethod
     def calc_wake_radius(self, algo, mdata, fdata, states_source_turbine, x, ct):
         """
         Calculate the wake radius, depending on x only (not r).
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
-        r : numpy.ndarray
+        r: numpy.ndarray
             The radial values for each x value, shape:
             (n_states, n_points, n_r_per_x, 2)
-        ct : numpy.ndarray
+        ct: numpy.ndarray
             The ct values of the wake-causing turbines,
             shape: (n_states, n_points)
 
         Returns
         -------
-        wake_r : numpy.ndarray
+        wake_r: numpy.ndarray
             The wake radii, shape: (n_states, n_points)
 
         """
         pass
 
     @abstractmethod
     def calc_centreline_wake_deltas(
         self, algo, mdata, fdata, states_source_turbine, sp_sel, x, wake_r, ct
     ):
         """
         Calculate centre line results of wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_sp_sel,)
-        wake_r : numpy.ndarray
+        wake_r: numpy.ndarray
             The wake radii, shape: (n_sp_sel,)
-        ct : numpy.ndarray
+        ct: numpy.ndarray
             The ct values of the wake-causing turbines,
             shape: (n_sp_sel,)
 
         Returns
         -------
-        cl_del : dict
+        cl_del: dict
             The centre line wake deltas. Key: variable name str,
             varlue: numpy.ndarray, shape: (n_sp_sel,)
 
         """
         pass
 
     def calc_wakes_spsel_x_r(self, algo, mdata, fdata, states_source_turbine, x, r):
         """
         Calculate wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
-        r : numpy.ndarray
+        r: numpy.ndarray
             The radial values for each x value, shape:
             (n_states, n_points, n_r_per_x, 2)
 
         Returns
         -------
-        wdeltas : dict
+        wdeltas: dict
             The wake deltas. Key: variable name str,
             value: numpy.ndarray, shape: (n_sp_sel, n_r_per_x)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
         n_states = mdata.n_states
         n_points = x.shape[1]
         st_sel = (np.arange(n_states), states_source_turbine)
```

### Comparing `foxes-0.3.5/foxes/models/wake_models/wind/bastankhah.py` & `foxes-0.4.0/foxes/models/wake_models/wind/bastankhah.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,47 +10,53 @@
     The Bastankhah wake model
 
     (https://doi.org/10.1016/j.renene.2014.01.002)
     Modifications: In the calculation of the initial wake radius
     a constant of 0.25 instead of 0.2 is used as it fits better
     to the validation data
 
-    Parameters
-    ----------
-    superpositions : dict
-        The superpositions. Key: variable name str,
-        value: The wake superposition model name,
-        will be looked up in model book
-    k : float, optional
-        The wake growth parameter k. If not given here
-        it will be searched in the farm data.
-    sbeta_factor : float
-        Factor multiplying sbeta
-    ct_max : float
-        The maximal value for ct, values beyond will be limited
-        to this number
-    k_var : str
-        The variable name for k
-
     Attributes
     ----------
-    k : float, optional
+    k: float, optional
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
-    sbeta_factor : float
+    sbeta_factor: float
         Factor multiplying sbeta
-    ct_max : float
+    ct_max: float
         The maximal value for ct, values beyond will be limited
         to this number
-    k_var : str
+    k_var: str
         The variable name for k
 
+    :group: models.wake_models.wind
+
     """
 
     def __init__(self, superposition, k=None, sbeta_factor=0.25, ct_max=0.9999, k_var=FV.K):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        superpositions: dict
+            The superpositions. Key: variable name str,
+            value: The wake superposition model name,
+            will be looked up in model book
+        k: float, optional
+            The wake growth parameter k. If not given here
+            it will be searched in the farm data.
+        sbeta_factor: float
+            Factor multiplying sbeta
+        ct_max: float
+            The maximal value for ct, values beyond will be limited
+            to this number
+        k_var: str
+            The variable name for k
+
+        """
         super().__init__(superpositions={FV.WS: superposition})
 
         self.ct_max = ct_max
         self.sbeta_factor = sbeta_factor
         self.k_var = k_var
 
         setattr(self, k_var, k)
@@ -65,23 +71,23 @@
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        n_points : int
+        n_points: int
             The number of wake evaluation points
-        wake_deltas : dict
+        wake_deltas: dict
             The wake deltas storage, add wake deltas
             on the fly. Keys: Variable name str, for which the
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
         n_states = mdata.n_states
@@ -90,32 +96,32 @@
     def calc_amplitude_sigma_spsel(self, algo, mdata, fdata, states_source_turbine, x):
         """
         Calculate the amplitude and the sigma,
         both depend only on x (not on r).
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
 
         Returns
         -------
-        amsi : tuple
+        amsi: tuple
             The amplitude and sigma, both numpy.ndarray
             with shape (n_sp_sel,)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
         # prepare:
         n_states = mdata.n_states
         n_points = x.shape[1]
```

### Comparing `foxes-0.3.5/foxes/models/wake_models/wind/jensen.py` & `foxes-0.4.0/foxes/models/wake_models/wind/jensen.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,40 +5,46 @@
 import foxes.constants as FC
 
 
 class JensenWake(TopHatWakeModel):
     """
     The Jensen wake model.
 
-    Parameters
-    ----------
-    superpositions : dict
-        The superpositions. Key: variable name str,
-        value: The wake superposition model name,
-        will be looked up in model book
-    k : float, optional
-        The wake growth parameter k. If not given here
-        it will be searched in the farm data.
-    ct_max : float
-        The maximal value for ct, values beyond will be limited
-        to this number
-    k_var : str
-        The variable name for k
-
     Attributes
     ----------
-    k : float, optional
+    k: float, optional
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
-    k_var : str
+    k_var: str
         The variable name for k
 
+    :group: models.wake_models.wind
+
     """
 
     def __init__(self, superposition, k=None, ct_max=0.9999, k_var=FV.K):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        superpositions: dict
+            The superpositions. Key: variable name str,
+            value: The wake superposition model name,
+            will be looked up in model book
+        k: float, optional
+            The wake growth parameter k. If not given here
+            it will be searched in the farm data.
+        ct_max: float
+            The maximal value for ct, values beyond will be limited
+            to this number
+        k_var: str
+            The variable name for k
+
+        """
         super().__init__(superpositions={FV.WS: superposition}, ct_max=ct_max)
 
         self.k_var = k_var
         setattr(self, k_var, k)
 
     def __repr__(self):
         k = getattr(self, self.k_var)
@@ -50,23 +56,23 @@
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        n_points : int
+        n_points: int
             The number of wake evaluation points
-        wake_deltas : dict
+        wake_deltas: dict
             The wake deltas storage, add wake deltas
             on the fly. Keys: Variable name str, for which the
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
         n_states = mdata.n_states
@@ -74,35 +80,35 @@
 
     def calc_wake_radius(self, algo, mdata, fdata, states_source_turbine, x, ct):
         """
         Calculate the wake radius, depending on x only (not r).
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
-        r : numpy.ndarray
+        r: numpy.ndarray
             The radial values for each x value, shape:
             (n_states, n_points, n_r_per_x, 2)
-        ct : numpy.ndarray
+        ct: numpy.ndarray
             The ct values of the wake-causing turbines,
             shape: (n_states, n_points)
 
         Returns
         -------
-        wake_r : numpy.ndarray
+        wake_r: numpy.ndarray
             The wake radii, shape: (n_states, n_points)
 
         """
         n_states = mdata.n_states
         st_sel = (np.arange(n_states), states_source_turbine)
 
         R = fdata[FV.D][st_sel][:, None] / 2
@@ -117,37 +123,37 @@
         self, algo, mdata, fdata, states_source_turbine, sp_sel, x, wake_r, ct
     ):
         """
         Calculate centre line results of wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_sp_sel,)
-        wake_r : numpy.ndarray
+        wake_r: numpy.ndarray
             The wake radii, shape: (n_sp_sel,)
-        ct : numpy.ndarray
+        ct: numpy.ndarray
             The ct values of the wake-causing turbines,
             shape: (n_sp_sel,)
 
         Returns
         -------
-        cl_del : dict
+        cl_del: dict
             The centre line wake deltas. Key: variable name str,
             varlue: numpy.ndarray, shape: (n_sp_sel,)
 
         """
         n_states = mdata.n_states
         n_points = sp_sel.shape[1]
         st_sel = (np.arange(n_states), states_source_turbine)
```

### Comparing `foxes-0.3.5/foxes/models/wake_models/wind/porte_agel.py` & `foxes-0.4.0/foxes/models/wake_models/wind/porte_agel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 import numpy as np
 
 from foxes.models.wake_models.dist_sliced import DistSlicedWakeModel
+from foxes.core.model import Model
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class PorteAgelModel:
+class PorteAgelModel(Model):
     """
     Common calculations for the wake model and the wake
     frame, such that code repetitions can be avoided.
 
-    Based on Bastankhah & Porte-Agel, 2016, https://doi.org/10.1017/jfm.2016.595
-
-    Parameters
-    ----------
-    ct_max : float
-        The maximal value for ct, values beyond will be limited
-        to this number, by default 0.9999
-    alpha : float
-        model parameter used to determine onset of far wake region
-    beta : float
-        model parameter used to determine onset of far wake region
+    Based on Bastankhah & Porte-Agel, 2016, 
+    https://doi.org/10.1017/jfm.2016.595
 
     Attributes
     ----------
-    ct_max : float
+    ct_max: float
         The maximal value for ct, values beyond will be limited
         to this number, by default 0.9999
-    alpha : float
+    alpha: float
         model parameter used to determine onset of far wake region
-    beta : float
+    beta: float
         model parameter used to determine onset of far wake region
+    
+    :group: models.wake_models.wind
 
     """
 
     MDATA_KEY = "PorteAgelModel"
     PARS = "pars"
     CHECK = "check"
     SP_SEL = "sp_sel"
@@ -48,30 +42,47 @@
 
     AMPL_FAR = "ampl_far"
     SIGMA_Y_FAR = "sigma_y_far"
     SIGMA_Z_FAR = "sigma_z_far"
     DELTA_FAR = "delta_far"
 
     def __init__(self, ct_max=0.9999, alpha=0.58, beta=0.07):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        ct_max: float
+            The maximal value for ct, values beyond will be limited
+            to this number, by default 0.9999
+        alpha: float
+            model parameter used to determine onset of far wake region
+        beta: float
+            model parameter used to determine onset of far wake region
+
+        """
+        super().__init__()
         self.ct_max = ct_max
-        self.alpha = alpha
-        self.beta = beta
+        setattr(self, FV.PA_ALPHA, alpha)
+        setattr(self, FV.PA_BETA, beta)
 
     @property
     def pars(self):
         """
         Dictionary of the model parameters
 
         Returns
         -------
         dict :
             Dictionary of the model parameters
 
         """
-        return dict(alpha=self.alpha, beta=self.beta, ct_max=self.ct_max)
+        alpha = getattr(self, FV.PA_ALPHA)
+        beta = getattr(self, FV.PA_BETA)
+        return dict(alpha=alpha, beta=beta, ct_max=self.ct_max)
 
     def calc_data(
         self,
         mdata,
         fdata,
         states_source_turbine,
         x,
@@ -79,34 +90,35 @@
         k,
     ):
         """
         Calculate common model data, store it in mdata.
 
         Parameters
         ----------
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
-        gamma : numpy.ndarray
+        gamma: numpy.ndarray
             The YAWM angles in radiants, shape: (n_states, n_points)
-        k : numpy.ndarray
+        k: numpy.ndarray
             The k parameter values, shape: (n_states, n_points)
 
         """
         # prepare:
         n_states = mdata.n_states
         n_points = x.shape[1]
         st_sel = (np.arange(n_states), states_source_turbine)
 
+
         # store parameters:
         out = {self.PARS: self.pars}
         out[self.CHECK] = (
             mdata[FC.STATE][0],
             states_source_turbine[0],
             x.shape,
         )
@@ -127,30 +139,38 @@
             ws = np.zeros((n_states, n_points), dtype=FC.DTYPE)
             ws[:] = fdata[FV.REWS][st_sel][:, None]
 
             # get TI:
             ti = np.zeros((n_states, n_points), dtype=FC.DTYPE)
             ti[:] = fdata[FV.TI][st_sel][:, None]
 
+            # get alpha:
+            alpha = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+            alpha[:] = Model.get_data(self, FV.PA_ALPHA, fdata, data_prio=True, upcast="farm")[st_sel][:, None]
+
+            # get beta:
+            beta = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+            beta[:] = Model.get_data(self, FV.PA_BETA, fdata, data_prio=True, upcast="farm")[st_sel][:, None]
+
             # apply filter:
             x = x[sp_sel]
             D = D[sp_sel]
             ct = ct[sp_sel]
             ws = ws[sp_sel]
             ti = ti[sp_sel]
             k = k[sp_sel]
             gamma = gamma[sp_sel]
-
+            alpha = alpha[sp_sel]
+            beta = beta[sp_sel]
+        
             # calc theta_c0, Eq. (6.12):
             cosg = np.cos(gamma)
             theta = 0.3 * gamma / cosg * (1 - np.sqrt(1 - ct * cosg))
 
             # calculate x0, Eq. (7.3):
-            alpha = self.alpha
-            beta = self.beta
             sqomct = np.sqrt(1 - ct)
             x0 = (
                 D
                 * (cosg * (1 + sqomct))
                 / (np.sqrt(2) * (4 * alpha * ti + 2 * beta * (1 - sqomct)))
             )
             out[self.X0] = x0
@@ -235,25 +255,25 @@
 
     def has_data(self, mdata, states_source_turbine, x):
         """
         Check if data exists
 
         Parameters
         ----------
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
 
         Returns
         -------
-        check : bool
+        check: bool
             True if data exists
 
         """
         check = (
             mdata[FC.STATE][0],
             states_source_turbine[0],
             x.shape,
@@ -262,22 +282,22 @@
 
     def get_data(self, key, mdata):
         """
         Return data entry
 
         Parameters
         ----------
-        key : str
+        key: str
             The data key
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
 
         Returns
         -------
-        data : numpy.ndarray
+        data: numpy.ndarray
             The data
 
         """
         return mdata[self.MDATA_KEY][key]
 
     def clean(self, mdata):
         """
@@ -286,52 +306,66 @@
         del mdata[self.MDATA_KEY]
 
 
 class PorteAgelWake(DistSlicedWakeModel):
     """
     The Bastankhah PorteAgel wake model
 
-    Based on Bastankhah & Porte-Agel, 2016, https://doi.org/10.1017/jfm.2016.595
-
-
-    Parameters
-    ----------
-    superposition : dict
-        The superpositions. Key: variable name str,
-        value: The wake superposition model name,
-        will be looked up in model book
-    k : float
-        The wake growth parameter k. If not given here
-        it will be searched in the farm data, by default None
-    ct_max : float
-        The maximal value for ct, values beyond will be limited
-        to this number, by default 0.9999
-    alpha : float
-        model parameter used to determine onset of far wake region
-    beta : float
-        model parameter used to determine onset of far wake region
-    k_var : str
-        The variable name for k
+    Based on Bastankhah & Porte-Agel, 2016, 
+    https://doi.org/10.1017/jfm.2016.595
 
     Attributes
     ----------
-    model : PorteAgelModel
+    model: PorteAgelModel
         The model for computing common data
-    K : float
+    K: float
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
-    YAWM : float
+    YAWM: float
         The yaw misalignment YAWM. If not given here
         it will be searched in the farm data.
-    k_var : str
+    k_var: str
         The variable name for k
 
+    :group: models.wake_models.wind
+
     """
 
-    def __init__(self, superposition, k=None, ct_max=0.9999, alpha=0.58, beta=0.07, k_var=FV.K):
+    def __init__(
+            self, 
+            superposition, 
+            k=None, 
+            ct_max=0.9999, 
+            alpha=0.58, 
+            beta=0.07, 
+            k_var=FV.K,
+        ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        superposition: dict
+            The superpositions. Key: variable name str,
+            value: The wake superposition model name,
+            will be looked up in model book
+        k: float
+            The wake growth parameter k. If not given here
+            it will be searched in the farm data, by default None
+        ct_max: float
+            The maximal value for ct, values beyond will be limited
+            to this number, by default 0.9999
+        alpha: float
+            model parameter used to determine onset of far wake region
+        beta: float
+            model parameter used to determine onset of far wake region
+        k_var: str
+            The variable name for k
+
+        """
         super().__init__(superpositions={FV.WS: superposition})
 
         self.model = PorteAgelModel(ct_max, alpha, beta)
         self.k_var = k_var
 
         setattr(self, k_var, k)
         setattr(self, FV.YAWM, 0.0)
@@ -346,23 +380,23 @@
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        n_points : int
+        n_points: int
             The number of wake evaluation points
-        wake_deltas : dict
+        wake_deltas: dict
             The wake deltas storage, add wake deltas
             on the fly. Keys: Variable name str, for which the
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
         n_states = mdata.n_states
@@ -370,35 +404,35 @@
 
     def calc_wakes_spsel_x_yz(self, algo, mdata, fdata, states_source_turbine, x, yz):
         """
         Calculate wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
-        yz : numpy.ndarray
+        yz: numpy.ndarray
             The yz values for each x value, shape:
             (n_states, n_points, n_yz_per_x, 2)
 
         Returns
         -------
-        wdeltas : dict
+        wdeltas: dict
             The wake deltas. Key: variable name str,
             value: numpy.ndarray, shape: (n_sp_sel, n_yz_per_x)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
         # prepare:
         n_states = mdata.n_states
         n_points = x.shape[1]
```

### Comparing `foxes-0.3.5/foxes/models/wake_models/wind/turbopark.py` & `foxes-0.4.0/foxes/models/wake_models/wind/turbopark.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,51 +7,57 @@
 
 class TurbOParkWake(GaussianWakeModel):
     """
     The TurbOPark wake model
 
     https://iopscience.iop.org/article/10.1088/1742-6596/2265/2/022063/pdf
 
-    Parameters
-    ----------
-    superpositions : dict
-        The superpositions. Key: variable name str,
-        value: The wake superposition model name,
-        will be looked up in model book
-    A : float
-        The wake growth parameter A.
-    sbeta_factor : float
-        Factor multiplying sbeta
-    ct_max : float
-        The maximal value for ct, values beyond will be limited
-        to this number
-    c1 : float
-        Factor from Frandsen turbulence model
-    c2 : float
-        Factor from Frandsen turbulence model
-
     Attributes
     ----------
-    A : float
+    A: float
         The wake growth parameter A.
-    sbeta_factor : float
+    sbeta_factor: float
         Factor multiplying sbeta
-    ct_max : float
+    ct_max: float
         The maximal value for ct, values beyond will be limited
         to this number
-    c1 : float
+    c1: float
         Factor from Frandsen turbulence model
-    c2 : float
+    c2: float
         Factor from Frandsen turbulence model
 
+    :group: models.wake_models.wind
+
     """
 
     def __init__(
         self, superposition, A, sbeta_factor=0.25, ct_max=0.9999, c1=1.5, c2=0.8
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        superpositions: dict
+            The superpositions. Key: variable name str,
+            value: The wake superposition model name,
+            will be looked up in model book
+        A: float
+            The wake growth parameter A.
+        sbeta_factor: float
+            Factor multiplying sbeta
+        ct_max: float
+            The maximal value for ct, values beyond will be limited
+            to this number
+        c1: float
+            Factor from Frandsen turbulence model
+        c2: float
+            Factor from Frandsen turbulence model
+
+        """
         super().__init__(superpositions={FV.WS: superposition})
 
         self.A = A
         self.ct_max = ct_max
         self.sbeta_factor = sbeta_factor
         self.c1 = c1
         self.c2 = c2
@@ -65,23 +71,23 @@
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        n_points : int
+        n_points: int
             The number of wake evaluation points
-        wake_deltas : dict
+        wake_deltas: dict
             The wake deltas storage, add wake deltas
             on the fly. Keys: Variable name str, for which the
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
         n_states = mdata.n_states
@@ -90,32 +96,32 @@
     def calc_amplitude_sigma_spsel(self, algo, mdata, fdata, states_source_turbine, x):
         """
         Calculate the amplitude and the sigma,
         both depend only on x (not on r).
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
 
         Returns
         -------
-        amsi : tuple
+        amsi: tuple
             The amplitude and sigma, both numpy.ndarray
             with shape (n_sp_sel,)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
         # prepare:
         n_states = mdata.n_states
         n_points = x.shape[1]
@@ -199,63 +205,68 @@
 
 class TurbOParkWakeIX(GaussianWakeModel):
     """
     The generalized TurbOPark wake model, integrating TI over the streamline.
 
     https://iopscience.iop.org/article/10.1088/1742-6596/2265/2/022063/pdf
 
-    Parameters
-    ----------
-    superpositions : dict
-        The superpositions. Key: variable name str,
-        value: The wake superposition model name,
-        will be looked up in model book
-    dx : float
-        The step size of the integral
-    A : float, optional
-        The wake growth parameter A.
-    sbeta_factor : float
-        Factor multiplying sbeta
-    ct_max : float
-        The maximal value for ct, values beyond will be limited
-        to this number
-    ti_var :  str
-        The TI variable
-    ipars : dict, optional
-        Additional parameters for centreline integration
-
-
     Attributes
     ----------
-    dx : float
+    dx: float
         The step size of the integral
-    A : float
+    A: float
         The wake growth parameter A.
-    sbeta_factor : float
+    sbeta_factor: float
         Factor multiplying sbeta
-    ct_max : float
+    ct_max: float
         The maximal value for ct, values beyond will be limited
         to this number
-    ti_var :  str
+    ti_var:  str
         The TI variable
-    ipars : dict
+    ipars: dict
         Additional parameters for centreline integration
 
+    :group: models.wake_models.wind
+
     """
 
     def __init__(
         self,
         superposition,
         dx,
         A,
         sbeta_factor=0.25,
         ct_max=0.9999,
         ti_var=FV.TI,
         **ipars,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        superpositions: dict
+            The superpositions. Key: variable name str,
+            value: The wake superposition model name,
+            will be looked up in model book
+        dx: float
+            The step size of the integral
+        A: float, optional
+            The wake growth parameter A.
+        sbeta_factor: float
+            Factor multiplying sbeta
+        ct_max: float
+            The maximal value for ct, values beyond will be limited
+            to this number
+        ti_var:  str
+            The TI variable
+        ipars: dict, optional
+            Additional parameters for centreline integration
+
+        """
         super().__init__(superpositions={FV.WS: superposition})
 
         self.dx = dx
         self.A = A
         self.ct_max = ct_max
         self.sbeta_factor = sbeta_factor
         self.ti_var = ti_var
@@ -270,23 +281,23 @@
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        n_points : int
+        n_points: int
             The number of wake evaluation points
-        wake_deltas : dict
+        wake_deltas: dict
             The wake deltas storage, add wake deltas
             on the fly. Keys: Variable name str, for which the
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
         n_states = mdata.n_states
@@ -295,32 +306,32 @@
     def calc_amplitude_sigma_spsel(self, algo, mdata, fdata, states_source_turbine, x):
         """
         Calculate the amplitude and the sigma,
         both depend only on x (not on r).
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x : numpy.ndarray
+        x: numpy.ndarray
             The x values, shape: (n_states, n_points)
 
         Returns
         -------
-        amsi : tuple
+        amsi: tuple
             The amplitude and sigma, both numpy.ndarray
             with shape (n_sp_sel,)
-        sp_sel : numpy.ndarray of bool
+        sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
         # prepare:
         n_states = mdata.n_states
         n_points = x.shape[1]
```

### Comparing `foxes-0.3.5/foxes/models/wake_superpositions/linear.py` & `foxes-0.4.0/foxes/models/wake_superpositions/linear.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,43 +7,49 @@
 
 
 class LinearSuperposition(WakeSuperposition):
     """
     Linear supersposition of wake model results,
     optionally rescaled.
 
-    Parameters
-    ----------
-    scalings : dict or number or str
-        Scaling rules. If `dict`, key: variable name str,
-        value: number or str. If `str`:
-        - `source_turbine`: Scale by source turbine value of variable
-        - `source_turbine_amb`: Scale by source turbine ambient value of variable
-        - `source_turbine_<var>`: Scale by source turbine value of variable <var>
-    lim_low : dict, optional
-        Lower limits of the final wake deltas. Key: variable str,
-        value: float
-    lim_high : dict, optional
-        Higher limits of the final wake deltas. Key: variable str,
-        value: float
-
     Attributes
     ----------
-    scalings : dict or number or str
+    scalings: dict or number or str
         The scaling rules
-    lim_low : dict
+    lim_low: dict
         Lower limits of the final wake deltas. Key: variable str,
         value: float
-    lim_high : dict
+    lim_high: dict
         Higher limits of the final wake deltas. Key: variable str,
         value: float
 
+    :group: models.wake_superpositions
+
     """
 
     def __init__(self, scalings, lim_low=None, lim_high=None):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        scalings: dict or number or str
+            Scaling rules. If `dict`, key: variable name str,
+            value: number or str. If `str`:
+            - `source_turbine`: Scale by source turbine value of variable
+            - `source_turbine_amb`: Scale by source turbine ambient value of variable
+            - `source_turbine_<var>`: Scale by source turbine value of variable <var>
+        lim_low: dict, optional
+            Lower limits of the final wake deltas. Key: variable str,
+            value: float
+        lim_high: dict, optional
+            Higher limits of the final wake deltas. Key: variable str,
+            value: float
+
+        """
         super().__init__()
 
         self.scalings = scalings
         self.lim_low = lim_low
         self.lim_high = lim_high
 
     def calc_wakes_plus_wake(
@@ -58,36 +64,36 @@
         wake_model_result,
     ):
         """
         Add a wake delta to previous wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        sel_sp : numpy.ndarray of bool
+        sel_sp: numpy.ndarray of bool
             The selection of points, shape: (n_states, n_points)
-        variable : str
+        variable: str
             The variable name for which the wake deltas applies
-        wake_delta : numpy.ndarray
+        wake_delta: numpy.ndarray
             The original wake deltas, shape: (n_states, n_points)
-        wake_model_result : numpy.ndarray
+        wake_model_result: numpy.ndarray
             The new wake deltas of the selected points,
             shape: (n_sel_sp,)
 
         Returns
         -------
-        wdelta : numpy.ndarray
+        wdelta: numpy.ndarray
             The updated wake deltas, shape: (n_states, n_points)
 
         """
         if isinstance(self.scalings, dict):
             try:
                 scaling = self.scalings[variable]
             except KeyError:
@@ -150,30 +156,30 @@
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        variable : str
+        variable: str
             The variable name for which the wake deltas applies
-        amb_results : numpy.ndarray
+        amb_results: numpy.ndarray
             The ambient results, shape: (n_states, n_points)
-        wake_delta : numpy.ndarray
+        wake_delta: numpy.ndarray
             The wake deltas, shape: (n_states, n_points)
 
         Returns
         -------
-        final_wake_delta : numpy.ndarray
+        final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
             results by simple plus operation. Shape: (n_states, n_points)
 
         """
         w = wake_delta
         if self.lim_low is not None and variable in self.lim_low:
             w = np.maximum(w, self.lim_low[variable] - amb_results)
```

### Comparing `foxes-0.3.5/foxes/models/wake_superpositions/max.py` & `foxes-0.4.0/foxes/models/wake_superpositions/quadratic.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,36 +2,42 @@
 import numbers
 
 from foxes.core import WakeSuperposition
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class MaxSuperposition(WakeSuperposition):
+class QuadraticSuperposition(WakeSuperposition):
     """
-    Maximum supersposition of wake model results,
+    Quadratic supersposition of wake model results,
     optionally rescaled.
 
-    Parameters
-    ----------
-    scalings : dict or number or str
-        Scaling rules. If `dict`, key: variable name str,
-        value: number or str. If `str`:
-        - `source_turbine`: Scale by source turbine value of variable
-        - `source_turbine_amb`: Scale by source turbine ambient value of variable
-        - `source_turbine_<var>`: Scale by source turbine value of variable <var>
-
     Attributes
     ----------
-    scalings : dict or number or str
+    scalings: dict or number or str
         The scaling rules
 
+    :group: models.wake_superpositions
+
     """
 
     def __init__(self, scalings):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        scalings: dict or number or str
+            Scaling rules. If `dict`, key: variable name str,
+            value: number or str. If `str`:
+            - `source_turbine`: Scale by source turbine value of variable
+            - `source_turbine_amb`: Scale by source turbine ambient value of variable
+            - `source_turbine_<var>`: Scale by source turbine value of variable <var>
+
+        """
         super().__init__()
         self.scalings = scalings
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
@@ -39,22 +45,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.SIGNS = self.var("SIGNS")
         return super().initialize(algo, verbosity)
@@ -71,43 +77,40 @@
         wake_model_result,
     ):
         """
         Add a wake delta to previous wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        sel_sp : numpy.ndarray of bool
+        sel_sp: numpy.ndarray of bool
             The selection of points, shape: (n_states, n_points)
-        variable : str
+        variable: str
             The variable name for which the wake deltas applies
-        wake_delta : numpy.ndarray
+        wake_delta: numpy.ndarray
             The original wake deltas, shape: (n_states, n_points)
-        wake_model_result : numpy.ndarray
+        wake_model_result: numpy.ndarray
             The new wake deltas of the selected points,
             shape: (n_sel_sp,)
 
         Returns
         -------
-        wdelta : numpy.ndarray
+        wdelta: numpy.ndarray
             The updated wake deltas, shape: (n_states, n_points)
 
         """
 
-        if np.all(np.max(np.abs(wake_model_result)) < 1e-10):
-            return wake_delta
-
         if self.SIGNS not in mdata:
             mdata[self.SIGNS] = {}
         if variable not in mdata[self.SIGNS]:
             mdata[self.SIGNS][variable] = (
                 -1 if np.all(wake_model_result <= 0.0) else 1.0
             )
 
@@ -117,23 +120,20 @@
             except KeyError:
                 raise KeyError(
                     f"Model '{self.name}': No scaling found for wake variable '{variable}'"
                 )
         else:
             scaling = self.scalings
 
-        wake_model_result = np.abs(wake_model_result)
-        odelta = wake_delta[sel_sp]
-
         if scaling is None:
-            wake_delta[sel_sp] = np.maximum(odelta, wake_model_result)
+            wake_delta[sel_sp] += wake_model_result**2
             return wake_delta
 
         elif isinstance(scaling, numbers.Number):
-            wake_delta[sel_sp] = np.maximum(odelta, scaling * wake_model_result)
+            wake_delta[sel_sp] += (scaling * wake_model_result) ** 2
             return wake_delta
 
         elif (
             isinstance(scaling, str)
             and len(scaling) >= 14
             and (
                 scaling == f"source_turbine"
@@ -159,15 +159,15 @@
             n_states = mdata.n_states
             n_points = wake_delta.shape[1]
             stsel = (np.arange(n_states), states_source_turbine)
             scale = np.zeros((n_states, n_points), dtype=FC.DTYPE)
             scale[:] = vdata[stsel][:, None]
             scale = scale[sel_sp]
 
-            wake_delta[sel_sp] = np.maximum(odelta, scale * wake_model_result)
+            wake_delta[sel_sp] += (scale * wake_model_result) ** 2
 
             return wake_delta
 
         else:
             raise ValueError(
                 f"Model '{self.name}': Invalid scaling choice '{scaling}' for wake variable '{variable}', valid choices: None, <scalar>, 'source_turbine', 'source_turbine_amb', 'source_turbine_<var>'"
             )
@@ -177,33 +177,33 @@
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        variable : str
+        variable: str
             The variable name for which the wake deltas applies
-        amb_results : numpy.ndarray
+        amb_results: numpy.ndarray
             The ambient results, shape: (n_states, n_points)
-        wake_delta : numpy.ndarray
+        wake_delta: numpy.ndarray
             The wake deltas, shape: (n_states, n_points)
 
         Returns
         -------
-        final_wake_delta : numpy.ndarray
+        final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
             results by simple plus operation. Shape: (n_states, n_points)
 
         """
         try:
-            return mdata[self.SIGNS][variable] * wake_delta
+            return mdata[self.SIGNS][variable] * np.sqrt(wake_delta)
         except KeyError as e:
             if np.max(np.abs(wake_delta)) < 1e-10:
                 return wake_delta
             raise e
```

### Comparing `foxes-0.3.5/foxes/models/wake_superpositions/product.py` & `foxes-0.4.0/foxes/models/wake_superpositions/product.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,35 +14,41 @@
     wind deficit should be rescaled with the wake
     corrected wind field, rather than the rotor
     equivalent wind speed.
 
     Source: https://arxiv.org/pdf/2010.03873.pdf
             Equation (8)
 
-    Parameters
-    ----------
-    lim_low : dict, optional
-        Lower limits of the final wake deltas. Key: variable str,
-        value: float
-    lim_high : dict, optional
-        Higher limits of the final wake deltas. Key: variable str,
-        value: float
-
     Attributes
     ----------
-    lim_low : dict
+    lim_low: dict
         Lower limits of the final wake deltas. Key: variable str,
         value: float
-    lim_high : dict
+    lim_high: dict
         Higher limits of the final wake deltas. Key: variable str,
         value: float
 
+    :group: models.wake_superpositions
+
     """
 
     def __init__(self, lim_low=None, lim_high=None):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        lim_low: dict, optional
+            Lower limits of the final wake deltas. Key: variable str,
+            value: float
+        lim_high: dict, optional
+            Higher limits of the final wake deltas. Key: variable str,
+            value: float
+
+        """
         super().__init__()
         self.lim_low = lim_low
         self.lim_high = lim_high
 
     def calc_wakes_plus_wake(
         self,
         algo,
@@ -55,36 +61,36 @@
         wake_model_result,
     ):
         """
         Add a wake delta to previous wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        sel_sp : numpy.ndarray of bool
+        sel_sp: numpy.ndarray of bool
             The selection of points, shape: (n_states, n_points)
-        variable : str
+        variable: str
             The variable name for which the wake deltas applies
-        wake_delta : numpy.ndarray
+        wake_delta: numpy.ndarray
             The original wake deltas, shape: (n_states, n_points)
-        wake_model_result : numpy.ndarray
+        wake_model_result: numpy.ndarray
             The new wake deltas of the selected points,
             shape: (n_sel_sp,)
 
         Returns
         -------
-        wdelta : numpy.ndarray
+        wdelta: numpy.ndarray
             The updated wake deltas, shape: (n_states, n_points)
 
         """
 
         if np.max(np.abs(wake_delta)) < 1e-14:
             wake_delta[:] = 1
         wake_delta[sel_sp] *= 1 + wake_model_result
@@ -95,30 +101,30 @@
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        variable : str
+        variable: str
             The variable name for which the wake deltas applies
-        amb_results : numpy.ndarray
+        amb_results: numpy.ndarray
             The ambient results, shape: (n_states, n_points)
-        wake_delta : numpy.ndarray
+        wake_delta: numpy.ndarray
             The wake deltas, shape: (n_states, n_points)
 
         Returns
         -------
-        final_wake_delta : numpy.ndarray
+        final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
             results by simple plus operation. Shape: (n_states, n_points)
 
         """
         w = amb_results * (wake_delta - 1)
         if self.lim_low is not None and variable in self.lim_low:
             w = np.maximum(w, self.lim_low[variable] - amb_results)
```

### Comparing `foxes-0.3.5/foxes/models/wake_superpositions/quadratic.py` & `foxes-0.4.0/foxes/models/wake_superpositions/max.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,36 +2,42 @@
 import numbers
 
 from foxes.core import WakeSuperposition
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class QuadraticSuperposition(WakeSuperposition):
+class MaxSuperposition(WakeSuperposition):
     """
-    Quadratic supersposition of wake model results,
+    Maximum supersposition of wake model results,
     optionally rescaled.
 
-    Parameters
-    ----------
-    scalings : dict or number or str
-        Scaling rules. If `dict`, key: variable name str,
-        value: number or str. If `str`:
-        - `source_turbine`: Scale by source turbine value of variable
-        - `source_turbine_amb`: Scale by source turbine ambient value of variable
-        - `source_turbine_<var>`: Scale by source turbine value of variable <var>
-
     Attributes
     ----------
-    scalings : dict or number or str
+    scalings: dict or number or str
         The scaling rules
 
+    :group: models.wake_superpositions
+
     """
 
     def __init__(self, scalings):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        scalings: dict or number or str
+            Scaling rules. If `dict`, key: variable name str,
+            value: number or str. If `str`:
+            - `source_turbine`: Scale by source turbine value of variable
+            - `source_turbine_amb`: Scale by source turbine ambient value of variable
+            - `source_turbine_<var>`: Scale by source turbine value of variable <var>
+
+        """
         super().__init__()
         self.scalings = scalings
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
@@ -39,22 +45,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.SIGNS = self.var("SIGNS")
         return super().initialize(algo, verbosity)
@@ -71,40 +77,43 @@
         wake_model_result,
     ):
         """
         Add a wake delta to previous wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        sel_sp : numpy.ndarray of bool
+        sel_sp: numpy.ndarray of bool
             The selection of points, shape: (n_states, n_points)
-        variable : str
+        variable: str
             The variable name for which the wake deltas applies
-        wake_delta : numpy.ndarray
+        wake_delta: numpy.ndarray
             The original wake deltas, shape: (n_states, n_points)
-        wake_model_result : numpy.ndarray
+        wake_model_result: numpy.ndarray
             The new wake deltas of the selected points,
             shape: (n_sel_sp,)
 
         Returns
         -------
-        wdelta : numpy.ndarray
+        wdelta: numpy.ndarray
             The updated wake deltas, shape: (n_states, n_points)
 
         """
 
+        if np.all(np.max(np.abs(wake_model_result)) < 1e-10):
+            return wake_delta
+
         if self.SIGNS not in mdata:
             mdata[self.SIGNS] = {}
         if variable not in mdata[self.SIGNS]:
             mdata[self.SIGNS][variable] = (
                 -1 if np.all(wake_model_result <= 0.0) else 1.0
             )
 
@@ -114,20 +123,23 @@
             except KeyError:
                 raise KeyError(
                     f"Model '{self.name}': No scaling found for wake variable '{variable}'"
                 )
         else:
             scaling = self.scalings
 
+        wake_model_result = np.abs(wake_model_result)
+        odelta = wake_delta[sel_sp]
+
         if scaling is None:
-            wake_delta[sel_sp] += wake_model_result**2
+            wake_delta[sel_sp] = np.maximum(odelta, wake_model_result)
             return wake_delta
 
         elif isinstance(scaling, numbers.Number):
-            wake_delta[sel_sp] += (scaling * wake_model_result) ** 2
+            wake_delta[sel_sp] = np.maximum(odelta, scaling * wake_model_result)
             return wake_delta
 
         elif (
             isinstance(scaling, str)
             and len(scaling) >= 14
             and (
                 scaling == f"source_turbine"
@@ -153,15 +165,15 @@
             n_states = mdata.n_states
             n_points = wake_delta.shape[1]
             stsel = (np.arange(n_states), states_source_turbine)
             scale = np.zeros((n_states, n_points), dtype=FC.DTYPE)
             scale[:] = vdata[stsel][:, None]
             scale = scale[sel_sp]
 
-            wake_delta[sel_sp] += (scale * wake_model_result) ** 2
+            wake_delta[sel_sp] = np.maximum(odelta, scale * wake_model_result)
 
             return wake_delta
 
         else:
             raise ValueError(
                 f"Model '{self.name}': Invalid scaling choice '{scaling}' for wake variable '{variable}', valid choices: None, <scalar>, 'source_turbine', 'source_turbine_amb', 'source_turbine_<var>'"
             )
@@ -171,33 +183,33 @@
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        variable : str
+        variable: str
             The variable name for which the wake deltas applies
-        amb_results : numpy.ndarray
+        amb_results: numpy.ndarray
             The ambient results, shape: (n_states, n_points)
-        wake_delta : numpy.ndarray
+        wake_delta: numpy.ndarray
             The wake deltas, shape: (n_states, n_points)
 
         Returns
         -------
-        final_wake_delta : numpy.ndarray
+        final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
             results by simple plus operation. Shape: (n_states, n_points)
 
         """
         try:
-            return mdata[self.SIGNS][variable] * np.sqrt(wake_delta)
+            return mdata[self.SIGNS][variable] * wake_delta
         except KeyError as e:
             if np.max(np.abs(wake_delta)) < 1e-10:
                 return wake_delta
             raise e
```

### Comparing `foxes-0.3.5/foxes/models/wake_superpositions/ti_superp.py` & `foxes-0.4.0/foxes/models/wake_superpositions/ti_superp.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,39 @@
 from foxes.core import WakeSuperposition
 
 
 class TISuperposition(WakeSuperposition):
     """
     A collection of superpositions for TI.
 
-    Parameters
-    ----------
-    ti_superp : str
-        The method choice: linear, quadratic, max
-    superp_to_amb : str
-        The method for combining ambient with wake deltas:
-        linear or quadratic
-
     Attributes
     ----------
-    ti_superp : str
+    ti_superp: str
         The method choice: linear, quadratic, max
-    superp_to_amb : str
+    superp_to_amb: str
         The method for combining ambient with wake deltas:
         linear or quadratic
 
+    :group: models.wake_superpositions
+
     """
 
     def __init__(self, ti_superp, superp_to_amb="quadratic"):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        ti_superp: str
+            The method choice: linear, quadratic, max
+        superp_to_amb: str
+            The method for combining ambient with wake deltas:
+            linear or quadratic
+
+        """
         super().__init__()
 
         self.ti_superp = ti_superp
         self.superp_to_amb = superp_to_amb
 
     def calc_wakes_plus_wake(
         self,
@@ -43,36 +49,36 @@
         wake_model_result,
     ):
         """
         Add a wake delta to previous wake deltas.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        states_source_turbine : numpy.ndarray
+        states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        sel_sp : numpy.ndarray of bool
+        sel_sp: numpy.ndarray of bool
             The selection of points, shape: (n_states, n_points)
-        variable : str
+        variable: str
             The variable name for which the wake deltas applies
-        wake_delta : numpy.ndarray
+        wake_delta: numpy.ndarray
             The original wake deltas, shape: (n_states, n_points)
-        wake_model_result : numpy.ndarray
+        wake_model_result: numpy.ndarray
             The new wake deltas of the selected points,
             shape: (n_sel_sp,)
 
         Returns
         -------
-        wdelta : numpy.ndarray
+        wdelta: numpy.ndarray
             The updated wake deltas, shape: (n_states, n_points)
 
         """
         # superposition of every turbines efect at each target point
         # linear ti delta:
         if self.ti_superp == "linear":
             wake_delta[sel_sp] += wake_model_result
@@ -98,30 +104,30 @@
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        variable : str
+        variable: str
             The variable name for which the wake deltas applies
-        amb_results : numpy.ndarray
+        amb_results: numpy.ndarray
             The ambient results, shape: (n_states, n_points)
-        wake_delta : numpy.ndarray
+        wake_delta: numpy.ndarray
             The wake deltas, shape: (n_states, n_points)
 
         Returns
         -------
-        final_wake_delta : numpy.ndarray
+        final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
             results by simple plus operation. Shape: (n_states, n_points)
 
         """
         # linear superposition to ambient:
         if self.superp_to_amb == "linear":
             if self.ti_superp == "linear" or self.ti_superp == "max":
```

### Comparing `foxes-0.3.5/foxes/opt/constraints/area_geometry.py` & `foxes-0.4.0/foxes/opt/constraints/area_geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,56 +5,62 @@
 
 
 class AreaGeometryConstraint(FarmConstraint):
     """
     Constrains turbine positions to the inside
     of a given area geometry.
 
-    Parameters
-    ----------
-    problem : foxes.opt.FarmOptProblem
-        The underlying optimization problem
-    name : str
-        The name of the constraint
-    geometry : foxes.utils.geom2d.AreaGeometry
-        The area geometry
-    sel_turbines : list of int, optional
-        The selected turbines
-    disc_inside : bool
-        Ensure full rotor disc inside boundary
-    D : float, optional
-        Use this radius for rotor disc inside condition
-    kwargs : dict, optional
-        Additional parameters for `iwopy.Constraint`
-
     Attributes
     ----------
     farm: foxes.WindFarm
         The wind farm
     sel_turbines: list
         The selected turbines
-    geometry : foxes.utils.geom2d.AreaGeometry
+    geometry: foxes.utils.geom2d.AreaGeometry
         The area geometry
-    disc_inside : bool
+    disc_inside: bool
         Ensure full rotor disc inside boundary
-    D : float
+    D: float
         Use this radius for rotor disc inside condition
+    
+    :group: opt.constraints
 
     """
 
     def __init__(
         self,
         problem,
         name,
         geometry,
         sel_turbines=None,
         disc_inside=False,
         D=None,
         **kwargs,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        problem : foxes.opt.FarmOptProblem
+            The underlying optimization problem
+        name : str
+            The name of the constraint
+        geometry : foxes.utils.geom2d.AreaGeometry
+            The area geometry
+        sel_turbines : list of int, optional
+            The selected turbines
+        disc_inside : bool
+            Ensure full rotor disc inside boundary
+        D : float, optional
+            Use this radius for rotor disc inside condition
+        kwargs : dict, optional
+            Additional parameters for `iwopy.Constraint`
+
+        """
         self.geometry = geometry
         self.disc_inside = disc_inside
         self.D = D
 
         selt = problem.sel_turbines if sel_turbines is None else sel_turbines
         vrs = []
         cns = []
@@ -82,15 +88,15 @@
     def vardeps_float(self):
         """
         Gets the dependencies of all components
         on the function float variables
 
         Returns
         -------
-        deps : numpy.ndarray of bool
+        deps: numpy.ndarray of bool
             The dependencies of components on function
             variables, shape: (n_components, n_vars_float)
 
         """
         deps = np.zeros((self.n_components(), self.n_components(), 2), dtype=bool)
         np.fill_diagonal(deps[:, :, 0], True)
         np.fill_diagonal(deps[:, :, 1], True)
@@ -99,27 +105,27 @@
     def calc_individual(self, vars_int, vars_float, problem_results, components=None):
         """
         Calculate values for a single individual of the
         underlying problem.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_vars_float,)
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
-        components : list of int, optional
+        components: list of int, optional
             The selected components or None for all
 
         Returns
         -------
-        values : np.array
+        values: np.array
             The component values, shape: (n_sel_components,)
 
         """
         s = np.s_[:]
         if components is not None and len(components) < self.n_components():
             s = components
         xy = vars_float.reshape(self.n_components(), 2)[s]
@@ -137,27 +143,27 @@
 
     def calc_population(self, vars_int, vars_float, problem_results, components=None):
         """
         Calculate values for all individuals of a population.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_pop, n_vars_int)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_pop, n_vars_float)
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
-        components : list of int, optional
+        components: list of int, optional
             The selected components or None for all
 
         Returns
         -------
-        values : np.array
+        values: np.array
             The component values, shape: (n_pop, n_sel_components)
 
         """
         n_pop = len(vars_float)
         n_cmpnts = self.n_components()
         s = np.s_[:]
         if components is not None and len(components) < self.n_components():
@@ -181,22 +187,28 @@
 
 
 class FarmBoundaryConstraint(AreaGeometryConstraint):
     """
     Constrains turbine positions to the inside of
     the wind farm boundary
 
-    Parameters
-    ----------
-    problem : foxes.opt.FarmOptProblem
-        The underlying optimization problem
-    name : str
-        The name of the constraint
-    kwargs : dict, optional
-        Additional parameters for `AreaGeometryConstraint`
+    :group: opt.constraints
 
     """
 
     def __init__(self, problem, name="boundary", **kwargs):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        problem: foxes.opt.FarmOptProblem
+            The underlying optimization problem
+        name: str
+            The name of the constraint
+        kwargs: dict, optional
+            Additional parameters for `AreaGeometryConstraint`
+
+        """
         b = problem.farm.boundary
         assert b is not None, f"Constraint '{name}': Missing wind farm boundary."
         super().__init__(problem, name, geometry=b, **kwargs)
```

### Comparing `foxes-0.3.5/foxes/opt/constraints/min_dist.py` & `foxes-0.4.0/foxes/opt/constraints/min_dist.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,51 +5,57 @@
 import foxes.constants as FC
 
 class MinDistConstraint(FarmConstraint):
     """
     Turbines must keep at least a minimal
     spatial distance.
 
-    Parameters
-    ----------
-    problem : foxes.opt.FarmOptProblem
-        The underlying optimization problem
-    min_dist : float
-        The minimal distance
-    min_dist_unit : str
-        The minimal distance unit, either m or D
-    name : str
-        The name of the constraint
-    sel_turbines : list of int, optional
-        The selected turbines
-    kwargs : dict, optional
-        Additional parameters for `iwopy.Constraint`
-
     Attributes
     ----------
     farm: foxes.WindFarm
         The wind farm
     sel_turbines: list
         The selected turbines
-    min_dist : float
+    min_dist: float
         The minimal distance
-    min_dist_unit : str
+    min_dist_unit: str
         The minimal distance unit, either m or D
 
+    :group: opt.constraints
+
     """
 
     def __init__(
         self,
         problem,
         min_dist,
         min_dist_unit="m",
         name="dist",
         sel_turbines=None,
         **kwargs,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        problem: foxes.opt.FarmOptProblem
+            The underlying optimization problem
+        min_dist: float
+            The minimal distance
+        min_dist_unit: str
+            The minimal distance unit, either m or D
+        name: str
+            The name of the constraint
+        sel_turbines: list of int, optional
+            The selected turbines
+        kwargs: dict, optional
+            Additional parameters for `iwopy.Constraint`
+
+        """
         self.min_dist = min_dist
         self.min_dist_unit = min_dist_unit
 
         selt = problem.sel_turbines if sel_turbines is None else sel_turbines
         vrs = []
         for ti in selt:
             vrs += [problem.tvar(FV.X, ti), problem.tvar(FV.Y, ti)]
@@ -58,15 +64,15 @@
 
     def initialize(self, verbosity=0):
         """
         Initialize the constaint.
 
         Parameters
         ----------
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         N = self.farm.n_turbines
         self._i2t = []  # i --> (ti, tj)
         self._t2i = np.full([N, N], -1)  # (ti, tj) --> i
         i = 0
@@ -97,15 +103,15 @@
     def vardeps_float(self):
         """
         Gets the dependencies of all components
         on the function float variables
 
         Returns
         -------
-        deps : numpy.ndarray of bool
+        deps: numpy.ndarray of bool
             The dependencies of components on function
             variables, shape: (n_components, n_vars_float)
 
         """
         turbs = list(self.problem.sel_turbines)
         deps = np.zeros((self.n_components(), len(turbs), 2), dtype=bool)
         for i, titj in enumerate(self._i2t):
@@ -118,27 +124,27 @@
     def calc_individual(self, vars_int, vars_float, problem_results, components=None):
         """
         Calculate values for a single individual of the
         underlying problem.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_vars_float,)
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
-        components : list of int, optional
+        components: list of int, optional
             The selected components or None for all
 
         Returns
         -------
-        values : np.array
+        values: np.array
             The component values, shape: (n_sel_components,)
 
         """
         xy = np.stack(
             [problem_results[FV.X].to_numpy(), problem_results[FV.Y].to_numpy()],
             axis=-1,
         )
@@ -173,27 +179,27 @@
 
     def calc_population(self, vars_int, vars_float, problem_results, components=None):
         """
         Calculate values for all individuals of a population.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_pop, n_vars_int)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_pop, n_vars_float)
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
-        components : list of int, optional
+        components: list of int, optional
             The selected components or None for all
 
         Returns
         -------
-        values : np.array
+        values: np.array
             The component values, shape: (n_pop, n_sel_components)
 
         """
         n_pop = problem_results["n_pop"].values
         n_states = problem_results["n_org_states"].values
         n_turbines = problem_results.dims[FC.TURBINE]
```

### Comparing `foxes-0.3.5/foxes/opt/core/farm_constraint.py` & `foxes-0.4.0/foxes/opt/core/farm_constraint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-from abc import abstractmethod
 from iwopy import Constraint
 
 from foxes.utils import all_subclasses
 
 
 class FarmConstraint(Constraint):
     """
     Abstract base class for foxes wind farm
     optimization constraints.
 
-    Parameters
-    ----------
-    problem : foxes.opt.FarmOptProblem
-        The underlying optimization problem
-    name : str
-        The name of the constraint
-    sel_turbines : list of int, optional
-        The selected turbines
-    kwargs : dict, optional
-        Additional parameters for `iwopy.Constraint`
+    :group: opt.core
 
     """
 
     def __init__(self, problem, name, sel_turbines=None, **kwargs):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        problem: foxes.opt.FarmOptProblem
+            The underlying optimization problem
+        name: str
+            The name of the constraint
+        sel_turbines: list of int, optional
+            The selected turbines
+        kwargs: dict, optional
+            Additional parameters for `iwopy.Constraint`
+
+        """
         super().__init__(problem, name, **kwargs)
         self._sel_turbines = sel_turbines
 
     @property
     def farm(self):
         """
         The wind farm
@@ -71,15 +76,15 @@
 
     def add_to_layout_figure(self, ax, **kwargs):
         """
         Add to a layout figure
 
         Parameters
         ----------
-        ax : matplotlib.pyplot.Axis
+        ax: matplotlib.pyplot.Axis
             The figure axis
 
         """
         return ax
 
     @classmethod
     def print_models(cls):
```

### Comparing `foxes-0.3.5/foxes/opt/core/farm_objective.py` & `foxes-0.4.0/foxes/opt/core/farm_objective.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,34 @@
 
 
 class FarmObjective(Objective):
     """
     Abstract base class for foxes wind farm
     objective functions.
 
-    Parameters
-    ----------
-    problem : foxes.opt.FarmOptProblem
-        The underlying optimization problem
-    name : str
-        The name of the objective function
-    sel_turbines : list of int, optional
-        The selected turbines
-    kwargs : dict, optional
-        Additional parameters for `iwopy.Objective`
+    :group: opt.core
 
     """
 
     def __init__(self, problem, name, sel_turbines=None, **kwargs):
+        """
+        Constraints.
+        
+        Parameters
+        ----------
+        problem: foxes.opt.FarmOptProblem
+            The underlying optimization problem
+        name: str
+            The name of the objective function
+        sel_turbines: list of int, optional
+            The selected turbines
+        kwargs: dict, optional
+            Additional parameters for `iwopy.Objective`
+
+        """
         super().__init__(problem, name, **kwargs)
         self._sel_turbines = sel_turbines
 
     @property
     def farm(self):
         """
         The wind farm
@@ -71,15 +77,15 @@
 
     def add_to_layout_figure(self, ax, **kwargs):
         """
         Add to a layout figure
 
         Parameters
         ----------
-        ax : matplotlib.pyplot.Axis
+        ax: matplotlib.pyplot.Axis
             The figure axis
 
         """
         return ax
 
     @classmethod
     def print_models(cls):
```

### Comparing `foxes-0.3.5/foxes/opt/core/farm_opt_problem.py` & `foxes-0.4.0/foxes/opt/core/farm_opt_problem.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,59 +1,72 @@
+import numpy as np
 from iwopy import Problem
 
 from foxes.utils.runners import DefaultRunner
 import foxes.constants as FC
 from .pop_states import PopStates
 
 
 class FarmOptProblem(Problem):
     """
     Abstract base class of wind farm optimization problems.
 
-    Parameters
-    ----------
-    name : str
-        The problem's name
-    algo : foxes.core.Algorithm
-        The algorithm
-    runner : foxes.core.Runner, optional
-        The runner for running the algorithm
-    sel_turbines : list of int, optional
-        The turbines selected for optimization,
-        or None for all
-    calc_farm_args : dict
-        Additional parameters for algo.calc_farm()
-    kwargs : dict, optional
-        Additional parameters for `iwopy.Problem`
-
     Attributes
     ----------
-    algo : foxes.core.Algorithm
+    algo: foxes.core.Algorithm
         The algorithm
-    runner : foxes.core.Runner
+    runner: foxes.core.Runner
         The runner for running the algorithm
-    calc_farm_args : dict
+    calc_farm_args: dict
         Additional parameters for algo.calc_farm()
+    points : numpy.ndarray
+        The probe points, shape: (n_states, n_points, 3)
+
+    :group: opt.core
 
     """
 
     def __init__(
         self,
         name,
         algo,
         runner=None,
         sel_turbines=None,
         calc_farm_args={},
+        points=None,
         **kwargs,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        name: str
+            The problem's name
+        algo: foxes.core.Algorithm
+            The algorithm
+        runner: foxes.core.Runner, optional
+            The runner for running the algorithm
+        sel_turbines: list of int, optional
+            The turbines selected for optimization,
+            or None for all
+        calc_farm_args: dict
+            Additional parameters for algo.calc_farm()
+        points : numpy.ndarray, optional
+            The probe points, shape: (n_states, n_points, 3)
+        kwargs: dict, optional
+            Additional parameters for `iwopy.Problem`
+
+        """
         super().__init__(name, **kwargs)
 
         self.algo = algo
         self.runner = runner
         self.calc_farm_args = calc_farm_args
+        self.points = points
 
         self._sel_turbines = sel_turbines
         self._count = None
 
     @property
     def farm(self):
         """
@@ -126,17 +139,17 @@
     @classmethod
     def tvar(cls, var, turbine_i):
         """
         Gets turbine variable name
 
         Parameters
         ----------
-        var : str
+        var: str
             The variable name
-        turbine_i : int
+        turbine_i: int
             The turbine index
 
         Returns
         -------
         str :
             The turbine variable name
 
@@ -147,41 +160,41 @@
     def parse_tvar(cls, tvr):
         """
         Parse foxes variable name and turbine index
         from turbine variable
 
         Parameters
         ----------
-        tvr : str
+        tvr: str
             The turbine variable name
 
         Returns
         -------
-        var : str
+        var: str
             The foxes variable name
-        turbine_i : int
+        turbine_i: int
             The turbine index
 
         """
         t = tvr.split("_")
         return t[0], int(t[1])
 
     def _update_keep_models(self, drop_vars, exclude=None, verbosity=1):
         """
         Updates algo.keep_models during initialization
 
         Parameters
         ----------
-        drop_vars : list of str
+        drop_vars: list of str
             Variables that decide about dropping model
             from algo.keep_models
-        exclude : list of str, optional
+        exclude: list of str, optional
             The model names to be excluded, default
             is original states and problem model names
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         if exclude is None:
             exclude = [self._org_states_name]
         self.algo.keep_models.append(self._org_states_name)
         for mname, idata in self.algo.idata_mem.items():
@@ -199,21 +212,21 @@
 
     def initialize(self, drop_vars=[FC.STATE], exclude=None, verbosity=1):
         """
         Initialize the object.
 
         Parameters
         ----------
-        drop_vars : list of str
+        drop_vars: list of str
             Variables that decide about dropping model
             from algo.keep_models
-        exclude : list of str, optional
+        exclude: list of str, optional
             The model names to be excluded, default
             is original states and problem model names
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         if self.runner is None:
             self.runner = DefaultRunner()
             self.runner.initialize()
         elif not self.runner.initialized:
@@ -248,17 +261,17 @@
         the latest optimization variables.
 
         This function is called before running the farm
         calculation.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_vars_float,)
 
         """
         # reset states, if needed:
         if isinstance(self.algo.states, PopStates):
             self._reset_states(self.algo.states.states)
             self.algo.n_states = self._org_n_states
@@ -269,17 +282,17 @@
         the latest optimization variables.
 
         This function is called before running the farm
         calculation.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_pop, n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_pop, n_vars_float,)
 
         """
         # set/reset pop states, if needed:
         n_pop = len(vars_float)
         if not isinstance(self.algo.states, PopStates):
             self._reset_states(PopStates(self.algo.states, n_pop))
@@ -289,65 +302,80 @@
 
     def apply_individual(self, vars_int, vars_float):
         """
         Apply new variables to the problem.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_vars_float,)
 
         Returns
         -------
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
 
         """
         self._count += 1
         self.update_problem_individual(vars_int, vars_float)
-        return self.runner.run(self.algo.calc_farm, kwargs=self.calc_farm_args)
+        farm_results = self.runner.run(self.algo.calc_farm, kwargs=self.calc_farm_args)
+
+        if self.points is None:
+            return farm_results
+        else:
+            point_results = self.runner.run(self.algo.calc_points, args=(farm_results, self.points))
+            return farm_results, point_results
 
     def apply_population(self, vars_int, vars_float):
         """
         Apply new variables to the problem,
         for a whole population.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_pop, n_vars_int)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_pop, n_vars_float)
 
         Returns
         -------
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
 
         """
         self._count += 1
 
         self.update_problem_population(vars_int, vars_float)
-        results = self.runner.run(self.algo.calc_farm, kwargs=self.calc_farm_args)
-        results["n_pop"] = len(vars_float)
-        results["n_org_states"] = self._org_n_states
-
-        return results
+        farm_results = self.runner.run(self.algo.calc_farm, kwargs=self.calc_farm_args)
+        farm_results["n_pop"] = len(vars_float)
+        farm_results["n_org_states"] = self._org_n_states
+
+        if self.points is None:
+            return farm_results
+        else:
+            n_pop = farm_results["n_pop"].values
+            n_states, n_points = self.points.shape[:2]
+            pop_points = np.zeros((n_pop, n_states, n_points, 3), dtype=FC.DTYPE)
+            pop_points[:] = self.points[None, :, : , :]
+            pop_points = pop_points.reshape(n_pop*n_states, n_points, 3)
+            point_results = self.runner.run(self.algo.calc_points, args=(farm_results, pop_points))
+            return farm_results, point_results
 
     def add_to_layout_figure(self, ax, **kwargs):
         """
         Add to a layout figure
 
         Parameters
         ----------
-        ax : matplotlib.pyplot.Axis
+        ax: matplotlib.pyplot.Axis
             The figure axis
 
         """
         for c in self.cons.functions:
             ax = c.add_to_layout_figure(ax, **kwargs)
         for f in self.objs.functions:
             ax = f.add_to_layout_figure(ax, **kwargs)
```

### Comparing `foxes-0.3.5/foxes/opt/core/farm_vars_problem.py` & `foxes-0.4.0/foxes/opt/core/farm_vars_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,34 @@
 import foxes.constants as FC
 
 
 class FarmVarsProblem(FarmOptProblem):
     """
     Abstract base class for models that optimize
     farm variables.
+
+    :group: opt.core
+    
     """
 
     def initialize(self, pre_rotor_vars, post_rotor_vars, verbosity=1, **kwargs):
         """
         Initialize the object.
 
         Parameters
         ----------
-        pre_rotor_vars : list of str or dict
+        pre_rotor_vars: list of str or dict
             The pre_rotor farm variables. If dict, then
             key: sub-model str, value: var names as list of str
-        post_rotor_vars : list of str or dict
+        post_rotor_vars: list of str or dict
             The post_rotor farm variables. If dict, then
             key: sub-model str, value: var names as list of str
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
-        kwargs : dict, optional
+        kwargs: dict, optional
             Additional parameters for super class init
 
         """
         self._vars_pre = {}
         self._vars_post = {}
         if isinstance(pre_rotor_vars, dict):
             self._vars_pre = {m: v for m, v in pre_rotor_vars.items() if len(v)}
@@ -77,50 +80,50 @@
     @abstractmethod
     def opt2farm_vars_individual(self, vars_int, vars_float):
         """
         Translates optimization variables to farm variables
 
         Parameters
         ----------
-        vars_int : numpy.ndarray
+        vars_int: numpy.ndarray
             The integer optimization variable values,
             shape: (n_vars_int,)
-        vars_float : numpy.ndarray
+        vars_float: numpy.ndarray
             The float optimization variable values,
             shape: (n_vars_float,)
 
         Returns
         -------
-        farm_vars : dict
+        farm_vars: dict
             The foxes farm variables. Key: var name,
             value: numpy.ndarray with values, shape:
             (n_states, n_sel_turbines)
 
         """
         pass
 
     @abstractmethod
     def opt2farm_vars_population(self, vars_int, vars_float, n_states):
         """
         Translates optimization variables to farm variables
 
         Parameters
         ----------
-        vars_int : numpy.ndarray
+        vars_int: numpy.ndarray
             The integer optimization variable values,
             shape: (n_pop, n_vars_int)
-        vars_float : numpy.ndarray
+        vars_float: numpy.ndarray
             The float optimization variable values,
             shape: (n_pop, n_vars_float)
-        n_states : int
+        n_states: int
             The number of original (non-pop) states
 
         Returns
         -------
-        farm_vars : dict
+        farm_vars: dict
             The foxes farm variables. Key: var name,
             value: numpy.ndarray with values, shape:
             (n_pop, n_states, n_sel_turbines)
 
         """
         pass
 
@@ -130,17 +133,17 @@
         the latest optimization variables.
 
         This function is called before running the farm
         calculation.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_vars_float,)
 
         """
         super().update_problem_individual(vars_int, vars_float)
 
         # prepare:
         n_states = self._org_n_states
@@ -173,17 +176,17 @@
         the latest optimization variables.
 
         This function is called before running the farm
         calculation.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_pop, n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_pop, n_vars_float,)
 
         """
         super().update_problem_population(vars_int, vars_float)
 
         # prepare:
         n_pop = len(vars_float)
```

### Comparing `foxes-0.3.5/foxes/opt/core/pop_states.py` & `foxes-0.4.0/foxes/opt/core/pop_states.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,31 +7,37 @@
 
 class PopStates(States):
     """
     Helper class for vectorized opt population
     calculation, via artificial states of length
     n_pop times n_states.
 
-    Parameters
-    ----------
-    states : foxes.core.States
-        The original states
-    n_pop : int
-        The population size
-
     Attributes
     ----------
-    states : foxes.core.States
+    states: foxes.core.States
         The original states
-    n_pop : int
+    n_pop: int
         The population size
 
+    :group: opt.core
+
     """
 
     def __init__(self, states, n_pop):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        states: foxes.core.States
+            The original states
+        n_pop: int
+            The population size
+
+        """
         super().__init__()
         self.states = states
         self.n_pop = n_pop
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
@@ -40,22 +46,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.STATE0 = self.var(FC.STATE + "0")
         self.SMAP = self.var("SMAP")
@@ -110,20 +116,20 @@
 
     def weights(self, algo):
         """
         The statistical weights of all states.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        weights : numpy.ndarray
+        weights: numpy.ndarray
             The weights, shape: (n_states, n_turbines)
 
         """
         weights = np.zeros(
             (self.n_pop, self.states.size(), algo.n_turbines), dtype=FC.DTYPE
         )
         weights[:] = self.states.weights(algo)[None, :, :] / self.n_pop
@@ -131,46 +137,46 @@
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return self.states.output_point_vars(algo)
 
     def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pdata : foxes.core.Data
+        pdata: foxes.core.Data
             The point data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
 
         hdata = {}
         hdims = {}
```

### Comparing `foxes-0.3.5/foxes/opt/objectives/farm_vars.py` & `foxes-0.4.0/foxes/opt/objectives/farm_vars.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,83 +5,88 @@
 from foxes import variables as FV
 import foxes.constants as FC
 
 class FarmVarObjective(FarmObjective):
     """
     Objectives based on farm variables.
 
-    Parameters
-    ----------
-    problem : foxes.opt.FarmOptProblem
-        The underlying optimization problem
-    name : str
-        The name of the objective function
-    variable : str
-        The foxes variable name
-    contract_states : str
-        Contraction rule for states: min, max, sum, mean
-    contract_turbines : str
-        Contraction rule for turbines: min, max, sum, mean
-    minimize : bool
-        Switch for maximizing or minimizing
-    deps : list of str
-        The foxes variables on which the variable depends,
-        or None for all
-    scale : float
-        The scaling factor
-    kwargs : dict, optional
-        Additional parameters for `FarmObjective`
-
     Attributes
     ----------
-    variable : str
+    variable: str
         The variable name
-    minimize : bool
+    minimize: bool
         Switch for maximizing or minimizing
-    deps : list of str
+    deps: list of str
         The foxes variables on which the variable depends,
         or None for all
-    rules : dict
+    rules: dict
         Contraction rules. Key: coordinate name str, value
         is str: min, max, sum, mean
-    scale : float
+    scale: float
         The scaling factor
 
+    :group: opt.objectives
+
     """
 
     def __init__(
         self,
         problem,
         name,
         variable,
         contract_states,
         contract_turbines,
         minimize,
         deps=None,
         scale=1.0,
         **kwargs,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        problem: foxes.opt.FarmOptProblem
+            The underlying optimization problem
+        name: str
+            The name of the objective function
+        variable: str
+            The foxes variable name
+        contract_states: str
+            Contraction rule for states: min, max, sum, mean
+        contract_turbines: str
+            Contraction rule for turbines: min, max, sum, mean
+        minimize: bool
+            Switch for maximizing or minimizing
+        deps: list of str
+            The foxes variables on which the variable depends,
+            or None for all
+        scale: float
+            The scaling factor
+        kwargs: dict, optional
+            Additional parameters for `FarmObjective`
+
+        """
         super().__init__(problem, name, **kwargs)
         self.variable = variable
         self.minimize = minimize
         self.deps = deps
         self.scale = scale
         self.rules = {FC.STATE: contract_states, FC.TURBINE: contract_turbines}
 
     def initialize(self, verbosity=0):
         """
         Initialize the object.
 
         Parameters
         ----------
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
-
         super().initialize(verbosity)
 
     def n_components(self):
         """
         Returns the number of components of the
         function.
 
@@ -95,29 +100,29 @@
 
     def maximize(self):
         """
         Returns flag for maximization of each component.
 
         Returns
         -------
-        flags : np.array
+        flags: np.array
             Bool array for component maximization,
             shape: (n_components,)
 
         """
         return [not self.minimize]
 
     def vardeps_float(self):
         """
         Gets the dependencies of all components
         on the function float variables
 
         Returns
         -------
-        deps : numpy.ndarray of bool
+        deps: numpy.ndarray of bool
             The dependencies of components on function
             variables, shape: (n_components, n_vars_float)
 
         """
         if self.deps is None:
             return super().vardeps_float()
 
@@ -151,27 +156,27 @@
     def calc_individual(self, vars_int, vars_float, problem_results, components=None):
         """
         Calculate values for a single individual of the
         underlying problem.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_vars_float,)
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
-        components : list of int, optional
+        components: list of int, optional
             The selected components or None for all
 
         Returns
         -------
-        values : np.array
+        values: np.array
             The component values, shape: (n_sel_components,)
 
         """
         data = problem_results[self.variable]
         if self.n_sel_turbines < self.farm.n_turbines:
             data = data[:, self.sel_turbines]
         data = self._contract(data) / self.scale
@@ -180,27 +185,27 @@
 
     def calc_population(self, vars_int, vars_float, problem_results, components=None):
         """
         Calculate values for all individuals of a population.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_pop, n_vars_int)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_pop, n_vars_float)
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
-        components : list of int, optional
+        components: list of int, optional
             The selected components or None for all
 
         Returns
         -------
-        values : np.array
+        values: np.array
             The component values, shape: (n_pop, n_sel_components)
 
         """
         n_pop = problem_results["n_pop"].values
         n_states = problem_results["n_org_states"].values
         n_turbines = problem_results.dims[FC.TURBINE]
         data = (
@@ -217,27 +222,27 @@
 
     def finalize_individual(self, vars_int, vars_float, problem_results, verbosity=1):
         """
         Finalization, given the champion data.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The optimal integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The optimal float variable values, shape: (n_vars_float,)
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        values : np.array
+        values: np.array
             The component values, shape: (n_components,)
 
         """
         return (
             super().finalize_individual(
                 vars_int, vars_float, problem_results, verbosity
             )
@@ -247,20 +252,22 @@
 
 class MaxFarmPower(FarmVarObjective):
     """
     Maximize the mean wind farm power
 
     Parameters
     ----------
-    problem : foxes.opt.FarmOptProblem
+    problem: foxes.opt.FarmOptProblem
         The underlying optimization problem
-    name : str
+    name: str
         The name of the objective function
-    kwargs : dict, optional
+    kwargs: dict, optional
         Additional parameters for `FarmVarObjective`
+    
+    :group: opt.objectives
 
     """
 
     def __init__(self, problem, name="maximize_power", **kwargs):
         if "scale" in kwargs:
             scale = kwargs.pop("scale")
         else:
@@ -286,20 +293,22 @@
 
 class MinimalMaxTI(FarmVarObjective):
     """
     Minimize the maximal turbine TI
 
     Parameters
     ----------
-    problem : foxes.opt.FarmOptProblem
+    problem: foxes.opt.FarmOptProblem
         The underlying optimization problem
-    name : str
+    name: str
         The name of the objective function
-    kwargs : dict, optional
+    kwargs: dict, optional
         Additional parameters for `FarmVarObjective`
+    
+    :group: opt.objectives
 
     """
 
     def __init__(self, problem, name="minimize_TI", **kwargs):
         scale = kwargs.pop("scale") if "scale" in kwargs else 1.0
         super().__init__(
             problem,
```

### Comparing `foxes-0.3.5/foxes/opt/objectives/max_n_turbines.py` & `foxes-0.4.0/foxes/opt/objectives/max_n_turbines.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,39 +3,45 @@
 from foxes.opt.core.farm_objective import FarmObjective
 import foxes.constants as FC
 
 class MaxNTurbines(FarmObjective):
     """
     Maximizes the number of turrbines.
 
-    Parameters
-    ----------
-    problem : foxes.opt.FarmOptProblem
-        The underlying optimization problem
-    name : str
-        The name of the objective function
-    check_valid : bool
-        Check FC.VALID variable before counting
-    kwargs : dict, optional
-        Additional parameters for `FarmObjective`
-
     Attributes
     ----------
-    check_valid : bool
+    check_valid: bool
         Check FC.VALID variable before counting
 
+    :group: opt.objectives
+
     """
 
     def __init__(
         self,
         problem,
         name="max_n_turbines",
         check_valid=True,
         **kwargs,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        problem: foxes.opt.FarmOptProblem
+            The underlying optimization problem
+        name: str
+            The name of the objective function
+        check_valid: bool
+            Check FC.VALID variable before counting
+        kwargs: dict, optional
+            Additional parameters for `FarmObjective`
+
+        """
         super().__init__(problem, name, **kwargs)
         self.check_valid = check_valid
 
     def n_components(self):
         """
         Returns the number of components of the
         function.
@@ -50,41 +56,41 @@
 
     def maximize(self):
         """
         Returns flag for maximization of each component.
 
         Returns
         -------
-        flags : np.array
+        flags: np.array
             Bool array for component maximization,
             shape: (n_components,)
 
         """
         return [True]
 
     def calc_individual(self, vars_int, vars_float, problem_results, components=None):
         """
         Calculate values for a single individual of the
         underlying problem.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_vars_float,)
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
-        components : list of int, optional
+        components: list of int, optional
             The selected components or None for all
 
         Returns
         -------
-        values : np.array
+        values: np.array
             The component values, shape: (n_sel_components,)
 
         """
         if FC.VALID in problem_results and self.check_valid:
             vld = np.sum(problem_results[FC.VALID].to_numpy(), axis=1)
             if np.min(vld) != np.max(vld):
                 raise ValueError(
@@ -96,27 +102,27 @@
 
     def calc_population(self, vars_int, vars_float, problem_results, components=None):
         """
         Calculate values for all individuals of a population.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_pop, n_vars_int)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_pop, n_vars_float)
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
-        components : list of int, optional
+        components: list of int, optional
             The selected components or None for all
 
         Returns
         -------
-        values : np.array
+        values: np.array
             The component values, shape: (n_pop, n_sel_components)
 
         """
         n_pop = problem_results["n_pop"].to_numpy()
         if self.check_valid:
             n_states = problem_results["n_org_states"].to_numpy()
             n_turbines = self.farm.n_turbines
```

### Comparing `foxes-0.3.5/foxes/opt/problems/layout/farm_layout.py` & `foxes-0.4.0/foxes/opt/problems/layout/farm_layout.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,38 +4,41 @@
 import foxes.variables as FV
 import foxes.constants as FC
 
 
 class FarmLayoutOptProblem(FarmVarsProblem):
     """
     The turbine positioning optimization problem
+
+    :group: opt.problems.layout
+    
     """
 
     def var_names_float(self):
         """
         The names of float variables.
 
         Returns
         -------
-        names : list of str
+        names: list of str
             The names of the float variables
 
         """
         vrs = []
         for ti in self.sel_turbines:
             vrs += [self.tvar(FV.X, ti), self.tvar(FV.Y, ti)]
         return vrs
 
     def initial_values_float(self):
         """
         The initial values of the float variables.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Initial float values, shape: (n_vars_float,)
 
         """
         out = np.zeros((self.n_sel_turbines, 2), dtype=FC.DTYPE)
         for i, ti in enumerate(self.sel_turbines):
             out[i] = self.farm.turbines[ti].xy
         return out.reshape(self.n_sel_turbines * 2)
@@ -44,15 +47,15 @@
         """
         The minimal values of the float variables.
 
         Use -numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Minimal float values, shape: (n_vars_float,)
 
         """
         b = self.farm.boundary
         assert b is not None, f"Problem '{self.name}': Missing wind farm boundary."
         out = np.zeros((self.n_sel_turbines, 2), dtype=FC.DTYPE)
         out[:] = b.p_min()[None, :]
@@ -62,15 +65,15 @@
         """
         The maximal values of the float variables.
 
         Use numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Maximal float values, shape: (n_vars_float,)
 
         """
         b = self.farm.boundary
         assert b is not None, f"Problem '{self.name}': Missing wind farm boundary."
         out = np.zeros((self.n_sel_turbines, 2), dtype=FC.DTYPE)
         out[:] = b.p_max()[None, :]
@@ -78,17 +81,17 @@
 
     def initialize(self, verbosity=1, **kwargs):
         """
         Initialize the object.
 
         Parameters
         ----------
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
-        kwargs : dict, optional
+        kwargs: dict, optional
             Additional parameters for super class init
 
         """
         super().initialize(
             pre_rotor_vars=[FV.X, FV.Y],
             post_rotor_vars=[],
             verbosity=verbosity,
@@ -97,24 +100,24 @@
 
     def opt2farm_vars_individual(self, vars_int, vars_float):
         """
         Translates optimization variables to farm variables
 
         Parameters
         ----------
-        vars_int : numpy.ndarray
+        vars_int: numpy.ndarray
             The integer optimization variable values,
             shape: (n_vars_int,)
-        vars_float : numpy.ndarray
+        vars_float: numpy.ndarray
             The float optimization variable values,
             shape: (n_vars_float,)
 
         Returns
         -------
-        farm_vars : dict
+        farm_vars: dict
             The foxes farm variables. Key: var name,
             value: numpy.ndarray with values, shape:
             (n_states, n_sel_turbines)
 
         """
         farm_vars = {
             FV.X: np.zeros((self.algo.n_states, self.n_sel_turbines), dtype=FC.DTYPE),
@@ -128,26 +131,26 @@
 
     def opt2farm_vars_population(self, vars_int, vars_float, n_states):
         """
         Translates optimization variables to farm variables
 
         Parameters
         ----------
-        vars_int : numpy.ndarray
+        vars_int: numpy.ndarray
             The integer optimization variable values,
             shape: (n_pop, n_vars_int)
-        vars_float : numpy.ndarray
+        vars_float: numpy.ndarray
             The float optimization variable values,
             shape: (n_pop, n_vars_float)
-        n_states : int
+        n_states: int
             The number of original (non-pop) states
 
         Returns
         -------
-        farm_vars : dict
+        farm_vars: dict
             The foxes farm variables. Key: var name,
             value: numpy.ndarray with values, shape:
             (n_pop, n_states, n_sel_turbines)
 
         """
         n_pop = len(vars_float)
         farm_vars = {
@@ -162,29 +165,29 @@
 
     def finalize_individual(self, vars_int, vars_float, verbosity=1):
         """
         Finalization, given the champion data.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The optimal integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The optimal float variable values, shape: (n_vars_float,)
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
-        objs : np.array
+        objs: np.array
             The objective function values, shape: (n_objectives,)
-        cons : np.array
+        cons: np.array
             The constraints values, shape: (n_constraints,)
 
         """
         res, objs, cons = super().finalize_individual(vars_int, vars_float, verbosity)
 
         xy = vars_float.reshape(self.n_sel_turbines, 2)
         for i, ti in enumerate(self.sel_turbines):
```

### Comparing `foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_layout.py` & `foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,50 +10,56 @@
     """
     A layout within a boundary geometry, purely
     defined by geometrical optimization (no wakes).
 
     This optimization problem does not involve
     wind farms.
 
-    Parameters
-    ----------
-    boundary : foxes.utils.geom2d.AreaGeometry
-        The boundary geometry
-    n_turbines : int
-        The number of turbines in the layout
-    min_dist : float, optional
-        The minimal distance between points
-    D : float, optional
-        The diameter of circle fully within boundary
-    calc_valid : bool, optional
-        Evaluate validity
-
     Attributes
     ----------
-    boundary : foxes.utils.geom2d.AreaGeometry
+    boundary: foxes.utils.geom2d.AreaGeometry
         The boundary geometry
-    n_turbines : int
+    n_turbines: int
         The number of turbines in the layout
-    min_dist : float
+    min_dist: float
         The minimal distance between points
-    D : float
+    D: float
         The diameter of circle fully within boundary
-    calc_valid : bool
+    calc_valid: bool
         Evaluate validity
+    
+    :group: opt.problems.layout.geom_layouts
 
     """
 
     def __init__(
         self,
         boundary,
         n_turbines,
         min_dist=None,
         D=None,
         calc_valid=None,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        boundary: foxes.utils.geom2d.AreaGeometry
+            The boundary geometry
+        n_turbines: int
+            The number of turbines in the layout
+        min_dist: float, optional
+            The minimal distance between points
+        D: float, optional
+            The diameter of circle fully within boundary
+        calc_valid: bool, optional
+            Evaluate validity
+
+        """
         super().__init__(name="geom_reg_grids")
 
         self.boundary = boundary
         self.n_turbines = n_turbines
         self.D = D
         self.min_dist = min_dist
         self.calc_valid = calc_valid
@@ -65,40 +71,40 @@
 
     def initialize(self, verbosity=1):
         """
         Initialize the object.
 
         Parameters
         ----------
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         super().initialize(verbosity)
         self.apply_individual(self.initial_values_int(), self.initial_values_float())
 
     def var_names_float(self):
         """
         The names of float variables.
 
         Returns
         -------
-        names : list of str
+        names: list of str
             The names of the float variables
 
         """
         return list(np.array([self._X, self._Y]).T.flat)
 
     def initial_values_float(self):
         """
         The initial values of the float variables.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Initial float values, shape: (n_vars_float,)
 
         """
         pmin = self.boundary.p_min()
         pmax = self.boundary.p_max()
         pc = 0.5 * (pmin + pmax)
         delta = 0.8 * (pmax - pmin)
@@ -115,15 +121,15 @@
         """
         The minimal values of the float variables.
 
         Use -numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Minimal float values, shape: (n_vars_float,)
 
         """
         vals = np.zeros((self.n_turbines, 2), dtype=FC.DTYPE)
         vals[:] = self.boundary.p_min()[None, :]
         return vals.reshape(self.n_turbines * 2)
 
@@ -131,36 +137,36 @@
         """
         The maximal values of the float variables.
 
         Use numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Maximal float values, shape: (n_vars_float,)
 
         """
         vals = np.zeros((self.n_turbines, 2), dtype=FC.DTYPE)
         vals[:] = self.boundary.p_max()[None, :]
         return vals.reshape(self.n_turbines * 2)
 
     def apply_individual(self, vars_int, vars_float):
         """
         Apply new variables to the problem.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_vars_float,)
 
         Returns
         -------
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
 
         """
         xy = vars_float.reshape(self.n_turbines, 2)
 
         valid = None
@@ -183,22 +189,22 @@
     def apply_population(self, vars_int, vars_float):
         """
         Apply new variables to the problem,
         for a whole population.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_pop, n_vars_int)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_pop, n_vars_float)
 
         Returns
         -------
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
 
         """
         n_pop = vars_float.shape[0]
         xy = vars_float.reshape(n_pop, self.n_turbines, 2)
 
@@ -226,30 +232,30 @@
         self, xy=None, valid=None, ax=None, title=None, true_circle=True, **bargs
     ):
         """
         Return plotly figure axis.
 
         Parameters
         ----------
-        xy : numpy.ndarary, optional
+        xy: numpy.ndarary, optional
             The xy coordinate array, shape: (n_points, 2)
-        valid : numpy.ndarray, optional
+        valid: numpy.ndarray, optional
             Boolean array of validity, shape: (n_points,)
-        ax : pyplot.Axis, optional
+        ax: pyplot.Axis, optional
             The figure axis
-        title : str, optional
+        title: str, optional
             The figure title
-        true_circle : bool
+        true_circle: bool
             Draw points as circles with diameter self.D
-        bars : dict, optional
+        bars: dict, optional
             The boundary plot arguments
 
         Returns
         -------
-        ax : pyplot.Axis
+        ax: pyplot.Axis
             The figure axis
 
         """
         if ax is None:
             __, ax = plt.subplots()
 
         hbargs = {"fill_mode": "inside_lightgray"}
```

### Comparing `foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py` & `foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,50 +11,56 @@
     A layout within a boundary geometry, purely
     defined by geometrical optimization (no wakes),
     on a fixes background point grid.
 
     This optimization problem does not involve
     wind farms.
 
-    Parameters
-    ----------
-    boundary : foxes.utils.geom2d.AreaGeometry
-        The boundary geometry
-    n_turbines : int
-        The number of turbines in the layout
-    grid_spacing : float
-        The background grid spacing
-    min_dist : float, optional
-        The minimal distance between points
-    D : float, optional
-        The diameter of circle fully within boundary
-
     Attributes
     ----------
-    boundary : foxes.utils.geom2d.AreaGeometry
+    boundary: foxes.utils.geom2d.AreaGeometry
         The boundary geometry
-    n_turbines : int
+    n_turbines: int
         The number of turbines in the layout
-    grid_spacing : float
+    grid_spacing: float
         The background grid spacing
-    min_dist : float
+    min_dist: float
         The minimal distance between points
-    D : float
+    D: float
         The diameter of circle fully within boundary
+    
+    :group: opt.problems.layout.geom_layouts
 
     """
 
     def __init__(
         self,
         boundary,
         n_turbines,
         grid_spacing,
         min_dist=None,
         D=None,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        boundary: foxes.utils.geom2d.AreaGeometry
+            The boundary geometry
+        n_turbines: int
+            The number of turbines in the layout
+        grid_spacing: float
+            The background grid spacing
+        min_dist: float, optional
+            The minimal distance between points
+        D: float, optional
+            The diameter of circle fully within boundary
+
+        """
         super().__init__(name="geom_reg_grids")
 
         self.boundary = boundary
         self.n_turbines = n_turbines
         self.grid_spacing = grid_spacing
         self.D = D
         self.min_dist = min_dist
@@ -63,15 +69,15 @@
 
     def initialize(self, verbosity=1):
         """
         Initialize the object.
 
         Parameters
         ----------
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         super().initialize(verbosity)
 
         pmin = self.boundary.p_min()
         pmax = self.boundary.p_max() + self.grid_spacing
@@ -107,70 +113,70 @@
 
     def var_names_int(self):
         """
         The names of int variables.
 
         Returns
         -------
-        names : list of str
+        names: list of str
             The names of the int variables
 
         """
         return self._I
 
     def initial_values_int(self):
         """
         The initial values of the int variables.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Initial int values, shape: (n_vars_int,)
 
         """
         return np.arange(self.n_turbines, dtype=FC.ITYPE)
 
     def min_values_int(self):
         """
         The minimal values of the int variables.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Minimal int values, shape: (n_vars_int,)
 
         """
         return np.zeros(self.n_turbines, dtype=FC.ITYPE)
 
     def max_values_int(self):
         """
         The maximal values of the int variables.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Maximal int values, shape: (n_vars_int,)
 
         """
         return np.full(self.n_turbines, self._N - 1, dtype=FC.ITYPE)
 
     def apply_individual(self, vars_int, vars_float):
         """
         Apply new variables to the problem.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_vars_float,)
 
         Returns
         -------
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
 
         """
         xy = self._pts[vars_int.astype(FC.ITYPE)]
         __, ui = np.unique(vars_int, return_index=True)
         valid = np.zeros(self.n_turbines, dtype=bool)
@@ -180,22 +186,22 @@
     def apply_population(self, vars_int, vars_float):
         """
         Apply new variables to the problem,
         for a whole population.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_pop, n_vars_int)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_pop, n_vars_float)
 
         Returns
         -------
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
 
         """
         n_pop = vars_int.shape[0]
 
         vint = vars_int.reshape(n_pop * self.n_turbines).astype(FC.ITYPE)
@@ -212,30 +218,30 @@
         self, xy=None, valid=None, ax=None, title=None, true_circle=True, **bargs
     ):
         """
         Return plotly figure axis.
 
         Parameters
         ----------
-        xy : numpy.ndarary, optional
+        xy: numpy.ndarary, optional
             The xy coordinate array, shape: (n_points, 2)
-        valid : numpy.ndarray, optional
+        valid: numpy.ndarray, optional
             Boolean array of validity, shape: (n_points,)
-        ax : pyplot.Axis, optional
+        ax: pyplot.Axis, optional
             The figure axis
-        title : str, optional
+        title: str, optional
             The figure title
-        true_circle : bool
+        true_circle: bool
             Draw points as circles with diameter self.D
-        bars : dict, optional
+        bars: dict, optional
             The boundary plot arguments
 
         Returns
         -------
-        ax : pyplot.Axis
+        ax: pyplot.Axis
             The figure axis
 
         """
         if ax is None:
             __, ax = plt.subplots()
 
         hbargs = {"fill_mode": "inside_lightgray"}
```

### Comparing `foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py` & `foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,50 +9,56 @@
 class GeomRegGrid(Problem):
     """
     A regular grid within a boundary geometry.
 
     This optimization problem does not involve
     wind farms.
 
-    Parameters
-    ----------
-    boundary : foxes.utils.geom2d.AreaGeometry
-        The boundary geometry
-    n_turbines : int
-        The number of turbines in the layout
-    min_dist : float
-        The minimal distance between points
-    max_dist : float, optional
-        The maximal distance between points
-    D : float, optional
-        The diameter of circle fully within boundary
-
     Attributes
     ----------
-    boundary : foxes.utils.geom2d.AreaGeometry
+    boundary: foxes.utils.geom2d.AreaGeometry
         The boundary geometry
-    n_turbines : int
+    n_turbines: int
         The number of turbines in the layout
-    min_dist : float
+    min_dist: float
         The minimal distance between points
-    max_dist : float
+    max_dist: float
         The maximal distance between points
-    D : float
+    D: float
         The diameter of circle fully within boundary
+    
+    :group: opt.problems.layout.geom_layouts
 
     """
 
     def __init__(
         self,
         boundary,
         n_turbines,
         min_dist,
         max_dist=None,
         D=None,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        boundary: foxes.utils.geom2d.AreaGeometry
+            The boundary geometry
+        n_turbines: int
+            The number of turbines in the layout
+        min_dist: float
+            The minimal distance between points
+        max_dist: float, optional
+            The maximal distance between points
+        D: float, optional
+            The diameter of circle fully within boundary
+
+        """
         super().__init__(name="geom_reg_grid")
 
         self.boundary = boundary
         self.n_turbines = n_turbines
         self.min_dist = float(min_dist)
         self.max_dist = float(max_dist) if max_dist is not None else max_dist
         self.D = D
@@ -65,15 +71,15 @@
 
     def initialize(self, verbosity=1):
         """
         Initialize the object.
 
         Parameters
         ----------
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         super().initialize(verbosity)
 
         pmin = self.boundary.p_min()
         pmax = self.boundary.p_max()
@@ -98,27 +104,27 @@
 
     def var_names_float(self):
         """
         The names of float variables.
 
         Returns
         -------
-        names : list of str
+        names: list of str
             The names of the float variables
 
         """
         return list(np.array([self._SX, self._SY, self._DX, self._DY, self._ALPHA]))
 
     def initial_values_float(self):
         """
         The initial values of the float variables.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Initial float values, shape: (n_vars_float,)
 
         """
         vals = np.zeros(5, dtype=FC.DTYPE)
         vals[2:4] = self.min_dist
         return vals
 
@@ -126,15 +132,15 @@
         """
         The minimal values of the float variables.
 
         Use -numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Minimal float values, shape: (n_vars_float,)
 
         """
         vals = np.zeros(5, dtype=FC.DTYPE)
         vals[:2] = -0.5
         vals[2:4] = self.min_dist
         return vals
@@ -143,15 +149,15 @@
         """
         The maximal values of the float variables.
 
         Use numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Maximal float values, shape: (n_vars_float,)
 
         """
         vals = np.zeros(5, dtype=FC.DTYPE)
         vals[:2] = 0.5
         vals[2:4] = self.max_dist
         vals[4] = 90.0
@@ -159,22 +165,22 @@
 
     def apply_individual(self, vars_int, vars_float):
         """
         Apply new variables to the problem.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_vars_float,)
 
         Returns
         -------
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
 
         """
         sx, sy, dx, dy, alpha = vars_float
 
         a = np.deg2rad(alpha)
@@ -211,22 +217,22 @@
     def apply_population(self, vars_int, vars_float):
         """
         Apply new variables to the problem,
         for a whole population.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_pop, n_vars_int)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_pop, n_vars_float)
 
         Returns
         -------
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
 
         """
         n_pop = vars_float.shape[0]
         sx = vars_float[:, 0]
         sy = vars_float[:, 1]
@@ -275,42 +281,42 @@
                 vld[pi] = np.ones(self.n_turbines, dtype=bool)
             else:
                 qts[pi] = np.append(
                     pts[pi, valid[pi]],
                     pts[pi, ~valid[pi]][: (self.n_turbines - nvl[pi])],
                     axis=0,
                 )
-                vld[pi, : nvl[pi]] = True
+                vld[pi,: nvl[pi]] = True
 
         return qts, vld
 
     def get_fig(
         self, xy=None, valid=None, ax=None, title=None, true_circle=True, **bargs
     ):
         """
         Return plotly figure axis.
 
         Parameters
         ----------
-        xy : numpy.ndarary, optional
+        xy: numpy.ndarary, optional
             The xy coordinate array, shape: (n_points, 2)
-        valid : numpy.ndarray, optional
+        valid: numpy.ndarray, optional
             Boolean array of validity, shape: (n_points,)
-        ax : pyplot.Axis, optional
+        ax: pyplot.Axis, optional
             The figure axis
-        title : str, optional
+        title: str, optional
             The figure title
-        true_circle : bool
+        true_circle: bool
             Draw points as circles with diameter self.D
-        bars : dict, optional
+        bars: dict, optional
             The boundary plot arguments
 
         Returns
         -------
-        ax : pyplot.Axis
+        ax: pyplot.Axis
             The figure axis
 
         """
         if ax is None:
             __, ax = plt.subplots()
 
         hbargs = {"fill_mode": "inside_lightgray"}
```

### Comparing `foxes-0.3.5/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py` & `foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,60 +9,66 @@
 class GeomRegGrids(Problem):
     """
     A regular grid within a boundary geometry.
 
     This optimization problem does not involve
     wind farms.
 
-    Parameters
-    ----------
-    boundary : foxes.utils.geom2d.AreaGeometry
-        The boundary geometry
-    min_dist : float
-        The minimal distance between points
-    n_grids : int
-        The number of grids
-    n_max : int, optional
-        The maximal number of points
-    n_row_max : int, optional
-        The maximal number of points in a row
-    max_dist : float, optional
-        The maximal distance between points
-    D : float, optional
-        The diameter of circle fully within boundary
-
     Attributes
     ----------
-    boundary : foxes.utils.geom2d.AreaGeometry
+    boundary: foxes.utils.geom2d.AreaGeometry
         The boundary geometry
-    min_dist : float
+    min_dist: float
         The minimal distance between points
-    n_grids : int
+    n_grids: int
         The number of grids
-    n_max : int
+    n_max: int
         The maximal number of points
-    n_row_max : int
+    n_row_max: int
         The maximal number of points in a row
-    max_dist : float
+    max_dist: float
         The maximal distance between points
-    D : float
+    D: float
         The diameter of circle fully within boundary
+    
+    :group: opt.problems.layout.geom_layouts
 
     """
 
     def __init__(
         self,
         boundary,
         min_dist,
         n_grids,
         n_max=None,
         n_row_max=None,
         max_dist=None,
         D=None,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        boundary: foxes.utils.geom2d.AreaGeometry
+            The boundary geometry
+        min_dist: float
+            The minimal distance between points
+        n_grids: int
+            The number of grids
+        n_max: int, optional
+            The maximal number of points
+        n_row_max: int, optional
+            The maximal number of points in a row
+        max_dist: float, optional
+            The maximal distance between points
+        D: float, optional
+            The diameter of circle fully within boundary
+
+        """
         super().__init__(name="geom_reg_grids")
 
         self.boundary = boundary
         self.n_grids = n_grids
         self.n_max = n_max
         self.n_row_max = n_row_max
         self.min_dist = float(min_dist)
@@ -79,15 +85,15 @@
 
     def initialize(self, verbosity=1):
         """
         Initialize the object.
 
         Parameters
         ----------
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         super().initialize(verbosity)
 
         pmin = self.boundary.p_min()
         pmax = self.boundary.p_max()
@@ -124,81 +130,81 @@
 
     def var_names_int(self):
         """
         The names of int variables.
 
         Returns
         -------
-        names : list of str
+        names: list of str
             The names of the int variables
 
         """
         return list(np.array([self._NX, self._NY]).T.flat)
 
     def initial_values_int(self):
         """
         The initial values of the int variables.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Initial int values, shape: (n_vars_int,)
 
         """
         return np.full(self.n_grids * 2, 2, dtype=FC.ITYPE)
 
     def min_values_int(self):
         """
         The minimal values of the integer variables.
 
         Use -self.INT_INF for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Minimal int values, shape: (n_vars_int,)
 
         """
         return np.ones(self.n_grids * 2, dtype=FC.ITYPE)
 
     def max_values_int(self):
         """
         The maximal values of the integer variables.
 
         Use self.INT_INF for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Maximal int values, shape: (n_vars_int,)
 
         """
         return np.full(self.n_grids * 2, self._nrow, dtype=FC.ITYPE)
 
     def var_names_float(self):
         """
         The names of float variables.
 
         Returns
         -------
-        names : list of str
+        names: list of str
             The names of the float variables
 
         """
         return list(
             np.array([self._OX, self._OY, self._DX, self._DY, self._ALPHA]).T.flat
         )
 
     def initial_values_float(self):
         """
         The initial values of the float variables.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Initial float values, shape: (n_vars_float,)
 
         """
         n = 5
         vals = np.zeros((self.n_grids, n), dtype=FC.DTYPE)
         vals[:, :2] = self._pmin + self._diag + self.min_dist + self._span / 2
         vals[:, 2:4] = 2 * self.min_dist
@@ -209,15 +215,15 @@
         """
         The minimal values of the float variables.
 
         Use -numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Minimal float values, shape: (n_vars_float,)
 
         """
         n = 5
         vals = np.zeros((self.n_grids, n), dtype=FC.DTYPE)
         vals[:, :2] = self._pmin
         vals[:, 2:4] = self.min_dist
@@ -228,15 +234,15 @@
         """
         The maximal values of the float variables.
 
         Use numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Maximal float values, shape: (n_vars_float,)
 
         """
         n = 5
         vals = np.zeros((self.n_grids, n), dtype=FC.DTYPE)
         vals[:, :2] = self._pmax
         vals[:, 2:4] = self.max_dist
@@ -246,22 +252,22 @@
 
     def apply_individual(self, vars_int, vars_float):
         """
         Apply new variables to the problem.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_vars_float,)
 
         Returns
         -------
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
 
         """
         vint = vars_int.reshape(self.n_grids, 2)
         vflt = vars_float.reshape(self.n_grids, 5)
         nx = vint[:, 0]
@@ -328,22 +334,22 @@
     def apply_population(self, vars_int, vars_float):
         """
         Apply new variables to the problem,
         for a whole population.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_pop, n_vars_int)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_pop, n_vars_float)
 
         Returns
         -------
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
 
         """
         n_pop = vars_int.shape[0]
         vint = vars_int.reshape(n_pop, self.n_grids, 2)
         vflt = vars_float.reshape(n_pop, self.n_grids, 5)
@@ -418,30 +424,30 @@
         self, xy=None, valid=None, ax=None, title=None, true_circle=True, **bargs
     ):
         """
         Return plotly figure axis.
 
         Parameters
         ----------
-        xy : numpy.ndarary, optional
+        xy: numpy.ndarary, optional
             The xy coordinate array, shape: (n_points, 2)
-        valid : numpy.ndarray, optional
+        valid: numpy.ndarray, optional
             Boolean array of validity, shape: (n_points,)
-        ax : pyplot.Axis, optional
+        ax: pyplot.Axis, optional
             The figure axis
-        title : str, optional
+        title: str, optional
             The figure title
-        true_circle : bool
+        true_circle: bool
             Draw points as circles with diameter self.D
-        bars : dict, optional
+        bars: dict, optional
             The boundary plot arguments
 
         Returns
         -------
-        ax : pyplot.Axis
+        ax: pyplot.Axis
             The figure axis
 
         """
         if ax is None:
             __, ax = plt.subplots()
 
         hbargs = {"fill_mode": "inside_lightgray"}
```

### Comparing `foxes-0.3.5/foxes/opt/problems/layout/reggrids_layout.py` & `foxes-0.4.0/foxes/opt/problems/layout/reggrids_layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,56 +12,62 @@
     """
     Places turbines on several regular grids and optimizes
     their parameters.
 
     Note that this problem has both int and float variables
     (mixed problem).
 
-    Parameters
-    ----------
-    name : str
-        The problem's name
-    algo : foxes.core.Algorithm
-        The algorithm
-    min_dist : float
-        The minimal distance between points
-    n_grids : int
-        The number of grids
-    n_row_max : int, optional
-        The maximal number of points in a row
-    max_dist : float, optional
-        The maximal distance between points
-    runner : foxes.core.Runner, optional
-        The runner for running the algorithm
-    kwargs : dict, optional
-        Additional parameters for `FarmVarsProblem`
-
     Attributes
     ----------
-    min_spacing : float
+    min_spacing: float
         The minimal turbine spacing
-    n_grids : int
+    n_grids: int
         The number of grids
-    max_n_row : int
+    max_n_row: int
         The maximal number of turbines per
         grid and row
+    
+    :group: opt.problems.layout
 
     """
 
     def __init__(
         self,
         name,
         algo,
         min_dist,
         n_grids=1,
         n_row_max=None,
         max_dist=None,
         runner=None,
         **kwargs,
     ):
+        """
+        Constraints.
+        
+        Parameters
+        ----------
+        name: str
+            The problem's name
+        algo: foxes.core.Algorithm
+            The algorithm
+        min_dist: float
+            The minimal distance between points
+        n_grids: int
+            The number of grids
+        n_row_max: int, optional
+            The maximal number of points in a row
+        max_dist: float, optional
+            The maximal distance between points
+        runner: foxes.core.Runner, optional
+            The runner for running the algorithm
+        kwargs: dict, optional
+            Additional parameters for `FarmVarsProblem`
+
+        """
         super().__init__(name, algo, runner, **kwargs)
 
         b = algo.farm.boundary
         assert b is not None, f"Problem '{self.name}': Missing wind farm boundary."
 
         self._geomp = GeomRegGrids(
             b,
@@ -73,17 +79,17 @@
 
     def initialize(self, verbosity=1, **kwargs):
         """
         Initialize the object.
 
         Parameters
         ----------
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
-        kwargs : dict, optional
+        kwargs: dict, optional
             Additional parameters for super class init
 
         """
         self._geomp.objs = self.objs
         self._geomp.cons = self.cons
         self._geomp.initialize(verbosity)
 
@@ -109,107 +115,107 @@
 
     def var_names_int(self):
         """
         The names of int variables.
 
         Returns
         -------
-        names : list of str
+        names: list of str
             The names of the int variables
 
         """
         return self._geomp.var_names_int()
 
     def initial_values_int(self):
         """
         The initial values of the int variables.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Initial int values, shape: (n_vars_int,)
 
         """
         return self._geomp.initial_values_int()
 
     def min_values_int(self):
         """
         The minimal values of the integer variables.
 
         Use -self.INT_INF for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Minimal int values, shape: (n_vars_int,)
 
         """
         return self._geomp.min_values_int()
 
     def max_values_int(self):
         """
         The maximal values of the integer variables.
 
         Use self.INT_INF for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Maximal int values, shape: (n_vars_int,)
 
         """
         return self._geomp.max_values_int()
 
     def var_names_float(self):
         """
         The names of float variables.
 
         Returns
         -------
-        names : list of str
+        names: list of str
             The names of the float variables
 
         """
         return self._geomp.var_names_float()
 
     def initial_values_float(self):
         """
         The initial values of the float variables.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Initial float values, shape: (n_vars_float,)
 
         """
         return self._geomp.initial_values_float()
 
     def min_values_float(self):
         """
         The minimal values of the float variables.
 
         Use -numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Minimal float values, shape: (n_vars_float,)
 
         """
         return self._geomp.min_values_float()
 
     def max_values_float(self):
         """
         The maximal values of the float variables.
 
         Use numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Maximal float values, shape: (n_vars_float,)
 
         """
         return self._geomp.max_values_float()
 
     def update_problem_individual(self, vars_int, vars_float):
         """
@@ -217,17 +223,17 @@
         the latest optimization variables.
 
         This function is called before running the farm
         calculation.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_vars_float,)
 
         """
         n0 = self.farm.n_turbines
         nxny = vars_int.reshape(self._geomp.n_grids, 2)
         n = np.sum(np.product(nxny, axis=1))
         if n0 > n:
@@ -248,17 +254,17 @@
         the latest optimization variables.
 
         This function is called before running the farm
         calculation.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The integer variable values, shape: (n_pop, n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The float variable values, shape: (n_pop, n_vars_float,)
 
         """
         n0 = self.farm.n_turbines
         n_pop = vars_int.shape[0]
         nxny = vars_int.reshape(n_pop, self._geomp.n_grids, 2)
         n = np.max(np.sum(np.product(nxny, axis=2), axis=1))
@@ -276,24 +282,24 @@
 
     def opt2farm_vars_individual(self, vars_int, vars_float):
         """
         Translates optimization variables to farm variables
 
         Parameters
         ----------
-        vars_int : numpy.ndarray
+        vars_int: numpy.ndarray
             The integer optimization variable values,
             shape: (n_vars_int,)
-        vars_float : numpy.ndarray
+        vars_float: numpy.ndarray
             The float optimization variable values,
             shape: (n_vars_float,)
 
         Returns
         -------
-        farm_vars : dict
+        farm_vars: dict
             The foxes farm variables. Key: var name,
             value: numpy.ndarray with values, shape:
             (n_states, n_sel_turbines)
 
         """
         pts, vld = self._geomp.apply_individual(vars_int, vars_float)
 
@@ -320,26 +326,26 @@
 
     def opt2farm_vars_population(self, vars_int, vars_float, n_states):
         """
         Translates optimization variables to farm variables
 
         Parameters
         ----------
-        vars_int : numpy.ndarray
+        vars_int: numpy.ndarray
             The integer optimization variable values,
             shape: (n_pop, n_vars_int)
-        vars_float : numpy.ndarray
+        vars_float: numpy.ndarray
             The float optimization variable values,
             shape: (n_pop, n_vars_float)
-        n_states : int
+        n_states: int
             The number of original (non-pop) states
 
         Returns
         -------
-        farm_vars : dict
+        farm_vars: dict
             The foxes farm variables. Key: var name,
             value: numpy.ndarray with values, shape:
             (n_pop, n_states, n_sel_turbines)
 
         """
         pts, vld = self._geomp.apply_population(vars_int, vars_float)
 
@@ -370,29 +376,29 @@
 
     def finalize_individual(self, vars_int, vars_float, verbosity=1):
         """
         Finalization, given the champion data.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The optimal integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The optimal float variable values, shape: (n_vars_float,)
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
-        objs : np.array
+        objs: np.array
             The objective function values, shape: (n_objectives,)
-        cons : np.array
+        cons: np.array
             The constraints values, shape: (n_constraints,)
 
         """
         pts, vld = self._geomp.apply_individual(vars_int, vars_float)
         xy = pts[vld]
         n_xy = xy.shape[0]
```

### Comparing `foxes-0.3.5/foxes/opt/problems/layout/regular_layout.py` & `foxes-0.4.0/foxes/opt/problems/layout/regular_layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,21 @@
 
 
 class RegularLayoutOptProblem(FarmVarsProblem):
     """
     Places turbines on a regular grid and optimizes
     its parameters.
 
-    Parameters
-    ----------
-    name : str
-        The problem's name
-    algo : foxes.core.Algorithm
-        The algorithm
-    min_spacing : float
-        The minimal turbine spacing
-    kwargs : dict, optional
-        Additional parameters for `FarmVarsProblem`
-
     Attributes
     ----------
-    min_spacing : float
+    min_spacing: float
         The minimal turbine spacing
 
+    :group: opt.problems.layout
+
     """
 
     SPACING_X = "spacing_x"
     SPACING_Y = "spacing_y"
     OFFSET_X = "offset_X"
     OFFSET_Y = "offset_Y"
     ANGLE = "angle"
@@ -39,26 +30,41 @@
     def __init__(
         self,
         name,
         algo,
         min_spacing,
         **kwargs,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        name: str
+            The problem's name
+        algo: foxes.core.Algorithm
+            The algorithm
+        min_spacing: float
+            The minimal turbine spacing
+        kwargs: dict, optional
+            Additional parameters for `FarmVarsProblem`
+
+        """
         super().__init__(name, algo, **kwargs)
         self.min_spacing = min_spacing
 
     def initialize(self, verbosity=1, **kwargs):
         """
         Initialize the object.
 
         Parameters
         ----------
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
-        kwargs : dict, optional
+        kwargs: dict, optional
             Additional parameters for super class init
 
         """
         self._mname = self.name + "_calc"
         for t in self.algo.farm.turbines:
             if self._mname not in t.models:
                 t.models.append(self._mname)
@@ -116,15 +122,15 @@
 
     def var_names_float(self):
         """
         The names of float variables.
 
         Returns
         -------
-        names : list of str
+        names: list of str
             The names of the float variables
 
         """
         return [
             self.SPACING_X,
             self.SPACING_Y,
             self.OFFSET_X,
@@ -134,29 +140,29 @@
 
     def initial_values_float(self):
         """
         The initial values of the float variables.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Initial float values, shape: (n_vars_float,)
 
         """
         return [self.min_spacing, self.min_spacing, 0.0, 0.0, 0.0]
 
     def min_values_float(self):
         """
         The minimal values of the float variables.
 
         Use -numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Minimal float values, shape: (n_vars_float,)
 
         """
         return [
             self.min_spacing,
             self.min_spacing,
             -self._halfspan[0] - self.min_spacing,
@@ -168,15 +174,15 @@
         """
         The maximal values of the float variables.
 
         Use numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Maximal float values, shape: (n_vars_float,)
 
         """
         return [
             self.max_spacing,
             self.max_spacing,
             self._halfspan[0] + self.min_spacing,
@@ -186,24 +192,24 @@
 
     def opt2farm_vars_individual(self, vars_int, vars_float):
         """
         Translates optimization variables to farm variables
 
         Parameters
         ----------
-        vars_int : numpy.ndarray
+        vars_int: numpy.ndarray
             The integer optimization variable values,
             shape: (n_vars_int,)
-        vars_float : numpy.ndarray
+        vars_float: numpy.ndarray
             The float optimization variable values,
             shape: (n_vars_float,)
 
         Returns
         -------
-        farm_vars : dict
+        farm_vars: dict
             The foxes farm variables. Key: var name,
             value: numpy.ndarray with values, shape:
             (n_states, n_sel_turbines)
 
         """
 
         dx, dy, ox, oy, a = vars_float
@@ -236,26 +242,26 @@
 
     def opt2farm_vars_population(self, vars_int, vars_float, n_states):
         """
         Translates optimization variables to farm variables
 
         Parameters
         ----------
-        vars_int : numpy.ndarray
+        vars_int: numpy.ndarray
             The integer optimization variable values,
             shape: (n_pop, n_vars_int)
-        vars_float : numpy.ndarray
+        vars_float: numpy.ndarray
             The float optimization variable values,
             shape: (n_pop, n_vars_float)
-        n_states : int
+        n_states: int
             The number of original (non-pop) states
 
         Returns
         -------
-        farm_vars : dict
+        farm_vars: dict
             The foxes farm variables. Key: var name,
             value: numpy.ndarray with values, shape:
             (n_pop, n_states, n_sel_turbines)
 
         """
         n_pop = len(vars_float)
         n_turbines = self.farm.n_turbines
@@ -305,29 +311,29 @@
 
     def finalize_individual(self, vars_int, vars_float, verbosity=1):
         """
         Finalization, given the champion data.
 
         Parameters
         ----------
-        vars_int : np.array
+        vars_int: np.array
             The optimal integer variable values, shape: (n_vars_int,)
-        vars_float : np.array
+        vars_float: np.array
             The optimal float variable values, shape: (n_vars_float,)
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        problem_results : Any
+        problem_results: Any
             The results of the variable application
             to the problem
-        objs : np.array
+        objs: np.array
             The objective function values, shape: (n_objectives,)
-        cons : np.array
+        cons: np.array
             The constraints values, shape: (n_constraints,)
 
         """
         farm_vars = self.opt2farm_vars_individual(vars_int, vars_float)
         sel = np.where(farm_vars[FC.VALID][0])[0]
         x = farm_vars[FV.X][0, sel]
         y = farm_vars[FV.Y][0, sel]
```

### Comparing `foxes-0.3.5/foxes/opt/problems/opt_farm_vars.py` & `foxes-0.4.0/foxes/opt/problems/opt_farm_vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import numpy as np
 import pandas as pd
 
 from foxes.opt.core import FarmVarsProblem
 from foxes.models.turbine_models import SetFarmVars
-import foxes.variables as FV
 import foxes.constants as FC
 
 
 class OptFarmVars(FarmVarsProblem):
     """
     Optimize a selection of farm variables.
 
-    Parameters
-    ----------
-    args : tuple, optional
-        Arguments for `FarmVarsProblem`
-    kwargs : dict, optional
-        Keyword arguments for `FarmVarsProblem`
+    :group: opt.problems
 
     """
 
     def __init__(self, *args, **kwargs):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        args: tuple, optional
+            Arguments for `FarmVarsProblem`
+        kwargs: dict, optional
+            Keyword arguments for `FarmVarsProblem`
+
+        """
         super().__init__(*args, **kwargs)
         self._vars = None
 
     def add_var(
         self,
         name,
         typ,
@@ -37,41 +42,37 @@
         model_key=None,
     ):
         """
         Add a variable.
 
         Parameters
         ----------
-        name : str
+        name: str
             The foxes farm variable name
-        typ : type
+        typ: type
             The variable type, either float or int
-        init : float or int
+        init: float or int
             The initial value
-        min : float or int
+        min: float or int
             The min value
-        max : float or int
+        max: float or int
             The max value
-        level : str
+        level: str
             Choices: uniform, state, turbine, state-turbine
-        sel : numpy.ndarray, optional
+        sel: numpy.ndarray, optional
             States/turbines/state-turbine selection,
             depending on the level
-        pre_rotor : bool
+        pre_rotor: bool
             Apply this variable before rotor model
-        model_key : str, optional
+        model_key: str, optional
             Creates sub-model which can then be placed in the
             turbine model list. Repeated keys are added to the
             same turbine model
 
         """
-        if not hasattr(FV, name):
-            raise ValueError(
-                f"Problem '{self.name}': Name '{name}' is not a foxes variable."
-            )
         if typ is not float and typ is not int:
             raise TypeError(
                 f"Problem '{self.name}': Expecting float or int, got type '{type(typ).__name__}'"
             )
 
         mname = self.name if model_key is None else model_key
         if mname in self.algo.mbook.turbine_models:
@@ -236,17 +237,17 @@
 
     def initialize(self, verbosity=1, **kwargs):
         """
         Initialize the object.
 
         Parameters
         ----------
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
-        kwargs : dict, optional
+        kwargs: dict, optional
             Additional parameters for super class init
 
         """
         if self._vars is None:
             raise ValueError(
                 f"Problem '{self.name}': No variables added for optimization."
             )
@@ -279,15 +280,15 @@
 
     def var_names_int(self):
         """
         The names of int variables.
 
         Returns
         -------
-        names : list of str
+        names: list of str
             The names of the int variables
 
         """
         if self._vars is None:
             raise ValueError(
                 f"Problem '{self.name}': No variables added for optimization."
             )
@@ -300,15 +301,15 @@
 
     def initial_values_int(self):
         """
         The initial values of the int variables.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Initial int values, shape: (n_vars_int,)
 
         """
         if self._vars is None:
             raise ValueError(
                 f"Problem '{self.name}': No variables added for optimization."
             )
@@ -323,15 +324,15 @@
         """
         The minimal values of the integer variables.
 
         Use -self.INT_INF for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Minimal int values, shape: (n_vars_int,)
 
         """
         if self._vars is None:
             raise ValueError(
                 f"Problem '{self.name}': No variables added for optimization."
             )
@@ -346,15 +347,15 @@
         """
         The maximal values of the integer variables.
 
         Use self.INT_INF for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Maximal int values, shape: (n_vars_int,)
 
         """
         if self._vars is None:
             raise ValueError(
                 f"Problem '{self.name}': No variables added for optimization."
             )
@@ -367,15 +368,15 @@
 
     def var_names_float(self):
         """
         The names of float variables.
 
         Returns
         -------
-        names : list of str
+        names: list of str
             The names of the float variables
 
         """
         if self._vars is None:
             raise ValueError(
                 f"Problem '{self.name}': No variables added for optimization."
             )
@@ -388,15 +389,15 @@
 
     def initial_values_float(self):
         """
         The initial values of the float variables.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Initial float values, shape: (n_vars_float,)
 
         """
         if self._vars is None:
             raise ValueError(
                 f"Problem '{self.name}': No variables added for optimization."
             )
@@ -411,15 +412,15 @@
         """
         The minimal values of the float variables.
 
         Use -numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Minimal float values, shape: (n_vars_float,)
 
         """
         if self._vars is None:
             raise ValueError(
                 f"Problem '{self.name}': No variables added for optimization."
             )
@@ -434,15 +435,15 @@
         """
         The maximal values of the float variables.
 
         Use numpy.inf for unbounded.
 
         Returns
         -------
-        values : numpy.ndarray
+        values: numpy.ndarray
             Maximal float values, shape: (n_vars_float,)
 
         """
         if self._vars is None:
             raise ValueError(
                 f"Problem '{self.name}': No variables added for optimization."
             )
@@ -455,39 +456,39 @@
 
     def opt2farm_vars_individual(self, vars_int, vars_float):
         """
         Translates optimization variables to farm variables
 
         Parameters
         ----------
-        vars_int : numpy.ndarray
+        vars_int: numpy.ndarray
             The integer optimization variable values,
             shape: (n_vars_int,)
-        vars_float : numpy.ndarray
+        vars_float: numpy.ndarray
             The float optimization variable values,
             shape: (n_vars_float,)
 
         Returns
         -------
-        farm_vars : dict
+        farm_vars: dict
             The foxes farm variables. Key: var name,
             value: numpy.ndarray with values, shape:
             (n_states, n_sel_turbines)
 
         """
         n_states = self.algo.n_states
         n_sturb = self.n_sel_turbines
 
         farm_vars = {}
         grps = self._vars.groupby(["type", "var", "level"])
         for (typ, var, level), g in grps:
             src = vars_int if typ == "int" else vars_float
             i0 = g.index[0]
             i1 = g.index[-1]
-            data = src[np.s_[i0 : i1 + 1]]
+            data = src[np.s_[i0: i1 + 1]]
 
             if level == "uniform":
                 farm_vars[var] = np.full((n_states, n_sturb), data[0], dtype=FC.DTYPE)
 
             elif level == "state":
                 farm_vars[var] = np.full((n_states, n_sturb), np.nan, dtype=FC.DTYPE)
                 if np.all(g["state"] == np.arange(n_states)):
@@ -515,41 +516,41 @@
 
     def opt2farm_vars_population(self, vars_int, vars_float, n_states):
         """
         Translates optimization variables to farm variables
 
         Parameters
         ----------
-        vars_int : numpy.ndarray
+        vars_int: numpy.ndarray
             The integer optimization variable values,
             shape: (n_pop, n_vars_int)
-        vars_float : numpy.ndarray
+        vars_float: numpy.ndarray
             The float optimization variable values,
             shape: (n_pop, n_vars_float)
-        n_states : int
+        n_states: int
             The number of original (non-pop) states
 
         Returns
         -------
-        farm_vars : dict
+        farm_vars: dict
             The foxes farm variables. Key: var name,
             value: numpy.ndarray with values, shape:
             (n_pop, n_states, n_sel_turbines)
 
         """
         n_pop = vars_float.shape[0]
         n_sturb = self.n_sel_turbines
 
         farm_vars = {}
         grps = self._vars.groupby(["type", "var", "level"])
         for (typ, var, level), g in grps:
             src = vars_int if typ == "int" else vars_float
             i0 = g.index[0]
             i1 = g.index[-1]
-            data = src[:, np.s_[i0 : i1 + 1]]
+            data = src[:, np.s_[i0: i1 + 1]]
 
             if level == "uniform":
                 farm_vars[var] = np.full(
                     (n_pop, n_states, n_sturb), np.nan, dtype=FC.DTYPE
                 )
                 farm_vars[var][:] = data[:, 0, None, None]
```

### Comparing `foxes-0.3.5/foxes/output/farm_layout.py` & `foxes-0.4.0/foxes/output/farm_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,45 +9,51 @@
 from foxes.output.output import Output
 
 
 class FarmLayoutOutput(Output):
     """
     Plot the farm layout
 
-    Parameters
-    ----------
-    farm : foxes.WindFarm
-        The wind farm
-    farm_results : xarray.Dataset, optional
-        The wind farm calculation results
-    from_results : bool, optional
-        Flag for coordinates from results data
-    results_state : int, optional
-        The state index, for from_res
-    D : float, optional
-        The rotor diameter, if not from data
-
     Attributes
     ----------
-    farm : foxes.WindFarm
+    farm: foxes.WindFarm
         The wind farm
-    fres : xarray.Dataset
+    fres: xarray.Dataset
         The wind farm calculation results
-    from_res : bool
+    from_res: bool
         Flag for coordinates from results data
-    results_state : int
+    results_state: int
         The state index, for from_res
-    D : float
+    D: float
         The rotor diameter, if not from data
 
+    :group: output
+
     """
 
     def __init__(
         self, farm, farm_results=None, from_results=False, results_state=None, D=None
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        farm: foxes.WindFarm
+            The wind farm
+        farm_results: xarray.Dataset, optional
+            The wind farm calculation results
+        from_results: bool, optional
+            Flag for coordinates from results data
+        results_state: int, optional
+            The state index, for from_res
+        D: float, optional
+            The rotor diameter, if not from data
+
+        """
         self.farm = farm
         self.fres = farm_results
         self.from_res = from_results
         self.rstate = results_state
         self.D = D
 
         if from_results and farm_results is None:
@@ -124,47 +130,47 @@
         **kwargs,
     ):
         """
         Creates farm layout figure.
 
         Parameters
         ----------
-        color_by : str, optional
+        color_by: str, optional
             Set scatter color by variable results.
             Use "mean_REWS" etc for means, also
             min, max, sum. All wrt states
-        fontsize : int, optional
+        fontsize: int, optional
             Size of the turbine numbers
-        figsize : tuple, optional
+        figsize: tuple, optional
             The figsize for plt.Figure
-        annotate : int, optional
+        annotate: int, optional
             Turbine index printing, Choices:
             0 = No annotation
             1 = Turbine indices
             2 = Turbine names
-        title : str, optional
+        title: str, optional
             The plot title, or None for automatic
-        fig : matplotlib.pyplot.Figure, optional
+        fig: matplotlib.pyplot.Figure, optional
             The figure object to which to add
-        ax : matplotlib.pyplot.Axis, optional
+        ax: matplotlib.pyplot.Axis, optional
             The axis object, to which to add
-        normalize_D : bool
+        normalize_D: bool
             Normalize x, y wrt rotor diameter
-        ret_im : bool
+        ret_im: bool
             Flag for returned image object
-        bargs : dict
+        bargs: dict
             Arguments for boundary plotting
-        kwargs : dict, optional
+        kwargs: dict, optional
             Parameters forwarded to `matplotlib.pyplot.scatter`
 
         Returns
         -------
-        ax : matplotlib.pyplot.Axis
+        ax: matplotlib.pyplot.Axis
             The axis object
-        im : matplotlib.pyplot.PathCollection, optional
+        im: matplotlib.pyplot.PathCollection, optional
             The image object
 
         """
 
         if fig is None:
             fig = plt.figure(figsize=figsize)
             ax = fig.add_subplot(111)
@@ -270,18 +276,18 @@
         """
         Writes the layout plot to file.
 
         The kwargs are forwarded to self.get_figure
 
         Parameters
         ----------
-        file_path : str
+        file_path: str
             The file into which to plot, or None
             for default
-        fontsize : int
+        fontsize: int
             Size of the turbine numbers
 
         """
 
         ax = self.get_figure(fontsize=fontsize, ret_im=False, **kwargs)
         fig = ax.get_figure()
 
@@ -292,15 +298,15 @@
 
     def write_xyh(self, file_path=None):
         """
         Writes xyh layout file.
 
         Parameters
         ----------
-        file_path : str
+        file_path: str
             The file into which to plot, or None
             for default
 
         """
 
         data = self.get_layout_data()
 
@@ -309,15 +315,15 @@
 
     def write_csv(self, file_path=None):
         """
         Writes csv layout file.
 
         Parameters
         ----------
-        file_path : str
+        file_path: str
             The file into which to plot, or None
             for default
 
         """
 
         data = self.get_layout_data()
 
@@ -338,15 +344,15 @@
 
     def write_json(self, file_path=None):
         """
         Writes xyh layout file.
 
         Parameters
         ----------
-        file_path : str
+        file_path: str
             The file into which to plot, or None
             for default
 
         """
 
         data = self.get_layout_dict()
```

### Comparing `foxes-0.3.5/foxes/output/farm_results_eval.py` & `foxes-0.4.0/foxes/output/farm_results_eval.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,49 +9,55 @@
 class FarmResultsEval(Output):
     """
     Evaluates farm results data.
 
     This sums over turbines and/or states,
     given the state-turbine farm_calc results.
 
-    Parameters
-    ----------
-    farm_results : xarray.Dataset
-        The farm results
-
     Attributes
     ----------
-    results : xarray.Dataset
+    results: xarray.Dataset
         The farm results
 
+    :group: output
+
     """
 
     def __init__(self, farm_results):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        farm_results: xarray.Dataset
+            The farm results
+
+        """
         self.results = farm_results
 
     def weinsum(self, rhs, *vars):
         """
         Calculates Einstein sum, adding weights
         as last argument to the given fields.
 
         It's all about treating NaN values.
 
         Parameters
         ----------
-        rhs : str
+        rhs: str
             The right-hand side of the einsum expression.
             Convention: 's' for states, 't' for turbines
-        vars : tuple of str or np.ndarray
+        vars: tuple of str or np.ndarray
             The variables mentioned in the expression,
             but without the obligatory weights that will
             be added at the end
 
         Returns
         -------
-        result : np.ndarray
+        result: np.ndarray
             The results array
 
         """
         nas = None
         fields = []
         for v in vars:
             if isinstance(v, str):
@@ -83,22 +89,22 @@
 
     def reduce_states(self, vars_op):
         """
         Reduces the states dimension by some operation
 
         Parameters
         ----------
-        vars_op : dict
+        vars_op: dict
             The operation per variable. Key: str, the variable
             name. Value: str, the operation, choices
             are: sum, mean, min, max.
 
         Returns
         -------
-        data : pandas.DataFrame
+        data: pandas.DataFrame
             The results per turbine
 
         """
         n_turbines = self.results.dims[FC.TURBINE]
 
         rdata = {}
         for v, op in vars_op.items():
@@ -128,22 +134,22 @@
 
     def reduce_turbines(self, vars_op):
         """
         Reduces the turbine dimension by some operation
 
         Parameters
         ----------
-        vars_op : dict
+        vars_op: dict
             The operation per variable. Key: str, the variable
             name. Value: str, the operation, choices
             are: sum, mean, min, max.
 
         Returns
         -------
-        data : pandas.DataFrame
+        data: pandas.DataFrame
             The results per state
 
         """
         states = self.results.coords[FC.STATE].to_numpy()
 
         rdata = {}
         for v, op in vars_op.items():
@@ -170,28 +176,28 @@
 
     def reduce_all(self, states_op, turbines_op):
         """
         Reduces states and turbine dimension by some operation
 
         Parameters
         ----------
-        states_op : dict
+        states_op: dict
             The states contraction operations.
             Key: str, the variable name. Value:
             str, the operation, choices are:
             sum, mean, min, max.
-        turbines_op : dict
+        turbines_op: dict
             The turbines contraction operations.
             Key: str, the variable name. Value:
             str, the operation, choices are:
             sum, mean, min, max.
 
         Returns
         -------
-        data : dict
+        data: dict
             The fully contracted results
 
         """
         sdata = self.reduce_states(states_op)
 
         rdata = {}
         for v, op in turbines_op.items():
@@ -220,39 +226,39 @@
 
     def calc_states_mean(self, vars):
         """
         Calculates the mean wrt states.
 
         Parameters
         ----------
-        vars : list of str
+        vars: list of str
             The variables
 
         Returns
         -------
-        data : pandas.DataFrame
+        data: pandas.DataFrame
             The results per turbine
 
         """
         if isinstance(vars, str):
             return self.reduce_states({vars: "mean"})
         return self.reduce_states({v: "mean" for v in vars})
 
     def calc_states_sum(self, vars):
         """
         Calculates the sum wrt states.
 
         Parameters
         ----------
-        vars : list of str
+        vars: list of str
             The variables
 
         Returns
         -------
-        data : pandas.DataFrame
+        data: pandas.DataFrame
             The results per turbine
 
         """
         return self.reduce_states({v: "sum" for v in vars})
 
     def calc_states_std(self, vars):
         """
@@ -269,90 +275,90 @@
 
     def calc_turbine_mean(self, vars):
         """
         Calculates the mean wrt turbines.
 
         Parameters
         ----------
-        vars : list of str
+        vars: list of str
             The variables
 
         Returns
         -------
-        data : pandas.DataFrame
+        data: pandas.DataFrame
             The results per state
 
         """
         return self.reduce_turbines({v: "mean" for v in vars})
 
     def calc_turbine_sum(self, vars):
         """
         Calculates the sum wrt turbines.
 
         Parameters
         ----------
-        vars : list of str
+        vars: list of str
             The variables
 
         Returns
         -------
-        data : pandas.DataFrame
+        data: pandas.DataFrame
             The results per state
 
         """
         return self.reduce_turbines({v: "sum" for v in vars})
 
     def calc_farm_mean(self, vars):
         """
         Calculates the mean over states and turbines.
 
         Parameters
         ----------
-        vars : list of str
+        vars: list of str
             The variables
 
         Returns
         -------
-        data : dict
+        data: dict
             The fully contracted results
 
         """
         op = {v: "mean" for v in vars}
         return self.reduce_all(states_op=op, turbines_op=op)
 
     def calc_farm_sum(self, vars):
         """
         Calculates the sum over states and turbines.
 
         Parameters
         ----------
-        vars : list of str
+        vars: list of str
             The variables
 
         Returns
         -------
-        data : dict
+        data: dict
             The fully contracted results
 
         """
         op = {v: "sum" for v in vars}
         return self.reduce_all(states_op=op, turbines_op=op)
 
     def calc_mean_farm_power(self, ambient=False):
         """
         Calculates the mean total farm power.
 
         Parameters
         ----------
-        ambient : bool
+        ambient: bool
             Flag for ambient power
 
         Returns
         -------
-        data : float
+        data: float
             The mean wind farm power
 
         """
         v = FV.P if not ambient else FV.AMB_P
         cdata = self.reduce_all(states_op={v: "mean"}, turbines_op={v: "sum"})
         return cdata[v]
 
@@ -366,26 +372,26 @@
         P_unit_W=None,
     ):
         """
         Calculates the yield per turbine
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm, optional
+        algo: foxes.core.Algorithm, optional
             The algorithm, for P_nominal lookup
-        annual : bool, optional
+        annual: bool, optional
             Flag for returing annual results, by default False
-        ambient : bool, optional
+        ambient: bool, optional
             Flag for ambient power, by default False
-        hours : int, optional
+        hours: int, optional
             The duration time in hours, if not timeseries states
-        delta_t : np.datetime64, optional
+        delta_t: np.datetime64, optional
             The time delta step in case of time series data,
             by default automatically determined
-        P_unit_W : float
+        P_unit_W: float
             The power unit in Watts, 1000 for kW. Looked up
             in algorithm if not given
 
         Returns
         -------
         pandas.DataFrame
             A dataframe of yield values by turbine in GWh
@@ -437,21 +443,21 @@
 
     def add_capacity(self, algo=None, P_nom=None, ambient=False, verbosity=1):
         """
         Adds capacity to the farm results
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm, optional
+        algo: foxes.core.Algorithm, optional
             The algorithm, for nominal power calculation
-        P_nom : list of float, optional
+        P_nom: list of float, optional
             Nominal power values for each turbine, if algo not given
-        ambient : bool, optional
+        ambient: bool, optional
             Flag for calculating ambient capacity, by default False
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         if ambient:
             var_in = FV.AMB_P
             var_out = FV.AMB_CAP
         else:
@@ -481,30 +487,30 @@
 
     def calc_farm_yield(self, turbine_yield=None, power_uncert=None, **kwargs):
         """
         Calculates yield, P75 and P90 at the farm level
 
         Parameters
         ----------
-        turbine_yield : pandas.DataFrame, optional
+        turbine_yield: pandas.DataFrame, optional
             Yield values by turbine
-        power_uncert : float, optional
+        power_uncert: float, optional
             Uncertainty in the power value. Triggers
             P75 and P90 outputs
-        kwargs : dict, optional
+        kwargs: dict, optional
             Parameters for calc_turbine_yield(). Apply if
             turbine_yield is not given
 
         Returns
         -------
-        farm_yield : float
+        farm_yield: float
             Farm yield result, same unit as turbine yield
-        P75 : float, optional
+        P75: float, optional
             The P75 value, same unit as turbine yield
-        P90 : float, optional
+        P90: float, optional
             The P90 value, same unit as turbine yield
 
         """
         if turbine_yield is None:
             yargs = dict(annual=True)
             yargs.update(kwargs)
             turbine_yield = self.calc_turbine_yield(**yargs)
@@ -519,15 +525,15 @@
 
     def add_efficiency(self, verbosity=1):
         """
         Adds efficiency to the farm results
 
         Parameters
         ----------
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         """
         P = self.results[FV.P]
         P0 = self.results[FV.AMB_P] + 1e-14
         self.results[FV.EFF] = P / P0  # add to farm results
         if verbosity:
@@ -535,14 +541,14 @@
 
     def calc_farm_efficiency(self):
         """
         Calculates farm efficiency
 
         Returns
         -------
-        eff : float
+        eff: float
             The farm efficiency
 
         """
         P = self.calc_mean_farm_power()
         P0 = self.calc_mean_farm_power(ambient=True) + 1e-14
         return P / P0
```

### Comparing `foxes-0.3.5/foxes/output/flow_plots_2d.py` & `foxes-0.4.0/foxes/output/flow_plots_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,31 +8,37 @@
 import foxes.variables as FV
 
 
 class FlowPlots2D(Output):
     """
     Class for horizontal or vertical 2D flow plots
 
-    Parameters
-    ----------
-    algo : foxes.Algorithm
-        The algorithm for point calculation
-    farm_results : xarray.Dataset
-        The farm results
-
     Attributes
     ----------
-    algo : foxes.Algorithm
+    algo: foxes.Algorithm
         The algorithm for point calculation
-    farm_results : xarray.Dataset
+    farm_results: xarray.Dataset
         The farm results
 
+    :group: output
+
     """
 
     def __init__(self, algo, farm_results):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        algo: foxes.Algorithm
+            The algorithm for point calculation
+        farm_results: xarray.Dataset
+            The farm results
+
+        """
         self.algo = algo
         self.fres = farm_results
 
     def _get_fig(
         self,
         var,
         fig,
@@ -159,79 +165,79 @@
         **kwargs,
     ):
         """
         Generates 2D farm flow figure in a horizontal xy-plane.
 
         Parameters
         ----------
-        var : str
+        var: str
             The variable name
-        resolution : float
+        resolution: float
             The resolution in m
-        xmin : float
+        xmin: float
             The min x coordinate, or None for automatic
-        ymin : float
+        ymin: float
             The min y coordinate, or None for automatic
-        xmax : float
+        xmax: float
             The max x coordinate, or None for automatic
-        ymax : float
+        ymax: float
             The max y coordinate, or None for automatic
-        xlabel : str
+        xlabel: str
             The x axis label
-        ylabel : str
+        ylabel: str
             The y axis label
-        z : float
+        z: float
             The z coordinate of the plane
-        xspace : float
+        xspace: float
             The extra space in x direction, before and after wind farm
-        yspace : float
+        yspace: float
             The extra space in y direction, before and after wind farm
-        levels : int
+        levels: int
             The number of levels for the contourf plot, or None for pure image
-        var_min : float
+        var_min: float
             Minimum variable value
-        var_max : float
+        var_max: float
             Maximum variable value
-        figsize : tuple
+        figsize: tuple
             The figsize for plt.Figure
-        normalize_xy : float, optional
+        normalize_xy: float, optional
             Divide x and y by this value
-        normalize_var : float, optional
+        normalize_var: float, optional
             Divide the variable by this value
-        title : str, optional
+        title: str, optional
             The title
-        vlabel : str, optional
+        vlabel: str, optional
             The variable label
-        fig : plt.Figure, optional
+        fig: plt.Figure, optional
             The figure object
-        ax : plt.Axes, optional
+        ax: plt.Axes, optional
             The figure axes
-        add_bar : bool, optional
+        add_bar: bool, optional
             Add a color bar
-        cmap : str, optional
+        cmap: str, optional
             The colormap
-        weight_turbine : int, optional
+        weight_turbine: int, optional
             Index of the turbine from which to take the weight
-        verbosity : int, optional
+        verbosity: int, optional
             The verbosity level
-        ret_state : bool, optional
+        ret_state: bool, optional
             Flag for state index return
-        ret_im : bool, optional
+        ret_im: bool, optional
             Flag for image return
-        kwargs : dict, optional
+        kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
-        fig : matplotlib.Figure
+        fig: matplotlib.Figure
             The figure object
-        si : int, optional
+        si: int, optional
             The state index
-        im : matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
+        im: matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
             The image object
 
         """
 
         # prepare:
         n_states = self.algo.n_states
 
@@ -369,83 +375,83 @@
         **kwargs,
     ):
         """
         Generates 2D farm flow figure in a vertical xz-plane.
 
         Parameters
         ----------
-        var : str
+        var: str
             The variable name
-        resolution : float
+        resolution: float
             The resolution in m
-        x_direction : float
+        x_direction: float
             The direction of the x axis, 0 = north
-        xmin : float
+        xmin: float
             The min x coordinate, or None for automatic
-        zmin : float
+        zmin: float
             The min z coordinate
-        xmax : float
+        xmax: float
             The max x coordinate, or None for automatic
-        zmax : float
+        zmax: float
             The max z coordinate, or None for automatic
-        xlabel : str
+        xlabel: str
             The x axis label
-        zlabel : str
+        zlabel: str
             The z axis label
-        y : float
+        y: float
             The y coordinate of the plane
-        xspace : float
+        xspace: float
             The extra space in x direction, before and after wind farm
-        zspace : float
+        zspace: float
             The extra space in z direction, below and above wind farm
-        levels : int
+        levels: int
             The number of levels for the contourf plot, or None for pure image
-        var_min : float
+        var_min: float
             Minimum variable value
-        var_max : float
+        var_max: float
             Maximum variable value
-        figsize : tuple
+        figsize: tuple
             The figsize for plt.Figure
-        normalize_x : float, optional
+        normalize_x: float, optional
             Divide x by this value
-        normalize_z : float, optional
+        normalize_z: float, optional
             Divide z by this value
-        normalize_var : float, optional
+        normalize_var: float, optional
             Divide the variable by this value
-        title : str, optional
+        title: str, optional
             The title
-        vlabel : str, optional
+        vlabel: str, optional
             The variable label
-        fig : plt.Figure, optional
+        fig: plt.Figure, optional
             The figure object
-        ax : plt.Axes, optional
+        ax: plt.Axes, optional
             The figure axes
-        add_bar : bool, optional
+        add_bar: bool, optional
             Add a color bar
-        cmap : str, optional
+        cmap: str, optional
             The colormap
-        weight_turbine : int, optional
+        weight_turbine: int, optional
             Index of the turbine from which to take the weight
-        verbosity : int, optional
+        verbosity: int, optional
             The verbosity level
-        ret_state : bool, optional
+        ret_state: bool, optional
             Flag for state index return
-        ret_im : bool, optional
+        ret_im: bool, optional
             Flag for image return
-        kwargs : dict, optional
+        kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
-        fig : matplotlib.Figure
+        fig: matplotlib.Figure
             The figure object
-        si : int, optional
+        si: int, optional
             The state index
-        im : matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
+        im: matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
             The image object
 
         """
 
         # prepare:
         n_states = self.algo.n_states
         n_turbines = self.algo.n_turbines
@@ -599,83 +605,83 @@
         **kwargs,
     ):
         """
         Generates 2D farm flow figure in a vertical yz-plane.
 
         Parameters
         ----------
-        var : str
+        var: str
             The variable name
-        resolution : float
+        resolution: float
             The resolution in m
-        x_direction : float
+        x_direction: float
             The direction of the x axis, 0 = north
-        ymin : float
+        ymin: float
             The min y coordinate, or None for automatic
-        zmin : float
+        zmin: float
             The min z coordinate
-        ymax : float
+        ymax: float
             The max y coordinate, or None for automatic
-        zmax : float
+        zmax: float
             The max z coordinate, or None for automatic
-        ylabel : str
+        ylabel: str
             The y axis label
-        zlabel : str
+        zlabel: str
             The z axis label
-        x : float
+        x: float
             The x coordinate of the plane
-        yspace : float
+        yspace: float
             The extra space in y direction, before and after wind farm
-        zspace : float
+        zspace: float
             The extra space in z direction, below and above wind farm
-        levels : int
+        levels: int
             The number of levels for the contourf plot, or None for pure image
-        var_min : float
+        var_min: float
             Minimum variable value
-        var_max : float
+        var_max: float
             Maximum variable value
-        figsize : tuple
+        figsize: tuple
             The figsize for plt.Figure
-        normalize_y : float, optional
+        normalize_y: float, optional
             Divide y by this value
-        normalize_z : float, optional
+        normalize_z: float, optional
             Divide z by this value
-        normalize_var : float, optional
+        normalize_var: float, optional
             Divide the variable by this value
-        title : str, optional
+        title: str, optional
             The title
-        vlabel : str, optional
+        vlabel: str, optional
             The variable label
-        fig : plt.Figure, optional
+        fig: plt.Figure, optional
             The figure object
-        ax : plt.Axes, optional
+        ax: plt.Axes, optional
             The figure axes
-        add_bar : bool, optional
+        add_bar: bool, optional
             Add a color bar
-        cmap : str, optional
+        cmap: str, optional
             The colormap
-        weight_turbine : int, optional
+        weight_turbine: int, optional
             Index of the turbine from which to take the weight
-        verbosity : int, optional
+        verbosity: int, optional
             The verbosity level
-        ret_state : bool, optional
+        ret_state: bool, optional
             Flag for state index return
-        ret_im : bool, optional
+        ret_im: bool, optional
             Flag for image return
-        kwargs : dict, optional
+        kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
-        fig : matplotlib.Figure
+        fig: matplotlib.Figure
             The figure object
-        si : int, optional
+        si: int, optional
             The state index
-        im : matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
+        im: matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
             The image object
 
         """
 
         # prepare:
         n_states = self.algo.n_states
         n_turbines = self.algo.n_turbines
@@ -826,81 +832,81 @@
         **kwargs,
     ):
         """
         Generates 2D farm flow figure in a horizontal xy-plane.
 
         Parameters
         ----------
-        var : str
+        var: str
             The variable name
-        resolution : float
+        resolution: float
             The resolution in m
-        xmin : float
+        xmin: float
             The min x coordinate, or None for automatic
-        ymin : float
+        ymin: float
             The min y coordinate, or None for automatic
-        xmax : float
+        xmax: float
             The max x coordinate, or None for automatic
-        ymax : float
+        ymax: float
             The max y coordinate, or None for automatic
-        xlabel : str
+        xlabel: str
             The x axis label
-        ylabel : str
+        ylabel: str
             The y axis label
-        z : float
+        z: float
             The z coordinate of the plane
-        xspace : float
+        xspace: float
             The extra space in x direction, before and after wind farm
-        yspace : float
+        yspace: float
             The extra space in y direction, before and after wind farm
-        levels : int
+        levels: int
             The number of levels for the contourf plot, or None for pure image
-        var_min : float
+        var_min: float
             Minimum variable value
-        var_max : float
+        var_max: float
             Maximum variable value
-        figsize : tuple
+        figsize: tuple
             The figsize for plt.Figure
-        normalize_xy : float, optional
+        normalize_xy: float, optional
             Divide x and y by this value
-        normalize_var : float, optional
+        normalize_var: float, optional
             Divide the variable by this value
-        title : str, optional
+        title: str, optional
             The title
-        vlabel : str, optional
+        vlabel: str, optional
             The variable label
-        fig : plt.Figure, optional
+        fig: plt.Figure, optional
             The figure object
-        ax : plt.Axes, optional
+        ax: plt.Axes, optional
             The figure axes
-        add_bar : bool, optional
+        add_bar: bool, optional
             Add a color bar
-        cmap : str, optional
+        cmap: str, optional
             The colormap
-        quiver_n : int, optional
+        quiver_n: int, optional
             Place a vector at each `n`th point
-        quiver_pars : dict, optional
+        quiver_pars: dict, optional
             Parameters for plt.quiver
-        verbosity : int, optional
+        verbosity: int, optional
             The verbosity level
-        ret_state : bool, optional
+        ret_state: bool, optional
             Flag for state index return
-        ret_im : bool, optional
+        ret_im: bool, optional
             Flag for image return
-        kwargs : dict, optional
+        kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
-        fig : matplotlib.Figure
+        fig: matplotlib.Figure
             The figure object
-        si : int, optional
+        si: int, optional
             The state index
-        im : matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
+        im: matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
             The image object
 
         """
 
         # prepare:
         n_states = self.algo.n_states
 
@@ -1047,85 +1053,85 @@
         **kwargs,
     ):
         """
         Generates 2D farm flow figure in a vertical xz-plane.
 
         Parameters
         ----------
-        var : str
+        var: str
             The variable name
-        resolution : float
+        resolution: float
             The resolution in m
-        x_direction : float
+        x_direction: float
             The direction of the x axis, 0 = north
-        xmin : float
+        xmin: float
             The min x coordinate, or None for automatic
-        zmin : float
+        zmin: float
             The min z coordinate
-        xmax : float
+        xmax: float
             The max x coordinate, or None for automatic
-        zmax : float
+        zmax: float
             The max z coordinate, or None for automatic
-        xlabel : str
+        xlabel: str
             The x axis label
-        zlabel : str
+        zlabel: str
             The z axis label
-        y : float
+        y: float
             The y coordinate of the plane
-        xspace : float
+        xspace: float
             The extra space in x direction, before and after wind farm
-        zspace : float
+        zspace: float
             The extra space in z direction, below and above wind farm
-        levels : int
+        levels: int
             The number of levels for the contourf plot, or None for pure image
-        var_min : float
+        var_min: float
             Minimum variable value
-        var_max : float
+        var_max: float
             Maximum variable value
-        figsize : tuple
+        figsize: tuple
             The figsize for plt.Figure
-        normalize_x : float, optional
+        normalize_x: float, optional
             Divide x by this value
-        normalize_z : float, optional
+        normalize_z: float, optional
             Divide z by this value
-        normalize_var : float, optional
+        normalize_var: float, optional
             Divide the variable by this value
-        title : str, optional
+        title: str, optional
             The title
-        vlabel : str, optional
+        vlabel: str, optional
             The variable label
-        fig : plt.Figure, optional
+        fig: plt.Figure, optional
             The figure object
-        ax : plt.Axes, optional
+        ax: plt.Axes, optional
             The figure axes
-        add_bar : bool, optional
+        add_bar: bool, optional
             Add a color bar
-        cmap : str, optional
+        cmap: str, optional
             The colormap
-        quiver_n : int, optional
+        quiver_n: int, optional
             Place a vector at ech `n`th point
-        quiver_pars : dict, optional
+        quiver_pars: dict, optional
             Parameters for plt.quiver
-        verbosity : int, optional
+        verbosity: int, optional
             The verbosity level
-        ret_state : bool, optional
+        ret_state: bool, optional
             Flag for state index return
-        ret_im : bool, optional
+        ret_im: bool, optional
             Flag for image return
-        kwargs : dict, optional
+        kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
-        fig : matplotlib.Figure
+        fig: matplotlib.Figure
             The figure object
-        si : int, optional
+        si: int, optional
             The state index
-        im : matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
+        im: matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
             The image object
 
         """
 
         # prepare:
         n_states = self.algo.n_states
         n_turbines = self.algo.n_turbines
@@ -1289,85 +1295,85 @@
         **kwargs,
     ):
         """
         Generates 2D farm flow figure in a plane.
 
         Parameters
         ----------
-        var : str
+        var: str
             The variable name
-        resolution : float
+        resolution: float
             The resolution in m
-        x_direction : float
+        x_direction: float
             The direction of the x axis, 0 = north
-        ymin : float
+        ymin: float
             The min y coordinate, or None for automatic
-        zmin : float
+        zmin: float
             The min z coordinate
-        ymax : float
+        ymax: float
             The max y coordinate, or None for automatic
-        zmax : float
+        zmax: float
             The max z coordinate, or None for automatic
-        ylabel : str
+        ylabel: str
             The y axis label
-        zlabel : str
+        zlabel: str
             The z axis label
-        x : float
+        x: float
             The x coordinate of the plane
-        yspace : float
+        yspace: float
             The extra space in y direction, left and right of wind farm
-        zspace : float
+        zspace: float
             The extra space in z direction, below and above wind farm
-        levels : int
+        levels: int
             The number of levels for the contourf plot, or None for pure image
-        var_min : float
+        var_min: float
             Minimum variable value
-        var_max : float
+        var_max: float
             Maximum variable value
-        figsize : tuple
+        figsize: tuple
             The figsize for plt.Figure
-        normalize_y : float, optional
+        normalize_y: float, optional
             Divide y by this value
-        normalize_z : float, optional
+        normalize_z: float, optional
             Divide z by this value
-        normalize_var : float, optional
+        normalize_var: float, optional
             Divide the variable by this value
-        title : str, optional
+        title: str, optional
             The title
-        vlabel : str, optional
+        vlabel: str, optional
             The variable label
-        fig : plt.Figure, optional
+        fig: plt.Figure, optional
             The figure object
-        ax : plt.Axes, optional
+        ax: plt.Axes, optional
             The figure axes
-        add_bar : bool, optional
+        add_bar: bool, optional
             Add a color bar
-        cmap : str, optional
+        cmap: str, optional
             The colormap
-        quiver_n : int, optional
+        quiver_n: int, optional
             Place a vector at ech `n`th point
-        quiver_pars : dict, optional
+        quiver_pars: dict, optional
             Parameters for plt.quiver
-        verbosity : int, optional
+        verbosity: int, optional
             The verbosity level
-        ret_state : bool, optional
+        ret_state: bool, optional
             Flag for state index return
-        ret_im : bool, optional
+        ret_im: bool, optional
             Flag for image return
-        kwargs : dict, optional
+        kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
-        fig : matplotlib.Figure
+        fig: matplotlib.Figure
             The figure object
-        si : int, optional
+        si: int, optional
             The state index
-        im : matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
+        im: matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
             The image object
 
         """
 
         # prepare:
         n_states = self.algo.n_states
         n_turbines = self.algo.n_turbines
```

### Comparing `foxes-0.3.5/foxes/output/output.py` & `foxes-0.4.0/foxes/output/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,33 +4,35 @@
 class Output:
     """
     Base class for foxes output.
 
     The job of this class is to provide handy
     helper functions.
 
+    :group: output
+
     """
 
     @classmethod
     def write(cls, file_path, data, format_col2var={}, format_dict={}, **kwargs):
         """
         Writes data to file via pandas.
 
         The kwargs are forwarded to the underlying pandas writing function.
 
         Parameters
         ----------
-        file_path : string
+        file_path: string
             The path to the output file
-        data : pandas.DataFrame
+        data: pandas.DataFrame
             The data
-        format_col2var : dict
+        format_col2var: dict
             Mapping from column names to flappy variables,
             for formatting
-        format_dict : dict
+        format_dict: dict
             Dictionary with format entries for columns, e.g.
             {FV.P: '{:.4f}'}. Note that the keys are flappy variables
 
         """
         fdict = {}
         for c in data.columns:
             v = format_col2var.get(c, c)
@@ -53,15 +55,15 @@
     @classmethod
     def new(cls, model_type, **kwargs):
         """
         Run-time output model factory.
 
         Parameters
         ----------
-        model_type : string
+        model_type: string
             The selected derived class name
 
         """
 
         if model_type is None:
             return None
```

### Comparing `foxes-0.3.5/foxes/output/results_writer.py` & `foxes-0.4.0/foxes/output/results_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,35 @@
 import foxes.constants as FC
 
 
 class ResultsWriter(Output):
     """
     Writes results farm data to file.
 
-    Parameters
-    ----------
-    farm_results : xarray.Dataset, optional
-        The farm results, if data is None
-    data : pandas.DataFrame, optional
-        The data, if farm_results is None
-
     Attributes
     ----------
-    data : pandas.DataFrame
+    data: pandas.DataFrame
         The farm results
 
+    :group: output
+
     """
 
     def __init__(self, farm_results=None, data=None):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        farm_results: xarray.Dataset, optional
+            The farm results, if data is None
+        data: pandas.DataFrame, optional
+            The data, if farm_results is None
+
+        """
         if farm_results is not None and data is None:
             self.data = farm_results.to_dataframe().reset_index()
             self.data[FC.TNAME] = farm_results[FC.TNAME].to_numpy()[
                 self.data[FC.TURBINE]
             ]
             self.data.set_index([FC.STATE, FC.TURBINE], inplace=True)
         elif farm_results is None and data is not None:
@@ -43,26 +49,26 @@
         **kwargs,
     ):
         """
         Writes a csv file
 
         Parameters
         ----------
-        file_path : str
+        file_path: str
             Path the the csv file
-        variables : dict or list of str, optional
+        variables: dict or list of str, optional
             The variables to be written. If a dict, then
             the keys are the foxes variables and the values
             the column names. If None, then all data will be
             written.
-        turbine_names : bool
+        turbine_names: bool
             Use turbine names instead of turbine indices
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
-        kwargs : dict, optional
+        kwargs: dict, optional
             Additional parameters for Output.write()
 
         """
         if verbosity:
             print(f"ResultsWriter: Writing file '{file_path}'")
 
         if variables is None:
```

### Comparing `foxes-0.3.5/foxes/output/rose_plot.py` & `foxes-0.4.0/foxes/output/rose_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,33 @@
 from .output import Output
 
 
 class RosePlotOutput(Output):
     """
     Class for rose plot creation
 
-    Parameters
-    ----------
-    results : xarray.Dataset
-        The calculation results (farm or points)
-
     Attributes
     ----------
-    results : pandas.DataFrame
+    results: pandas.DataFrame
         The calculation results (farm or points)
 
+    :group: output
+
     """
 
     def __init__(self, results):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        results: xarray.Dataset
+            The calculation results (farm or points)
+
+        """
         dims = list(results.dims.keys())
         if dims[1] == FC.TURBINE:
             self._rtype = FC.TURBINE
         elif dims[1] == FC.POINT:
             self._rtype = FC.POINT
         else:
             raise KeyError(
@@ -43,22 +49,22 @@
     @classmethod
     def get_data_info(cls, dname):
         """
         Returns default description for a variable.
 
         Parameters
         ----------
-        dname : str
+        dname: str
             The variable name
 
         Returns
         -------
-        title : str
+        title: str
             The long name of the variable
-        legend : str
+        legend: str
             The legend/axis text
 
         """
 
         if dname == FV.D:
             return "Rotor diameter", f"{FV.D} [m]"
         if dname == FV.H:
@@ -104,31 +110,31 @@
         legend=None,
     ):
         """
         Get pandas DataFrame with wind rose data.
 
         Parameters
         ----------
-        sectors : int
+        sectors: int
             The number of wind direction sectors
-        var : str
+        var: str
             The data variable name
-        var_bins : list of float
+        var_bins: list of float
             The variable bin seperation values
-        wd_var : str, optional
+        wd_var: str, optional
             The wind direction variable name
-        turbine : int, optional
+        turbine: int, optional
             Only relevant in case of farm results.
             If None, mean over all turbines.
             Else, data from a single turbine
-        point : int, optional
+        point: int, optional
             Only relevant in case of point results.
             If None, mean over all points.
             Else, data from a single point
-        legend : str, optional
+        legend: str, optional
             The data legend string
 
         Returns
         -------
         pd.DataFrame :
             The wind rose data
 
@@ -183,35 +189,35 @@
         title_dict={},
     ):
         """
         Creates px figure object
 
         Parameters
         ----------
-        sectors : int
+        sectors: int
             The number of wind direction sectors
-        var : str
+        var: str
             The data variable name
-        var_bins : list of float
+        var_bins: list of float
             The variable bin seperation values
-        wd_var : str, optional
+        wd_var: str, optional
             The wind direction variable name
-        turbine : int, optional
+        turbine: int, optional
             Only relevant in case of farm results.
             If None, mean over all turbines.
             Else, data from a single turbine
-        point : int, optional
+        point: int, optional
             Only relevant in case of point results.
             If None, mean over all points.
             Else, data from a single point
-        legend : str, optional
+        legend: str, optional
             The data legend string
-        layout_dict : dict, optional
+        layout_dict: dict, optional
             Optional parameters for the px figure layout
-        title_dict : dict, optional
+        title_dict: dict, optional
             Optional parameters for the px title layout
 
         Returns
         -------
         px.Figure :
             The rose plot figure
 
@@ -268,37 +274,37 @@
         title_dict={},
     ):
         """
         Write rose plot to file
 
         Parameters
         ----------
-        file_name : str
+        file_name: str
             Path to the output file
-        sectors : int
+        sectors: int
             The number of wind direction sectors
-        var : str
+        var: str
             The data variable name
-        var_bins : list of float
+        var_bins: list of float
             The variable bin seperation values
-        wd_var : str, optional
+        wd_var: str, optional
             The wind direction variable name
-        turbine : int, optional
+        turbine: int, optional
             Only relevant in case of farm results.
             If None, mean over all turbines.
             Else, data from a single turbine
-        point : int, optional
+        point: int, optional
             Only relevant in case of point results.
             If None, mean over all points.
             Else, data from a single point
-        legend : str, optional
+        legend: str, optional
             The data legend string
-        layout_dict : dict, optional
+        layout_dict: dict, optional
             Optional parameters for the px figure layout
-        title_dict : dict, optional
+        title_dict: dict, optional
             Optional parameters for the px title layout
 
         """
 
         fig = self.get_figure(
             sectors=sectors,
             var=var,
@@ -318,21 +324,23 @@
 
 class StatesRosePlotOutput(RosePlotOutput):
     """
     Class for rose plot creation directly from states
 
     Parameters
     ----------
-    states : foxes.core.States
+    states: foxes.core.States
         The states from which to compute the wind rose
-    point : numpy.ndarray
+    point: numpy.ndarray
         The evaluation point, shape: (3,)
-    mbook : foxes.models.ModelBook, optional
+    mbook: foxes.models.ModelBook, optional
         The model book
 
+    :group: output
+
     """
 
     def __init__(self, states, point, mbook=None, ws_var=FV.AMB_REWS):
         farm = WindFarm()
         farm.add_turbine(
             Turbine(
                 xy=point[:2],
```

### Comparing `foxes-0.3.5/foxes/output/state_turbine_map.py` & `foxes-0.4.0/foxes/output/state_turbine_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,33 @@
 
 
 class StateTurbineMap(Output):
     """
     Creates heat maps with turbines on the one
     and states on the other axis.
 
-    Parameters
-    ----------
-    farm_results : xarray.Dataset
-        The farm results
-
     Attributes
     ----------
-    results : xarray.Dataset
+    results: xarray.Dataset
         The farm results
+    
+    :group: output
 
     """
 
     def __init__(self, farm_results):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        farm_results: xarray.Dataset
+            The farm results
+
+        """
         self.results = farm_results
 
     def plot_map(
         self,
         variable,
         title=None,
         ax=None,
@@ -34,29 +40,29 @@
         **kwargs,
     ):
         """
         Plot the heat map for the selected variable.
 
         Parameters
         ----------
-        variable : str
+        variable: str
             The variable to plot
-        title : str, optional
+        title: str, optional
             The plot title
-        ax : pyplot.Axis, optional
+        ax: pyplot.Axis, optional
             The axis
-        figsize : tuple
+        figsize: tuple
             The figsize argument for plt.subplots()
             in case ax is not provided
-        kwargs : dict, optional
+        kwargs: dict, optional
             Additional parameters for plt.pcolormesh()
 
         Returns
         -------
-        ax : pyplot.Axis
+        ax: pyplot.Axis
             The plot axis
 
         """
         turbines = self.results[FC.TURBINE].to_numpy()
         states = self.results[FC.STATE].to_numpy()
 
         if ax is None:
```

### Comparing `foxes-0.3.5/foxes/output/turbine_type_curves.py` & `foxes-0.4.0/foxes/output/turbine_type_curves.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,27 +13,33 @@
 
 
 class TurbineTypeCurves(Output):
     """
     Creates power and ct curves for turbine
     types, optionally including derating/boost.
 
-    Parameters
-    ----------
-    mbook : foxes.models.ModelBook
-        The model book
-
     Attributes
     ----------
-    mbook : foxes.models.ModelBook
+    mbook: foxes.models.ModelBook
         The model book
+    
+    :group: output
 
     """
 
     def __init__(self, mbook):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        mbook: foxes.models.ModelBook
+            The model book
+
+        """
         self.mbook = mbook
 
     def plot_curves(
         self,
         turbine_type,
         variables,
         P_max=None,
@@ -51,51 +57,51 @@
         **kwargs,
     ):
         """
         Plot the power or ct curve.
 
         Parameters
         ----------
-        turbine_type : str
+        turbine_type: str
             The turbine type name from the
             model book
-        variables : str or list of str
+        variables: str or list of str
             For example FV.P or FV.CT
-        P_max : float, optional
+        P_max: float, optional
             The power mask value, if of interest
-        titles : list of str, optional
+        titles: list of str, optional
             The plot titles, one for each variable
-        x_label : str, optional
+        x_label: str, optional
             The x axis label
-        y_labels : list of str, optional
+        y_labels: list of str, optional
             The y axis lables, one for each variable
-        ws_min : float
+        ws_min: float
             The minimal wind speed
-        ws_max : float
+        ws_max: float
             The maximal wind speed
-        ws_step : float
+        ws_step: float
             The wind speed step size
-        ti : float
+        ti: float
             The TI value
-        rho : float
+        rho: float
             The air density value
-        axs : list of pyplot.Axis, optional
+        axs: list of pyplot.Axis, optional
             The axis, one for each variable
-        figsize : tuple
+        figsize: tuple
             The figsize argument for plt.subplots()
             in case ax is not provided
-        pmax_args : dict, optional
+        pmax_args: dict, optional
             Additionals parameters for plt.plot()
             for power mask case
-        kwargs : dict, optional
+        kwargs: dict, optional
             Additional parameters for plt.plot()
 
         Returns
         -------
-        axs : list of pyplot.Axis
+        axs: list of pyplot.Axis
             The plot axes, one for each variable
 
         """
         vars = [variables] if isinstance(variables, str) else variables
         if isinstance(titles, str):
             titles = [titles]
         elif titles is None:
```

### Comparing `foxes-0.3.5/foxes/utils/abl/neutral.py` & `foxes-0.4.0/foxes/utils/abl/stable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,105 @@
 import numpy as np
+from .neutral import logz as lgz
 
 
 def logz(height, z0):
     """
     Calculates the log factor for
     wind speed profiles.
 
     Parameters
     ----------
-    height : float
+    height: float
         The evaluation height
-    z0 : float
+    z0: float
         The roughness length
 
     Returns
     -------
-    lz : float
+    lz: float
         The log factor
+    
+    :group: utils.abl.stable
 
     """
-    h = np.maximum(height, z0)
-    return np.log(h / z0)
+    return lgz(height, z0)
 
 
-def ustar(ws_ref, h_ref, z0, kappa=0.41):
+def psi(height, mol):
+    """
+    The Psi function
+
+    Parameters
+    ----------
+    height: float
+        The height value
+    mol: float
+        The Monin-Obukhov height
+
+    Returns
+    -------
+    psi: float
+        The Psi function value
+
+    :group: utils.abl.stable
+
+    """
+    h = np.minimum(height, np.abs(mol))
+    return -5.0 * h / mol
+
+
+def ustar(ws_ref, h_ref, z0, mol, kappa=0.41):
     """
     Calculates the friction velocity,
     based on reference data.
 
     Parameters
     ----------
-    ws_ref : float
+    ws_ref: float
         The reference wind speed
-    h_ref : float
+    h_ref: float
         The reference height
-    z0 : float
+    z0: float
         The roughness length
-    kappa : float
+    mol: float
+        The Monin-Obukhov height
+    kappa: float
         The van-Karman constant
 
     Returns
     -------
-    ustar : float
+    ustar: float
         The friction velocity
 
+    :group: utils.abl.stable
+
     """
-    lz = logz(h_ref, z0)
-    return ws_ref * kappa / lz
+    return ws_ref * kappa / (logz(h_ref, z0) - psi(h_ref, mol))
 
 
-def calc_ws(height, z0, ustar, kappa=0.41):
+def calc_ws(height, z0, ustar, psi, kappa=0.41):
     """
     Calculate wind speeds at given height
 
     Parameters
     ----------
-    height : float
+    height: float
         The evaluation height
-    z0 : float
+    z0: float
         The roughness length
-    ustar : float
+    ustar: float
         The friction velocity
-    kappa : float
+    psi: float
+        The Psi function values
+    kappa: float
         The van-Karman constant
 
     Returns
     -------
-    ws : float
+    ws: float
         The wind speed
 
+    :group: utils.abl.stable
+
     """
-    return ustar / kappa * logz(height, z0)
+    return ustar / kappa * (logz(height, z0) - psi)
```

### Comparing `foxes-0.3.5/foxes/utils/abl/stable.py` & `foxes-0.4.0/foxes/models/vertical_profiles/uniform.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,64 @@
 import numpy as np
-from .neutral import logz as lgz
 
-
-def logz(height, z0):
-    """
-    Calculates the log factor for
-    wind speed profiles.
-
-    Parameters
-    ----------
-    height : float
-        The evaluation height
-    z0 : float
-        The roughness length
-
-    Returns
-    -------
-    lz : float
-        The log factor
-
-    """
-    return lgz(height, z0)
-
-
-def psi(height, mol):
-    """
-    The Psi function
-
-    Parameters
-    ----------
-    height : float
-        The height value
-    mol : float
-        The Monin-Obukhov height
-
-    Returns
-    -------
-    psi : float
-        The Psi function value
-
-    """
-    h = np.minimum(height, np.abs(mol))
-    return -5.0 * h / mol
+from foxes.core import VerticalProfile
 
 
-def ustar(ws_ref, h_ref, z0, mol, kappa=0.41):
+class UniformProfile(VerticalProfile):
     """
-    Calculates the friction velocity,
-    based on reference data.
+    A profile with uniform values.
 
-    Parameters
+    Attributes
     ----------
-    ws_ref : float
-        The reference wind speed
-    h_ref : float
-        The reference height
-    z0 : float
-        The roughness length
-    mol : float
-        The Monin-Obukhov height
-    kappa : float
-        The van-Karman constant
-
-    Returns
-    -------
-    ustar : float
-        The friction velocity
-
-    """
-    return ws_ref * kappa / (logz(h_ref, z0) - psi(h_ref, mol))
-
-
-def calc_ws(height, z0, ustar, psi, kappa=0.41):
-    """
-    Calculate wind speeds at given height
-
-    Parameters
-    ----------
-    height : float
-        The evaluation height
-    z0 : float
-        The roughness length
-    ustar : float
-        The friction velocity
-    psi : float
-        The Psi function values
-    kappa : float
-        The van-Karman constant
-
-    Returns
-    -------
-    ws : float
-        The wind speed
-
-    """
-    return ustar / kappa * (logz(height, z0) - psi)
+    var: float
+        The value
+    
+    :group: models.vertical_profiles
+
+    """
+    def __init__(self, variable):
+        """
+        Constructor
+        
+        Parameters
+        ----------
+        variable: float
+            The value
+
+        """
+        super().__init__(self)
+        self.var = variable
+
+    def input_vars(self):
+        """
+        The input variables needed for the profile
+        calculation.
+
+        Returns
+        -------
+        vars: list of str
+            The variable names
+
+        """
+        return [self.var]
+
+    def calculate(self, data, heights):
+        """
+        Run the profile calculation.
+
+        Parameters
+        ----------
+        data: dict
+            The input data
+        heights: numpy.ndarray
+            The evaluation heights
+
+        Returns
+        -------
+        results: numpy.ndarray
+            The profile results, same
+            shape as heights
+
+        """
+        out = np.zeros_like(heights)
+        out[:] = data[self.var]
+        return out
```

### Comparing `foxes-0.3.5/foxes/utils/abl/unstable.py` & `foxes-0.4.0/foxes/utils/abl/neutral.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,79 @@
 import numpy as np
 
-from .stable import logz
 
-
-def psi(height, mol):
+def logz(height, z0):
     """
-    The Psi function
+    Calculates the log factor for
+    wind speed profiles.
 
     Parameters
     ----------
-    height : float
-        The height value
-    mol : float
-        The Monin-Obukhov height
+    height: float
+        The evaluation height
+    z0: float
+        The roughness length
 
     Returns
     -------
-    psi : float
-        The Psi function value
+    lz: float
+        The log factor
+    
+    :group: utils.abl.neutral
 
     """
-    x = (1.0 - 16.0 * height / mol) ** 0.25
-    return (
-        2.0 * np.log((1.0 + x) / 2.0)
-        + np.log((1.0 + x**2) / 2.0)
-        - 2.0 * np.arctan(x)
-        + np.pi / 2.0
-    )
+    h = np.maximum(height, z0)
+    return np.log(h / z0)
 
 
-def ustar(ws_ref, h_ref, z0, mol, kappa=0.41):
+def ustar(ws_ref, h_ref, z0, kappa=0.41):
     """
     Calculates the friction velocity,
     based on reference data.
 
     Parameters
     ----------
-    ws_ref : float
+    ws_ref: float
         The reference wind speed
-    h_ref : float
+    h_ref: float
         The reference height
-    z0 : float
+    z0: float
         The roughness length
-    mol : float
-        The Monin-Obukhov height
-    kappa : float
+    kappa: float
         The van-Karman constant
 
     Returns
     -------
-    ustar : float
+    ustar: float
         The friction velocity
+    
+    :group: utils.abl.neutral
 
     """
-    return ws_ref * kappa / (logz(h_ref, z0) - psi(h_ref, mol))
+    lz = logz(h_ref, z0)
+    return ws_ref * kappa / lz
 
 
-def calc_ws(height, z0, ustar, psi, kappa=0.41):
+def calc_ws(height, z0, ustar, kappa=0.41):
     """
     Calculate wind speeds at given height
 
     Parameters
     ----------
-    height : float
+    height: float
         The evaluation height
-    z0 : float
+    z0: float
         The roughness length
-    ustar : float
+    ustar: float
         The friction velocity
-    psi : float
-        The Psi function values
-    kappa : float
+    kappa: float
         The van-Karman constant
 
     Returns
     -------
-    ws : float
+    ws: float
         The wind speed
+    
+    :group: utils.abl.neutral
 
     """
-    return ustar / kappa * (logz(height, z0) - psi)
+    return ustar / kappa * logz(height, z0)
```

### Comparing `foxes-0.3.5/foxes/utils/cubic_roots.py` & `foxes-0.4.0/foxes/utils/cubic_roots.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,31 @@
     this works fast for an array of polynomials,
     so you spare yourself looping over them.
 
     Source: https://github.com/opencv/opencv/blob/master/modules/calib3d/src/polynom_solver.cpp
 
     Parameters
     ----------
-    a0 : numpy.ndarray
+    a0: numpy.ndarray
         The coefficients a[0]
-    a1 : numpy.ndarray
+    a1: numpy.ndarray
         The coefficients a[1]
-    a2 : numpy.ndarray
+    a2: numpy.ndarray
         The coefficients a[2]
-    a3 : numpy.ndarray
+    a3: numpy.ndarray
         The coefficients a[3], or None for ones
 
     Returns
     -------
-    roots : numpy.ndarray
+    roots: numpy.ndarray
         The real roots of the polynomial,
         shape: (n_a0, 3). If one root only
         the two last columns will be np.nan
 
+    :group: utils
 
     """
 
     N = len(a0)
     out = np.full([N, 3], np.nan)
 
     # Calculate the normalized form x^3 + a2 * x^2 + a1 * x + a0 = 0
```

### Comparing `foxes-0.3.5/foxes/utils/data_book.py` & `foxes-0.4.0/foxes/utils/data_book.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,43 +6,54 @@
 class DataBook:
     """
     Container class for file paths, either directly
     given or as static data within a package.
 
     Parameters
     ----------
-    data_book : DataBook, optional
+    data_book: DataBook, optional
         A data book to start from
 
     Attributes
     ----------
-    dbase : dict
+    dbase: dict
         The data base. Key: context str,
         value: dict (file name str to pathlib.Path)
+    
+    :group: utils
 
     """
 
     def __init__(self, data_book=None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        data_book: DataBook, optional
+            A data book to start from
+
+        """
         self.dbase = {}
         if data_book is not None:
             for c, d in data_book.items():
                 self.dbase[c] = {}
                 self.dbase[c].update(d)
 
     def add_data_package(self, context, package, file_sfx):
         """
         Add static files from a package location.
 
         Parameters
         ----------
-        context : str
+        context: str
             The context
-        package : str or package
+        package: str or package
             The package, must contain init file
-        file_sfx : list of str
+        file_sfx: list of str
             File endings to include
 
         """
         if context not in self.dbase:
             self.dbase[context] = {}
 
         if isinstance(file_sfx, str):
@@ -71,19 +82,19 @@
 
     def add_data_package_file(self, context, package, file_name):
         """
         Add a static file from a package location.
 
         Parameters
         ----------
-        context : str
+        context: str
             The context
-        package : str or package
+        package: str or package
             The package, must contain init.py` file
-        file_mane : str
+        file_mane: str
             The file name
 
         """
         if context not in self.dbase:
             self.dbase[context] = {}
 
         try:
@@ -96,17 +107,17 @@
 
     def add_files(self, context, file_paths):
         """
         Add file paths
 
         Parameters
         ----------
-        context : str
+        context: str
             The context
-        file_paths : list of str
+        file_paths: list of str
             The file paths
 
         """
 
         if context not in self.dbase:
             self.dbase[context] = {}
 
@@ -120,42 +131,42 @@
 
     def add_file(self, context, file_path):
         """
         Add a file path
 
         Parameters
         ----------
-        context : str
+        context: str
             The context
-        file_path : str
+        file_path: str
             The file path
 
         """
         self.add_files(context, [file_path])
 
     def get_file_path(self, context, file_name, check_raw=True, errors=True):
         """
         Get path of a file
 
         Parameters
         ----------
-        context : str
+        context: str
             The context
-        file_name : str
+        file_name: str
             The file name
-        check_raw : bool
+        check_raw: bool
             Check if `file_name` exists as given, and in
             that case return the path
-        errors : bool
+        errors: bool
             Flag for raising KeyError, otherwise return None,
             if context of file_name not found
 
         Returns
         -------
-        path : pathlib.Path
+        path: pathlib.Path
             The path
 
         """
 
         if check_raw:
             path = Path(file_name)
             if path.is_file():
@@ -183,17 +194,17 @@
 
     def toc(self, context):
         """
         Get list of contents
 
         Parameters
         ----------
-        context : str
+        context: str
             The context
 
         Returns
         -------
-        keys : list of str
+        keys: list of str
             The data keys
 
         """
         return sorted(list(self.dbase[context].keys()))
```

### Comparing `foxes-0.3.5/foxes/utils/geom2d/area_geometry.py` & `foxes-0.4.0/foxes/utils/geom2d/area_geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,79 +4,81 @@
 from matplotlib.colors import ListedColormap
 
 
 class AreaGeometry(metaclass=ABCMeta):
     """
     Abstract base class for closed 2D geometries.
 
+    :group: utils.geom2d
+
     """
 
     @abstractmethod
     def p_min(self):
         """
         Returns minimal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The minimal (x,y) point, shape = (2,)
 
         """
         pass
 
     @abstractmethod
     def p_max(self):
         """
         Returns maximal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The maximal (x,y) point, shape = (2,)
 
         """
         pass
 
     @abstractmethod
     def points_distance(self, points, return_nearest=False):
         """
         Calculates point distances wrt boundary.
 
         Parameters
         ----------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The probe points, shape (n_points, 2)
-        return_nearest : bool
+        return_nearest: bool
             Flag for return of the nearest point on bundary
 
         Returns
         -------
-        dist : numpy.ndarray
+        dist: numpy.ndarray
             The smallest distances to the boundary,
             shape: (n_points,)
-        p_nearest : numpy.ndarray, optional
+        p_nearest: numpy.ndarray, optional
             The nearest points on the boundary, if
             return_nearest is True, shape: (n_points, 2)
 
         """
         pass
 
     @abstractmethod
     def points_inside(self, points):
         """
         Tests if points are inside the geometry.
 
         Parameters
         ----------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The probe points, shape (n_points, 2)
 
         Returns
         -------
-        inside : numpy.ndarray
+        inside: numpy.ndarray
             True if point is inside, shape: (n_points,)
 
         """
         pass
 
     def add_to_figure(
         self,
@@ -87,25 +89,25 @@
         pars_distance={},
     ):
         """
         Add image to (x,y) figure.
 
         Parameters
         ----------
-        ax : matplotlib.pyplot.Axis
+        ax: matplotlib.pyplot.Axis
             The axis object
-        show_boundary : bool
+        show_boundary: bool
             Add the boundary line to the image
-        fill_mode : str, optional
+        fill_mode: str, optional
             Fill the area. Options:
             dist, dist_inside, dist_outside, inside_<color>,
             outside_<color>
-        pars_boundary : dict
+        pars_boundary: dict
             Parameters for boundary plotting command
-        pars_distance : dict
+        pars_distance: dict
             Parameters for distance plotting command
 
         """
         if fill_mode is not None:
             if "Nx" in pars_distance or "Ny" in pars_distance:
                 Nx = pars_distance.pop("Nx")
                 Ny = pars_distance.pop("Ny")
@@ -192,15 +194,15 @@
 
     def inverse(self):
         """
         Get the inverted geometry
 
         Returns
         -------
-        inverted : foxes.utils.geom2d.InvertedAreaGeometry
+        inverted: foxes.utils.geom2d.InvertedAreaGeometry
             The inverted geometry
 
         """
         return InvertedAreaGeometry(self)
 
     def __add__(self, g):
         if isinstance(g, list):
@@ -216,32 +218,38 @@
         else:
             return AreaIntersection([self, g.inverse()])
 
 
 class InvertedAreaGeometry(AreaGeometry):
     """
     Base class for inverted geometries.
-
-    Parameters
-    ----------
-    geometry : geom2d.AreaGeometry
-        The original geometry
+    
+    :group: utils.geom2d
 
     """
 
     def __init__(self, geometry):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        geometry: geom2d.AreaGeometry
+            The original geometry
+
+        """
         self._geometry = geometry
 
     def p_min(self):
         """
         Returns minimal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The minimal (x,y) point, shape = (2,)
 
         """
         pmi = self._geometry.p_min()
         if not np.any(np.isinf(pmi)):
             return np.full(2, -np.inf, dtype=np.float64)
         elif isinstance(self._geometry, InvertedAreaGeometry):
@@ -258,15 +266,15 @@
 
     def p_max(self):
         """
         Returns maximal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The maximal (x,y) point, shape = (2,)
 
         """
         pma = self._geometry.p_max()
         if not np.any(np.isinf(pma)):
             return np.full(2, np.inf, dtype=np.float64)
         elif isinstance(self._geometry, InvertedAreaGeometry):
@@ -283,43 +291,43 @@
 
     def points_distance(self, points, return_nearest=False):
         """
         Calculates point distances wrt boundary.
 
         Parameters
         ----------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The probe points, shape (n_points, 2)
-        return_nearest : bool
+        return_nearest: bool
             Flag for return of the nearest point on bundary
 
         Returns
         -------
-        dist : numpy.ndarray
+        dist: numpy.ndarray
             The smallest distances to the boundary,
             shape: (n_points,)
-        p_nearest : numpy.ndarray, optional
+        p_nearest: numpy.ndarray, optional
             The nearest points on the boundary, if
             return_nearest is True, shape: (n_points, 2)
 
         """
         return self._geometry.points_distance(points, return_nearest)
 
     def points_inside(self, points):
         """
         Tests if points are inside the geometry.
 
         Parameters
         ----------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The probe points, shape (n_points, 2)
 
         Returns
         -------
-        inside : numpy.ndarray
+        inside: numpy.ndarray
             True if point is inside, shape: (n_points,)
 
         """
         return ~self._geometry.points_inside(points)
 
     def add_to_figure(
         self,
@@ -330,25 +338,25 @@
         pars_distance={},
     ):
         """
         Add image to (x,y) figure.
 
         Parameters
         ----------
-        ax : matplotlib.pyplot.Axis
+        ax: matplotlib.pyplot.Axis
             The axis object
-        show_boundary : bool
+        show_boundary: bool
             Add the boundary line to the image
-        fill_mode : str, optional
+        fill_mode: str, optional
             Fill the area. Options:
             dist, dist_inside, dist_outside, inside_<color>,
             outside_<color>
-        pars_boundary : dict
+        pars_boundary: dict
             Parameters for boundary plotting command
-        pars_distance : dict
+        pars_distance: dict
             Parameters for distance plotting command
 
         """
         self._geometry.add_to_figure(
             ax,
             show_boundary,
             fill_mode=None,
@@ -361,47 +369,53 @@
 
     def inverse(self):
         """
         Get the inverted geometry
 
         Returns
         -------
-        inverted : foxes.utils.geom2d.InvertedAreaGeometry
+        inverted: foxes.utils.geom2d.InvertedAreaGeometry
             The inverted geometry
 
         """
         return self._geometry
 
 
 class AreaUnion(AreaGeometry):
     """
     The union of area geometries.
 
-    Parameters
-    ----------
-    geometries : list of geom2d.AreaGeometry
-        The geometries
-
     Attributes
     ----------
-    geometries : list of geom2d.AreaGeometry
+    geometries: list of geom2d.AreaGeometry
         The geometries
+    
+    :group: utils.geom2d
 
     """
 
     def __init__(self, geometries):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        geometries: list of geom2d.AreaGeometry
+            The geometries
+
+        """
         self.geometries = geometries
 
     def p_min(self):
         """
         Returns minimal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The minimal (x,y) point, shape = (2,)
 
         """
         out = None
         for g in self.geometries:
             pmi = g.p_min()
             if out is None:
@@ -412,15 +426,15 @@
 
     def p_max(self):
         """
         Returns maximal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The maximal (x,y) point, shape = (2,)
 
         """
         out = None
         for g in self.geometries:
             pma = g.p_max()
             if out is None:
@@ -431,25 +445,25 @@
 
     def points_distance(self, points, return_nearest=False):
         """
         Calculates point distances wrt boundary.
 
         Parameters
         ----------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The probe points, shape (n_points, 2)
-        return_nearest : bool
+        return_nearest: bool
             Flag for return of the nearest point on bundary
 
         Returns
         -------
-        dist : numpy.ndarray
+        dist: numpy.ndarray
             The smallest distances to the boundary,
             shape: (n_points,)
-        p_nearest : numpy.ndarray, optional
+        p_nearest: numpy.ndarray, optional
             The nearest points on the boundary, if
             return_nearest is True, shape: (n_points, 2)
 
         """
         if len(self.geometries) == 1:
             return self.geometries[0].points_distance(points, return_nearest)
 
@@ -491,20 +505,20 @@
 
     def points_inside(self, points):
         """
         Tests if points are inside the geometry.
 
         Parameters
         ----------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The probe points, shape (n_points, 2)
 
         Returns
         -------
-        inside : numpy.ndarray
+        inside: numpy.ndarray
             True if point is inside, shape: (n_points,)
 
         """
         if len(self.geometries) == 1:
             return self.geometries[0].points_inside(points)
 
         n_pts = len(points)
@@ -522,25 +536,25 @@
         pars_distance={},
     ):
         """
         Add image to (x,y) figure.
 
         Parameters
         ----------
-        ax : matplotlib.pyplot.Axis
+        ax: matplotlib.pyplot.Axis
             The axis object
-        show_boundary : bool
+        show_boundary: bool
             Add the boundary line to the image
-        fill_mode : str, optional
+        fill_mode: str, optional
             Fill the area. Options:
             dist, dist_inside, dist_outside, inside_<color>,
             outside_<color>
-        pars_boundary : dict
+        pars_boundary: dict
             Parameters for boundary plotting command
-        pars_distance : dict
+        pars_distance: dict
             Parameters for distance plotting command
 
         """
         if show_boundary:
             for g in self.geometries:
                 g.add_to_figure(
                     ax,
@@ -560,15 +574,15 @@
 
     def inverse(self):
         """
         Get the inverted geometry
 
         Returns
         -------
-        inverted : foxes.utils.geom2d.InvertedAreaGeometry
+        inverted: foxes.utils.geom2d.InvertedAreaGeometry
             The inverted geometry
 
         """
         return InvertedAreaUnion(self)
 
     def __add__(self, g):
         if isinstance(g, list):
@@ -579,31 +593,36 @@
             return AreaUnion(self.geometries + [g])
 
 
 class InvertedAreaUnion(InvertedAreaGeometry):
     """
     Inversion of a union of areas
 
-    Parameters
-    ----------
-    union : geom2d.AreaUnion
-        The original area union geometry
+    :group: utils.geom2d
 
     """
-
     def __init__(self, union):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        union: geom2d.AreaUnion
+            The original area union geometry
+
+        """
         super().__init__(union)
 
     def p_min(self):
         """
         Returns minimal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The minimal (x,y) point, shape = (2,)
 
         """
         if len(self._geometry.geometries) == 1:
             return self._geometry.geometries[0].inverse().p_min()
 
         pmi = self._geometry.p_min()
@@ -623,15 +642,15 @@
 
     def p_max(self):
         """
         Returns maximal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The maximal (x,y) point, shape = (2,)
 
         """
         if len(self._geometry.geometries) == 1:
             return self._geometry.geometries[0].inverse().p_max()
 
         pma = self._geometry.p_max()
@@ -650,16 +669,22 @@
             return out
 
 
 class AreaIntersection(AreaGeometry):
     """
     The intersection of area geometries.
 
-    Parameters
-    ----------
-    geometries : list of geom2d.AreaGeometry
-        The geometries
+    :group: utils.geom2d
 
     """
 
     def __new__(cls, geometries):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        geometries: list of geom2d.AreaGeometry
+            The geometries
+
+        """
         return AreaUnion([g.inverse() for g in geometries]).inverse()
```

### Comparing `foxes-0.3.5/foxes/utils/geom2d/circle.py` & `foxes-0.4.0/foxes/utils/geom2d/circle.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,75 +4,81 @@
 from .area_geometry import AreaGeometry
 
 
 class Circle(AreaGeometry):
     """
     This class represents the area of a circle.
 
-    Parameters
-    ----------
-    centre : numpy.ndarray
-        The centre point, shape: (2,)
-    radius : float
-        The radius
-
     Attributes
     ----------
-    centre : numpy.ndarray
+    centre: numpy.ndarray
         The centre point, shape: (2,)
-    radius : float
+    radius: float
         The radius
 
+    :group: utils.geom2d
+
     """
 
     def __init__(self, centre, radius):
+        """
+        Cobnstructor.
+        
+        Parameters
+        ----------
+        centre: numpy.ndarray
+            The centre point, shape: (2,)
+        radius: float
+            The radius
+
+        """
         self.centre = np.array(centre, dtype=np.float64)
         self.radius = radius
 
     def p_min(self):
         """
         Returns minimal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The minimal (x,y) point, shape = (2,)
 
         """
         return self.centre - self.radius
 
     def p_max(self):
         """
         Returns maximal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The maximal (x,y) point, shape = (2,)
 
         """
         return self.centre + self.radius
 
     def points_distance(self, points, return_nearest=False):
         """
         Calculates point distances wrt boundary.
 
         Parameters
         ----------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The probe points, shape (n_points, 2)
-        return_nearest : bool
+        return_nearest: bool
             Flag for return of the nearest point on bundary
 
         Returns
         -------
-        dist : numpy.ndarray
+        dist: numpy.ndarray
             The smallest distances to the boundary,
             shape: (n_points,)
-        p_nearest : numpy.ndarray, optional
+        p_nearest: numpy.ndarray, optional
             The nearest points on the boundary, if
             return_nearest is True, shape: (n_points, 2)
 
         """
 
         deltas = points - self.centre[None, :]
         magd = np.linalg.norm(deltas, axis=-1)
@@ -93,45 +99,45 @@
 
     def points_inside(self, points):
         """
         Tests if points are inside the geometry.
 
         Parameters
         ----------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The probe points, shape (n_points, 2)
 
         Returns
         -------
-        inside : numpy.ndarray
+        inside: numpy.ndarray
             True if point is inside, shape: (n_points,)
 
         """
         magd = np.linalg.norm(points - self.centre[None, :], axis=-1)
         return magd <= self.radius
 
     def add_to_figure(
         self, ax, show_boundary=True, fill_mode=None, pars_boundary={}, pars_distance={}
     ):
         """
         Add image to (x,y) figure.
 
         Parameters
         ----------
-        ax : matplotlib.pyplot.Axis
+        ax: matplotlib.pyplot.Axis
             The axis object
-        show_boundary : bool
+        show_boundary: bool
             Add the boundary line to the image
-        fill_mode : str, optional
+        fill_mode: str, optional
             Fill the area. Options:
             dist, dist_inside, dist_outside, inside_<color>,
             outside_<color>
-        pars_boundary : dict
+        pars_boundary: dict
             Parameters for boundary plotting command
-        pars_distance : dict
+        pars_distance: dict
             Parameters for distance plotting command
 
         """
         if show_boundary:
             pars = dict(color="darkblue", linewidth=1, fill=False)
             pars.update(pars_boundary)
```

### Comparing `foxes-0.3.5/foxes/utils/geom2d/example_intersection.py` & `foxes-0.4.0/foxes/utils/geom2d/example_intersection.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/utils/geom2d/example_union.py` & `foxes-0.4.0/foxes/utils/geom2d/example_union.py`

 * *Files identical despite different names*

### Comparing `foxes-0.3.5/foxes/utils/geom2d/half_plane.py` & `foxes-0.4.0/foxes/utils/geom2d/half_plane.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,45 +4,51 @@
 from .area_geometry import AreaGeometry
 
 
 class HalfPlane(AreaGeometry):
     """
     This class represents a half plane in 2d.
 
-    Parameters
-    ----------
-    centre : numpy.ndarray
-        The centre point, shape: (2,)
-    n : numpy.ndarray
-        The direction vector to the inside, shape: (2,)
-
     Attributes
     ----------
-    centre : numpy.ndarray
+    centre: numpy.ndarray
         The centre point, shape: (2,)
-    n : numpy.ndarray
+    n: numpy.ndarray
         The direction vector to the inside, shape: (2,)
-    n : numpy.ndarray
+    n: numpy.ndarray
         The direction vector orthogonal to n, shape: (2,)
 
+    :group: utils.geom2d
+
     """
 
     def __init__(self, centre, n):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        centre: numpy.ndarray
+            The centre point, shape: (2,)
+        n: numpy.ndarray
+            The direction vector to the inside, shape: (2,)
+
+        """
         self.centre = np.array(centre, dtype=np.float64)
         self.n = np.array(n, dtype=np.float64)
         self.n /= np.linalg.norm(self.n)
         self.m = np.array([-self.n[1], self.n[0]], dtype=np.float64)
 
     def p_min(self):
         """
         Returns minimal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The minimal (x,y) point, shape = (2,)
 
         """
         if np.linalg.norm(self.n - np.array([1, 0])) < 1e-13:
             return np.array([self.centre[0], -np.inf], dtype=np.float64)
         if np.linalg.norm(self.n - np.array([-1, 0])) < 1e-13:
             return np.array([-np.inf, -np.inf], dtype=np.float64)
@@ -55,15 +61,15 @@
 
     def p_max(self):
         """
         Returns maximal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The maximal (x,y) point, shape = (2,)
 
         """
         if np.linalg.norm(self.n - np.array([1, 0])) < 1e-13:
             return np.array([np.inf, np.inf], dtype=np.float64)
         if np.linalg.norm(self.n - np.array([-1, 0])) < 1e-13:
             return np.array([self.centre[0], np.inf], dtype=np.float64)
@@ -76,25 +82,25 @@
 
     def points_distance(self, points, return_nearest=False):
         """
         Calculates point distances wrt boundary.
 
         Parameters
         ----------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The probe points, shape (n_points, 2)
-        return_nearest : bool
+        return_nearest: bool
             Flag for return of the nearest point on bundary
 
         Returns
         -------
-        dist : numpy.ndarray
+        dist: numpy.ndarray
             The smallest distances to the boundary,
             shape: (n_points,)
-        p_nearest : numpy.ndarray, optional
+        p_nearest: numpy.ndarray, optional
             The nearest points on the boundary, if
             return_nearest is True, shape: (n_points, 2)
 
         """
 
         deltas = points - self.centre[None, :]
         x = np.einsum("pd,d->p", deltas, self.n)
@@ -108,20 +114,20 @@
 
     def points_inside(self, points):
         """
         Tests if points are inside the geometry.
 
         Parameters
         ----------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The probe points, shape (n_points, 2)
 
         Returns
         -------
-        inside : numpy.ndarray
+        inside: numpy.ndarray
             True if point is inside, shape: (n_points,)
 
         """
         deltas = points - self.centre[None, :]
         x = np.einsum("pd,d->p", deltas, self.n)
         return x >= 0.0
 
@@ -129,25 +135,25 @@
         self, ax, show_boundary=True, fill_mode=None, pars_boundary={}, pars_distance={}
     ):
         """
         Add image to (x,y) figure.
 
         Parameters
         ----------
-        ax : matplotlib.pyplot.Axis
+        ax: matplotlib.pyplot.Axis
             The axis object
-        show_boundary : bool
+        show_boundary: bool
             Add the boundary line to the image
-        fill_mode : str, optional
+        fill_mode: str, optional
             Fill the area. Options:
             dist, dist_inside, dist_outside, inside_<color>,
             outside_<color>
-        pars_boundary : dict
+        pars_boundary: dict
             Parameters for boundary plotting command
-        pars_distance : dict
+        pars_distance: dict
             Parameters for distance plotting command
 
         """
         if show_boundary:
             pars = dict(color="darkblue", linewidth=1)
             pars.update(pars_boundary)
 
@@ -159,15 +165,15 @@
 
     def inverse(self):
         """
         Get the inverted geometry
 
         Returns
         -------
-        inverted : foxes.utils.geom2d.InvertedAreaGeometry
+        inverted: foxes.utils.geom2d.InvertedAreaGeometry
             The inverted geometry
 
         """
         return HalfPlane(self.centre, -self.n)
 
 
 if __name__ == "__main__":
```

### Comparing `foxes-0.3.5/foxes/utils/geom2d/polygon.py` & `foxes-0.4.0/foxes/utils/geom2d/polygon.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,29 +7,35 @@
 from .area_geometry import AreaGeometry
 
 
 class ClosedPolygon(AreaGeometry):
     """
     This class represents a closed 2D polygon.
 
-    Parameters
-    ----------
-    points : numpy.ndarray
-        The polygon points, shape: (n_points, 2)
-
     Attributes
     ----------
-    points : numpy.ndarray
+    points: numpy.ndarray
         The polygon points
-    poly : matplotlib.path.Path
+    poly: matplotlib.path.Path
         The closed polygon geometry
 
+    :group: utils.geom2d
+
     """
 
     def __init__(self, points):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        points: numpy.ndarray
+            The polygon points, shape: (n_points, 2)
+
+        """
         self.points = points
 
         if not np.all(points[0] == points[-1]):
             self.points = np.append(self.points, points[[0]], axis=0)
 
         self.poly = Path(self.points, closed=True)
 
@@ -37,49 +43,49 @@
 
     def p_min(self):
         """
         Returns minimal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The minimal (x,y) point, shape = (2,)
 
         """
         return np.min(self.points, axis=0)
 
     def p_max(self):
         """
         Returns maximal (x,y) point.
 
         Returns
         -------
-        p_min : numpy.ndarray
+        p_min: numpy.ndarray
             The maximal (x,y) point, shape = (2,)
 
         """
         return np.max(self.points, axis=0)
 
     def points_distance(self, points, return_nearest=False):
         """
         Calculates point distances wrt boundary.
 
         Parameters
         ----------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The probe points, shape (n_points, 2)
-        return_nearest : bool
+        return_nearest: bool
             Flag for return of the nearest point on bundary
 
         Returns
         -------
-        dist : numpy.ndarray
+        dist: numpy.ndarray
             The smallest distances to the boundary,
             shape: (n_points,)
-        p_nearest : numpy.ndarray, optional
+        p_nearest: numpy.ndarray, optional
             The nearest points on the boundary, if
             return_nearest is True, shape: (n_points, 2)
 
         """
 
         dists = cdist(points, self.points[:-1])
 
@@ -128,44 +134,44 @@
 
     def points_inside(self, points):
         """
         Tests if points are inside the geometry.
 
         Parameters
         ----------
-        points : numpy.ndarray
+        points: numpy.ndarray
             The probe points, shape (n_points, 2)
 
         Returns
         -------
-        inside : numpy.ndarray
+        inside: numpy.ndarray
             True if point is inside, shape: (n_points,)
 
         """
         return self.poly.contains_points(points)
 
     def add_to_figure(
         self, ax, show_boundary=True, fill_mode=None, pars_boundary={}, pars_distance={}
     ):
         """
         Add image to (x,y) figure.
 
         Parameters
         ----------
-        ax : matplotlib.pyplot.Axis
+        ax: matplotlib.pyplot.Axis
             The axis object
-        show_boundary : bool
+        show_boundary: bool
             Add the boundary line to the image
-        fill_mode : str, optional
+        fill_mode: str, optional
             Fill the area. Options:
             dist, dist_inside, dist_outside, inside_<color>,
             outside_<color>
-        pars_boundary : dict
+        pars_boundary: dict
             Parameters for boundary plotting command
-        pars_distance : dict
+        pars_distance: dict
             Parameters for distance plotting command
 
         """
         if show_boundary:
             pars = dict(facecolor="none", edgecolor="darkblue", linewidth=1)
             pars.update(pars_boundary)
```

### Comparing `foxes-0.3.5/foxes/utils/geopandas_helpers.py` & `foxes-0.4.0/foxes/utils/geopandas_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,46 +50,50 @@
 
 def read_shp(fname, **kwargs):
     """
     Read a shape file
 
     Parameters
     ----------
-    fname : str
+    fname: str
         Path to the .shp file
-    kwargs : dict, optional
+    kwargs: dict, optional
         Additional parameters for geopandas.read_file()
 
     Returns
     -------
-    data : geopandas.GeoDataFrame
+    data: geopandas.GeoDataFrame
         The data frame in WSG84
+    
+    :group: utils
 
     """
     check_import_gpd()
     gpdf = gpd.read_file(fname, **kwargs)
     return gpdf.to_crs("EPSG:4326")  # Convert to WGS84
 
 
 def shp2csv(ifile, ofile, in_kwargs={}, out_kwargs={}, verbosity=1):
     """
     Read shape file, write csv file
 
     Parameters
     ----------
-    iname : str
+    iname: str
         Path to the input .shp file
-    oname : str
+    oname: str
         Path to the output .csv file
-    in_kwargs : dict
+    in_kwargs: dict
         Additional parameters for geopandas.read_file()
-    out_kwargs : dict
+    out_kwargs: dict
         Additional parameters for geopandas to_csv()
-    verbosity : int
+    verbosity: int
         The verbosity level, 0 = silent
+    
+    :group: utils
 
     """
     if verbosity > 0:
         print("Reading file", ifile)
 
     gpdf = read_shp(ifile, **in_kwargs)
 
@@ -132,41 +136,43 @@
     **kwargs,
 ):
     """
     Reads the polygon points from a shp file.
 
     Parameters
     ----------
-    fname : str
+    fname: str
         Path to the .shp file
-    names : list: of str, optinal
+    names: list: of str, optinal
         The names of the polygons to be extracted. All by
         default
-    name_col : int
+    name_col: int
         Column that contains the area names
-    geom_col : str
+    geom_col: str
         The geometry column
-    to_utm : bool or str, optional
+    to_utm: bool or str, optional
         Convert to UTM coordinates. If str, then UTM zone
         plus letter, e.g. "32U"
-    ret_utm_zone : bool
+    ret_utm_zone: bool
         Return UTM zone plus letter as str
-    kwargs : dict, optional
+    kwargs: dict, optional
         Additional parameters for geopandas.read_shp()
 
     Returns
     -------
-    point_dict_exterior : dict
+    point_dict_exterior: dict
         Dict with list of array of points. Key: area name,
         Value: list:np.ndarray, shape of latter: (n_points, 2)
-    point_dict_interior : dict
+    point_dict_interior: dict
         Dict with list of array of points. Key: area name,
         Value: list:np.ndarray, shape of latter: (n_points, 2)
-    utm_zone_str : str, optional
+    utm_zone_str: str, optional
         The utem zone plus letter as str, e.g. "32U"
+    
+    :group: utils
 
     """
 
     pdf = read_shp(fname, **kwargs)
     pnames = list(pdf[name_col])
 
     utmz = None
@@ -221,28 +227,30 @@
 
 def shp2geom2d(*args, ret_utm_zone=False, **kwargs):
     """
     Read shapefile into geom2d geometry
 
     Parameters
     ----------
-    args : tuple, optional
+    args: tuple, optional
         Arguments for read_shp_polygons()
-    ret_utm_zone : bool
+    ret_utm_zone: bool
         Return UTM zone plus letter as str
-    kwargs : dict, optional
+    kwargs: dict, optional
         Keyword arguments for read_shp_polygons()
 
     Returns
     -------
-    geom : foxes.tools.geom2D.AreaGeometry
+    geom: foxes.tools.geom2D.AreaGeometry
         The geometry object
-    utm_zone_str : str, optional
+    utm_zone_str: str, optional
         The utem zone plus letter as str, e.g. "32U"
-
+    
+    :group: utils
+    
     """
 
     exint = read_shp_polygons(*args, ret_utm_zone=ret_utm_zone, **kwargs)
 
     def _create_geom(data):
         if not len(data):
             return None
```

### Comparing `foxes-0.3.5/foxes/utils/pandas_helpers.py` & `foxes-0.4.0/foxes/utils/pandas_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,26 @@
 class PandasFileHelper:
     """
     This class helps reading and writing data
     to files via pandas.
 
     Attributes
     ----------
-    DEFAULT_READING_PARAMETERS : dict
+    DEFAULT_READING_PARAMETERS: dict
         Default parameters for file reading
         for the supported file formats
-    DEFAULT_WRITING_PARAMETERS : dict
+    DEFAULT_WRITING_PARAMETERS: dict
         Default parameters for file writing
         for the supported file formats
-    DATA_FILE_FORMAT : list:str
+    DATA_FILE_FORMAT: list:str
         The supported file formats for data export
-    DEFAULT_FORMAT_DICT : dict
+    DEFAULT_FORMAT_DICT: dict
         Default column formatting
+    
+    :group: utils
 
     """
 
     DEFAULT_READING_PARAMETERS = {
         "csv": {},
         "csv.gz": {},
         "csv.bz2": {},
@@ -76,17 +78,17 @@
     @classmethod
     def read_file(cls, file_path, **kwargs):
         """
         Helper for reading data according to file ending.
 
         Parameters
         ----------
-        file_path : str
+        file_path: str
             The path to the file
-        **kwargs : dict, optional
+        **kwargs: dict, optional
             Parameters forwarded to the pandas reading method.
 
         Returns
         -------
         pandas.DataFrame :
             The data
 
@@ -120,22 +122,22 @@
     @classmethod
     def write_file(cls, data, file_path, format_dict={}, **kwargs):
         """
         Helper for writing data according to file ending.
 
         Parameters
         ----------
-        data : pandas.DataFrame
+        data: pandas.DataFrame
             The data
-        file_path : str
+        file_path: str
             The path to the file
-        format_dict : dict
+        format_dict: dict
             Dictionary with format entries for
             columns, e.g. '{:.4f}'
-        **kwargs : dict, optional
+        **kwargs: dict, optional
             Parameters forwarded to the pandas writing method.
 
         """
 
         fdict = deepcopy(cls.DEFAULT_FORMAT_DICT)
         fdict.update(format_dict)
```

### Comparing `foxes-0.3.5/foxes/utils/runners.py` & `foxes-0.4.0/foxes/utils/runners/runners.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from abc import abstractmethod, ABCMeta
 import dask
+from abc import abstractmethod, ABCMeta
+from copy import deepcopy
 from dask.distributed import Client, LocalCluster
 from dask.distributed import get_client
 from dask.diagnostics import ProgressBar
 
-import foxes.constants as FC
-
 class Runner(metaclass=ABCMeta):
     """
     Abstract base class for runners.
+
+    :group: utils.runners
+
     """
 
     def __init__(self):
         self._initialized = False
 
     def initialize(self):
         """
@@ -40,24 +42,24 @@
     @abstractmethod
     def run(self, func, args=tuple(), kwargs={}):
         """
         Runs the given function.
 
         Parameters
         ----------
-        func : Function
+        func: Function
             The function to be run
-        args : tuple
+        args: tuple
             The function arguments
-        kwargs : dict
+        kwargs: dict
             The function keyword arguments
 
         Returns
         -------
-        results : Any
+        results: Any
             The functions return value
 
         """
         pass
 
     def finalize(self):
         """
@@ -68,85 +70,94 @@
     def __exit__(self, exc_type, exc_value, traceback):
         self.finalize()
 
 
 class DefaultRunner(Runner):
     """
     Class for default function execution.
+
+    :group: utils.runners
+
     """
 
     def run(self, func, args=tuple(), kwargs={}):
         """
         Runs the given function.
 
         Parameters
         ----------
-        func : Function
+        func: Function
             The function to be run
-        args : tuple
+        args: tuple
             The function arguments
-        kwargs : dict
+        kwargs: dict
             The function keyword arguments
 
         Returns
         -------
-        results : Any
+        results: Any
             The functions return value
 
         """
         return func(*args, **kwargs)
 
 
 class DaskRunner(Runner):
     """
     Class for function execution via dask
 
-    Parameters
-    ----------
-    scheduler : str, optional
-        The dask scheduler choice
-    n_workers : int, optional
-        The number of workers for parallel run
-    threads_per_worker : int, optional
-        The number of threads per worker for parallel run
-    progress_bar : bool
-        Flag for showing progress bar
-    cluster_args : dict, optional
-        Explicit arguments for the cluster setup
-    client_args : dict, optional
-        Explicit arguments for the client setup
-    verbosity : int
-        The verbosity level, 0 = silent
-
     Attributes
     ----------
-    scheduler : str, optional
+    scheduler: str, optional
         The dask scheduler choice
-    progress_bar : bool
+    progress_bar: bool
         Flag for showing progress bar
-    cluster_args : dict, optional
+    cluster_args: dict, optional
         Explicit arguments for the cluster setup
-    client_args : dict, optional
+    client_args: dict, optional
         Explicit arguments for the client setup
-    verbosity : int
+    verbosity: int
         The verbosity level, 0 = silent
 
+    :group: utils.runners
+
     """
 
     def __init__(
         self,
         scheduler=None,
         n_workers=None,
         threads_per_worker=None,
         processes=True,
         cluster_args=None,
         client_args={},
         progress_bar=True,
         verbosity=1,
     ):
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        scheduler: str, optional
+            The dask scheduler choice
+        n_workers: int, optional
+            The number of workers for parallel run
+        threads_per_worker: int, optional
+            The number of threads per worker for parallel run
+        progress_bar: bool
+            Flag for showing progress bar
+        cluster_args: dict, optional
+            Explicit arguments for the cluster setup
+        client_args: dict, optional
+            Explicit arguments for the client setup
+        verbosity: int
+            The verbosity level, 0 = silent
+
+        """
         super().__init__()
 
         self.scheduler = scheduler
         self.client_args = client_args
         self.progress_bar = progress_bar
         self.verbosity = verbosity
 
@@ -179,22 +190,39 @@
             return False
 
     def initialize(self):
         """
         Initialize the runner
         """
         if self.scheduler == "distributed":
-            self.print("Launching dask cluster..")
+
+            self.print("Launching local dask cluster..")
 
             self._cluster = LocalCluster(**self.cluster_args)
             self._client = Client(self._cluster, **self.client_args)
 
             self.print(self._cluster)
             self.print(f"Dashboard: {self._client.dashboard_link}\n")
 
+        elif self.scheduler == "slurm":
+
+            from dask_jobqueue import SLURMCluster
+
+            self.print("Launching dask cluster on HPC using SLURM..")
+
+            cargs = deepcopy(self.cluster_args)
+            nodes = cargs.pop("nodes", 1)
+            
+            self._cluster = SLURMCluster(**cargs)
+            self._cluster.scale(jobs=nodes)
+            self._client = Client(self._cluster, **self.client_args)
+
+            self.print(self._cluster)
+            self.print(f"Dashboard: {self._client.dashboard_link}\n")
+
         super().initialize()
 
     def print(self, *args, **kwargs):
         """
         Prints if verbosity is not zero
         """
         if self.verbosity > 0:
@@ -202,24 +230,24 @@
 
     def run(self, func, args=tuple(), kwargs={}):
         """
         Runs the given function.
 
         Parameters
         ----------
-        func : Function
+        func: Function
             The function to be run
-        args : tuple
+        args: tuple
             The function arguments
-        kwargs : dict
+        kwargs: dict
             The function keyword arguments
 
         Returns
         -------
-        results : Any
+        results: Any
             The functions return value
 
         """
         if self.progress_bar:
             with ProgressBar():
                 results = func(*args, **kwargs)
         else:
@@ -227,15 +255,15 @@
 
         return results
 
     def finalize(self):
         """
         Finallize the runner
         """
-        if self.scheduler == "distributed":
+        if self.scheduler in ["distributed", "slurm"]:
             self.print("\n\nShutting down dask cluster")
             self._client.close()
             self._cluster.close()
 
         dask.config.refresh()
 
         super().finalize()
```

### Comparing `foxes-0.3.5/foxes/utils/two_circles.py` & `foxes-0.4.0/foxes/utils/two_circles.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 
 def area(r1, r2, d):
-    """ "
+    """
     Calculates the intersection of two
     circles with radii r1, r2 and a centre
     point distance d.
 
     Make sure that
 
         1) r1 >= r2
@@ -16,26 +16,28 @@
     within the function.
 
     Source:
     https://diego.assencio.com/?index=8d6ca3d82151bad815f78addf9b5c1c6
 
     Parameters
     ----------
-    r1 : float or numpy.ndarray
+    r1: float or numpy.ndarray
         The radius of circle 1
-    r2 : float or numpy.ndarray
+    r2: float or numpy.ndarray
         The radius of circle 2
-    d : float or numpy.ndarray
+    d: float or numpy.ndarray
         The distance between the centre points
         of the two circles
 
     Returns
     -------
-    area : float or numpy.ndarray
+    area: float or numpy.ndarray
         The intersectional area
+    
+    :group: utils.two_circles
 
     """
     d1 = (r1**2 - r2**2 + d**2) / (2 * d)
     d2 = d - d1
 
     a = np.maximum(np.minimum(d1 / r1, 1.0), -1)
     b = np.maximum(r1**2 - d1**2, 0.0)
@@ -58,26 +60,28 @@
     Calculates the intersection of two circles.
 
     All parameters should have the same shape,
     or be broadcastable to one another.
 
     Parameters
     ----------
-    r1 : numpy.ndarray
+    r1: numpy.ndarray
         The radius of circle 1
-    r2 : numpy.ndarray
+    r2: numpy.ndarray
         The radius of circle 2
-    d : numpy.ndarray
+    d: numpy.ndarray
         The distance between the centre points
         of the two circles
 
     Returns
     -------
-    area : numpy.ndarray
+    area: numpy.ndarray
         The intersectional area
+    
+    :group: utils.two_circles
 
     """
 
     # prepare:
     out = np.zeros_like(d)
 
     # condition d < r1 + r2:
```

### Comparing `foxes-0.3.5/foxes/utils/wind_dir.py` & `foxes-0.4.0/foxes/utils/wind_dir.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 def wd2wdvec(wd, ws=1.0, axis=-1):
     """
     Calculate wind direction vectors from wind directions
     in degrees.
 
     Parameters
     ----------
-    wd : numpy.ndarray
+    wd: numpy.ndarray
         Wind direction array (any shape)
-    ws : float or numpy.ndarray
+    ws: float or numpy.ndarray
         The wind speed. Has to broadcast against wd.
-    axis : int
+    axis: int
         Location where to insert the (x, y) dimension
         into the shape of wd
 
     Returns
     -------
-    wdvec : numpy.ndarray
+    wdvec: numpy.ndarray
         The wind direction vectors
+    
+    :group: utils
 
     """
 
     wdr = wd * np.pi / 180.0
     n = np.stack([np.sin(wdr), np.cos(wdr)], axis=axis)
 
     if np.isscalar(ws):
@@ -35,47 +37,51 @@
 def wd2uv(wd, ws=1.0, axis=-1):
     """
     Calculate wind vectors from wind directions
     in degrees.
 
     Parameters
     ----------
-    wd : numpy.ndarray
+    wd: numpy.ndarray
         Wind direction array (any shape)
-    ws : float or numpy.ndarray
+    ws: float or numpy.ndarray
         The wind speed. Has to broadcast against wd.
-    axis : int
+    axis: int
         Axis location where to insert the (u, v) components
         into the shape of wd
 
     Returns
     -------
-    uv : numpy.ndarray
+    uv: numpy.ndarray
         The wind vectors
 
+    :group: utils
+
     """
     return -wd2wdvec(wd, ws, axis)
 
 
 def uv2wd(uv, axis=-1):
     """
     Calculate wind direction from wind vectors.
 
     Parameters
     ----------
-    uv : numpy.ndarray
+    uv: numpy.ndarray
         The wind vectors, any shape
-    axis : int
+    axis: int
         The axis which corresponds to (u, v) components
 
     Returns
     -------
-    wd : numpy.ndarray
+    wd: numpy.ndarray
         The wind direction array
 
+    :group: utils
+
     """
 
     if axis == -1:
         u = uv[..., 0]
         v = uv[..., 1]
     else:
         s = tuple(0 if a == axis else slice(None) for a in range(len(uv.shape)))
@@ -88,47 +94,51 @@
 
 def wdvec2wd(wdvec, axis=-1):
     """
     Calculate wind direction from wind direction vectors.
 
     Parameters
     ----------
-    wdvec : numpy.ndarray
+    wdvec: numpy.ndarray
         The wind direction vectors, any shape
-    axis : int
+    axis: int
         The axis which corresponds to (x, y) components
 
     Returns
     -------
-    wd : numpy.ndarray
+    wd: numpy.ndarray
         The wind direction array
 
+    :group: utils
+
     """
     return uv2wd(-wdvec, axis)
 
 
 def delta_wd(wd_a, wd_b):
     """
     Calculates wd_b - wd_a.
 
     Parameters
     ----------
-    wd_a : numpy.ndarray
+    wd_a: numpy.ndarray
         Array of wind directions.
         Shape: any shape
-    wd_b : numpy.ndarray
+    wd_b: numpy.ndarray
         Array of wind directions.
         Shape: same as wd_a
 
     Returns
     -------
     numpy.ndarray :
         Array of wind direction deltas.
         Shape: same as wd_a, wd_b
 
+    :group: utils
+
     """
     out = wd_b - wd_a
 
     out[out < -180.0] += 360.0
     out[out > 180.0] -= 360.0
 
     return out
```

### Comparing `foxes-0.3.5/foxes/variables.py` & `foxes-0.4.0/foxes/variables.py`

 * *Files 15% similar despite different names*

```diff
@@ -98,14 +98,18 @@
     Factor between K and TI, K = KB + KTI*TI
 Z0 : str
     The roughness length in m
 MOL : str
     The Monin-Ubukhof length in m
 SHEAR : str
     The shear exponent
+PA_ALPHA : str
+    The alpha parameter of the PorteAgel wake model
+PA_BETA : str
+    The beta parameter of the PorteAgel wake model
 
 """
 
 X = "X"
 Y = "Y"
 H = "H"
 D = "D"
@@ -172,7 +176,10 @@
 K = "k"
 KB = "kb"
 KTI = "kTI"
 
 Z0 = "z0"
 MOL = "MOL"
 SHEAR = "shear"
+
+PA_ALPHA = "PA_alpha"
+PA_BETA = "PA_beta"
```

### Comparing `foxes-0.3.5/foxes.egg-info/PKG-INFO` & `foxes-0.4.0/foxes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.3.5
+Version: 0.4.0
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
@@ -53,105 +53,105 @@
 
 - `Python 3.7`
 - `Python 3.8`
 - `Python 3.9`
 - `Python 3.10`
 - `Python 3.11`
 
-## Installation via conda
+## Installation via pip
 
 ### Virtual Python environment
 
-First create a new `conda` environment, for example called `foxes`, by
+First create a new `venv` environment, for example called `foxes` and located at `~/venv/foxes` (choose any other convenient name and location in your file system if you prefer), by
 
 ```console
-conda create -c conda-forge --name foxes
+python3 -m venv ~/venv/foxes
 ```
 
 Then activate the environment every time you work with `foxes`, by
 
 ```console
-conda activate foxes
+source ~/venv/foxes/bin/activate
 ```
 
 You can leave the environment by
 
 ```console
-conda deactivate
+deactivate
 ```
 
-The `conda` installation commands below should be executed within the active `foxes` environment.
+The `pip` installation commands below should be executed within the active `foxes` environment.
 
 ### Standard users
 
-The `foxes` package is available on the channel [conda-forge](https://anaconda.org/conda-forge/foxes). You can install the latest version by
+As a standard user, you can install the latest release via [pip](https://pypi.org/project/foxes/) by
 
 ```console
-conda install -c conda-forge foxes
+pip install foxes
+```
+
+This commands installs the version that correspond to the `main` branch at [github](https://github.com/FraunhoferIWES/foxes). Alternatively, you can decide to install the latest pre-release developments (non-stable) by
+
+```console
+pip install git+https://github.com/FraunhoferIWES/foxes@dev#egg=foxes
 ```
 
 ### Developers
 
-For developers using `conda`, we recommend first installing foxes, then removing only the `foxes` package while keeping the dependencies, and then adding `foxes` again from a git using `conda develop`:
+For developers using `pip`, simply invoke the `-e` flag in the installation command in your local clone:
 
 ```console
-conda install -c conda-forge foxes conda-build
-conda remove foxes --force
 git clone https://github.com/FraunhoferIWES/foxes.git
 cd foxes
-conda develop .
+pip install -e .
 ```
 The last line makes sure that all your code changes are included whenever importing `foxes`. Concerning the `git clone` line, we actually recommend that you fork `foxes` on GitHub and then replace that command by cloning your fork instead.
 
-## Installation via pip
+## Installation via conda
 
 ### Virtual Python environment
 
-First create a new `venv` environment, for example called `foxes` and located at `~/venv/foxes` (choose any other convenient name and location in your file system if you prefer), by
+First create a new `conda` environment, for example called `foxes`, by
 
 ```console
-python3 -m venv ~/venv/foxes
+conda create -c conda-forge --name foxes
 ```
 
 Then activate the environment every time you work with `foxes`, by
 
 ```console
-source ~/venv/foxes/bin/activate
+conda activate foxes
 ```
 
 You can leave the environment by
 
 ```console
-deactivate
+conda deactivate
 ```
 
-The `pip` installation commands below should be executed within the active `foxes` environment.
+The `conda` installation commands below should be executed within the active `foxes` environment.
 
 ### Standard users
 
-As a standard user, you can install the latest release via [pip](https://pypi.org/project/foxes/) by
-
-```console
-pip install foxes
-```
-
-This commands installs the version that correspond to the `main` branch at [github](https://github.com/FraunhoferIWES/foxes). Alternatively, you can decide to install the latest pre-release developments (non-stable) by
+The `foxes` package is available on the channel [conda-forge](https://anaconda.org/conda-forge/foxes). You can install the latest version by
 
 ```console
-pip install git+https://github.com/FraunhoferIWES/foxes@dev#egg=foxes
+conda install -c conda-forge foxes
 ```
 
 ### Developers
 
-For developers using `pip`, simply invoke the `-e` flag in the installation command in your local clone:
+For developers using `conda`, we recommend first installing foxes, then removing only the `foxes` package while keeping the dependencies, and then adding `foxes` again from a git using `conda develop`:
 
 ```console
+conda install -c conda-forge foxes conda-build
+conda remove foxes --force
 git clone https://github.com/FraunhoferIWES/foxes.git
 cd foxes
-pip install -e .
+conda develop .
 ```
 The last line makes sure that all your code changes are included whenever importing `foxes`. Concerning the `git clone` line, we actually recommend that you fork `foxes` on GitHub and then replace that command by cloning your fork instead.
 
 ## Usage
 
 For detailed examples of how to run _foxes_, check the `examples` and `notebooks` folders in this repository. A minimal running example is the following, based on provided static `csv` data files:
```

### Comparing `foxes-0.3.5/foxes.egg-info/SOURCES.txt` & `foxes-0.4.0/foxes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 foxes/models/point_models/wake_deltas.py
 foxes/models/rotor_models/__init__.py
 foxes/models/rotor_models/centre.py
 foxes/models/rotor_models/grid.py
 foxes/models/turbine_models/__init__.py
 foxes/models/turbine_models/calculator.py
 foxes/models/turbine_models/kTI_model.py
+foxes/models/turbine_models/lookup_table.py
 foxes/models/turbine_models/power_mask.py
 foxes/models/turbine_models/rotor_centre_calc.py
 foxes/models/turbine_models/sector_management.py
 foxes/models/turbine_models/set_XYHD.py
 foxes/models/turbine_models/set_farm_vars.py
 foxes/models/turbine_models/table_factors.py
 foxes/models/turbine_models/thrust2ct.py
@@ -119,23 +120,22 @@
 foxes/models/turbine_models/yawm2yaw.py
 foxes/models/turbine_types/CpCt_file.py
 foxes/models/turbine_types/CpCt_from_two.py
 foxes/models/turbine_types/PCt_file.py
 foxes/models/turbine_types/PCt_from_two.py
 foxes/models/turbine_types/__init__.py
 foxes/models/turbine_types/null_type.py
-foxes/models/turbine_types/wsrho2PCt_two_files.py
+foxes/models/turbine_types/wsrho2PCt_from_two.py
 foxes/models/vertical_profiles/__init__.py
+foxes/models/vertical_profiles/abl_log_neutral_ws.py
+foxes/models/vertical_profiles/abl_log_stable_ws.py
+foxes/models/vertical_profiles/abl_log_unstable_ws.py
+foxes/models/vertical_profiles/abl_log_ws.py
+foxes/models/vertical_profiles/sheared_ws.py
 foxes/models/vertical_profiles/uniform.py
-foxes/models/vertical_profiles/abl_log/__init__.py
-foxes/models/vertical_profiles/abl_log/abl_log_neutral_ws.py
-foxes/models/vertical_profiles/abl_log/abl_log_stable_ws.py
-foxes/models/vertical_profiles/abl_log/abl_log_unstable_ws.py
-foxes/models/vertical_profiles/abl_log/abl_log_ws.py
-foxes/models/vertical_profiles/abl_log/sheared_ws.py
 foxes/models/wake_frames/__init__.py
 foxes/models/wake_frames/farm_order.py
 foxes/models/wake_frames/rotor_wd.py
 foxes/models/wake_frames/streamlines.py
 foxes/models/wake_frames/yawed_wakes.py
 foxes/models/wake_models/__init__.py
 foxes/models/wake_models/axisymmetric.py
@@ -194,23 +194,24 @@
 foxes/utils/__init__.py
 foxes/utils/cubic_roots.py
 foxes/utils/data_book.py
 foxes/utils/dict.py
 foxes/utils/geopandas_helpers.py
 foxes/utils/pandas_helpers.py
 foxes/utils/plotly_helpers.py
-foxes/utils/runners.py
 foxes/utils/subclasses.py
 foxes/utils/two_circles.py
 foxes/utils/wind_dir.py
 foxes/utils/abl/__init__.py
 foxes/utils/abl/neutral.py
 foxes/utils/abl/sheared.py
 foxes/utils/abl/stable.py
 foxes/utils/abl/unstable.py
 foxes/utils/geom2d/__init__.py
 foxes/utils/geom2d/area_geometry.py
 foxes/utils/geom2d/circle.py
 foxes/utils/geom2d/example_intersection.py
 foxes/utils/geom2d/example_union.py
 foxes/utils/geom2d/half_plane.py
-foxes/utils/geom2d/polygon.py
+foxes/utils/geom2d/polygon.py
+foxes/utils/runners/__init__.py
+foxes/utils/runners/runners.py
```

### Comparing `foxes-0.3.5/setup.cfg` & `foxes-0.4.0/setup.cfg`

 * *Files identical despite different names*

