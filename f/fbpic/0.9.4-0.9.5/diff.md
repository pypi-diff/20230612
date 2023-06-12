# Comparing `tmp/fbpic-0.9.4.tar.gz` & `tmp/fbpic-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fbpic-0.9.4.tar", last modified: Mon Aug  6 16:26:36 2018, max compression
+gzip compressed data, was "dist/fbpic-0.9.5.tar", last modified: Fri Oct  5 16:29:58 2018, max compression
```

## Comparing `fbpic-0.9.4.tar` & `fbpic-0.9.5.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     5161 2018-08-06 16:21:09.000000 fbpic-0.9.4/README.md
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)       38 2018-08-06 16:26:36.000000 fbpic-0.9.4/setup.cfg
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     1860 2018-08-02 21:22:34.000000 fbpic-0.9.4/setup.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic.egg-info/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)       39 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic.egg-info/requires.txt
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)        6 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic.egg-info/top_level.txt
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)        1 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic.egg-info/dependency_links.txt
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     3678 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic.egg-info/SOURCES.txt
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     6952 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic.egg-info/PKG-INFO
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)       39 2018-07-20 16:39:35.000000 fbpic-0.9.4/requirements.txt
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/particles/
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/particles/elementary_process/
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/particles/elementary_process/compton/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    11509 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/elementary_process/compton/compton.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    12765 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/elementary_process/compton/numba_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     4819 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/elementary_process/compton/inline_functions.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)      188 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/elementary_process/compton/__init__.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    12725 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/elementary_process/compton/cuda_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     5810 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/particles/elementary_process/cuda_numba_utils.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/particles/elementary_process/ionization/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     5338 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/particles/elementary_process/ionization/numba_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     4577 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/particles/elementary_process/ionization/inline_functions.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)      210 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/elementary_process/ionization/__init__.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    33649 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/elementary_process/ionization/atomic_data.txt
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     3497 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/elementary_process/ionization/read_atomic_data.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    16467 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/particles/elementary_process/ionization/ionizer.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     4938 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/particles/elementary_process/ionization/cuda_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)        0 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/elementary_process/__init__.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/particles/injection/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    12417 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/injection/continuous_injection.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)      392 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/injection/__init__.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     2142 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/injection/ballistic_before_plane.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/particles/deposition/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    28543 2018-08-02 21:27:22.000000 fbpic-0.9.4/fbpic/particles/deposition/threading_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    44365 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/deposition/cuda_methods_one_mode.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     2403 2018-08-02 21:27:22.000000 fbpic-0.9.4/fbpic/particles/deposition/numba_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)        0 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/deposition/__init__.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    59181 2018-08-02 21:27:22.000000 fbpic-0.9.4/fbpic/particles/deposition/cuda_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    46694 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/particles/particles.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/particles/gathering/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    11133 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/particles/gathering/threading_methods_one_mode.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    12167 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/particles/gathering/threading_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    10674 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/particles/gathering/cuda_methods_one_mode.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     6575 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/particles/gathering/inline_functions.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)        0 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/gathering/__init__.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    11475 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/particles/gathering/cuda_methods.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/particles/push/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     3355 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/particles/push/numba_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     1499 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/particles/push/inline_functions.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)        0 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/push/__init__.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     4918 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/particles/push/cuda_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)      248 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/__init__.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/particles/tracking/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     5838 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/tracking/tracking.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)      237 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/tracking/__init__.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/particles/utilities/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     6302 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/utilities/cuda_sorting.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)        0 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/utilities/__init__.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     3539 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/particles/utilities/utility_methods.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/boundaries/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    11099 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/boundaries/moving_window.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    18806 2018-08-02 21:22:34.000000 fbpic-0.9.4/fbpic/boundaries/field_buffer_handling.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    46242 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/boundaries/boundary_communicator.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    29294 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/boundaries/particle_buffer_handling.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)      321 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/boundaries/__init__.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    15718 2018-08-02 21:27:22.000000 fbpic-0.9.4/fbpic/boundaries/cuda_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)      502 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/__init__.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/lpa_utils/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     9434 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/lpa_utils/boosted_frame.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/lpa_utils/laser/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    27873 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/lpa_utils/laser/laser_profiles.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)      491 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/lpa_utils/laser/__init__.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     8317 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/lpa_utils/laser/laser.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    22806 2018-08-02 21:22:34.000000 fbpic-0.9.4/fbpic/lpa_utils/laser/antenna_injection.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     9114 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/lpa_utils/laser/direct_injection.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)        0 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/lpa_utils/__init__.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     5123 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/lpa_utils/external_fields.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    21563 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/lpa_utils/bunch.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/openpmd_diag/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    12550 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/openpmd_diag/checkpoint_restart.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     6712 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/openpmd_diag/generic_diag.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     4363 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/openpmd_diag/particle_density_diag.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    13579 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/openpmd_diag/field_diag.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)      722 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/openpmd_diag/__init__.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    37399 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/openpmd_diag/boosted_particle_diag.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    18174 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/openpmd_diag/particle_diag.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     1466 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/openpmd_diag/data_dict.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    32587 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/openpmd_diag/boosted_field_diag.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     4979 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/openpmd_diag/cuda_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    40780 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/main.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/fields/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    17774 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/fields/spectral_grid.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     7751 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/fields/interpolation_grid.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     6706 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/fields/psatd_coefs.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    15010 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/fields/numba_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)      268 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/fields/__init__.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/fields/spectral_transform/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     6477 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/fields/spectral_transform/fourier.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     9195 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/fields/spectral_transform/hankel.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     9693 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/fields/spectral_transform/spectral_transformer.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     3695 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/fields/spectral_transform/numba_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)      296 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/fields/spectral_transform/__init__.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     5537 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/fields/spectral_transform/mkl_fft.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     4887 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/fields/spectral_transform/cuda_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     7432 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/fields/utility_methods.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    23569 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/fields/fields.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    15478 2018-08-06 15:57:36.000000 fbpic-0.9.4/fbpic/fields/cuda_methods.py
-drwxrwxr-x   0 rlehe     (1001) rlehe     (1001)        0 2018-08-06 16:26:36.000000 fbpic-0.9.4/fbpic/utils/
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     2112 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/utils/mpi.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)        0 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/utils/__init__.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     3436 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/utils/cuda.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     3050 2018-08-06 16:21:09.000000 fbpic-0.9.4/fbpic/utils/threading.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)    12254 2018-07-20 16:39:35.000000 fbpic-0.9.4/fbpic/utils/printing.py
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)      113 2018-07-20 16:39:35.000000 fbpic-0.9.4/MANIFEST.in
--rw-rw-r--   0 rlehe     (1001) rlehe     (1001)     6952 2018-08-06 16:26:36.000000 fbpic-0.9.4/PKG-INFO
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/
+-rw-r--r--   0 rlehe      (501) staff       (20)      502 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/__init__.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/boundaries/
+-rw-r--r--   0 rlehe      (501) staff       (20)      321 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/boundaries/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    46242 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/boundaries/boundary_communicator.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    15718 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/boundaries/cuda_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    18806 2018-08-18 00:08:46.000000 fbpic-0.9.5/fbpic/boundaries/field_buffer_handling.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    11099 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/boundaries/moving_window.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    29294 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/boundaries/particle_buffer_handling.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/fields/
+-rw-r--r--   0 rlehe      (501) staff       (20)      268 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/fields/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    15478 2018-09-22 21:25:59.000000 fbpic-0.9.5/fbpic/fields/cuda_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    23569 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/fields/fields.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     7751 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/fields/interpolation_grid.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    15010 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/fields/numba_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     6706 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/fields/psatd_coefs.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    17774 2018-09-22 21:25:59.000000 fbpic-0.9.5/fbpic/fields/spectral_grid.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/fields/spectral_transform/
+-rw-r--r--   0 rlehe      (501) staff       (20)      296 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/fields/spectral_transform/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     4887 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/fields/spectral_transform/cuda_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     6477 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/fields/spectral_transform/fourier.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     9195 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/fields/spectral_transform/hankel.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     5537 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/fields/spectral_transform/mkl_fft.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     3695 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/fields/spectral_transform/numba_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     9693 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/fields/spectral_transform/spectral_transformer.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     7696 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/fields/utility_methods.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/lpa_utils/
+-rw-r--r--   0 rlehe      (501) staff       (20)        0 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/lpa_utils/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     9434 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/lpa_utils/boosted_frame.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    21650 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/lpa_utils/bunch.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     5123 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/lpa_utils/external_fields.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/lpa_utils/laser/
+-rw-r--r--   0 rlehe      (501) staff       (20)      491 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/lpa_utils/laser/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    22806 2018-08-18 00:08:46.000000 fbpic-0.9.5/fbpic/lpa_utils/laser/antenna_injection.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     9114 2018-06-25 00:38:36.000000 fbpic-0.9.5/fbpic/lpa_utils/laser/direct_injection.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     8317 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/lpa_utils/laser/laser.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    27873 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/lpa_utils/laser/laser_profiles.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    40780 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/main.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/openpmd_diag/
+-rw-r--r--   0 rlehe      (501) staff       (20)      722 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/openpmd_diag/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    32587 2018-08-25 01:30:23.000000 fbpic-0.9.5/fbpic/openpmd_diag/boosted_field_diag.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    37399 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/openpmd_diag/boosted_particle_diag.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    12550 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/openpmd_diag/checkpoint_restart.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     4979 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/openpmd_diag/cuda_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     1466 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/openpmd_diag/data_dict.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    13579 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/openpmd_diag/field_diag.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     6712 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/openpmd_diag/generic_diag.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     4363 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/openpmd_diag/particle_density_diag.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    18174 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/openpmd_diag/particle_diag.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/particles/
+-rw-r--r--   0 rlehe      (501) staff       (20)      248 2018-08-03 18:07:20.000000 fbpic-0.9.5/fbpic/particles/__init__.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/particles/deposition/
+-rw-r--r--   0 rlehe      (501) staff       (20)        0 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/deposition/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    59181 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/particles/deposition/cuda_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    44365 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/deposition/cuda_methods_one_mode.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     2403 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/particles/deposition/numba_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    28539 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/particles/deposition/threading_methods.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/particles/elementary_process/
+-rw-r--r--   0 rlehe      (501) staff       (20)        0 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/elementary_process/__init__.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/particles/elementary_process/compton/
+-rw-r--r--   0 rlehe      (501) staff       (20)      188 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/elementary_process/compton/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    11509 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/elementary_process/compton/compton.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    12725 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/elementary_process/compton/cuda_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     4819 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/elementary_process/compton/inline_functions.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    12765 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/elementary_process/compton/numba_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     5810 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/particles/elementary_process/cuda_numba_utils.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/particles/elementary_process/ionization/
+-rw-r--r--   0 rlehe      (501) staff       (20)      210 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/elementary_process/ionization/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    33649 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/elementary_process/ionization/atomic_data.txt
+-rw-r--r--   0 rlehe      (501) staff       (20)     4938 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/particles/elementary_process/ionization/cuda_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     4577 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/particles/elementary_process/ionization/inline_functions.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    16467 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/particles/elementary_process/ionization/ionizer.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     5338 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/particles/elementary_process/ionization/numba_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     3497 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/elementary_process/ionization/read_atomic_data.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/particles/gathering/
+-rw-r--r--   0 rlehe      (501) staff       (20)        0 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/gathering/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    11475 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/particles/gathering/cuda_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    10674 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/particles/gathering/cuda_methods_one_mode.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     6575 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/particles/gathering/inline_functions.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    12167 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/particles/gathering/threading_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    11133 2018-09-20 15:00:35.000000 fbpic-0.9.5/fbpic/particles/gathering/threading_methods_one_mode.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/particles/injection/
+-rw-r--r--   0 rlehe      (501) staff       (20)      392 2018-08-03 18:07:20.000000 fbpic-0.9.5/fbpic/particles/injection/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     2142 2018-07-19 20:21:10.000000 fbpic-0.9.5/fbpic/particles/injection/ballistic_before_plane.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    12417 2018-08-03 18:07:20.000000 fbpic-0.9.5/fbpic/particles/injection/continuous_injection.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    46678 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/particles/particles.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/particles/push/
+-rw-r--r--   0 rlehe      (501) staff       (20)        0 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/push/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     4918 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/particles/push/cuda_methods.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     1499 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/particles/push/inline_functions.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     3355 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/particles/push/numba_methods.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/particles/tracking/
+-rw-r--r--   0 rlehe      (501) staff       (20)      237 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/tracking/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     5838 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/tracking/tracking.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/particles/utilities/
+-rw-r--r--   0 rlehe      (501) staff       (20)        0 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/utilities/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     6302 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/utilities/cuda_sorting.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     3539 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/particles/utilities/utility_methods.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic/utils/
+-rw-r--r--   0 rlehe      (501) staff       (20)        0 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/utils/__init__.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     3436 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/utils/cuda.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     2112 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/utils/mpi.py
+-rw-r--r--   0 rlehe      (501) staff       (20)    12254 2018-06-08 22:18:19.000000 fbpic-0.9.5/fbpic/utils/printing.py
+-rw-r--r--   0 rlehe      (501) staff       (20)     3050 2018-10-05 16:17:32.000000 fbpic-0.9.5/fbpic/utils/threading.py
+drwxr-xr-x   0 rlehe      (501) staff       (20)        0 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic.egg-info/
+-rw-r--r--   0 rlehe      (501) staff       (20)        1 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic.egg-info/dependency_links.txt
+-rw-r--r--   0 rlehe      (501) staff       (20)     6953 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic.egg-info/PKG-INFO
+-rw-r--r--   0 rlehe      (501) staff       (20)       39 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic.egg-info/requires.txt
+-rw-r--r--   0 rlehe      (501) staff       (20)     3678 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic.egg-info/SOURCES.txt
+-rw-r--r--   0 rlehe      (501) staff       (20)        6 2018-10-05 16:29:58.000000 fbpic-0.9.5/fbpic.egg-info/top_level.txt
+-rw-r--r--   0 rlehe      (501) staff       (20)      113 2018-06-08 22:18:19.000000 fbpic-0.9.5/MANIFEST.in
+-rw-r--r--   0 rlehe      (501) staff       (20)     6953 2018-10-05 16:29:58.000000 fbpic-0.9.5/PKG-INFO
+-rw-r--r--   0 rlehe      (501) staff       (20)     5162 2018-10-05 16:17:32.000000 fbpic-0.9.5/README.md
+-rw-r--r--   0 rlehe      (501) staff       (20)       39 2018-08-03 18:07:20.000000 fbpic-0.9.5/requirements.txt
+-rw-r--r--   0 rlehe      (501) staff       (20)       38 2018-10-05 16:29:58.000000 fbpic-0.9.5/setup.cfg
+-rw-r--r--   0 rlehe      (501) staff       (20)     1877 2018-10-05 16:17:32.000000 fbpic-0.9.5/setup.py
```

### Comparing `fbpic-0.9.4/README.md` & `fbpic-0.9.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 cylindrical geometry** (Fourier-Bessel
 decomposition) for the fields. This combines the advantages of **spectral 3D** PIC codes (high accuracy and stability) and
 those of **finite-difference cylindrical** PIC codes
 (orders-of-magnitude speedup when compared to 3D simulations).  
 For more details on the algorithm, its advantages and limitations, see
 the [documentation](http://fbpic.github.io).
 
-### Language and harware
+### Language and hardware
 
 FBPIC is written entirely in Python, but uses
 [Numba](http://numba.pydata.org/) Just-In-Time compiler for high
 performance. In addition, the code can run on **CPU** (with multi-threading)
 and on **GPU**. For large simulations, running the
 code on GPU can be much faster than on CPU.
```

### Comparing `fbpic-0.9.4/setup.py` & `fbpic-0.9.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # License: 3-Clause-BSD-LBNL
 import sys
 from setuptools import setup, find_packages
 from setuptools.command.test import test as TestCommand
 import fbpic # In order to extract the version number
 
 # Obtain the long description from README.md
-long_description = open('./README.md').read()
+with open('./README.md') as f:
+    long_description = f.read()
 # Get the package requirements from the requirements.txt file
 with open('requirements.txt') as f:
     install_requires = [ line.strip('\n') for line in f.readlines() ]
 
 # Define a custom class to run the py.test with `python setup.py test`
 class PyTest(TestCommand):
 
@@ -21,15 +22,15 @@
         sys.exit(errcode)
 
 setup(
     name='fbpic',
     version=fbpic.__version__,
     description='Spectral, quasi-3D Particle-In-Cell for CPU and GPU',
     long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description_content_type='text/markdown',
     maintainer='Remi Lehe',
     maintainer_email='remi.lehe@normalesup.org',
     license='BSD-3-Clause-LBNL',
     packages=find_packages('.'),
     tests_require=['pytest', 'openpmd_viewer'],
     cmdclass={'test': PyTest},
     install_requires=install_requires,
```

### Comparing `fbpic-0.9.4/fbpic.egg-info/SOURCES.txt` & `fbpic-0.9.5/fbpic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic.egg-info/PKG-INFO` & `fbpic-0.9.5/fbpic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbpic
-Version: 0.9.4
+Version: 0.9.5
 Summary: Spectral, quasi-3D Particle-In-Cell for CPU and GPU
 Home-page: http://github.com/fbpic/fbpic
 Maintainer: Remi Lehe
 Maintainer-email: remi.lehe@normalesup.org
 License: BSD-3-Clause-LBNL
 Description: # Fourier-Bessel Particle-In-Cell code (FBPIC)
         
@@ -33,15 +33,15 @@
         cylindrical geometry** (Fourier-Bessel
         decomposition) for the fields. This combines the advantages of **spectral 3D** PIC codes (high accuracy and stability) and
         those of **finite-difference cylindrical** PIC codes
         (orders-of-magnitude speedup when compared to 3D simulations).  
         For more details on the algorithm, its advantages and limitations, see
         the [documentation](http://fbpic.github.io).
         
-        ### Language and harware
+        ### Language and hardware
         
         FBPIC is written entirely in Python, but uses
         [Numba](http://numba.pydata.org/) Just-In-Time compiler for high
         performance. In addition, the code can run on **CPU** (with multi-threading)
         and on **GPU**. For large simulations, running the
         code on GPU can be much faster than on CPU.
```

### Comparing `fbpic-0.9.4/fbpic/particles/elementary_process/compton/compton.py` & `fbpic-0.9.5/fbpic/particles/elementary_process/compton/compton.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/elementary_process/compton/numba_methods.py` & `fbpic-0.9.5/fbpic/particles/elementary_process/compton/numba_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/elementary_process/compton/inline_functions.py` & `fbpic-0.9.5/fbpic/particles/elementary_process/compton/inline_functions.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/elementary_process/compton/cuda_methods.py` & `fbpic-0.9.5/fbpic/particles/elementary_process/compton/cuda_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/elementary_process/cuda_numba_utils.py` & `fbpic-0.9.5/fbpic/particles/elementary_process/cuda_numba_utils.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/elementary_process/ionization/numba_methods.py` & `fbpic-0.9.5/fbpic/particles/elementary_process/ionization/numba_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/elementary_process/ionization/inline_functions.py` & `fbpic-0.9.5/fbpic/particles/elementary_process/ionization/inline_functions.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/elementary_process/ionization/atomic_data.txt` & `fbpic-0.9.5/fbpic/particles/elementary_process/ionization/atomic_data.txt`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/elementary_process/ionization/read_atomic_data.py` & `fbpic-0.9.5/fbpic/particles/elementary_process/ionization/read_atomic_data.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/elementary_process/ionization/ionizer.py` & `fbpic-0.9.5/fbpic/particles/elementary_process/ionization/ionizer.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/elementary_process/ionization/cuda_methods.py` & `fbpic-0.9.5/fbpic/particles/elementary_process/ionization/cuda_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/injection/continuous_injection.py` & `fbpic-0.9.5/fbpic/particles/injection/continuous_injection.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/injection/ballistic_before_plane.py` & `fbpic-0.9.5/fbpic/particles/injection/ballistic_before_plane.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/deposition/threading_methods.py` & `fbpic-0.9.5/fbpic/particles/deposition/threading_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
 
             # Positions of the particles, in the cell unit
             r_cell = invdr*(rj - rmin) - 0.5
             z_cell = invdz*(zj - zmin) - 0.5
             # Index of the lowest cell of `global_array` that gets modified
             # by this particle (note: `global_array` has 2 guard cells)
             # (`min` function avoids out-of-bounds access at high r)
-            ir_cell = min( int(math.floor(r_cell))+1, Nr+1 )
+            ir_cell = min( int(math.floor(r_cell))+1, Nr )
             iz_cell = int(math.floor( z_cell )) + 1
 
             # Add contribution of this particle to the global array
             for m in range(Nm):
                 rho_global[i_thread,m,iz_cell+0,ir_cell+0] += Sz_cubic(z_cell, 0)*Sr_cubic(r_cell, 0)*rho_scal[m]
                 rho_global[i_thread,m,iz_cell+0,ir_cell+1] += Sz_cubic(z_cell, 0)*Sr_cubic(r_cell, 1)*rho_scal[m]
                 rho_global[i_thread,m,iz_cell+0,ir_cell+2] += Sz_cubic(z_cell, 0)*Sr_cubic(r_cell, 2)*rho_scal[m]
@@ -560,15 +560,15 @@
 
             # Positions of the particles, in the cell unit
             r_cell = invdr*(rj - rmin) - 0.5
             z_cell = invdz*(zj - zmin) - 0.5
             # Index of the lowest cell of `global_array` that gets modified
             # by this particle (note: `global_array` has 2 guard cells)
             # (`min` function avoids out-of-bounds access at high r)
-            ir_cell = min( int(math.floor(r_cell))+1, Nr+1 )
+            ir_cell = min( int(math.floor(r_cell))+1, Nr )
             iz_cell = int(math.floor( z_cell )) + 1
 
             # Add contribution of this particle to the global array
             for m in range(Nm):
                 j_r_global[i_thread,m,iz_cell+0,ir_cell+0] += Sz_cubic(z_cell, 0)*Sr_cubic(r_cell, 0)*jr_scal[m]
                 j_r_global[i_thread,m,iz_cell+0,ir_cell+1] += Sz_cubic(z_cell, 0)*Sr_cubic(r_cell, 1)*jr_scal[m]
                 j_r_global[i_thread,m,iz_cell+0,ir_cell+2] += Sz_cubic(z_cell, 0)*Sr_cubic(r_cell, 2)*jr_scal[m]
```

### Comparing `fbpic-0.9.4/fbpic/particles/deposition/cuda_methods_one_mode.py` & `fbpic-0.9.5/fbpic/particles/deposition/cuda_methods_one_mode.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/deposition/numba_methods.py` & `fbpic-0.9.5/fbpic/particles/deposition/numba_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/deposition/cuda_methods.py` & `fbpic-0.9.5/fbpic/particles/deposition/cuda_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/particles.py` & `fbpic-0.9.5/fbpic/particles/particles.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,20 +432,17 @@
         ----------
         element: string
             The atomic symbol of the considered ionizable species
             (e.g. 'He', 'N' ;  do not use 'Helium' or 'Nitrogen')
 
         target_species: a `Particles` object, or a dictionary of `Particles`
             Stores the electron macroparticles that are created in
-            the ionization process.
-
-            - If a single `Particles` object is passed, than electrons from all
-            ionization levels are stored into this object.
-
-            - If a dictionary is passed, then its keys should be integers
+            the ionization process. If a single `Particles` object is passed, 
+            then electrons from all ionization levels are stored into this 
+            object. If a dictionary is passed, then its keys should be integers
             (corresponding to the ionizable levels of `element`, starting
             at `level_start`), and its values should be `Particles` objects.
             In this case, the electrons from each distinct ionizable level
             will be stored into these separate objects. Note that using
             separate objects will typically require longer computing time.
 
         level_start: int
```

### Comparing `fbpic-0.9.4/fbpic/particles/gathering/threading_methods_one_mode.py` & `fbpic-0.9.5/fbpic/particles/gathering/threading_methods_one_mode.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/gathering/threading_methods.py` & `fbpic-0.9.5/fbpic/particles/gathering/threading_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/gathering/cuda_methods_one_mode.py` & `fbpic-0.9.5/fbpic/particles/gathering/cuda_methods_one_mode.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/gathering/inline_functions.py` & `fbpic-0.9.5/fbpic/particles/gathering/inline_functions.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/gathering/cuda_methods.py` & `fbpic-0.9.5/fbpic/particles/gathering/cuda_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/push/numba_methods.py` & `fbpic-0.9.5/fbpic/particles/push/numba_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/push/inline_functions.py` & `fbpic-0.9.5/fbpic/particles/push/inline_functions.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/push/cuda_methods.py` & `fbpic-0.9.5/fbpic/particles/push/cuda_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/tracking/tracking.py` & `fbpic-0.9.5/fbpic/particles/tracking/tracking.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/utilities/cuda_sorting.py` & `fbpic-0.9.5/fbpic/particles/utilities/cuda_sorting.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/particles/utilities/utility_methods.py` & `fbpic-0.9.5/fbpic/particles/utilities/utility_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/boundaries/moving_window.py` & `fbpic-0.9.5/fbpic/boundaries/moving_window.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/boundaries/field_buffer_handling.py` & `fbpic-0.9.5/fbpic/boundaries/field_buffer_handling.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/boundaries/boundary_communicator.py` & `fbpic-0.9.5/fbpic/boundaries/boundary_communicator.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/boundaries/particle_buffer_handling.py` & `fbpic-0.9.5/fbpic/boundaries/particle_buffer_handling.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/boundaries/cuda_methods.py` & `fbpic-0.9.5/fbpic/boundaries/cuda_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/lpa_utils/boosted_frame.py` & `fbpic-0.9.5/fbpic/lpa_utils/boosted_frame.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/lpa_utils/laser/laser_profiles.py` & `fbpic-0.9.5/fbpic/lpa_utils/laser/laser_profiles.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/lpa_utils/laser/laser.py` & `fbpic-0.9.5/fbpic/lpa_utils/laser/laser.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/lpa_utils/laser/antenna_injection.py` & `fbpic-0.9.5/fbpic/lpa_utils/laser/antenna_injection.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/lpa_utils/laser/direct_injection.py` & `fbpic-0.9.5/fbpic/lpa_utils/laser/direct_injection.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/lpa_utils/external_fields.py` & `fbpic-0.9.5/fbpic/lpa_utils/external_fields.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/lpa_utils/bunch.py` & `fbpic-0.9.5/fbpic/lpa_utils/bunch.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,17 @@
     gamma0 : float
         The Lorentz factor of the electrons.
 
     sig_gamma : float
         The absolute energy spread of the bunch.
 
     Q : float (in Coulomb)
-        The total charge of the bunch (should be a positive number)
+        The total charge of the bunch (in absolute value)
+        (if a negative number is given, its absolute value will
+        automatically be taken)
 
     N : int
         The number of particles the bunch should consist of.
 
     zf: float (in meters), optional
         Position of the focus.
 
@@ -171,15 +173,15 @@
                   " sig_gamma will be set to zero. \n")
     # Finally we calculate the uz of each particle
     # from the gamma and the transverse momenta ux, uy
     uz = np.sqrt((gamma**2-1) - ux**2 - uy**2)
     # Get inverse gamma
     inv_gamma = 1./gamma
     # Get weight of each particle
-    w = Q / (N*e) * np.ones_like(x)
+    w = abs(Q) / (N*e) * np.ones_like(x)
 
     # Propagate distribution to an out-of-focus position tf.
     # (without taking space charge effects into account)
     if tf != 0.:
         x = x - ux*inv_gamma*c*tf
         y = y - uy*inv_gamma*c*tf
         z = z - uz*inv_gamma*c*tf
@@ -551,12 +553,12 @@
     spect.Ez[:,:] += -1.j*spect.kz * phi + 1.j*beta*c*spect.kz * Az
     if not neglect_transverse_currents:
         spect.Ep[:,:] += 1.j*beta*c*spect.kz * Ap
         spect.Em[:,:] += 1.j*beta*c*spect.kz * Am
 
     # Deduce the B field
     spect.Bp[:,:] += -0.5j*spect.kr * Az
-    spect.Bm[:,:] += -0.5j*spect.kr * Az    
+    spect.Bm[:,:] += -0.5j*spect.kr * Az
     if not neglect_transverse_currents:
         spect.Bp[:,:] += spect.kz * Ap
         spect.Bm[:,:] -= spect.kz * Am
         spect.Bz[:,:] += 1.j*spect.kr * Ap + 1.j*spect.kr * Am
```

### Comparing `fbpic-0.9.4/fbpic/openpmd_diag/checkpoint_restart.py` & `fbpic-0.9.5/fbpic/openpmd_diag/checkpoint_restart.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/openpmd_diag/generic_diag.py` & `fbpic-0.9.5/fbpic/openpmd_diag/generic_diag.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/openpmd_diag/particle_density_diag.py` & `fbpic-0.9.5/fbpic/openpmd_diag/particle_density_diag.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/openpmd_diag/field_diag.py` & `fbpic-0.9.5/fbpic/openpmd_diag/field_diag.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/openpmd_diag/__init__.py` & `fbpic-0.9.5/fbpic/openpmd_diag/__init__.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/openpmd_diag/boosted_particle_diag.py` & `fbpic-0.9.5/fbpic/openpmd_diag/boosted_particle_diag.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/openpmd_diag/particle_diag.py` & `fbpic-0.9.5/fbpic/openpmd_diag/particle_diag.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/openpmd_diag/data_dict.py` & `fbpic-0.9.5/fbpic/openpmd_diag/data_dict.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/openpmd_diag/boosted_field_diag.py` & `fbpic-0.9.5/fbpic/openpmd_diag/boosted_field_diag.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/openpmd_diag/cuda_methods.py` & `fbpic-0.9.5/fbpic/openpmd_diag/cuda_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/main.py` & `fbpic-0.9.5/fbpic/main.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/fields/spectral_grid.py` & `fbpic-0.9.5/fbpic/fields/spectral_grid.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/fields/interpolation_grid.py` & `fbpic-0.9.5/fbpic/fields/interpolation_grid.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/fields/psatd_coefs.py` & `fbpic-0.9.5/fbpic/fields/psatd_coefs.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/fields/numba_methods.py` & `fbpic-0.9.5/fbpic/fields/numba_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/fields/spectral_transform/fourier.py` & `fbpic-0.9.5/fbpic/fields/spectral_transform/fourier.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/fields/spectral_transform/hankel.py` & `fbpic-0.9.5/fbpic/fields/spectral_transform/hankel.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/fields/spectral_transform/spectral_transformer.py` & `fbpic-0.9.5/fbpic/fields/spectral_transform/spectral_transformer.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/fields/spectral_transform/numba_methods.py` & `fbpic-0.9.5/fbpic/fields/spectral_transform/numba_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/fields/spectral_transform/mkl_fft.py` & `fbpic-0.9.5/fbpic/fields/spectral_transform/mkl_fft.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/fields/spectral_transform/cuda_methods.py` & `fbpic-0.9.5/fbpic/fields/spectral_transform/cuda_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/fields/utility_methods.py` & `fbpic-0.9.5/fbpic/fields/utility_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,15 +138,19 @@
     Returns:
     -------
     Number of cells needed for the stencil to decrease to machine precision
     """
     k = np.sqrt(kz**2 + kperp**2)
     # Calculation of the Theta coefficient if the Galilean scheme is used
     if use_galilean is True:
-        theta = np.exp(1.j * v_comoving * kz * cdt / c / 2)
+        # When using the galilean scheme the stencil reach is always larger
+        # in the direction of v_comoving. Use abs(v_comoving) to have the
+        # maximum stencil extent
+        abs_v_comoving = np.abs(v_comoving)
+        theta = np.exp(1.j * abs_v_comoving * kz * cdt / c / 2)
     else:
         theta = np.ones_like(kz)
     # Calculation of the stencils for the three C/S coefficients
     # in the cylindrical PSATD equations
     cos_stencil = np.fft.ifft(
         theta ** 2 * np.cos( k * cdt) )
     sin_z_stencil = np.fft.ifft(
@@ -156,15 +160,16 @@
 
     # Combination of the stencil function of all three C/S coefficients
     alpha = np.sqrt(np.abs(cos_stencil)**2 +
                     np.abs(sin_z_stencil)**2 +
                     np.abs(sin_perp_stencil)**2)
     # Reach of the stencil defined at the position, when the signal
     # decreased to machine precision
-    stencil_reach = np.where(np.abs(alpha)[:int(alpha.shape[0]/2)] < 1.e-16)[0][0]
+    stencil_reach = np.where(np.abs(alpha)
+                             [:int(alpha.shape[0] / 2)] < 1.e-16)[0][0]
 
     return int(stencil_reach)
 
 
 def get_stencil_reach(Nz, dz, cdt, n_order, v_comoving, use_galilean):
     """
     Return the stencil reach (in spatial space) for a given finite order
@@ -209,8 +214,9 @@
     # Calculate the real kz for the given grid (Nz)
     real_kz = 2 * np.pi * np.fft.fftfreq(Nz, d=dz)
     # Get the modified, finite order kz
     kz = get_modified_k(real_kz, n_order, dz=dz)
 
     # Calculate the stencil reach at an arbitrary kperp = 0.5
     # (Note: The stencil reach depends only weakly on kperp)
+
     return stencil_reach(kz, 0.5, cdt, v_comoving, use_galilean)
```

### Comparing `fbpic-0.9.4/fbpic/fields/fields.py` & `fbpic-0.9.5/fbpic/fields/fields.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/fields/cuda_methods.py` & `fbpic-0.9.5/fbpic/fields/cuda_methods.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/utils/mpi.py` & `fbpic-0.9.5/fbpic/utils/mpi.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/utils/cuda.py` & `fbpic-0.9.5/fbpic/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/utils/threading.py` & `fbpic-0.9.5/fbpic/utils/threading.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/fbpic/utils/printing.py` & `fbpic-0.9.5/fbpic/utils/printing.py`

 * *Files identical despite different names*

### Comparing `fbpic-0.9.4/PKG-INFO` & `fbpic-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbpic
-Version: 0.9.4
+Version: 0.9.5
 Summary: Spectral, quasi-3D Particle-In-Cell for CPU and GPU
 Home-page: http://github.com/fbpic/fbpic
 Maintainer: Remi Lehe
 Maintainer-email: remi.lehe@normalesup.org
 License: BSD-3-Clause-LBNL
 Description: # Fourier-Bessel Particle-In-Cell code (FBPIC)
         
@@ -33,15 +33,15 @@
         cylindrical geometry** (Fourier-Bessel
         decomposition) for the fields. This combines the advantages of **spectral 3D** PIC codes (high accuracy and stability) and
         those of **finite-difference cylindrical** PIC codes
         (orders-of-magnitude speedup when compared to 3D simulations).  
         For more details on the algorithm, its advantages and limitations, see
         the [documentation](http://fbpic.github.io).
         
-        ### Language and harware
+        ### Language and hardware
         
         FBPIC is written entirely in Python, but uses
         [Numba](http://numba.pydata.org/) Just-In-Time compiler for high
         performance. In addition, the code can run on **CPU** (with multi-threading)
         and on **GPU**. For large simulations, running the
         code on GPU can be much faster than on CPU.
```

