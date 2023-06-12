# Comparing `tmp/autoarray-2023.7.7.1.tar.gz` & `tmp/autoarray-2023.7.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoarray-2023.7.7.1.tar", last modified: Wed Jun  7 09:44:45 2023, max compression
+gzip compressed data, was "autoarray-2023.7.7.2.tar", last modified: Wed Jun  7 09:58:38 2023, max compression
```

## Comparing `autoarray-2023.7.7.1.tar` & `autoarray-2023.7.7.2.tar`

### file list

```diff
@@ -1,425 +1,425 @@
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:45.047043 autoarray-2023.7.7.1/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.601516 autoarray-2023.7.7.1/.github/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.666601 autoarray-2023.7.7.1/.github/workflows/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3065 2022-12-19 16:37:07.000000 autoarray-2023.7.7.1/.github/workflows/main.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1095 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/LICENSE
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      385 2022-12-02 11:50:15.000000 autoarray-2023.7.7.1/MANIFEST.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1006 2023-06-07 09:44:45.046043 autoarray-2023.7.7.1/PKG-INFO
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       87 2022-05-03 18:33:14.000000 autoarray-2023.7.7.1/README.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.685670 autoarray-2023.7.7.1/autoarray/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4721 2023-06-07 09:38:14.000000 autoarray-2023.7.7.1/autoarray/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1656 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/abstract_ndarray.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.698728 autoarray-2023.7.7.1/autoarray/config/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/autoarray/config/.gitignore
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      630 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/config/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1431 2023-06-06 18:37:08.000000 autoarray-2023.7.7.1/autoarray/config/general.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       57 2022-11-29 17:43:26.000000 autoarray-2023.7.7.1/autoarray/config/grids.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      416 2021-06-17 13:08:16.000000 autoarray-2023.7.7.1/autoarray/config/logging.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.722473 autoarray-2023.7.7.1/autoarray/config/visualize/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      696 2022-12-02 11:50:15.000000 autoarray-2023.7.7.1/autoarray/config/visualize/README.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2775 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/config/visualize/general.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1412 2022-12-21 13:17:54.000000 autoarray-2023.7.7.1/autoarray/config/visualize/include.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4233 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/config/visualize/mat_wrap.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1209 2022-12-02 11:50:15.000000 autoarray-2023.7.7.1/autoarray/config/visualize/mat_wrap_1d.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3987 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/config/visualize/mat_wrap_2d.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3208 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/config/visualize/plots.yaml
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.728474 autoarray-2023.7.7.1/autoarray/dataset/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/autoarray/dataset/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.740728 autoarray-2023.7.7.1/autoarray/dataset/abstract/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/dataset/abstract/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4826 2023-06-03 08:48:54.000000 autoarray-2023.7.7.1/autoarray/dataset/abstract/dataset.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4663 2023-05-17 16:06:23.000000 autoarray-2023.7.7.1/autoarray/dataset/abstract/settings.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1750 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/dataset/abstract/w_tilde.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.755774 autoarray-2023.7.7.1/autoarray/dataset/imaging/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/dataset/imaging/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12906 2023-06-03 08:47:07.000000 autoarray-2023.7.7.1/autoarray/dataset/imaging/imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3269 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/dataset/imaging/settings.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4573 2023-06-03 08:45:47.000000 autoarray-2023.7.7.1/autoarray/dataset/imaging/simulator.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1839 2023-02-06 13:53:42.000000 autoarray-2023.7.7.1/autoarray/dataset/imaging/w_tilde.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.770787 autoarray-2023.7.7.1/autoarray/dataset/interferometer/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/dataset/interferometer/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7830 2023-06-03 09:02:33.000000 autoarray-2023.7.7.1/autoarray/dataset/interferometer/interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2471 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/dataset/interferometer/settings.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3700 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/dataset/interferometer/simulator.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2043 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/dataset/interferometer/w_tilde.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.776787 autoarray-2023.7.7.1/autoarray/dataset/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/dataset/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      192 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/dataset/mock/mock_dataset.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.784805 autoarray-2023.7.7.1/autoarray/dataset/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/dataset/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8157 2023-06-03 08:56:57.000000 autoarray-2023.7.7.1/autoarray/dataset/plot/imaging_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12160 2023-06-03 16:54:06.000000 autoarray-2023.7.7.1/autoarray/dataset/plot/interferometer_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20436 2023-06-03 09:10:24.000000 autoarray-2023.7.7.1/autoarray/dataset/preprocess.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3138 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/exc.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.799861 autoarray-2023.7.7.1/autoarray/fit/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/autoarray/fit/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11912 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/fit/fit_dataset.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2592 2023-06-03 08:43:24.000000 autoarray-2023.7.7.1/autoarray/fit/fit_imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6016 2023-06-03 09:34:51.000000 autoarray-2023.7.7.1/autoarray/fit/fit_interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18328 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/fit/fit_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.807893 autoarray-2023.7.7.1/autoarray/fit/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/fit/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1304 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/fit/mock/mock_fit_imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      894 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/fit/mock/mock_fit_interferometer.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.821117 autoarray-2023.7.7.1/autoarray/fit/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/fit/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11054 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/fit/plot/fit_imaging_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22589 2023-06-03 16:41:28.000000 autoarray-2023.7.7.1/autoarray/fit/plot/fit_interferometer_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10437 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/fit/plot/fit_vector_yx_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13605 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/fixtures.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.838408 autoarray-2023.7.7.1/autoarray/geometry/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/autoarray/geometry/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1065 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/geometry/abstract_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2768 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/geometry/geometry_1d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12385 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/geometry/geometry_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1687 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/geometry/geometry_2d_irregular.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27690 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/geometry/geometry_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.841405 autoarray-2023.7.7.1/autoarray/inversion/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-19 14:59:34.000000 autoarray-2023.7.7.1/autoarray/inversion/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.864525 autoarray-2023.7.7.1/autoarray/inversion/inversion/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:42.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35991 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15443 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/factory.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.882596 autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11938 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34720 2023-06-03 09:10:24.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/inversion_imaging_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12033 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/mapping.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27386 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/w_tilde.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.904699 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6128 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5655 2023-03-13 18:37:33.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5331 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/lop.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8257 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/mapping.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9532 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/w_tilde.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12793 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/inversion_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    42583 2023-04-24 16:16:24.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/inversion_util_secret.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38687 2023-04-24 16:16:24.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/inversion_util_secret_clean.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4733 2023-06-03 09:10:24.000000 autoarray-2023.7.7.1/autoarray/inversion/inversion/settings.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.920745 autoarray-2023.7.7.1/autoarray/inversion/linear_obj/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/linear_obj/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4922 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/linear_obj/func_list.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7267 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/linear_obj/linear_obj.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1859 2022-12-21 17:08:33.000000 autoarray-2023.7.7.1/autoarray/inversion/linear_obj/neighbors.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1701 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/linear_obj/unique_mappings.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.953848 autoarray-2023.7.7.1/autoarray/inversion/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6792 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_inversion.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3080 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_inversion_imaging.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1132 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_inversion_interferometer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      888 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_linear_obj.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      912 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_linear_obj_func_list.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2270 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_mapper.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1675 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_mesh.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1023 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_pixelization.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      508 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/mock/mock_regularization.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.963927 autoarray-2023.7.7.1/autoarray/inversion/pixelization/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:43.992150 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21230 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10119 2023-03-13 19:00:38.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/delaunay.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3235 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/factory.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3665 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/mapper_grids.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27357 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/mapper_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6780 2023-03-13 19:00:38.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/rectangular.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12734 2023-04-24 16:13:52.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/voronoi.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.021248 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      360 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5486 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13091 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/delaunay.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24438 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/mesh_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7143 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/rectangular.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4713 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/triangulation.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13162 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/voronoi.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5281 2022-12-22 08:54:23.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/voronoi_nn.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7677 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/pixelization.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1451 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/pixelization/settings.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.030452 autoarray-2023.7.7.1/autoarray/inversion/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/inversion/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10447 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/plot/inversion_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6803 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/plot/mapper_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.065747 autoarray-2023.7.7.1/autoarray/inversion/regularization/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      455 2023-04-01 14:36:25.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8894 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4728 2023-04-01 14:36:25.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/adaptive_brightness.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4508 2023-04-01 14:36:25.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/adaptive_brightness_split.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5208 2023-04-01 14:36:25.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3391 2023-04-01 14:36:25.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/brightness_zeroth.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2964 2023-02-06 13:53:42.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/constant.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3226 2022-12-19 16:33:57.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/constant_split.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2187 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/constant_zeroth.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15369 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/regularization_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3030 2023-02-06 13:53:42.000000 autoarray-2023.7.7.1/autoarray/inversion/regularization/zeroth.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.075741 autoarray-2023.7.7.1/autoarray/layout/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-06-17 13:08:16.000000 autoarray-2023.7.7.1/autoarray/layout/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11370 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/layout/layout.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7309 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/layout/layout_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14064 2023-05-25 17:19:43.000000 autoarray-2023.7.7.1/autoarray/layout/region.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.093025 autoarray-2023.7.7.1/autoarray/mask/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/autoarray/mask/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5222 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/abstract_mask.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.113102 autoarray-2023.7.7.1/autoarray/mask/derive/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-29 16:03:57.000000 autoarray-2023.7.7.1/autoarray/mask/derive/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3485 2023-01-13 16:54:26.000000 autoarray-2023.7.7.1/autoarray/mask/derive/grid_1d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16580 2023-01-13 16:54:26.000000 autoarray-2023.7.7.1/autoarray/mask/derive/grid_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21875 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/derive/indexes_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5317 2023-01-13 16:54:26.000000 autoarray-2023.7.7.1/autoarray/mask/derive/mask_1d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21304 2023-01-13 16:54:26.000000 autoarray-2023.7.7.1/autoarray/mask/derive/mask_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5990 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/mask_1d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3659 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/mask_1d_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35868 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/mask_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48943 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/mask_2d_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.119100 autoarray-2023.7.7.1/autoarray/mask/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/mask/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/mask/mock/mock_mask.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1556 2023-02-12 10:43:58.000000 autoarray-2023.7.7.1/autoarray/mock.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4767 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/numba_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.130113 autoarray-2023.7.7.1/autoarray/operators/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/autoarray/operators/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22050 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/operators/convolver.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.136164 autoarray-2023.7.7.1/autoarray/operators/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/operators/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      244 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/operators/mock/mock_convolver.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11017 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/operators/transformer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7717 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/operators/transformer_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.148178 autoarray-2023.7.7.1/autoarray/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3668 2023-06-03 09:03:18.000000 autoarray-2023.7.7.1/autoarray/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7455 2023-06-03 10:15:39.000000 autoarray-2023.7.7.1/autoarray/plot/abstract_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      477 2023-06-03 16:38:13.000000 autoarray-2023.7.7.1/autoarray/plot/auto_labels.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.159197 autoarray-2023.7.7.1/autoarray/plot/get_visuals/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/get_visuals/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2662 2022-12-21 17:08:33.000000 autoarray-2023.7.7.1/autoarray/plot/get_visuals/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2394 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/get_visuals/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9159 2023-01-13 16:54:26.000000 autoarray-2023.7.7.1/autoarray/plot/get_visuals/two_d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.171054 autoarray-2023.7.7.1/autoarray/plot/include/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/include/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1718 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/include/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1263 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/include/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4182 2022-12-21 13:25:52.000000 autoarray-2023.7.7.1/autoarray/plot/include/two_d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.183088 autoarray-2023.7.7.1/autoarray/plot/mat_plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/mat_plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10623 2023-06-03 16:30:58.000000 autoarray-2023.7.7.1/autoarray/plot/mat_plot/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10971 2023-06-03 09:24:37.000000 autoarray-2023.7.7.1/autoarray/plot/mat_plot/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26131 2023-06-04 12:43:35.000000 autoarray-2023.7.7.1/autoarray/plot/mat_plot/two_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2319 2023-05-15 17:44:36.000000 autoarray-2023.7.7.1/autoarray/plot/multi_plotters.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.195184 autoarray-2023.7.7.1/autoarray/plot/visuals/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/visuals/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2690 2023-05-12 10:15:02.000000 autoarray-2023.7.7.1/autoarray/plot/visuals/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1262 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/visuals/one_d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3396 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/visuals/two_d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.201183 autoarray-2023.7.7.1/autoarray/plot/wrap/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2250 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/__init__.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.256874 autoarray-2023.7.7.1/autoarray/plot/wrap/base/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      469 2023-02-12 10:45:24.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3900 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      544 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/annotate.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1900 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/axis.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3736 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/cmap.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6309 2023-05-15 17:44:36.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/colorbar.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      446 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/colorbar_tickparams.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3042 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/figure.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2865 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/label.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      789 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/legend.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6068 2023-06-05 13:02:24.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/output.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      525 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/text.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      542 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/tickparams.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13250 2023-06-05 13:24:35.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/ticks.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      910 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/title.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2166 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/base/units.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.277894 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      133 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      586 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1961 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/avxline.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1826 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/fill_between.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2802 2023-06-03 16:54:27.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/yx_plot.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/yx_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44375 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/segmentdata.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.343403 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      791 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      586 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      778 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/array_overlay.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      324 2022-12-29 16:03:57.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/border_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4685 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/grid_errorbar.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3733 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/grid_plot.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6735 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/grid_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      316 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/index_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4542 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/interpolated_reconstruction.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      306 2022-12-29 16:03:57.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/mask_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      288 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/mesh_grid_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      310 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/origin_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      279 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/parallel_overscan_plot.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1029 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/patch_overlay.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      321 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/positions_scatter.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/serial_overscan_plot.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      273 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/serial_prescan_plot.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1222 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/vector_yx_quiver.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3220 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/voronoi_drawer.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22159 2023-06-06 10:32:10.000000 autoarray-2023.7.7.1/autoarray/preloads.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.356530 autoarray-2023.7.7.1/autoarray/structures/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-08-13 18:02:25.000000 autoarray-2023.7.7.1/autoarray/structures/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2955 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/abstract_structure.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.378549 autoarray-2023.7.7.1/autoarray/structures/arrays/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-11 15:40:14.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9227 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/array_1d_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31344 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/array_2d_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4901 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/irregular.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18861 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/kernel_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11029 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/uniform_1d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    42401 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/structures/arrays/uniform_2d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.408648 autoarray-2023.7.7.1/autoarray/structures/grids/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-11 15:32:21.000000 autoarray-2023.7.7.1/autoarray/structures/grids/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9412 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/grids/grid_1d_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32851 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/grids/grid_2d_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18547 2023-05-12 10:10:35.000000 autoarray-2023.7.7.1/autoarray/structures/grids/irregular_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41103 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/grids/iterate_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8537 2023-05-11 09:40:23.000000 autoarray-2023.7.7.1/autoarray/structures/grids/sparse_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5498 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/grids/sparse_2d_util.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      256 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/grids/transformed_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18087 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/grids/uniform_1d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48025 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/structures/grids/uniform_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1579 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/header.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.427747 autoarray-2023.7.7.1/autoarray/structures/mesh/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/structures/mesh/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1500 2023-04-24 16:13:52.000000 autoarray-2023.7.7.1/autoarray/structures/mesh/abstract_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3544 2023-04-24 16:13:52.000000 autoarray-2023.7.7.1/autoarray/structures/mesh/delaunay_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7848 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/mesh/rectangular_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10536 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/mesh/triangulation_2d.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3645 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/mesh/voronoi_2d.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.436747 autoarray-2023.7.7.1/autoarray/structures/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/structures/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2679 2023-05-11 17:33:46.000000 autoarray-2023.7.7.1/autoarray/structures/mock/mock_grid.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10875 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/mock/mock_structure_decorators.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.442765 autoarray-2023.7.7.1/autoarray/structures/plot/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/structures/plot/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7227 2022-11-11 15:49:29.000000 autoarray-2023.7.7.1/autoarray/structures/plot/structure_plotters.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22127 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/structure_decorators.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.453799 autoarray-2023.7.7.1/autoarray/structures/vectors/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/structures/vectors/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1028 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/vectors/abstract.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5747 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/vectors/irregular.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21670 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/structures/vectors/uniform.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9550 2023-06-05 19:59:54.000000 autoarray-2023.7.7.1/autoarray/structures/visibilities.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1692 2023-04-24 16:13:52.000000 autoarray-2023.7.7.1/autoarray/type.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.465209 autoarray-2023.7.7.1/autoarray/util/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1273 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2642 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/util/cholesky_funcs.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5284 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/util/fnnls.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2603 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/misc_util.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.470223 autoarray-2023.7.7.1/autoarray/util/nn/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1731 2023-03-21 17:41:19.000000 autoarray-2023.7.7.1/autoarray/util/nn/README.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3897 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/autoarray/util/nn/nn_py.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.474239 autoarray-2023.7.7.1/autoarray/util/nn/src/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1248 2022-12-20 22:03:05.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/README.md
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.645016 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      558 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/.indent.pro
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5420 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/CHANGELOG
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1190 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/CUSTOMISE
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1343 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/LICENSE
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3231 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      166 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/config.h.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   141175 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/configure
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2745 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/configure.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19071 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/delaunay.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1261 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/delaunay.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2408 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/delaunay_internal.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3877 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/distribute.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      717 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/distribute.h
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.650014 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.857596 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      233 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      603 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/generate.awk
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       64 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2810 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/suptitle.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/test.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1430 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/viewexample.m
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.901234 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1258 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   240932 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/data.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      518 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      835 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/mpitest.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2810 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/suptitle.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      760 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/test.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      997 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/viewdata.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1229 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/viewexample.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2958 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/viewinterp.m
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.924294 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1300 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      440 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/generate-data.awk
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      235 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/generate-points.awk
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       46 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      627 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/test.sh
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.957326 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      556 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   132840 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/data.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       56 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      740 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/test.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      999 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/viewdata.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1244 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/viewexample.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2966 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/viewinterp.m
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:44.994531 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      456 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1407289 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/data.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       54 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      461 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/test.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      536 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/viewexample.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2981 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/viewinterp.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2614 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/viewinterp2.m
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:45.023399 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      613 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   165065 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/data.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       45 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      425 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/test.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       34 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/viewexample.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2979 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/viewinterp.m
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      655 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/README
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22150 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/hash.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2040 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/hash.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4772 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/install-sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1398 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/istack.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      767 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/istack.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      600 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/istack_internal.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4154 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/lpi.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3271 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/makefile.example
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3217 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/makefile.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3145 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/makefile_autolens
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36312 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/minell.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      920 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/minell.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      668 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/mkinstalldirs
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      891 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nan.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10955 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nn.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      949 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nn_internal.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11021 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnai.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30764 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnbathy.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2344 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nncommon-vulnerable.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14340 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nncommon.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      390 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nncommon.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnconfig.h.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2220 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnhpi_customized.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40728 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnpi.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      183 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnpi.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4699 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/preader.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      740 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/preader.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2326 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/sample.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)   652743 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/triangle.c
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21562 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/triangle.h
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      425 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/autoarray/util/nn/src/nn/version.c
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:45.044044 autoarray-2023.7.7.1/autoarray.egg-info/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14122 2023-06-07 09:44:43.000000 autoarray-2023.7.7.1/autoarray.egg-info/SOURCES.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:45.034416 autoarray-2023.7.7.1/docs/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/docs/Makefile
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3624 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/docs/conf.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       26 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/docs/index.rst
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      795 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/docs/make.bat
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      148 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/eden.ini
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:44:45.042048 autoarray-2023.7.7.1/files/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2021-06-17 13:08:16.000000 autoarray-2023.7.7.1/files/eden.ini
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      546 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/files/release.sh
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      626 2021-04-02 09:27:57.000000 autoarray-2023.7.7.1/files/to_do_list
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       39 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/optional_requirements.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      210 2022-11-04 15:14:02.000000 autoarray-2023.7.7.1/readthedocs.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      141 2023-03-21 17:41:15.000000 autoarray-2023.7.7.1/requirements.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-06-07 09:44:45.047043 autoarray-2023.7.7.1/setup.cfg
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2036 2023-06-07 09:44:29.000000 autoarray-2023.7.7.1/setup.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1572 2023-05-10 13:41:54.000000 autoarray-2023.7.7.1/to_do_list
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.605314 autoarray-2023.7.7.2/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.828517 autoarray-2023.7.7.2/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.871515 autoarray-2023.7.7.2/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3065 2022-12-19 16:37:07.000000 autoarray-2023.7.7.2/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1095 2021-04-02 09:27:57.000000 autoarray-2023.7.7.2/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      385 2022-12-02 11:50:15.000000 autoarray-2023.7.7.2/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1006 2023-06-07 09:58:38.605314 autoarray-2023.7.7.2/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       87 2022-05-03 18:33:14.000000 autoarray-2023.7.7.2/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.883529 autoarray-2023.7.7.2/autoarray/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4721 2023-06-07 09:57:30.000000 autoarray-2023.7.7.2/autoarray/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1656 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/abstract_ndarray.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.892561 autoarray-2023.7.7.2/autoarray/config/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       11 2021-04-02 09:27:57.000000 autoarray-2023.7.7.2/autoarray/config/.gitignore
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      630 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/config/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1431 2023-06-06 18:37:08.000000 autoarray-2023.7.7.2/autoarray/config/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       57 2022-11-29 17:43:26.000000 autoarray-2023.7.7.2/autoarray/config/grids.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      416 2021-06-17 13:08:16.000000 autoarray-2023.7.7.2/autoarray/config/logging.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.905402 autoarray-2023.7.7.2/autoarray/config/visualize/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      696 2022-12-02 11:50:15.000000 autoarray-2023.7.7.2/autoarray/config/visualize/README.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2775 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/config/visualize/general.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1412 2022-12-21 13:17:54.000000 autoarray-2023.7.7.2/autoarray/config/visualize/include.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4233 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/config/visualize/mat_wrap.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1209 2022-12-02 11:50:15.000000 autoarray-2023.7.7.2/autoarray/config/visualize/mat_wrap_1d.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3987 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/config/visualize/mat_wrap_2d.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3208 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/config/visualize/plots.yaml
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.909401 autoarray-2023.7.7.2/autoarray/dataset/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.2/autoarray/dataset/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.916409 autoarray-2023.7.7.2/autoarray/dataset/abstract/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/dataset/abstract/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4826 2023-06-03 08:48:54.000000 autoarray-2023.7.7.2/autoarray/dataset/abstract/dataset.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4663 2023-05-17 16:06:23.000000 autoarray-2023.7.7.2/autoarray/dataset/abstract/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1750 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/dataset/abstract/w_tilde.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.924941 autoarray-2023.7.7.2/autoarray/dataset/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/dataset/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12906 2023-06-03 08:47:07.000000 autoarray-2023.7.7.2/autoarray/dataset/imaging/imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3269 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/dataset/imaging/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4573 2023-06-03 08:45:47.000000 autoarray-2023.7.7.2/autoarray/dataset/imaging/simulator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1839 2023-02-06 13:53:42.000000 autoarray-2023.7.7.2/autoarray/dataset/imaging/w_tilde.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.934512 autoarray-2023.7.7.2/autoarray/dataset/interferometer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/dataset/interferometer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7830 2023-06-03 09:02:33.000000 autoarray-2023.7.7.2/autoarray/dataset/interferometer/interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2471 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/dataset/interferometer/settings.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3700 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/dataset/interferometer/simulator.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2043 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/dataset/interferometer/w_tilde.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.937512 autoarray-2023.7.7.2/autoarray/dataset/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/dataset/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      192 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/dataset/mock/mock_dataset.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.943503 autoarray-2023.7.7.2/autoarray/dataset/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/dataset/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8157 2023-06-03 08:56:57.000000 autoarray-2023.7.7.2/autoarray/dataset/plot/imaging_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12160 2023-06-03 16:54:06.000000 autoarray-2023.7.7.2/autoarray/dataset/plot/interferometer_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    20436 2023-06-03 09:10:24.000000 autoarray-2023.7.7.2/autoarray/dataset/preprocess.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3138 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/exc.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.951316 autoarray-2023.7.7.2/autoarray/fit/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.2/autoarray/fit/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11912 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/fit/fit_dataset.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2592 2023-06-03 08:43:24.000000 autoarray-2023.7.7.2/autoarray/fit/fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6016 2023-06-03 09:34:51.000000 autoarray-2023.7.7.2/autoarray/fit/fit_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18328 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/fit/fit_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.956950 autoarray-2023.7.7.2/autoarray/fit/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/fit/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1304 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/fit/mock/mock_fit_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      894 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/fit/mock/mock_fit_interferometer.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.964723 autoarray-2023.7.7.2/autoarray/fit/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/fit/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11054 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/fit/plot/fit_imaging_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22589 2023-06-03 16:41:28.000000 autoarray-2023.7.7.2/autoarray/fit/plot/fit_interferometer_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10437 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/fit/plot/fit_vector_yx_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13605 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/fixtures.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.974584 autoarray-2023.7.7.2/autoarray/geometry/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.2/autoarray/geometry/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1065 2023-05-11 17:33:46.000000 autoarray-2023.7.7.2/autoarray/geometry/abstract_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2768 2023-05-11 17:33:46.000000 autoarray-2023.7.7.2/autoarray/geometry/geometry_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12385 2023-05-11 17:33:46.000000 autoarray-2023.7.7.2/autoarray/geometry/geometry_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1687 2023-05-11 17:33:46.000000 autoarray-2023.7.7.2/autoarray/geometry/geometry_2d_irregular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27690 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/geometry/geometry_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.975582 autoarray-2023.7.7.2/autoarray/inversion/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-19 14:59:34.000000 autoarray-2023.7.7.2/autoarray/inversion/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.988582 autoarray-2023.7.7.2/autoarray/inversion/inversion/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-02-14 09:21:42.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35991 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15443 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/factory.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:37.999528 autoarray-2023.7.7.2/autoarray/inversion/inversion/imaging/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/imaging/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11938 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/imaging/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    34720 2023-06-03 09:10:24.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/imaging/inversion_imaging_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12033 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/imaging/mapping.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27386 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/imaging/w_tilde.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.012436 autoarray-2023.7.7.2/autoarray/inversion/inversion/interferometer/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/interferometer/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6128 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/interferometer/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5655 2023-03-13 18:37:33.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5331 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/interferometer/lop.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8257 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/interferometer/mapping.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9532 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/interferometer/w_tilde.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12793 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/inversion_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    42565 2023-06-07 09:55:12.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/inversion_util_secret.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    38687 2023-04-24 16:16:24.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/inversion_util_secret_clean.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4733 2023-06-03 09:10:24.000000 autoarray-2023.7.7.2/autoarray/inversion/inversion/settings.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.021434 autoarray-2023.7.7.2/autoarray/inversion/linear_obj/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/inversion/linear_obj/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4922 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/linear_obj/func_list.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7267 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/linear_obj/linear_obj.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1859 2022-12-21 17:08:33.000000 autoarray-2023.7.7.2/autoarray/inversion/linear_obj/neighbors.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1701 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/inversion/linear_obj/unique_mappings.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.040425 autoarray-2023.7.7.2/autoarray/inversion/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/inversion/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6792 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/mock/mock_inversion.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3080 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/mock/mock_inversion_imaging.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1132 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/mock/mock_inversion_interferometer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      888 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/mock/mock_linear_obj.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      912 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/mock/mock_linear_obj_func_list.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2270 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/inversion/mock/mock_mapper.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1675 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/inversion/mock/mock_mesh.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1023 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/inversion/mock/mock_pixelization.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      508 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/mock/mock_regularization.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.046230 autoarray-2023.7.7.2/autoarray/inversion/pixelization/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.064005 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21230 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10119 2023-03-13 19:00:38.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/delaunay.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3235 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/factory.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3665 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/mapper_grids.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    27357 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/mapper_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6780 2023-03-13 19:00:38.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/rectangular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    12734 2023-04-24 16:13:52.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/voronoi.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.081049 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      360 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5486 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13091 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/delaunay.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    24438 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/mesh_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7143 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/rectangular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4713 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/triangulation.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13162 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/voronoi.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5281 2022-12-22 08:54:23.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/voronoi_nn.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7677 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/pixelization.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1451 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/inversion/pixelization/settings.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.086115 autoarray-2023.7.7.2/autoarray/inversion/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/inversion/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10447 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/plot/inversion_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6803 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/plot/mapper_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.107976 autoarray-2023.7.7.2/autoarray/inversion/regularization/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      455 2023-04-01 14:36:25.000000 autoarray-2023.7.7.2/autoarray/inversion/regularization/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8894 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/inversion/regularization/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4728 2023-04-01 14:36:25.000000 autoarray-2023.7.7.2/autoarray/inversion/regularization/adaptive_brightness.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4508 2023-04-01 14:36:25.000000 autoarray-2023.7.7.2/autoarray/inversion/regularization/adaptive_brightness_split.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5208 2023-04-01 14:36:25.000000 autoarray-2023.7.7.2/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3391 2023-04-01 14:36:25.000000 autoarray-2023.7.7.2/autoarray/inversion/regularization/brightness_zeroth.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2964 2023-02-06 13:53:42.000000 autoarray-2023.7.7.2/autoarray/inversion/regularization/constant.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3226 2022-12-19 16:33:57.000000 autoarray-2023.7.7.2/autoarray/inversion/regularization/constant_split.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2187 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/regularization/constant_zeroth.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    15369 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/inversion/regularization/regularization_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3030 2023-02-06 13:53:42.000000 autoarray-2023.7.7.2/autoarray/inversion/regularization/zeroth.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.113956 autoarray-2023.7.7.2/autoarray/layout/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-06-17 13:08:16.000000 autoarray-2023.7.7.2/autoarray/layout/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11370 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/layout/layout.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7309 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/layout/layout_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14064 2023-05-25 17:19:43.000000 autoarray-2023.7.7.2/autoarray/layout/region.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.123949 autoarray-2023.7.7.2/autoarray/mask/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.2/autoarray/mask/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5222 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/mask/abstract_mask.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.135754 autoarray-2023.7.7.2/autoarray/mask/derive/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-12-29 16:03:57.000000 autoarray-2023.7.7.2/autoarray/mask/derive/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3485 2023-01-13 16:54:26.000000 autoarray-2023.7.7.2/autoarray/mask/derive/grid_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    16580 2023-01-13 16:54:26.000000 autoarray-2023.7.7.2/autoarray/mask/derive/grid_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21875 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/mask/derive/indexes_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5317 2023-01-13 16:54:26.000000 autoarray-2023.7.7.2/autoarray/mask/derive/mask_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21304 2023-01-13 16:54:26.000000 autoarray-2023.7.7.2/autoarray/mask/derive/mask_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5990 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/mask/mask_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3659 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/mask/mask_1d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    35868 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/mask/mask_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48943 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/mask/mask_2d_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.138754 autoarray-2023.7.7.2/autoarray/mask/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/mask/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/mask/mock/mock_mask.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1556 2023-02-12 10:43:58.000000 autoarray-2023.7.7.2/autoarray/mock.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4767 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/numba_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.145755 autoarray-2023.7.7.2/autoarray/operators/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-04-02 09:27:57.000000 autoarray-2023.7.7.2/autoarray/operators/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22050 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/operators/convolver.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.148754 autoarray-2023.7.7.2/autoarray/operators/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/operators/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      244 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/operators/mock/mock_convolver.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11017 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/operators/transformer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7717 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/operators/transformer_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.155551 autoarray-2023.7.7.2/autoarray/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3668 2023-06-03 09:03:18.000000 autoarray-2023.7.7.2/autoarray/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7455 2023-06-03 10:15:39.000000 autoarray-2023.7.7.2/autoarray/plot/abstract_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      477 2023-06-03 16:38:13.000000 autoarray-2023.7.7.2/autoarray/plot/auto_labels.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.162550 autoarray-2023.7.7.2/autoarray/plot/get_visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/get_visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2662 2022-12-21 17:08:33.000000 autoarray-2023.7.7.2/autoarray/plot/get_visuals/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2394 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/get_visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9159 2023-01-13 16:54:26.000000 autoarray-2023.7.7.2/autoarray/plot/get_visuals/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.170549 autoarray-2023.7.7.2/autoarray/plot/include/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/include/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1718 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/include/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1263 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/include/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4182 2022-12-21 13:25:52.000000 autoarray-2023.7.7.2/autoarray/plot/include/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.177441 autoarray-2023.7.7.2/autoarray/plot/mat_plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/mat_plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10623 2023-06-03 16:30:58.000000 autoarray-2023.7.7.2/autoarray/plot/mat_plot/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10971 2023-06-03 09:24:37.000000 autoarray-2023.7.7.2/autoarray/plot/mat_plot/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    26131 2023-06-04 12:43:35.000000 autoarray-2023.7.7.2/autoarray/plot/mat_plot/two_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2319 2023-05-15 17:44:36.000000 autoarray-2023.7.7.2/autoarray/plot/multi_plotters.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.185014 autoarray-2023.7.7.2/autoarray/plot/visuals/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/visuals/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2690 2023-05-12 10:15:02.000000 autoarray-2023.7.7.2/autoarray/plot/visuals/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1262 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/visuals/one_d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3396 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/visuals/two_d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.189012 autoarray-2023.7.7.2/autoarray/plot/wrap/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2250 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/__init__.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.223158 autoarray-2023.7.7.2/autoarray/plot/wrap/base/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      469 2023-02-12 10:45:24.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3900 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      544 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/annotate.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1900 2023-05-11 17:33:46.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/axis.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3736 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/cmap.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6309 2023-05-15 17:44:36.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/colorbar.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      446 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/colorbar_tickparams.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3042 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/figure.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2865 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/label.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      789 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/legend.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6068 2023-06-05 13:02:24.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/output.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      525 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/text.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      542 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/tickparams.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    13250 2023-06-05 13:24:35.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/ticks.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      910 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/title.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2166 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/base/units.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.235095 autoarray-2023.7.7.2/autoarray/plot/wrap/one_d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      133 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/one_d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      586 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/one_d/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1961 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/one_d/avxline.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1826 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/one_d/fill_between.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2802 2023-06-03 16:54:27.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/one_d/yx_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1168 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/one_d/yx_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    44375 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/segmentdata.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.275703 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      791 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      586 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      778 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/array_overlay.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      324 2022-12-29 16:03:57.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/border_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4685 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/grid_errorbar.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3733 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/grid_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6735 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/grid_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      316 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/index_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4542 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/interpolated_reconstruction.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      306 2022-12-29 16:03:57.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/mask_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      288 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/mesh_grid_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      310 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/origin_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      279 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/parallel_overscan_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1029 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/patch_overlay.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      321 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/positions_scatter.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      275 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/serial_overscan_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      273 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/serial_prescan_plot.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1222 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/vector_yx_quiver.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3220 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/voronoi_drawer.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22159 2023-06-06 10:32:10.000000 autoarray-2023.7.7.2/autoarray/preloads.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.284702 autoarray-2023.7.7.2/autoarray/structures/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-08-13 18:02:25.000000 autoarray-2023.7.7.2/autoarray/structures/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2955 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/abstract_structure.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.297873 autoarray-2023.7.7.2/autoarray/structures/arrays/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-11 15:40:14.000000 autoarray-2023.7.7.2/autoarray/structures/arrays/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9227 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/arrays/array_1d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    31344 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/arrays/array_2d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4901 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/arrays/irregular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18861 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/arrays/kernel_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11029 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/arrays/uniform_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    42401 2023-05-11 17:33:46.000000 autoarray-2023.7.7.2/autoarray/structures/arrays/uniform_2d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.316679 autoarray-2023.7.7.2/autoarray/structures/grids/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-03-11 15:32:21.000000 autoarray-2023.7.7.2/autoarray/structures/grids/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9412 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/grids/grid_1d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    32851 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/grids/grid_2d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18547 2023-05-12 10:10:35.000000 autoarray-2023.7.7.2/autoarray/structures/grids/irregular_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    41103 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/grids/iterate_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     8537 2023-05-11 09:40:23.000000 autoarray-2023.7.7.2/autoarray/structures/grids/sparse_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5498 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/grids/sparse_2d_util.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      256 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/grids/transformed_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18087 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/grids/uniform_1d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    48025 2023-05-11 17:33:46.000000 autoarray-2023.7.7.2/autoarray/structures/grids/uniform_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1579 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/header.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.327581 autoarray-2023.7.7.2/autoarray/structures/mesh/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/structures/mesh/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1500 2023-04-24 16:13:52.000000 autoarray-2023.7.7.2/autoarray/structures/mesh/abstract_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3544 2023-04-24 16:13:52.000000 autoarray-2023.7.7.2/autoarray/structures/mesh/delaunay_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7848 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/mesh/rectangular_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10536 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/mesh/triangulation_2d.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3645 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/mesh/voronoi_2d.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.333580 autoarray-2023.7.7.2/autoarray/structures/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/structures/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2679 2023-05-11 17:33:46.000000 autoarray-2023.7.7.2/autoarray/structures/mock/mock_grid.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10875 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/mock/mock_structure_decorators.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.338612 autoarray-2023.7.7.2/autoarray/structures/plot/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/structures/plot/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     7227 2022-11-11 15:49:29.000000 autoarray-2023.7.7.2/autoarray/structures/plot/structure_plotters.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22127 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/structure_decorators.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.345622 autoarray-2023.7.7.2/autoarray/structures/vectors/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/structures/vectors/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1028 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/vectors/abstract.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5747 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/vectors/irregular.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21670 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/structures/vectors/uniform.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     9550 2023-06-05 19:59:54.000000 autoarray-2023.7.7.2/autoarray/structures/visibilities.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1692 2023-04-24 16:13:52.000000 autoarray-2023.7.7.2/autoarray/type.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.352655 autoarray-2023.7.7.2/autoarray/util/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1273 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2646 2023-06-07 09:54:43.000000 autoarray-2023.7.7.2/autoarray/util/cholesky_funcs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5284 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/util/fnnls.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2603 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/misc_util.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.356655 autoarray-2023.7.7.2/autoarray/util/nn/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1731 2023-03-21 17:41:19.000000 autoarray-2023.7.7.2/autoarray/util/nn/README.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3897 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/autoarray/util/nn/nn_py.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.358656 autoarray-2023.7.7.2/autoarray/util/nn/src/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1248 2022-12-20 22:03:05.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/README.md
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.466570 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      558 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/.indent.pro
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     5420 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/CHANGELOG
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1190 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/CUSTOMISE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1343 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3231 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      166 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/config.h.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   141175 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/configure
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2745 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/configure.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    19071 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/delaunay.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1261 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/delaunay.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2408 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/delaunay_internal.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3877 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/distribute.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      717 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/distribute.h
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.469569 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.487091 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/1/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      233 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/1/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      603 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/1/generate.awk
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       64 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/1/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2810 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/1/suptitle.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/1/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1430 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/1/viewexample.m
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.514724 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1258 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   240932 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/data.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      518 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      835 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/mpitest.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2810 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/suptitle.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      760 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      997 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/viewdata.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1229 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/viewexample.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2958 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/viewinterp.m
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.528715 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/3/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1300 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/3/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      440 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/3/generate-data.awk
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      235 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/3/generate-points.awk
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       46 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/3/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      627 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/3/test.sh
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.551714 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      556 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   132840 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/data.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       56 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      740 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      999 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/viewdata.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1244 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/viewexample.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2966 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/viewinterp.m
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.574462 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/5/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      456 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/5/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)  1407289 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/5/data.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       54 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/5/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      461 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/5/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      536 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/5/viewexample.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2981 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/5/viewinterp.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2614 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/5/viewinterp2.m
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.592407 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/6/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      613 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/6/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   165065 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/6/data.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       45 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/6/makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      425 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/6/test.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       34 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/6/viewexample.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2979 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/6/viewinterp.m
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      655 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/README
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    22150 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/hash.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2040 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/hash.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4772 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/install-sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1398 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/istack.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      767 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/istack.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      600 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/istack_internal.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4154 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/lpi.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3271 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/makefile.example
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3217 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/makefile.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3145 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/makefile_autolens
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    36312 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/minell.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      920 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/minell.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      668 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/mkinstalldirs
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      891 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nan.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10955 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nn.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      949 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nn_internal.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    11021 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nnai.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    30764 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nnbathy.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2344 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nncommon-vulnerable.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14340 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nncommon.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      390 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nncommon.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nnconfig.h.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2220 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nnhpi_customized.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    40728 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nnpi.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      183 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nnpi.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     4699 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/preader.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      740 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/preader.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2326 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/sample.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)   652743 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/triangle.c
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    21562 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/triangle.h
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      425 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/autoarray/util/nn/src/nn/version.c
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.604480 autoarray-2023.7.7.2/autoarray.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    14122 2023-06-07 09:58:37.000000 autoarray-2023.7.7.2/autoarray.egg-info/SOURCES.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.598437 autoarray-2023.7.7.2/docs/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      654 2021-04-02 09:27:57.000000 autoarray-2023.7.7.2/docs/Makefile
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3624 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/docs/conf.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       26 2021-04-02 09:27:57.000000 autoarray-2023.7.7.2/docs/index.rst
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      795 2021-04-02 09:27:57.000000 autoarray-2023.7.7.2/docs/make.bat
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      148 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/eden.ini
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:58:38.602445 autoarray-2023.7.7.2/files/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       33 2021-06-17 13:08:16.000000 autoarray-2023.7.7.2/files/eden.ini
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      546 2021-04-02 09:27:57.000000 autoarray-2023.7.7.2/files/release.sh
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      626 2021-04-02 09:27:57.000000 autoarray-2023.7.7.2/files/to_do_list
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       39 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/optional_requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      210 2022-11-04 15:14:02.000000 autoarray-2023.7.7.2/readthedocs.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      141 2023-03-21 17:41:15.000000 autoarray-2023.7.7.2/requirements.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2023-06-07 09:58:38.605314 autoarray-2023.7.7.2/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2036 2023-06-07 09:57:48.000000 autoarray-2023.7.7.2/setup.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1572 2023-05-10 13:41:54.000000 autoarray-2023.7.7.2/to_do_list
```

### Comparing `autoarray-2023.7.7.1/.github/workflows/main.yml` & `autoarray-2023.7.7.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/LICENSE` & `autoarray-2023.7.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/PKG-INFO` & `autoarray-2023.7.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoarray
-Version: 2023.7.7.1
+Version: 2023.7.7.2
 Summary: PyAuto Data Structures
 Home-page: https://github.com/Jammy2211/PyAutoArray
 Author: James Nightingale and Richard Hayes
 Author-email: james.w.nightingale@durham.ac.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
```

### Comparing `autoarray-2023.7.7.1/autoarray/__init__.py` & `autoarray-2023.7.7.2/autoarray/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,8 @@
 from .structures.visibilities import Visibilities
 from .structures.visibilities import VisibilitiesNoiseMap
 
 from autoconf import conf
 
 conf.instance.register(__file__)
 
-__version__ = "2023.7.7.1"
+__version__ = "2023.7.7.2"
```

### Comparing `autoarray-2023.7.7.1/autoarray/abstract_ndarray.py` & `autoarray-2023.7.7.2/autoarray/abstract_ndarray.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/config/README.rst` & `autoarray-2023.7.7.2/autoarray/config/README.rst`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/config/general.yaml` & `autoarray-2023.7.7.2/autoarray/config/general.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/config/visualize/README.rst` & `autoarray-2023.7.7.2/autoarray/config/visualize/README.rst`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/config/visualize/general.yaml` & `autoarray-2023.7.7.2/autoarray/config/visualize/general.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/config/visualize/include.yaml` & `autoarray-2023.7.7.2/autoarray/config/visualize/include.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/config/visualize/mat_wrap.yaml` & `autoarray-2023.7.7.2/autoarray/config/visualize/mat_wrap.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/config/visualize/mat_wrap_1d.yaml` & `autoarray-2023.7.7.2/autoarray/config/visualize/mat_wrap_1d.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/config/visualize/mat_wrap_2d.yaml` & `autoarray-2023.7.7.2/autoarray/config/visualize/mat_wrap_2d.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/config/visualize/plots.yaml` & `autoarray-2023.7.7.2/autoarray/config/visualize/plots.yaml`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/abstract/dataset.py` & `autoarray-2023.7.7.2/autoarray/dataset/abstract/dataset.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/abstract/settings.py` & `autoarray-2023.7.7.2/autoarray/dataset/abstract/settings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/abstract/w_tilde.py` & `autoarray-2023.7.7.2/autoarray/dataset/abstract/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/imaging/imaging.py` & `autoarray-2023.7.7.2/autoarray/dataset/imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/imaging/settings.py` & `autoarray-2023.7.7.2/autoarray/dataset/imaging/settings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/imaging/simulator.py` & `autoarray-2023.7.7.2/autoarray/dataset/imaging/simulator.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/imaging/w_tilde.py` & `autoarray-2023.7.7.2/autoarray/dataset/imaging/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/interferometer/interferometer.py` & `autoarray-2023.7.7.2/autoarray/dataset/interferometer/interferometer.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/interferometer/settings.py` & `autoarray-2023.7.7.2/autoarray/dataset/interferometer/settings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/interferometer/simulator.py` & `autoarray-2023.7.7.2/autoarray/dataset/interferometer/simulator.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/interferometer/w_tilde.py` & `autoarray-2023.7.7.2/autoarray/dataset/interferometer/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/plot/imaging_plotters.py` & `autoarray-2023.7.7.2/autoarray/dataset/plot/imaging_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/plot/interferometer_plotters.py` & `autoarray-2023.7.7.2/autoarray/dataset/plot/interferometer_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/dataset/preprocess.py` & `autoarray-2023.7.7.2/autoarray/dataset/preprocess.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/exc.py` & `autoarray-2023.7.7.2/autoarray/exc.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/fit/fit_dataset.py` & `autoarray-2023.7.7.2/autoarray/fit/fit_dataset.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/fit/fit_imaging.py` & `autoarray-2023.7.7.2/autoarray/fit/fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/fit/fit_interferometer.py` & `autoarray-2023.7.7.2/autoarray/fit/fit_interferometer.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/fit/fit_util.py` & `autoarray-2023.7.7.2/autoarray/fit/fit_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/fit/mock/mock_fit_imaging.py` & `autoarray-2023.7.7.2/autoarray/fit/mock/mock_fit_imaging.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/fit/mock/mock_fit_interferometer.py` & `autoarray-2023.7.7.2/autoarray/fit/mock/mock_fit_interferometer.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/fit/plot/fit_imaging_plotters.py` & `autoarray-2023.7.7.2/autoarray/fit/plot/fit_imaging_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/fit/plot/fit_interferometer_plotters.py` & `autoarray-2023.7.7.2/autoarray/fit/plot/fit_interferometer_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/fit/plot/fit_vector_yx_plotters.py` & `autoarray-2023.7.7.2/autoarray/fit/plot/fit_vector_yx_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/fixtures.py` & `autoarray-2023.7.7.2/autoarray/fixtures.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/geometry/abstract_2d.py` & `autoarray-2023.7.7.2/autoarray/geometry/abstract_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/geometry/geometry_1d.py` & `autoarray-2023.7.7.2/autoarray/geometry/geometry_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/geometry/geometry_2d.py` & `autoarray-2023.7.7.2/autoarray/geometry/geometry_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/geometry/geometry_2d_irregular.py` & `autoarray-2023.7.7.2/autoarray/geometry/geometry_2d_irregular.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/geometry/geometry_util.py` & `autoarray-2023.7.7.2/autoarray/geometry/geometry_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/abstract.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/factory.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/factory.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/abstract.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/imaging/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/inversion_imaging_util.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/imaging/inversion_imaging_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/mapping.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/imaging/mapping.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/imaging/w_tilde.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/imaging/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/abstract.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/interferometer/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/interferometer/inversion_interferometer_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/lop.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/interferometer/lop.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/mapping.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/interferometer/mapping.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/interferometer/w_tilde.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/interferometer/w_tilde.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/inversion_util.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/inversion_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/inversion_util_secret.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/inversion_util_secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 
 from typing import Tuple
 
 from autoarray import numba_util
 
 logger = logging.getLogger(__name__)
 
-import numba
-
-
 @numba_util.jit()
 def w_tilde_data_interferometer_from(
     visibilities_real: np.ndarray,
     noise_map_real: np.ndarray,
     uv_wavelengths: np.ndarray,
     grid_radians_slim: np.ndarray,
     native_index_for_slim_index,
```

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/inversion_util_secret_clean.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/inversion_util_secret_clean.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/inversion/settings.py` & `autoarray-2023.7.7.2/autoarray/inversion/inversion/settings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/linear_obj/func_list.py` & `autoarray-2023.7.7.2/autoarray/inversion/linear_obj/func_list.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/linear_obj/linear_obj.py` & `autoarray-2023.7.7.2/autoarray/inversion/linear_obj/linear_obj.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/linear_obj/neighbors.py` & `autoarray-2023.7.7.2/autoarray/inversion/linear_obj/neighbors.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/linear_obj/unique_mappings.py` & `autoarray-2023.7.7.2/autoarray/inversion/linear_obj/unique_mappings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_inversion.py` & `autoarray-2023.7.7.2/autoarray/inversion/mock/mock_inversion.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_inversion_imaging.py` & `autoarray-2023.7.7.2/autoarray/inversion/mock/mock_inversion_imaging.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_inversion_interferometer.py` & `autoarray-2023.7.7.2/autoarray/inversion/mock/mock_inversion_interferometer.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_linear_obj.py` & `autoarray-2023.7.7.2/autoarray/inversion/mock/mock_linear_obj.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_linear_obj_func_list.py` & `autoarray-2023.7.7.2/autoarray/inversion/mock/mock_linear_obj_func_list.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_mapper.py` & `autoarray-2023.7.7.2/autoarray/inversion/mock/mock_mapper.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_mesh.py` & `autoarray-2023.7.7.2/autoarray/inversion/mock/mock_mesh.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/mock/mock_pixelization.py` & `autoarray-2023.7.7.2/autoarray/inversion/mock/mock_pixelization.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/abstract.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/delaunay.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/delaunay.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/factory.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/factory.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/mapper_grids.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/mapper_grids.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/mapper_util.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/mapper_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/rectangular.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/rectangular.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mappers/voronoi.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mappers/voronoi.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/abstract.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/delaunay.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/delaunay.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/mesh_util.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/mesh_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/rectangular.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/rectangular.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/triangulation.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/triangulation.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/voronoi.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/voronoi.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/mesh/voronoi_nn.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/mesh/voronoi_nn.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/pixelization.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/pixelization.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/pixelization/settings.py` & `autoarray-2023.7.7.2/autoarray/inversion/pixelization/settings.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/plot/inversion_plotters.py` & `autoarray-2023.7.7.2/autoarray/inversion/plot/inversion_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/plot/mapper_plotters.py` & `autoarray-2023.7.7.2/autoarray/inversion/plot/mapper_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/regularization/abstract.py` & `autoarray-2023.7.7.2/autoarray/inversion/regularization/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/regularization/adaptive_brightness.py` & `autoarray-2023.7.7.2/autoarray/inversion/regularization/adaptive_brightness.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/regularization/adaptive_brightness_split.py` & `autoarray-2023.7.7.2/autoarray/inversion/regularization/adaptive_brightness_split.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py` & `autoarray-2023.7.7.2/autoarray/inversion/regularization/adaptive_brightness_split_zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/regularization/brightness_zeroth.py` & `autoarray-2023.7.7.2/autoarray/inversion/regularization/brightness_zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/regularization/constant.py` & `autoarray-2023.7.7.2/autoarray/inversion/regularization/constant.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/regularization/constant_split.py` & `autoarray-2023.7.7.2/autoarray/inversion/regularization/constant_split.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/regularization/constant_zeroth.py` & `autoarray-2023.7.7.2/autoarray/inversion/regularization/constant_zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/regularization/regularization_util.py` & `autoarray-2023.7.7.2/autoarray/inversion/regularization/regularization_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/inversion/regularization/zeroth.py` & `autoarray-2023.7.7.2/autoarray/inversion/regularization/zeroth.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/layout/layout.py` & `autoarray-2023.7.7.2/autoarray/layout/layout.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/layout/layout_util.py` & `autoarray-2023.7.7.2/autoarray/layout/layout_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/layout/region.py` & `autoarray-2023.7.7.2/autoarray/layout/region.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/mask/abstract_mask.py` & `autoarray-2023.7.7.2/autoarray/mask/abstract_mask.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/mask/derive/grid_1d.py` & `autoarray-2023.7.7.2/autoarray/mask/derive/grid_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/mask/derive/grid_2d.py` & `autoarray-2023.7.7.2/autoarray/mask/derive/grid_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/mask/derive/indexes_2d.py` & `autoarray-2023.7.7.2/autoarray/mask/derive/indexes_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/mask/derive/mask_1d.py` & `autoarray-2023.7.7.2/autoarray/mask/derive/mask_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/mask/derive/mask_2d.py` & `autoarray-2023.7.7.2/autoarray/mask/derive/mask_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/mask/mask_1d.py` & `autoarray-2023.7.7.2/autoarray/mask/mask_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/mask/mask_1d_util.py` & `autoarray-2023.7.7.2/autoarray/mask/mask_1d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/mask/mask_2d.py` & `autoarray-2023.7.7.2/autoarray/mask/mask_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/mask/mask_2d_util.py` & `autoarray-2023.7.7.2/autoarray/mask/mask_2d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/mock.py` & `autoarray-2023.7.7.2/autoarray/mock.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/numba_util.py` & `autoarray-2023.7.7.2/autoarray/numba_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/operators/convolver.py` & `autoarray-2023.7.7.2/autoarray/operators/convolver.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/operators/transformer.py` & `autoarray-2023.7.7.2/autoarray/operators/transformer.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/operators/transformer_util.py` & `autoarray-2023.7.7.2/autoarray/operators/transformer_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/__init__.py` & `autoarray-2023.7.7.2/autoarray/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/abstract_plotters.py` & `autoarray-2023.7.7.2/autoarray/plot/abstract_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/get_visuals/abstract.py` & `autoarray-2023.7.7.2/autoarray/plot/get_visuals/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/get_visuals/one_d.py` & `autoarray-2023.7.7.2/autoarray/plot/get_visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/get_visuals/two_d.py` & `autoarray-2023.7.7.2/autoarray/plot/get_visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/include/abstract.py` & `autoarray-2023.7.7.2/autoarray/plot/include/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/include/one_d.py` & `autoarray-2023.7.7.2/autoarray/plot/include/one_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/include/two_d.py` & `autoarray-2023.7.7.2/autoarray/plot/include/two_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/mat_plot/abstract.py` & `autoarray-2023.7.7.2/autoarray/plot/mat_plot/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/mat_plot/one_d.py` & `autoarray-2023.7.7.2/autoarray/plot/mat_plot/one_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/mat_plot/two_d.py` & `autoarray-2023.7.7.2/autoarray/plot/mat_plot/two_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/multi_plotters.py` & `autoarray-2023.7.7.2/autoarray/plot/multi_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/visuals/abstract.py` & `autoarray-2023.7.7.2/autoarray/plot/visuals/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/visuals/one_d.py` & `autoarray-2023.7.7.2/autoarray/plot/visuals/one_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/visuals/two_d.py` & `autoarray-2023.7.7.2/autoarray/plot/visuals/two_d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/__init__.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/__init__.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/abstract.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/annotate.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/annotate.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/axis.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/axis.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/cmap.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/cmap.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/colorbar.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/colorbar.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/figure.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/figure.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/label.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/label.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/legend.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/legend.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/output.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/output.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/text.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/text.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/tickparams.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/tickparams.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/ticks.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/ticks.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/title.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/title.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/base/units.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/base/units.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/abstract.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/one_d/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/avxline.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/one_d/avxline.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/fill_between.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/one_d/fill_between.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/yx_plot.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/one_d/yx_plot.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/one_d/yx_scatter.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/one_d/yx_scatter.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/segmentdata.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/segmentdata.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/__init__.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/__init__.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/abstract.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/array_overlay.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/array_overlay.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/grid_errorbar.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/grid_errorbar.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/grid_plot.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/grid_plot.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/grid_scatter.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/grid_scatter.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/interpolated_reconstruction.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/interpolated_reconstruction.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/patch_overlay.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/patch_overlay.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/vector_yx_quiver.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/vector_yx_quiver.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/plot/wrap/two_d/voronoi_drawer.py` & `autoarray-2023.7.7.2/autoarray/plot/wrap/two_d/voronoi_drawer.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/preloads.py` & `autoarray-2023.7.7.2/autoarray/preloads.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/abstract_structure.py` & `autoarray-2023.7.7.2/autoarray/structures/abstract_structure.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/arrays/array_1d_util.py` & `autoarray-2023.7.7.2/autoarray/structures/arrays/array_1d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/arrays/array_2d_util.py` & `autoarray-2023.7.7.2/autoarray/structures/arrays/array_2d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/arrays/irregular.py` & `autoarray-2023.7.7.2/autoarray/structures/arrays/irregular.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/arrays/kernel_2d.py` & `autoarray-2023.7.7.2/autoarray/structures/arrays/kernel_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/arrays/uniform_1d.py` & `autoarray-2023.7.7.2/autoarray/structures/arrays/uniform_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/arrays/uniform_2d.py` & `autoarray-2023.7.7.2/autoarray/structures/arrays/uniform_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/grids/grid_1d_util.py` & `autoarray-2023.7.7.2/autoarray/structures/grids/grid_1d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/grids/grid_2d_util.py` & `autoarray-2023.7.7.2/autoarray/structures/grids/grid_2d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/grids/irregular_2d.py` & `autoarray-2023.7.7.2/autoarray/structures/grids/irregular_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/grids/iterate_2d.py` & `autoarray-2023.7.7.2/autoarray/structures/grids/iterate_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/grids/sparse_2d.py` & `autoarray-2023.7.7.2/autoarray/structures/grids/sparse_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/grids/sparse_2d_util.py` & `autoarray-2023.7.7.2/autoarray/structures/grids/sparse_2d_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/grids/uniform_1d.py` & `autoarray-2023.7.7.2/autoarray/structures/grids/uniform_1d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/grids/uniform_2d.py` & `autoarray-2023.7.7.2/autoarray/structures/grids/uniform_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/header.py` & `autoarray-2023.7.7.2/autoarray/structures/header.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/mesh/abstract_2d.py` & `autoarray-2023.7.7.2/autoarray/structures/mesh/abstract_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/mesh/delaunay_2d.py` & `autoarray-2023.7.7.2/autoarray/structures/mesh/delaunay_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/mesh/rectangular_2d.py` & `autoarray-2023.7.7.2/autoarray/structures/mesh/rectangular_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/mesh/triangulation_2d.py` & `autoarray-2023.7.7.2/autoarray/structures/mesh/triangulation_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/mesh/voronoi_2d.py` & `autoarray-2023.7.7.2/autoarray/structures/mesh/voronoi_2d.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/mock/mock_grid.py` & `autoarray-2023.7.7.2/autoarray/structures/mock/mock_grid.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/mock/mock_structure_decorators.py` & `autoarray-2023.7.7.2/autoarray/structures/mock/mock_structure_decorators.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/plot/structure_plotters.py` & `autoarray-2023.7.7.2/autoarray/structures/plot/structure_plotters.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/structure_decorators.py` & `autoarray-2023.7.7.2/autoarray/structures/structure_decorators.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/vectors/abstract.py` & `autoarray-2023.7.7.2/autoarray/structures/vectors/abstract.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/vectors/irregular.py` & `autoarray-2023.7.7.2/autoarray/structures/vectors/irregular.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/vectors/uniform.py` & `autoarray-2023.7.7.2/autoarray/structures/vectors/uniform.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/structures/visibilities.py` & `autoarray-2023.7.7.2/autoarray/structures/visibilities.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/type.py` & `autoarray-2023.7.7.2/autoarray/type.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/__init__.py` & `autoarray-2023.7.7.2/autoarray/util/__init__.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/cholesky_funcs.py` & `autoarray-2023.7.7.2/autoarray/util/cholesky_funcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from scipy import linalg
 import math
 import time
-from numba import njit
+from autoarray import numba_util
 
 
-@njit(fastmath=True)
+@numba_util.jit()
 def _choldowndate(U, x):
     n = x.size
     for k in range(n - 1):
         Ukk = U[k, k]
         xk = x[k]
         r = math.sqrt(Ukk**2 - xk**2)
         c = r / Ukk
@@ -19,15 +19,15 @@
         x[k + 1 :] = c * x[k + 1 :] - s * U[k, k + 1 :]
 
     k = n - 1
     U[k, k] = math.sqrt(U[k, k] ** 2 - x[k] ** 2)
     return U
 
 
-@njit(fastmath=True)
+@numba_util.jit()
 def _cholupdate(U, x):
     n = x.size
     for k in range(n - 1):
         Ukk = U[k, k]
         xk = x[k]
 
         r = np.sqrt(Ukk**2 + xk**2)
```

### Comparing `autoarray-2023.7.7.1/autoarray/util/fnnls.py` & `autoarray-2023.7.7.2/autoarray/util/fnnls.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/misc_util.py` & `autoarray-2023.7.7.2/autoarray/util/misc_util.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/README.md` & `autoarray-2023.7.7.2/autoarray/util/nn/README.md`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/nn_py.py` & `autoarray-2023.7.7.2/autoarray/util/nn/nn_py.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/README.md` & `autoarray-2023.7.7.2/autoarray/util/nn/src/README.md`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/.indent.pro` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/.indent.pro`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/CHANGELOG` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/CHANGELOG`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/CUSTOMISE` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/CUSTOMISE`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/LICENSE` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/LICENSE`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/README` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/README`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/configure` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/configure`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/configure.in` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/configure.in`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/delaunay.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/delaunay.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/delaunay.h` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/delaunay.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/delaunay_internal.h` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/delaunay_internal.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/distribute.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/distribute.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/distribute.h` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/distribute.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/generate.awk` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/1/generate.awk`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/suptitle.m` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/1/suptitle.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/test.sh` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/1/test.sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/1/viewexample.m` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/1/viewexample.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/README` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/README`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/data.txt` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/data.txt`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/makefile` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/makefile`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/mpitest.sh` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/mpitest.sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/suptitle.m` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/suptitle.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/test.sh` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/test.sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/viewdata.m` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/viewdata.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/viewexample.m` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/viewexample.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/2/viewinterp.m` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/2/viewinterp.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/README` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/3/README`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/3/test.sh` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/3/test.sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/README` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/README`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/data.txt` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/data.txt`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/test.sh` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/test.sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/viewdata.m` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/viewdata.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/viewexample.m` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/viewexample.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/4/viewinterp.m` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/4/viewinterp.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/data.txt` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/5/data.txt`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/viewexample.m` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/5/viewexample.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/viewinterp.m` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/5/viewinterp.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/5/viewinterp2.m` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/5/viewinterp2.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/README` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/6/README`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/data.txt` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/6/data.txt`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/6/viewinterp.m` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/6/viewinterp.m`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/examples/README` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/examples/README`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/hash.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/hash.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/hash.h` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/hash.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/install-sh` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/install-sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/istack.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/istack.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/istack.h` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/istack.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/istack_internal.h` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/istack_internal.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/lpi.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/lpi.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/makefile.example` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/makefile.example`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/makefile.in` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/makefile.in`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/makefile_autolens` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/makefile_autolens`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/minell.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/minell.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/minell.h` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/minell.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/mkinstalldirs` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/mkinstalldirs`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nan.h` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nan.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nn.h` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nn.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nn_internal.h` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nn_internal.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnai.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nnai.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnbathy.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nnbathy.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nncommon-vulnerable.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nncommon-vulnerable.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nncommon.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nncommon.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnhpi_customized.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nnhpi_customized.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/nnpi.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/nnpi.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/preader.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/preader.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/preader.h` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/preader.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/sample.py` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/sample.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/triangle.c` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/triangle.c`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray/util/nn/src/nn/triangle.h` & `autoarray-2023.7.7.2/autoarray/util/nn/src/nn/triangle.h`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/autoarray.egg-info/SOURCES.txt` & `autoarray-2023.7.7.2/autoarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/docs/Makefile` & `autoarray-2023.7.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/docs/conf.py` & `autoarray-2023.7.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/docs/make.bat` & `autoarray-2023.7.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/files/release.sh` & `autoarray-2023.7.7.2/files/release.sh`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/files/to_do_list` & `autoarray-2023.7.7.2/files/to_do_list`

 * *Files identical despite different names*

### Comparing `autoarray-2023.7.7.1/setup.py` & `autoarray-2023.7.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, "README.rst"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
-version = environ.get("VERSION", "2023.7.7.1")
+version = environ.get("VERSION", "2023.7.7.2")
 requirements.extend([f"autoconf=={version}"])
 
 
 def config_packages(directory):
     paths = [directory.replace("/", ".")]
     for path, directories, filenames in os.walk(directory):
         for directory in directories:
```

### Comparing `autoarray-2023.7.7.1/to_do_list` & `autoarray-2023.7.7.2/to_do_list`

 * *Files identical despite different names*

