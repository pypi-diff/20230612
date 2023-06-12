# Comparing `tmp/autolens-2023.6.12.4.tar.gz` & `tmp/autolens-2023.7.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autolens-2023.6.12.4.tar", last modified: Mon Jun 12 13:49:14 2023, max compression
+gzip compressed data, was "autolens-2023.7.7.2.tar", last modified: Wed Jun  7 09:59:22 2023, max compression
```

## Comparing `autolens-2023.6.12.4.tar` & `autolens-2023.7.7.2.tar`

### file list

```diff
@@ -1,121 +1,272 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.106236 autolens-2023.6.12.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/CITATIONS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-06-12 13:49:14.106236 autolens-2023.6.12.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.098236 autolens-2023.6.12.4/autolens/
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-12 13:49:05.000000 autolens-2023.6.12.4/autolens/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.098236 autolens-2023.6.12.4/autolens/aggregator/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/aggregator/fit_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/aggregator/fit_interferometer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/aggregator/subhalo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/aggregator/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.098236 autolens-2023.6.12.4/autolens/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18275 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/analysis/maker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.098236 autolens-2023.6.12.4/autolens/analysis/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/analysis/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/analysis/mock/mock_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/analysis/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/analysis/preloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/analysis/result.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/analysis/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/analysis/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/analysis/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.098236 autolens-2023.6.12.4/autolens/config/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/config/general.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/config/non_linear.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.098236 autolens-2023.6.12.4/autolens/config/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/config/visualize/plots.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.102236 autolens-2023.6.12.4/autolens/imaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/imaging/fit_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/imaging/imaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.102236 autolens-2023.6.12.4/autolens/imaging/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/imaging/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/imaging/mock/mock_fit_imaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.102236 autolens-2023.6.12.4/autolens/imaging/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/imaging/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20800 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/imaging/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/imaging/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/imaging/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.102236 autolens-2023.6.12.4/autolens/imaging/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/imaging/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21821 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/imaging/plot/fit_imaging_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.102236 autolens-2023.6.12.4/autolens/interferometer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/interferometer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/interferometer/fit_interferometer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/interferometer/interferometer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.102236 autolens-2023.6.12.4/autolens/interferometer/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/interferometer/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25353 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/interferometer/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/interferometer/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/interferometer/model/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.102236 autolens-2023.6.12.4/autolens/interferometer/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/interferometer/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/interferometer/plot/fit_interferometer_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.102236 autolens-2023.6.12.4/autolens/lens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/lens/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.102236 autolens-2023.6.12.4/autolens/lens/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/lens/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/lens/mock/mock_to_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/lens/mock/mock_tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.102236 autolens-2023.6.12.4/autolens/lens/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/lens/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/lens/plot/ray_tracing_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24518 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/lens/ray_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/lens/ray_tracing_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/lens/subhalo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/lens/to_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.102236 autolens-2023.6.12.4/autolens/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/plot/abstract_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.102236 autolens-2023.6.12.4/autolens/plot/get_visuals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/plot/get_visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/plot/get_visuals/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/plot/get_visuals/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.102236 autolens-2023.6.12.4/autolens/point/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.106236 autolens-2023.6.12.4/autolens/point/fit_point/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/fit_point/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/fit_point/fluxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/fit_point/max_separation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/fit_point/point_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/fit_point/point_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/fit_point/positions_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/fit_point/positions_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.106236 autolens-2023.6.12.4/autolens/point/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/mock/mock_point_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.106236 autolens-2023.6.12.4/autolens/point/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/model/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.106236 autolens-2023.6.12.4/autolens/point/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/plot/fit_point_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/plot/point_dataset_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/point_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    27183 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/point/point_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.106236 autolens-2023.6.12.4/autolens/quantity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/quantity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/quantity/fit_quantity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.106236 autolens-2023.6.12.4/autolens/quantity/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/quantity/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/quantity/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/quantity/model/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.106236 autolens-2023.6.12.4/autolens/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-12 13:49:04.000000 autolens-2023.6.12.4/autolens/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:14.106236 autolens-2023.6.12.4/autolens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-12 13:49:14.000000 autolens-2023.6.12.4/autolens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 13:49:05.000000 autolens-2023.6.12.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:05.000000 autolens-2023.6.12.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:49:14.106236 autolens-2023.6.12.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-12 13:49:05.000000 autolens-2023.6.12.4/setup.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.715563 autolens-2023.7.7.2/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        2 2023-01-29 10:55:28.000000 autolens-2023.7.7.2/.gitattributes
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.212536 autolens-2023.7.7.2/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.259528 autolens-2023.7.7.2/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3309 2022-12-19 16:37:24.000000 autolens-2023.7.7.2/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2204 2022-12-19 11:17:33.000000 autolens-2023.7.7.2/CITATIONS.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18883 2022-12-19 11:17:33.000000 autolens-2023.7.7.2/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2478 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/CONTRIBUTING.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1087 2020-11-17 10:41:26.000000 autolens-2023.7.7.2/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      382 2022-11-28 11:07:42.000000 autolens-2023.7.7.2/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8654 2023-06-07 09:59:22.714568 autolens-2023.7.7.2/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7880 2023-06-04 13:24:21.000000 autolens-2023.7.7.2/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.267527 autolens-2023.7.7.2/autolens/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5693 2023-06-07 09:57:30.000000 autolens-2023.7.7.2/autolens/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.278528 autolens-2023.7.7.2/autolens/aggregator/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      687 2023-05-11 09:41:21.000000 autolens-2023.7.7.2/autolens/aggregator/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4387 2023-06-03 09:30:52.000000 autolens-2023.7.7.2/autolens/aggregator/fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4396 2023-06-03 09:30:27.000000 autolens-2023.7.7.2/autolens/aggregator/fit_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1501 2023-06-03 09:30:52.000000 autolens-2023.7.7.2/autolens/aggregator/subhalo.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2602 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/autolens/aggregator/tracer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.295528 autolens-2023.7.7.2/autolens/analysis/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/analysis/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18281 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/autolens/analysis/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      179 2022-04-16 11:29:26.000000 autolens-2023.7.7.2/autolens/analysis/maker.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.299528 autolens-2023.7.7.2/autolens/analysis/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.7.7.2/autolens/analysis/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4143 2023-06-05 20:15:31.000000 autolens-2023.7.7.2/autolens/analysis/mock/mock_result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13123 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/analysis/positions.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12889 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/analysis/preloads.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15030 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/analysis/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      448 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/analysis/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1121 2023-04-24 16:24:52.000000 autolens-2023.7.7.2/autolens/analysis/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12590 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/analysis/visualizer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        2 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.302528 autolens-2023.7.7.2/autolens/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       52 2023-02-20 16:58:21.000000 autolens-2023.7.7.2/autolens/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1524 2022-12-05 10:32:56.000000 autolens-2023.7.7.2/autolens/config/non_linear.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.304527 autolens-2023.7.7.2/autolens/config/visualize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6526 2023-04-29 16:48:45.000000 autolens-2023.7.7.2/autolens/config/visualize/plots.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2099 2023-03-30 11:03:14.000000 autolens-2023.7.7.2/autolens/exc.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4402 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.309527 autolens-2023.7.7.2/autolens/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12978 2023-06-03 08:43:24.000000 autolens-2023.7.7.2/autolens/imaging/fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4985 2023-06-03 08:43:51.000000 autolens-2023.7.7.2/autolens/imaging/imaging.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.313526 autolens-2023.7.7.2/autolens/imaging/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.7.7.2/autolens/imaging/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      897 2022-08-01 13:03:47.000000 autolens-2023.7.7.2/autolens/imaging/mock/mock_fit_imaging.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.321527 autolens-2023.7.7.2/autolens/imaging/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/imaging/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22133 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/imaging/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3135 2023-04-24 16:24:52.000000 autolens-2023.7.7.2/autolens/imaging/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4431 2023-06-03 08:35:51.000000 autolens-2023.7.7.2/autolens/imaging/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.325527 autolens-2023.7.7.2/autolens/imaging/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/imaging/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21770 2023-06-03 16:20:05.000000 autolens-2023.7.7.2/autolens/imaging/plot/fit_imaging_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.331527 autolens-2023.7.7.2/autolens/interferometer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/interferometer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11508 2023-06-05 20:15:31.000000 autolens-2023.7.7.2/autolens/interferometer/fit_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3711 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/interferometer/interferometer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.342528 autolens-2023.7.7.2/autolens/interferometer/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/interferometer/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23148 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/interferometer/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2754 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/interferometer/model/result.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5483 2023-06-03 09:05:20.000000 autolens-2023.7.7.2/autolens/interferometer/model/visualizer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.349530 autolens-2023.7.7.2/autolens/interferometer/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/interferometer/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15248 2023-06-03 16:54:40.000000 autolens-2023.7.7.2/autolens/interferometer/plot/fit_interferometer_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.366528 autolens-2023.7.7.2/autolens/lens/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/autolens/lens/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.373527 autolens-2023.7.7.2/autolens/lens/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.7.7.2/autolens/lens/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      486 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/lens/mock/mock_to_inversion.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1698 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/lens/mock/mock_tracer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.378528 autolens-2023.7.7.2/autolens/lens/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/lens/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14835 2023-04-30 10:34:18.000000 autolens-2023.7.7.2/autolens/lens/plot/ray_tracing_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24526 2023-05-15 18:35:29.000000 autolens-2023.7.7.2/autolens/lens/ray_tracing.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6602 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/lens/ray_tracing_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12096 2023-06-03 09:37:39.000000 autolens-2023.7.7.2/autolens/lens/subhalo.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9280 2023-05-13 12:14:38.000000 autolens-2023.7.7.2/autolens/lens/to_inversion.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      459 2022-04-15 18:27:13.000000 autolens-2023.7.7.2/autolens/mock.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.383529 autolens-2023.7.7.2/autolens/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3808 2023-06-03 09:03:18.000000 autolens-2023.7.7.2/autolens/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      531 2022-11-11 15:50:09.000000 autolens-2023.7.7.2/autolens/plot/abstract_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.392528 autolens-2023.7.7.2/autolens/plot/get_visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:50:09.000000 autolens-2023.7.7.2/autolens/plot/get_visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1273 2022-11-11 15:50:09.000000 autolens-2023.7.7.2/autolens/plot/get_visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7666 2023-06-03 17:45:21.000000 autolens-2023.7.7.2/autolens/plot/get_visuals/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.399527 autolens-2023.7.7.2/autolens/point/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/point/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.414528 autolens-2023.7.7.2/autolens/point/fit_point/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.7.7.2/autolens/point/fit_point/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4187 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/fit_point/fluxes.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3317 2023-01-13 16:58:19.000000 autolens-2023.7.7.2/autolens/point/fit_point/max_separation.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2522 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/fit_point/point_dataset.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1522 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/fit_point/point_dict.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3681 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/fit_point/positions_image.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3415 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/fit_point/positions_source.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.418528 autolens-2023.7.7.2/autolens/point/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-12 15:33:01.000000 autolens-2023.7.7.2/autolens/point/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      287 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/mock/mock_point_solver.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.424528 autolens-2023.7.7.2/autolens/point/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/point/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3832 2023-06-03 08:44:08.000000 autolens-2023.7.7.2/autolens/point/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      349 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/model/result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.430527 autolens-2023.7.7.2/autolens/point/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/point/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3574 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/plot/fit_point_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5882 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/plot/point_dataset_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6786 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/point_dataset.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27183 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/autolens/point/point_solver.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.433528 autolens-2023.7.7.2/autolens/quantity/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/quantity/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1715 2022-10-16 15:04:29.000000 autolens-2023.7.7.2/autolens/quantity/fit_quantity.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.439528 autolens-2023.7.7.2/autolens/quantity/model/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/autolens/quantity/model/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7448 2023-04-06 18:40:49.000000 autolens-2023.7.7.2/autolens/quantity/model/analysis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2383 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/autolens/quantity/model/result.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.440528 autolens-2023.7.7.2/autolens/util/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1404 2023-06-04 09:51:02.000000 autolens-2023.7.7.2/autolens/util/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.713551 autolens-2023.7.7.2/autolens.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7619 2023-06-07 09:59:22.000000 autolens-2023.7.7.2/autolens.egg-info/SOURCES.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.445527 autolens-2023.7.7.2/docs/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.449528 autolens-2023.7.7.2/docs/_templates/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      832 2022-12-21 16:35:52.000000 autolens-2023.7.7.2/docs/_templates/custom-class-template.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1293 2022-12-16 17:06:50.000000 autolens-2023.7.7.2/docs/_templates/custom_module_template.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.456527 autolens-2023.7.7.2/docs/advanced/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      387 2022-04-17 15:21:49.000000 autolens-2023.7.7.2/docs/advanced/chaining.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6425 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/docs/advanced/database.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1374 2023-03-29 16:14:17.000000 autolens-2023.7.7.2/docs/advanced/graphical.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      502 2023-01-14 16:37:15.000000 autolens-2023.7.7.2/docs/advanced/slam.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.474527 autolens-2023.7.7.2/docs/api/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1627 2023-01-13 16:58:19.000000 autolens-2023.7.7.2/docs/api/data.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      307 2022-12-20 17:31:51.000000 autolens-2023.7.7.2/docs/api/fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      735 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/docs/api/galaxy.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      531 2022-12-14 14:59:54.000000 autolens-2023.7.7.2/docs/api/light.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1717 2023-05-31 17:00:51.000000 autolens-2023.7.7.2/docs/api/mass.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1350 2023-06-06 10:32:06.000000 autolens-2023.7.7.2/docs/api/modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1274 2022-12-14 15:52:09.000000 autolens-2023.7.7.2/docs/api/pixelization.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3173 2023-04-24 16:24:52.000000 autolens-2023.7.7.2/docs/api/plot.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      281 2022-12-14 15:52:09.000000 autolens-2023.7.7.2/docs/api/point.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      744 2022-12-15 16:03:11.000000 autolens-2023.7.7.2/docs/api/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4788 2023-04-24 16:26:16.000000 autolens-2023.7.7.2/docs/conf.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.489528 autolens-2023.7.7.2/docs/general/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2204 2022-12-19 11:17:33.000000 autolens-2023.7.7.2/docs/general/citations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1023 2022-11-27 17:16:09.000000 autolens-2023.7.7.2/docs/general/configs.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1313 2021-08-21 09:36:01.000000 autolens-2023.7.7.2/docs/general/credits.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7996 2023-06-03 08:42:12.000000 autolens-2023.7.7.2/docs/general/demagnified_solutions.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.497528 autolens-2023.7.7.2/docs/general/images/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   294534 2022-07-16 16:37:21.000000 autolens-2023.7.7.2/docs/general/images/maresca_fig1.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   544260 2022-07-16 16:37:21.000000 autolens-2023.7.7.2/docs/general/images/maresca_fig2.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   202096 2022-07-16 16:37:21.000000 autolens-2023.7.7.2/docs/general/images/maresca_fig7.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      979 2022-05-03 11:39:22.000000 autolens-2023.7.7.2/docs/general/likelihood_function.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13858 2023-03-29 13:46:46.000000 autolens-2023.7.7.2/docs/general/model_cookbook.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4664 2023-04-24 16:24:52.000000 autolens-2023.7.7.2/docs/general/papers.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2702 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/docs/general/workspace.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.510527 autolens-2023.7.7.2/docs/howtolens/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2528 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/docs/howtolens/chapter_1_introduction.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2305 2022-08-01 13:03:47.000000 autolens-2023.7.7.2/docs/howtolens/chapter_2_lens_modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1831 2022-04-18 16:40:35.000000 autolens-2023.7.7.2/docs/howtolens/chapter_3_search_chaining.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2870 2023-06-01 19:03:35.000000 autolens-2023.7.7.2/docs/howtolens/chapter_4_pixelizations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      657 2021-08-21 09:36:11.000000 autolens-2023.7.7.2/docs/howtolens/chapter_optional.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3988 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/docs/howtolens/howtolens.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10685 2023-06-04 13:19:09.000000 autolens-2023.7.7.2/docs/index.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.522527 autolens-2023.7.7.2/docs/installation/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3972 2022-12-15 09:24:56.000000 autolens-2023.7.7.2/docs/installation/conda.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3525 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/docs/installation/numba.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2443 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/docs/installation/overview.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3410 2022-12-15 09:24:56.000000 autolens-2023.7.7.2/docs/installation/pip.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4984 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/docs/installation/source.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2840 2023-01-14 16:37:15.000000 autolens-2023.7.7.2/docs/installation/troubleshooting.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.542528 autolens-2023.7.7.2/docs/overview/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.237527 autolens-2023.7.7.2/docs/overview/images/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.545758 autolens-2023.7.7.2/docs/overview/images/clusters/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   318153 2021-08-21 09:36:01.000000 autolens-2023.7.7.2/docs/overview/images/clusters/cluster.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.580527 autolens-2023.7.7.2/docs/overview/images/fitting/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    72357 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/bad_chi_squared_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   111397 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/bad_normalized_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    98136 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/bad_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    91304 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/chi_squared_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    54590 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    61586 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/masked_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    64844 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/model_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    76236 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/noise_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   124025 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/normalized_residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30348 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/psf.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   113085 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/residual_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   375168 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/subplot_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    57718 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/fitting/tracer_image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.582528 autolens-2023.7.7.2/docs/overview/images/groups/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    97053 2021-08-21 09:36:01.000000 autolens-2023.7.7.2/docs/overview/images/groups/image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.611043 autolens-2023.7.7.2/docs/overview/images/interferometry/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41942 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/chi_squared_map_imag.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    46412 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/chi_squared_map_real.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   140414 2022-04-18 16:53:09.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   123013 2022-04-18 16:53:09.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/dirty_signal_to_noise.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   541388 2022-04-18 16:03:47.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/fit_dirty_images.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    97404 2022-04-18 16:55:25.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/image_pre_ft.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45276 2022-04-18 16:03:46.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/model_visibilities.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41124 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/residual_map_imag.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    45680 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/residual_map_real.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29898 2022-04-18 16:53:09.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/uv_wavelengths.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30858 2022-04-18 16:53:09.000000 autolens-2023.7.7.2/docs/overview/images/interferometry/visibilities.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.635065 autolens-2023.7.7.2/docs/overview/images/lensing/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    59062 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/complex_source.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    28199 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/grid.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    43370 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/isothermal_mass_profile_convergence.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    50440 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/isothermal_mass_profile_deflections_x.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    50354 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/isothermal_mass_profile_deflections_y.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    50181 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/isothermal_mass_profile_potential.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   400067 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/schematic.jpg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32399 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/sersic_light_profile.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    58721 2020-11-11 17:15:07.000000 autolens-2023.7.7.2/docs/overview/images/lensing/tracer_image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.637043 autolens-2023.7.7.2/docs/overview/images/modeling/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1516307 2021-08-21 09:36:01.000000 autolens-2023.7.7.2/docs/overview/images/modeling/cornerplot.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.647551 autolens-2023.7.7.2/docs/overview/images/multiwavelength/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    88546 2022-04-22 12:33:05.000000 autolens-2023.7.7.2/docs/overview/images/multiwavelength/dirty_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    49979 2022-04-22 12:34:38.000000 autolens-2023.7.7.2/docs/overview/images/multiwavelength/g_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38512 2022-04-22 12:34:38.000000 autolens-2023.7.7.2/docs/overview/images/multiwavelength/r_image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.664551 autolens-2023.7.7.2/docs/overview/images/pixelizations/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    70438 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/pixelizations/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    66987 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/pixelizations/reconstructed_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   124125 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/pixelizations/rectangular.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   289664 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/pixelizations/voronoi.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   911846 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/pixelizations/voronoi_fit.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   463891 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/pixelizations/voronoi_fit_plane_1.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.668551 autolens-2023.7.7.2/docs/overview/images/point_sources/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36445 2021-08-21 09:36:01.000000 autolens-2023.7.7.2/docs/overview/images/point_sources/image.png
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.685567 autolens-2023.7.7.2/docs/overview/images/simulating/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   196067 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/ao_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35458 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/euclid_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    56736 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/hst_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48477 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    70333 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/noise_map.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30341 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/psf.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    33987 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/docs/overview/images/simulating/vro_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5850 2023-06-03 08:54:22.000000 autolens-2023.7.7.2/docs/overview/overview_10_clusters.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9869 2023-06-03 08:55:28.000000 autolens-2023.7.7.2/docs/overview/overview_1_lensing.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5564 2023-06-03 08:51:27.000000 autolens-2023.7.7.2/docs/overview/overview_2_fitting.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    23775 2023-06-03 08:58:48.000000 autolens-2023.7.7.2/docs/overview/overview_3_modeling.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3100 2023-06-03 09:00:29.000000 autolens-2023.7.7.2/docs/overview/overview_4_simulate.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4256 2023-06-03 08:42:12.000000 autolens-2023.7.7.2/docs/overview/overview_5_pixelizations.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8439 2023-06-03 12:30:35.000000 autolens-2023.7.7.2/docs/overview/overview_6_interferometry.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11468 2023-06-03 09:10:23.000000 autolens-2023.7.7.2/docs/overview/overview_7_multi_wavelength.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7843 2023-06-03 09:10:24.000000 autolens-2023.7.7.2/docs/overview/overview_8_point_sources.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4579 2023-06-03 08:54:21.000000 autolens-2023.7.7.2/docs/overview/overview_9_groups.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      150 2022-12-14 15:52:59.000000 autolens-2023.7.7.2/docs/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       31 2022-04-26 16:24:37.000000 autolens-2023.7.7.2/eden.ini
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.700551 autolens-2023.7.7.2/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    29338 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/files/citations.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1787 2023-01-28 10:33:10.000000 autolens-2023.7.7.2/files/citations.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2398 2023-01-28 10:34:47.000000 autolens-2023.7.7.2/files/citations.tex
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    87075 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/files/image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   395739 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/files/imageaxis.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   363152 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/files/imagenoaxis.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    75357 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/files/model_image.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   202826 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/files/reconstruction.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      176 2020-11-17 10:41:27.000000 autolens-2023.7.7.2/libraries.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      111 2023-06-03 19:29:54.000000 autolens-2023.7.7.2/optional_requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:59:22.711552 autolens-2023.7.7.2/paper/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      188 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/paper/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   395739 2020-11-11 17:15:08.000000 autolens-2023.7.7.2/paper/imageaxis.png
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    75916 2023-05-23 09:39:19.000000 autolens-2023.7.7.2/paper/paper.bib
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      826 2022-02-14 09:21:43.000000 autolens-2023.7.7.2/paper/paper.json
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14346 2022-09-30 11:20:01.000000 autolens-2023.7.7.2/paper/paper.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      175 2022-10-10 12:28:19.000000 autolens-2023.7.7.2/readthedocs.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      545 2021-02-12 14:30:10.000000 autolens-2023.7.7.2/release.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-05-03 10:57:57.000000 autolens-2023.7.7.2/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-06-07 09:59:22.715563 autolens-2023.7.7.2/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2014 2023-06-07 09:57:48.000000 autolens-2023.7.7.2/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3552 2022-12-08 17:52:44.000000 autolens-2023.7.7.2/to_do_list
```

### Comparing `autolens-2023.6.12.4/CITATIONS.rst` & `autolens-2023.7.7.2/CITATIONS.rst`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/LICENSE` & `autolens-2023.7.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/PKG-INFO` & `autolens-2023.7.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autolens
-Version: 2023.6.12.4
+Version: 2023.7.7.2
 Summary: Open-Source Strong Lensing
 Home-page: https://github.com/Jammy2211/PyAutoLens
 Author: James Nightingale and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
@@ -62,18 +62,18 @@
 This is called strong gravitational lensing and **PyAutoLens** makes it simple to model strong gravitational lenses.
 
 Getting Started
 ---------------
 
 The following links are useful for new starters:
 
-- `The PyAutoLens readthedocs <https://pyautolens.readthedocs.io/en/latest>`_, which includes `an installation guide <https://pyautolens.readthedocs.io/en/latest/installation/overview.html>`_ and an `overview of **PyAutoLens**'s core features <https://pyautolens.readthedocs.io/en/latest/overview/overview_1_lensing.html>`_.
-
 - `The introduction Jupyter Notebook on Binder <https://mybinder.org/v2/gh/Jammy2211/autolens_workspace/release?filepath=introduction.ipynb>`_, where you can try **PyAutoLens** in a web browser (without installation).
 
+- `The PyAutoLens readthedocs <https://pyautolens.readthedocs.io/en/latest>`_, which includes `an installation guide <https://pyautolens.readthedocs.io/en/latest/installation/overview.html>`_ and an overview of **PyAutoLens**'s core features.
+
 - `The autolens_workspace GitHub repository <https://github.com/Jammy2211/autolens_workspace>`_, which includes example scripts and the `HowToLens Jupyter notebook tutorials <https://github.com/Jammy2211/autolens_workspace/tree/master/notebooks/howtolens>`_ which give new users a step-by-step introduction to **PyAutoLens**.
 
 API Overview
 ------------
 
 Lensing calculations are performed in **PyAutoLens** by building a ``Tracer`` object from ``LightProfile``,
 ``MassProfile`` and ``Galaxy`` objects. Below, we create a simple strong lens system where a redshift 0.5
```

### Comparing `autolens-2023.6.12.4/README.rst` & `autolens-2023.7.7.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -41,18 +41,18 @@
 This is called strong gravitational lensing and **PyAutoLens** makes it simple to model strong gravitational lenses.
 
 Getting Started
 ---------------
 
 The following links are useful for new starters:
 
-- `The PyAutoLens readthedocs <https://pyautolens.readthedocs.io/en/latest>`_, which includes `an installation guide <https://pyautolens.readthedocs.io/en/latest/installation/overview.html>`_ and an `overview of **PyAutoLens**'s core features <https://pyautolens.readthedocs.io/en/latest/overview/overview_1_lensing.html>`_.
-
 - `The introduction Jupyter Notebook on Binder <https://mybinder.org/v2/gh/Jammy2211/autolens_workspace/release?filepath=introduction.ipynb>`_, where you can try **PyAutoLens** in a web browser (without installation).
 
+- `The PyAutoLens readthedocs <https://pyautolens.readthedocs.io/en/latest>`_, which includes `an installation guide <https://pyautolens.readthedocs.io/en/latest/installation/overview.html>`_ and an overview of **PyAutoLens**'s core features.
+
 - `The autolens_workspace GitHub repository <https://github.com/Jammy2211/autolens_workspace>`_, which includes example scripts and the `HowToLens Jupyter notebook tutorials <https://github.com/Jammy2211/autolens_workspace/tree/master/notebooks/howtolens>`_ which give new users a step-by-step introduction to **PyAutoLens**.
 
 API Overview
 ------------
 
 Lensing calculations are performed in **PyAutoLens** by building a ``Tracer`` object from ``LightProfile``,
 ``MassProfile`` and ``Galaxy`` objects. Below, we create a simple strong lens system where a redshift 0.5
```

### Comparing `autolens-2023.6.12.4/autolens/__init__.py` & `autolens-2023.7.7.2/autolens/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,8 +110,8 @@
 from . import mock as m
 from . import util
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2023.6.12.4"
+__version__ = "2023.7.7.2"
```

### Comparing `autolens-2023.6.12.4/autolens/aggregator/__init__.py` & `autolens-2023.7.7.2/autolens/aggregator/__init__.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/aggregator/fit_imaging.py` & `autolens-2023.7.7.2/autolens/aggregator/fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/aggregator/fit_interferometer.py` & `autolens-2023.7.7.2/autolens/aggregator/fit_interferometer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/aggregator/subhalo.py` & `autolens-2023.7.7.2/autolens/aggregator/subhalo.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/aggregator/tracer.py` & `autolens-2023.7.7.2/autolens/aggregator/tracer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/analysis/analysis.py` & `autolens-2023.7.7.2/autolens/analysis/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,21 +63,21 @@
         self.cosmology = cosmology
         self.settings_lens = settings_lens or SettingsLens()
         self.positions_likelihood = positions_likelihood
 
     def tracer_via_instance_from(
         self,
         instance: af.ModelInstance,
-        run_time_dict: Optional[Dict] = None,
+        profiling_dict: Optional[Dict] = None,
         tracer_cls=Tracer,
     ) -> Tracer:
         """
         Create a `Tracer` from the galaxies contained in a model instance.
 
-        If PyAutoFit's profiling tools are used with the analsyis class, this function may receive a `run_time_dict`
+        If PyAutoFit's profiling tools are used with the analsyis class, this function may receive a `profiling_dict`
         which times how long each set of the model-fit takes to perform.
 
         Parameters
         ----------
         instance
             An instance of the model that is fitted to the data by this analysis (whose parameters may have been set
             via a non-linear search).
@@ -103,26 +103,26 @@
 
             instance.galaxies.subhalo.mass.centre = tuple(subhalo_centre.in_list[0])
 
         if hasattr(instance, "clumps"):
             return Tracer.from_galaxies(
                 galaxies=instance.galaxies + instance.clumps,
                 cosmology=self.cosmology,
-                run_time_dict=run_time_dict,
+                profiling_dict=profiling_dict,
             )
 
         if hasattr(instance, "cosmology"):
             cosmology = instance.cosmology
         else:
             cosmology = self.cosmology
 
         return tracer_cls.from_galaxies(
             galaxies=instance.galaxies,
             cosmology=cosmology,
-            run_time_dict=run_time_dict,
+            profiling_dict=profiling_dict,
         )
 
     def log_likelihood_positions_overwrite_from(
         self, instance: af.ModelInstance
     ) -> Optional[float]:
         """
         Call the positions overwrite log likelihood function, which add a penalty term to the likelihood if the
```

### Comparing `autolens-2023.6.12.4/autolens/analysis/mock/mock_result.py` & `autolens-2023.7.7.2/autolens/analysis/mock/mock_result.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/analysis/positions.py` & `autolens-2023.7.7.2/autolens/analysis/positions.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/analysis/preloads.py` & `autolens-2023.7.7.2/autolens/analysis/preloads.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/analysis/result.py` & `autolens-2023.7.7.2/autolens/analysis/result.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/analysis/setup.py` & `autolens-2023.7.7.2/autolens/analysis/setup.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/analysis/visualizer.py` & `autolens-2023.7.7.2/autolens/analysis/visualizer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/config/non_linear.yaml` & `autolens-2023.7.7.2/autolens/config/non_linear.yaml`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/config/visualize/plots.yaml` & `autolens-2023.7.7.2/autolens/config/visualize/plots.yaml`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/exc.py` & `autolens-2023.7.7.2/autolens/exc.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/fixtures.py` & `autolens-2023.7.7.2/autolens/fixtures.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/imaging/fit_imaging.py` & `autolens-2023.7.7.2/autolens/imaging/fit_imaging.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def __init__(
         self,
         dataset: aa.Imaging,
         tracer: Tracer,
         settings_pixelization: aa.SettingsPixelization = aa.SettingsPixelization(),
         settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
         preloads: Preloads = Preloads(),
-        run_time_dict: Optional[Dict] = None,
+        profiling_dict: Optional[Dict] = None,
     ):
         """
         Fits an imaging dataset using a `Tracer` object.
 
         The fit performs the following steps:
 
         1) Compute the sum of all images of galaxy light profiles in the `Tracer`.
@@ -59,20 +59,20 @@
             Settings controlling how a pixelization is fitted for example if a border is used when creating the
             pixelization.
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
         preloads
             Contains preloaded calculations (e.g. linear algebra matrices) which can skip certain calculations in
             the fit.
-        run_time_dict
+        profiling_dict
             A dictionary which if passed to the fit records how long fucntion calls which have the `profile_func`
             decorator take to run.
         """
 
-        super().__init__(dataset=dataset, run_time_dict=run_time_dict)
+        super().__init__(dataset=dataset, profiling_dict=profiling_dict)
         AbstractFitInversion.__init__(
             self=self, model_obj=tracer, settings_inversion=settings_inversion
         )
 
         self.tracer = tracer
 
         self.settings_pixelization = settings_pixelization
@@ -303,23 +303,23 @@
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
 
         Returns
         -------
         A new fit which has used new preloads input into this function but the same dataset, tracer and other settings.
         """
-        run_time_dict = {} if self.run_time_dict is not None else None
+        profiling_dict = {} if self.profiling_dict is not None else None
 
         settings_inversion = (
             self.settings_inversion
             if settings_inversion is None
             else settings_inversion
         )
 
         return FitImaging(
             dataset=self.dataset,
             tracer=self.tracer,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=settings_inversion,
             preloads=preloads,
-            run_time_dict=run_time_dict,
+            profiling_dict=profiling_dict,
         )
```

### Comparing `autolens-2023.6.12.4/autolens/imaging/imaging.py` & `autolens-2023.7.7.2/autolens/imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/imaging/mock/mock_fit_imaging.py` & `autolens-2023.7.7.2/autolens/imaging/mock/mock_fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/imaging/model/analysis.py` & `autolens-2023.7.7.2/autolens/imaging/model/analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+import json
 import logging
 import numpy as np
-from typing import Dict, Optional, Tuple
+import os
+import time
+from typing import Dict, Optional
+from os import path
 
+from autoconf import conf
 import autofit as af
 import autogalaxy as ag
 
 from autoarray.exc import PixelizationException
 
 from autolens.analysis.analysis import AnalysisDataset
 from autolens.analysis.preloads import Preloads
@@ -123,15 +128,15 @@
         ) as e:
             raise exc.FitException from e
 
     def fit_imaging_via_instance_from(
         self,
         instance: af.ModelInstance,
         preload_overwrite: Optional[Preloads] = None,
-        run_time_dict: Optional[Dict] = None,
+        profiling_dict: Optional[Dict] = None,
     ) -> FitImaging:
         """
         Given a model instance create a `FitImaging` object.
 
         This function is used in the `log_likelihood_function` to fit the model to the imaging data and compute the
         log likelihood.
 
@@ -141,52 +146,52 @@
             An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
             via a non-linear search).
         preload_overwrite
             If a `Preload` object is input this is used instead of the preloads stored as an attribute in the analysis.
         check_positions
             Whether the multiple image positions of the lensed source should be checked, i.e. whether they trace
             within the position threshold of one another in the source plane.
-        run_time_dict
+        profiling_dict
             A dictionary which times functions called to fit the model to data, for profiling.
 
         Returns
         -------
         FitImaging
             The fit of the plane to the imaging dataset, which includes the log likelihood.
         """
         self.instance_with_associated_adapt_images_from(instance=instance)
         tracer = self.tracer_via_instance_from(
-            instance=instance, run_time_dict=run_time_dict
+            instance=instance, profiling_dict=profiling_dict
         )
 
         return self.fit_imaging_via_tracer_from(
             tracer=tracer,
             preload_overwrite=preload_overwrite,
-            run_time_dict=run_time_dict,
+            profiling_dict=profiling_dict,
         )
 
     def fit_imaging_via_tracer_from(
         self,
         tracer: Tracer,
         preload_overwrite: Optional[Preloads] = None,
-        run_time_dict: Optional[Dict] = None,
+        profiling_dict: Optional[Dict] = None,
     ) -> FitImaging:
         """
         Given a `Tracer`, which the analysis constructs from a model instance, create a `FitImaging` object.
 
         This function is used in the `log_likelihood_function` to fit the model to the imaging data and compute the
         log likelihood.
 
         Parameters
         ----------
         tracer
             The tracer of galaxies whose ray-traced model images are used to fit the imaging data.
         preload_overwrite
             If a `Preload` object is input this is used instead of the preloads stored as an attribute in the analysis.
-        run_time_dict
+        profiling_dict
             A dictionary which times functions called to fit the model to data, for profiling.
 
         Returns
         -------
         FitImaging
             The fit of the plane to the imaging dataset, which includes the log likelihood.
         """
@@ -194,21 +199,99 @@
 
         return FitImaging(
             dataset=self.dataset,
             tracer=tracer,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=self.settings_inversion,
             preloads=preloads,
-            run_time_dict=run_time_dict,
+            profiling_dict=profiling_dict,
         )
 
     @property
     def fit_func(self):
         return self.fit_imaging_via_instance_from
 
+    def profile_log_likelihood_function(
+        self, instance: af.ModelInstance, paths: Optional[af.DirectoryPaths] = None
+    ):
+        """
+        This function is optionally called throughout a model-fit to profile the log likelihood function.
+
+        All function calls inside the `log_likelihood_function` that are decorated with the `profile_func` are timed
+        with their times stored in a dictionary called the `profiling_dict`.
+
+        An `info_dict` is also created which stores information no aspects of the model and dataset that dictate
+        run times, so the profiled times can be interpreted with this context.
+
+        The results of this profiling are then output to hard-disk in the `preloads` folder of the model-fit results,
+        which they can be inspected to ensure run-times are as expected.
+
+        Parameters
+        ----------
+        instance
+            An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
+            via a non-linear search).
+        paths
+            The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
+            visualization and the pickled objects used by the aggregator output by this function.
+        """
+        profiling_dict = {}
+        info_dict = {}
+
+        repeats = conf.instance["general"]["profiling"]["repeats"]
+        info_dict["repeats"] = repeats
+
+        start = time.time()
+
+        for i in range(repeats):
+
+            try:
+                fit = self.fit_imaging_via_instance_from(instance=instance)
+                fit.figure_of_merit
+            except Exception:
+                logger.info("Profiling failed. Returning without outputting information.")
+                return
+
+        fit_time = (time.time() - start) / repeats
+
+        info_dict["fit_time"] = fit_time
+
+        fit = self.fit_imaging_via_instance_from(
+            instance=instance, profiling_dict=profiling_dict
+        )
+        fit.figure_of_merit
+
+        info_dict["image_pixels"] = self.dataset.grid.sub_shape_slim
+        info_dict["sub_size_light_profiles"] = self.dataset.grid.sub_size
+        info_dict["sub_size_pixelization"] = self.dataset.grid_pixelization.sub_size
+        info_dict["psf_shape_2d"] = self.dataset.psf.shape_native
+
+        if fit.inversion is not None:
+            info_dict["source_pixels"] = len(fit.inversion.reconstruction)
+
+        if hasattr(fit.inversion, "w_tilde"):
+            info_dict[
+                "w_tilde_curvature_preload_size"
+            ] = fit.inversion.w_tilde.curvature_preload.shape[0]
+
+        if paths is not None:
+
+            try:
+                os.makedirs(paths.profile_path)
+            except FileExistsError:
+                pass
+
+            with open(path.join(paths.profile_path, "profiling_dict.json"), "w+") as f:
+                json.dump(fit.profiling_dict, f, indent=4)
+
+            with open(path.join(paths.profile_path, "info_dict.json"), "w+") as f:
+                json.dump(info_dict, f, indent=4)
+
+        return profiling_dict
+
     def stochastic_log_likelihoods_via_instance_from(self, instance: af.ModelInstance):
         """
         Certain `Inversion`'s have stochasticity in their log likelihood estimate.
 
         For example, the `VoronoiBrightnessImage` pixelization, which changes the likelihood depending on how different
         KMeans seeds change the pixel-grid.
 
@@ -292,15 +375,15 @@
 
         visualizer = VisualizerImaging(visualize_path=paths.image_path)
 
         visualizer.visualize_imaging(dataset=self.dataset)
 
         if self.positions_likelihood is not None:
             visualizer.visualize_image_with_positions(
-                image=self.dataset.data,
+                image=self.dataset.image,
                 positions=self.positions_likelihood.positions,
             )
 
         visualizer.visualize_adapt_images(
             adapt_galaxy_image_path_dict=self.adapt_galaxy_image_path_dict,
             adapt_model_image=self.adapt_model_image,
         )
@@ -456,46 +539,7 @@
             visualization, and the pickled objects used by the aggregator output by this function.
         """
         super().save_attributes_for_aggregator(paths=paths)
 
         paths.save_object("psf", self.dataset.psf)
         paths.save_object("mask", self.dataset.mask)
         paths.save_object("positions_likelihood", self.positions_likelihood)
-
-    def profile_log_likelihood_function(
-        self, instance: af.ModelInstance, paths: Optional[af.DirectoryPaths] = None
-    ) -> Tuple[Dict, Dict]:
-        """
-        This function is optionally called throughout a model-fit to profile the log likelihood function.
-
-        All function calls inside the `log_likelihood_function` that are decorated with the `profile_func` are timed
-        with their times stored in a dictionary called the `run_time_dict`.
-
-        An `info_dict` is also created which stores information on aspects of the model and dataset that dictate
-        run times, so the profiled times can be interpreted with this context.
-
-        The results of this profiling are then output to hard-disk in the `preloads` folder of the model-fit results,
-        which they can be inspected to ensure run-times are as expected.
-
-        Parameters
-        ----------
-        instance
-            An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
-            via a non-linear search).
-        paths
-            The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
-            visualization and the pickled objects used by the aggregator output by this function.
-
-        Returns
-        -------
-        Two dictionaries, the profiling dictionary and info dictionary, which contain the profiling times of the
-        `log_likelihood_function` and information on the model and dataset used to perform the profiling.
-        """
-        run_time_dict, info_dict = super().profile_log_likelihood_function(
-            instance=instance,
-        )
-
-        info_dict["psf_shape_2d"] = self.dataset.psf.shape_native
-
-        self.output_profiling_info(paths=paths, run_time_dict=run_time_dict, info_dict=info_dict)
-
-        return run_time_dict, info_dict
```

### Comparing `autolens-2023.6.12.4/autolens/imaging/model/result.py` & `autolens-2023.7.7.2/autolens/imaging/model/result.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/imaging/model/visualizer.py` & `autolens-2023.7.7.2/autolens/imaging/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/imaging/plot/fit_imaging_plotters.py` & `autolens-2023.7.7.2/autolens/imaging/plot/fit_imaging_plotters.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,14 @@
             inversion=self.fit.inversion,
             mat_plot_2d=self.mat_plot_2d,
             visuals_2d=self.tracer_plotter.get_visuals_2d_of_plane(
                 plane_index=plane_index
             ),
             include_2d=self.include_2d,
         )
-        inversion_plotter.visuals_2d.mask = None
         inversion_plotter.visuals_2d.border = None
         return inversion_plotter
 
     def plane_indexes_from(self, plane_index: int):
         """
         Returns a list of all indexes of the planes in the fit, which is iterated over in figures that plot
         individual figures of each plane in a tracer.
@@ -234,15 +233,14 @@
                     )
 
                 elif self.tracer.planes[plane_index].has(cls=aa.Pixelization):
 
                     inversion_plotter = self.inversion_plotter_of_plane(
                         plane_index=plane_index
                     )
-
                     inversion_plotter.figures_2d_of_pixelization(
                         pixelization_index=0,
                         reconstruction=True,
                         zoom_to_brightest=zoom_to_brightest,
                         interpolate_to_uniform=interpolate_to_uniform
                     )
 
@@ -457,15 +455,15 @@
 
             if use_source_vmax:
                 self.mat_plot_2d.cmap.kwargs["vmax"] = np.max(self.fit.model_images_of_planes_list[-1])
 
             self.mat_plot_2d.plot_array(
                 array=self.fit.data,
                 visuals_2d=visuals_2d_no_critical_caustic,
-                auto_labels=AutoLabels(title="Data", filename=f"data{suffix}"),
+                auto_labels=AutoLabels(title="Image", filename=f"data{suffix}"),
             )
 
             if use_source_vmax:
                 self.mat_plot_2d.cmap.kwargs.pop("vmax")
 
         if noise_map:
```

### Comparing `autolens-2023.6.12.4/autolens/interferometer/fit_interferometer.py` & `autolens-2023.7.7.2/autolens/interferometer/fit_interferometer.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def __init__(
         self,
         dataset: aa.Interferometer,
         tracer: Tracer,
         settings_pixelization: aa.SettingsPixelization = aa.SettingsPixelization(),
         settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
         preloads: Preloads = Preloads(),
-        run_time_dict: Optional[Dict] = None,
+        profiling_dict: Optional[Dict] = None,
     ):
         """
         Fits an interferometer dataset using a `Tracer` object.
 
         The fit performs the following steps:
 
         1) Compute the sum of all images of galaxy light profiles in the `Tracer`.
@@ -58,15 +58,15 @@
             Settings controlling how a pixelization is fitted for example if a border is used when creating the
             pixelization.
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
         preloads
             Contains preloaded calculations (e.g. linear algebra matrices) which can skip certain calculations in
             the fit.
-        run_time_dict
+        profiling_dict
             A dictionary which if passed to the fit records how long fucntion calls which have the `profile_func`
             decorator take to run.
         """
 
         try:
             from autoarray.inversion.inversion import inversion_util_secret
         except ImportError:
@@ -75,17 +75,17 @@
         self.tracer = tracer
 
         self.settings_pixelization = settings_pixelization
         self.settings_inversion = settings_inversion
 
         self.preloads = preloads
 
-        self.run_time_dict = run_time_dict
+        self.profiling_dict = profiling_dict
 
-        super().__init__(dataset=dataset, run_time_dict=run_time_dict)
+        super().__init__(dataset=dataset, profiling_dict=profiling_dict)
         AbstractFitInversion.__init__(
             self=self, model_obj=tracer, settings_inversion=settings_inversion
         )
 
     @property
     def profile_visibilities(self) -> aa.Visibilities:
         """
@@ -253,23 +253,23 @@
         settings_inversion
             Settings controlling how an inversion is fitted for example which linear algebra formalism is used.
 
         Returns
         -------
         A new fit which has used new preloads input into this function but the same dataset, tracer and other settings.
         """
-        if self.run_time_dict is not None:
-            run_time_dict = {}
+        if self.profiling_dict is not None:
+            profiling_dict = {}
         else:
-            run_time_dict = None
+            profiling_dict = None
 
         if settings_inversion is None:
             settings_inversion = self.settings_inversion
 
         return FitInterferometer(
             dataset=self.interferometer,
             tracer=self.tracer,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=settings_inversion,
             preloads=preloads,
-            run_time_dict=run_time_dict,
+            profiling_dict=profiling_dict,
         )
```

### Comparing `autolens-2023.6.12.4/autolens/interferometer/interferometer.py` & `autolens-2023.7.7.2/autolens/interferometer/interferometer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/interferometer/model/analysis.py` & `autolens-2023.7.7.2/autolens/interferometer/model/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import numpy as np
-from typing import Dict, Optional, Tuple, Union
+import os
+from typing import Optional, Union
 
 import autofit as af
 import autoarray as aa
 import autogalaxy as ag
 
 from autoarray.exc import PixelizationException
 
@@ -188,15 +189,15 @@
             OverflowError,
         ) as e:
             raise exc.FitException from e
 
     def fit_interferometer_via_instance_from(
         self,
         instance: af.ModelInstance,
-        run_time_dict: Optional[Dict] = None,
+        preload_overwrite: Optional[Preloads] = None,
     ) -> FitInterferometer:
         """
         Given a model instance create a `FitInterferometer` object.
 
         This function is used in the `log_likelihood_function` to fit the model to the interferometer data and compute
         the log likelihood.
 
@@ -206,50 +207,47 @@
             An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
             via a non-linear search).
         preload_overwrite
             If a `Preload` object is input this is used instead of the preloads stored as an attribute in the analysis.
         check_positions
             Whether the multiple image positions of the lensed source should be checked, i.e. whether they trace
             within the position threshold of one another in the source plane.
-        run_time_dict
+        profiling_dict
             A dictionary which times functions called to fit the model to data, for profiling.
 
         Returns
         -------
         FitInterferometer
             The fit of the plane to the interferometer dataset, which includes the log likelihood.
         """
         self.instance_with_associated_adapt_images_from(instance=instance)
-        tracer = self.tracer_via_instance_from(
-            instance=instance, run_time_dict=run_time_dict
-        )
+        tracer = self.tracer_via_instance_from(instance=instance)
 
         return self.fit_interferometer_via_tracer_from(
-            tracer=tracer, run_time_dict=run_time_dict
+            tracer=tracer,
         )
 
     def fit_interferometer_via_tracer_from(
         self,
         tracer: Tracer,
         preload_overwrite: Optional[Preloads] = None,
-        run_time_dict: Optional[Dict] = None,
     ):
         """
         Given a `Tracer`, which the analysis constructs from a model instance, create a `FitInterferometer` object.
 
         This function is used in the `log_likelihood_function` to fit the model to the imaging data and compute the
         log likelihood.
 
         Parameters
         ----------
         tracer
             The tracer of galaxies whose ray-traced model images are used to fit the imaging data.
         preload_overwrite
             If a `Preload` object is input this is used instead of the preloads stored as an attribute in the analysis.
-        run_time_dict
+        profiling_dict
             A dictionary which times functions called to fit the model to data, for profiling.
 
         Returns
         -------
         FitImaging
             The fit of the plane to the imaging dataset, which includes the log likelihood.
         """
@@ -257,15 +255,14 @@
 
         return FitInterferometer(
             dataset=self.dataset,
             tracer=tracer,
             settings_pixelization=self.settings_pixelization,
             settings_inversion=self.settings_inversion,
             preloads=preloads,
-            run_time_dict=run_time_dict,
         )
 
     @property
     def fit_func(self):
         return self.fit_interferometer_via_instance_from
 
     def stochastic_log_likelihoods_via_instance_from(self, instance):
@@ -527,49 +524,7 @@
         paths.save_object("real_space_mask", self.dataset.real_space_mask)
         paths.save_object("positions_likelihood", self.positions_likelihood)
         if self.preloads.sparse_image_plane_grid_pg_list is not None:
             paths.save_object(
                 "preload_sparse_grids_of_planes",
                 self.preloads.sparse_image_plane_grid_pg_list,
             )
-
-    def profile_log_likelihood_function(
-        self, instance: af.ModelInstance, paths: Optional[af.DirectoryPaths] = None
-    ) -> Tuple[Dict, Dict]:
-        """
-        This function is optionally called throughout a model-fit to profile the log likelihood function.
-
-        All function calls inside the `log_likelihood_function` that are decorated with the `profile_func` are timed
-        with their times stored in a dictionary called the `run_time_dict`.
-
-        An `info_dict` is also created which stores information on aspects of the model and dataset that dictate
-        run times, so the profiled times can be interpreted with this context.
-
-        The results of this profiling are then output to hard-disk in the `preloads` folder of the model-fit results,
-        which they can be inspected to ensure run-times are as expected.
-
-        Parameters
-        ----------
-        instance
-            An instance of the model that is being fitted to the data by this analysis (whose parameters have been set
-            via a non-linear search).
-        paths
-            The PyAutoFit paths object which manages all paths, e.g. where the non-linear search outputs are stored,
-            visualization and the pickled objects used by the aggregator output by this function.
-
-        Returns
-        -------
-        Two dictionaries, the profiling dictionary and info dictionary, which contain the profiling times of the
-        `log_likelihood_function` and information on the model and dataset used to perform the profiling.
-        """
-        run_time_dict, info_dict = super().profile_log_likelihood_function(
-            instance=instance,
-        )
-
-        info_dict["number_of_visibilities"] = self.dataset.visibilities.shape[0]
-        info_dict["transformer_cls"] = self.dataset.transformer.__class__.__name__
-
-        self.output_profiling_info(
-            paths=paths, run_time_dict=run_time_dict, info_dict=info_dict
-        )
-
-        return run_time_dict, info_dict
```

### Comparing `autolens-2023.6.12.4/autolens/interferometer/model/result.py` & `autolens-2023.7.7.2/autolens/interferometer/model/result.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/interferometer/model/visualizer.py` & `autolens-2023.7.7.2/autolens/interferometer/model/visualizer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/interferometer/plot/fit_interferometer_plotters.py` & `autolens-2023.7.7.2/autolens/interferometer/plot/fit_interferometer_plotters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional
 
 import autoarray as aa
+import autogalaxy as ag
 import autogalaxy.plot as aplt
 
 from autoarray.fit.plot.fit_interferometer_plotters import FitInterferometerPlotterMeta
 
 from autolens.interferometer.fit_interferometer import FitInterferometer
 from autolens.lens.ray_tracing import Tracer
 from autolens.lens.plot.ray_tracing_plotters import TracerPlotter
@@ -270,22 +271,18 @@
             dirty_model_image=dirty_model_image,
             dirty_residual_map=dirty_residual_map,
             dirty_normalized_residual_map=dirty_normalized_residual_map,
             dirty_chi_squared_map=dirty_chi_squared_map,
         )
 
         if image:
-            plane_index = len(self.tracer.planes) - 1
-
-            if not self.tracer.planes[plane_index].has(cls=aa.Pixelization):
+            if self.fit.inversion is None:
                 self.tracer_plotter.figures_2d(image=True)
-            elif self.tracer.planes[plane_index].has(cls=aa.Pixelization):
-                inversion_plotter = self.inversion_plotter_of_plane(
-                    plane_index=plane_index
-                )
+            else:
+                inversion_plotter = self.inversion_plotter_of_plane(plane_index=1)
                 inversion_plotter.figures_2d(reconstructed_image=True)
 
     def figures_2d_of_planes(
         self,
         plane_index: Optional[int] = None,
         plane_image: bool = False,
         zoom_to_brightest: bool = True,
```

### Comparing `autolens-2023.6.12.4/autolens/lens/mock/mock_tracer.py` & `autolens-2023.7.7.2/autolens/lens/mock/mock_tracer.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/lens/plot/ray_tracing_plotters.py` & `autolens-2023.7.7.2/autolens/lens/plot/ray_tracing_plotters.py`

 * *Files 3% similar despite different names*

```diff
@@ -231,34 +231,27 @@
             the brightest regions of the galaxies being plotted as opposed to the full extent of the grid.
         """
         plane_indexes = self.plane_indexes_from(plane_index=plane_index)
 
         for plane_index in plane_indexes:
             plane_plotter = self.plane_plotter_from(plane_index=plane_index)
 
-            if plane_index == 1:
-                source_plane_title = True
-            else:
-                source_plane_title = False
-
             if plane_image:
                 plane_plotter.figures_2d(
                     plane_image=True,
                     zoom_to_brightest=zoom_to_brightest,
                     title_suffix=f" Of Plane {plane_index}",
                     filename_suffix=f"_of_plane_{plane_index}",
-                    source_plane_title=source_plane_title,
                 )
 
             if plane_grid:
                 plane_plotter.figures_2d(
                     plane_grid=True,
                     title_suffix=f" Of Plane {plane_index}",
                     filename_suffix=f"_of_plane_{plane_index}",
-                    source_plane_title=source_plane_title,
                 )
 
     def subplot(
         self,
         image: bool = False,
         source_plane: bool = False,
         convergence: bool = False,
```

### Comparing `autolens-2023.6.12.4/autolens/lens/ray_tracing.py` & `autolens-2023.7.7.2/autolens/lens/ray_tracing.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class Tracer(ABC, ag.OperateImageGalaxies, ag.OperateDeflections, Dictable):
     def __init__(
         self,
         planes,
         cosmology: ag.cosmo.LensingCosmology,
-        run_time_dict: Optional[Dict] = None,
+        profiling_dict: Optional[Dict] = None,
     ):
         """
         Ray-tracer for a lens system with any number of planes.
 
         The redshift of these planes are specified by the redshits of the galaxies; there is a unique plane redshift \
         for every unique galaxy redshift (galaxies with identical redshifts are put in the same plane).
 
@@ -44,28 +44,28 @@
         cosmology : astropy.cosmology
             The cosmology of the ray-tracing calculation.
         """
         self.planes = planes
         self.plane_redshifts = [plane.redshift for plane in planes]
         self.cosmology = cosmology
 
-        self.run_time_dict = run_time_dict
+        self.profiling_dict = profiling_dict
 
     @classmethod
     def from_galaxies(
         cls,
         galaxies,
         cosmology: ag.cosmo.LensingCosmology = ag.cosmo.Planck15(),
-        run_time_dict: Optional[Dict] = None,
+        profiling_dict: Optional[Dict] = None,
     ):
         planes = ag.util.plane.planes_via_galaxies_from(
-            galaxies=galaxies, run_time_dict=run_time_dict
+            galaxies=galaxies, profiling_dict=profiling_dict
         )
 
-        return cls(planes=planes, cosmology=cosmology, run_time_dict=run_time_dict)
+        return cls(planes=planes, cosmology=cosmology, profiling_dict=profiling_dict)
 
     @classmethod
     def sliced_tracer_from(
         cls,
         lens_galaxies,
         line_of_sight_galaxies,
         source_galaxies,
```

### Comparing `autolens-2023.6.12.4/autolens/lens/ray_tracing_util.py` & `autolens-2023.7.7.2/autolens/lens/ray_tracing_util.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/lens/subhalo.py` & `autolens-2023.7.7.2/autolens/lens/subhalo.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/lens/to_inversion.py` & `autolens-2023.7.7.2/autolens/lens/to_inversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,27 +17,27 @@
         dataset: Optional[Union[aa.Imaging, aa.Interferometer]] = None,
         data: Optional[Union[aa.Array2D, aa.Visibilities]] = None,
         noise_map: Optional[Union[aa.Array2D, aa.VisibilitiesNoiseMap]] = None,
         w_tilde: Optional[Union[aa.WTildeImaging, aa.WTildeInterferometer]] = None,
         settings_pixelization=aa.SettingsPixelization(),
         settings_inversion: aa.SettingsInversion = aa.SettingsInversion(),
         preloads=Preloads(),
-        run_time_dict: Optional[Dict] = None,
+        profiling_dict: Optional[Dict] = None,
     ):
         self.tracer = tracer
 
         super().__init__(
             dataset=dataset,
             data=data,
             noise_map=noise_map,
             w_tilde=w_tilde,
             settings_pixelization=settings_pixelization,
             settings_inversion=settings_inversion,
             preloads=preloads,
-            run_time_dict=run_time_dict,
+            profiling_dict=profiling_dict,
         )
 
     @property
     def planes(self):
         return self.tracer.planes
 
     @cached_property
@@ -231,13 +231,13 @@
             dataset=self.dataset,
             data=self.data,
             noise_map=self.noise_map,
             w_tilde=self.w_tilde,
             linear_obj_list=self.linear_obj_list,
             settings=self.settings_inversion,
             preloads=self.preloads,
-            run_time_dict=self.tracer.run_time_dict,
+            profiling_dict=self.tracer.profiling_dict,
         )
 
         inversion.linear_obj_galaxy_dict = self.linear_obj_galaxy_dict
 
         return inversion
```

### Comparing `autolens-2023.6.12.4/autolens/plot/__init__.py` & `autolens-2023.7.7.2/autolens/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/plot/abstract_plotters.py` & `autolens-2023.7.7.2/autolens/plot/abstract_plotters.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/plot/get_visuals/one_d.py` & `autolens-2023.7.7.2/autolens/plot/get_visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/plot/get_visuals/two_d.py` & `autolens-2023.7.7.2/autolens/plot/get_visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/point/fit_point/fluxes.py` & `autolens-2023.7.7.2/autolens/point/fit_point/fluxes.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/point/fit_point/max_separation.py` & `autolens-2023.7.7.2/autolens/point/fit_point/max_separation.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/point/fit_point/point_dataset.py` & `autolens-2023.7.7.2/autolens/point/fit_point/point_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Dict, Optional
-
 import autogalaxy as ag
 
 from autolens.point.point_dataset import PointDataset
 from autolens.point.point_solver import PointSolver
 from autolens.point.fit_point.fluxes import FitFluxes
 from autolens.point.fit_point.positions_image import FitPositionsImage
 from autolens.point.fit_point.positions_source import FitPositionsSource
@@ -17,23 +15,17 @@
     NumbaException = numba.errors.TypingError
 except ModuleNotFoundError:
     NumbaException = AttributeError
 
 
 class FitPointDataset:
     def __init__(
-        self,
-        point_dataset: PointDataset,
-        tracer: Tracer,
-        point_solver: PointSolver,
-        run_time_dict: Optional[Dict] = None,
+        self, point_dataset: PointDataset, tracer: Tracer, point_solver: PointSolver
     ):
         self.point_dataset = point_dataset
-        self.tracer = tracer
-        self.run_time_dict = run_time_dict
 
         point_profile = tracer.extract_profile(profile_name=point_dataset.name)
 
         try:
             if isinstance(point_profile, ag.ps.PointSourceChi):
                 self.positions = FitPositionsSource(
                     name=point_dataset.name,
@@ -67,22 +59,14 @@
                 tracer=tracer,
             )
 
         except exc.PointExtractionException:
             self.flux = None
 
     @property
-    def model_obj(self):
-        return self.tracer
-
-    @property
     def log_likelihood(self) -> float:
         log_likelihood_positions = (
             self.positions.log_likelihood if self.positions is not None else 0.0
         )
         log_likelihood_flux = self.flux.log_likelihood if self.flux is not None else 0.0
 
         return log_likelihood_positions + log_likelihood_flux
-
-    @property
-    def figure_of_merit(self) -> float:
-        return self.log_likelihood
```

### Comparing `autolens-2023.6.12.4/autolens/point/fit_point/positions_image.py` & `autolens-2023.7.7.2/autolens/point/fit_point/positions_image.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/point/fit_point/positions_source.py` & `autolens-2023.7.7.2/autolens/point/fit_point/positions_source.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/point/model/analysis.py` & `autolens-2023.7.7.2/autolens/point/model/analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-from typing import Callable, Dict, Optional, Tuple
-
 import autofit as af
 import autogalaxy as ag
 
-from autogalaxy.analysis.analysis import Analysis as AgAnalysis
-
 from autolens.analysis.analysis import AnalysisLensing
 from autolens.analysis.visualizer import Visualizer
 from autolens.point.point_dataset import PointDict
 from autolens.point.fit_point.point_dict import FitPointDict
 from autolens.point.model.result import ResultPoint
 
 from autolens.point.point_solver import PointSolver
@@ -20,20 +16,20 @@
     import numba
 
     NumbaException = numba.errors.TypingError
 except ModuleNotFoundError:
     NumbaException = ValueError
 
 
-class AnalysisPoint(AgAnalysis, AnalysisLensing):
+class AnalysisPoint(af.Analysis, AnalysisLensing):
     def __init__(
         self,
         point_dict: PointDict,
         solver: PointSolver,
-        dataset=None,
+        imaging=None,
         cosmology: ag.cosmo.LensingCosmology = ag.cosmo.Planck15(),
         settings_lens=SettingsLens(),
     ):
         """
         The analysis performed for model-fitting a point-source dataset, for example fitting the point-sources of a
         multiply imaged lensed quasar or supernovae of many source galaxies of a galaxy cluster.
 
@@ -43,37 +39,33 @@
 
         Parameters
         ----------
         point_dict
             A dictionary containing the full point source dictionary that is used for model-fitting.
         solver
             The object which is used to determine the image-plane of source-plane positions of a model (via a `Tracer`).
-        dataset
+        imaging
             The imaging of the point-source dataset, which is not used for model-fitting but can be used for
             visualization.
         cosmology
             The cosmology of the ray-tracing calculation.
         settings_lens
             Settings which control how the model-fit is performed.
         """
 
-        super().__init__(cosmology=cosmology)
+        super().__init__(settings_lens=settings_lens, cosmology=cosmology)
 
         AnalysisLensing.__init__(
             self=self, settings_lens=settings_lens, cosmology=cosmology
         )
 
         self.point_dict = point_dict
 
         self.solver = solver
-        self.dataset = dataset
-
-    @property
-    def fit_func(self) -> Callable:
-        return self.fit_positions_for
+        self.dataset = imaging
 
     def log_likelihood_function(self, instance):
         """
         Determine the fit of the strong lens system of lens galaxies and source galaxies to the point source data.
 
         Parameters
         ----------
@@ -87,26 +79,19 @@
         """
         try:
             fit = self.fit_positions_for(instance=instance)
             return fit.log_likelihood
         except (AttributeError, ValueError, TypeError, NumbaException) as e:
             raise exc.FitException from e
 
-    def fit_positions_for(
-        self, instance, run_time_dict: Optional[Dict] = None
-    ) -> FitPointDict:
-        tracer = self.tracer_via_instance_from(
-            instance=instance, run_time_dict=run_time_dict
-        )
+    def fit_positions_for(self, instance):
+        tracer = self.tracer_via_instance_from(instance=instance)
 
         return FitPointDict(
-            point_dict=self.point_dict,
-            tracer=tracer,
-            point_solver=self.solver,
-            run_time_dict=run_time_dict,
+            point_dict=self.point_dict, tracer=tracer, point_solver=self.solver
         )
 
     def visualize(self, paths, instance, during_analysis):
         tracer = self.tracer_via_instance_from(instance=instance)
 
         visualizer = Visualizer(visualize_path=paths.image_path)
```

### Comparing `autolens-2023.6.12.4/autolens/point/plot/fit_point_plotters.py` & `autolens-2023.7.7.2/autolens/point/plot/fit_point_plotters.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/point/plot/point_dataset_plotters.py` & `autolens-2023.7.7.2/autolens/point/plot/point_dataset_plotters.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/point/point_dataset.py` & `autolens-2023.7.7.2/autolens/point/point_dataset.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/point/point_solver.py` & `autolens-2023.7.7.2/autolens/point/point_solver.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/quantity/fit_quantity.py` & `autolens-2023.7.7.2/autolens/quantity/fit_quantity.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/quantity/model/analysis.py` & `autolens-2023.7.7.2/autolens/quantity/model/analysis.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/quantity/model/result.py` & `autolens-2023.7.7.2/autolens/quantity/model/result.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/autolens/util/__init__.py` & `autolens-2023.7.7.2/autolens/util/__init__.py`

 * *Files identical despite different names*

### Comparing `autolens-2023.6.12.4/setup.py` & `autolens-2023.7.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "1.0.dev0")
+version = environ.get("VERSION", "2023.7.7.2")
 requirements.extend(
     [
         f"autoarray=={version}",
         f"autoconf=={version}",
         f"autofit=={version}",
         f"autogalaxy=={version}",
     ]
```

