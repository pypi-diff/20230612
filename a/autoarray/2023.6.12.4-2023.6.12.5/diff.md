# Comparing `tmp/autoarray-2023.6.12.4.tar.gz` & `tmp/autoarray-2023.6.12.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoarray-2023.6.12.4.tar", last modified: Mon Jun 12 13:49:10 2023, max compression
+gzip compressed data, was "autoarray-2023.6.12.5.tar", last modified: Mon Jun 12 14:10:19 2023, max compression
```

## Comparing `autoarray-2023.6.12.4.tar` & `autoarray-2023.6.12.5.tar`

### file list

```diff
@@ -1,310 +1,310 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.036392 autoarray-2023.6.12.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-12 13:49:10.036392 autoarray-2023.6.12.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.952390 autoarray-2023.6.12.4/autoarray/
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/abstract_ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.952390 autoarray-2023.6.12.4/autoarray/config/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/config/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/config/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/config/general.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/config/grids.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/config/logging.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.956390 autoarray-2023.6.12.4/autoarray/config/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/config/visualize/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/config/visualize/general.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/config/visualize/include.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/config/visualize/mat_wrap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/config/visualize/mat_wrap_1d.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/config/visualize/mat_wrap_2d.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/config/visualize/plots.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.960390 autoarray-2023.6.12.4/autoarray/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.960390 autoarray-2023.6.12.4/autoarray/dataset/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/abstract/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/abstract/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/abstract/w_tilde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.964390 autoarray-2023.6.12.4/autoarray/dataset/imaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/imaging/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/imaging/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/imaging/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/imaging/w_tilde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.968390 autoarray-2023.6.12.4/autoarray/dataset/interferometer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/interferometer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/interferometer/interferometer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/interferometer/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/interferometer/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/interferometer/w_tilde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.968390 autoarray-2023.6.12.4/autoarray/dataset/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/mock/mock_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.968390 autoarray-2023.6.12.4/autoarray/dataset/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/plot/imaging_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/plot/interferometer_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    20418 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/dataset/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.972390 autoarray-2023.6.12.4/autoarray/fit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/fit/fit_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/fit/fit_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/fit/fit_interferometer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/fit/fit_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.972390 autoarray-2023.6.12.4/autoarray/fit/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/fit/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/fit/mock/mock_fit_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/fit/mock/mock_fit_interferometer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.972390 autoarray-2023.6.12.4/autoarray/fit/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/fit/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/fit/plot/fit_imaging_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    22617 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/fit/plot/fit_interferometer_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/fit/plot/fit_vector_yx_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.976390 autoarray-2023.6.12.4/autoarray/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/geometry/abstract_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/geometry/geometry_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/geometry/geometry_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/geometry/geometry_2d_irregular.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/geometry/geometry_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.976390 autoarray-2023.6.12.4/autoarray/inversion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.980390 autoarray-2023.6.12.4/autoarray/inversion/inversion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35987 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    15417 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.980390 autoarray-2023.6.12.4/autoarray/inversion/inversion/imaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/imaging/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    34720 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/imaging/inversion_imaging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/imaging/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    27382 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/imaging/w_tilde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.984391 autoarray-2023.6.12.4/autoarray/inversion/inversion/interferometer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/interferometer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/interferometer/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/interferometer/lop.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/interferometer/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/interferometer/w_tilde.py
--rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/inversion_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/inversion/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.984391 autoarray-2023.6.12.4/autoarray/inversion/linear_obj/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/linear_obj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/linear_obj/func_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/linear_obj/linear_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/linear_obj/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/linear_obj/unique_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.988391 autoarray-2023.6.12.4/autoarray/inversion/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/mock/mock_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/mock/mock_inversion_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/mock/mock_inversion_interferometer.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/mock/mock_linear_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/mock/mock_linear_obj_func_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/mock/mock_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/mock/mock_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/mock/mock_pixelization.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/mock/mock_regularization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.992391 autoarray-2023.6.12.4/autoarray/inversion/pixelization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.992391 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/delaunay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/mapper_grids.py
--rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/mapper_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/rectangular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/voronoi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:09.996391 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/delaunay.py
--rw-r--r--   0 runner    (1001) docker     (123)    24438 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/mesh_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/rectangular.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/triangulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/voronoi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/voronoi_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/pixelization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/pixelization/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.000391 autoarray-2023.6.12.4/autoarray/inversion/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/plot/inversion_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/plot/mapper_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.004391 autoarray-2023.6.12.4/autoarray/inversion/regularization/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/regularization/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/regularization/adaptive_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/regularization/adaptive_brightness_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/regularization/brightness_zeroth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/regularization/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/regularization/constant_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/regularization/constant_zeroth.py
--rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/regularization/regularization_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/inversion/regularization/zeroth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.004391 autoarray-2023.6.12.4/autoarray/layout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/layout/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/layout/layout_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/layout/region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.008391 autoarray-2023.6.12.4/autoarray/mask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/abstract_mask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.008391 autoarray-2023.6.12.4/autoarray/mask/derive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/derive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/derive/grid_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/derive/grid_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    21875 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/derive/indexes_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/derive/mask_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/derive/mask_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/mask_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/mask_1d_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    35868 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/mask_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    48943 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/mask_2d_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.012391 autoarray-2023.6.12.4/autoarray/mask/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mask/mock/mock_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/numba_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.012391 autoarray-2023.6.12.4/autoarray/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22050 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/operators/convolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.012391 autoarray-2023.6.12.4/autoarray/operators/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/operators/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/operators/mock/mock_convolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/operators/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/operators/transformer_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.016391 autoarray-2023.6.12.4/autoarray/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/abstract_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/auto_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.016391 autoarray-2023.6.12.4/autoarray/plot/get_visuals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/get_visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/get_visuals/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/get_visuals/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/get_visuals/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.016391 autoarray-2023.6.12.4/autoarray/plot/include/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/include/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/include/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/include/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/include/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.020392 autoarray-2023.6.12.4/autoarray/plot/mat_plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/mat_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/mat_plot/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/mat_plot/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)    26093 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/mat_plot/two_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/multi_plotters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.020392 autoarray-2023.6.12.4/autoarray/plot/visuals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/visuals/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/visuals/one_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/visuals/two_d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.020392 autoarray-2023.6.12.4/autoarray/plot/wrap/
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.028392 autoarray-2023.6.12.4/autoarray/plot/wrap/base/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/cmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/colorbar_tickparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/figure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/label.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/legend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/tickparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/ticks.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/base/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.028392 autoarray-2023.6.12.4/autoarray/plot/wrap/one_d/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/one_d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/one_d/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/one_d/avxline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/one_d/fill_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/one_d/yx_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/one_d/yx_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44375 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/segmentdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.032392 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/array_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/border_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/grid_errorbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/grid_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/grid_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/index_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/interpolated_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/mask_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/mesh_grid_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/origin_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/parallel_overscan_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/patch_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/positions_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/serial_overscan_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/serial_prescan_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/vector_yx_quiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/voronoi_drawer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/preloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.032392 autoarray-2023.6.12.4/autoarray/structures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/abstract_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.032392 autoarray-2023.6.12.4/autoarray/structures/arrays/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/arrays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/arrays/array_1d_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    31344 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/arrays/array_2d_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/arrays/irregular.py
--rw-r--r--   0 runner    (1001) docker     (123)    18861 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/arrays/kernel_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/arrays/uniform_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    42401 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/arrays/uniform_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.036392 autoarray-2023.6.12.4/autoarray/structures/grids/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/grids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/grids/grid_1d_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    32851 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/grids/grid_2d_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/grids/irregular_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    41103 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/grids/iterate_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/grids/sparse_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/grids/sparse_2d_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/grids/transformed_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/grids/uniform_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    48699 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/grids/uniform_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/header.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.036392 autoarray-2023.6.12.4/autoarray/structures/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/mesh/abstract_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/mesh/delaunay_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/mesh/rectangular_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/mesh/triangulation_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/mesh/voronoi_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.036392 autoarray-2023.6.12.4/autoarray/structures/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/mock/mock_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/mock/mock_structure_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.036392 autoarray-2023.6.12.4/autoarray/structures/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/plot/structure_plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/structure_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.036392 autoarray-2023.6.12.4/autoarray/structures/vectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/vectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/vectors/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/vectors/irregular.py
--rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/vectors/uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/structures/visibilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.036392 autoarray-2023.6.12.4/autoarray/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/util/cholesky_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/util/fnnls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/autoarray/util/misc_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.036392 autoarray-2023.6.12.4/autoarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-06-12 13:49:09.000000 autoarray-2023.6.12.4/autoarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:49:10.036392 autoarray-2023.6.12.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-12 13:48:59.000000 autoarray-2023.6.12.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.549271 autoarray-2023.6.12.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-12 14:10:19.549271 autoarray-2023.6.12.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.497267 autoarray-2023.6.12.5/autoarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-12 14:10:09.000000 autoarray-2023.6.12.5/autoarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/abstract_ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.497267 autoarray-2023.6.12.5/autoarray/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/config/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/config/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/config/general.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/config/grids.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/config/logging.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.497267 autoarray-2023.6.12.5/autoarray/config/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/config/visualize/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/config/visualize/general.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/config/visualize/include.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/config/visualize/mat_wrap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/config/visualize/mat_wrap_1d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/config/visualize/mat_wrap_2d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/config/visualize/plots.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.497267 autoarray-2023.6.12.5/autoarray/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.497267 autoarray-2023.6.12.5/autoarray/dataset/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/abstract/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/abstract/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/abstract/w_tilde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.497267 autoarray-2023.6.12.5/autoarray/dataset/imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/imaging/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/imaging/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/imaging/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/imaging/w_tilde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.501267 autoarray-2023.6.12.5/autoarray/dataset/interferometer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/interferometer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/interferometer/interferometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/interferometer/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/interferometer/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/interferometer/w_tilde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.501267 autoarray-2023.6.12.5/autoarray/dataset/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/mock/mock_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.501267 autoarray-2023.6.12.5/autoarray/dataset/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/plot/imaging_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/plot/interferometer_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20418 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/dataset/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.501267 autoarray-2023.6.12.5/autoarray/fit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/fit/fit_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/fit/fit_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/fit/fit_interferometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/fit/fit_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.501267 autoarray-2023.6.12.5/autoarray/fit/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/fit/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/fit/mock/mock_fit_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/fit/mock/mock_fit_interferometer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.501267 autoarray-2023.6.12.5/autoarray/fit/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/fit/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/fit/plot/fit_imaging_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22617 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/fit/plot/fit_interferometer_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/fit/plot/fit_vector_yx_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.501267 autoarray-2023.6.12.5/autoarray/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/geometry/abstract_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/geometry/geometry_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/geometry/geometry_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/geometry/geometry_2d_irregular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/geometry/geometry_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.501267 autoarray-2023.6.12.5/autoarray/inversion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.505268 autoarray-2023.6.12.5/autoarray/inversion/inversion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35987 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15417 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.505268 autoarray-2023.6.12.5/autoarray/inversion/inversion/imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/imaging/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34720 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/imaging/inversion_imaging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/imaging/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27382 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/imaging/w_tilde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.505268 autoarray-2023.6.12.5/autoarray/inversion/inversion/interferometer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/interferometer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/interferometer/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/interferometer/lop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/interferometer/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/interferometer/w_tilde.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/inversion_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/inversion/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.505268 autoarray-2023.6.12.5/autoarray/inversion/linear_obj/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/linear_obj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/linear_obj/func_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/linear_obj/linear_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/linear_obj/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/linear_obj/unique_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.505268 autoarray-2023.6.12.5/autoarray/inversion/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/mock/mock_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/mock/mock_inversion_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/mock/mock_inversion_interferometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/mock/mock_linear_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/mock/mock_linear_obj_func_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/mock/mock_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/mock/mock_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/mock/mock_pixelization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/mock/mock_regularization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.509268 autoarray-2023.6.12.5/autoarray/inversion/pixelization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.509268 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/delaunay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/mapper_grids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/mapper_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/rectangular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/voronoi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.509268 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/delaunay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24438 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/mesh_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/rectangular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/triangulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/voronoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/voronoi_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/pixelization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/pixelization/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.509268 autoarray-2023.6.12.5/autoarray/inversion/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/plot/inversion_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/plot/mapper_plotters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.513268 autoarray-2023.6.12.5/autoarray/inversion/regularization/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/regularization/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/regularization/adaptive_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/regularization/adaptive_brightness_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/regularization/brightness_zeroth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/regularization/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/regularization/constant_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/regularization/constant_zeroth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/regularization/regularization_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/inversion/regularization/zeroth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.513268 autoarray-2023.6.12.5/autoarray/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/layout/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/layout/layout_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/layout/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.513268 autoarray-2023.6.12.5/autoarray/mask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/abstract_mask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.513268 autoarray-2023.6.12.5/autoarray/mask/derive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/derive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/derive/grid_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/derive/grid_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21875 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/derive/indexes_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/derive/mask_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/derive/mask_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/mask_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/mask_1d_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35868 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/mask_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48943 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/mask_2d_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.513268 autoarray-2023.6.12.5/autoarray/mask/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mask/mock/mock_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/numba_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.513268 autoarray-2023.6.12.5/autoarray/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22050 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/operators/convolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.513268 autoarray-2023.6.12.5/autoarray/operators/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/operators/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/operators/mock/mock_convolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/operators/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/operators/transformer_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.517269 autoarray-2023.6.12.5/autoarray/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/abstract_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/auto_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.517269 autoarray-2023.6.12.5/autoarray/plot/get_visuals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/get_visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/get_visuals/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/get_visuals/one_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/get_visuals/two_d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.517269 autoarray-2023.6.12.5/autoarray/plot/include/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/include/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/include/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/include/one_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/include/two_d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.521269 autoarray-2023.6.12.5/autoarray/plot/mat_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/mat_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/mat_plot/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/mat_plot/one_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26093 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/mat_plot/two_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/multi_plotters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.521269 autoarray-2023.6.12.5/autoarray/plot/visuals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/visuals/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/visuals/one_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/visuals/two_d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.521269 autoarray-2023.6.12.5/autoarray/plot/wrap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.525269 autoarray-2023.6.12.5/autoarray/plot/wrap/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/cmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/colorbar_tickparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/tickparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/ticks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/base/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.529269 autoarray-2023.6.12.5/autoarray/plot/wrap/one_d/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/one_d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/one_d/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/one_d/avxline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/one_d/fill_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/one_d/yx_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/one_d/yx_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44375 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/segmentdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.533270 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/array_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/border_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/grid_errorbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/grid_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/grid_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/index_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/interpolated_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/mask_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/mesh_grid_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/origin_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/parallel_overscan_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/patch_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/positions_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/serial_overscan_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/serial_prescan_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/vector_yx_quiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/voronoi_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/preloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.537270 autoarray-2023.6.12.5/autoarray/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/abstract_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.537270 autoarray-2023.6.12.5/autoarray/structures/arrays/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/arrays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/arrays/array_1d_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31344 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/arrays/array_2d_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/arrays/irregular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18861 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/arrays/kernel_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/arrays/uniform_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42401 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/arrays/uniform_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.541270 autoarray-2023.6.12.5/autoarray/structures/grids/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/grids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/grids/grid_1d_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32851 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/grids/grid_2d_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/grids/irregular_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41103 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/grids/iterate_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/grids/sparse_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/grids/sparse_2d_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/grids/transformed_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/grids/uniform_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48699 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/grids/uniform_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/header.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.545271 autoarray-2023.6.12.5/autoarray/structures/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/mesh/abstract_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/mesh/delaunay_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/mesh/rectangular_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/mesh/triangulation_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/mesh/voronoi_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.545271 autoarray-2023.6.12.5/autoarray/structures/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/mock/mock_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/mock/mock_structure_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.545271 autoarray-2023.6.12.5/autoarray/structures/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/plot/structure_plotters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/structure_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.549271 autoarray-2023.6.12.5/autoarray/structures/vectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/vectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/vectors/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/vectors/irregular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/vectors/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/structures/visibilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.549271 autoarray-2023.6.12.5/autoarray/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/util/cholesky_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/util/fnnls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/autoarray/util/misc_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:19.549271 autoarray-2023.6.12.5/autoarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-06-12 14:10:19.000000 autoarray-2023.6.12.5/autoarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:10:19.549271 autoarray-2023.6.12.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-12 14:10:08.000000 autoarray-2023.6.12.5/setup.py
```

### Comparing `autoarray-2023.6.12.4/LICENSE` & `autoarray-2023.6.12.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/PKG-INFO` & `autoarray-2023.6.12.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoarray
-Version: 2023.6.12.4
+Version: 2023.6.12.5
 Summary: PyAuto Data Structures
 Home-page: https://github.com/Jammy2211/PyAutoArray
 Author: James Nightingale and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
```

### Comparing `autoarray-2023.6.12.4/autoarray/__init__.py` & `autoarray-2023.6.12.5/autoarray/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,8 @@
 from .structures.visibilities import Visibilities
 from .structures.visibilities import VisibilitiesNoiseMap
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2023.6.12.4"
+__version__ = "2023.6.12.5"
```

### Comparing `autoarray-2023.6.12.4/autoarray/abstract_ndarray.py` & `autoarray-2023.6.12.5/autoarray/abstract_ndarray.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/config/README.rst` & `autoarray-2023.6.12.5/autoarray/config/README.rst`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/config/general.yaml` & `autoarray-2023.6.12.5/autoarray/config/general.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/config/visualize/README.rst` & `autoarray-2023.6.12.5/autoarray/config/visualize/README.rst`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/config/visualize/general.yaml` & `autoarray-2023.6.12.5/autoarray/config/visualize/general.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/config/visualize/include.yaml` & `autoarray-2023.6.12.5/autoarray/config/visualize/include.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/config/visualize/mat_wrap.yaml` & `autoarray-2023.6.12.5/autoarray/config/visualize/mat_wrap.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/config/visualize/mat_wrap_1d.yaml` & `autoarray-2023.6.12.5/autoarray/config/visualize/mat_wrap_1d.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/config/visualize/mat_wrap_2d.yaml` & `autoarray-2023.6.12.5/autoarray/config/visualize/mat_wrap_2d.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/config/visualize/plots.yaml` & `autoarray-2023.6.12.5/autoarray/config/visualize/plots.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/abstract/dataset.py` & `autoarray-2023.6.12.5/autoarray/dataset/abstract/dataset.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/abstract/settings.py` & `autoarray-2023.6.12.5/autoarray/dataset/abstract/settings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/abstract/w_tilde.py` & `autoarray-2023.6.12.5/autoarray/dataset/abstract/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/imaging/imaging.py` & `autoarray-2023.6.12.5/autoarray/dataset/imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/imaging/settings.py` & `autoarray-2023.6.12.5/autoarray/dataset/imaging/settings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/imaging/simulator.py` & `autoarray-2023.6.12.5/autoarray/dataset/imaging/simulator.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/imaging/w_tilde.py` & `autoarray-2023.6.12.5/autoarray/dataset/imaging/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/interferometer/interferometer.py` & `autoarray-2023.6.12.5/autoarray/dataset/interferometer/interferometer.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/interferometer/settings.py` & `autoarray-2023.6.12.5/autoarray/dataset/interferometer/settings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/interferometer/simulator.py` & `autoarray-2023.6.12.5/autoarray/dataset/interferometer/simulator.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/interferometer/w_tilde.py` & `autoarray-2023.6.12.5/autoarray/dataset/interferometer/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/plot/imaging_plotters.py` & `autoarray-2023.6.12.5/autoarray/dataset/plot/imaging_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/plot/interferometer_plotters.py` & `autoarray-2023.6.12.5/autoarray/dataset/plot/interferometer_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/dataset/preprocess.py` & `autoarray-2023.6.12.5/autoarray/dataset/preprocess.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/exc.py` & `autoarray-2023.6.12.5/autoarray/exc.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/fit/fit_dataset.py` & `autoarray-2023.6.12.5/autoarray/fit/fit_dataset.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/fit/fit_imaging.py` & `autoarray-2023.6.12.5/autoarray/fit/fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/fit/fit_interferometer.py` & `autoarray-2023.6.12.5/autoarray/fit/fit_interferometer.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/fit/fit_util.py` & `autoarray-2023.6.12.5/autoarray/fit/fit_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/fit/mock/mock_fit_imaging.py` & `autoarray-2023.6.12.5/autoarray/fit/mock/mock_fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/fit/mock/mock_fit_interferometer.py` & `autoarray-2023.6.12.5/autoarray/fit/mock/mock_fit_interferometer.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/fit/plot/fit_imaging_plotters.py` & `autoarray-2023.6.12.5/autoarray/fit/plot/fit_imaging_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/fit/plot/fit_interferometer_plotters.py` & `autoarray-2023.6.12.5/autoarray/fit/plot/fit_interferometer_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/fit/plot/fit_vector_yx_plotters.py` & `autoarray-2023.6.12.5/autoarray/fit/plot/fit_vector_yx_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/fixtures.py` & `autoarray-2023.6.12.5/autoarray/fixtures.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/geometry/abstract_2d.py` & `autoarray-2023.6.12.5/autoarray/geometry/abstract_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/geometry/geometry_1d.py` & `autoarray-2023.6.12.5/autoarray/geometry/geometry_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/geometry/geometry_2d.py` & `autoarray-2023.6.12.5/autoarray/geometry/geometry_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/geometry/geometry_2d_irregular.py` & `autoarray-2023.6.12.5/autoarray/geometry/geometry_2d_irregular.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/geometry/geometry_util.py` & `autoarray-2023.6.12.5/autoarray/geometry/geometry_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/inversion/abstract.py` & `autoarray-2023.6.12.5/autoarray/inversion/inversion/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/inversion/factory.py` & `autoarray-2023.6.12.5/autoarray/inversion/inversion/factory.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/inversion/imaging/abstract.py` & `autoarray-2023.6.12.5/autoarray/inversion/inversion/imaging/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/inversion/imaging/inversion_imaging_util.py` & `autoarray-2023.6.12.5/autoarray/inversion/inversion/imaging/inversion_imaging_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/inversion/imaging/mapping.py` & `autoarray-2023.6.12.5/autoarray/inversion/inversion/imaging/mapping.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/inversion/imaging/w_tilde.py` & `autoarray-2023.6.12.5/autoarray/inversion/inversion/imaging/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/inversion/interferometer/abstract.py` & `autoarray-2023.6.12.5/autoarray/inversion/inversion/interferometer/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py` & `autoarray-2023.6.12.5/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/inversion/interferometer/lop.py` & `autoarray-2023.6.12.5/autoarray/inversion/inversion/interferometer/lop.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/inversion/interferometer/mapping.py` & `autoarray-2023.6.12.5/autoarray/inversion/inversion/interferometer/mapping.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/inversion/interferometer/w_tilde.py` & `autoarray-2023.6.12.5/autoarray/inversion/inversion/interferometer/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/inversion/inversion_util.py` & `autoarray-2023.6.12.5/autoarray/inversion/inversion/inversion_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/inversion/settings.py` & `autoarray-2023.6.12.5/autoarray/inversion/inversion/settings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/linear_obj/func_list.py` & `autoarray-2023.6.12.5/autoarray/inversion/linear_obj/func_list.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/linear_obj/linear_obj.py` & `autoarray-2023.6.12.5/autoarray/inversion/linear_obj/linear_obj.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/linear_obj/neighbors.py` & `autoarray-2023.6.12.5/autoarray/inversion/linear_obj/neighbors.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/linear_obj/unique_mappings.py` & `autoarray-2023.6.12.5/autoarray/inversion/linear_obj/unique_mappings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/mock/mock_inversion.py` & `autoarray-2023.6.12.5/autoarray/inversion/mock/mock_inversion.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/mock/mock_inversion_imaging.py` & `autoarray-2023.6.12.5/autoarray/inversion/mock/mock_inversion_imaging.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/mock/mock_inversion_interferometer.py` & `autoarray-2023.6.12.5/autoarray/inversion/mock/mock_inversion_interferometer.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/mock/mock_linear_obj.py` & `autoarray-2023.6.12.5/autoarray/inversion/mock/mock_linear_obj.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/mock/mock_linear_obj_func_list.py` & `autoarray-2023.6.12.5/autoarray/inversion/mock/mock_linear_obj_func_list.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/mock/mock_mapper.py` & `autoarray-2023.6.12.5/autoarray/inversion/mock/mock_mapper.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/mock/mock_mesh.py` & `autoarray-2023.6.12.5/autoarray/inversion/mock/mock_mesh.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/mock/mock_pixelization.py` & `autoarray-2023.6.12.5/autoarray/inversion/mock/mock_pixelization.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/abstract.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/delaunay.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/delaunay.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/factory.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/factory.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/mapper_grids.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/mapper_grids.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/mapper_util.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/mapper_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/rectangular.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/rectangular.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mappers/voronoi.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mappers/voronoi.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/abstract.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/delaunay.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/delaunay.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/mesh_util.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/mesh_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/rectangular.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/rectangular.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/triangulation.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/triangulation.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/voronoi.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/voronoi.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/mesh/voronoi_nn.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/mesh/voronoi_nn.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/pixelization.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/pixelization.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/pixelization/settings.py` & `autoarray-2023.6.12.5/autoarray/inversion/pixelization/settings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/plot/inversion_plotters.py` & `autoarray-2023.6.12.5/autoarray/inversion/plot/inversion_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/plot/mapper_plotters.py` & `autoarray-2023.6.12.5/autoarray/inversion/plot/mapper_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/regularization/abstract.py` & `autoarray-2023.6.12.5/autoarray/inversion/regularization/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/regularization/adaptive_brightness.py` & `autoarray-2023.6.12.5/autoarray/inversion/regularization/adaptive_brightness.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/regularization/adaptive_brightness_split.py` & `autoarray-2023.6.12.5/autoarray/inversion/regularization/adaptive_brightness_split.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py` & `autoarray-2023.6.12.5/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/regularization/brightness_zeroth.py` & `autoarray-2023.6.12.5/autoarray/inversion/regularization/brightness_zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/regularization/constant.py` & `autoarray-2023.6.12.5/autoarray/inversion/regularization/constant.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/regularization/constant_split.py` & `autoarray-2023.6.12.5/autoarray/inversion/regularization/constant_split.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/regularization/constant_zeroth.py` & `autoarray-2023.6.12.5/autoarray/inversion/regularization/constant_zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/regularization/regularization_util.py` & `autoarray-2023.6.12.5/autoarray/inversion/regularization/regularization_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/inversion/regularization/zeroth.py` & `autoarray-2023.6.12.5/autoarray/inversion/regularization/zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/layout/layout.py` & `autoarray-2023.6.12.5/autoarray/layout/layout.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/layout/layout_util.py` & `autoarray-2023.6.12.5/autoarray/layout/layout_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/layout/region.py` & `autoarray-2023.6.12.5/autoarray/layout/region.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/mask/abstract_mask.py` & `autoarray-2023.6.12.5/autoarray/mask/abstract_mask.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/mask/derive/grid_1d.py` & `autoarray-2023.6.12.5/autoarray/mask/derive/grid_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/mask/derive/grid_2d.py` & `autoarray-2023.6.12.5/autoarray/mask/derive/grid_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/mask/derive/indexes_2d.py` & `autoarray-2023.6.12.5/autoarray/mask/derive/indexes_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/mask/derive/mask_1d.py` & `autoarray-2023.6.12.5/autoarray/mask/derive/mask_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/mask/derive/mask_2d.py` & `autoarray-2023.6.12.5/autoarray/mask/derive/mask_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/mask/mask_1d.py` & `autoarray-2023.6.12.5/autoarray/mask/mask_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/mask/mask_1d_util.py` & `autoarray-2023.6.12.5/autoarray/mask/mask_1d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/mask/mask_2d.py` & `autoarray-2023.6.12.5/autoarray/mask/mask_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/mask/mask_2d_util.py` & `autoarray-2023.6.12.5/autoarray/mask/mask_2d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/mock.py` & `autoarray-2023.6.12.5/autoarray/mock.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/numba_util.py` & `autoarray-2023.6.12.5/autoarray/numba_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/operators/convolver.py` & `autoarray-2023.6.12.5/autoarray/operators/convolver.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/operators/transformer.py` & `autoarray-2023.6.12.5/autoarray/operators/transformer.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/operators/transformer_util.py` & `autoarray-2023.6.12.5/autoarray/operators/transformer_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/__init__.py` & `autoarray-2023.6.12.5/autoarray/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/abstract_plotters.py` & `autoarray-2023.6.12.5/autoarray/plot/abstract_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/get_visuals/abstract.py` & `autoarray-2023.6.12.5/autoarray/plot/get_visuals/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/get_visuals/one_d.py` & `autoarray-2023.6.12.5/autoarray/plot/get_visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/get_visuals/two_d.py` & `autoarray-2023.6.12.5/autoarray/plot/get_visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/include/abstract.py` & `autoarray-2023.6.12.5/autoarray/plot/include/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/include/one_d.py` & `autoarray-2023.6.12.5/autoarray/plot/include/one_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/include/two_d.py` & `autoarray-2023.6.12.5/autoarray/plot/include/two_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/mat_plot/abstract.py` & `autoarray-2023.6.12.5/autoarray/plot/mat_plot/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/mat_plot/one_d.py` & `autoarray-2023.6.12.5/autoarray/plot/mat_plot/one_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/mat_plot/two_d.py` & `autoarray-2023.6.12.5/autoarray/plot/mat_plot/two_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/multi_plotters.py` & `autoarray-2023.6.12.5/autoarray/plot/multi_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/visuals/abstract.py` & `autoarray-2023.6.12.5/autoarray/plot/visuals/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/visuals/one_d.py` & `autoarray-2023.6.12.5/autoarray/plot/visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/visuals/two_d.py` & `autoarray-2023.6.12.5/autoarray/plot/visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/__init__.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/__init__.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/abstract.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/annotate.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/annotate.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/axis.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/axis.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/cmap.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/cmap.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/colorbar.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/colorbar.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/figure.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/figure.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/label.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/label.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/legend.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/legend.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/output.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/output.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/text.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/text.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/tickparams.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/tickparams.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/ticks.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/ticks.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/title.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/title.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/base/units.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/base/units.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/one_d/abstract.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/one_d/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/one_d/avxline.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/one_d/avxline.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/one_d/fill_between.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/one_d/fill_between.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/one_d/yx_plot.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/one_d/yx_plot.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/one_d/yx_scatter.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/one_d/yx_scatter.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/segmentdata.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/segmentdata.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/__init__.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/__init__.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/abstract.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/array_overlay.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/array_overlay.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/grid_errorbar.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/grid_errorbar.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/grid_plot.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/grid_plot.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/grid_scatter.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/grid_scatter.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/interpolated_reconstruction.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/interpolated_reconstruction.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/patch_overlay.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/patch_overlay.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/vector_yx_quiver.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/vector_yx_quiver.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/plot/wrap/two_d/voronoi_drawer.py` & `autoarray-2023.6.12.5/autoarray/plot/wrap/two_d/voronoi_drawer.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/preloads.py` & `autoarray-2023.6.12.5/autoarray/preloads.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/abstract_structure.py` & `autoarray-2023.6.12.5/autoarray/structures/abstract_structure.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/arrays/array_1d_util.py` & `autoarray-2023.6.12.5/autoarray/structures/arrays/array_1d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/arrays/array_2d_util.py` & `autoarray-2023.6.12.5/autoarray/structures/arrays/array_2d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/arrays/irregular.py` & `autoarray-2023.6.12.5/autoarray/structures/arrays/irregular.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/arrays/kernel_2d.py` & `autoarray-2023.6.12.5/autoarray/structures/arrays/kernel_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/arrays/uniform_1d.py` & `autoarray-2023.6.12.5/autoarray/structures/arrays/uniform_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/arrays/uniform_2d.py` & `autoarray-2023.6.12.5/autoarray/structures/arrays/uniform_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/grids/grid_1d_util.py` & `autoarray-2023.6.12.5/autoarray/structures/grids/grid_1d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/grids/grid_2d_util.py` & `autoarray-2023.6.12.5/autoarray/structures/grids/grid_2d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/grids/irregular_2d.py` & `autoarray-2023.6.12.5/autoarray/structures/grids/irregular_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/grids/iterate_2d.py` & `autoarray-2023.6.12.5/autoarray/structures/grids/iterate_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/grids/sparse_2d.py` & `autoarray-2023.6.12.5/autoarray/structures/grids/sparse_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/grids/sparse_2d_util.py` & `autoarray-2023.6.12.5/autoarray/structures/grids/sparse_2d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/grids/uniform_1d.py` & `autoarray-2023.6.12.5/autoarray/structures/grids/uniform_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/grids/uniform_2d.py` & `autoarray-2023.6.12.5/autoarray/structures/grids/uniform_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/header.py` & `autoarray-2023.6.12.5/autoarray/structures/header.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/mesh/abstract_2d.py` & `autoarray-2023.6.12.5/autoarray/structures/mesh/abstract_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/mesh/delaunay_2d.py` & `autoarray-2023.6.12.5/autoarray/structures/mesh/delaunay_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/mesh/rectangular_2d.py` & `autoarray-2023.6.12.5/autoarray/structures/mesh/rectangular_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/mesh/triangulation_2d.py` & `autoarray-2023.6.12.5/autoarray/structures/mesh/triangulation_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/mesh/voronoi_2d.py` & `autoarray-2023.6.12.5/autoarray/structures/mesh/voronoi_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/mock/mock_grid.py` & `autoarray-2023.6.12.5/autoarray/structures/mock/mock_grid.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/mock/mock_structure_decorators.py` & `autoarray-2023.6.12.5/autoarray/structures/mock/mock_structure_decorators.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/plot/structure_plotters.py` & `autoarray-2023.6.12.5/autoarray/structures/plot/structure_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/structure_decorators.py` & `autoarray-2023.6.12.5/autoarray/structures/structure_decorators.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/vectors/abstract.py` & `autoarray-2023.6.12.5/autoarray/structures/vectors/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/vectors/irregular.py` & `autoarray-2023.6.12.5/autoarray/structures/vectors/irregular.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/vectors/uniform.py` & `autoarray-2023.6.12.5/autoarray/structures/vectors/uniform.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/structures/visibilities.py` & `autoarray-2023.6.12.5/autoarray/structures/visibilities.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/type.py` & `autoarray-2023.6.12.5/autoarray/type.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/util/__init__.py` & `autoarray-2023.6.12.5/autoarray/util/__init__.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/util/cholesky_funcs.py` & `autoarray-2023.6.12.5/autoarray/util/cholesky_funcs.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/util/fnnls.py` & `autoarray-2023.6.12.5/autoarray/util/fnnls.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray/util/misc_util.py` & `autoarray-2023.6.12.5/autoarray/util/misc_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/autoarray.egg-info/SOURCES.txt` & `autoarray-2023.6.12.5/autoarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoarray-2023.6.12.4/setup.py` & `autoarray-2023.6.12.5/setup.py`

 * *Files identical despite different names*

