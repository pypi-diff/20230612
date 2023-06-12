# Comparing `tmp/normflows-1.6.2.tar.gz` & `tmp/normflows-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/normflows-1.6.2.tar", last modified: Fri Apr 28 14:53:22 2023, max compression
+gzip compressed data, was "dist/normflows-1.7.0.tar", last modified: Mon Jun 12 11:55:44 2023, max compression
```

## Comparing `normflows-1.6.2.tar` & `normflows-1.7.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1072 2021-11-22 13:57:32.000000 normflows-1.6.2/LICENSE
--rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)       42 2021-11-22 13:57:32.000000 normflows-1.6.2/MANIFEST.in
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    14023 2023-04-28 14:53:22.000000 normflows-1.6.2/PKG-INFO
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    13434 2023-04-28 14:51:39.000000 normflows-1.6.2/README.md
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      253 2023-04-28 14:51:39.000000 normflows-1.6.2/normflows/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    15220 2023-04-28 14:51:17.000000 normflows-1.6.2/normflows/core.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     7502 2023-04-28 14:51:17.000000 normflows-1.6.2/normflows/core_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/distributions/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      659 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/distributions/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    21489 2023-02-25 15:05:55.000000 normflows-1.6.2/normflows/distributions/base.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4508 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/base_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2699 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/distributions/decoder.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1589 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/decoder_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1756 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/distribution_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5745 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/encoder.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     3493 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/encoder_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      663 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/distributions/linear_interpolation.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2176 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/distributions/mh_proposal.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9434 2023-01-23 18:21:11.000000 normflows-1.6.2/normflows/distributions/prior.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1651 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/prior_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4930 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/distributions/target.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      844 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/target_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/flows/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      913 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/flows/__init__.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/flows/affine/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      218 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/flows/affine/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4158 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/flows/affine/autoregressive.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      974 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/affine/autoregressive_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9923 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/flows/affine/coupling.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1662 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/flows/affine/coupling_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     3330 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/affine/glow.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1264 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/affine/glow_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1924 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/base.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1267 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/flows/base_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1325 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/flow_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    18397 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/mixing.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1360 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/mixing_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/flows/neural_spline/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      252 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/flows/neural_spline/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4849 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/neural_spline/autoregressive.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      778 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/neural_spline/autoregressive_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    13084 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/neural_spline/coupling.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1961 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/neural_spline/coupling_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    10166 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/neural_spline/wrapper.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1861 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/neural_spline/wrapper_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2303 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/flows/normalization.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2047 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/flows/periodic.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1332 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/periodic_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2878 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/planar.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      722 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/planar_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1491 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/radial.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      506 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/radial_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4047 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/flows/reshape.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    14772 2023-01-20 17:37:19.000000 normflows-1.6.2/normflows/flows/residual.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2739 2023-01-23 14:38:51.000000 normflows-1.6.2/normflows/flows/residual_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4278 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/stochastic.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1321 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/stochastic_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/nets/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      212 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/nets/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2028 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/nets/cnn.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    25793 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/nets/lipschitz.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9712 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/nets/made.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4741 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/nets/made_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2284 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/nets/mlp.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     6999 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/nets/resnet.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/sampling/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       23 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/sampling/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1999 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/sampling/hais.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1982 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/transforms.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      656 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/transforms_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/utils/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      262 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/utils/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2046 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/utils/eval.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1660 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/utils/masks.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5660 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/utils/nn.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      852 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/utils/optim.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1168 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/utils/preprocessing.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     7744 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/utils/splines.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2318 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/utils/splines_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows.egg-info/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    14023 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows.egg-info/PKG-INFO
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2436 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows.egg-info/SOURCES.txt
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)        1 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows.egg-info/dependency_links.txt
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       63 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows.egg-info/requires.txt
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       10 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows.egg-info/top_level.txt
--rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)       11 2022-07-26 12:32:34.000000 normflows-1.6.2/requirements.txt
--rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)      108 2023-04-28 14:53:22.000000 normflows-1.6.2/setup.cfg
--rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)     1368 2023-04-28 14:51:39.000000 normflows-1.6.2/setup.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1072 2021-11-22 13:57:32.000000 normflows-1.7.0/LICENSE
+-rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)       42 2021-11-22 13:57:32.000000 normflows-1.7.0/MANIFEST.in
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    15779 2023-06-12 11:55:44.000000 normflows-1.7.0/PKG-INFO
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    15190 2023-06-12 11:53:08.000000 normflows-1.7.0/README.md
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      253 2023-06-12 11:52:41.000000 normflows-1.7.0/normflows/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    16860 2023-06-06 13:57:44.000000 normflows-1.7.0/normflows/core.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     7805 2023-06-06 13:57:44.000000 normflows-1.7.0/normflows/core_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/distributions/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      699 2023-05-31 15:25:11.000000 normflows-1.7.0/normflows/distributions/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    22844 2023-05-30 15:55:17.000000 normflows-1.7.0/normflows/distributions/base.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4884 2023-05-30 15:55:17.000000 normflows-1.7.0/normflows/distributions/base_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2699 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/distributions/decoder.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1589 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/distributions/decoder_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1756 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/distributions/distribution_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5745 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/distributions/encoder.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     3493 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/distributions/encoder_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      663 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/distributions/linear_interpolation.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2176 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/distributions/mh_proposal.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9434 2023-01-23 18:21:11.000000 normflows-1.7.0/normflows/distributions/prior.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1651 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/distributions/prior_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5694 2023-05-31 15:25:11.000000 normflows-1.7.0/normflows/distributions/target.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1334 2023-05-31 15:25:11.000000 normflows-1.7.0/normflows/distributions/target_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/flows/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      913 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/flows/__init__.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/flows/affine/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      218 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/flows/affine/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4158 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/flows/affine/autoregressive.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      974 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/affine/autoregressive_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9923 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/flows/affine/coupling.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1662 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/flows/affine/coupling_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     3330 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/affine/glow.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1264 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/affine/glow_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1924 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/base.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1267 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/flows/base_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1325 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/flow_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    18397 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/mixing.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1360 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/mixing_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/flows/neural_spline/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      252 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/flows/neural_spline/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4849 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/neural_spline/autoregressive.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      778 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/neural_spline/autoregressive_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    13084 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/neural_spline/coupling.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1961 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/neural_spline/coupling_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    10166 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/neural_spline/wrapper.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1861 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/neural_spline/wrapper_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2303 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/flows/normalization.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2047 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/flows/periodic.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1332 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/periodic_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2878 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/planar.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      722 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/planar_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1491 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/radial.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      506 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/radial_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4047 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/flows/reshape.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    14772 2023-01-20 17:37:19.000000 normflows-1.7.0/normflows/flows/residual.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2739 2023-01-23 14:38:51.000000 normflows-1.7.0/normflows/flows/residual_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4278 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/stochastic.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1321 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/stochastic_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/nets/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      212 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/nets/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2028 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/nets/cnn.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    25793 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/nets/lipschitz.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9712 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/nets/made.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4741 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/nets/made_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2284 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/nets/mlp.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     6999 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/nets/resnet.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/sampling/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       23 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/sampling/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1999 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/sampling/hais.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1982 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/transforms.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      656 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/transforms_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/utils/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      262 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/utils/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2046 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/utils/eval.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1660 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/utils/masks.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5660 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/utils/nn.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      852 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/utils/optim.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1168 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/utils/preprocessing.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     7744 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/utils/splines.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2318 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/utils/splines_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows.egg-info/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    15779 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows.egg-info/PKG-INFO
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2436 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows.egg-info/SOURCES.txt
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)        1 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows.egg-info/dependency_links.txt
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       63 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows.egg-info/requires.txt
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       10 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows.egg-info/top_level.txt
+-rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)       11 2022-07-26 12:32:34.000000 normflows-1.7.0/requirements.txt
+-rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)      108 2023-06-12 11:55:44.000000 normflows-1.7.0/setup.cfg
+-rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)     1368 2023-06-12 11:52:17.000000 normflows-1.7.0/setup.py
```

### Comparing `normflows-1.6.2/LICENSE` & `normflows-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/PKG-INFO` & `normflows-1.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: normflows
-Version: 1.6.2
+Version: 1.7.0
 Summary: Pytorch implementation of normalizing flows
 Home-page: https://github.com/VincentStimper/normalizing-flows
 Author: Vincent Stimper
 Author-email: vincent.stimper@tuebingen.mpg.de
 License: MIT
 Download-URL: https://github.com/VincentStimper/normalizing-flows/archive/refs/heads/master.zip
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 # `normflows`: A PyTorch Package for Normalizing Flows
 
 [![documentation](https://github.com/VincentStimper/normalizing-flows/actions/workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-flows/)
 ![unit-tests](https://github.com/VincentStimper/normalizing-flows/actions/workflows/pytest.yaml/badge.svg)
 ![code coverage](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true)
 [![License: MIT](https://img.shields.io/badge/Licence-MIT-lightgrey)](https://opensource.org/licenses/MIT)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/2302.12014) 
-[![PyPI](https://img.shields.io/badge/PyPI-1.6.2-blue.svg)](https://pypi.org/project/normflows/)
+[![PyPI](https://img.shields.io/badge/PyPI-1.7.0-blue.svg)](https://pypi.org/project/normflows/)
 [![Downloads](https://static.pepy.tech/personalized-badge/normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/normflows)
 
 
 `normflows` is a PyTorch implementation of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed via pip](#installation).
 The basic usage is described [here](#usage), and a [full documentation](https://vincentstimper.github.io/normalizing-flows/) 
 is available as well. A more detailed description of this package is given in out accompanying 
@@ -36,18 +36,19 @@
 [`examples` folder](https://github.com/VincentStimper/normalizing-flows/blob/master/examples), 
 including [Glow](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/glow.ipynb),
 a [VAE](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/vae.py), and
 a [Residual Flow](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/residual.ipynb).
 Moreover, two simple applications are highlighed in the [examples section](#examples). You can run them 
 yourself in Google Colab using the links below to get a feeling for `normflows`.
 
-| Link                                                                                                                                                                                                                                         | Description                                                                   |
-|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------|
-| <a href="https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/real_nvp_colab.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> | Real NVP applied to a 2D bimodal target distribution                          |
+| Link                                                                                                                                                                                                                                                  | Description                                                             |
+|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------|
+| <a href="https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/real_nvp_colab.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>          | Real NVP applied to a 2D bimodal target distribution                    |
 | <a href="https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/paper_example_nsf_colab.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> | Modeling a distribution on a cylinder surface with a neural spline flow |
+| <a href="https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/glow_colab.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>              | Modeling and generating CIFAR-10 images with Glow                       |
 
 
 ## Implemented Flows
 
 | Architecture | Reference                                                                                                                 |
 |--------------|---------------------------------------------------------------------------------------------------------------------------|
 | Planar Flow  | [Rezende & Mohamed, 2015](http://proceedings.mlr.press/v37/rezende15.html)                                                |
@@ -189,14 +190,38 @@
 which is available in [Colab](https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/paper_example_nsf_colab.ipynb)
 as well, we apply a Neural Spline Flow model to a distribution defined on a cylinder. The resulting density is visualized below.
 
 ![Neural Spline Flow applied to target distribution on a cylinder](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/master/figures/nsf_cylinder_3d.png)
 
 This example is considered in the [paper](https://arxiv.org/abs/2302.12014) accompanying this repository.
 
+## Support
+
+If you have problems, please read the [package documentation](https://vincentstimper.github.io/normalizing-flows/)
+and check out the [examples section](#examples) above. You are also welcome to 
+[create issues on GitHub](https://github.com/VincentStimper/normalizing-flows/issues) to get help. Note that it is
+worthwhile browsing the existing [open](https://github.com/VincentStimper/normalizing-flows/issues?q=is%3Aopen+is%3Aissue) 
+and [closed](https://github.com/VincentStimper/normalizing-flows/issues?q=is%3Aissue+is%3Aclosed) issues, which might
+address the problem you are facing.
+
+## Contributing
+
+If you find a bug or have a feature request, please 
+[file an issue on GitHub](https://github.com/VincentStimper/normalizing-flows/issues).
+
+You are welcome to contribute to the package by fixing the bug or adding the feature yourself. If you want to 
+contribute, please add tests for the code you added or modified and ensure it passes successfully by running `pytest`.
+This can be done by simply executing
+```
+pytest
+```
+within your local version of the repository. Make sure you code is well documented, and we also encourage contributions
+to the existing documentation. Once you finished coding and testing, please 
+[create a pull request on GitHub](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).
+
 ## Used by
 
 The package has been used in several research papers, which are listed below.
 
 > Andrew Campbell, Wenlong Chen, Vincent Stimper, José Miguel Hernández-Lobato, and Yichuan Zhang. 
 > [A gradient based strategy for Hamiltonian Monte Carlo hyperparameter optimization](https://proceedings.mlr.press/v139/campbell21a.html). 
 > In Proceedings of the 38th International Conference on Machine Learning, pp. 1238–1248. PMLR, 2021.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: normflows Version: 1.6.2 Summary: Pytorch
+Metadata-Version: 2.1 Name: normflows Version: 1.7.0 Summary: Pytorch
 implementation of normalizing flows Home-page: https://github.com/
 VincentStimper/normalizing-flows Author: Vincent Stimper Author-email:
 vincent.stimper@tuebingen.mpg.de License: MIT Download-URL: https://github.com/
 VincentStimper/normalizing-flows/archive/refs/heads/master.zip Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown Provides-Extra: docs License-File:
@@ -11,15 +11,15 @@
 workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-
 flows/) ![unit-tests](https://github.com/VincentStimper/normalizing-flows/
 actions/workflows/pytest.yaml/badge.svg) ![code coverage](https://
 raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/
 coverage.svg?raw=true) [![License: MIT](https://img.shields.io/badge/Licence-
 MIT-lightgrey)](https://opensource.org/licenses/MIT) [![arXiv](https://
 img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/
-2302.12014) [![PyPI](https://img.shields.io/badge/PyPI-1.6.2-blue.svg)](https:/
+2302.12014) [![PyPI](https://img.shields.io/badge/PyPI-1.7.0-blue.svg)](https:/
 /pypi.org/project/normflows/) [![Downloads](https://static.pepy.tech/
 personalized-badge/
 normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)]
 (https://pepy.tech/project/normflows) `normflows` is a PyTorch implementation
 of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed
 via pip](#installation). The basic usage is described [here](#usage), and a
@@ -33,18 +33,19 @@
 examples/vae.py), and a [Residual Flow](https://github.com/VincentStimper/
 normalizing-flows/blob/master/examples/residual.ipynb). Moreover, two simple
 applications are highlighed in the [examples section](#examples). You can run
 them yourself in Google Colab using the links below to get a feeling for
 `normflows`. | Link | Description | |------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
---------------------------------------|----------------------------------------
----------------------------------------| | [Open_In_Colab] | Real NVP applied
-to a 2D bimodal target distribution | | [Open_In_Colab] | Modeling a
-distribution on a cylinder surface with a neural spline flow | ## Implemented
+-----------------------------------------------|-------------------------------
+------------------------------------------| | [Open_In_Colab] | Real NVP
+applied to a 2D bimodal target distribution | | [Open_In_Colab] | Modeling a
+distribution on a cylinder surface with a neural spline flow | | [Open_In
+Colab] | Modeling and generating CIFAR-10 images with Glow | ## Implemented
 Flows | Architecture | Reference | |--------------|----------------------------
 -------------------------------------------------------------------------------
 ----------------| | Planar Flow | [Rezende & Mohamed, 2015](http://
 proceedings.mlr.press/v37/rezende15.html) | | Radial Flow | [Rezende & Mohamed,
 2015](http://proceedings.mlr.press/v37/rezende15.html) | | NICE | [Dinh et al.,
 2014](https://arxiv.org/abs/1410.8516) | | Real NVP | [Dinh et al., 2017]
 (https://openreview.net/forum?id=HkpbnH9lx) | | Glow | [Kingma et al., 2018]
@@ -127,34 +128,53 @@
 (https://colab.research.google.com/github/VincentStimper/normalizing-flows/
 blob/master/examples/paper_example_nsf_colab.ipynb) as well, we apply a Neural
 Spline Flow model to a distribution defined on a cylinder. The resulting
 density is visualized below. ![Neural Spline Flow applied to target
 distribution on a cylinder](https://raw.githubusercontent.com/VincentStimper/
 normalizing-flows/master/figures/nsf_cylinder_3d.png) This example is
 considered in the [paper](https://arxiv.org/abs/2302.12014) accompanying this
-repository. ## Used by The package has been used in several research papers,
-which are listed below. > Andrew Campbell, Wenlong Chen, Vincent Stimper, JosÃ©
-Miguel HernÃ¡ndez-Lobato, and Yichuan Zhang. > [A gradient based strategy for
-Hamiltonian Monte Carlo hyperparameter optimization](https://
-proceedings.mlr.press/v139/campbell21a.html). > In Proceedings of the 38th
-International Conference on Machine Learning, pp. 1238â1248. PMLR, 2021. > >
-[Code available on GitHub.](https://github.com/VincentStimper/hmc-
-hyperparameter-tuning) > Vincent Stimper, Bernhard SchÃ¶lkopf, JosÃ© Miguel
-HernÃ¡ndez-Lobato. > [Resampling Base Distributions of Normalizing Flows]
-(https://proceedings.mlr.press/v151/stimper22a). > In Proceedings of The 25th
-International Conference on Artificial Intelligence and Statistics, volume 151,
-pp. 4915â4936, 2022. > > [Code available on GitHub.](https://github.com/
-VincentStimper/resampled-base-flows) > Laurence I. Midgley, Vincent Stimper,
-Gregor N. C. Simm, Bernhard SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Flow
-Annealed Importance Sampling Bootstrap](https://arxiv.org/abs/2208.01893). >
-arXiv preprint arXiv:2208.01893, 2022. > > [Code available on GitHub.](https://
-github.com/lollcat/fab-torch) Moreover, the [`boltzgen`](https://github.com/
-VincentStimper/boltzmann-generators) package has been build upon `normflows`.
-## Citation If you use `normflows`, please consider citing the [corresponding
-paper](https://arxiv.org/abs/2302.12014) as follows. > Vincent Stimper, David
-Liu, Andrew Campbell, Vincent Berenz, Lukas Ryll, Bernhard SchÃ¶lkopf, JosÃ©
-Miguel HernÃ¡ndez-Lobato. > normflows: A PyTorch Package for Normalizing Flows,
-arXiv preprint arXiv:2302.12014, 2023. **Bibtex** ``` @article{normflows,
-author = {Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz
-and Lukas Ryll and Bernhard Sch{\"o}lkopf and Jos{\'e} Miguel Hern{\'a}ndez-
-Lobato}, title = {normflows: {A} {P}y{T}orch {P}ackage for {N}ormalizing
-{F}lows}, journal = {arXiv preprint arXiv:2302.12014}, year = {2023} } ```
+repository. ## Support If you have problems, please read the [package
+documentation](https://vincentstimper.github.io/normalizing-flows/) and check
+out the [examples section](#examples) above. You are also welcome to [create
+issues on GitHub](https://github.com/VincentStimper/normalizing-flows/issues)
+to get help. Note that it is worthwhile browsing the existing [open](https://
+github.com/VincentStimper/normalizing-flows/issues?q=is%3Aopen+is%3Aissue) and
+[closed](https://github.com/VincentStimper/normalizing-flows/
+issues?q=is%3Aissue+is%3Aclosed) issues, which might address the problem you
+are facing. ## Contributing If you find a bug or have a feature request, please
+[file an issue on GitHub](https://github.com/VincentStimper/normalizing-flows/
+issues). You are welcome to contribute to the package by fixing the bug or
+adding the feature yourself. If you want to contribute, please add tests for
+the code you added or modified and ensure it passes successfully by running
+`pytest`. This can be done by simply executing ``` pytest ``` within your local
+version of the repository. Make sure you code is well documented, and we also
+encourage contributions to the existing documentation. Once you finished coding
+and testing, please [create a pull request on GitHub](https://docs.github.com/
+en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-
+work-with-pull-requests/creating-a-pull-request). ## Used by The package has
+been used in several research papers, which are listed below. > Andrew
+Campbell, Wenlong Chen, Vincent Stimper, JosÃ© Miguel HernÃ¡ndez-Lobato, and
+Yichuan Zhang. > [A gradient based strategy for Hamiltonian Monte Carlo
+hyperparameter optimization](https://proceedings.mlr.press/v139/
+campbell21a.html). > In Proceedings of the 38th International Conference on
+Machine Learning, pp. 1238â1248. PMLR, 2021. > > [Code available on GitHub.]
+(https://github.com/VincentStimper/hmc-hyperparameter-tuning) > Vincent
+Stimper, Bernhard SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Resampling
+Base Distributions of Normalizing Flows](https://proceedings.mlr.press/v151/
+stimper22a). > In Proceedings of The 25th International Conference on
+Artificial Intelligence and Statistics, volume 151, pp. 4915â4936, 2022. > >
+[Code available on GitHub.](https://github.com/VincentStimper/resampled-base-
+flows) > Laurence I. Midgley, Vincent Stimper, Gregor N. C. Simm, Bernhard
+SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Flow Annealed Importance
+Sampling Bootstrap](https://arxiv.org/abs/2208.01893). > arXiv preprint arXiv:
+2208.01893, 2022. > > [Code available on GitHub.](https://github.com/lollcat/
+fab-torch) Moreover, the [`boltzgen`](https://github.com/VincentStimper/
+boltzmann-generators) package has been build upon `normflows`. ## Citation If
+you use `normflows`, please consider citing the [corresponding paper](https://
+arxiv.org/abs/2302.12014) as follows. > Vincent Stimper, David Liu, Andrew
+Campbell, Vincent Berenz, Lukas Ryll, Bernhard SchÃ¶lkopf, JosÃ© Miguel
+HernÃ¡ndez-Lobato. > normflows: A PyTorch Package for Normalizing Flows, arXiv
+preprint arXiv:2302.12014, 2023. **Bibtex** ``` @article{normflows, author =
+{Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz and Lukas
+Ryll and Bernhard Sch{\"o}lkopf and Jos{\'e} Miguel Hern{\'a}ndez-Lobato},
+title = {normflows: {A} {P}y{T}orch {P}ackage for {N}ormalizing {F}lows},
+journal = {arXiv preprint arXiv:2302.12014}, year = {2023} } ```
```

### Comparing `normflows-1.6.2/README.md` & `normflows-1.7.0/normflows.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,32 @@
+Metadata-Version: 2.1
+Name: normflows
+Version: 1.7.0
+Summary: Pytorch implementation of normalizing flows
+Home-page: https://github.com/VincentStimper/normalizing-flows
+Author: Vincent Stimper
+Author-email: vincent.stimper@tuebingen.mpg.de
+License: MIT
+Download-URL: https://github.com/VincentStimper/normalizing-flows/archive/refs/heads/master.zip
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+License-File: LICENSE
+
 # `normflows`: A PyTorch Package for Normalizing Flows
 
 [![documentation](https://github.com/VincentStimper/normalizing-flows/actions/workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-flows/)
 ![unit-tests](https://github.com/VincentStimper/normalizing-flows/actions/workflows/pytest.yaml/badge.svg)
 ![code coverage](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true)
 [![License: MIT](https://img.shields.io/badge/Licence-MIT-lightgrey)](https://opensource.org/licenses/MIT)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/2302.12014) 
-[![PyPI](https://img.shields.io/badge/PyPI-1.6.2-blue.svg)](https://pypi.org/project/normflows/)
+[![PyPI](https://img.shields.io/badge/PyPI-1.7.0-blue.svg)](https://pypi.org/project/normflows/)
 [![Downloads](https://static.pepy.tech/personalized-badge/normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/normflows)
 
 
 `normflows` is a PyTorch implementation of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed via pip](#installation).
 The basic usage is described [here](#usage), and a [full documentation](https://vincentstimper.github.io/normalizing-flows/) 
 is available as well. A more detailed description of this package is given in out accompanying 
@@ -19,18 +36,19 @@
 [`examples` folder](https://github.com/VincentStimper/normalizing-flows/blob/master/examples), 
 including [Glow](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/glow.ipynb),
 a [VAE](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/vae.py), and
 a [Residual Flow](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/residual.ipynb).
 Moreover, two simple applications are highlighed in the [examples section](#examples). You can run them 
 yourself in Google Colab using the links below to get a feeling for `normflows`.
 
-| Link                                                                                                                                                                                                                                         | Description                                                                   |
-|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------|
-| <a href="https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/real_nvp_colab.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> | Real NVP applied to a 2D bimodal target distribution                          |
+| Link                                                                                                                                                                                                                                                  | Description                                                             |
+|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------|
+| <a href="https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/real_nvp_colab.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>          | Real NVP applied to a 2D bimodal target distribution                    |
 | <a href="https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/paper_example_nsf_colab.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> | Modeling a distribution on a cylinder surface with a neural spline flow |
+| <a href="https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/glow_colab.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>              | Modeling and generating CIFAR-10 images with Glow                       |
 
 
 ## Implemented Flows
 
 | Architecture | Reference                                                                                                                 |
 |--------------|---------------------------------------------------------------------------------------------------------------------------|
 | Planar Flow  | [Rezende & Mohamed, 2015](http://proceedings.mlr.press/v37/rezende15.html)                                                |
@@ -172,14 +190,38 @@
 which is available in [Colab](https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/paper_example_nsf_colab.ipynb)
 as well, we apply a Neural Spline Flow model to a distribution defined on a cylinder. The resulting density is visualized below.
 
 ![Neural Spline Flow applied to target distribution on a cylinder](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/master/figures/nsf_cylinder_3d.png)
 
 This example is considered in the [paper](https://arxiv.org/abs/2302.12014) accompanying this repository.
 
+## Support
+
+If you have problems, please read the [package documentation](https://vincentstimper.github.io/normalizing-flows/)
+and check out the [examples section](#examples) above. You are also welcome to 
+[create issues on GitHub](https://github.com/VincentStimper/normalizing-flows/issues) to get help. Note that it is
+worthwhile browsing the existing [open](https://github.com/VincentStimper/normalizing-flows/issues?q=is%3Aopen+is%3Aissue) 
+and [closed](https://github.com/VincentStimper/normalizing-flows/issues?q=is%3Aissue+is%3Aclosed) issues, which might
+address the problem you are facing.
+
+## Contributing
+
+If you find a bug or have a feature request, please 
+[file an issue on GitHub](https://github.com/VincentStimper/normalizing-flows/issues).
+
+You are welcome to contribute to the package by fixing the bug or adding the feature yourself. If you want to 
+contribute, please add tests for the code you added or modified and ensure it passes successfully by running `pytest`.
+This can be done by simply executing
+```
+pytest
+```
+within your local version of the repository. Make sure you code is well documented, and we also encourage contributions
+to the existing documentation. Once you finished coding and testing, please 
+[create a pull request on GitHub](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).
+
 ## Used by
 
 The package has been used in several research papers, which are listed below.
 
 > Andrew Campbell, Wenlong Chen, Vincent Stimper, José Miguel Hernández-Lobato, and Yichuan Zhang. 
 > [A gradient based strategy for Hamiltonian Monte Carlo hyperparameter optimization](https://proceedings.mlr.press/v139/campbell21a.html). 
 > In Proceedings of the 38th International Conference on Machine Learning, pp. 1238–1248. PMLR, 2021.
@@ -219,7 +261,9 @@
 }
 ```
 
 
 
 
 
+
+
```

#### html2text {}

```diff
@@ -1,18 +1,27 @@
-# `normflows`: A PyTorch Package for Normalizing Flows [![documentation](https:
-//github.com/VincentStimper/normalizing-flows/actions/workflows/mkdocs.yaml/
-badge.svg)](https://vincentstimper.github.io/normalizing-flows/) ![unit-tests]
-(https://github.com/VincentStimper/normalizing-flows/actions/workflows/
-pytest.yaml/badge.svg) ![code coverage](https://raw.githubusercontent.com/
-VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true) [!
-[License: MIT](https://img.shields.io/badge/Licence-MIT-lightgrey)](https://
-opensource.org/licenses/MIT) [![arXiv](https://img.shields.io/badge/arXiv-
-2302.12014-b31b1b.svg)](https://arxiv.org/abs/2302.12014) [![PyPI](https://
-img.shields.io/badge/PyPI-1.6.2-blue.svg)](https://pypi.org/project/normflows/
-) [![Downloads](https://static.pepy.tech/personalized-badge/
+Metadata-Version: 2.1 Name: normflows Version: 1.7.0 Summary: Pytorch
+implementation of normalizing flows Home-page: https://github.com/
+VincentStimper/normalizing-flows Author: Vincent Stimper Author-email:
+vincent.stimper@tuebingen.mpg.de License: MIT Download-URL: https://github.com/
+VincentStimper/normalizing-flows/archive/refs/heads/master.zip Platform:
+UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
+Audience :: Developers Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown Provides-Extra: docs License-File:
+LICENSE # `normflows`: A PyTorch Package for Normalizing Flows [!
+[documentation](https://github.com/VincentStimper/normalizing-flows/actions/
+workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-
+flows/) ![unit-tests](https://github.com/VincentStimper/normalizing-flows/
+actions/workflows/pytest.yaml/badge.svg) ![code coverage](https://
+raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/
+coverage.svg?raw=true) [![License: MIT](https://img.shields.io/badge/Licence-
+MIT-lightgrey)](https://opensource.org/licenses/MIT) [![arXiv](https://
+img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/
+2302.12014) [![PyPI](https://img.shields.io/badge/PyPI-1.7.0-blue.svg)](https:/
+/pypi.org/project/normflows/) [![Downloads](https://static.pepy.tech/
+personalized-badge/
 normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)]
 (https://pepy.tech/project/normflows) `normflows` is a PyTorch implementation
 of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed
 via pip](#installation). The basic usage is described [here](#usage), and a
 [full documentation](https://vincentstimper.github.io/normalizing-flows/) is
 available as well. A more detailed description of this package is given in out
@@ -24,18 +33,19 @@
 examples/vae.py), and a [Residual Flow](https://github.com/VincentStimper/
 normalizing-flows/blob/master/examples/residual.ipynb). Moreover, two simple
 applications are highlighed in the [examples section](#examples). You can run
 them yourself in Google Colab using the links below to get a feeling for
 `normflows`. | Link | Description | |------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
---------------------------------------|----------------------------------------
----------------------------------------| | [Open_In_Colab] | Real NVP applied
-to a 2D bimodal target distribution | | [Open_In_Colab] | Modeling a
-distribution on a cylinder surface with a neural spline flow | ## Implemented
+-----------------------------------------------|-------------------------------
+------------------------------------------| | [Open_In_Colab] | Real NVP
+applied to a 2D bimodal target distribution | | [Open_In_Colab] | Modeling a
+distribution on a cylinder surface with a neural spline flow | | [Open_In
+Colab] | Modeling and generating CIFAR-10 images with Glow | ## Implemented
 Flows | Architecture | Reference | |--------------|----------------------------
 -------------------------------------------------------------------------------
 ----------------| | Planar Flow | [Rezende & Mohamed, 2015](http://
 proceedings.mlr.press/v37/rezende15.html) | | Radial Flow | [Rezende & Mohamed,
 2015](http://proceedings.mlr.press/v37/rezende15.html) | | NICE | [Dinh et al.,
 2014](https://arxiv.org/abs/1410.8516) | | Real NVP | [Dinh et al., 2017]
 (https://openreview.net/forum?id=HkpbnH9lx) | | Glow | [Kingma et al., 2018]
@@ -118,34 +128,53 @@
 (https://colab.research.google.com/github/VincentStimper/normalizing-flows/
 blob/master/examples/paper_example_nsf_colab.ipynb) as well, we apply a Neural
 Spline Flow model to a distribution defined on a cylinder. The resulting
 density is visualized below. ![Neural Spline Flow applied to target
 distribution on a cylinder](https://raw.githubusercontent.com/VincentStimper/
 normalizing-flows/master/figures/nsf_cylinder_3d.png) This example is
 considered in the [paper](https://arxiv.org/abs/2302.12014) accompanying this
-repository. ## Used by The package has been used in several research papers,
-which are listed below. > Andrew Campbell, Wenlong Chen, Vincent Stimper, JosÃ©
-Miguel HernÃ¡ndez-Lobato, and Yichuan Zhang. > [A gradient based strategy for
-Hamiltonian Monte Carlo hyperparameter optimization](https://
-proceedings.mlr.press/v139/campbell21a.html). > In Proceedings of the 38th
-International Conference on Machine Learning, pp. 1238â1248. PMLR, 2021. > >
-[Code available on GitHub.](https://github.com/VincentStimper/hmc-
-hyperparameter-tuning) > Vincent Stimper, Bernhard SchÃ¶lkopf, JosÃ© Miguel
-HernÃ¡ndez-Lobato. > [Resampling Base Distributions of Normalizing Flows]
-(https://proceedings.mlr.press/v151/stimper22a). > In Proceedings of The 25th
-International Conference on Artificial Intelligence and Statistics, volume 151,
-pp. 4915â4936, 2022. > > [Code available on GitHub.](https://github.com/
-VincentStimper/resampled-base-flows) > Laurence I. Midgley, Vincent Stimper,
-Gregor N. C. Simm, Bernhard SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Flow
-Annealed Importance Sampling Bootstrap](https://arxiv.org/abs/2208.01893). >
-arXiv preprint arXiv:2208.01893, 2022. > > [Code available on GitHub.](https://
-github.com/lollcat/fab-torch) Moreover, the [`boltzgen`](https://github.com/
-VincentStimper/boltzmann-generators) package has been build upon `normflows`.
-## Citation If you use `normflows`, please consider citing the [corresponding
-paper](https://arxiv.org/abs/2302.12014) as follows. > Vincent Stimper, David
-Liu, Andrew Campbell, Vincent Berenz, Lukas Ryll, Bernhard SchÃ¶lkopf, JosÃ©
-Miguel HernÃ¡ndez-Lobato. > normflows: A PyTorch Package for Normalizing Flows,
-arXiv preprint arXiv:2302.12014, 2023. **Bibtex** ``` @article{normflows,
-author = {Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz
-and Lukas Ryll and Bernhard Sch{\"o}lkopf and Jos{\'e} Miguel Hern{\'a}ndez-
-Lobato}, title = {normflows: {A} {P}y{T}orch {P}ackage for {N}ormalizing
-{F}lows}, journal = {arXiv preprint arXiv:2302.12014}, year = {2023} } ```
+repository. ## Support If you have problems, please read the [package
+documentation](https://vincentstimper.github.io/normalizing-flows/) and check
+out the [examples section](#examples) above. You are also welcome to [create
+issues on GitHub](https://github.com/VincentStimper/normalizing-flows/issues)
+to get help. Note that it is worthwhile browsing the existing [open](https://
+github.com/VincentStimper/normalizing-flows/issues?q=is%3Aopen+is%3Aissue) and
+[closed](https://github.com/VincentStimper/normalizing-flows/
+issues?q=is%3Aissue+is%3Aclosed) issues, which might address the problem you
+are facing. ## Contributing If you find a bug or have a feature request, please
+[file an issue on GitHub](https://github.com/VincentStimper/normalizing-flows/
+issues). You are welcome to contribute to the package by fixing the bug or
+adding the feature yourself. If you want to contribute, please add tests for
+the code you added or modified and ensure it passes successfully by running
+`pytest`. This can be done by simply executing ``` pytest ``` within your local
+version of the repository. Make sure you code is well documented, and we also
+encourage contributions to the existing documentation. Once you finished coding
+and testing, please [create a pull request on GitHub](https://docs.github.com/
+en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-
+work-with-pull-requests/creating-a-pull-request). ## Used by The package has
+been used in several research papers, which are listed below. > Andrew
+Campbell, Wenlong Chen, Vincent Stimper, JosÃ© Miguel HernÃ¡ndez-Lobato, and
+Yichuan Zhang. > [A gradient based strategy for Hamiltonian Monte Carlo
+hyperparameter optimization](https://proceedings.mlr.press/v139/
+campbell21a.html). > In Proceedings of the 38th International Conference on
+Machine Learning, pp. 1238â1248. PMLR, 2021. > > [Code available on GitHub.]
+(https://github.com/VincentStimper/hmc-hyperparameter-tuning) > Vincent
+Stimper, Bernhard SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Resampling
+Base Distributions of Normalizing Flows](https://proceedings.mlr.press/v151/
+stimper22a). > In Proceedings of The 25th International Conference on
+Artificial Intelligence and Statistics, volume 151, pp. 4915â4936, 2022. > >
+[Code available on GitHub.](https://github.com/VincentStimper/resampled-base-
+flows) > Laurence I. Midgley, Vincent Stimper, Gregor N. C. Simm, Bernhard
+SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Flow Annealed Importance
+Sampling Bootstrap](https://arxiv.org/abs/2208.01893). > arXiv preprint arXiv:
+2208.01893, 2022. > > [Code available on GitHub.](https://github.com/lollcat/
+fab-torch) Moreover, the [`boltzgen`](https://github.com/VincentStimper/
+boltzmann-generators) package has been build upon `normflows`. ## Citation If
+you use `normflows`, please consider citing the [corresponding paper](https://
+arxiv.org/abs/2302.12014) as follows. > Vincent Stimper, David Liu, Andrew
+Campbell, Vincent Berenz, Lukas Ryll, Bernhard SchÃ¶lkopf, JosÃ© Miguel
+HernÃ¡ndez-Lobato. > normflows: A PyTorch Package for Normalizing Flows, arXiv
+preprint arXiv:2302.12014, 2023. **Bibtex** ``` @article{normflows, author =
+{Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz and Lukas
+Ryll and Bernhard Sch{\"o}lkopf and Jos{\'e} Miguel Hern{\'a}ndez-Lobato},
+title = {normflows: {A} {P}y{T}orch {P}ackage for {N}ormalizing {F}lows},
+journal = {arXiv preprint arXiv:2302.12014}, year = {2023} } ```
```

### Comparing `normflows-1.6.2/normflows/core.py` & `normflows-1.7.0/normflows/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -342,14 +342,63 @@
           y: Batch of targets, if applicable
 
         Returns:
             Negative log-likelihood of the batch
         """
         return -self.log_prob(x, y)
 
+    def forward_and_log_det(self, z):
+        """Get observed variable x from list of latent variables z
+
+        Args:
+            z: List of latent variables
+
+        Returns:
+            Observed variable x, log determinant of Jacobian
+        """
+        log_det = torch.zeros(len(z[0]), dtype=z[0].dtype, device=z[0].device)
+        for i in range(len(self.q0)):
+            if i == 0:
+                z_ = z[0]
+            else:
+                z_, log_det_ = self.merges[i - 1]([z_, z[i]])
+                log_det += log_det_
+            for flow in self.flows[i]:
+                z_, log_det_ = flow(z_)
+                log_det += log_det_
+        if self.transform is not None:
+            z_, log_det_ = self.transform(z_)
+            log_det += log_det_
+        return z_, log_det
+
+    def inverse_and_log_det(self, x):
+        """Get latent variable z from observed variable x
+
+        Args:
+            x: Observed variable
+
+        Returns:
+            List of latent variables z, log determinant of Jacobian
+        """
+        log_det = torch.zeros(len(x), dtype=x.dtype, device=x.device)
+        if self.transform is not None:
+            x, log_det_ = self.transform.inverse(x)
+            log_det += log_det_
+        z = [None] * len(self.q0)
+        for i in range(len(self.q0) - 1, -1, -1):
+            for flow in reversed(self.flows[i]):
+                x, log_det_ = flow.inverse(x)
+                log_det += log_det_
+            if i == 0:
+                z[i] = x
+            else:
+                [x, z[i]], log_det_ = self.merges[i - 1].inverse(x)
+                log_det += log_det_
+        return z, log_det
+
     def sample(self, num_samples=1, y=None, temperature=None):
         """Samples from flow-based approximate distribution
 
         Args:
           num_samples: Number of samples to draw
           y: Classes to sample from, will be sampled uniformly if None
           temperature: Temperature parameter for temp annealed sampling
```

### Comparing `normflows-1.6.2/normflows/core_test.py` & `normflows-1.7.0/normflows/core_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,20 @@
                 assert log_q_.shape == (batch_size,)
                 assert log_q.dtype == x.dtype
                 assert log_q_.dtype == x.dtype
                 assert_close(log_q, log_q_)
                 fwd = model.forward(x, y)
                 fwd_kld = model.forward_kld(x, y)
                 assert_close(torch.mean(fwd), fwd_kld)
+                z, log_det = model.inverse_and_log_det(x)
+                x_, log_det_ = model.forward_and_log_det(z)
+                assert len(z) == L
+                assert x_.shape == (batch_size,) + (input_shape)
+                assert_close(x_, x)
+                assert_close(log_det, -log_det_)
 
 
     def test_normalizing_flow_vae(self):
         batch_size = 5
         n_dim = 10
         n_layers = 2
         n_bottleneck = 3
```

### Comparing `normflows-1.6.2/normflows/distributions/__init__.py` & `normflows-1.7.0/normflows/distributions/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,21 @@
     ClassCondDiagGaussian,
     GlowBase,
     AffineGaussian,
     GaussianMixture,
     GaussianPCA,
     UniformGaussian,
 )
-from .target import Target, TwoMoons, CircularGaussianMixture, RingMixture
+from .target import (
+    Target,
+    TwoMoons,
+    CircularGaussianMixture,
+    RingMixture,
+    TwoIndependent
+)
 
 from .encoder import BaseEncoder, Dirac, Uniform, NNDiagGaussian
 from .decoder import BaseDecoder, NNDiagGaussianDecoder, NNBernoulliDecoder
 from .prior import (
     PriorDistribution,
     ImagePrior,
     TwoModes,
```

### Comparing `normflows-1.6.2/normflows/distributions/base.py` & `normflows-1.7.0/normflows/distributions/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,54 @@
         log_p = -0.5 * self.d * np.log(2 * np.pi) - torch.sum(
             log_scale + 0.5 * torch.pow((z - self.loc) / torch.exp(log_scale), 2),
             list(range(1, self.n_dim + 1)),
         )
         return log_p
 
 
+class Uniform(BaseDistribution):
+    """
+    Multivariate uniform distribution
+    """
+
+    def __init__(self, shape, low=-1.0, high=1.0):
+        """Constructor
+
+        Args:
+          shape: Tuple with shape of data, if int shape has one dimension
+          low: Lower bound of uniform distribution
+          high: Upper bound of uniform distribution
+        """
+        super().__init__()
+        if isinstance(shape, int):
+            shape = (shape,)
+        if isinstance(shape, list):
+            shape = tuple(shape)
+        self.shape = shape
+        self.d = np.prod(shape)
+        self.low = torch.tensor(low)
+        self.high = torch.tensor(high)
+        self.log_prob_val = -self.d * np.log(self.high - self.low)
+
+    def forward(self, num_samples=1):
+        eps = torch.rand(
+            (num_samples,) + self.shape, dtype=self.low.dtype, device=self.low.device
+        )
+        z = self.low + (self.high - self.low) * eps
+        log_p = self.log_prob_val * torch.ones(num_samples, device=self.low.device)
+        return z, log_p
+
+    def log_prob(self, z):
+        log_p = self.log_prob_val * torch.ones(z.shape[0], device=z.device)
+        out_range = torch.logical_or(z < self.low, z > self.high)
+        ind_inf = torch.any(torch.reshape(out_range, (z.shape[0], -1)), dim=-1)
+        log_p[ind_inf] = -np.inf
+        return log_p
+
+
 class UniformGaussian(BaseDistribution):
     """
     Distribution of a 1D random variable with some entries having a uniform and
     others a Gaussian distribution
     """
 
     def __init__(self, ndim, ind, scale=None):
```

### Comparing `normflows-1.6.2/normflows/distributions/base_test.py` & `normflows-1.7.0/normflows/distributions/base_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import unittest
 import torch
 import numpy as np
 
 from normflows.distributions.base import DiagGaussian, UniformGaussian, \
     ClassCondDiagGaussian, GlowBase, AffineGaussian, GaussianMixture, \
-    GaussianPCA
+    GaussianPCA, Uniform
 from normflows.distributions.distribution_test import DistributionTest
 
 
 class BaseTest(DistributionTest):
     def test_diag_gaussian(self):
         for shape in [1, (3,), [2, 3]]:
             for num_samples in [1, 3]:
                 with self.subTest(shape=shape, num_samples=num_samples):
                     distribution = DiagGaussian(shape)
                     self.checkForwardLogProb(distribution, num_samples)
                     _ = self.checkSample(distribution, num_samples)
 
+    def test_uniform(self):
+        for shape in [1, (3,), [2, 3]]:
+            for num_samples in [1, 3]:
+                with self.subTest(shape=shape, num_samples=num_samples):
+                    distribution = Uniform(shape)
+                    self.checkForwardLogProb(distribution, num_samples)
+                    _ = self.checkSample(distribution, num_samples)
+
     def test_uniform_gaussian(self):
         params = [(2, 1, None), (2, (0,), 0.5 * torch.ones(2)),
                   (4, [2], None), (3, [2, 0], np.pi * torch.ones(3))]
         for ndim, ind, scale in params:
             for num_samples in [1, 3]:
                 with self.subTest(ndim=ndim, ind=ind, scale=scale,
                                   num_samples=num_samples):
@@ -82,14 +90,14 @@
                     _ = self.checkSample(distribution, num_samples)
 
     def test_gaussian_pca(self):
         params = [(1, 1), (4, 2), (5, 1)]
         for dim, latent_dim in params:
             for num_samples in [1, 3]:
                 with self.subTest(dim=dim, latent_dim=latent_dim):
-                    distribution = GaussianMixture(dim, latent_dim)
+                    distribution = GaussianPCA(dim, latent_dim)
                     self.checkForwardLogProb(distribution, num_samples)
                     _ = self.checkSample(distribution, num_samples)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `normflows-1.6.2/normflows/distributions/decoder.py` & `normflows-1.7.0/normflows/distributions/decoder.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/distributions/decoder_test.py` & `normflows-1.7.0/normflows/distributions/decoder_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/distributions/distribution_test.py` & `normflows-1.7.0/normflows/distributions/distribution_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/distributions/encoder.py` & `normflows-1.7.0/normflows/distributions/encoder.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/distributions/encoder_test.py` & `normflows-1.7.0/normflows/distributions/encoder_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/distributions/linear_interpolation.py` & `normflows-1.7.0/normflows/distributions/linear_interpolation.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/distributions/mh_proposal.py` & `normflows-1.7.0/normflows/distributions/mh_proposal.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/distributions/prior.py` & `normflows-1.7.0/normflows/distributions/prior.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/distributions/prior_test.py` & `normflows-1.7.0/normflows/distributions/prior_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/distributions/target.py` & `normflows-1.7.0/normflows/distributions/target.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numpy as np
 import torch
 from torch import nn
 
+from ..flows.reshape import Split
+
 
 class Target(nn.Module):
     """
     Sample target distributions to test models
     """
 
     def __init__(self, prop_scale=torch.tensor(6.0), prop_shift=torch.tensor(-3.0)):
@@ -67,14 +69,37 @@
         while len(z) < num_samples:
             z_ = self.rejection_sampling(num_samples)
             ind = np.min([len(z_), num_samples - len(z)])
             z = torch.cat([z, z_[:ind, :]], 0)
         return z
 
 
+class TwoIndependent(Target):
+    """
+    Target distribution that combines two independent distributions of equal
+    size into one distribution. This is needed for Augmented Normalizing Flows,
+    see https://arxiv.org/abs/2002.07101
+    """
+
+    def __init__(self, target1, target2):
+        super().__init__()
+        self.target1 = target1
+        self.target2 = target2
+        self.split = Split(mode='channel')
+
+    def log_prob(self, z):
+        z1, z2 = self.split(z)[0]
+        return self.target1.log_prob(z1) + self.target2.log_prob(z2)
+
+    def sample(self, num_samples=1):
+        z1 = self.target1.sample(num_samples)
+        z2 = self.target2.sample(num_samples)
+        return self.split.inverse([z1, z2])[0]
+
+
 class TwoMoons(Target):
     """
     Bimodal two-dimensional distribution
     """
 
     def __init__(self):
         super().__init__()
```

### Comparing `normflows-1.6.2/normflows/distributions/target_test.py` & `normflows-1.7.0/normflows/distributions/target_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 import unittest
-import torch
 
+from normflows.distributions.base import DiagGaussian
 from normflows.distributions.target import TwoMoons, \
-    CircularGaussianMixture, RingMixture
+    CircularGaussianMixture, RingMixture, TwoIndependent
 
 
 class TargetTest(unittest.TestCase):
     def test_targets(self):
         targets = [TwoMoons, CircularGaussianMixture,
                    RingMixture]
         for num_samples in [1, 5]:
             for target_ in targets:
                 with self.subTest(num_samples=num_samples,
                                   target_=target_):
-                    # Set up prior
+                    # Set up target
                     target = target_()
-                    # Test prior
+                    # Test target
                     samples = target.sample(num_samples)
                     assert samples.shape == (num_samples, 2)
                     log_p = target.log_prob(samples)
                     assert log_p.shape == (num_samples,)
 
+    def test_two_independent(self):
+        target = TwoIndependent(TwoMoons(), DiagGaussian(2))
+        for num_samples in [1, 5]:
+            with self.subTest(num_samples=num_samples):
+                # Test target
+                samples = target.sample(num_samples)
+                assert samples.shape == (num_samples, 4)
+                log_p = target.log_prob(samples)
+                assert log_p.shape == (num_samples,)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `normflows-1.6.2/normflows/flows/__init__.py` & `normflows-1.7.0/normflows/flows/__init__.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/affine/autoregressive.py` & `normflows-1.7.0/normflows/flows/affine/autoregressive.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/affine/autoregressive_test.py` & `normflows-1.7.0/normflows/flows/affine/autoregressive_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/affine/coupling.py` & `normflows-1.7.0/normflows/flows/affine/coupling.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/affine/coupling_test.py` & `normflows-1.7.0/normflows/flows/affine/coupling_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/affine/glow.py` & `normflows-1.7.0/normflows/flows/affine/glow.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/affine/glow_test.py` & `normflows-1.7.0/normflows/flows/affine/glow_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/base.py` & `normflows-1.7.0/normflows/flows/base.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/base_test.py` & `normflows-1.7.0/normflows/flows/base_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/flow_test.py` & `normflows-1.7.0/normflows/flows/flow_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/mixing.py` & `normflows-1.7.0/normflows/flows/mixing.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/mixing_test.py` & `normflows-1.7.0/normflows/flows/mixing_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/neural_spline/autoregressive.py` & `normflows-1.7.0/normflows/flows/neural_spline/autoregressive.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/neural_spline/autoregressive_test.py` & `normflows-1.7.0/normflows/flows/neural_spline/autoregressive_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/neural_spline/coupling.py` & `normflows-1.7.0/normflows/flows/neural_spline/coupling.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/neural_spline/coupling_test.py` & `normflows-1.7.0/normflows/flows/neural_spline/coupling_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/neural_spline/wrapper.py` & `normflows-1.7.0/normflows/flows/neural_spline/wrapper.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/neural_spline/wrapper_test.py` & `normflows-1.7.0/normflows/flows/neural_spline/wrapper_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/normalization.py` & `normflows-1.7.0/normflows/flows/normalization.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/periodic.py` & `normflows-1.7.0/normflows/flows/periodic.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/periodic_test.py` & `normflows-1.7.0/normflows/flows/periodic_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/planar.py` & `normflows-1.7.0/normflows/flows/planar.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/planar_test.py` & `normflows-1.7.0/normflows/flows/planar_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/radial.py` & `normflows-1.7.0/normflows/flows/radial.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/reshape.py` & `normflows-1.7.0/normflows/flows/reshape.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/residual.py` & `normflows-1.7.0/normflows/flows/residual.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/residual_test.py` & `normflows-1.7.0/normflows/flows/residual_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/stochastic.py` & `normflows-1.7.0/normflows/flows/stochastic.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/flows/stochastic_test.py` & `normflows-1.7.0/normflows/flows/stochastic_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/nets/cnn.py` & `normflows-1.7.0/normflows/nets/cnn.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/nets/lipschitz.py` & `normflows-1.7.0/normflows/nets/lipschitz.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/nets/made.py` & `normflows-1.7.0/normflows/nets/made.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/nets/made_test.py` & `normflows-1.7.0/normflows/nets/made_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/nets/mlp.py` & `normflows-1.7.0/normflows/nets/mlp.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/nets/resnet.py` & `normflows-1.7.0/normflows/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/sampling/hais.py` & `normflows-1.7.0/normflows/sampling/hais.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/transforms.py` & `normflows-1.7.0/normflows/transforms.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/transforms_test.py` & `normflows-1.7.0/normflows/transforms_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/utils/eval.py` & `normflows-1.7.0/normflows/utils/eval.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/utils/masks.py` & `normflows-1.7.0/normflows/utils/masks.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/utils/nn.py` & `normflows-1.7.0/normflows/utils/nn.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/utils/optim.py` & `normflows-1.7.0/normflows/utils/optim.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/utils/preprocessing.py` & `normflows-1.7.0/normflows/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/utils/splines.py` & `normflows-1.7.0/normflows/utils/splines.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows/utils/splines_test.py` & `normflows-1.7.0/normflows/utils/splines_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/normflows.egg-info/PKG-INFO` & `normflows-1.7.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,15 @@
-Metadata-Version: 2.1
-Name: normflows
-Version: 1.6.2
-Summary: Pytorch implementation of normalizing flows
-Home-page: https://github.com/VincentStimper/normalizing-flows
-Author: Vincent Stimper
-Author-email: vincent.stimper@tuebingen.mpg.de
-License: MIT
-Download-URL: https://github.com/VincentStimper/normalizing-flows/archive/refs/heads/master.zip
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-License-File: LICENSE
-
 # `normflows`: A PyTorch Package for Normalizing Flows
 
 [![documentation](https://github.com/VincentStimper/normalizing-flows/actions/workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-flows/)
 ![unit-tests](https://github.com/VincentStimper/normalizing-flows/actions/workflows/pytest.yaml/badge.svg)
 ![code coverage](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true)
 [![License: MIT](https://img.shields.io/badge/Licence-MIT-lightgrey)](https://opensource.org/licenses/MIT)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/2302.12014) 
-[![PyPI](https://img.shields.io/badge/PyPI-1.6.2-blue.svg)](https://pypi.org/project/normflows/)
+[![PyPI](https://img.shields.io/badge/PyPI-1.7.0-blue.svg)](https://pypi.org/project/normflows/)
 [![Downloads](https://static.pepy.tech/personalized-badge/normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/normflows)
 
 
 `normflows` is a PyTorch implementation of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed via pip](#installation).
 The basic usage is described [here](#usage), and a [full documentation](https://vincentstimper.github.io/normalizing-flows/) 
 is available as well. A more detailed description of this package is given in out accompanying 
@@ -36,18 +19,19 @@
 [`examples` folder](https://github.com/VincentStimper/normalizing-flows/blob/master/examples), 
 including [Glow](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/glow.ipynb),
 a [VAE](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/vae.py), and
 a [Residual Flow](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/residual.ipynb).
 Moreover, two simple applications are highlighed in the [examples section](#examples). You can run them 
 yourself in Google Colab using the links below to get a feeling for `normflows`.
 
-| Link                                                                                                                                                                                                                                         | Description                                                                   |
-|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------|
-| <a href="https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/real_nvp_colab.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> | Real NVP applied to a 2D bimodal target distribution                          |
+| Link                                                                                                                                                                                                                                                  | Description                                                             |
+|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------|
+| <a href="https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/real_nvp_colab.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>          | Real NVP applied to a 2D bimodal target distribution                    |
 | <a href="https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/paper_example_nsf_colab.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> | Modeling a distribution on a cylinder surface with a neural spline flow |
+| <a href="https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/glow_colab.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>              | Modeling and generating CIFAR-10 images with Glow                       |
 
 
 ## Implemented Flows
 
 | Architecture | Reference                                                                                                                 |
 |--------------|---------------------------------------------------------------------------------------------------------------------------|
 | Planar Flow  | [Rezende & Mohamed, 2015](http://proceedings.mlr.press/v37/rezende15.html)                                                |
@@ -189,14 +173,38 @@
 which is available in [Colab](https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/paper_example_nsf_colab.ipynb)
 as well, we apply a Neural Spline Flow model to a distribution defined on a cylinder. The resulting density is visualized below.
 
 ![Neural Spline Flow applied to target distribution on a cylinder](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/master/figures/nsf_cylinder_3d.png)
 
 This example is considered in the [paper](https://arxiv.org/abs/2302.12014) accompanying this repository.
 
+## Support
+
+If you have problems, please read the [package documentation](https://vincentstimper.github.io/normalizing-flows/)
+and check out the [examples section](#examples) above. You are also welcome to 
+[create issues on GitHub](https://github.com/VincentStimper/normalizing-flows/issues) to get help. Note that it is
+worthwhile browsing the existing [open](https://github.com/VincentStimper/normalizing-flows/issues?q=is%3Aopen+is%3Aissue) 
+and [closed](https://github.com/VincentStimper/normalizing-flows/issues?q=is%3Aissue+is%3Aclosed) issues, which might
+address the problem you are facing.
+
+## Contributing
+
+If you find a bug or have a feature request, please 
+[file an issue on GitHub](https://github.com/VincentStimper/normalizing-flows/issues).
+
+You are welcome to contribute to the package by fixing the bug or adding the feature yourself. If you want to 
+contribute, please add tests for the code you added or modified and ensure it passes successfully by running `pytest`.
+This can be done by simply executing
+```
+pytest
+```
+within your local version of the repository. Make sure you code is well documented, and we also encourage contributions
+to the existing documentation. Once you finished coding and testing, please 
+[create a pull request on GitHub](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).
+
 ## Used by
 
 The package has been used in several research papers, which are listed below.
 
 > Andrew Campbell, Wenlong Chen, Vincent Stimper, José Miguel Hernández-Lobato, and Yichuan Zhang. 
 > [A gradient based strategy for Hamiltonian Monte Carlo hyperparameter optimization](https://proceedings.mlr.press/v139/campbell21a.html). 
 > In Proceedings of the 38th International Conference on Machine Learning, pp. 1238–1248. PMLR, 2021.
@@ -236,9 +244,7 @@
 }
 ```
 
 
 
 
 
-
-
```

#### html2text {}

```diff
@@ -1,27 +1,18 @@
-Metadata-Version: 2.1 Name: normflows Version: 1.6.2 Summary: Pytorch
-implementation of normalizing flows Home-page: https://github.com/
-VincentStimper/normalizing-flows Author: Vincent Stimper Author-email:
-vincent.stimper@tuebingen.mpg.de License: MIT Download-URL: https://github.com/
-VincentStimper/normalizing-flows/archive/refs/heads/master.zip Platform:
-UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
-Audience :: Developers Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown Provides-Extra: docs License-File:
-LICENSE # `normflows`: A PyTorch Package for Normalizing Flows [!
-[documentation](https://github.com/VincentStimper/normalizing-flows/actions/
-workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-
-flows/) ![unit-tests](https://github.com/VincentStimper/normalizing-flows/
-actions/workflows/pytest.yaml/badge.svg) ![code coverage](https://
-raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/
-coverage.svg?raw=true) [![License: MIT](https://img.shields.io/badge/Licence-
-MIT-lightgrey)](https://opensource.org/licenses/MIT) [![arXiv](https://
-img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/
-2302.12014) [![PyPI](https://img.shields.io/badge/PyPI-1.6.2-blue.svg)](https:/
-/pypi.org/project/normflows/) [![Downloads](https://static.pepy.tech/
-personalized-badge/
+# `normflows`: A PyTorch Package for Normalizing Flows [![documentation](https:
+//github.com/VincentStimper/normalizing-flows/actions/workflows/mkdocs.yaml/
+badge.svg)](https://vincentstimper.github.io/normalizing-flows/) ![unit-tests]
+(https://github.com/VincentStimper/normalizing-flows/actions/workflows/
+pytest.yaml/badge.svg) ![code coverage](https://raw.githubusercontent.com/
+VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true) [!
+[License: MIT](https://img.shields.io/badge/Licence-MIT-lightgrey)](https://
+opensource.org/licenses/MIT) [![arXiv](https://img.shields.io/badge/arXiv-
+2302.12014-b31b1b.svg)](https://arxiv.org/abs/2302.12014) [![PyPI](https://
+img.shields.io/badge/PyPI-1.7.0-blue.svg)](https://pypi.org/project/normflows/
+) [![Downloads](https://static.pepy.tech/personalized-badge/
 normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)]
 (https://pepy.tech/project/normflows) `normflows` is a PyTorch implementation
 of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed
 via pip](#installation). The basic usage is described [here](#usage), and a
 [full documentation](https://vincentstimper.github.io/normalizing-flows/) is
 available as well. A more detailed description of this package is given in out
@@ -33,18 +24,19 @@
 examples/vae.py), and a [Residual Flow](https://github.com/VincentStimper/
 normalizing-flows/blob/master/examples/residual.ipynb). Moreover, two simple
 applications are highlighed in the [examples section](#examples). You can run
 them yourself in Google Colab using the links below to get a feeling for
 `normflows`. | Link | Description | |------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
---------------------------------------|----------------------------------------
----------------------------------------| | [Open_In_Colab] | Real NVP applied
-to a 2D bimodal target distribution | | [Open_In_Colab] | Modeling a
-distribution on a cylinder surface with a neural spline flow | ## Implemented
+-----------------------------------------------|-------------------------------
+------------------------------------------| | [Open_In_Colab] | Real NVP
+applied to a 2D bimodal target distribution | | [Open_In_Colab] | Modeling a
+distribution on a cylinder surface with a neural spline flow | | [Open_In
+Colab] | Modeling and generating CIFAR-10 images with Glow | ## Implemented
 Flows | Architecture | Reference | |--------------|----------------------------
 -------------------------------------------------------------------------------
 ----------------| | Planar Flow | [Rezende & Mohamed, 2015](http://
 proceedings.mlr.press/v37/rezende15.html) | | Radial Flow | [Rezende & Mohamed,
 2015](http://proceedings.mlr.press/v37/rezende15.html) | | NICE | [Dinh et al.,
 2014](https://arxiv.org/abs/1410.8516) | | Real NVP | [Dinh et al., 2017]
 (https://openreview.net/forum?id=HkpbnH9lx) | | Glow | [Kingma et al., 2018]
@@ -127,34 +119,53 @@
 (https://colab.research.google.com/github/VincentStimper/normalizing-flows/
 blob/master/examples/paper_example_nsf_colab.ipynb) as well, we apply a Neural
 Spline Flow model to a distribution defined on a cylinder. The resulting
 density is visualized below. ![Neural Spline Flow applied to target
 distribution on a cylinder](https://raw.githubusercontent.com/VincentStimper/
 normalizing-flows/master/figures/nsf_cylinder_3d.png) This example is
 considered in the [paper](https://arxiv.org/abs/2302.12014) accompanying this
-repository. ## Used by The package has been used in several research papers,
-which are listed below. > Andrew Campbell, Wenlong Chen, Vincent Stimper, JosÃ©
-Miguel HernÃ¡ndez-Lobato, and Yichuan Zhang. > [A gradient based strategy for
-Hamiltonian Monte Carlo hyperparameter optimization](https://
-proceedings.mlr.press/v139/campbell21a.html). > In Proceedings of the 38th
-International Conference on Machine Learning, pp. 1238â1248. PMLR, 2021. > >
-[Code available on GitHub.](https://github.com/VincentStimper/hmc-
-hyperparameter-tuning) > Vincent Stimper, Bernhard SchÃ¶lkopf, JosÃ© Miguel
-HernÃ¡ndez-Lobato. > [Resampling Base Distributions of Normalizing Flows]
-(https://proceedings.mlr.press/v151/stimper22a). > In Proceedings of The 25th
-International Conference on Artificial Intelligence and Statistics, volume 151,
-pp. 4915â4936, 2022. > > [Code available on GitHub.](https://github.com/
-VincentStimper/resampled-base-flows) > Laurence I. Midgley, Vincent Stimper,
-Gregor N. C. Simm, Bernhard SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Flow
-Annealed Importance Sampling Bootstrap](https://arxiv.org/abs/2208.01893). >
-arXiv preprint arXiv:2208.01893, 2022. > > [Code available on GitHub.](https://
-github.com/lollcat/fab-torch) Moreover, the [`boltzgen`](https://github.com/
-VincentStimper/boltzmann-generators) package has been build upon `normflows`.
-## Citation If you use `normflows`, please consider citing the [corresponding
-paper](https://arxiv.org/abs/2302.12014) as follows. > Vincent Stimper, David
-Liu, Andrew Campbell, Vincent Berenz, Lukas Ryll, Bernhard SchÃ¶lkopf, JosÃ©
-Miguel HernÃ¡ndez-Lobato. > normflows: A PyTorch Package for Normalizing Flows,
-arXiv preprint arXiv:2302.12014, 2023. **Bibtex** ``` @article{normflows,
-author = {Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz
-and Lukas Ryll and Bernhard Sch{\"o}lkopf and Jos{\'e} Miguel Hern{\'a}ndez-
-Lobato}, title = {normflows: {A} {P}y{T}orch {P}ackage for {N}ormalizing
-{F}lows}, journal = {arXiv preprint arXiv:2302.12014}, year = {2023} } ```
+repository. ## Support If you have problems, please read the [package
+documentation](https://vincentstimper.github.io/normalizing-flows/) and check
+out the [examples section](#examples) above. You are also welcome to [create
+issues on GitHub](https://github.com/VincentStimper/normalizing-flows/issues)
+to get help. Note that it is worthwhile browsing the existing [open](https://
+github.com/VincentStimper/normalizing-flows/issues?q=is%3Aopen+is%3Aissue) and
+[closed](https://github.com/VincentStimper/normalizing-flows/
+issues?q=is%3Aissue+is%3Aclosed) issues, which might address the problem you
+are facing. ## Contributing If you find a bug or have a feature request, please
+[file an issue on GitHub](https://github.com/VincentStimper/normalizing-flows/
+issues). You are welcome to contribute to the package by fixing the bug or
+adding the feature yourself. If you want to contribute, please add tests for
+the code you added or modified and ensure it passes successfully by running
+`pytest`. This can be done by simply executing ``` pytest ``` within your local
+version of the repository. Make sure you code is well documented, and we also
+encourage contributions to the existing documentation. Once you finished coding
+and testing, please [create a pull request on GitHub](https://docs.github.com/
+en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-
+work-with-pull-requests/creating-a-pull-request). ## Used by The package has
+been used in several research papers, which are listed below. > Andrew
+Campbell, Wenlong Chen, Vincent Stimper, JosÃ© Miguel HernÃ¡ndez-Lobato, and
+Yichuan Zhang. > [A gradient based strategy for Hamiltonian Monte Carlo
+hyperparameter optimization](https://proceedings.mlr.press/v139/
+campbell21a.html). > In Proceedings of the 38th International Conference on
+Machine Learning, pp. 1238â1248. PMLR, 2021. > > [Code available on GitHub.]
+(https://github.com/VincentStimper/hmc-hyperparameter-tuning) > Vincent
+Stimper, Bernhard SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Resampling
+Base Distributions of Normalizing Flows](https://proceedings.mlr.press/v151/
+stimper22a). > In Proceedings of The 25th International Conference on
+Artificial Intelligence and Statistics, volume 151, pp. 4915â4936, 2022. > >
+[Code available on GitHub.](https://github.com/VincentStimper/resampled-base-
+flows) > Laurence I. Midgley, Vincent Stimper, Gregor N. C. Simm, Bernhard
+SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Flow Annealed Importance
+Sampling Bootstrap](https://arxiv.org/abs/2208.01893). > arXiv preprint arXiv:
+2208.01893, 2022. > > [Code available on GitHub.](https://github.com/lollcat/
+fab-torch) Moreover, the [`boltzgen`](https://github.com/VincentStimper/
+boltzmann-generators) package has been build upon `normflows`. ## Citation If
+you use `normflows`, please consider citing the [corresponding paper](https://
+arxiv.org/abs/2302.12014) as follows. > Vincent Stimper, David Liu, Andrew
+Campbell, Vincent Berenz, Lukas Ryll, Bernhard SchÃ¶lkopf, JosÃ© Miguel
+HernÃ¡ndez-Lobato. > normflows: A PyTorch Package for Normalizing Flows, arXiv
+preprint arXiv:2302.12014, 2023. **Bibtex** ``` @article{normflows, author =
+{Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz and Lukas
+Ryll and Bernhard Sch{\"o}lkopf and Jos{\'e} Miguel Hern{\'a}ndez-Lobato},
+title = {normflows: {A} {P}y{T}orch {P}ackage for {N}ormalizing {F}lows},
+journal = {arXiv preprint arXiv:2302.12014}, year = {2023} } ```
```

### Comparing `normflows-1.6.2/normflows.egg-info/SOURCES.txt` & `normflows-1.7.0/normflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `normflows-1.6.2/setup.py` & `normflows-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
-__version__ = "1.6.2"
+__version__ = "1.7.0"
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
```

