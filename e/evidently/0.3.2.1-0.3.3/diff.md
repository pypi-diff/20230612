# Comparing `tmp/evidently-0.3.2.1.tar.gz` & `tmp/evidently-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evidently-0.3.2.1.tar", last modified: Mon May 22 10:49:13 2023, max compression
+gzip compressed data, was "evidently-0.3.3.tar", last modified: Mon Jun 12 17:22:56 2023, max compression
```

## Comparing `evidently-0.3.2.1.tar` & `evidently-0.3.3.tar`

### file list

```diff
@@ -1,209 +1,221 @@
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.036625 evidently-0.3.2.1/
--rw-r--r--   0 emelidral   (501) staff       (20)      375 2023-05-22 10:49:13.036769 evidently-0.3.2.1/PKG-INFO
--rw-r--r--   0 emelidral   (501) staff       (20)     1447 2023-04-11 11:50:44.033151 evidently-0.3.2.1/setup.cfg
--rw-r--r--   0 emelidral   (501) staff       (20)     2103 2023-05-19 15:16:08.556083 evidently-0.3.2.1/setup.py
--rw-r--r--   0 emelidral   (501) staff       (20)    22071 2023-04-11 11:50:44.033364 evidently-0.3.2.1/setupbase.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:12.997738 evidently-0.3.2.1/src/
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.001421 evidently-0.3.2.1/src/evidently/
--rw-r--r--   0 emelidral   (501) staff       (20)      256 2023-04-11 11:50:44.033482 evidently-0.3.2.1/src/evidently/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1892 2023-04-27 10:27:02.402053 evidently-0.3.2.1/src/evidently/__main__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      162 2023-04-11 11:50:44.033618 evidently-0.3.2.1/src/evidently/_config.py
--rw-r--r--   0 emelidral   (501) staff       (20)      114 2023-05-22 10:49:07.844116 evidently-0.3.2.1/src/evidently/_version.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7505 2023-04-27 10:27:02.402425 evidently-0.3.2.1/src/evidently/base_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.002922 evidently-0.3.2.1/src/evidently/calculations/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.034605 evidently-0.3.2.1/src/evidently/calculations/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    14543 2023-04-11 11:50:44.034697 evidently-0.3.2.1/src/evidently/calculations/classification_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)    16746 2023-05-19 15:16:08.556277 evidently-0.3.2.1/src/evidently/calculations/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2662 2023-04-11 11:50:44.034844 evidently-0.3.2.1/src/evidently/calculations/data_integration.py
--rw-r--r--   0 emelidral   (501) staff       (20)    32977 2023-05-19 15:16:08.556544 evidently-0.3.2.1/src/evidently/calculations/data_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8286 2023-04-11 11:50:44.035061 evidently-0.3.2.1/src/evidently/calculations/regression_performance.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.007816 evidently-0.3.2.1/src/evidently/calculations/stattests/
--rw-r--r--   0 emelidral   (501) staff       (20)     1258 2023-04-27 10:27:02.403157 evidently-0.3.2.1/src/evidently/calculations/stattests/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1337 2023-04-11 11:50:44.035216 evidently-0.3.2.1/src/evidently/calculations/stattests/anderson_darling_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1741 2023-04-11 11:50:44.035280 evidently-0.3.2.1/src/evidently/calculations/stattests/chisquare_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7331 2023-04-27 10:27:02.403563 evidently-0.3.2.1/src/evidently/calculations/stattests/cramer_von_mises_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1533 2023-04-11 11:50:44.035446 evidently-0.3.2.1/src/evidently/calculations/stattests/energy_distance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2108 2023-04-11 11:50:44.035531 evidently-0.3.2.1/src/evidently/calculations/stattests/epps_singleton_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2592 2023-04-11 11:50:44.035581 evidently-0.3.2.1/src/evidently/calculations/stattests/fisher_exact_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2025 2023-04-11 11:50:44.035635 evidently-0.3.2.1/src/evidently/calculations/stattests/g_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2983 2023-04-11 11:50:44.035704 evidently-0.3.2.1/src/evidently/calculations/stattests/hellinger_distance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2152 2023-04-11 11:50:44.035768 evidently-0.3.2.1/src/evidently/calculations/stattests/jensenshannon.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1899 2023-04-11 11:50:44.035819 evidently-0.3.2.1/src/evidently/calculations/stattests/kl_div.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1545 2023-04-11 11:50:44.035878 evidently-0.3.2.1/src/evidently/calculations/stattests/ks_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1752 2023-05-19 15:16:08.556697 evidently-0.3.2.1/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4683 2023-04-11 11:50:44.036014 evidently-0.3.2.1/src/evidently/calculations/stattests/mmd_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1812 2023-04-11 11:50:44.036061 evidently-0.3.2.1/src/evidently/calculations/stattests/psi.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4696 2023-04-27 10:27:02.403868 evidently-0.3.2.1/src/evidently/calculations/stattests/registry.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1490 2023-04-11 11:50:44.036213 evidently-0.3.2.1/src/evidently/calculations/stattests/t_test.py
--rw-r--r--   0 emelidral   (501) staff       (20)      799 2023-04-27 10:27:02.404121 evidently-0.3.2.1/src/evidently/calculations/stattests/text_content_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)      791 2023-04-27 10:27:02.404318 evidently-0.3.2.1/src/evidently/calculations/stattests/text_content_drift_abs.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2746 2023-04-11 11:50:44.036327 evidently-0.3.2.1/src/evidently/calculations/stattests/tvd_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4825 2023-04-11 11:50:44.036404 evidently-0.3.2.1/src/evidently/calculations/stattests/utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1832 2023-04-11 11:50:44.036454 evidently-0.3.2.1/src/evidently/calculations/stattests/wasserstein_distance_norm.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2878 2023-04-11 11:50:44.036512 evidently-0.3.2.1/src/evidently/calculations/stattests/z_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.036630 evidently-0.3.2.1/src/evidently/calculations/utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7042 2023-04-24 17:06:50.387018 evidently-0.3.2.1/src/evidently/core.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.008892 evidently-0.3.2.1/src/evidently/descriptors/
--rw-r--r--   0 emelidral   (501) staff       (20)      249 2023-04-11 11:50:44.040731 evidently-0.3.2.1/src/evidently/descriptors/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      578 2023-04-11 11:50:44.040789 evidently-0.3.2.1/src/evidently/descriptors/non_letter_character_percentage_descriptor.py
--rw-r--r--   0 emelidral   (501) staff       (20)      582 2023-04-11 11:50:44.040840 evidently-0.3.2.1/src/evidently/descriptors/oov_words_percentage_descriptor.py
--rw-r--r--   0 emelidral   (501) staff       (20)      464 2023-04-11 11:50:44.040888 evidently-0.3.2.1/src/evidently/descriptors/text_length_descriptor.py
--rw-r--r--   0 emelidral   (501) staff       (20)      776 2023-04-11 11:50:44.040933 evidently-0.3.2.1/src/evidently/descriptors/trigger_words_presence_descriptor.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.010153 evidently-0.3.2.1/src/evidently/features/
--rw-r--r--   0 emelidral   (501) staff       (20)     1682 2023-04-11 11:50:44.041013 evidently-0.3.2.1/src/evidently/features/OOV_words_percentage_feature.py
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.041037 evidently-0.3.2.1/src/evidently/features/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1894 2023-04-11 11:50:44.041102 evidently-0.3.2.1/src/evidently/features/generated_features.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1095 2023-04-11 11:50:44.041157 evidently-0.3.2.1/src/evidently/features/non_letter_character_percentage_feature.py
--rw-r--r--   0 emelidral   (501) staff       (20)      966 2023-04-11 11:50:44.041206 evidently-0.3.2.1/src/evidently/features/text_length_feature.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2121 2023-04-11 11:50:44.041271 evidently-0.3.2.1/src/evidently/features/trigger_words_presence_feature.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.011770 evidently-0.3.2.1/src/evidently/metric_preset/
--rw-r--r--   0 emelidral   (501) staff       (20)      496 2023-04-11 11:50:44.041350 evidently-0.3.2.1/src/evidently/metric_preset/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2526 2023-04-11 11:50:44.041407 evidently-0.3.2.1/src/evidently/metric_preset/classification_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4787 2023-04-27 10:27:02.404624 evidently-0.3.2.1/src/evidently/metric_preset/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1325 2023-04-11 11:50:44.041535 evidently-0.3.2.1/src/evidently/metric_preset/data_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)      343 2023-04-11 11:50:44.041591 evidently-0.3.2.1/src/evidently/metric_preset/metric_preset.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1817 2023-04-11 11:50:44.041650 evidently-0.3.2.1/src/evidently/metric_preset/regression_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7282 2023-04-11 11:50:44.041719 evidently-0.3.2.1/src/evidently/metric_preset/target_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1811 2023-04-11 11:50:44.041776 evidently-0.3.2.1/src/evidently/metric_preset/text_overview.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8904 2023-05-19 15:16:08.556895 evidently-0.3.2.1/src/evidently/metric_results.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.012364 evidently-0.3.2.1/src/evidently/metrics/
--rw-r--r--   0 emelidral   (501) staff       (20)     3737 2023-04-11 11:50:44.041950 evidently-0.3.2.1/src/evidently/metrics/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      691 2023-04-11 11:50:44.042032 evidently-0.3.2.1/src/evidently/metrics/base_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.015254 evidently-0.3.2.1/src/evidently/metrics/classification_performance/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.042092 evidently-0.3.2.1/src/evidently/metrics/classification_performance/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3021 2023-05-19 15:16:08.557044 evidently-0.3.2.1/src/evidently/metrics/classification_performance/base_classification_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3132 2023-04-27 10:27:02.405129 evidently-0.3.2.1/src/evidently/metrics/classification_performance/class_balance_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6441 2023-05-19 15:16:08.557179 evidently-0.3.2.1/src/evidently/metrics/classification_performance/class_separation_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12015 2023-04-27 10:27:02.405315 evidently-0.3.2.1/src/evidently/metrics/classification_performance/classification_dummy_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5193 2023-04-11 11:50:44.042500 evidently-0.3.2.1/src/evidently/metrics/classification_performance/classification_quality_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3569 2023-04-27 10:27:02.405480 evidently-0.3.2.1/src/evidently/metrics/classification_performance/confusion_matrix_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1534 2023-04-11 11:50:44.042621 evidently-0.3.2.1/src/evidently/metrics/classification_performance/objects.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4483 2023-04-11 11:50:44.042685 evidently-0.3.2.1/src/evidently/metrics/classification_performance/pr_curve_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6020 2023-04-11 11:50:44.042749 evidently-0.3.2.1/src/evidently/metrics/classification_performance/pr_table_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5959 2023-04-11 11:50:44.042828 evidently-0.3.2.1/src/evidently/metrics/classification_performance/probability_distribution_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7318 2023-04-11 11:50:44.042904 evidently-0.3.2.1/src/evidently/metrics/classification_performance/quality_by_class_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    17138 2023-05-19 15:16:08.557405 evidently-0.3.2.1/src/evidently/metrics/classification_performance/quality_by_feature_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4425 2023-04-11 11:50:44.043054 evidently-0.3.2.1/src/evidently/metrics/classification_performance/roc_curve_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.017255 evidently-0.3.2.1/src/evidently/metrics/data_drift/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043120 evidently-0.3.2.1/src/evidently/metrics/data_drift/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    18498 2023-05-22 10:48:01.966184 evidently-0.3.2.1/src/evidently/metrics/data_drift/column_drift_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     9686 2023-05-19 15:16:08.557756 evidently-0.3.2.1/src/evidently/metrics/data_drift/column_value_plot.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13396 2023-05-19 15:16:08.557920 evidently-0.3.2.1/src/evidently/metrics/data_drift/data_drift_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4733 2023-05-19 15:16:08.558070 evidently-0.3.2.1/src/evidently/metrics/data_drift/dataset_drift_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    10729 2023-04-27 10:27:02.406479 evidently-0.3.2.1/src/evidently/metrics/data_drift/embedding_drift_methods.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4538 2023-05-19 15:16:08.558192 evidently-0.3.2.1/src/evidently/metrics/data_drift/embeddings_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13793 2023-05-19 15:16:08.558333 evidently-0.3.2.1/src/evidently/metrics/data_drift/target_by_features_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)    11082 2023-05-19 15:16:08.558473 evidently-0.3.2.1/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    11173 2023-04-11 11:50:44.043845 evidently-0.3.2.1/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.018445 evidently-0.3.2.1/src/evidently/metrics/data_integrity/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043904 evidently-0.3.2.1/src/evidently/metrics/data_integrity/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8345 2023-04-11 11:50:44.043991 evidently-0.3.2.1/src/evidently/metrics/data_integrity/column_missing_values_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7142 2023-04-11 11:50:44.044068 evidently-0.3.2.1/src/evidently/metrics/data_integrity/column_regexp_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    28022 2023-05-19 15:16:08.558666 evidently-0.3.2.1/src/evidently/metrics/data_integrity/column_summary_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12456 2023-04-11 11:50:44.044306 evidently-0.3.2.1/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8789 2023-04-11 11:50:44.044393 evidently-0.3.2.1/src/evidently/metrics/data_integrity/dataset_summary_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.020816 evidently-0.3.2.1/src/evidently/metrics/data_quality/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.044472 evidently-0.3.2.1/src/evidently/metrics/data_quality/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5821 2023-04-11 11:50:44.044563 evidently-0.3.2.1/src/evidently/metrics/data_quality/column_correlations_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3054 2023-04-11 11:50:44.044629 evidently-0.3.2.1/src/evidently/metrics/data_quality/column_distribution_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5896 2023-04-27 10:27:02.407846 evidently-0.3.2.1/src/evidently/metrics/data_quality/column_quantile_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6872 2023-04-11 11:50:44.044766 evidently-0.3.2.1/src/evidently/metrics/data_quality/column_value_list_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8991 2023-04-11 11:50:44.044848 evidently-0.3.2.1/src/evidently/metrics/data_quality/column_value_range_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4336 2023-04-11 11:50:44.044913 evidently-0.3.2.1/src/evidently/metrics/data_quality/conflict_prediction_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3927 2023-04-11 11:50:44.044975 evidently-0.3.2.1/src/evidently/metrics/data_quality/conflict_target_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13927 2023-04-11 11:50:44.045061 evidently-0.3.2.1/src/evidently/metrics/data_quality/dataset_correlations_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2657 2023-04-11 11:50:44.045118 evidently-0.3.2.1/src/evidently/metrics/data_quality/stability_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7248 2023-04-11 11:50:44.045194 evidently-0.3.2.1/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5215 2023-04-11 11:50:44.045257 evidently-0.3.2.1/src/evidently/metrics/data_quality/text_descriptors_distribution.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.023777 evidently-0.3.2.1/src/evidently/metrics/regression_performance/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.045310 evidently-0.3.2.1/src/evidently/metrics/regression_performance/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6449 2023-05-19 15:16:08.558812 evidently-0.3.2.1/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py
--rw-r--r--   0 emelidral   (501) staff       (20)    28994 2023-05-19 15:16:08.558914 evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_bias_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3936 2023-04-11 11:50:44.045565 evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_distribution.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6093 2023-05-19 15:16:08.559044 evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_in_time.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7598 2023-05-19 15:16:08.559168 evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_normality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1675 2023-04-11 11:50:44.045735 evidently-0.3.2.1/src/evidently/metrics/regression_performance/objects.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7833 2023-05-19 15:16:08.559285 evidently-0.3.2.1/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6610 2023-05-19 15:16:08.559434 evidently-0.3.2.1/src/evidently/metrics/regression_performance/predicted_vs_actual.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8427 2023-04-11 11:50:44.045914 evidently-0.3.2.1/src/evidently/metrics/regression_performance/regression_dummy_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12823 2023-04-11 11:50:44.045990 evidently-0.3.2.1/src/evidently/metrics/regression_performance/regression_performance_metrics.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12845 2023-04-11 11:50:44.046056 evidently-0.3.2.1/src/evidently/metrics/regression_performance/regression_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13755 2023-05-19 15:16:08.559658 evidently-0.3.2.1/src/evidently/metrics/regression_performance/top_error.py
--rw-r--r--   0 emelidral   (501) staff       (20)      628 2023-04-11 11:50:44.046174 evidently-0.3.2.1/src/evidently/metrics/regression_performance/utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4630 2023-04-11 11:50:44.046235 evidently-0.3.2.1/src/evidently/metrics/regression_performance/visualization.py
--rw-r--r--   0 emelidral   (501) staff       (20)      847 2023-04-11 11:50:44.046284 evidently-0.3.2.1/src/evidently/metrics/utils.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.024350 evidently-0.3.2.1/src/evidently/model/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.046336 evidently-0.3.2.1/src/evidently/model/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      230 2023-04-11 11:50:44.046390 evidently-0.3.2.1/src/evidently/model/dashboard.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-04-11 11:50:44.046446 evidently-0.3.2.1/src/evidently/model/widget.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.024544 evidently-0.3.2.1/src/evidently/nbextension/
--rw-r--r--   0 emelidral   (501) staff       (20)      195 2023-04-11 11:50:44.047775 evidently-0.3.2.1/src/evidently/nbextension/__init__.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.025353 evidently-0.3.2.1/src/evidently/nbextension/static/
--rw-r--r--   0 emelidral   (501) staff       (20)      409 2023-04-11 11:50:44.047847 evidently-0.3.2.1/src/evidently/nbextension/static/extension.js
--rw-r--r--   0 emelidral   (501) staff       (20)  2586352 2023-04-11 11:50:44.055472 evidently-0.3.2.1/src/evidently/nbextension/static/index.js
--rw-r--r--   0 emelidral   (501) staff       (20)     2238 2023-04-11 11:50:44.055652 evidently-0.3.2.1/src/evidently/nbextension/static/index.js.LICENSE.txt
--rw-r--r--   0 emelidral   (501) staff       (20)    94648 2023-04-11 11:50:44.056026 evidently-0.3.2.1/src/evidently/nbextension/static/material-ui-icons.woff2
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.026717 evidently-0.3.2.1/src/evidently/options/
--rw-r--r--   0 emelidral   (501) staff       (20)      471 2023-04-27 10:27:02.408578 evidently-0.3.2.1/src/evidently/options/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      102 2023-05-19 15:16:08.559716 evidently-0.3.2.1/src/evidently/options/agg_data.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2770 2023-05-19 15:16:08.559823 evidently-0.3.2.1/src/evidently/options/base.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3357 2023-05-19 15:16:08.559935 evidently-0.3.2.1/src/evidently/options/color_scheme.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8204 2023-04-11 11:50:44.056254 evidently-0.3.2.1/src/evidently/options/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)       67 2023-04-27 10:27:02.409017 evidently-0.3.2.1/src/evidently/options/option.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1209 2023-04-11 11:50:44.056307 evidently-0.3.2.1/src/evidently/options/quality_metrics.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.027105 evidently-0.3.2.1/src/evidently/pipeline/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056358 evidently-0.3.2.1/src/evidently/pipeline/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1162 2023-04-27 10:27:02.409249 evidently-0.3.2.1/src/evidently/pipeline/column_mapping.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.028131 evidently-0.3.2.1/src/evidently/renderers/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056636 evidently-0.3.2.1/src/evidently/renderers/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3114 2023-04-11 11:50:44.056702 evidently-0.3.2.1/src/evidently/renderers/base_renderer.py
--rw-r--r--   0 emelidral   (501) staff       (20)    29101 2023-05-19 15:16:08.560226 evidently-0.3.2.1/src/evidently/renderers/html_widgets.py
--rw-r--r--   0 emelidral   (501) staff       (20)      733 2023-04-11 11:50:44.056873 evidently-0.3.2.1/src/evidently/renderers/notebook_utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1781 2023-04-11 11:50:44.056927 evidently-0.3.2.1/src/evidently/renderers/render_utils.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.028569 evidently-0.3.2.1/src/evidently/report/
--rw-r--r--   0 emelidral   (501) staff       (20)       27 2023-04-11 11:50:44.057001 evidently-0.3.2.1/src/evidently/report/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7413 2023-05-19 15:16:08.560356 evidently-0.3.2.1/src/evidently/report/report.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.029264 evidently-0.3.2.1/src/evidently/runner/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057130 evidently-0.3.2.1/src/evidently/runner/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2842 2023-04-11 11:50:44.057260 evidently-0.3.2.1/src/evidently/runner/loader.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2134 2023-04-11 11:50:44.057381 evidently-0.3.2.1/src/evidently/runner/runner.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.030003 evidently-0.3.2.1/src/evidently/suite/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057438 evidently-0.3.2.1/src/evidently/suite/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    14249 2023-05-19 15:16:08.560498 evidently-0.3.2.1/src/evidently/suite/base_suite.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1991 2023-04-11 11:50:44.057593 evidently-0.3.2.1/src/evidently/suite/execution_graph.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.030420 evidently-0.3.2.1/src/evidently/telemetry/
--rw-r--r--   0 emelidral   (501) staff       (20)       36 2023-04-11 11:50:44.057752 evidently-0.3.2.1/src/evidently/telemetry/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1007 2023-04-11 11:50:44.057808 evidently-0.3.2.1/src/evidently/telemetry/sender.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.032523 evidently-0.3.2.1/src/evidently/test_preset/
--rw-r--r--   0 emelidral   (501) staff       (20)      859 2023-04-11 11:50:44.057891 evidently-0.3.2.1/src/evidently/test_preset/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2707 2023-04-11 11:50:44.058127 evidently-0.3.2.1/src/evidently/test_preset/classification_binary.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1948 2023-04-11 11:50:44.058178 evidently-0.3.2.1/src/evidently/test_preset/classification_binary_topk.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2507 2023-04-11 11:50:44.058248 evidently-0.3.2.1/src/evidently/test_preset/classification_multiclass.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7352 2023-04-27 10:27:02.410133 evidently-0.3.2.1/src/evidently/test_preset/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.058356 evidently-0.3.2.1/src/evidently/test_preset/data_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1559 2023-04-11 11:50:44.058402 evidently-0.3.2.1/src/evidently/test_preset/data_stability.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6811 2023-04-27 10:27:02.410385 evidently-0.3.2.1/src/evidently/test_preset/no_target_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)      750 2023-04-11 11:50:44.058506 evidently-0.3.2.1/src/evidently/test_preset/regression.py
--rw-r--r--   0 emelidral   (501) staff       (20)      298 2023-04-11 11:50:44.058559 evidently-0.3.2.1/src/evidently/test_preset/test_preset.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.032945 evidently-0.3.2.1/src/evidently/test_suite/
--rw-r--r--   0 emelidral   (501) staff       (20)       34 2023-04-11 11:50:44.058625 evidently-0.3.2.1/src/evidently/test_suite/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8647 2023-05-19 15:16:08.560630 evidently-0.3.2.1/src/evidently/test_suite/test_suite.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.034615 evidently-0.3.2.1/src/evidently/tests/
--rw-r--r--   0 emelidral   (501) staff       (20)     4460 2023-04-27 10:27:02.410897 evidently-0.3.2.1/src/evidently/tests/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    11758 2023-04-11 11:50:44.058862 evidently-0.3.2.1/src/evidently/tests/base_test.py
--rw-r--r--   0 emelidral   (501) staff       (20)    22752 2023-04-11 11:50:44.059177 evidently-0.3.2.1/src/evidently/tests/classification_performance_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    21931 2023-05-19 15:16:08.560789 evidently-0.3.2.1/src/evidently/tests/data_drift_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    42332 2023-04-27 10:27:02.411682 evidently-0.3.2.1/src/evidently/tests/data_integrity_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    53681 2023-04-27 10:27:02.412175 evidently-0.3.2.1/src/evidently/tests/data_quality_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    10930 2023-04-11 11:50:44.059579 evidently-0.3.2.1/src/evidently/tests/regression_performance_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    16360 2023-04-11 11:50:44.059661 evidently-0.3.2.1/src/evidently/tests/utils.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.036582 evidently-0.3.2.1/src/evidently/utils/
--rw-r--r--   0 emelidral   (501) staff       (20)       40 2023-04-11 11:50:44.059731 evidently-0.3.2.1/src/evidently/utils/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5800 2023-04-11 11:50:44.059794 evidently-0.3.2.1/src/evidently/utils/dashboard.py
--rw-r--r--   0 emelidral   (501) staff       (20)     9086 2023-04-27 10:27:02.412473 evidently-0.3.2.1/src/evidently/utils/data_drift_utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8133 2023-04-11 11:50:44.059931 evidently-0.3.2.1/src/evidently/utils/data_operations.py
--rw-r--r--   0 emelidral   (501) staff       (20)    20996 2023-04-11 11:50:44.060030 evidently-0.3.2.1/src/evidently/utils/data_preprocessing.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4375 2023-04-11 11:50:44.060100 evidently-0.3.2.1/src/evidently/utils/generators.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1392 2023-04-24 17:06:50.391821 evidently-0.3.2.1/src/evidently/utils/numpy_encoder.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-04-11 11:50:44.060206 evidently-0.3.2.1/src/evidently/utils/types.py
--rw-r--r--   0 emelidral   (501) staff       (20)    35867 2023-05-19 15:16:08.561016 evidently-0.3.2.1/src/evidently/utils/visualizations.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.306076 evidently-0.3.3/
+-rw-r--r--   0 emelidral   (501) staff       (20)      373 2023-06-12 17:22:56.306188 evidently-0.3.3/PKG-INFO
+-rw-r--r--   0 emelidral   (501) staff       (20)     1468 2023-06-12 17:21:25.353948 evidently-0.3.3/setup.cfg
+-rw-r--r--   0 emelidral   (501) staff       (20)     2103 2023-05-19 15:16:08.556083 evidently-0.3.3/setup.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    22071 2023-04-11 11:50:44.033364 evidently-0.3.3/setupbase.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.264225 evidently-0.3.3/src/
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.268130 evidently-0.3.3/src/evidently/
+-rw-r--r--   0 emelidral   (501) staff       (20)      358 2023-06-09 20:16:27.247523 evidently-0.3.3/src/evidently/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1892 2023-04-27 10:27:02.402053 evidently-0.3.3/src/evidently/__main__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      162 2023-04-11 11:50:44.033618 evidently-0.3.3/src/evidently/_config.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      111 2023-06-12 17:22:20.682881 evidently-0.3.3/src/evidently/_version.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8632 2023-06-12 17:21:25.354070 evidently-0.3.3/src/evidently/base_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.269602 evidently-0.3.3/src/evidently/calculations/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.034605 evidently-0.3.3/src/evidently/calculations/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    14543 2023-04-11 11:50:44.034697 evidently-0.3.3/src/evidently/calculations/classification_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    17663 2023-06-12 17:21:25.354215 evidently-0.3.3/src/evidently/calculations/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2662 2023-04-11 11:50:44.034844 evidently-0.3.3/src/evidently/calculations/data_integration.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    33604 2023-06-12 17:21:25.354408 evidently-0.3.3/src/evidently/calculations/data_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8286 2023-04-11 11:50:44.035061 evidently-0.3.3/src/evidently/calculations/regression_performance.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.274668 evidently-0.3.3/src/evidently/calculations/stattests/
+-rw-r--r--   0 emelidral   (501) staff       (20)     1885 2023-06-09 20:16:27.248227 evidently-0.3.3/src/evidently/calculations/stattests/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1318 2023-06-09 20:16:27.248345 evidently-0.3.3/src/evidently/calculations/stattests/anderson_darling_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1741 2023-04-11 11:50:44.035280 evidently-0.3.3/src/evidently/calculations/stattests/chisquare_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7331 2023-04-27 10:27:02.403563 evidently-0.3.3/src/evidently/calculations/stattests/cramer_von_mises_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1533 2023-04-11 11:50:44.035446 evidently-0.3.3/src/evidently/calculations/stattests/energy_distance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2108 2023-04-11 11:50:44.035531 evidently-0.3.3/src/evidently/calculations/stattests/epps_singleton_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2592 2023-04-11 11:50:44.035581 evidently-0.3.3/src/evidently/calculations/stattests/fisher_exact_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2025 2023-04-11 11:50:44.035635 evidently-0.3.3/src/evidently/calculations/stattests/g_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2983 2023-04-11 11:50:44.035704 evidently-0.3.3/src/evidently/calculations/stattests/hellinger_distance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2152 2023-04-11 11:50:44.035768 evidently-0.3.3/src/evidently/calculations/stattests/jensenshannon.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1899 2023-04-11 11:50:44.035819 evidently-0.3.3/src/evidently/calculations/stattests/kl_div.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1545 2023-04-11 11:50:44.035878 evidently-0.3.3/src/evidently/calculations/stattests/ks_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1752 2023-05-19 15:16:08.556697 evidently-0.3.3/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4683 2023-04-11 11:50:44.036014 evidently-0.3.3/src/evidently/calculations/stattests/mmd_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1812 2023-04-11 11:50:44.036061 evidently-0.3.3/src/evidently/calculations/stattests/psi.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4696 2023-04-27 10:27:02.403868 evidently-0.3.3/src/evidently/calculations/stattests/registry.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1490 2023-04-11 11:50:44.036213 evidently-0.3.3/src/evidently/calculations/stattests/t_test.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      799 2023-04-27 10:27:02.404121 evidently-0.3.3/src/evidently/calculations/stattests/text_content_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      791 2023-04-27 10:27:02.404318 evidently-0.3.3/src/evidently/calculations/stattests/text_content_drift_abs.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2746 2023-04-11 11:50:44.036327 evidently-0.3.3/src/evidently/calculations/stattests/tvd_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4825 2023-04-11 11:50:44.036404 evidently-0.3.3/src/evidently/calculations/stattests/utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1832 2023-04-11 11:50:44.036454 evidently-0.3.3/src/evidently/calculations/stattests/wasserstein_distance_norm.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2878 2023-04-11 11:50:44.036512 evidently-0.3.3/src/evidently/calculations/stattests/z_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.036630 evidently-0.3.3/src/evidently/calculations/utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8150 2023-06-12 17:21:25.354522 evidently-0.3.3/src/evidently/core.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.276395 evidently-0.3.3/src/evidently/descriptors/
+-rw-r--r--   0 emelidral   (501) staff       (20)      554 2023-06-09 20:16:27.248619 evidently-0.3.3/src/evidently/descriptors/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      578 2023-04-11 11:50:44.040789 evidently-0.3.3/src/evidently/descriptors/non_letter_character_percentage_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      555 2023-06-12 17:21:25.354607 evidently-0.3.3/src/evidently/descriptors/oov_words_percentage_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      482 2023-06-09 20:16:27.248823 evidently-0.3.3/src/evidently/descriptors/sentence_count_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      455 2023-06-09 20:16:27.249089 evidently-0.3.3/src/evidently/descriptors/sentiment_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      464 2023-04-11 11:50:44.040888 evidently-0.3.3/src/evidently/descriptors/text_length_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      714 2023-06-12 17:21:25.354687 evidently-0.3.3/src/evidently/descriptors/trigger_words_presence_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      458 2023-06-09 20:16:27.249657 evidently-0.3.3/src/evidently/descriptors/word_count_descriptor.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.278279 evidently-0.3.3/src/evidently/features/
+-rw-r--r--   0 emelidral   (501) staff       (20)     1860 2023-06-12 17:21:25.354776 evidently-0.3.3/src/evidently/features/OOV_words_percentage_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.041037 evidently-0.3.3/src/evidently/features/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1990 2023-06-12 17:21:25.354860 evidently-0.3.3/src/evidently/features/generated_features.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1144 2023-06-12 17:21:25.354961 evidently-0.3.3/src/evidently/features/non_letter_character_percentage_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1149 2023-06-12 17:21:25.355342 evidently-0.3.3/src/evidently/features/sentence_count_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1154 2023-06-12 17:21:25.355563 evidently-0.3.3/src/evidently/features/sentiment_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1015 2023-06-12 17:21:25.355638 evidently-0.3.3/src/evidently/features/text_length_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2257 2023-06-12 17:21:25.355725 evidently-0.3.3/src/evidently/features/trigger_words_presence_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1065 2023-06-12 17:21:25.355806 evidently-0.3.3/src/evidently/features/word_count_feature.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.279864 evidently-0.3.3/src/evidently/metric_preset/
+-rw-r--r--   0 emelidral   (501) staff       (20)      496 2023-04-11 11:50:44.041350 evidently-0.3.3/src/evidently/metric_preset/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2526 2023-04-11 11:50:44.041407 evidently-0.3.3/src/evidently/metric_preset/classification_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4767 2023-06-09 20:16:27.250501 evidently-0.3.3/src/evidently/metric_preset/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1325 2023-04-11 11:50:44.041535 evidently-0.3.3/src/evidently/metric_preset/data_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      343 2023-04-11 11:50:44.041591 evidently-0.3.3/src/evidently/metric_preset/metric_preset.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1817 2023-04-11 11:50:44.041650 evidently-0.3.3/src/evidently/metric_preset/regression_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7282 2023-04-11 11:50:44.041719 evidently-0.3.3/src/evidently/metric_preset/target_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1811 2023-04-11 11:50:44.041776 evidently-0.3.3/src/evidently/metric_preset/text_overview.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    11037 2023-06-12 17:21:25.355924 evidently-0.3.3/src/evidently/metric_results.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.280467 evidently-0.3.3/src/evidently/metrics/
+-rw-r--r--   0 emelidral   (501) staff       (20)     5260 2023-06-09 20:16:27.250916 evidently-0.3.3/src/evidently/metrics/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      691 2023-04-11 11:50:44.042032 evidently-0.3.3/src/evidently/metrics/base_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.283381 evidently-0.3.3/src/evidently/metrics/classification_performance/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.042092 evidently-0.3.3/src/evidently/metrics/classification_performance/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3146 2023-06-12 17:21:25.356036 evidently-0.3.3/src/evidently/metrics/classification_performance/base_classification_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3132 2023-04-27 10:27:02.405129 evidently-0.3.3/src/evidently/metrics/classification_performance/class_balance_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6991 2023-06-12 17:21:25.356145 evidently-0.3.3/src/evidently/metrics/classification_performance/class_separation_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12128 2023-06-12 17:21:25.356265 evidently-0.3.3/src/evidently/metrics/classification_performance/classification_dummy_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5328 2023-06-12 17:21:25.356359 evidently-0.3.3/src/evidently/metrics/classification_performance/classification_quality_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3972 2023-06-12 17:21:25.356454 evidently-0.3.3/src/evidently/metrics/classification_performance/confusion_matrix_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1622 2023-06-12 17:21:25.356546 evidently-0.3.3/src/evidently/metrics/classification_performance/objects.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4464 2023-06-09 20:16:27.251441 evidently-0.3.3/src/evidently/metrics/classification_performance/pr_curve_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6379 2023-06-12 17:21:25.356651 evidently-0.3.3/src/evidently/metrics/classification_performance/pr_table_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5940 2023-06-09 20:16:27.251685 evidently-0.3.3/src/evidently/metrics/classification_performance/probability_distribution_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7480 2023-06-12 17:21:25.356752 evidently-0.3.3/src/evidently/metrics/classification_performance/quality_by_class_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    17143 2023-06-12 17:21:25.356933 evidently-0.3.3/src/evidently/metrics/classification_performance/quality_by_feature_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4406 2023-06-09 20:16:27.251920 evidently-0.3.3/src/evidently/metrics/classification_performance/roc_curve_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.285764 evidently-0.3.3/src/evidently/metrics/data_drift/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043120 evidently-0.3.3/src/evidently/metrics/data_drift/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1183 2023-06-12 17:21:25.357005 evidently-0.3.3/src/evidently/metrics/data_drift/base.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    18587 2023-06-12 17:21:25.357143 evidently-0.3.3/src/evidently/metrics/data_drift/column_drift_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    10039 2023-06-12 17:21:25.357269 evidently-0.3.3/src/evidently/metrics/data_drift/column_value_plot.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13980 2023-06-12 17:21:25.357382 evidently-0.3.3/src/evidently/metrics/data_drift/data_drift_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5440 2023-06-12 17:21:25.357473 evidently-0.3.3/src/evidently/metrics/data_drift/dataset_drift_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    10729 2023-04-27 10:27:02.406479 evidently-0.3.3/src/evidently/metrics/data_drift/embedding_drift_methods.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4633 2023-06-12 17:21:25.357563 evidently-0.3.3/src/evidently/metrics/data_drift/embeddings_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13752 2023-06-12 17:21:25.357734 evidently-0.3.3/src/evidently/metrics/data_drift/target_by_features_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    11468 2023-06-12 17:21:25.357882 evidently-0.3.3/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    11289 2023-06-12 17:21:25.358002 evidently-0.3.3/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1136 2023-06-12 17:21:25.358098 evidently-0.3.3/src/evidently/metrics/data_drift/text_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.286992 evidently-0.3.3/src/evidently/metrics/data_integrity/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043904 evidently-0.3.3/src/evidently/metrics/data_integrity/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8586 2023-06-12 17:21:25.358216 evidently-0.3.3/src/evidently/metrics/data_integrity/column_missing_values_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7258 2023-06-12 17:21:25.358337 evidently-0.3.3/src/evidently/metrics/data_integrity/column_regexp_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    28143 2023-06-12 17:21:25.358497 evidently-0.3.3/src/evidently/metrics/data_integrity/column_summary_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13061 2023-06-12 17:21:25.358652 evidently-0.3.3/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     9781 2023-06-12 17:21:25.358766 evidently-0.3.3/src/evidently/metrics/data_integrity/dataset_summary_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.289434 evidently-0.3.3/src/evidently/metrics/data_quality/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.044472 evidently-0.3.3/src/evidently/metrics/data_quality/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5824 2023-06-12 17:21:25.358882 evidently-0.3.3/src/evidently/metrics/data_quality/column_correlations_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3163 2023-06-12 17:21:25.358982 evidently-0.3.3/src/evidently/metrics/data_quality/column_distribution_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6088 2023-06-12 17:21:25.359083 evidently-0.3.3/src/evidently/metrics/data_quality/column_quantile_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6988 2023-06-12 17:21:25.359187 evidently-0.3.3/src/evidently/metrics/data_quality/column_value_list_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     9194 2023-06-12 17:21:25.359296 evidently-0.3.3/src/evidently/metrics/data_quality/column_value_range_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4336 2023-04-11 11:50:44.044913 evidently-0.3.3/src/evidently/metrics/data_quality/conflict_prediction_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3927 2023-04-11 11:50:44.044975 evidently-0.3.3/src/evidently/metrics/data_quality/conflict_target_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    14033 2023-06-12 17:21:25.359428 evidently-0.3.3/src/evidently/metrics/data_quality/dataset_correlations_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2820 2023-06-12 17:21:25.359518 evidently-0.3.3/src/evidently/metrics/data_quality/stability_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7526 2023-06-12 17:21:25.359639 evidently-0.3.3/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5493 2023-06-12 17:21:25.359724 evidently-0.3.3/src/evidently/metrics/data_quality/text_descriptors_distribution.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.292490 evidently-0.3.3/src/evidently/metrics/regression_performance/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.045310 evidently-0.3.3/src/evidently/metrics/regression_performance/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6625 2023-06-12 17:21:25.359835 evidently-0.3.3/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    29078 2023-06-12 17:21:25.359923 evidently-0.3.3/src/evidently/metrics/regression_performance/error_bias_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3897 2023-06-09 20:16:27.254075 evidently-0.3.3/src/evidently/metrics/regression_performance/error_distribution.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6273 2023-06-12 17:21:25.360026 evidently-0.3.3/src/evidently/metrics/regression_performance/error_in_time.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7573 2023-06-09 20:16:27.254274 evidently-0.3.3/src/evidently/metrics/regression_performance/error_normality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2371 2023-06-12 17:21:25.360111 evidently-0.3.3/src/evidently/metrics/regression_performance/objects.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7892 2023-06-12 17:21:25.360199 evidently-0.3.3/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6610 2023-05-19 15:16:08.559434 evidently-0.3.3/src/evidently/metrics/regression_performance/predicted_vs_actual.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8607 2023-06-12 17:21:25.360292 evidently-0.3.3/src/evidently/metrics/regression_performance/regression_dummy_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12778 2023-06-09 20:16:27.254711 evidently-0.3.3/src/evidently/metrics/regression_performance/regression_performance_metrics.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12781 2023-06-09 20:16:27.254860 evidently-0.3.3/src/evidently/metrics/regression_performance/regression_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13755 2023-05-19 15:16:08.559658 evidently-0.3.3/src/evidently/metrics/regression_performance/top_error.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      845 2023-06-12 17:21:25.360379 evidently-0.3.3/src/evidently/metrics/regression_performance/utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4474 2023-06-12 17:21:25.360533 evidently-0.3.3/src/evidently/metrics/regression_performance/visualization.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      847 2023-04-11 11:50:44.046284 evidently-0.3.3/src/evidently/metrics/utils.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.293076 evidently-0.3.3/src/evidently/model/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.046336 evidently-0.3.3/src/evidently/model/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      230 2023-04-11 11:50:44.046390 evidently-0.3.3/src/evidently/model/dashboard.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-04-11 11:50:44.046446 evidently-0.3.3/src/evidently/model/widget.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.293287 evidently-0.3.3/src/evidently/nbextension/
+-rw-r--r--   0 emelidral   (501) staff       (20)      195 2023-04-11 11:50:44.047775 evidently-0.3.3/src/evidently/nbextension/__init__.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.294122 evidently-0.3.3/src/evidently/nbextension/static/
+-rw-r--r--   0 emelidral   (501) staff       (20)      409 2023-04-11 11:50:44.047847 evidently-0.3.3/src/evidently/nbextension/static/extension.js
+-rw-r--r--   0 emelidral   (501) staff       (20)  2586352 2023-04-11 11:50:44.055472 evidently-0.3.3/src/evidently/nbextension/static/index.js
+-rw-r--r--   0 emelidral   (501) staff       (20)     2238 2023-04-11 11:50:44.055652 evidently-0.3.3/src/evidently/nbextension/static/index.js.LICENSE.txt
+-rw-r--r--   0 emelidral   (501) staff       (20)    94648 2023-04-11 11:50:44.056026 evidently-0.3.3/src/evidently/nbextension/static/material-ui-icons.woff2
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.295665 evidently-0.3.3/src/evidently/options/
+-rw-r--r--   0 emelidral   (501) staff       (20)      561 2023-06-09 20:16:27.255084 evidently-0.3.3/src/evidently/options/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      102 2023-05-19 15:16:08.559716 evidently-0.3.3/src/evidently/options/agg_data.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2770 2023-05-19 15:16:08.559823 evidently-0.3.3/src/evidently/options/base.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3357 2023-05-19 15:16:08.559935 evidently-0.3.3/src/evidently/options/color_scheme.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8261 2023-06-12 17:21:25.360633 evidently-0.3.3/src/evidently/options/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)       95 2023-06-12 17:21:25.360707 evidently-0.3.3/src/evidently/options/option.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1209 2023-04-11 11:50:44.056307 evidently-0.3.3/src/evidently/options/quality_metrics.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.296112 evidently-0.3.3/src/evidently/pipeline/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056358 evidently-0.3.3/src/evidently/pipeline/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1162 2023-04-27 10:27:02.409249 evidently-0.3.3/src/evidently/pipeline/column_mapping.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4124 2023-06-12 17:21:25.360769 evidently-0.3.3/src/evidently/pydantic_utils.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.297128 evidently-0.3.3/src/evidently/renderers/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056636 evidently-0.3.3/src/evidently/renderers/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3114 2023-04-11 11:50:44.056702 evidently-0.3.3/src/evidently/renderers/base_renderer.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    29436 2023-06-09 20:16:27.255267 evidently-0.3.3/src/evidently/renderers/html_widgets.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      733 2023-04-11 11:50:44.056873 evidently-0.3.3/src/evidently/renderers/notebook_utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1781 2023-04-11 11:50:44.056927 evidently-0.3.3/src/evidently/renderers/render_utils.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.297540 evidently-0.3.3/src/evidently/report/
+-rw-r--r--   0 emelidral   (501) staff       (20)       49 2023-06-09 20:16:27.255377 evidently-0.3.3/src/evidently/report/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8403 2023-06-12 17:21:25.360891 evidently-0.3.3/src/evidently/report/report.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.298189 evidently-0.3.3/src/evidently/runner/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057130 evidently-0.3.3/src/evidently/runner/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2842 2023-04-11 11:50:44.057260 evidently-0.3.3/src/evidently/runner/loader.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2134 2023-04-11 11:50:44.057381 evidently-0.3.3/src/evidently/runner/runner.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.298799 evidently-0.3.3/src/evidently/suite/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057438 evidently-0.3.3/src/evidently/suite/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    16447 2023-06-12 17:21:25.361036 evidently-0.3.3/src/evidently/suite/base_suite.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1991 2023-04-11 11:50:44.057593 evidently-0.3.3/src/evidently/suite/execution_graph.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.299223 evidently-0.3.3/src/evidently/telemetry/
+-rw-r--r--   0 emelidral   (501) staff       (20)       67 2023-06-09 20:16:27.255610 evidently-0.3.3/src/evidently/telemetry/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1007 2023-04-11 11:50:44.057808 evidently-0.3.3/src/evidently/telemetry/sender.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.301259 evidently-0.3.3/src/evidently/test_preset/
+-rw-r--r--   0 emelidral   (501) staff       (20)      859 2023-04-11 11:50:44.057891 evidently-0.3.3/src/evidently/test_preset/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2707 2023-04-11 11:50:44.058127 evidently-0.3.3/src/evidently/test_preset/classification_binary.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1948 2023-04-11 11:50:44.058178 evidently-0.3.3/src/evidently/test_preset/classification_binary_topk.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2507 2023-04-11 11:50:44.058248 evidently-0.3.3/src/evidently/test_preset/classification_multiclass.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7352 2023-04-27 10:27:02.410133 evidently-0.3.3/src/evidently/test_preset/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.058356 evidently-0.3.3/src/evidently/test_preset/data_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1559 2023-04-11 11:50:44.058402 evidently-0.3.3/src/evidently/test_preset/data_stability.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6811 2023-04-27 10:27:02.410385 evidently-0.3.3/src/evidently/test_preset/no_target_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      750 2023-04-11 11:50:44.058506 evidently-0.3.3/src/evidently/test_preset/regression.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      298 2023-04-11 11:50:44.058559 evidently-0.3.3/src/evidently/test_preset/test_preset.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.301667 evidently-0.3.3/src/evidently/test_suite/
+-rw-r--r--   0 emelidral   (501) staff       (20)       59 2023-06-09 20:16:27.255703 evidently-0.3.3/src/evidently/test_suite/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     9272 2023-06-12 17:21:25.361173 evidently-0.3.3/src/evidently/test_suite/test_suite.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.303430 evidently-0.3.3/src/evidently/tests/
+-rw-r--r--   0 emelidral   (501) staff       (20)     6685 2023-06-09 20:16:27.255932 evidently-0.3.3/src/evidently/tests/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    11718 2023-06-12 17:21:25.361299 evidently-0.3.3/src/evidently/tests/base_test.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    23432 2023-06-12 17:21:25.361430 evidently-0.3.3/src/evidently/tests/classification_performance_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    22404 2023-06-12 17:21:25.361568 evidently-0.3.3/src/evidently/tests/data_drift_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    42741 2023-06-12 17:21:25.361751 evidently-0.3.3/src/evidently/tests/data_integrity_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    54223 2023-06-12 17:21:25.361969 evidently-0.3.3/src/evidently/tests/data_quality_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    11174 2023-06-12 17:21:25.362090 evidently-0.3.3/src/evidently/tests/regression_performance_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    16330 2023-06-12 17:21:25.362201 evidently-0.3.3/src/evidently/tests/utils.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.305548 evidently-0.3.3/src/evidently/utils/
+-rw-r--r--   0 emelidral   (501) staff       (20)       68 2023-06-09 20:16:27.256199 evidently-0.3.3/src/evidently/utils/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5800 2023-04-11 11:50:44.059794 evidently-0.3.3/src/evidently/utils/dashboard.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     9086 2023-04-27 10:27:02.412473 evidently-0.3.3/src/evidently/utils/data_drift_utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8133 2023-04-11 11:50:44.059931 evidently-0.3.3/src/evidently/utils/data_operations.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    20996 2023-04-11 11:50:44.060030 evidently-0.3.3/src/evidently/utils/data_preprocessing.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4375 2023-04-11 11:50:44.060100 evidently-0.3.3/src/evidently/utils/generators.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1460 2023-06-12 17:21:25.362290 evidently-0.3.3/src/evidently/utils/numpy_encoder.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2075 2023-06-12 17:21:25.362374 evidently-0.3.3/src/evidently/utils/types.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    36113 2023-06-12 17:21:25.362546 evidently-0.3.3/src/evidently/utils/visualizations.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-06-12 17:22:56.306034 evidently-0.3.3/tests/
+-rw-r--r--   0 emelidral   (501) staff       (20)     5872 2023-04-11 11:50:44.068461 evidently-0.3.3/tests/test_metric_results.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2538 2023-04-11 11:50:44.069079 evidently-0.3.3/tests/test_utils.py
```

### Comparing `evidently-0.3.2.1/setup.cfg` & `evidently-0.3.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,26 @@
     =src
 
 [options.packages.find]
 where = src
 
 
 [flake8]
-ignore = E501,F401,W503,W504,E203
+ignore = E501,W503,W504,E203
 max-line-length = 140
 per-file-ignores =
      src/evidently/tabs/__init__.py: F403
      src/evidently/profile_sections/__init__.py: F403
      src/evidently/widgets/__init__.py: F403
 
 [mypy]
 show_error_codes = True
 files = src/evidently
 python_version = 3.7
+disable_error_code = misc
 
 [mypy-nltk.*]
 ignore_missing_imports = True
 
 [mypy-pandas.*]
 ignore_missing_imports = True
```

### Comparing `evidently-0.3.2.1/setup.py` & `evidently-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/setupbase.py` & `evidently-0.3.3/setupbase.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/__main__.py` & `evidently-0.3.3/src/evidently/__main__.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/base_metric.py` & `evidently-0.3.3/src/evidently/base_metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,57 +10,71 @@
 from typing import TypeVar
 from typing import Union
 
 import pandas as pd
 
 from evidently.core import BaseResult
 from evidently.core import ColumnType
+from evidently.core import IncludeTags
 from evidently.features.generated_features import GeneratedFeature
 from evidently.options.base import AnyOptions
 from evidently.options.base import Options
 from evidently.pipeline.column_mapping import ColumnMapping
+from evidently.pydantic_utils import EnumValueMixin
+from evidently.pydantic_utils import EvidentlyBaseModel
+from evidently.pydantic_utils import PolymorphicModel
+from evidently.pydantic_utils import WithTestAndMetricDependencies
 from evidently.utils.data_preprocessing import DataDefinition
 
 if TYPE_CHECKING:
     from evidently.suite.base_suite import Context
 
 
-class MetricResult(BaseResult):
-    pass
+class MetricResult(PolymorphicModel, BaseResult):  # type: ignore[misc] # pydantic Config
+    class Config:
+        field_tags = {"type": {IncludeTags.TypeField}}
 
 
 class ErrorResult:
     exception: BaseException
 
     def __init__(self, exception: BaseException):
         self.exception = exception
 
 
 class DatasetType(Enum):
     MAIN = "main"
     ADDITIONAL = "additional"
 
 
-@dataclass(eq=True, unsafe_hash=True)
-class ColumnName:
+class ColumnName(EnumValueMixin, EvidentlyBaseModel):
     name: str
     display_name: str
     dataset: DatasetType
     feature_class: Optional[GeneratedFeature]
 
+    def __init__(
+        self, name: str, display_name: str, dataset: DatasetType, feature_class: Optional[GeneratedFeature] = None
+    ):
+        super().__init__(name=name, display_name=display_name, dataset=dataset, feature_class=feature_class)
+
     def is_main_dataset(self):
         return self.dataset == DatasetType.MAIN
 
     @staticmethod
     def main_dataset(name: str):
         return ColumnName(name, name, DatasetType.MAIN, None)
 
     def __str__(self):
         return self.display_name
 
+    @classmethod
+    def from_any(cls, column_name: Union[str, "ColumnName"]):
+        return column_name if not isinstance(column_name, str) else ColumnName.main_dataset(column_name)
+
 
 def additional_feature(feature: GeneratedFeature, feature_name: str, display_name: str) -> ColumnName:
     return ColumnName(
         name=feature.__class__.__name__ + "." + feature_name,
         display_name=display_name,
         dataset=DatasetType.ADDITIONAL,
         feature_class=feature,
@@ -135,49 +149,51 @@
             _column = column
         return _column
 
 
 TResult = TypeVar("TResult", bound=MetricResult)
 
 
-class Metric(Generic[TResult]):
-    context: Optional["Context"] = None
+class Metric(WithTestAndMetricDependencies, Generic[TResult]):
+    _context: Optional["Context"] = None
 
     # TODO: if we want metric-specific options
     options: Options
+
     # resulting options will be determined via
     # options = global_option.override(display_options).override(metric_options)
 
-    def __init__(self, options: AnyOptions = None):
+    def __init__(self, options: AnyOptions = None, **data):
         self.options = Options.from_any_options(options)
+        super().__init__(**data)
 
     def get_id(self) -> str:
         return self.__class__.__name__
 
     @abc.abstractmethod
     def calculate(self, data: InputData) -> TResult:
         raise NotImplementedError()
 
     def set_context(self, context):
-        self.context = context
+        self._context = context
 
     def get_result(self) -> TResult:
-        if self.context is None:
+        if not hasattr(self, "_context") or self._context is None:
             raise ValueError("No context is set")
-        result = self.context.metric_results.get(self, None)
+        result = self._context.metric_results.get(self, None)
         if isinstance(result, ErrorResult):
             raise result.exception
         if result is None:
             raise ValueError(f"No result found for metric {self} of type {type(self).__name__}")
         return result  # type: ignore[return-value]
 
     def get_parameters(self) -> Optional[tuple]:
         attributes = []
         for field, value in sorted(self.__dict__.items(), key=lambda x: x[0]):
-            if field in ["context"]:
+            if field in ["_context"]:
                 continue
             if isinstance(value, list):
                 attributes.append(tuple(value))
             else:
                 attributes.append(value)
         params = tuple(attributes)
         try:
@@ -194,16 +210,16 @@
                 continue
             if issubclass(type(value), ColumnName) and value.feature_class is not None:
                 required_features.append(value.feature_class)
         return required_features
 
     def get_options(self):
         options = self.options if hasattr(self, "options") else Options()
-        if self.context is not None:
-            options = self.context.options.override(options)
+        if self._context is not None:
+            options = self._context.options.override(options)
         return options
 
 
 class ColumnMetricResult(MetricResult):
     column_name: str
     # todo: use enum
     column_type: str
@@ -212,8 +228,12 @@
         return pd.DataFrame.from_dict({self.column_name: self.collect_pandas_columns()}, orient="index")
 
 
 ColumnTResult = TypeVar("ColumnTResult", bound=ColumnMetricResult)
 
 
 class ColumnMetric(Metric, Generic[ColumnTResult], abc.ABC):
-    column_name: str
+    column_name: ColumnName
+
+    def __init__(self, column_name: Union[ColumnName, str], options: AnyOptions = None):
+        self.column_name = ColumnName.from_any(column_name)
+        super().__init__(options)
```

### Comparing `evidently-0.3.2.1/src/evidently/calculations/classification_performance.py` & `evidently-0.3.3/src/evidently/calculations/classification_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/data_drift.py` & `evidently-0.3.3/src/evidently/calculations/data_drift.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 from evidently.base_metric import MetricResult
 from evidently.calculations.stattests import get_stattest
 from evidently.core import ColumnType
 from evidently.core import IncludeTags
 from evidently.metric_results import DatasetColumns
 from evidently.metric_results import Distribution
 from evidently.metric_results import DistributionIncluded
+from evidently.metric_results import ScatterAggField
 from evidently.metric_results import ScatterField
+from evidently.metric_results import raw_agg_properties
 from evidently.options import DataDriftOptions
 from evidently.utils.data_drift_utils import get_text_data_for_plots
 from evidently.utils.data_operations import recognize_column_type_
 from evidently.utils.types import Numeric
 from evidently.utils.visualizations import get_distribution_for_column
 from evidently.utils.visualizations import prepare_df_for_time_index_plot
 
@@ -30,34 +32,44 @@
 Words = List[str]
 
 
 class DriftStatsField(MetricResult):
     class Config:
         dict_exclude_fields = {"characteristic_examples", "characteristic_words", "correlations"}
         # todo: after tests PR
-        field_tags = {k: {IncludeTags.Render} for k in dict_exclude_fields}
+        field_tags = {
+            "characteristic_examples": {IncludeTags.Render},
+            "characteristic_words": {IncludeTags.Render},
+            "correlations": {IncludeTags.Render},
+            "type": {IncludeTags.TypeField},
+        }
         pd_include = False
 
     distribution: Optional[Distribution]
     characteristic_examples: Optional[Examples]
     characteristic_words: Optional[Words]
     small_distribution: Optional[DistributionIncluded]
     correlations: Optional[Dict[str, float]]
 
 
 class ColumnDataDriftMetrics(ColumnMetricResult):
+    class Config:
+        # todo: change to field_tags: render
+        dict_exclude_fields = {"scatter"}
+
     stattest_name: str
     stattest_threshold: Optional[float]
     drift_score: Numeric
     drift_detected: bool
 
     current: DriftStatsField
     reference: DriftStatsField
 
-    scatter: Optional[ScatterField]
+    scatter: Optional[Union[ScatterField, ScatterAggField]]
+    scatter_raw, scatter_agg = raw_agg_properties("scatter", ScatterField, ScatterAggField, True)
 
 
 @dataclass
 class DatasetDrift:
     """Dataset drift calculation results"""
 
     number_of_drifted_columns: int
@@ -148,15 +160,15 @@
 
         if not pd.api.types.is_numeric_dtype(current_column):
             raise ValueError(f"Column '{column_name}' in current dataset should contain numerical values only.")
 
     drift_test_function = get_stattest(reference_column, current_column, column_type.value, stattest)
     drift_result = drift_test_function(reference_column, current_column, column_type.value, threshold)
 
-    scatter: Optional[ScatterField] = None
+    scatter: Optional[Union[ScatterField, ScatterAggField]] = None
     if column_type == ColumnType.Numerical:
         numeric_columns = dataset_columns.num_feature_names
 
         if column_name not in numeric_columns:
             # for target and prediction cases add the column_name in the numeric columns list
             numeric_columns = numeric_columns + [column_name]
 
@@ -198,22 +210,31 @@
                 column_name,
                 datetime_column_name,
             )
             current_scatter["current"] = df
             if prefix is None:
                 x_name = "Index binned"
             else:
-                x_name = f"{datetime_column_name} ({prefix})"
+                if datetime_column_name is not None:
+                    name = datetime_column_name
+                elif curr_data.index.name is not None:
+                    name = curr_data.index.name
+                else:
+                    name = "Index"
+                x_name = f"{name} ({prefix})"
 
         plot_shape = {}
         reference_mean = reference_data[column_name].mean()
         reference_std = reference_data[column_name].std()
         plot_shape["y0"] = reference_mean - reference_std
         plot_shape["y1"] = reference_mean + reference_std
-        scatter = ScatterField(scatter=current_scatter, x_name=x_name, plot_shape=plot_shape)
+        if agg_data:
+            scatter = ScatterAggField(scatter=current_scatter, x_name=x_name, plot_shape=plot_shape)
+        else:
+            scatter = ScatterField(scatter=current_scatter, x_name=x_name, plot_shape=plot_shape)
 
     elif column_type == ColumnType.Categorical:
         reference_counts = reference_data[column_name].value_counts(sort=False)
         current_counts = current_data[column_name].value_counts(sort=False)
         keys = set(reference_counts.keys()).union(set(current_counts.keys()))
 
         for key in keys:
```

### Comparing `evidently-0.3.2.1/src/evidently/calculations/data_integration.py` & `evidently-0.3.3/src/evidently/calculations/data_integration.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/data_quality.py` & `evidently-0.3.3/src/evidently/calculations/data_quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from evidently.metric_results import DatasetColumns
 from evidently.metric_results import Distribution
 from evidently.metric_results import Histogram
 from evidently.metric_results import HistogramData
 from evidently.utils.data_preprocessing import DataDefinition
 from evidently.utils.types import ColumnDistribution
 from evidently.utils.visualizations import get_gaussian_kde
+from evidently.utils.visualizations import is_possible_contour
 from evidently.utils.visualizations import make_hist_for_cat_plot
 from evidently.utils.visualizations import make_hist_for_num_plot
 
 MAX_CATEGORIES = 5
 
 
 def get_rows_count(data: Union[pd.DataFrame, pd.Series]) -> int:
@@ -592,31 +593,39 @@
         if column_type == ColumnType.Numerical and target_type == ColumnType.Categorical:
             data_by_target = {
                 "data_for_plots": _prepare_box_data(curr_df, ref_df, target_name, column_name),
                 "target_name": target_name,
                 "target_type": target_type.value,
             }
         if column_type == ColumnType.Numerical and target_type == ColumnType.Numerical:
-            if not agg_data:
+            if (
+                not agg_data
+                or not is_possible_contour(target_current.loc[current_data.index], current_data)
+                or (
+                    reference_data is not None
+                    and target_reference is not None
+                    and not is_possible_contour(target_reference.loc[reference_data.index], reference_data)
+                )
+            ):
                 result = {
                     "current": {
                         column_name: current_data.tolist(),
                         target_name: target_current.tolist(),
                     }
                 }
                 if reference_data is not None and target_reference is not None:
                     result["reference"] = {
                         column_name: reference_data.tolist(),
                         target_name: target_reference.tolist(),
                     }
 
             else:
-                result = {"current": get_gaussian_kde(target_current, current_data)}
+                result = {"current": get_gaussian_kde(target_current.loc[current_data.index], current_data)}
                 if reference_data is not None and target_reference is not None:
-                    result["reference"] = get_gaussian_kde(target_reference, reference_data)
+                    result["reference"] = get_gaussian_kde(target_reference.loc[reference_data.index], reference_data)
 
             data_by_target = {
                 "data_for_plots": result,
                 "target_name": target_name,
                 "target_type": target_type.value,
             }
 
@@ -801,15 +810,19 @@
 
     for kind in ["pearson", "spearman", "kendall"]:
         correlations_columns = []
         correlations_values = []
 
         for other_column_name in features.columns:
             correlations_columns.append(other_column_name)
-            correlations_values.append(column.corr(features[other_column_name], method=kind))
+            correlations_values.append(
+                column.replace([np.inf, -np.inf], np.nan).corr(
+                    features[other_column_name].replace([np.inf, -np.inf], np.nan), method=kind
+                )
+            )
 
         result.append(
             ColumnCorrelations(
                 column_name=column_display_name,
                 kind=kind,
                 values=Distribution(x=correlations_columns, y=correlations_values),
             )
```

### Comparing `evidently-0.3.2.1/src/evidently/calculations/regression_performance.py` & `evidently-0.3.3/src/evidently/calculations/regression_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/anderson_darling_stattest.py` & `evidently-0.3.3/src/evidently/calculations/stattests/anderson_darling_stattest.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     Using by name:
 
     >>> from evidently.options import DataDriftOptions
     >>> options = DataDriftOptions(all_features_stattest="anderson")
 """
 from typing import Tuple
 
-import numpy as np
 import pandas as pd
 from scipy.stats import anderson_ksamp
 
 from evidently.calculations.stattests.registry import StatTest
 from evidently.calculations.stattests.registry import register_stattest
```

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/chisquare_stattest.py` & `evidently-0.3.3/src/evidently/calculations/stattests/chisquare_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/cramer_von_mises_stattest.py` & `evidently-0.3.3/src/evidently/calculations/stattests/cramer_von_mises_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/energy_distance.py` & `evidently-0.3.3/src/evidently/calculations/stattests/energy_distance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/epps_singleton_stattest.py` & `evidently-0.3.3/src/evidently/calculations/stattests/epps_singleton_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/fisher_exact_stattest.py` & `evidently-0.3.3/src/evidently/calculations/stattests/fisher_exact_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/g_stattest.py` & `evidently-0.3.3/src/evidently/calculations/stattests/g_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/hellinger_distance.py` & `evidently-0.3.3/src/evidently/calculations/stattests/hellinger_distance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/jensenshannon.py` & `evidently-0.3.3/src/evidently/calculations/stattests/jensenshannon.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/kl_div.py` & `evidently-0.3.3/src/evidently/calculations/stattests/kl_div.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/ks_stattest.py` & `evidently-0.3.3/src/evidently/calculations/stattests/ks_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py` & `evidently-0.3.3/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/mmd_stattest.py` & `evidently-0.3.3/src/evidently/calculations/stattests/mmd_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/psi.py` & `evidently-0.3.3/src/evidently/calculations/stattests/psi.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/registry.py` & `evidently-0.3.3/src/evidently/calculations/stattests/registry.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/t_test.py` & `evidently-0.3.3/src/evidently/calculations/stattests/t_test.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/text_content_drift.py` & `evidently-0.3.3/src/evidently/calculations/stattests/text_content_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/text_content_drift_abs.py` & `evidently-0.3.3/src/evidently/calculations/stattests/text_content_drift_abs.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/tvd_stattest.py` & `evidently-0.3.3/src/evidently/calculations/stattests/tvd_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/utils.py` & `evidently-0.3.3/src/evidently/calculations/stattests/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/wasserstein_distance_norm.py` & `evidently-0.3.3/src/evidently/calculations/stattests/wasserstein_distance_norm.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/stattests/z_stattest.py` & `evidently-0.3.3/src/evidently/calculations/stattests/z_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/calculations/utils.py` & `evidently-0.3.3/src/evidently/calculations/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/core.py` & `evidently-0.3.3/src/evidently/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import ClassVar
 from typing import Dict
 from typing import Optional
 from typing import Set
 from typing import Type
 from typing import Union
 
+import numpy as np
 import pandas as pd
 from pydantic.fields import SHAPE_DICT
 from pydantic.fields import SHAPE_LIST
 from pydantic.fields import SHAPE_SET
 from pydantic.fields import SHAPE_TUPLE
 from pydantic.fields import ModelField
 
@@ -60,14 +61,56 @@
 
     def __bool__(self):
         return True
 
 
 class IncludeTags(Enum):
     Render = "render"
+    TypeField = "type_field"
+
+
+def pydantic_type_validator(type_: Type[Any]):
+    def decorator(f):
+        from pydantic.validators import _VALIDATORS
+
+        for cls, validators in _VALIDATORS:
+            if cls is type_:
+                validators.append(f)
+                return
+
+        _VALIDATORS.append(
+            (type_, [f]),
+        )
+
+    return decorator
+
+
+@pydantic_type_validator(pd.Series)
+def series_validator(value):
+    return pd.Series(value)
+
+
+@pydantic_type_validator(pd.DataFrame)
+def dataframe_validator(value):
+    return pd.DataFrame(value)
+
+
+# @pydantic_type_validator(pd.Index)
+# def index_validator(value):
+#     return pd.Index(value)
+
+
+@pydantic_type_validator(np.float_)
+def np_inf_valudator(value):
+    return np.float(value)
+
+
+@pydantic_type_validator(np.ndarray)
+def np_array_valudator(value):
+    return np.array(value)
 
 
 class BaseResult(BaseModel):
     class Config(BaseConfig):
         arbitrary_types_allowed = True
         dict_include: bool = True
         pd_include: bool = True
@@ -75,14 +118,15 @@
 
         dict_include_fields: set = set()
         dict_exclude_fields: set = set()
         pd_include_fields: set = set()
         pd_exclude_fields: set = set()
 
         tags: Set[IncludeTags] = set()
+        field_tags: Dict[str, set] = {}
 
     if TYPE_CHECKING:
         __config__: ClassVar[Type[Config]] = Config
 
     def get_dict(
         self,
         include_render: bool = False,
@@ -108,16 +152,19 @@
         include = include or {}
         dict_include_fields = (
             set(() if isinstance(include, bool) else include)
             or self.__config__.dict_include_fields
             or set(self.__fields__.keys())
         )
         dict_exclude_fields = self.__config__.dict_exclude_fields or set()
+        field_tags = self.__config__.field_tags or {}
         result: Dict[str, Any] = {}
         for name, field in self.__fields__.items():
+            if field_tags.get(name) and all(tag not in include_tags for tag in field_tags.get(name, set())):
+                continue
             if isinstance(field.type_, type) and issubclass(field.type_, BaseResult):
                 if (
                     (not field.type_.__config__.dict_include or name in dict_exclude_fields)
                     and not field.field_info.include
                     and name not in include
                     and all(tag not in include_tags for tag in field.type_.__config__.tags)
                 ):
```

### Comparing `evidently-0.3.2.1/src/evidently/descriptors/non_letter_character_percentage_descriptor.py` & `evidently-0.3.3/src/evidently/descriptors/non_letter_character_percentage_descriptor.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/descriptors/oov_words_percentage_descriptor.py` & `evidently-0.3.3/src/evidently/descriptors/oov_words_percentage_descriptor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from typing import Tuple
+
 from evidently.features.generated_features import FeatureDescriptor
 from evidently.features.generated_features import GeneratedFeature
 from evidently.features.OOV_words_percentage_feature import OOVWordsPercentage
 
 
 class OOV(FeatureDescriptor):
+    ignore_words: Tuple = ()
+
     def feature(self, column_name: str) -> GeneratedFeature:
         return OOVWordsPercentage(column_name, self.ignore_words)
 
-    def __init__(self, ignore_words=()):
-        self.ignore_words = ignore_words
-
     def for_column(self, column_name: str):
         return OOVWordsPercentage(column_name, self.ignore_words).feature_name()
```

### Comparing `evidently-0.3.2.1/src/evidently/features/OOV_words_percentage_feature.py` & `evidently-0.3.3/src/evidently/features/OOV_words_percentage_feature.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 import re
 from typing import Optional
+from typing import Set
+from typing import Tuple
 
 import pandas as pd
 from nltk.corpus import words
 from nltk.stem.wordnet import WordNetLemmatizer
 
 from evidently.base_metric import additional_feature
 from evidently.features.generated_features import GeneratedFeature
 from evidently.utils.data_preprocessing import DataDefinition
 
 
 class OOVWordsPercentage(GeneratedFeature):
+    column_name: str
+    ignore_words: Tuple = ()
+    _lem: WordNetLemmatizer
+    _eng_words: Set
+
     def __init__(self, column_name: str, ignore_words=()):
-        self.lem = WordNetLemmatizer()
-        self.eng_words = set(words.words())
+        self._lem = WordNetLemmatizer()
+        self._eng_words = set(words.words())
         self.column_name = column_name
         self.ignore_words = ignore_words
+        super().__init__()
 
     def generate_feature(self, data: pd.DataFrame, data_definition: DataDefinition) -> pd.DataFrame:
         def oov_share(s, ignore_words=()):
             if s is None:
                 return 0
             oov_num = 0
             words_ = re.sub("[^A-Za-z0-9 ]+", "", s).split()  # leave only letters, digits and spaces, split by spaces
             for word in words_:
-                if word.lower() not in ignore_words and self.lem.lemmatize(word.lower()) not in self.eng_words:
+                if word.lower() not in ignore_words and self._lem.lemmatize(word.lower()) not in self._eng_words:
                     oov_num += 1
             return 100 * oov_num / len(words_)
 
         return pd.DataFrame(
             dict(
                 [
                     (
```

### Comparing `evidently-0.3.2.1/src/evidently/features/generated_features.py` & `evidently-0.3.3/src/evidently/features/generated_features.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import abc
 import logging
 import typing
 from typing import Optional
 
 import pandas as pd
 
+from evidently.pydantic_utils import EvidentlyBaseModel
 from evidently.utils.data_preprocessing import DataDefinition
 
 if typing.TYPE_CHECKING:
     from evidently.base_metric import ColumnName
 
 
-class GeneratedFeature:
+class GeneratedFeature(EvidentlyBaseModel):
     """
     Class for computation of additional features.
     """
 
     @abc.abstractmethod
     def generate_feature(self, data: pd.DataFrame, data_definition: DataDefinition) -> pd.DataFrame:
         """
@@ -50,15 +51,15 @@
             hash(params)
         except TypeError:
             logging.warning(f"unhashable params for {type(self)}. Fallback to unique.")
             return None
         return params
 
 
-class FeatureDescriptor:
+class FeatureDescriptor(EvidentlyBaseModel):
     @abc.abstractmethod
     def for_column(self, column_name: str):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def feature(self, column_name: str) -> GeneratedFeature:
         raise NotImplementedError()
```

### Comparing `evidently-0.3.2.1/src/evidently/features/non_letter_character_percentage_feature.py` & `evidently-0.3.3/src/evidently/features/non_letter_character_percentage_feature.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 from evidently.base_metric import ColumnName
 from evidently.base_metric import additional_feature
 from evidently.features.generated_features import GeneratedFeature
 from evidently.utils.data_preprocessing import DataDefinition
 
 
 class NonLetterCharacterPercentage(GeneratedFeature):
+    column_name: str
+
     def __init__(self, column_name: str):
         self.column_name = column_name
+        super().__init__()
 
     def generate_feature(self, data: pd.DataFrame, data_definition: DataDefinition) -> pd.DataFrame:
 
         # counts share of characters that are not letters or spaces
         def non_letter_share(s):
             if s is None:
                 return 0
```

### Comparing `evidently-0.3.2.1/src/evidently/features/text_length_feature.py` & `evidently-0.3.3/src/evidently/features/text_length_feature.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 from evidently.base_metric import ColumnName
 from evidently.base_metric import additional_feature
 from evidently.features.generated_features import GeneratedFeature
 from evidently.utils.data_preprocessing import DataDefinition
 
 
 class TextLength(GeneratedFeature):
+    column_name: str
+
     def __init__(self, column_name: str):
         self.column_name = column_name
+        super().__init__()
 
     def generate_feature(self, data: pd.DataFrame, data_definition: DataDefinition) -> pd.DataFrame:
         def text_len(s):
             if s is None:
                 return 0
             return len(s)
```

### Comparing `evidently-0.3.2.1/src/evidently/features/trigger_words_presence_feature.py` & `evidently-0.3.3/src/evidently/features/trigger_words_presence_feature.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 import re
+from typing import Tuple
 
 import pandas as pd
 from nltk.stem.wordnet import WordNetLemmatizer
 
 from evidently.base_metric import additional_feature
 from evidently.features.generated_features import GeneratedFeature
 from evidently.utils.data_preprocessing import DataDefinition
 
 
 class TriggerWordsPresent(GeneratedFeature):
-    def __init__(self, column_name: str, words_list=(), lemmatisize=True):
-        self.lem = WordNetLemmatizer()
+    column_name: str
+    words_list: Tuple = ()
+    lemmatize: bool = True
+    _lem: WordNetLemmatizer
+
+    def __init__(self, column_name: str, words_list=(), lemmatize=True):
+        self._lem = WordNetLemmatizer()
         self.column_name = column_name
         self.words_list = words_list
-        self.lemmatisize = lemmatisize
+        self.lemmatize = lemmatize
+        super().__init__()
 
     def generate_feature(self, data: pd.DataFrame, data_definition: DataDefinition) -> pd.DataFrame:
-        def listed_words_present(s, words_list=(), lemmatisize=True):
+        def listed_words_present(s, words_list=(), lemmatize=True):
             if s is None:
                 return 0
             words = re.sub("[^A-Za-z0-9 ]+", "", s).split()
             for word_ in words:
                 word = word_.lower()
-                if lemmatisize:
-                    word = self.lem.lemmatize(word)
+                if lemmatize:
+                    word = self._lem.lemmatize(word)
                 if word in words_list:
                     return 1
             return 0
 
         return pd.DataFrame(
             dict(
                 [
                     (
                         self._feature_column_name(),
                         data[self.column_name].apply(
                             lambda x: listed_words_present(
                                 x,
                                 words_list=self.words_list,
-                                lemmatisize=self.lemmatisize,
+                                lemmatize=self.lemmatize,
                             )
                         ),
                     )
                 ]
             )
         )
 
     def get_parameters(self):
-        return self.column_name, tuple(self.words_list), self.lemmatisize
+        return self.column_name, tuple(self.words_list), self.lemmatize
 
     def feature_name(self):
         return additional_feature(self, self._feature_column_name(), self._feature_display_name())
 
     def _feature_column_name(self):
-        return self.column_name + "_" + "_".join(self.words_list) + "_" + str(self.lemmatisize)
+        return self.column_name + "_" + "_".join(self.words_list) + "_" + str(self.lemmatize)
 
     def _feature_display_name(self):
-        return f"TriggerWordsPresent [words: {self.words_list}, lemmatisize: {self.lemmatisize}] for {self.column_name}"
+        return f"TriggerWordsPresent [words: {self.words_list}, lemmatize: {self.lemmatize}] for {self.column_name}"
```

### Comparing `evidently-0.3.2.1/src/evidently/metric_preset/classification_performance.py` & `evidently-0.3.3/src/evidently/metric_preset/classification_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/metric_preset/data_drift.py` & `evidently-0.3.3/src/evidently/metric_preset/data_drift.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 
-import numpy as np
-
 from evidently.base_metric import InputData
 from evidently.calculations.stattests import PossibleStatTestType
 from evidently.metric_preset.metric_preset import MetricPreset
 from evidently.metric_results import DatasetColumns
 from evidently.metrics import DataDriftTable
 from evidently.metrics import DatasetDriftMetric
 from evidently.metrics import EmbeddingsDriftMetric
```

### Comparing `evidently-0.3.2.1/src/evidently/metric_preset/data_quality.py` & `evidently-0.3.3/src/evidently/metric_preset/data_quality.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/metric_preset/regression_performance.py` & `evidently-0.3.3/src/evidently/metric_preset/regression_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/metric_preset/target_drift.py` & `evidently-0.3.3/src/evidently/metric_preset/target_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/metric_preset/text_overview.py` & `evidently-0.3.3/src/evidently/metric_preset/text_overview.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/metric_results.py` & `evidently-0.3.3/src/evidently/metric_results.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,31 +6,72 @@
 from typing import Type
 from typing import TypeVar
 from typing import Union
 from typing import overload
 
 import numpy as np
 import pandas as pd
+from pydantic import parse_obj_as
+from pydantic import validator
 from typing_extensions import Literal
 
 from evidently.base_metric import MetricResult
 from evidently.core import IncludeTags
+from evidently.core import pydantic_type_validator
 from evidently.pipeline.column_mapping import TargetNames
 
 Label = Union[int, str]
-ScatterData = Union[pd.Series, List[float], pd.Index, pd.DataFrame]
+
+
+class _LabelKeyType(int):
+    pass
+
+
+LabelKey = Union[_LabelKeyType, Label]  # type: ignore[valid-type]
+
+
+@pydantic_type_validator(_LabelKeyType)
+def label_key_valudator(value):
+    try:
+        return int(value)
+    except ValueError:
+        return value
+
+
+ScatterData = Union[pd.Series]
 ContourData = Tuple[np.ndarray, List[float], List[float]]
-ColumnScatter = Dict[Label, ScatterData]
+ColumnScatter = Dict[LabelKey, ScatterData]
+
+ScatterAggData = Union[pd.DataFrame]
+ColumnAggScatter = Dict[LabelKey, ScatterAggData]
+
+
+class _ColumnScatterOrAggType:
+    pass
+
+
+ColumnScatterOrAgg = Union[_ColumnScatterOrAggType, ColumnScatter, ColumnAggScatter]  # type: ignore[valid-type]
+
+
+@pydantic_type_validator(_ColumnScatterOrAggType)
+def column_scatter_valudator(value):
+    if any(isinstance(o, dict) for o in value.values()):
+        # dict -> dataframe -> agg
+        return parse_obj_as(ColumnAggScatter, value)
+    if any(isinstance(o, (pd.DataFrame, pd.Series)) for o in value.values()):
+        return value
+    return parse_obj_as(ColumnScatter, value)
 
 
 class Distribution(MetricResult):
     class Config:
         dict_include = False
         pd_include = False
         tags = {IncludeTags.Render}
+        smart_union = True
 
     x: Union[np.ndarray, list, pd.Categorical, pd.Series]
     y: Union[np.ndarray, list, pd.Categorical, pd.Series]
 
 
 class ConfusionMatrix(MetricResult):
     class Config:
@@ -41,16 +82,35 @@
 
 
 class PredictionData(MetricResult):
     class Config:
         dict_include = False
 
     predictions: pd.Series
-    prediction_probas: Optional[pd.DataFrame]
     labels: List[Label]
+    prediction_probas: Optional[pd.DataFrame]
+
+    @validator("prediction_probas")
+    def validate_prediction_probas(cls, value: pd.DataFrame, values):
+        """Align label types"""
+        if value is None:
+            return None
+        labels = values["labels"]
+        for col in list(value.columns):
+            if col not in labels:
+                if str(col) in labels:
+                    value.rename(columns={col: str(col)}, inplace=True)
+                    continue
+                try:
+                    int_col = int(col)
+                    if int_col in labels:
+                        value.rename(columns={col: int_col}, inplace=True)
+                except ValueError:
+                    pass
+        return value
 
 
 class StatsByFeature(MetricResult):
     class Config:
         dict_include = False
         pd_include = False
         tags = {IncludeTags.Render}
@@ -156,14 +216,27 @@
         return None
     data = {column: df[column] for column in df.columns}
     if with_index:
         data["index"] = df.index
     return data
 
 
+class ScatterAggField(MetricResult):
+    class Config:
+        smart_union = True
+        dict_include = False
+        pd_include = False
+
+        tags = {IncludeTags.Render}
+
+    scatter: ColumnAggScatter
+    x_name: str
+    plot_shape: Dict[str, float]
+
+
 class ScatterField(MetricResult):
     class Config:
         smart_union = True
         dict_include = False
         pd_include = False
 
         tags = {IncludeTags.Render}
@@ -182,14 +255,19 @@
 
     current: ColumnScatter
     reference: Optional[ColumnScatter]
     x_name: str
     x_name_ref: Optional[str] = None
 
 
+class ColumnAggScatterResult(ColumnScatterResult):
+    current: ColumnAggScatter
+    reference: Optional[ColumnAggScatter]
+
+
 PlotData = List[float]
 
 
 class Boxes(MetricResult):
     class Config:
         dict_include = False
         tags = {IncludeTags.Render}
@@ -318,20 +396,20 @@
 
 
 def raw_agg_properties(field_name, raw_type: Type[TR], agg_type: Type[TA], optional: bool) -> Tuple[TR, TA]:
     def property_raw(self):
         val = getattr(self, field_name)
         if optional and val is None:
             return None
-        if not isinstance(val, raw_type):
+        if isinstance(raw_type, type) and not isinstance(val, raw_type):
             raise ValueError("Raw data not available")
         return val
 
     def property_agg(self):
         val = getattr(self, field_name)
         if optional and val is None:
             return None
-        if not isinstance(val, agg_type):
+        if isinstance(agg_type, type) and not isinstance(val, agg_type):
             raise ValueError("Agg data not available")
         return val
 
     return property(property_raw), property(property_agg)  # type: ignore[return-value]
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/base_metric.py` & `evidently-0.3.3/src/evidently/metrics/base_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/metrics/classification_performance/base_classification_metric.py` & `evidently-0.3.3/src/evidently/metrics/classification_performance/base_classification_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from abc import ABC
+from typing import Generic
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
 
 from evidently import ColumnMapping
 from evidently.base_metric import Metric
 from evidently.base_metric import TResult
 from evidently.calculations.classification_performance import get_prediction_data
 from evidently.calculations.classification_performance import k_probability_threshold
 from evidently.metric_results import DatasetColumns
 from evidently.metric_results import PredictionData
+from evidently.options.base import AnyOptions
 from evidently.utils.data_operations import process_columns
 
 
 def _cleanup_data(data: pd.DataFrame, dataset_columns: DatasetColumns) -> pd.DataFrame:
     target = dataset_columns.utility_columns.target
     prediction = dataset_columns.utility_columns.prediction
     subset = []
@@ -27,27 +29,27 @@
     if prediction is not None and isinstance(prediction, str):
         subset.append(prediction)
     if len(subset) > 0:
         return data.replace([np.inf, -np.inf], np.nan).dropna(axis=0, how="any", subset=subset)
     return data
 
 
-class ThresholdClassificationMetric(Metric[TResult], ABC):
+class ThresholdClassificationMetric(Metric, Generic[TResult], ABC):
     probas_threshold: Optional[float]
     k: Optional[Union[float, int]]
 
-    def __init__(self, probas_threshold: Optional[float], k: Optional[Union[float, int]]):
-        super().__init__()
+    def __init__(self, probas_threshold: Optional[float], k: Optional[Union[float, int]], options: AnyOptions = None):
         if probas_threshold is not None and k is not None:
             raise ValueError(
                 f"{self.__class__.__name__}: should provide only stattest_threshold or top_k argument, not both."
             )
 
         self.probas_threshold = probas_threshold
         self.k = k
+        super().__init__(options=options)
 
     def get_target_prediction_data(
         self, data: pd.DataFrame, column_mapping: ColumnMapping
     ) -> Tuple[pd.Series, PredictionData]:
         dataset_columns = process_columns(data, column_mapping)
         data = _cleanup_data(data, dataset_columns)
         prediction = get_prediction_data(data, dataset_columns, column_mapping.pos_label)
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/classification_performance/class_balance_metric.py` & `evidently-0.3.3/src/evidently/metrics/classification_performance/class_balance_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/metrics/classification_performance/class_separation_metric.py` & `evidently-0.3.3/src/evidently/metrics/classification_performance/class_separation_metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,38 +4,44 @@
 import numpy as np
 import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.classification_performance import get_prediction_data
+from evidently.metric_results import ColumnAggScatter
 from evidently.metric_results import ColumnScatter
+from evidently.metric_results import ColumnScatterOrAgg
 from evidently.metric_results import column_scatter_from_df
 from evidently.metric_results import df_from_column_scatter
+from evidently.metric_results import raw_agg_properties
 from evidently.model.widget import BaseWidgetInfo
 from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import get_class_separation_plot_data
 from evidently.renderers.html_widgets import get_class_separation_plot_data_agg
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import widget_tabs
 from evidently.utils.data_operations import process_columns
 
 
 class ClassificationClassSeparationPlotResults(MetricResult):
     class Config:
-        smart_union = True
         dict_exclude_fields = {"current", "reference"}
         pd_exclude_fields = {"current", "reference"}
 
     target_name: str
-    current: Optional[ColumnScatter] = None
-    reference: Optional[ColumnScatter] = None
+
+    current: Optional[ColumnScatterOrAgg] = None
+    current_raw, current_agg = raw_agg_properties("current", ColumnScatter, ColumnAggScatter, True)
+
+    reference: Optional[ColumnScatterOrAgg] = None
+    reference_raw, reference_agg = raw_agg_properties("reference", ColumnScatter, ColumnAggScatter, True)
 
 
 def prepare_box_data(df: pd.DataFrame, target_name: str, prediction_names: List[str]):
     res = {}
     for name in prediction_names:
         df_name = df.copy()
         df_name[target_name] = (df_name[target_name] == name).astype(int)
@@ -100,38 +106,40 @@
             target_name=target_name,
         )
 
 
 @default_renderer(wrap_type=ClassificationClassSeparationPlot)
 class ClassificationClassSeparationPlotRenderer(MetricRenderer):
     def render_html(self, obj: ClassificationClassSeparationPlot) -> List[BaseWidgetInfo]:
-        current_plot = obj.get_result().current
-        reference_plot = obj.get_result().reference
-        target_name = obj.get_result().target_name
+        metric_result = obj.get_result()
+        target_name = metric_result.target_name
         agg_data = not obj.get_options().render_options.raw_data
-        if current_plot is None:
+        if metric_result.current is None:
             return []
         if not agg_data:
+            assert metric_result.current_raw is not None  # checked before
             # todo changing data here, consider doing this in calculation
-            current_df = df_from_column_scatter(current_plot)
+            current_df = df_from_column_scatter(metric_result.current_raw)
             current_df.replace([np.inf, -np.inf], np.nan, inplace=True)
             reference_df = None
+            reference_plot = metric_result.reference_raw
             if reference_plot is not None:
                 reference_df = df_from_column_scatter(reference_plot)
                 reference_df.replace([np.inf, -np.inf], np.nan, inplace=True)
             tab_data = get_class_separation_plot_data(
                 current_df,
                 reference_df,
                 target_name,
                 color_options=self.color_options,
             )
         else:
+            assert metric_result.current_agg is not None  # checked before
             tab_data = get_class_separation_plot_data_agg(
-                current_plot,
-                reference_plot,
+                metric_result.current_agg,
+                metric_result.reference_agg,
                 target_name,
                 color_options=self.color_options,
             )
         tabs = [TabData(name, widget) for name, widget in tab_data]
         return [
             header_text(label="Class Separation Quality"),
             widget_tabs(title="", tabs=tabs),
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/classification_performance/classification_dummy_metric.py` & `evidently-0.3.3/src/evidently/metrics/classification_performance/classification_dummy_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from evidently.metric_results import PredictionData
 from evidently.metrics.classification_performance.base_classification_metric import ThresholdClassificationMetric
 from evidently.metrics.classification_performance.classification_quality_metric import ClassificationQualityMetric
 from evidently.metrics.classification_performance.objects import ClassesMetrics
 from evidently.metrics.classification_performance.objects import ClassificationReport
 from evidently.metrics.classification_performance.objects import ClassMetric
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import table_data
 from evidently.utils.data_operations import process_columns
 
 
@@ -36,34 +37,39 @@
     dummy: DatasetClassificationQuality
     by_reference_dummy: Optional[DatasetClassificationQuality]
     model_quality: Optional[DatasetClassificationQuality]
     metrics_matrix: ClassesMetrics
 
 
 class ClassificationDummyMetric(ThresholdClassificationMetric[ClassificationDummyMetricResults]):
-    quality_metric: ClassificationQualityMetric
+    _quality_metric: ClassificationQualityMetric
 
-    def __init__(self, probas_threshold: Optional[float] = None, k: Optional[Union[float, int]] = None):
-        super().__init__(probas_threshold, k)
+    def __init__(
+        self,
+        probas_threshold: Optional[float] = None,
+        k: Optional[Union[float, int]] = None,
+        options: AnyOptions = None,
+    ):
         self.probas_threshold = probas_threshold
         self.k = k
-        self.quality_metric = ClassificationQualityMetric()
+        super().__init__(probas_threshold, k, options)
+        self._quality_metric = ClassificationQualityMetric()
 
     def calculate(self, data: InputData) -> ClassificationDummyMetricResults:
         quality_metric: Optional[ClassificationQualityMetric]
         dataset_columns = process_columns(data.current_data, data.column_mapping)
         target_name = dataset_columns.utility_columns.target
         prediction_name = dataset_columns.utility_columns.prediction
 
         if target_name is None:
             raise ValueError("The column 'target' should present")
         if prediction_name is None:
             quality_metric = None
         else:
-            quality_metric = self.quality_metric
+            quality_metric = self._quality_metric
 
         #  dummy by current
         labels_ratio = data.current_data[target_name].value_counts(normalize=True)
         np.random.seed(0)
         dummy_preds = np.random.choice(labels_ratio.index, data.current_data.shape[0], p=labels_ratio)
         dummy_preds = pd.Series(dummy_preds)
         prediction: Optional[PredictionData] = None
@@ -121,20 +127,20 @@
             neg_label_precision = precision_score(target, dummy_preds, pos_label=labels[1]) * coeff_precision
             neg_label_recall = recall_score(target, dummy_preds, pos_label=labels[1]) * coeff_recall
             f1_label2_value = 2 * neg_label_precision * neg_label_recall / (neg_label_precision + neg_label_recall)
             metrics_matrix = {
                 str(labels[0]): ClassMetric(
                     precision=current_dummy.precision,
                     recall=current_dummy.recall,
-                    **{"f1-score": current_dummy.f1},
+                    **{"f1": current_dummy.f1},
                 ),
                 str(labels[1]): ClassMetric(
                     precision=neg_label_precision,
                     recall=neg_label_recall,
-                    **{"f1-score": f1_label2_value},
+                    **{"f1": f1_label2_value},
                 ),
             }
         if prediction is not None and prediction.prediction_probas is not None:
             # dummy log_loss and roc_auc
             binaraized_target = (target.astype(str).values.reshape(-1, 1) == list(labels)).astype(int)
             dummy_prediction = np.full(
                 prediction.prediction_probas.shape,
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/classification_performance/classification_quality_metric.py` & `evidently-0.3.3/src/evidently/metrics/classification_performance/classification_quality_metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from evidently.base_metric import InputData
 from evidently.base_metric import MetricResult
 from evidently.calculations.classification_performance import calculate_metrics
 from evidently.metric_results import DatasetClassificationQuality
 from evidently.metrics.classification_performance.base_classification_metric import ThresholdClassificationMetric
 from evidently.metrics.classification_performance.confusion_matrix_metric import ClassificationConfusionMatrix
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import header_text
 from evidently.utils.data_operations import process_columns
 
@@ -20,39 +21,44 @@
 class ClassificationQualityMetricResult(MetricResult):
     current: DatasetClassificationQuality
     reference: Optional[DatasetClassificationQuality]
     target_name: str
 
 
 class ClassificationQualityMetric(ThresholdClassificationMetric[ClassificationQualityMetricResult]):
-    confusion_matrix_metric: ClassificationConfusionMatrix
+    _confusion_matrix_metric: ClassificationConfusionMatrix
 
-    def __init__(self, probas_threshold: Optional[float] = None, k: Optional[Union[float, int]] = None):
-        super().__init__(probas_threshold=probas_threshold, k=k)
-        self.confusion_matrix_metric = ClassificationConfusionMatrix(probas_threshold=probas_threshold, k=k)
+    def __init__(
+        self,
+        probas_threshold: Optional[float] = None,
+        k: Optional[Union[float, int]] = None,
+        options: AnyOptions = None,
+    ):
+        self._confusion_matrix_metric = ClassificationConfusionMatrix(probas_threshold=probas_threshold, k=k)
+        super().__init__(probas_threshold=probas_threshold, k=k, options=options)
 
     def calculate(self, data: InputData) -> ClassificationQualityMetricResult:
         dataset_columns = process_columns(data.current_data, data.column_mapping)
         target_name = dataset_columns.utility_columns.target
         prediction_name = dataset_columns.utility_columns.prediction
         if target_name is None or prediction_name is None:
             raise ValueError("The columns 'target' and 'prediction' columns should be present")
         target, prediction = self.get_target_prediction_data(data.current_data, data.column_mapping)
         current = calculate_metrics(
             data.column_mapping,
-            self.confusion_matrix_metric.get_result().current_matrix,
+            self._confusion_matrix_metric.get_result().current_matrix,
             target,
             prediction,
         )
 
         reference = None
         if data.reference_data is not None:
-            ref_matrix = self.confusion_matrix_metric.get_result().reference_matrix
+            ref_matrix = self._confusion_matrix_metric.get_result().reference_matrix
             if ref_matrix is None:
-                raise ValueError(f"Dependency {self.confusion_matrix_metric.__class__} should have reference data")
+                raise ValueError(f"Dependency {self._confusion_matrix_metric.__class__} should have reference data")
             target, prediction = self.get_target_prediction_data(data.reference_data, data.column_mapping)
             reference = calculate_metrics(
                 data.column_mapping,
                 ref_matrix,
                 target,
                 prediction,
             )
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/classification_performance/confusion_matrix_metric.py` & `evidently-0.3.3/src/evidently/metrics/classification_performance/confusion_matrix_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
+from pydantic import BaseModel
+
 from evidently.base_metric import InputData
 from evidently.base_metric import MetricResult
 from evidently.calculations.classification_performance import calculate_matrix
 from evidently.metric_results import ConfusionMatrix
 from evidently.metrics.classification_performance.base_classification_metric import ThresholdClassificationMetric
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.pipeline.column_mapping import TargetNames
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import plotly_figure
 from evidently.utils.visualizations import plot_conf_mtrx
 
@@ -21,20 +24,32 @@
 
 class ClassificationConfusionMatrixResult(MetricResult):
     current_matrix: ConfusionMatrix
     reference_matrix: Optional[ConfusionMatrix]
     target_names: Optional[TargetNames] = None
 
 
-class ClassificationConfusionMatrix(ThresholdClassificationMetric[ClassificationConfusionMatrixResult]):
+class ClassificationConfusionMatrixParameters(BaseModel):
     probas_threshold: Optional[float]
     k: Optional[Union[float, int]]
 
-    def __init__(self, probas_threshold: Optional[float] = None, k: Optional[Union[float, int]] = None):
-        super().__init__(probas_threshold=probas_threshold, k=k)
+    def confusion_matric_metric(self):
+        return ClassificationConfusionMatrix(probas_threshold=self.probas_threshold, k=self.k)
+
+
+class ClassificationConfusionMatrix(
+    ThresholdClassificationMetric[ClassificationConfusionMatrixResult], ClassificationConfusionMatrixParameters
+):
+    def __init__(
+        self,
+        probas_threshold: Optional[float] = None,
+        k: Optional[Union[float, int]] = None,
+        options: AnyOptions = None,
+    ):
+        super().__init__(probas_threshold=probas_threshold, k=k, options=options)
 
     def calculate(self, data: InputData) -> ClassificationConfusionMatrixResult:
         current_target_data, current_pred = self.get_target_prediction_data(data.current_data, data.column_mapping)
         target_names = data.column_mapping.target_names
         current_results = calculate_matrix(
             current_target_data,
             current_pred.predictions,
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/classification_performance/objects.py` & `evidently-0.3.3/src/evidently/metrics/classification_performance/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import Dict
 from typing import Optional
-from typing import Union
 
 from pydantic import Field
 from pydantic import parse_obj_as
 from sklearn.metrics import classification_report
 
 from evidently.base_metric import MetricResult
 from evidently.metric_results import Label
 
 
 class ClassMetric(MetricResult):
     precision: float
     recall: float
-    f1: float = Field(alias="f1-score")
+    f1: float
     support: Optional[float] = None
 
 
 ClassesMetrics = Dict[Label, ClassMetric]
 
 
 class ClassificationReport(MetricResult):
@@ -45,10 +44,14 @@
             labels=class_metrics,
             target_names=target_names,
             sample_weight=sample_weight,
             digits=digits,
             output_dict=True,
             zero_division=zero_division,
         )
+        for v in report.values():
+            if not isinstance(v, dict):
+                continue
+            v["f1"] = v.pop("f1-score")
         class_metrics = {k: parse_obj_as(ClassMetric, report[str(k)]) for k in classes}
         other = {k: v for k, v in report.items() if k not in [str(cl) for cl in classes]}
         return parse_obj_as(cls, {"classes": class_metrics, **other})
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/classification_performance/pr_curve_metric.py` & `evidently-0.3.3/src/evidently/metrics/classification_performance/pr_curve_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import dataclasses
 from typing import List
 from typing import Optional
 
 import pandas as pd
 from sklearn import metrics
 
 from evidently.base_metric import InputData
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/classification_performance/pr_table_metric.py` & `evidently-0.3.3/src/evidently/metrics/classification_performance/pr_table_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-import dataclasses
+from typing import TYPE_CHECKING
+from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Type
 from typing import Union
 
 import pandas as pd
+from pydantic import BaseModel
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.classification_performance import calculate_pr_table
 from evidently.calculations.classification_performance import get_prediction_data
 from evidently.metric_results import Label
@@ -18,21 +21,32 @@
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import WidgetSize
 from evidently.renderers.html_widgets import table_data
 from evidently.renderers.html_widgets import widget_tabs
 from evidently.utils.data_operations import process_columns
 
-PRTable = Dict[Label, List[List[Union[float, int]]]]
+if TYPE_CHECKING:
+    from pydantic.main import Model
 
 
-class ClassificationPRTableResults(MetricResult):
-    class Config:
-        smart_union = True
+class LabelModel(BaseModel):
+    __root__: Union[int, str]
+
+    def validate(cls: Type["Model"], value: Any):  # type: ignore[override, misc]
+        try:
+            return int(value)
+        except TypeError:
+            return value
+
 
+PRTable = Dict[Union[LabelModel, Label], List[List[Union[float, int]]]]
+
+
+class ClassificationPRTableResults(MetricResult):
     current: Optional[PRTable] = None
     reference: Optional[PRTable] = None
 
 
 class ClassificationPRTable(Metric[ClassificationPRTableResults]):
     def calculate(self, data: InputData) -> ClassificationPRTableResults:
         dataset_columns = process_columns(data.current_data, data.column_mapping)
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/classification_performance/probability_distribution_metric.py` & `evidently-0.3.3/src/evidently/metrics/classification_performance/probability_distribution_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import dataclasses
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 
 import numpy as np
 import pandas as pd
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/classification_performance/quality_by_class_metric.py` & `evidently-0.3.3/src/evidently/metrics/classification_performance/quality_by_class_metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,58 @@
-import dataclasses
-from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
 import plotly.figure_factory as ff
 import sklearn
 from plotly import graph_objs as go
 from plotly.subplots import make_subplots
 
 from evidently.base_metric import InputData
 from evidently.base_metric import MetricResult
+from evidently.core import AllDict
 from evidently.metric_results import DatasetColumns
 from evidently.metrics.classification_performance.base_classification_metric import ThresholdClassificationMetric
 from evidently.metrics.classification_performance.objects import ClassesMetrics
 from evidently.metrics.classification_performance.objects import ClassificationReport
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import WidgetSize
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import plotly_figure
 from evidently.utils.data_operations import process_columns
 
 
 class ClassificationQuality(MetricResult):
     metrics: ClassesMetrics
     roc_aucs: Optional[List[float]]
 
     @property
     def metrics_dict(self):
-        return self.dict(include={"metrics"})["metrics"]
+        return self.dict(include={"metrics"}, exclude={"metrics": AllDict({"type"})})["metrics"]
 
 
 class ClassificationQualityByClassResult(MetricResult):
     columns: DatasetColumns
     current: ClassificationQuality
     reference: Optional[ClassificationQuality]
 
 
 class ClassificationQualityByClass(ThresholdClassificationMetric[ClassificationQualityByClassResult]):
-    def __init__(self, probas_threshold: Optional[float] = None, k: Optional[Union[float, int]] = None):
-        super().__init__(probas_threshold, k)
+    def __init__(
+        self,
+        probas_threshold: Optional[float] = None,
+        k: Optional[Union[float, int]] = None,
+        options: AnyOptions = None,
+    ):
+        super().__init__(probas_threshold, k, options=options)
 
     def calculate(self, data: InputData) -> ClassificationQualityByClassResult:
         columns = process_columns(data.current_data, data.column_mapping)
         target, prediction = self.get_target_prediction_data(
             data.current_data,
             column_mapping=data.column_mapping,
         )
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/classification_performance/quality_by_feature_table.py` & `evidently-0.3.3/src/evidently/metrics/classification_performance/quality_by_feature_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,26 +36,26 @@
     target_name: str
     columns: List[str]
 
 
 class ClassificationQualityByFeatureTable(Metric[ClassificationQualityByFeatureTableResults]):
     columns: Optional[List[str]]
     descriptors: Optional[Dict[str, Dict[str, FeatureDescriptor]]]
-    text_features_gen: Optional[Dict[str, Dict[str, GeneratedFeature]]]
+    _text_features_gen: Optional[Dict[str, Dict[str, GeneratedFeature]]]
 
     def __init__(
         self,
         columns: Optional[List[str]] = None,
         descriptors: Optional[Dict[str, Dict[str, FeatureDescriptor]]] = None,
         options: AnyOptions = None,
     ):
-        super().__init__(options=options)
         self.columns = columns
-        self.text_features_gen = None
+        self._text_features_gen = None
         self.descriptors = descriptors
+        super().__init__(options=options)
 
     def required_features(self, data_definition: DataDefinition):
         if len(data_definition.get_columns("text_features")) > 0:
             text_cols = [col.column_name for col in data_definition.get_columns("text_features")]
             text_features_gen = {}
             text_features_gen_result = []
             for col in text_cols:
@@ -69,15 +69,15 @@
                     }
                 else:
                     column_descriptors = self.descriptors[col]
                     col_dict = {f"{col}: " + name: value.feature(col) for name, value in column_descriptors.items()}
 
                 text_features_gen_result += list(col_dict.values())
                 text_features_gen[col] = col_dict
-            self.text_features_gen = text_features_gen
+            self._text_features_gen = text_features_gen
 
             return text_features_gen_result
         else:
             return []
 
     def get_parameters(self) -> tuple:
         return ()
@@ -119,16 +119,16 @@
                         + dataset_columns.text_feature_names
                     ),
                 )
             )
 
         # process text columns
 
-        if self.text_features_gen is not None:
-            for column, features in self.text_features_gen.items():
+        if self._text_features_gen is not None:
+            for column, features in self._text_features_gen.items():
                 columns.remove(column)
                 columns += list(features.keys())
                 curr_text_df = pd.concat([data.get_current_column(x.feature_name()) for x in features.values()], axis=1)
                 curr_text_df.columns = list(features.keys())
                 curr_df = pd.concat([curr_df.reset_index(drop=True), curr_text_df.reset_index(drop=True)], axis=1)
 
                 if ref_df is not None:
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/classification_performance/roc_curve_metric.py` & `evidently-0.3.3/src/evidently/metrics/classification_performance/roc_curve_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import dataclasses
 from typing import List
 from typing import Optional
 
 import pandas as pd
 from sklearn import metrics
 
 from evidently.base_metric import InputData
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_drift/column_drift_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_drift/column_drift_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from evidently.calculations.data_drift import DistributionIncluded
 from evidently.calculations.data_drift import DriftStatsField
 from evidently.calculations.data_drift import ScatterField
 from evidently.calculations.data_drift import get_distribution_for_column
 from evidently.calculations.data_drift import get_stattest
 from evidently.calculations.data_drift import get_text_data_for_plots
 from evidently.calculations.stattests import PossibleStatTestType
+from evidently.metric_results import ScatterAggField
 from evidently.model.widget import BaseWidgetInfo
 from evidently.options import DataDriftOptions
 from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import TabData
@@ -100,15 +101,15 @@
 
         if not pd.api.types.is_numeric_dtype(current_column):
             raise ValueError(f"Column '{column}' in current dataset should contain numerical values only.")
 
     drift_test_function = get_stattest(reference_column, current_column, column_type.value, stattest)
     drift_result = drift_test_function(reference_column, current_column, column_type.value, threshold)
 
-    scatter: Optional[ScatterField] = None
+    scatter: Optional[Union[ScatterField, ScatterAggField]] = None
     if column_type == ColumnType.Numerical:
         current_nbinsx = options.get_nbinsx(column.name)
         current_small_distribution = [
             t.tolist()
             for t in np.histogram(
                 current_column[np.isfinite(current_column)],
                 bins=current_nbinsx,
@@ -154,15 +155,18 @@
                 x_name = f"Timestamp ({prefix})"
 
         plot_shape = {}
         reference_mean = reference_column.mean()
         reference_std = reference_column.std()
         plot_shape["y0"] = reference_mean - reference_std
         plot_shape["y1"] = reference_mean + reference_std
-        scatter = ScatterField(scatter=current_scatter, x_name=x_name, plot_shape=plot_shape)
+        if agg_data:
+            scatter = ScatterAggField(scatter=current_scatter, x_name=x_name, plot_shape=plot_shape)
+        else:
+            scatter = ScatterField(scatter=current_scatter, x_name=x_name, plot_shape=plot_shape)
 
     elif column_type == ColumnType.Categorical:
         reference_counts = reference_column.value_counts(sort=False)
         current_counts = current_column.value_counts(sort=False)
         keys = set(reference_counts.keys()).union(set(current_counts.keys()))
 
         for key in keys:
@@ -263,65 +267,58 @@
 
     return metrics
 
 
 class ColumnDriftMetric(ColumnMetric[ColumnDataDriftMetrics]):
     """Calculate drift metric for a column"""
 
-    column: ColumnName
-
     stattest: Optional[PossibleStatTestType]
     stattest_threshold: Optional[float]
 
     def __init__(
         self,
         column_name: Union[ColumnName, str],
         stattest: Optional[PossibleStatTestType] = None,
         stattest_threshold: Optional[float] = None,
         options: AnyOptions = None,
     ):
-        super().__init__(options=options)
-        if isinstance(column_name, str):
-            column = ColumnName.main_dataset(column_name)
-        else:
-            column = column_name
-        self.column = column
-        self.column_name = column.name
+
         self.stattest = stattest
         self.stattest_threshold = stattest_threshold
+        super().__init__(column_name=column_name, options=options)
 
     def get_parameters(self) -> tuple:
-        return self.column, self.stattest_threshold, self.stattest
+        return self.column_name, self.stattest_threshold, self.stattest
 
     def calculate(self, data: InputData) -> ColumnDataDriftMetrics:
         if data.reference_data is None:
             raise ValueError("Reference dataset should be present")
 
         try:
-            current_feature_data = data.get_current_column(self.column)
+            current_feature_data = data.get_current_column(self.column_name)
         except ColumnNotFound as ex:
             raise ValueError(f"Cannot find column '{ex.column_name}' in current dataset")
         try:
-            reference_feature_data = data.get_reference_column(self.column)
+            reference_feature_data = data.get_reference_column(self.column_name)
         except ColumnNotFound as ex:
             raise ValueError(f"Cannot find column '{ex.column_name}' in reference dataset")
 
         column_type = ColumnType.Numerical
-        if self.column.is_main_dataset():
-            column_type = data.data_definition.get_column(self.column.name).column_type
+        if self.column_name.is_main_dataset():
+            column_type = data.data_definition.get_column(self.column_name.name).column_type
         datetime_column = data.data_definition.get_datetime_column()
         options = DataDriftOptions(all_features_stattest=self.stattest, threshold=self.stattest_threshold)
         if self.get_options().render_options.raw_data:
             agg_data = False
         else:
             agg_data = True
         drift_result = get_one_column_drift(
             current_feature_data=current_feature_data,
             reference_feature_data=reference_feature_data,
-            column=self.column,
+            column=self.column_name,
             index_data=data.current_data.index,
             column_type=column_type,
             datetime_data=data.current_data[datetime_column.column_name] if datetime_column else None,
             data_definition=data.data_definition,
             options=options,
             agg_data=agg_data,
         )
@@ -371,14 +368,15 @@
                     curr_data=result.scatter.scatter,
                     ref_data=None,
                     line=(result.scatter.plot_shape["y0"] + result.scatter.plot_shape["y1"]) / 2,
                     std=(result.scatter.plot_shape["y0"] - result.scatter.plot_shape["y1"]) / 2,
                     xaxis_name=result.scatter.x_name,
                     xaxis_name_ref=None,
                     yaxis_name=result.column_name,
+                    color_options=self.color_options,
                     return_json=False,
                 )
             tabs.append(TabData("DATA DRIFT", plotly_figure(title="", figure=scatter_fig)))
 
         if result.current.distribution is not None and result.reference.distribution is not None:
             distr_fig = get_distribution_plot_figure(
                 current_distribution=result.current.distribution,
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_drift/column_value_plot.py` & `evidently-0.3.3/src/evidently/metrics/data_drift/column_value_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from pandas.api.types import is_numeric_dtype
 from plotly import graph_objs as go
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.core import IncludeTags
+from evidently.metric_results import ColumnAggScatter
 from evidently.metric_results import ColumnScatter
-from evidently.metric_results import ScatterData
+from evidently.metric_results import ColumnScatterOrAgg
 from evidently.metric_results import column_scatter_from_df
 from evidently.metric_results import raw_agg_properties
 from evidently.model.widget import BaseWidgetInfo
 from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import WidgetSize
@@ -26,32 +27,34 @@
 from evidently.utils.visualizations import choose_agg_period
 from evidently.utils.visualizations import plot_agg_line_data
 from evidently.utils.visualizations import prepare_df_for_time_index_plot
 
 
 class ColumnValuePlotResults(MetricResult):
     class Config:
-        smart_union = True
         dict_include = False
         pd_include = False
         tags = {IncludeTags.Render}
 
     column_name: str
     datetime_column_name: Optional[str]
-    current: ColumnScatter
-    reference: ColumnScatter
+    current: Union[ColumnScatterOrAgg]
+    current_raw, current_agg = raw_agg_properties("current", ColumnScatter, ColumnAggScatter, False)
+
+    reference: Union[ColumnScatterOrAgg]
+    reference_raw, reference_agg = raw_agg_properties("reference", ColumnScatter, ColumnAggScatter, False)
     prefix: Optional[str] = None
 
 
 class ColumnValuePlot(Metric[ColumnValuePlotResults]):
     column_name: str
 
     def __init__(self, column_name: str, options: AnyOptions = None):
-        super().__init__(options=options)
         self.column_name = column_name
+        super().__init__(options=options)
 
     def calculate(self, data: InputData) -> ColumnValuePlotResults:
         if self.column_name not in data.current_data.columns:
             raise ValueError(f"Column '{self.column_name}' should present in the current dataset")
 
         if data.reference_data is None:
             raise ValueError("Reference data should be present")
@@ -117,15 +120,16 @@
 
 
 @default_renderer(wrap_type=ColumnValuePlot)
 class ColumnValuePlotRenderer(MetricRenderer):
     def render_raw(self, current_scatter, reference_scatter, column_name, datetime_column_name):
         # todo: better typing
         column = reference_scatter[column_name]
-        assert isinstance(column, pd.Series)
+        if not isinstance(column, pd.Series):
+            column = pd.Series(column)
         mean_ref = column.mean()
         std_ref = column.std()
         y0 = mean_ref - std_ref
         y1 = mean_ref + std_ref
 
         if datetime_column_name is not None:
             curr_x = current_scatter[datetime_column_name]
@@ -218,14 +222,15 @@
             curr_data=data,
             ref_data=None,
             line=None,
             std=None,
             xaxis_name=xaxis_name,
             xaxis_name_ref=None,
             yaxis_name=column_name + " value",
+            color_options=self.color_options,
         )
 
         return [
             header_text(label=f"Column '{column_name}' Values"),
             BaseWidgetInfo(
                 title="",
                 size=2,
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_drift/data_drift_table.py` & `evidently-0.3.3/src/evidently/metrics/data_drift/data_drift_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from evidently.base_metric import InputData
-from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.data_drift import ColumnDataDriftMetrics
 from evidently.calculations.data_drift import get_drift_for_columns
 from evidently.calculations.stattests import PossibleStatTestType
 from evidently.metric_results import DatasetColumns
+from evidently.metrics.data_drift.base import WithDriftOptions
 from evidently.model.widget import BaseWidgetInfo
 from evidently.options import DataDriftOptions
 from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import ColumnDefinition
 from evidently.renderers.html_widgets import ColumnType
@@ -36,17 +36,16 @@
     number_of_drifted_columns: int
     share_of_drifted_columns: float
     dataset_drift: bool
     drift_by_columns: Dict[str, ColumnDataDriftMetrics]
     dataset_columns: DatasetColumns
 
 
-class DataDriftTable(Metric[DataDriftTableResults]):
+class DataDriftTable(WithDriftOptions[DataDriftTableResults]):
     columns: Optional[List[str]]
-    drift_options: DataDriftOptions
 
     def __init__(
         self,
         columns: Optional[List[str]] = None,
         stattest: Optional[PossibleStatTestType] = None,
         cat_stattest: Optional[PossibleStatTestType] = None,
         num_stattest: Optional[PossibleStatTestType] = None,
@@ -55,17 +54,29 @@
         stattest_threshold: Optional[float] = None,
         cat_stattest_threshold: Optional[float] = None,
         num_stattest_threshold: Optional[float] = None,
         text_stattest_threshold: Optional[float] = None,
         per_column_stattest_threshold: Optional[Dict[str, float]] = None,
         options: AnyOptions = None,
     ):
-        super().__init__(options=options)
         self.columns = columns
-        self.drift_options = DataDriftOptions(
+        super().__init__(
+            stattest=stattest,
+            cat_stattest=cat_stattest,
+            num_stattest=num_stattest,
+            text_stattest=text_stattest,
+            per_column_stattest=per_column_stattest,
+            stattest_threshold=stattest_threshold,
+            cat_stattest_threshold=cat_stattest_threshold,
+            num_stattest_threshold=num_stattest_threshold,
+            text_stattest_threshold=text_stattest_threshold,
+            per_column_stattest_threshold=per_column_stattest_threshold,
+            options=options,
+        )
+        self._drift_options = DataDriftOptions(
             all_features_stattest=stattest,
             cat_features_stattest=cat_stattest,
             num_features_stattest=num_stattest,
             text_features_stattest=text_stattest,
             per_feature_stattest=per_column_stattest,
             all_features_threshold=stattest_threshold,
             cat_features_threshold=cat_stattest_threshold,
@@ -192,14 +203,15 @@
                         curr_data=data.scatter.scatter,
                         ref_data=None,
                         line=(data.scatter.plot_shape["y0"] + data.scatter.plot_shape["y1"]) / 2,
                         std=(data.scatter.plot_shape["y0"] - data.scatter.plot_shape["y1"]) / 2,
                         xaxis_name=data.scatter.x_name,
                         xaxis_name_ref=None,
                         yaxis_name=data.column_name,
+                        color_options=self.color_options,
                         return_json=False,
                     )
                 scatter = plotly_figure(title="", figure=scatter_fig)
                 details.with_part("DATA DRIFT", info=scatter)
             fig = get_distribution_plot_figure(
                 current_distribution=data.current.distribution,
                 reference_distribution=data.reference.distribution,
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_drift/dataset_drift_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_drift/dataset_drift_metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from evidently.base_metric import InputData
-from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.data_drift import get_drift_for_columns
 from evidently.calculations.stattests import PossibleStatTestType
+from evidently.metrics.data_drift.base import WithDriftOptions
 from evidently.model.widget import BaseWidgetInfo
 from evidently.options import DataDriftOptions
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import counter
 from evidently.utils.data_operations import process_columns
 
 
@@ -20,17 +21,18 @@
     drift_share: float
     number_of_columns: int
     number_of_drifted_columns: int
     share_of_drifted_columns: float
     dataset_drift: bool
 
 
-class DatasetDriftMetric(Metric[DatasetDriftMetricResults]):
+class DatasetDriftMetric(
+    WithDriftOptions[DatasetDriftMetricResults],
+):
     columns: Optional[List[str]]
-    drift_options: DataDriftOptions
     drift_share: float
 
     def __init__(
         self,
         columns: Optional[List[str]] = None,
         drift_share: float = 0.5,
         stattest: Optional[PossibleStatTestType] = None,
@@ -39,29 +41,43 @@
         text_stattest: Optional[PossibleStatTestType] = None,
         per_column_stattest: Optional[Dict[str, PossibleStatTestType]] = None,
         stattest_threshold: Optional[float] = None,
         cat_stattest_threshold: Optional[float] = None,
         num_stattest_threshold: Optional[float] = None,
         text_stattest_threshold: Optional[float] = None,
         per_column_stattest_threshold: Optional[Dict[str, float]] = None,
+        options: AnyOptions = None,
     ):
         self.columns = columns
-        self.drift_options = DataDriftOptions(
-            all_features_stattest=stattest,
-            cat_features_stattest=cat_stattest,
-            num_features_stattest=num_stattest,
-            text_features_stattest=text_stattest,
-            per_feature_stattest=per_column_stattest,
-            all_features_threshold=stattest_threshold,
-            cat_features_threshold=cat_stattest_threshold,
-            num_features_threshold=num_stattest_threshold,
-            text_features_threshold=text_stattest_threshold,
-            per_feature_threshold=per_column_stattest_threshold,
-        )
         self.drift_share = drift_share
+        super().__init__(
+            stattest=stattest,
+            cat_stattest=cat_stattest,
+            num_stattest=num_stattest,
+            text_stattest=text_stattest,
+            per_column_stattest=per_column_stattest,
+            stattest_threshold=stattest_threshold,
+            cat_stattest_threshold=cat_stattest_threshold,
+            num_stattest_threshold=num_stattest_threshold,
+            text_stattest_threshold=text_stattest_threshold,
+            per_column_stattest_threshold=per_column_stattest_threshold,
+            options=options,
+        )
+        self._drift_options = DataDriftOptions(
+            all_features_stattest=self.stattest,
+            cat_features_stattest=self.cat_stattest,
+            num_features_stattest=self.num_stattest,
+            text_features_stattest=self.text_stattest,
+            per_feature_stattest=self.per_column_stattest,
+            all_features_threshold=self.stattest_threshold,
+            cat_features_threshold=self.cat_stattest_threshold,
+            num_features_threshold=self.num_stattest_threshold,
+            text_features_threshold=self.text_stattest_threshold,
+            per_feature_threshold=self.per_column_stattest_threshold,
+        )
 
     def get_parameters(self) -> tuple:
         return (
             self.drift_share,
             None if self.columns is None else tuple(self.columns),
             self.drift_options,
         )
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_drift/embedding_drift_methods.py` & `evidently-0.3.3/src/evidently/metrics/data_drift/embedding_drift_methods.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_drift/embeddings_drift.py` & `evidently-0.3.3/src/evidently/metrics/data_drift/embeddings_drift.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.core import IncludeTags
 from evidently.metrics.data_drift.embedding_drift_methods import model
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import WidgetSize
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import plotly_figure
 from evidently.utils.visualizations import get_gaussian_kde
@@ -38,36 +39,36 @@
     method_name: str
     reference: np.ndarray
     current: np.ndarray
 
 
 class EmbeddingsDriftMetric(Metric[EmbeddingsDriftMetricResults]):
     embeddings_name: str
-    drift_method: Optional[Callable]
+    _drift_method: Optional[Callable]
 
-    def __init__(self, embeddings_name: str, drift_method: Optional[Callable] = None):
-        super().__init__()
+    def __init__(self, embeddings_name: str, drift_method: Optional[Callable] = None, options: AnyOptions = None):
         self.embeddings_name = embeddings_name
-        self.drift_method = drift_method
+        self._drift_method = drift_method
+        super().__init__(options=options)
 
     def calculate(self, data: InputData) -> EmbeddingsDriftMetricResults:
         if data.reference_data is None:
             raise ValueError("Reference dataset should be present")
-        if self.drift_method is None:
+        if self._drift_method is None:
             is_bootstrap = False
             if data.reference_data.shape[0] < 1000:
                 is_bootstrap = True
-            self.drift_method = model(bootstrap=is_bootstrap)
+            self._drift_method = model(bootstrap=is_bootstrap)
         emb_dict = data.data_definition.embeddings()
         if emb_dict is None:
-            raise ValueError("Embeddings shold be defined in column mapping")
+            raise ValueError("Embeddings should be defined in column mapping")
         if self.embeddings_name not in emb_dict.keys():
             raise ValueError(f"{self.embeddings_name} not in column_mapping.embeddings")
         emb_list = emb_dict[self.embeddings_name]
-        drift_score, drift_detected, method_name = self.drift_method(
+        drift_score, drift_detected, method_name = self._drift_method(
             data.current_data[emb_list], data.reference_data[emb_list]
         )
         # visualisation
         ref_sample_size = min(SAMPLE_CONSTANT, data.reference_data.shape[0])
         curr_sample_size = min(SAMPLE_CONSTANT, data.current_data.shape[0])
         ref_sample = data.reference_data[emb_list].sample(ref_sample_size, random_state=24)
         curr_sample = data.current_data[emb_list].sample(curr_sample_size, random_state=24)
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_drift/target_by_features_table.py` & `evidently-0.3.3/src/evidently/metrics/data_drift/target_by_features_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.classification_performance import get_prediction_data
 from evidently.features.non_letter_character_percentage_feature import NonLetterCharacterPercentage
 from evidently.features.OOV_words_percentage_feature import OOVWordsPercentage
 from evidently.features.text_length_feature import TextLength
-from evidently.metric_results import PredictionData
 from evidently.metric_results import StatsByFeature
 from evidently.model.widget import AdditionalGraphInfo
 from evidently.model.widget import BaseWidgetInfo
 from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.utils.data_operations import process_columns
@@ -39,25 +38,25 @@
     target_name: Optional[str]
     columns: List[str]
     task: str
 
 
 class TargetByFeaturesTable(Metric[TargetByFeaturesTableResults]):
     columns: Optional[List[str]]
-    text_features_gen: Optional[
+    _text_features_gen: Optional[
         Dict[
             str,
             Dict[str, Union[TextLength, NonLetterCharacterPercentage, OOVWordsPercentage]],
         ]
     ]
 
     def __init__(self, columns: Optional[List[str]] = None, options: AnyOptions = None):
-        super().__init__(options=options)
         self.columns = columns
-        self.text_features_gen = None
+        super().__init__(options=options)
+        self._text_features_gen = None
 
     def required_features(self, data_definition: DataDefinition):
         if len(data_definition.get_columns("text_features")) > 0:
             text_cols = [col.column_name for col in data_definition.get_columns("text_features")]
             text_features_gen = {}
             text_features_gen_result = []
             for col in text_cols:
@@ -71,15 +70,15 @@
 
                 text_features_gen_result += [
                     col_dict[f"{col}: Text Length"],
                     col_dict[f"{col}: Non Letter Character %"],
                     col_dict[f"{col}: OOV %"],
                 ]
                 text_features_gen[col] = col_dict
-            self.text_features_gen = text_features_gen
+            self._text_features_gen = text_features_gen
 
             return text_features_gen_result
         else:
             return []
 
     def get_parameters(self) -> tuple:
         return ()
@@ -140,42 +139,42 @@
                     task = "classification"
                 else:
                     task = "regression"
             else:
                 raise ValueError("Task parameter of column_mapping should be specified")
         # process text columns
         if (
-            self.text_features_gen is not None
-            and len(np.intersect1d(list(self.text_features_gen.keys()), columns)) >= 1
+            self._text_features_gen is not None
+            and len(np.intersect1d(list(self._text_features_gen.keys()), columns)) >= 1
         ):
-            for col in np.intersect1d(list(self.text_features_gen.keys()), columns):
-                columns += list(self.text_features_gen[col].keys())
+            for col in np.intersect1d(list(self._text_features_gen.keys()), columns):
+                columns += list(self._text_features_gen[col].keys())
                 columns.remove(col)
                 curr_text_df = pd.concat(
-                    [data.get_current_column(x.feature_name()) for x in list(self.text_features_gen[col].values())],
+                    [data.get_current_column(x.feature_name()) for x in list(self._text_features_gen[col].values())],
                     axis=1,
                 )
-                curr_text_df.columns = list(self.text_features_gen[col].keys())
+                curr_text_df.columns = list(self._text_features_gen[col].keys())
                 curr_df = pd.concat(
                     [
                         curr_df.reset_index(drop=True),
                         curr_text_df.reset_index(drop=True),
                     ],
                     axis=1,
                 )
 
                 if ref_df is not None:
                     ref_text_df = pd.concat(
                         [
                             data.get_reference_column(x.feature_name())
-                            for x in list(self.text_features_gen[col].values())
+                            for x in list(self._text_features_gen[col].values())
                         ],
                         axis=1,
                     )
-                    ref_text_df.columns = list(self.text_features_gen[col].keys())
+                    ref_text_df.columns = list(self._text_features_gen[col].keys())
                     ref_df = pd.concat(
                         [
                             ref_df.reset_index(drop=True),
                             ref_text_df.reset_index(drop=True),
                         ],
                         axis=1,
                     )
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,49 +45,59 @@
     dataset_drift: bool
     drift_by_columns: Dict[str, ColumnDataDriftMetrics]
     dataset_columns: DatasetColumns
 
 
 class TextDescriptorsDriftMetric(Metric[TextDescriptorsDriftMetricResults]):
     column_name: str
-    drift_options: DataDriftOptions
-    generated_text_features: Dict[str, GeneratedFeature]
+    stattest: Optional[PossibleStatTestType] = None
+    stattest_threshold: Optional[float] = None
+    descriptors: Dict[str, FeatureDescriptor]
+    _drift_options: DataDriftOptions
+    _generated_text_features: Dict[str, GeneratedFeature]
 
     def __init__(
         self,
         column_name: str,
         descriptors: Optional[Dict[str, FeatureDescriptor]] = None,
         stattest: Optional[PossibleStatTestType] = None,
         stattest_threshold: Optional[float] = None,
         options: AnyOptions = None,
     ):
-        super().__init__(options=options)
         self.column_name = column_name
-        self.drift_options = DataDriftOptions(all_features_stattest=stattest, all_features_threshold=stattest_threshold)
+
         if descriptors:
             self.descriptors = descriptors
         else:
             self.descriptors = {
                 "Text Length": TextLength(),
                 "Non Letter Character %": NonLetterCharacterPercentage(),
                 "OOV %": OOV(),
             }
-        self.generated_text_features = {}
+        super().__init__(stattest=stattest, stattest_threshold=stattest_threshold, options=options)
+        self._generated_text_features = {}
+        self._drift_options = DataDriftOptions(
+            all_features_stattest=stattest, all_features_threshold=stattest_threshold
+        )
+
+    @property
+    def generated_text_features(self):
+        return self._generated_text_features
 
     def required_features(self, data_definition: DataDefinition):
         column_type = data_definition.get_column(self.column_name).column_type
         if column_type == ColumnType_data.Text:
-            self.generated_text_features = {
+            self._generated_text_features = {
                 name: desc.feature(self.column_name) for name, desc in self.descriptors.items()
             }
             return list(self.generated_text_features.values())
         return []
 
     def get_parameters(self) -> tuple:
-        return self.column_name, self.drift_options
+        return self.column_name, self._drift_options
 
     def calculate(self, data: InputData) -> TextDescriptorsDriftMetricResults:
         if data.reference_data is None:
             raise ValueError("Reference dataset should be present")
         if self.get_options().render_options.raw_data:
             agg_data = False
         else:
@@ -108,15 +118,15 @@
 
         drift_by_columns = {}
         for col in curr_text_df.columns:
             drift_by_columns[col] = get_one_column_drift(
                 current_data=curr_text_df,
                 reference_data=ref_text_df,
                 column_name=col,
-                options=self.drift_options,
+                options=self._drift_options,
                 dataset_columns=text_dataset_columns,
                 agg_data=agg_data,
             )
         dataset_drift = get_dataset_drift(drift_by_columns, 0)
 
         return TextDescriptorsDriftMetricResults(
             number_of_columns=curr_text_df.shape[1],
@@ -159,14 +169,15 @@
                     curr_data=data.scatter.scatter,
                     ref_data=None,
                     line=(data.scatter.plot_shape["y0"] + data.scatter.plot_shape["y1"]) / 2,
                     std=(data.scatter.plot_shape["y0"] - data.scatter.plot_shape["y1"]) / 2,
                     xaxis_name=data.scatter.x_name,
                     xaxis_name_ref=None,
                     yaxis_name=data.column_name,
+                    color_options=self.color_options,
                     return_json=False,
                 )
             scatter = plotly_figure(title="", figure=scatter_fig)
             details.with_part("DATA DRIFT", info=scatter)
             fig = get_distribution_plot_figure(
                 current_distribution=data.current.distribution,
                 reference_distribution=data.reference.distribution,
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from sklearn.model_selection import train_test_split
 from sklearn.pipeline import Pipeline
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import table_data
 from evidently.renderers.html_widgets import widget_tabs
@@ -36,16 +37,17 @@
     current: TextDomainField
     reference: TextDomainField
 
 
 class TextDomainClassifierDriftMetric(Metric[TextDomainClassifierDriftResult]):
     text_column_name: str
 
-    def __init__(self, text_column_name: str) -> None:
+    def __init__(self, text_column_name: str, options: AnyOptions = None) -> None:
         self.text_column_name = text_column_name
+        super().__init__(options=options)
 
     @staticmethod
     def roc_auc_domain_classifier(X_train, X_test, y_train, y_test) -> Tuple:
         pipeline = Pipeline(
             [
                 (
                     "vectorization",
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_integrity/column_missing_values_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_integrity/column_missing_values_metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import dataclasses
 from typing import Any
+from typing import ClassVar
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import table_data
@@ -54,31 +55,37 @@
     Value None in the list means that Pandas null values will be included in the calculation.
 
     If `replace` parameter is False - add defaults to user's list.
     If `replace` parameter is True - use values from `missing_values` list only.
     """
 
     # default missing values list
-    DEFAULT_MISSING_VALUES = ["", np.inf, -np.inf, None]
+    DEFAULT_MISSING_VALUES: ClassVar = ["", np.inf, -np.inf, None]
     missing_values: frozenset
     column_name: str
 
-    def __init__(self, column_name: str, missing_values: Optional[list] = None, replace: bool = True) -> None:
+    def __init__(
+        self, column_name: str, missing_values: Optional[list] = None, replace: bool = True, options: AnyOptions = None
+    ) -> None:
         self.column_name = column_name
 
+        _missing_values: list
         if missing_values is None:
             # use default missing values list if we have no user-defined missed values
-            missing_values = self.DEFAULT_MISSING_VALUES
+            _missing_values = self.DEFAULT_MISSING_VALUES
 
         elif not replace:
             # add default missing values to user-defined list
-            missing_values = self.DEFAULT_MISSING_VALUES + missing_values
+            _missing_values = self.DEFAULT_MISSING_VALUES + missing_values
+        else:
+            _missing_values = missing_values
 
         # use frozenset because metrics parameters should be immutable/hashable for deduplication
-        self.missing_values = frozenset(missing_values)
+        self.missing_values = frozenset(_missing_values)
+        super().__init__(options=options)
 
     def _calculate_missing_values_stats(self, column: pd.Series) -> ColumnMissingValues:
         different_missing_values = {value: 0 for value in self.missing_values}
         number_of_missing_values = 0
 
         number_of_rows = len(column)
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_integrity/column_regexp_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_integrity/column_regexp_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.data_quality import get_rows_count
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import table_data
@@ -56,19 +57,20 @@
     column_name: str
     # the regular expression
     reg_exp: str
     top: int
     # compiled regular expression for speed optimization
     _reg_exp_compiled: Pattern
 
-    def __init__(self, column_name: str, reg_exp: str, top: int = 10):
+    def __init__(self, column_name: str, reg_exp: str, top: int = 10, options: AnyOptions = None):
         self.top = top
         self.reg_exp = reg_exp
         self.column_name = column_name
         self._reg_exp_compiled = re.compile(reg_exp)
+        super().__init__(options=options)
 
     def _calculate_stats_by_regexp(self, column: pd.Series) -> DataIntegrityValueByRegexpStat:
         number_of_matched = 0
         number_of_na = 0
         number_of_not_matched = 0
         table_of_matched: Dict[str, int] = collections.defaultdict(int)
         table_of_not_matched: Dict[str, int] = collections.defaultdict(int)
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_integrity/column_summary_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_integrity/column_summary_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,19 +97,22 @@
 class DataInTime(MetricResult):
     data_for_plots: Dict[str, Optional[pd.DataFrame]]
     freq: str
     datetime_name: str
 
 
 class DataByTarget(MetricResult):
+    class Config:
+        smart_union = True
+
     data_for_plots: Union[
         Dict[
             str,
             Union[
-                Dict[str, Union[list, pd.DataFrame, np.ndarray, pd.Categorical]],
+                Dict[str, pd.DataFrame],
                 pd.DataFrame,
             ],
         ],
         None,
         Dict[str, ContourData],
     ]
     target_name: str
@@ -136,67 +139,62 @@
 
     reference_characteristics: Optional[ColumnCharacteristics]
     current_characteristics: ColumnCharacteristics
     plot_data: DataQualityPlot
 
 
 class ColumnSummaryMetric(ColumnMetric[ColumnSummaryResult]):
-    generated_text_features: Optional[Dict[str, Union[TextLength, NonLetterCharacterPercentage, OOVWordsPercentage]]]
+    _generated_text_features: Optional[Dict[str, Union[TextLength, NonLetterCharacterPercentage, OOVWordsPercentage]]]
 
     def __init__(self, column_name: Union[str, ColumnName], options: AnyOptions = None):
-        super().__init__(options=options)
-        if isinstance(column_name, str):
-            self.column = ColumnName.main_dataset(column_name)
-        else:
-            self.column = column_name
-        self.column_name = self.column.name
-        self.generated_text_features = None
+        self._generated_text_features = None
+        super().__init__(column_name=column_name, options=options)
 
     def required_features(self, data_definition: DataDefinition):
-        if not self.column.is_main_dataset():
+        if not self.column_name.is_main_dataset():
             return ColumnMetric.required_features(self, data_definition)
-        column_type = data_definition.get_column(self.column_name).column_type
+        column_type = data_definition.get_column(self.column_name.name).column_type
         if column_type == ColumnType.Text:
-            self.generated_text_features = {
-                "text_length": TextLength(self.column_name),
-                "non_letter_char": NonLetterCharacterPercentage(self.column_name),
-                "oov": OOVWordsPercentage(self.column_name),
+            self._generated_text_features = {
+                "text_length": TextLength(self.column_name.name),
+                "non_letter_char": NonLetterCharacterPercentage(self.column_name.name),
+                "oov": OOVWordsPercentage(self.column_name.name),
             }
-            return list(self.generated_text_features.values())
+            return list(self._generated_text_features.values())
         return []
 
     def get_parameters(self) -> tuple:
         return (self.column_name,)
 
     @staticmethod
     def acceptable_types() -> List[ColumnType]:
         return [ColumnType.Numerical, ColumnType.Categorical, ColumnType.Text]
 
     def calculate(self, data: InputData) -> ColumnSummaryResult:
 
-        if not data.has_column(self.column):
-            raise ValueError(f"Column '{self.column.display_name}' not found in dataset.")
+        if not data.has_column(self.column_name):
+            raise ValueError(f"Column '{self.column_name.display_name}' not found in dataset.")
 
-        column_type, column_current_data, column_reference_data = data.get_data(self.column)
+        column_type, column_current_data, column_reference_data = data.get_data(self.column_name)
 
         curr_characteristics: ColumnCharacteristics
         ref_characteristics: Optional[ColumnCharacteristics] = None
-        if column_type == ColumnType.Text and self.generated_text_features is not None:
+        if column_type == ColumnType.Text and self._generated_text_features is not None:
             if column_reference_data is not None:
                 ref_characteristics = self.get_text_stats(
                     "reference",
                     data,
                     column_reference_data,
-                    self.generated_text_features,
+                    self._generated_text_features,
                 )
             curr_characteristics = self.get_text_stats(
                 "current",
                 data,
                 column_current_data,
-                self.generated_text_features,
+                self._generated_text_features,
             )
         else:
             if column_reference_data is not None:
                 ref_characteristics = self.map_data(get_features_stats(column_reference_data, column_type))
             curr_characteristics = self.map_data(get_features_stats(column_current_data, column_type))
 
             if column_reference_data is not None and column_type == ColumnType.Categorical:
@@ -214,34 +212,37 @@
                 curr_characteristics.new_in_current_values_count = new_in_current_values_count
                 curr_characteristics.unused_in_current_values_count = unused_in_current_values_count
 
         datetime_column = data.data_definition.get_datetime_column()
         datetime_data = None
         if (
             datetime_column is not None
-            and datetime_column.column_name != self.column.name
+            and datetime_column.column_name != self.column_name.name
             and column_type != ColumnType.Datetime
         ):
             datetime_type, datetime_current, datetime_reference = data.get_data(datetime_column.column_name)
             datetime_data = (datetime_column.column_name, datetime_type, datetime_current, datetime_reference)
 
         target_column = data.data_definition.get_target_column()
         target_data = None
         if (
             target_column is not None
-            and target_column.column_name != self.column.name
+            and target_column.column_name != self.column_name.name
             and column_type != ColumnType.Datetime
         ):
             target_type, target_current, target_reference = data.get_data(target_column.column_name)
             target_data = (target_column.column_name, target_type, target_current, target_reference)
         agg_data = True
         if self.get_options().render_options.raw_data:
             agg_data = False
+        column_current_data = column_current_data.replace([np.inf, -np.inf], np.nan)
+        if column_reference_data is not None:
+            column_reference_data = column_reference_data.replace([np.inf, -np.inf], np.nan)
         bins_for_hist, data_in_time, data_by_target = plot_data(
-            (self.column.display_name, column_type, column_current_data, column_reference_data),
+            (self.column_name.display_name, column_type, column_current_data, column_reference_data),
             datetime_data,
             target_data,
             agg_data,
         )
 
         counts_of_values = None
         if column_type in [ColumnType.Categorical, ColumnType.Numerical]:
@@ -251,15 +252,15 @@
             counts_of_values["current"] = current_counts.head(10)
             if column_reference_data is not None:
                 reference_counts = column_reference_data.value_counts(dropna=False).reset_index()
                 reference_counts.columns = ["x", "count"]
                 counts_of_values["reference"] = reference_counts.head(10)
 
         return ColumnSummaryResult(
-            column_name=self.column_name,
+            column_name=self.column_name.name,
             column_type=column_type.value,
             reference_characteristics=ref_characteristics,
             current_characteristics=curr_characteristics,
             plot_data=DataQualityPlot(
                 bins_for_hist=bins_for_hist,
                 data_in_time=data_in_time,
                 data_by_target=data_by_target,
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,58 @@
-import dataclasses
-from dataclasses import dataclass
 from typing import Any
+from typing import ClassVar
 from typing import Dict
+from typing import FrozenSet
 from typing import List
 from typing import Optional
+from typing import Union
 
 import numpy as np
 import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.data_quality import get_rows_count
+from evidently.core import pydantic_type_validator
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import HistogramData
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import histogram
 from evidently.renderers.html_widgets import table_data
 from evidently.renderers.html_widgets import widget_tabs
 
+NoneKey = type("NoneKey", tuple(), {})
+
+
+@pydantic_type_validator(NoneKey)
+def null_valudator(value):
+    if value is None or value == "null":
+        return None
+    raise ValueError("not a None")
+
+
+MissingValue = Union[np.float_, NoneKey, Any]  # type: ignore[valid-type]
+
 
 class DatasetMissingValues(MetricResult):
     """Statistics about missed values in a dataset"""
 
     # set of different missing values in the dataset
-    different_missing_values: Dict[Any, int]
+    different_missing_values: Dict[MissingValue, int]
     # number of different missing values in the dataset
     number_of_different_missing_values: int
     # set of different missing values for each column
-    different_missing_values_by_column: Dict[str, Dict[Any, int]]
+    different_missing_values_by_column: Dict[str, Dict[MissingValue, int]]
     # count of different missing values for each column
     number_of_different_missing_values_by_column: Dict[str, int]
     # count of missing values in all dataset
     number_of_missing_values: int
     # share of missing values in all dataset
     share_of_missing_values: float
     # count of missing values for each column
@@ -77,28 +92,32 @@
     Value `None` in the list means that Pandas null values will be included in the calculation.
 
     If `replace` parameter is False - add defaults to user's list.
     If `replace` parameter is True - use values from `missing_values` list only.
     """
 
     # default missing values list
-    DEFAULT_MISSING_VALUES = ["", np.inf, -np.inf, None]
-    missing_values: frozenset
+    DEFAULT_MISSING_VALUES: ClassVar = ["", np.inf, -np.inf, None]
+    missing_values: FrozenSet[MissingValue]
 
-    def __init__(self, missing_values: Optional[list] = None, replace: bool = True) -> None:
+    def __init__(self, missing_values: Optional[list] = None, replace: bool = True, options: AnyOptions = None) -> None:
+        _missing_values: list
         if missing_values is None:
             # use default missing values list if we have no user-defined values
-            missing_values = self.DEFAULT_MISSING_VALUES
+            _missing_values = self.DEFAULT_MISSING_VALUES
 
         elif not replace:
             # add default values to the user-defined list
-            missing_values = self.DEFAULT_MISSING_VALUES + missing_values
+            _missing_values = self.DEFAULT_MISSING_VALUES + missing_values
+        else:
+            _missing_values = missing_values
 
         # use frozenset because metrics parameters should be immutable/hashable for deduplication
-        self.missing_values = frozenset(missing_values)
+        self.missing_values = frozenset(_missing_values)
+        super().__init__(options=options)
 
     def _calculate_missing_values_stats(self, dataset: pd.DataFrame) -> DatasetMissingValues:
         different_missing_values = {value: 0 for value in self.missing_values}
         columns_with_missing_values = set()
         number_of_missing_values = 0
         number_of_missing_values_by_column: Dict[str, int] = {}
         different_missing_values_by_column: Dict[str, Dict[Any, int]] = {}
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_integrity/dataset_summary_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_integrity/dataset_summary_metric.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,61 @@
-import dataclasses
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Union
 
+import numpy as np
 import pandas as pd
 
 from evidently import ColumnMapping
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.data_integration import get_number_of_all_pandas_missed_values
 from evidently.calculations.data_integration import get_number_of_almost_constant_columns
 from evidently.calculations.data_integration import get_number_of_almost_duplicated_columns
 from evidently.calculations.data_integration import get_number_of_constant_columns
 from evidently.calculations.data_integration import get_number_of_duplicated_columns
 from evidently.calculations.data_integration import get_number_of_empty_columns
 from evidently.calculations.data_quality import get_rows_count
+from evidently.metric_results import Label
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
+from evidently.pydantic_utils import ExcludeNoneMixin
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import table_data
 from evidently.utils.data_operations import process_columns
 
 
+class NumpyDtype(ExcludeNoneMixin):
+    dtype: str
+    categories: Optional[List[str]] = None
+
+    @property
+    def type(self):
+        if self.dtype == "category":
+            return pd.CategoricalDtype(categories=self.categories)
+        return np.dtype(self.dtype)
+
+    @classmethod
+    def from_dtype(cls, dtype: np.dtype):
+        if isinstance(dtype, pd.CategoricalDtype):
+            return cls(dtype=dtype.name, categories=list(dtype.categories))
+        return cls(dtype=dtype.name)
+
+
 class DatasetSummary(MetricResult):
     """Columns information in a dataset"""
 
     class Config:
-        dict_exclude_fields = {"columns_type"}
-        pd_exclude_fields = {"columns_type"}
+        dict_exclude_fields = {"columns_type_data"}
+        pd_exclude_fields = {"columns_type_data"}
 
     target: Optional[str]
     prediction: Optional[Union[str, Sequence[str]]]
     date_column: Optional[str]
     id_column: Optional[str]
     number_of_columns: int
     number_of_rows: int
@@ -46,35 +67,45 @@
     number_of_constant_columns: int
     number_of_almost_constant_columns: int
     number_of_duplicated_columns: int
     number_of_almost_duplicated_columns: int
     number_of_empty_rows: int
     number_of_empty_columns: int
     number_of_duplicated_rows: int
-    columns_type: dict
+    columns_type_data: Dict[Label, NumpyDtype]
     nans_by_columns: dict
     number_uniques_by_columns: dict
 
+    @property
+    def columns_type(self) -> Dict[Label, np.dtype]:
+        return {k: v.type for k, v in self.columns_type_data.items()}
+
 
 class DatasetSummaryMetricResult(MetricResult):
     almost_duplicated_threshold: float
     current: DatasetSummary
     reference: Optional[DatasetSummary] = None
 
 
 class DatasetSummaryMetric(Metric[DatasetSummaryMetricResult]):
     """Common dataset(s) columns/features characteristics"""
 
     # threshold for calculating the number of almost duplicated columns
     almost_duplicated_threshold: float
     almost_constant_threshold: float
 
-    def __init__(self, almost_duplicated_threshold: float = 0.95, almost_constant_threshold: float = 0.95):
+    def __init__(
+        self,
+        almost_duplicated_threshold: float = 0.95,
+        almost_constant_threshold: float = 0.95,
+        options: AnyOptions = None,
+    ):
         self.almost_duplicated_threshold = almost_duplicated_threshold
         self.almost_constant_threshold = almost_constant_threshold
+        super().__init__(options=options)
 
     def _calculate_dataset_common_stats(self, dataset: pd.DataFrame, column_mapping: ColumnMapping) -> DatasetSummary:
         columns = process_columns(dataset, column_mapping)
         return DatasetSummary(
             target=columns.utility_columns.target,
             prediction=columns.utility_columns.prediction,
             date_column=columns.utility_columns.date,
@@ -93,15 +124,15 @@
             ),
             number_of_duplicated_columns=get_number_of_duplicated_columns(dataset),
             number_of_almost_duplicated_columns=get_number_of_almost_duplicated_columns(
                 dataset, self.almost_duplicated_threshold
             ),
             number_of_empty_rows=dataset.isna().all(1).sum(),
             number_of_duplicated_rows=dataset.duplicated().sum(),
-            columns_type=dict(dataset.dtypes.to_dict()),
+            columns_type_data={k: NumpyDtype.from_dtype(v) for k, v in dataset.dtypes.to_dict().items()},
             nans_by_columns=dataset.isna().sum().to_dict(),
             number_uniques_by_columns=dict(dataset.nunique().to_dict()),
         )
 
     def calculate(self, data: InputData) -> DatasetSummaryMetricResult:
         if self.almost_duplicated_threshold < 0.5 or self.almost_duplicated_threshold > 1:
             raise ValueError("Almost duplicated threshold should be in range [0.5, 1]")
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_quality/column_correlations_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_quality/column_correlations_metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.data_quality import calculate_category_correlation
 from evidently.calculations.data_quality import calculate_numerical_correlation
 from evidently.core import ColumnType
 from evidently.metric_results import ColumnCorrelations
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import get_histogram_for_distribution
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import widget_tabs
 from evidently.utils.data_preprocessing import DataDefinition
@@ -31,19 +32,17 @@
 
 class ColumnCorrelationsMetric(Metric[ColumnCorrelationsMetricResult]):
     """Calculates correlations between the selected column and all the other columns.
     In the current and reference (if presented) datasets"""
 
     column_name: ColumnName
 
-    def __init__(self, column_name: Union[str, ColumnName]) -> None:
-        if isinstance(column_name, ColumnName):
-            self.column_name = column_name
-        else:
-            self.column_name = ColumnName.main_dataset(column_name)
+    def __init__(self, column_name: Union[str, ColumnName], options: AnyOptions = None) -> None:
+        self.column_name = ColumnName.from_any(column_name)
+        super().__init__(options=options)
 
     @staticmethod
     def _calculate_correlation(
         column_name: ColumnName,
         column_data: pd.Series,
         dataset: pd.DataFrame,
         data_definition: DataDefinition,
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_quality/column_distribution_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_quality/column_distribution_metric.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from typing import List
 from typing import Optional
 from typing import Union
 
+import numpy as np
+
 from evidently.base_metric import ColumnName
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.core import ColumnType
 from evidently.metric_results import Distribution
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import WidgetSize
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import plotly_figure
 from evidently.renderers.render_utils import get_distribution_plot_figure
 from evidently.utils.visualizations import get_distribution_for_column
@@ -25,32 +28,30 @@
 
 
 class ColumnDistributionMetric(Metric[ColumnDistributionMetricResult]):
     """Calculates distribution for the column"""
 
     column_name: ColumnName
 
-    def __init__(self, column_name: Union[str, ColumnName]) -> None:
-        if isinstance(column_name, str):
-            self.column_name = ColumnName.main_dataset(column_name)
-        else:
-            self.column_name = column_name
+    def __init__(self, column_name: Union[str, ColumnName], options: AnyOptions = None) -> None:
+        self.column_name = ColumnName.from_any(column_name)
+        super().__init__(options=options)
 
     def calculate(self, data: InputData) -> ColumnDistributionMetricResult:
         if not data.has_column(self.column_name):
             raise ValueError(f"Column '{self.column_name.display_name}' was not found in data.")
 
         if not self.column_name.is_main_dataset():
             column_type = ColumnType.Numerical
         else:
             column_type = data.data_definition.get_column(self.column_name.name).column_type
-        current_column = data.get_current_column(self.column_name)
-        reference_column = None
-        if data.reference_data is not None:
-            reference_column = data.get_reference_column(self.column_name)
+        current_column = data.get_current_column(self.column_name).replace([np.inf, -np.inf], np.nan)
+        reference_column = data.get_reference_column(self.column_name)
+        if reference_column is not None:
+            reference_column = reference_column.replace([np.inf, -np.inf], np.nan)
         current, reference = get_distribution_for_column(
             column_type=column_type.value,
             current=current_column,
             reference=reference_column,
         )
 
         return ColumnDistributionMetricResult(
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_quality/column_quantile_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_quality/column_quantile_metric.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import List
 from typing import Optional
 from typing import Union
 
+import numpy as np
 import pandas as pd
 
 from evidently.base_metric import ColumnMetricResult
 from evidently.base_metric import ColumnName
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.core import ColumnType
 from evidently.metric_results import Distribution
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import HistogramData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import get_histogram_figure_with_quantile
 from evidently.renderers.html_widgets import header_text
@@ -36,59 +38,58 @@
     current: QuantileStats
     reference: Optional[QuantileStats] = None
 
 
 class ColumnQuantileMetric(Metric[ColumnQuantileMetricResult]):
     """Calculates quantile with specified range"""
 
-    column: ColumnName
+    column_name: ColumnName
     quantile: float
 
-    def __init__(self, column_name: Union[str, ColumnName], quantile: float) -> None:
+    def __init__(self, column_name: Union[str, ColumnName], quantile: float, options: AnyOptions = None) -> None:
         self.quantile = quantile
-        if isinstance(column_name, str):
-            self.column = ColumnName.main_dataset(column_name)
-        else:
-            self.column = column_name
+        self.column_name = ColumnName.from_any(column_name)
+        super().__init__(options=options)
 
     def calculate(self, data: InputData) -> ColumnQuantileMetricResult:
         if not 0 < self.quantile <= 1:
             raise ValueError("Quantile should all be in the interval (0, 1].")
 
-        if not data.has_column(self.column):
-            raise ValueError(f"Column '{self.column}' is not in data.")
+        if not data.has_column(self.column_name):
+            raise ValueError(f"Column '{self.column_name}' is not in data.")
 
-        column_type, current_column, reference_column = data.get_data(self.column)
+        column_type, current_column, reference_column = data.get_data(self.column_name)
 
         if not pd.api.types.is_numeric_dtype(current_column.dtype):
-            raise ValueError(f"Column '{self.column}' in current data is not numeric.")
+            raise ValueError(f"Column '{self.column_name}' in current data is not numeric.")
 
         current_quantile = current_column.quantile(self.quantile)
 
         if reference_column is not None:
             if not pd.api.types.is_numeric_dtype(reference_column.dtype):
-                raise ValueError(f"Column '{self.column}' in reference data is not numeric.")
+                raise ValueError(f"Column '{self.column_name}' in reference data is not numeric.")
 
             reference_quantile = reference_column.quantile(self.quantile)
+            reference_column = reference_column.replace([np.inf, -np.inf], np.nan)
 
         else:
             reference_column = None
             reference_quantile = None
 
         distributions = get_distribution_for_column(
-            column_type="num", current=current_column, reference=reference_column
+            column_type="num", current=current_column.replace([np.inf, -np.inf], np.nan), reference=reference_column
         )
         reference = None
         if reference_quantile is not None:
             reference = QuantileStats(
                 value=reference_quantile,
                 distribution=distributions[1],
             )
         return ColumnQuantileMetricResult(
-            column_name=self.column.display_name,
+            column_name=self.column_name.display_name,
             column_type=ColumnType.Numerical.value,
             current=QuantileStats(
                 value=current_quantile,
                 distribution=distributions[0],
             ),
             quantile=self.quantile,
             reference=reference,
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_quality/column_value_list_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_quality/column_value_list_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.data_quality import get_rows_count
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import table_data
@@ -39,17 +40,18 @@
 
 class ColumnValueListMetric(Metric[ColumnValueListMetricResult]):
     """Calculates count and shares of values in the predefined values list"""
 
     column_name: str
     values: Optional[list]
 
-    def __init__(self, column_name: str, values: Optional[list] = None) -> None:
+    def __init__(self, column_name: str, values: Optional[list] = None, options: AnyOptions = None) -> None:
         self.values = values
         self.column_name = column_name
+        super().__init__(options=options)
 
     @staticmethod
     def _calculate_stats(values: list, column: pd.Series) -> ValueListStat:
         rows_count = get_rows_count(column)
         values_in_list = {}
         values_not_in_list = {}
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_quality/column_value_range_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_quality/column_value_range_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.data_quality import get_rows_count
 from evidently.core import ColumnType
 from evidently.metric_results import Distribution
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import CounterData
 from evidently.renderers.html_widgets import HistogramData
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import counter
 from evidently.renderers.html_widgets import get_histogram_figure_with_range
@@ -45,27 +46,29 @@
     current: ValuesInRangeStat
     reference: Optional[ValuesInRangeStat] = None
 
 
 class ColumnValueRangeMetric(Metric[ColumnValueRangeMetricResult]):
     """Calculates count and shares of values in the predefined values range"""
 
-    column_name: Union[str, ColumnName]
+    column_name: ColumnName
     left: Optional[Numeric]
     right: Optional[Numeric]
 
     def __init__(
         self,
         column_name: Union[str, ColumnName],
         left: Optional[Numeric] = None,
         right: Optional[Numeric] = None,
+        options: AnyOptions = None,
     ) -> None:
         self.left = left
         self.right = right
-        self.column_name = column_name
+        self.column_name = ColumnName.from_any(column_name)
+        super().__init__(options=options)
 
     @staticmethod
     def _calculate_in_range_stats(
         column: pd.Series, left: Numeric, right: Numeric, distribution: Distribution
     ) -> ValuesInRangeStat:
         column = column.dropna()
         rows_count = get_rows_count(column)
@@ -115,16 +118,16 @@
 
         else:
             right = self.right
 
         # calculate distribution for visualisation
         cur_distribution, ref_distribution = get_distribution_for_column(
             column_type="num",
-            current=current_data,
-            reference=reference_data if reference_data is not None else None,
+            current=current_data.replace([np.inf, -np.inf], np.nan),
+            reference=reference_data.replace([np.inf, -np.inf], np.nan) if reference_data is not None else None,
         )
 
         current = self._calculate_in_range_stats(current_data, left, right, cur_distribution)
         reference = None
         if reference_data is not None:
             # always should be present
             assert ref_distribution is not None
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_quality/conflict_prediction_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_quality/conflict_prediction_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_quality/conflict_target_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_quality/conflict_target_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_quality/dataset_correlations_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_quality/dataset_correlations_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import copy
-import dataclasses
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
@@ -14,14 +13,15 @@
 from evidently.calculations.classification_performance import get_prediction_data
 from evidently.calculations.data_quality import calculate_correlations
 from evidently.core import ColumnType
 from evidently.features.non_letter_character_percentage_feature import NonLetterCharacterPercentage
 from evidently.features.OOV_words_percentage_feature import OOVWordsPercentage
 from evidently.features.text_length_feature import TextLength
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import HeatmapData
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import get_heatmaps_widget
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import widget_tabs
@@ -58,23 +58,24 @@
     reference: Optional[DatasetCorrelation]
     target_correlation: Optional[str]
 
 
 class DatasetCorrelationsMetric(Metric[DatasetCorrelationsMetricResult]):
     """Calculate different correlations with target, predictions and features"""
 
-    text_features_gen: Optional[
+    _text_features_gen: Optional[
         Dict[
             str,
             Dict[str, Union[TextLength, NonLetterCharacterPercentage, OOVWordsPercentage]],
         ]
     ]
 
-    def __init__(self):
-        self.text_features_gen = None
+    def __init__(self, options: AnyOptions = None):
+        self._text_features_gen = None
+        super().__init__(options=options)
 
     def required_features(self, data_definition: DataDefinition):
         if len(data_definition.get_columns("text_features")) > 0:
             text_cols = [col.column_name for col in data_definition.get_columns("text_features")]
             text_features_gen = {}
             text_features_gen_result = []
             for col in text_cols:
@@ -88,15 +89,15 @@
 
                 text_features_gen_result += [
                     col_dict[f"{col}: Text Length"],
                     col_dict[f"{col}: Non Letter Character %"],
                     col_dict[f"{col}: OOV %"],
                 ]
                 text_features_gen[col] = col_dict
-            self.text_features_gen = text_features_gen
+            self._text_features_gen = text_features_gen
 
             return text_features_gen_result
         else:
             return []
 
     def get_parameters(self) -> tuple:
         return ()
@@ -227,39 +228,39 @@
                 prediction_probas=prediction_data.prediction_probas,
                 predicted_values=ColumnDefinition(prediction_labels_name, target_type),
             )
             data_definition._columns[prediction_labels_name] = ColumnDefinition(prediction_labels_name, target_type)
 
         # process text columns
         text_columns = []
-        if self.text_features_gen is not None:
-            for col in list(self.text_features_gen.keys()):
+        if self._text_features_gen is not None:
+            for col in list(self._text_features_gen.keys()):
                 curr_text_df = pd.concat(
-                    [data.get_current_column(x.feature_name()) for x in list(self.text_features_gen[col].values())],
+                    [data.get_current_column(x.feature_name()) for x in list(self._text_features_gen[col].values())],
                     axis=1,
                 )
-                curr_text_df.columns = list(self.text_features_gen[col].keys())
+                curr_text_df.columns = list(self._text_features_gen[col].keys())
                 text_columns.append(list(curr_text_df.columns))
                 curr_df = pd.concat(
                     [
                         curr_df.copy().reset_index(drop=True),
                         curr_text_df.reset_index(drop=True),
                     ],
                     axis=1,
                 )
 
                 if ref_df is not None:
                     ref_text_df = pd.concat(
                         [
                             data.get_reference_column(x.feature_name())
-                            for x in list(self.text_features_gen[col].values())
+                            for x in list(self._text_features_gen[col].values())
                         ],
                         axis=1,
                     )
-                    ref_text_df.columns = list(self.text_features_gen[col].keys())
+                    ref_text_df.columns = list(self._text_features_gen[col].keys())
                     ref_df = pd.concat(
                         [
                             ref_df.copy().reset_index(drop=True),
                             ref_text_df.reset_index(drop=True),
                         ],
                         axis=1,
                     )
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_quality/stability_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_quality/stability_metric.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,37 +17,39 @@
     number_not_stable_prediction: Optional[int] = None
 
 
 class DataQualityStabilityMetric(Metric[DataQualityStabilityMetricResult]):
     """Calculates stability by target and prediction"""
 
     def calculate(self, data: InputData) -> DataQualityStabilityMetricResult:
-        result = DataQualityStabilityMetricResult()
         target_name = data.column_mapping.target
         prediction_name = data.column_mapping.prediction
         columns = [column for column in data.current_data.columns if column not in (target_name, prediction_name)]
 
         if not columns:
-            result.number_not_stable_target = 0
-            result.number_not_stable_prediction = 0
-            return result
+            return DataQualityStabilityMetricResult(number_not_stable_target=0, number_not_stable_prediction=0)
 
         duplicates = data.current_data[data.current_data.duplicated(subset=columns, keep=False)]
 
+        number_not_stable_target = None
+        number_not_stable_prediction = None
+
         if target_name in data.current_data:
-            result.number_not_stable_target = duplicates.drop(
+            number_not_stable_target = duplicates.drop(
                 data.current_data[data.current_data.duplicated(subset=columns + [target_name], keep=False)].index
             ).shape[0]
 
         if prediction_name in data.current_data:
-            result.number_not_stable_prediction = duplicates.drop(
+            number_not_stable_prediction = duplicates.drop(
                 data.current_data[data.current_data.duplicated(subset=columns + [prediction_name], keep=False)].index
             ).shape[0]
 
-        return result
+        return DataQualityStabilityMetricResult(
+            number_not_stable_target=number_not_stable_target, number_not_stable_prediction=number_not_stable_prediction
+        )
 
 
 @default_renderer(wrap_type=DataQualityStabilityMetric)
 class DataQualityStabilityMetricRenderer(MetricRenderer):
     def render_html(self, obj: DataQualityStabilityMetric) -> List[BaseWidgetInfo]:
         metric_result = obj.get_result()
         result = [
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py` & `evidently-0.3.3/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from evidently.descriptors import OOV
 from evidently.descriptors import NonLetterCharacterPercentage
 from evidently.descriptors import TextLength
 from evidently.features.generated_features import FeatureDescriptor
 from evidently.features.generated_features import GeneratedFeature
 from evidently.metric_results import ColumnCorrelations
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import TabData
 from evidently.renderers.html_widgets import get_histogram_for_distribution
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import widget_tabs
 from evidently.utils.data_preprocessing import DataDefinition
@@ -31,32 +32,40 @@
     reference: Optional[Dict[str, Dict[str, ColumnCorrelations]]] = None
 
 
 class TextDescriptorsCorrelationMetric(Metric[TextDescriptorsCorrelationMetricResult]):
     """Calculates correlations between each auto-generated text feature for column_name and other dataset columns"""
 
     column_name: str
-    generated_text_features: Dict[str, GeneratedFeature]
+    _generated_text_features: Dict[str, GeneratedFeature]
+    descriptors: Dict[str, FeatureDescriptor]
 
-    def __init__(self, column_name: str, descriptors: Optional[Dict[str, FeatureDescriptor]] = None) -> None:
+    def __init__(
+        self, column_name: str, descriptors: Optional[Dict[str, FeatureDescriptor]] = None, options: AnyOptions = None
+    ) -> None:
         self.column_name = column_name
         if descriptors:
             self.descriptors = descriptors
         else:
             self.descriptors = {
                 "Text Length": TextLength(),
                 "Non Letter Character %": NonLetterCharacterPercentage(),
                 "OOV %": OOV(),
             }
-        self.generated_text_features = {}
+        super().__init__(options=options)
+        self._generated_text_features = {}
+
+    @property
+    def generated_text_features(self):
+        return self._generated_text_features
 
     def required_features(self, data_definition: DataDefinition):
         column_type = data_definition.get_column(self.column_name).column_type
         if column_type == ColumnType_data.Text:
-            self.generated_text_features = {
+            self._generated_text_features = {
                 name: desc.feature(self.column_name) for name, desc in self.descriptors.items()
             }
             return list(self.generated_text_features.values())
         return []
 
     def get_parameters(self) -> tuple:
         return (self.column_name,)
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/data_quality/text_descriptors_distribution.py` & `evidently-0.3.3/src/evidently/metrics/data_quality/text_descriptors_distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from evidently.descriptors import OOV
 from evidently.descriptors import NonLetterCharacterPercentage
 from evidently.descriptors import TextLength
 from evidently.features.generated_features import FeatureDescriptor
 from evidently.features.generated_features import GeneratedFeature
 from evidently.metric_results import Distribution
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import WidgetSize
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import plotly_figure
 from evidently.renderers.render_utils import get_distribution_plot_figure
 from evidently.utils.data_operations import process_columns
@@ -31,32 +32,40 @@
     reference: Optional[Dict[str, Distribution]] = None
 
 
 class TextDescriptorsDistribution(Metric[TextDescriptorsDistributionResult]):
     """Calculates distribution for the column"""
 
     column_name: str
-    generated_text_features: Dict[str, GeneratedFeature]
+    _generated_text_features: Dict[str, GeneratedFeature]
+    descriptors: Dict[str, FeatureDescriptor]
 
-    def __init__(self, column_name: str, descriptors: Optional[Dict[str, FeatureDescriptor]] = None) -> None:
+    def __init__(
+        self, column_name: str, descriptors: Optional[Dict[str, FeatureDescriptor]] = None, options: AnyOptions = None
+    ) -> None:
         self.column_name = column_name
         if descriptors:
             self.descriptors = descriptors
         else:
             self.descriptors = {
                 "Text Length": TextLength(),
                 "Non Letter Character %": NonLetterCharacterPercentage(),
                 "OOV %": OOV(),
             }
-        self.generated_text_features = {}
+        super().__init__(options=options)
+        self._generated_text_features = {}
+
+    @property
+    def generated_text_features(self):
+        return self._generated_text_features
 
     def required_features(self, data_definition: DataDefinition):
         column_type = data_definition.get_column(self.column_name).column_type
         if column_type == ColumnType.Text:
-            self.generated_text_features = {
+            self._generated_text_features = {
                 name: desc.feature(self.column_name) for name, desc in self.descriptors.items()
             }
             return list(self.generated_text_features.values())
         return []
 
     def get_parameters(self) -> tuple:
         return (self.column_name,)
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py` & `evidently-0.3.3/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 from typing import Union
 
 import numpy as np
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
-from evidently.base_metric import MetricResult
+from evidently.metric_results import ColumnAggScatterResult
 from evidently.metric_results import ColumnScatter
 from evidently.metric_results import ColumnScatterResult
 from evidently.model.widget import BaseWidgetInfo
 from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import header_text
@@ -43,15 +43,16 @@
         if ref_df is not None:
             ref_df = self._make_df_for_plot(ref_df.copy(), target_name, prediction_name, datetime_column_name)
             ref_df["Absolute Percentage Error"] = (
                 100 * np.abs(ref_df[prediction_name] - ref_df[target_name]) / ref_df[target_name]
             )
             ref_df.dropna(axis=0, how="any", inplace=True, subset=["Absolute Percentage Error"])
         reference_scatter: Optional[Union[ColumnScatter, dict]] = None
-        if self.get_options().render_options.raw_data:
+        raw_data = self.get_options().render_options.raw_data
+        if raw_data:
             current_scatter = {}
             current_scatter["Absolute Percentage Error"] = curr_df["Absolute Percentage Error"]
             if datetime_column_name is not None:
                 current_scatter["x"] = curr_df[datetime_column_name]
                 x_name = "Timestamp"
             else:
                 current_scatter["x"] = curr_df.index
@@ -81,15 +82,19 @@
                 x_name_ref = "Index binned"
             else:
                 x_name_ref = datetime_column_name + f" ({prefix_ref})"
         if datetime_column_name is None:
             x_name = "Index binned"
         else:
             x_name = datetime_column_name + f" ({prefix})"
-        return ColumnScatterResult(
+        cls = ColumnScatterResult
+        if not raw_data:
+            cls = ColumnAggScatterResult
+
+        return cls(
             current=current_scatter,
             reference=reference_scatter,
             x_name=x_name,
             x_name_ref=x_name_ref,
         )
 
     def _make_df_for_plot(self, df, target_name: str, prediction_name: str, datetime_column_name: Optional[str]):
@@ -128,14 +133,15 @@
                 curr_data=current,
                 ref_data=reference,
                 line=0,
                 std=None,
                 xaxis_name=result.x_name,
                 xaxis_name_ref=result.x_name_ref,
                 yaxis_name="Percent",
+                color_options=self.color_options,
             )
         return [
             header_text(label="Absolute Percentage Error"),
             BaseWidgetInfo(
                 title="",
                 size=2,
                 type="big_graph",
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_bias_table.py` & `evidently-0.3.3/src/evidently/metrics/regression_performance/error_bias_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import json
+from typing import ClassVar
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
@@ -44,39 +45,39 @@
     cat_feature_names: List[str]
     error_bias: Optional[dict] = None
     columns: Optional[List[str]] = None
 
 
 class RegressionErrorBiasTable(Metric[RegressionErrorBiasTableResults]):
     # by default, we get 5% values for the error bias calculations
-    TOP_ERROR_DEFAULT = 0.05
-    TOP_ERROR_MIN = 0
-    TOP_ERROR_MAX = 0.5
+    TOP_ERROR_DEFAULT: ClassVar[float] = 0.05
+    TOP_ERROR_MIN: ClassVar[float] = 0
+    TOP_ERROR_MAX: ClassVar[float] = 0.5
     top_error: float
     columns: Optional[List[str]]
     descriptors: Optional[Dict[str, Dict[str, FeatureDescriptor]]]
-    text_features_gen: Optional[Dict[str, Dict[str, GeneratedFeature]]]
+    _text_features_gen: Optional[Dict[str, Dict[str, GeneratedFeature]]]
 
     def __init__(
         self,
         columns: Optional[List[str]] = None,
         top_error: Optional[float] = None,
         descriptors: Optional[Dict[str, Dict[str, FeatureDescriptor]]] = None,
         options: AnyOptions = None,
     ):
-        super().__init__(options=options)
         if top_error is None:
             self.top_error = self.TOP_ERROR_DEFAULT
 
         else:
             self.top_error = top_error
 
         self.columns = columns
-        self.text_features_gen = None
+        self._text_features_gen = None
         self.descriptors = descriptors
+        super().__init__(options=options)
 
     def required_features(self, data_definition: DataDefinition):
         if len(data_definition.get_columns("text_features")) > 0:
             text_cols = [col.column_name for col in data_definition.get_columns("text_features")]
             text_features_gen = {}
             text_features_gen_result = []
             for col in text_cols:
@@ -90,15 +91,15 @@
                     }
                 else:
                     column_descriptors = self.descriptors[col]
                     col_dict = {f"{col}: " + name: value.feature(col) for name, value in column_descriptors.items()}
 
                 text_features_gen_result += list(col_dict.values())
                 text_features_gen[col] = col_dict
-            self.text_features_gen = text_features_gen
+            self._text_features_gen = text_features_gen
 
             return text_features_gen_result
         else:
             return []
 
     def get_parameters(self) -> tuple:
         return ()
@@ -146,16 +147,16 @@
 
         else:
             columns = self.columns
 
         num_feature_names = list(np.intersect1d(dataset_columns.num_feature_names, columns))
         cat_feature_names = list(np.intersect1d(dataset_columns.cat_feature_names, columns))
         # process text columns
-        if self.text_features_gen is not None:
-            for column, features in self.text_features_gen.items():
+        if self._text_features_gen is not None:
+            for column, features in self._text_features_gen.items():
                 columns.remove(column)
                 num_feature_names += list(features.keys())
                 columns += list(features.keys())
                 curr_text_df = pd.concat([data.get_current_column(x.feature_name()) for x in features.values()], axis=1)
                 curr_text_df.columns = list(features.keys())
                 curr_df = pd.concat([curr_df.reset_index(drop=True), curr_text_df.reset_index(drop=True)], axis=1)
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_distribution.py` & `evidently-0.3.3/src/evidently/metrics/regression_performance/error_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import dataclasses
 from typing import List
 from typing import Optional
 
 import numpy as np
-import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.metric_results import HistogramData
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_in_time.py` & `evidently-0.3.3/src/evidently/metrics/regression_performance/error_in_time.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import dataclasses
-from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
+from evidently.metric_results import ColumnAggScatterResult
 from evidently.metric_results import ColumnScatter
 from evidently.metric_results import ColumnScatterResult
 from evidently.model.widget import BaseWidgetInfo
 from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import header_text
@@ -41,15 +40,16 @@
         curr_error = curr_df[prediction_name] - curr_df[target_name]
         ref_error: Optional[pd.Series] = None
         if ref_df is not None:
             ref_df = self._make_df_for_plot(ref_df.copy(), target_name, prediction_name, datetime_column_name)
             ref_error = ref_df[prediction_name] - ref_df[target_name]
         current_scatter = {}
         reference_scatter: Optional[Union[dict, ColumnScatter]] = None
-        if self.get_options().render_options.raw_data:
+        raw_data = self.get_options().render_options.raw_data
+        if raw_data:
             current_scatter["Predicted - Actual"] = curr_error
             if datetime_column_name is not None:
                 current_scatter["x"] = curr_df[datetime_column_name]
                 x_name = "Timestamp"
             else:
                 current_scatter["x"] = curr_df.index
                 x_name = "Index"
@@ -77,15 +77,19 @@
                 x_name_ref = "Index binned"
             else:
                 x_name_ref = datetime_column_name + f" ({prefix_ref})"
         if datetime_column_name is None:
             x_name = "Index binned"
         else:
             x_name = datetime_column_name + f" ({prefix})"
-        return ColumnScatterResult(
+        cls = ColumnScatterResult
+        if not raw_data:
+            cls = ColumnAggScatterResult
+
+        return cls(
             current=current_scatter,
             reference=reference_scatter,
             x_name=x_name,
             x_name_ref=x_name_ref,
         )
 
     def _make_df_for_plot(self, df, target_name: str, prediction_name: str, datetime_column_name: Optional[str]):
@@ -125,14 +129,15 @@
                 curr_data=current,
                 ref_data=reference,
                 line=0,
                 std=None,
                 xaxis_name=result.x_name,
                 xaxis_name_ref=result.x_name_ref,
                 yaxis_name="Error",
+                color_options=self.color_options,
             )
         return [
             header_text(label="Error (Predicted - Actual)"),
             BaseWidgetInfo(
                 title="",
                 size=2,
                 type="big_graph",
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_normality.py` & `evidently-0.3.3/src/evidently/metrics/regression_performance/error_normality.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 from typing import Any
 from typing import List
 from typing import Optional
-from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from plotly import graph_objs as go
 from plotly.subplots import make_subplots
 from scipy.stats import probplot
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py` & `evidently-0.3.3/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-import dataclasses
-from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
-import pandas as pd
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
-from evidently.base_metric import MetricResult
-from evidently.core import IncludeTags
+from evidently.metric_results import ColumnAggScatterResult
 from evidently.metric_results import ColumnScatter
 from evidently.metric_results import ColumnScatterResult
-from evidently.metric_results import raw_agg_properties
 from evidently.model.widget import BaseWidgetInfo
 from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import header_text
 from evidently.utils.data_operations import process_columns
 from evidently.utils.visualizations import plot_agg_line_data
@@ -40,15 +35,16 @@
             raise ValueError("The columns 'target' and 'prediction' columns should be present")
         if not isinstance(prediction_name, str):
             raise ValueError("Expect one column for prediction. List of columns was provided.")
         curr_df = self._make_df_for_plot(curr_df, target_name, prediction_name, datetime_column_name)
         if ref_df is not None:
             ref_df = self._make_df_for_plot(ref_df.copy(), target_name, prediction_name, datetime_column_name)
         reference_scatter: Optional[Union[dict, ColumnScatter]] = None
-        if self.get_options().render_options.raw_data:
+        raw_data = self.get_options().render_options.raw_data
+        if raw_data:
             current_scatter = {}
             current_scatter["Predicted"] = curr_df[prediction_name]
             current_scatter["Actual"] = curr_df[target_name]
             if datetime_column_name is not None:
                 current_scatter["x"] = curr_df[datetime_column_name]
                 x_name = "Timestamp"
             else:
@@ -78,15 +74,18 @@
                 x_name_ref = "Index binned"
             else:
                 x_name_ref = datetime_column_name + f" ({prefix_ref})"
         if datetime_column_name is None:
             x_name = "Index binned"
         else:
             x_name = datetime_column_name + f" ({prefix})"
-        return ColumnScatterResult(
+        cls = ColumnScatterResult
+        if not raw_data:
+            cls = ColumnAggScatterResult
+        return cls(
             current=current_scatter,
             reference=reference_scatter,
             x_name=x_name,
             x_name_ref=x_name_ref,
         )
 
     def _make_df_for_plot(self, df, target_name: str, prediction_name: str, datetime_column_name: Optional[str]):
@@ -131,14 +130,15 @@
             curr_data=current,
             ref_data=reference,
             line=0,
             std=None,
             xaxis_name=x_name,
             xaxis_name_ref=x_name_ref,
             yaxis_name="Value",
+            color_options=self.color_options,
         )
         return [
             header_text(label="Predicted vs Actual in Time"),
             BaseWidgetInfo(
                 title="",
                 size=2,
                 type="big_graph",
@@ -172,14 +172,15 @@
             curr_data=current,
             ref_data=reference,
             line=0,
             std=None,
             xaxis_name=result.x_name,
             xaxis_name_ref=result.x_name_ref,
             yaxis_name="Value",
+            color_options=self.color_options,
         )
         return [
             header_text(label="Predicted vs Actual in Time"),
             BaseWidgetInfo(
                 title="",
                 size=2,
                 type="big_graph",
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/regression_performance/predicted_vs_actual.py` & `evidently-0.3.3/src/evidently/metrics/regression_performance/predicted_vs_actual.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/metrics/regression_performance/regression_dummy_metric.py` & `evidently-0.3.3/src/evidently/metrics/regression_performance/regression_dummy_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import dataclasses
 from typing import List
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 from sklearn.metrics import mean_absolute_error
 from sklearn.metrics import mean_absolute_percentage_error
 from sklearn.metrics import mean_squared_error
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.metrics.regression_performance.regression_quality import RegressionQualityMetric
 from evidently.model.widget import BaseWidgetInfo
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import table_data
 from evidently.utils.data_operations import process_columns
 
 
@@ -32,18 +32,23 @@
     rmse_by_ref: Optional[float] = None
     rmse: Optional[float] = None
     abs_error_max_by_ref: Optional[float] = None
     abs_error_max: Optional[float] = None
 
 
 class RegressionDummyMetric(Metric[RegressionDummyMetricResults]):
-    quality_metric: RegressionQualityMetric
+    _quality_metric: RegressionQualityMetric
 
-    def __init__(self):
-        self.quality_metric = RegressionQualityMetric()
+    def __init__(self, options: AnyOptions = None):
+        super().__init__(options=options)
+        self._quality_metric = RegressionQualityMetric()
+
+    @property
+    def quality_metric(self):
+        return self._quality_metric
 
     def calculate(self, data: InputData) -> RegressionDummyMetricResults:
         quality_metric: Optional[RegressionQualityMetric]
         dataset_columns = process_columns(data.current_data, data.column_mapping)
         target_name = dataset_columns.utility_columns.target
         prediction_name = dataset_columns.utility_columns.prediction
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/regression_performance/regression_performance_metrics.py` & `evidently-0.3.3/src/evidently/metrics/regression_performance/regression_performance_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Dict
 from typing import List
 from typing import Optional
-from typing import Union
 
 import numpy as np
-import pandas as pd
 from sklearn.metrics import mean_absolute_error
 from sklearn.metrics import mean_absolute_percentage_error
 from sklearn.metrics import mean_squared_error
 from sklearn.metrics import r2_score
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/regression_performance/regression_quality.py` & `evidently-0.3.3/src/evidently/metrics/regression_performance/regression_quality.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import dataclasses
 from typing import Dict
 from typing import List
 from typing import Optional
-from typing import Union
 
 import numpy as np
-import pandas as pd
 from sklearn.metrics import mean_absolute_error
 from sklearn.metrics import mean_absolute_percentage_error
 from sklearn.metrics import mean_squared_error
 from sklearn.metrics import r2_score
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/regression_performance/top_error.py` & `evidently-0.3.3/src/evidently/metrics/regression_performance/top_error.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/metrics/regression_performance/utils.py` & `evidently-0.3.3/src/evidently/metrics/regression_performance/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,26 @@
+from evidently.metrics.regression_performance.objects import IntervalSeries
 from evidently.metrics.regression_performance.objects import RegressionMetricScatter
 
 
 def apply_func_to_binned_data(
     df_for_bins, func, target_column, preds_column, is_ref_data=False
 ) -> RegressionMetricScatter:
     def _apply(x):
         if x.shape[0] == 0:
             return None
         return func(x[target_column], x[preds_column])
 
+    reference = None
+    if is_ref_data:
+        reference = IntervalSeries.from_data(
+            df_for_bins[df_for_bins.data == "ref"].groupby("target_binned").apply(_apply)
+        )
+
     result = RegressionMetricScatter(
-        current=df_for_bins[df_for_bins.data == "curr"].groupby("target_binned").apply(_apply)
+        current=IntervalSeries.from_data(
+            df_for_bins[df_for_bins.data == "curr"].groupby("target_binned").apply(_apply)
+        ),
+        reference=reference,
     )
 
-    if is_ref_data:
-        result.reference = df_for_bins[df_for_bins.data == "ref"].groupby("target_binned").apply(_apply)
     return result
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/regression_performance/visualization.py` & `evidently-0.3.3/src/evidently/metrics/regression_performance/visualization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import json
-from typing import Dict
 from typing import Optional
 from typing import Union
 
 import numpy as np
-import pandas as pd
 from plotly import graph_objs as go
 from plotly.subplots import make_subplots
 
 from evidently.metric_results import Histogram
 from evidently.metrics.regression_performance.objects import RegressionMetricScatter
 from evidently.metrics.regression_performance.objects import RegressionScatter
 from evidently.options.color_scheme import ColorOptions
@@ -81,32 +79,29 @@
     curr_metric: float,
     ref_metric: float = None,
     color_options: ColorOptions,
 ):
     current_color = color_options.get_current_data_color()
     reference_color = color_options.get_reference_data_color()
     fig = make_subplots(rows=2, cols=1, shared_xaxes=True)
-    # todo: better typing
-    assert isinstance(val_for_plot.current, pd.Series)
-    sorted_index = val_for_plot.current.sort_index()
+    sorted_index = val_for_plot.current.data.sort_index()
     x = [str(idx) for idx in sorted_index.index]
     y = list(sorted_index)
     trace = go.Scatter(x=x, y=y, mode="lines+markers", name=name, marker_color=current_color)
     fig.add_trace(trace, 1, 1)
 
     df = hist_for_plot.current.to_df().sort_values("x")
     x = [str(x) for x in df.x]
     y = list(df["count"])
     trace = go.Bar(name="current", x=x, y=y, marker_color=current_color)
     fig.add_trace(trace, 2, 1)
 
     if hist_for_plot.reference is not None:
-        # todo: better typing
-        assert isinstance(val_for_plot.reference, pd.Series)
-        sorted_index = val_for_plot.reference.sort_index()
+        assert val_for_plot.reference is not None
+        sorted_index = val_for_plot.reference.data.sort_index()
         x = [str(idx) for idx in sorted_index.index]
         y = list(sorted_index)
         trace = go.Scatter(x=x, y=y, mode="lines+markers", name=name, marker_color=reference_color)
         fig.add_trace(trace, 1, 1)
 
         df = hist_for_plot.reference.to_df().sort_values("x")
         x = [str(x) for x in df.x]
```

### Comparing `evidently-0.3.2.1/src/evidently/metrics/utils.py` & `evidently-0.3.3/src/evidently/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/model/widget.py` & `evidently-0.3.3/src/evidently/model/widget.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/nbextension/static/index.js` & `evidently-0.3.3/src/evidently/nbextension/static/index.js`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/nbextension/static/index.js.LICENSE.txt` & `evidently-0.3.3/src/evidently/nbextension/static/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/nbextension/static/material-ui-icons.woff2` & `evidently-0.3.3/src/evidently/nbextension/static/material-ui-icons.woff2`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/options/base.py` & `evidently-0.3.3/src/evidently/options/base.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/options/color_scheme.py` & `evidently-0.3.3/src/evidently/options/color_scheme.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/options/data_drift.py` & `evidently-0.3.3/src/evidently/options/data_drift.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import warnings
-from dataclasses import dataclass
+from typing import ClassVar
 from typing import Dict
 from typing import Optional
 from typing import Union
 
+from pydantic import BaseModel
+
 from evidently.calculations.stattests import PossibleStatTestType
 from evidently.calculations.stattests import StatTest
 from evidently.utils.data_drift_utils import resolve_stattest_threshold
 
-DEFAULT_NBINSX = 10
-
 
-@dataclass
-class DataDriftOptions:
+class DataDriftOptions(BaseModel):
     """Configuration for Data Drift calculations.
 
     Args:
         confidence: Defines the confidence level for statistical tests.
                     Applies to all features (if passed as float) or certain features (if passed as dictionary).
                     (Deprecated) Use `threshold` to define confidence level for statistical
                     tests as more universal solution.
@@ -37,14 +36,16 @@
                                for numerical features only.
         per_feature_stattest: Defines a custom statistical test for drift detection in the Data Drift report
                               per feature.
         cat_target_stattest_func: Defines a custom statistical test to detect target drift in category target.
         num_target_stattest_func: Defines a custom statistical test to detect target drift in numeric target.
     """
 
+    DEFAULT_NBINSX: ClassVar = 10
+
     confidence: Optional[Union[float, Dict[str, float]]] = None
     threshold: Optional[Union[float, Dict[str, float]]] = None
     drift_share: float = 0.5
     nbinsx: Union[int, Dict[str, int]] = DEFAULT_NBINSX
     xbins: Optional[Dict[str, int]] = None
 
     feature_stattest_func: Optional[Union[PossibleStatTestType, Dict[str, PossibleStatTestType]]] = None
@@ -121,15 +122,15 @@
 
         return threshold
 
     def get_nbinsx(self, feature_name: str) -> int:
         if isinstance(self.nbinsx, int):
             return self.nbinsx
         if isinstance(self.nbinsx, dict):
-            return self.nbinsx.get(feature_name, DEFAULT_NBINSX)
+            return self.nbinsx.get(feature_name, DataDriftOptions.DEFAULT_NBINSX)
         raise ValueError(f"DataDriftOptions.nbinsx is incorrect type {type(self.nbinsx)}")
 
     def get_feature_stattest_func(self, feature_name: str, feature_type: str) -> Optional[PossibleStatTestType]:
         if self.feature_stattest_func is not None and any(
             [
                 self.all_features_stattest,
                 self.cat_features_stattest,
```

### Comparing `evidently-0.3.2.1/src/evidently/options/quality_metrics.py` & `evidently-0.3.3/src/evidently/options/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/pipeline/column_mapping.py` & `evidently-0.3.3/src/evidently/pipeline/column_mapping.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/renderers/base_renderer.py` & `evidently-0.3.3/src/evidently/renderers/base_renderer.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/renderers/html_widgets.py` & `evidently-0.3.3/src/evidently/renderers/html_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -917,7 +917,18 @@
             for trace in traces:
                 fig.add_trace(trace, 1, 2)
 
         fig.update_layout(yaxis_title="Probability", showlegend=False)
 
         additional_plots.append((str(label), plotly_figure(title="", figure=fig)))
     return additional_plots
+
+
+def text_widget(*, text: str, title: str = "", size: WidgetSize = WidgetSize.FULL):
+    """
+    generate widget with markdown text
+    Args:
+        text: markdown formatted text
+        title: widget title
+        size: widget size
+    """
+    return BaseWidgetInfo(title=title, type="text", size=size.value, params={"text": text})
```

### Comparing `evidently-0.3.2.1/src/evidently/renderers/notebook_utils.py` & `evidently-0.3.3/src/evidently/renderers/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/renderers/render_utils.py` & `evidently-0.3.3/src/evidently/renderers/render_utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/report/report.py` & `evidently-0.3.3/src/evidently/report/report.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 from collections import defaultdict
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
+from pydantic import BaseModel
+from pydantic import parse_obj_as
 
 from evidently import ColumnMapping
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.core import IncludeOptions
 from evidently.metric_preset.metric_preset import MetricPreset
 from evidently.metric_results import DatasetColumns
 from evidently.model.dashboard import DashboardInfo
 from evidently.model.widget import AdditionalGraphInfo
 from evidently.options.base import AnyOptions
+from evidently.options.base import Options
 from evidently.renderers.base_renderer import DetailsInfo
+from evidently.suite.base_suite import ContextPayload
 from evidently.suite.base_suite import Display
 from evidently.suite.base_suite import Suite
 from evidently.suite.base_suite import find_metric_renderer
 from evidently.utils.data_operations import process_columns
 from evidently.utils.data_preprocessing import create_data_definition
 from evidently.utils.generators import BaseGenerator
 
@@ -180,7 +184,33 @@
             "evidently_dashboard_" + str(uuid.uuid4()).replace("-", ""),
             DashboardInfo("Report", widgets=[result for result in metrics_results]),
             {
                 f"{item.id}": dataclasses.asdict(item.info) if dataclasses.is_dataclass(item.info) else item.info
                 for item in additional_graphs
             },
         )
+
+    def _get_payload(self) -> BaseModel:
+        ctx = self._inner_suite.context
+        suite = ContextPayload.from_context(ctx)
+        return _ReportPayload(
+            suite=suite, metrics_ids=[suite.metrics.index(m) for m in self._first_level_metrics], options=self.options
+        )
+
+    @classmethod
+    def _parse_payload(cls, payload: Dict) -> "Report":
+        return parse_obj_as(_ReportPayload, payload).load()
+
+
+class _ReportPayload(BaseModel):
+    suite: ContextPayload
+    metrics_ids: List[int]
+    options: Options
+
+    def load(self):
+        ctx = self.suite.to_context()
+        metrics = [ctx.metrics[i] for i in self.metrics_ids]
+        report = Report(metrics=metrics, options=self.options)
+        report._first_level_metrics = metrics
+        report._inner_suite.context = ctx
+
+        return report
```

### Comparing `evidently-0.3.2.1/src/evidently/runner/loader.py` & `evidently-0.3.3/src/evidently/runner/loader.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/runner/runner.py` & `evidently-0.3.3/src/evidently/runner/runner.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/suite/base_suite.py` & `evidently-0.3.3/src/evidently/suite/base_suite.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 import logging
 from datetime import datetime
 from typing import Dict
 from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Tuple
+from typing import Type
+from typing import TypeVar
 from typing import Union
 
 import pandas as pd
+from pydantic import BaseModel
 
 import evidently
 from evidently.base_metric import ErrorResult
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.core import IncludeOptions
 from evidently.options.base import AnyOptions
 from evidently.options.base import Options
-from evidently.options.option import Option
 from evidently.renderers.base_renderer import DEFAULT_RENDERERS
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import RenderersDefinitions
 from evidently.renderers.base_renderer import TestRenderer
 from evidently.renderers.notebook_utils import determine_template
 from evidently.suite.execution_graph import ExecutionGraph
 from evidently.suite.execution_graph import SimpleExecutionGraph
@@ -71,14 +73,17 @@
         return predefined
     if renderers.default_html_metric_renderer:
         return renderers.default_html_metric_renderer
     raise KeyError(f"No renderer found for {obj}")
 
 
 def _discover_dependencies(test: Union[Metric, Test]) -> Iterator[Tuple[str, Union[Metric, Test]]]:
+    if hasattr(test, "__evidently_dependencies__"):
+        yield from test.__evidently_dependencies__()  # type: ignore[union-attr]
+        return
     for field_name, field in test.__dict__.items():
         if issubclass(type(field), (Metric, Test)):
             yield field_name, field
 
 
 @dataclasses.dataclass
 class Context:
@@ -90,18 +95,60 @@
     metric_results: Dict[Metric, MetricResult]
     test_results: Dict[Test, TestResult]
     state: State
     renderers: RenderersDefinitions
     options: Options = Options()
 
 
+class ContextPayload(BaseModel):
+    metrics: List[Metric]
+    metric_results: List[MetricResult]
+    tests: List[Test]
+    test_results: List[TestResult]
+    options: Options = Options()
+
+    @classmethod
+    def from_context(cls, context: Context):
+        return cls(
+            metrics=list(context.metric_results.keys()),
+            metric_results=list(context.metric_results.values()),
+            tests=list(context.test_results.keys()),
+            test_results=list(context.test_results.values()),
+            options=context.options,
+        )
+
+    def to_context(self) -> Context:
+        ctx = Context(
+            None,
+            metrics=self.metrics,
+            tests=self.tests,
+            metric_results={m: mr for m, mr in zip(self.metrics, self.metric_results)},
+            test_results={t: tr for t, tr in zip(self.tests, self.test_results)},
+            state=States.Calculated,
+            renderers=DEFAULT_RENDERERS,
+            options=self.options,
+        )
+        for m in ctx.metrics:
+            m.set_context(ctx)
+            for _, dep in _discover_dependencies(m):
+                dep.set_context(ctx)
+        for t in ctx.tests:
+            t.set_context(ctx)
+            for _, dep in _discover_dependencies(t):
+                dep.set_context(ctx)
+        return ctx
+
+
 class ExecutionError(Exception):
     pass
 
 
+T = TypeVar("T", bound="Display")
+
+
 class Display:
     # collection of all possible common options
     options: Options
 
     def __init__(self, options: AnyOptions = None):
         self.options = Options.from_any_options(options)
 
@@ -214,14 +261,36 @@
                 out_file,
                 cls=NumpyEncoder,
             )
 
     def _render(self, temple_func, template_params: TemplateParams):
         return temple_func(params=template_params)
 
+    @abc.abstractmethod
+    def _get_payload(self) -> BaseModel:
+        raise NotImplementedError
+
+    @classmethod
+    @abc.abstractmethod
+    def _parse_payload(cls: Type[T], payload: Dict) -> T:
+        raise NotImplementedError
+
+    def _save(self, filename):
+        """Save state to file (experimental)"""
+        payload = self._get_payload()
+
+        with open(filename, "w") as f:
+            json.dump(payload.dict(), f, indent=2, cls=NumpyEncoder)
+
+    @classmethod
+    def _load(cls: Type[T], filename) -> T:
+        """Load state from file (experimental)"""
+        with open(filename, "r") as f:
+            return cls._parse_payload(json.load(f))
+
 
 class Suite:
     context: Context
 
     def __init__(self, options: Options):
         self.context = Context(
             execution_graph=None,
```

### Comparing `evidently-0.3.2.1/src/evidently/suite/execution_graph.py` & `evidently-0.3.3/src/evidently/suite/execution_graph.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/telemetry/sender.py` & `evidently-0.3.3/src/evidently/telemetry/sender.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/test_preset/__init__.py` & `evidently-0.3.3/src/evidently/test_preset/__init__.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/test_preset/classification_binary.py` & `evidently-0.3.3/src/evidently/test_preset/classification_binary.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/test_preset/classification_binary_topk.py` & `evidently-0.3.3/src/evidently/test_preset/classification_binary_topk.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/test_preset/classification_multiclass.py` & `evidently-0.3.3/src/evidently/test_preset/classification_multiclass.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/test_preset/data_drift.py` & `evidently-0.3.3/src/evidently/test_preset/data_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/test_preset/data_quality.py` & `evidently-0.3.3/src/evidently/test_preset/data_quality.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/test_preset/data_stability.py` & `evidently-0.3.3/src/evidently/test_preset/data_stability.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/test_preset/no_target_performance.py` & `evidently-0.3.3/src/evidently/test_preset/no_target_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/test_preset/regression.py` & `evidently-0.3.3/src/evidently/test_preset/regression.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/test_suite/test_suite.py` & `evidently-0.3.3/src/evidently/test_suite/test_suite.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-import copy
 import dataclasses
 import uuid
 from collections import Counter
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
+from pydantic import BaseModel
+from pydantic import parse_obj_as
 
 from evidently.base_metric import InputData
 from evidently.core import IncludeOptions
 from evidently.metric_results import DatasetColumns
 from evidently.model.dashboard import DashboardInfo
 from evidently.model.widget import BaseWidgetInfo
-from evidently.options import ColorOptions
 from evidently.options.base import AnyOptions
 from evidently.options.base import Options
 from evidently.pipeline.column_mapping import ColumnMapping
 from evidently.renderers.base_renderer import TestRenderer
+from evidently.suite.base_suite import ContextPayload
 from evidently.suite.base_suite import Display
 from evidently.suite.base_suite import Suite
 from evidently.suite.base_suite import find_test_renderer
 from evidently.test_preset.test_preset import TestPreset
 from evidently.tests.base_test import DEFAULT_GROUP
 from evidently.tests.base_test import Test
 from evidently.tests.base_test import TestStatus
@@ -59,15 +60,15 @@
                 self._tests.append(original_test)
 
     def _add_tests(self):
         for original_test in self._tests or []:
             self._add_test(original_test)
 
     def _add_test(self, test: Test):
-        new_test = copy.copy(test)
+        new_test = test.copy()  # copy.copy(test)
         self._inner_suite.add_test(new_test)
 
     def __bool__(self):
         return all(test_result.is_passed() for _, test_result in self._inner_suite.context.test_results.items())
 
     def _add_tests_from_generator(self, test_generator: BaseGenerator):
         for test_item in test_generator.generate(columns_info=self._columns_info):
@@ -90,15 +91,14 @@
         data = InputData(reference_data, current_data, None, None, column_mapping, data_definition)
         for preset in self._test_presets:
             tests = preset.generate_tests(data, self._columns_info)
 
             for test in tests:
                 if isinstance(test, BaseGenerator):
                     self._add_tests_from_generator(test)
-
                 else:
                     self._add_test(test)
 
         for test_generator in self._test_generators:
             self._add_tests_from_generator(test_generator)
         self._inner_suite.verify()
         curr_add, ref_add = self._inner_suite.create_additional_features(current_data, reference_data, data_definition)
@@ -213,7 +213,24 @@
             additionalGraphs=[],
         )
         return (
             "evidently_dashboard_" + str(uuid.uuid4()).replace("-", ""),
             DashboardInfo("Test Suite", widgets=[summary_widget, test_suite_widget]),
             {item.id: dataclasses.asdict(item.info) for idx, info in enumerate(test_results) for item in info.details},
         )
+
+    def _get_payload(self) -> BaseModel:
+        return _TestSuitePayload(suite=ContextPayload.from_context(self._inner_suite.context), options=self.options)
+
+    @classmethod
+    def _parse_payload(cls, payload: Dict) -> "TestSuite":
+        return parse_obj_as(_TestSuitePayload, payload).load()
+
+
+class _TestSuitePayload(BaseModel):
+    suite: ContextPayload
+    options: Options
+
+    def load(self):
+        suite = TestSuite(tests=None, options=self.options)
+        suite._inner_suite.context = self.suite.to_context()
+        return suite
```

### Comparing `evidently-0.3.2.1/src/evidently/tests/base_test.py` & `evidently-0.3.3/src/evidently/tests/base_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,28 +9,31 @@
 from typing import Generic
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
-from pydantic import BaseModel
 from pydantic import Field
 
+from evidently.base_metric import BaseResult
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
+from evidently.core import IncludeTags
+from evidently.pydantic_utils import EnumValueMixin
+from evidently.pydantic_utils import EvidentlyBaseModel
+from evidently.pydantic_utils import ExcludeNoneMixin
+from evidently.pydantic_utils import WithTestAndMetricDependencies
 from evidently.utils.generators import BaseGenerator
 from evidently.utils.generators import make_generator_by_columns
 from evidently.utils.types import ApproxValue
 from evidently.utils.types import Numeric
 from evidently.utils.types import NumericApprox
 
 if TYPE_CHECKING:
-    from pydantic.typing import DictStrAny
-
     from evidently.suite.base_suite import Context
 
 
 @dataclasses.dataclass
 class GroupData:
     id: str
     title: str
@@ -81,37 +84,26 @@
     GroupingTypes.ByFeature,
     GroupingTypes.TestGroup,
     GroupingTypes.TestType,
     GroupingTypes.ByClass,
 ]
 
 
-class EnumValueMixin(BaseModel):
-    def dict(self, *args, **kwargs) -> "DictStrAny":
-        res = super().dict(*args, **kwargs)
-        return {k: v.value if isinstance(v, Enum) else v for k, v in res.items()}
-
-
-class ExcludeNoneMixin(BaseModel):
-    def dict(self, *args, **kwargs) -> "DictStrAny":
-        kwargs["exclude_none"] = True
-        return super().dict(*args, **kwargs)
-
-
 class TestStatus(Enum):
     # Constants for test result status
     SUCCESS = "SUCCESS"  # the test was passed
     FAIL = "FAIL"  # success pass for the test
     WARNING = "WARNING"  # the test was passed, but we have some issues during the execution
     ERROR = "ERROR"  # cannot calculate the test result, no data
     SKIPPED = "SKIPPED"  # the test was skipped
 
 
-class TestParameters(MetricResult):
-    pass
+class TestParameters(EvidentlyBaseModel, BaseResult):  # type: ignore[misc] # pydantic Config
+    class Config:
+        field_tags = {"type": {IncludeTags.TypeField}}
 
 
 class TestResult(EnumValueMixin, MetricResult):  # todo: create common base class
     # short name/title from the test class
     name: str
     # what was checked, what threshold (current value 13 is not ok with condition less than 5)
     description: str
@@ -141,34 +133,34 @@
     def mark_as_warning(self, description: Optional[str] = None):
         self.set_status(TestStatus.WARNING, description=description)
 
     def is_passed(self):
         return self.status in [TestStatus.SUCCESS, TestStatus.WARNING]
 
 
-class Test:
+class Test(WithTestAndMetricDependencies):
     """
     all fields in test class with type that is subclass of Metric would be used as dependencies of test.
     """
 
-    name: str
-    group: str
-    context: Optional["Context"] = None
+    name: ClassVar[str]
+    group: ClassVar[str]
+    _context: Optional["Context"] = None
 
     @abc.abstractmethod
     def check(self) -> TestResult:
         raise NotImplementedError
 
     def set_context(self, context: "Context"):
-        self.context = context
+        self._context = context
 
     def get_result(self) -> TestResult:
-        if self.context is None:
+        if self._context is None:
             raise ValueError("No context is set")
-        result = self.context.test_results.get(self, None)
+        result = self._context.test_results.get(self, None)
         if result is None:
             raise ValueError(f"No result found for metric {self} of type {type(self).__name__}")
         return result  # type: ignore[return-value]
 
     def get_id(self) -> str:
         return self.__class__.__name__
 
@@ -271,41 +263,38 @@
         return f"{' and '.join(conditions)}"
 
 
 class ConditionTestParameters(TestParameters):
     condition: TestValueCondition
 
 
-class BaseConditionsTest(Test, ABC):
+class BaseConditionsTest(Test, TestValueCondition, ABC):
     """
     Base class for all tests with a condition
     """
 
-    condition: TestValueCondition
+    class Config:
+        arbitrary_types_allowed = True
+        use_enum_values = True
+        smart_union = True
+        underscore_attrs_are_private = True
+
+    # condition: TestValueCondition
 
-    def __init__(
-        self,
-        eq: Optional[NumericApprox] = None,
-        gt: Optional[Numeric] = None,
-        gte: Optional[Numeric] = None,
-        is_in: Optional[List[Union[Numeric, str, bool]]] = None,
-        lt: Optional[Numeric] = None,
-        lte: Optional[Numeric] = None,
-        not_eq: Optional[Numeric] = None,
-        not_in: Optional[List[Union[Numeric, str, bool]]] = None,
-    ):
-        self.condition = TestValueCondition(
-            eq=eq,
-            gt=gt,
-            gte=gte,
-            is_in=is_in,
-            lt=lt,
-            lte=lte,
-            not_eq=not_eq,
-            not_in=not_in,
+    @property
+    def condition(self) -> TestValueCondition:
+        return TestValueCondition(
+            eq=self.eq,
+            gt=self.gt,
+            gte=self.gte,
+            is_in=self.is_in,
+            lt=self.lt,
+            lte=self.lte,
+            not_eq=self.not_eq,
+            not_in=self.not_in,
         )
 
 
 class CheckValueParameters(ConditionTestParameters):
     value: Optional[Numeric]
 
 
@@ -314,15 +303,15 @@
 
 
 class BaseCheckValueTest(BaseConditionsTest):
     """
     Base class for all tests with checking a value condition
     """
 
-    value: Numeric
+    _value: Numeric
 
     @abc.abstractmethod
     def calculate_value_for_test(self) -> Optional[Any]:
         """Method for getting the checking value.
 
         Define it in a child class"""
         raise NotImplementedError()
@@ -338,26 +327,26 @@
     def get_condition(self) -> TestValueCondition:
         return self.condition
 
     def groups(self) -> Dict[str, str]:
         return {}
 
     def get_parameters(self) -> CheckValueParameters:
-        return CheckValueParameters(condition=self.get_condition(), value=self.value)
+        return CheckValueParameters(condition=self.get_condition(), value=self._value)
 
     def check(self):
         result = TestResult(
             name=self.name,
             description="The test was not launched",
             status=TestStatus.SKIPPED,
             group=self.group,
             parameters=None,
         )
         value = self.calculate_value_for_test()
-        self.value = value
+        self._value = value
         result.description = self.get_description(value)
         result.parameters = self.get_parameters()
 
         try:
             if value is None:
                 result.mark_as_error()
 
@@ -383,27 +372,31 @@
 
 
 T = TypeVar("T", bound=MetricResult)
 
 
 class ConditionFromReferenceMixin(BaseCheckValueTest, Generic[T], ABC):
     reference_field: ClassVar[str] = "reference"
-    metric: Metric
+    _metric: Metric
 
     def get_condition_from_reference(self, reference: Optional[T]) -> TestValueCondition:
         raise NotImplementedError
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
 
         reference_stats = getattr(self.metric.get_result(), self.reference_field)
 
         return self.get_condition_from_reference(reference_stats)
 
+    @property
+    def metric(self):
+        return self._metric
+
 
 def generate_column_tests(
     test_class: Type[Test], columns: Optional[Union[str, list]] = None, parameters: Optional[Dict] = None
 ) -> BaseGenerator:
     """Function for generating tests for columns"""
     return make_generator_by_columns(
         base_class=test_class,
```

### Comparing `evidently-0.3.2.1/src/evidently/tests/classification_performance_tests.py` & `evidently-0.3.3/src/evidently/tests/classification_performance_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from evidently.metric_results import DatasetClassificationQuality
 from evidently.metric_results import Label
 from evidently.metric_results import ROCCurve
 from evidently.metrics.classification_performance.classification_dummy_metric import ClassificationDummyMetric
 from evidently.metrics.classification_performance.classification_quality_metric import ClassificationConfusionMatrix
 from evidently.metrics.classification_performance.classification_quality_metric import ClassificationQualityMetric
 from evidently.metrics.classification_performance.classification_quality_metric import ClassificationQualityMetricResult
+from evidently.metrics.classification_performance.confusion_matrix_metric import ClassificationConfusionMatrixParameters
 from evidently.metrics.classification_performance.objects import ClassMetric
 from evidently.metrics.classification_performance.quality_by_class_metric import ClassificationQualityByClass
 from evidently.metrics.classification_performance.roc_curve_metric import ClassificationRocCurve
 from evidently.renderers.base_renderer import TestHtmlInfo
 from evidently.renderers.base_renderer import TestRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import TabData
@@ -38,42 +39,51 @@
 CLASSIFICATION_GROUP = GroupData("classification", "Classification", "")
 GroupingTypes.TestGroup.add_value(CLASSIFICATION_GROUP)
 
 
 class SimpleClassificationTest(BaseCheckValueTest):
     condition_arg: ClassVar[str] = "gt"
 
-    group = CLASSIFICATION_GROUP.id
-    name: str
-    metric: ClassificationQualityMetric
-    dummy_metric: ClassificationDummyMetric
+    group: ClassVar = CLASSIFICATION_GROUP.id
+    name: ClassVar[str]
+    _metric: ClassificationQualityMetric
+    _dummy_metric: ClassificationDummyMetric
 
     def __init__(
         self,
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
     ):
+
         super().__init__(
             eq=eq,
             gt=gt,
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        self.metric = ClassificationQualityMetric()
-        self.dummy_metric = ClassificationDummyMetric()
+        self._metric = ClassificationQualityMetric()
+        self._dummy_metric = ClassificationDummyMetric()
+
+    @property
+    def metric(self):
+        return self._metric
+
+    @property
+    def dummy_metric(self):
+        return self._dummy_metric
 
     def calculate_value_for_test(self) -> Optional[Any]:
         return self.get_value(self.metric.get_result().current)
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
@@ -93,55 +103,56 @@
         )
 
     @abc.abstractmethod
     def get_value(self, result: DatasetClassificationQuality):
         raise NotImplementedError()
 
 
-class SimpleClassificationTestTopK(SimpleClassificationTest, ABC):
-    metric: ClassificationQualityMetric
-    dummy_metric: ClassificationDummyMetric
-    conf_matrix: ClassificationConfusionMatrix
-    probas_threshold: Optional[float]
-    k: Optional[Union[float, int]]
+class SimpleClassificationTestTopK(SimpleClassificationTest, ClassificationConfusionMatrixParameters, ABC):
+    _conf_matrix: ClassificationConfusionMatrix
 
     def __init__(
         self,
         probas_threshold: Optional[float] = None,
         k: Optional[Union[float, int]] = None,
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
     ):
+
+        if k is not None and probas_threshold is not None:
+            raise ValueError("Only one of 'probas_threshold' or 'k' should be given")
+        self.k = k
+        self.probas_threshold = probas_threshold
         super().__init__(
             eq=eq,
             gt=gt,
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        if k is not None and probas_threshold is not None:
-            raise ValueError("Only one of 'probas_threshold' or 'k' should be given")
-        self.k = k
-        self.probas_threshold = probas_threshold
-        self.dummy_metric = ClassificationDummyMetric(probas_threshold=self.probas_threshold, k=self.k)
-        self.metric = ClassificationQualityMetric(probas_threshold=self.probas_threshold, k=self.k)
-        self.conf_matrix = ClassificationConfusionMatrix(probas_threshold=self.probas_threshold, k=self.k)
+        self._dummy_metric = ClassificationDummyMetric(probas_threshold=self.probas_threshold, k=self.k)
+        self._metric = ClassificationQualityMetric(probas_threshold=self.probas_threshold, k=self.k)
+        self._conf_matrix = self.confusion_matric_metric()
 
     def calculate_value_for_test(self) -> Optional[Any]:
         return self.get_value(self.metric.get_result().current)
 
+    @property
+    def conf_matrix(self):
+        return self._conf_matrix
+
 
 class TestAccuracyScore(SimpleClassificationTestTopK):
     name = "Accuracy Score"
 
     def get_value(self, result: DatasetClassificationQuality):
         return result.accuracy
 
@@ -178,15 +189,15 @@
         ref_matrix = obj.conf_matrix.get_result().reference_matrix
         fig = plot_conf_mtrx(curr_matrix, ref_matrix)
         info.with_details("Precision Score", plotly_figure(figure=fig, title=""))
         return info
 
 
 class TestF1Score(SimpleClassificationTestTopK):
-    name = "F1 Score"
+    name: ClassVar = "F1 Score"
 
     def get_value(self, result: DatasetClassificationQuality):
         return result.f1
 
     def get_description(self, value: Numeric) -> str:
         return f"The F1 Score is {value:.3g}. The test threshold is {self.get_condition()}"
 
@@ -220,39 +231,39 @@
         ref_matrix = obj.conf_matrix.get_result().reference_matrix
         fig = plot_conf_mtrx(curr_matrix, ref_matrix)
         info.with_details("Recall Score", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestRocAuc(SimpleClassificationTest):
-    name = "ROC AUC Score"
-    roc_curve: ClassificationRocCurve
+    name: ClassVar = "ROC AUC Score"
+    _roc_curve: ClassificationRocCurve
 
     def __init__(
         self,
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
     ):
+        self._roc_curve = ClassificationRocCurve()
         super().__init__(
             eq=eq,
             gt=gt,
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        self.roc_curve = ClassificationRocCurve()
 
     def get_value(self, result: DatasetClassificationQuality):
         return result.roc_auc
 
     def get_description(self, value: Numeric) -> str:
         if value is None:
             return "Not enough data to calculate ROC AUC. Consider providing probabilities instead of labels."
@@ -261,16 +272,16 @@
             return f"The ROC AUC Score is {value:.3g}. The test threshold is {self.get_condition()}"
 
 
 @default_renderer(wrap_type=TestRocAuc)
 class TestRocAucRenderer(TestRenderer):
     def render_html(self, obj: TestRocAuc) -> TestHtmlInfo:
         info = super().render_html(obj)
-        curr_roc_curve: Optional[ROCCurve] = obj.roc_curve.get_result().current_roc_curve
-        ref_roc_curve: Optional[ROCCurve] = obj.roc_curve.get_result().reference_roc_curve
+        curr_roc_curve: Optional[ROCCurve] = obj._roc_curve.get_result().current_roc_curve
+        ref_roc_curve: Optional[ROCCurve] = obj._roc_curve.get_result().reference_roc_curve
 
         if curr_roc_curve is None:
             return info
 
         tab_data = get_roc_auc_tab_data(curr_roc_curve, ref_roc_curve, color_options=self.color_options)
 
         if len(tab_data) == 1:
@@ -462,19 +473,22 @@
 
 
 class ByClassParameters(CheckValueParameters):
     label: Label
 
 
 class ByClassClassificationTest(BaseCheckValueTest, ABC):
-    group = CLASSIFICATION_GROUP.id
-    metric: ClassificationQualityMetric
-    by_class_metric: ClassificationQualityByClass
-    dummy_metric: ClassificationDummyMetric
-    conf_matrix: ClassificationConfusionMatrix
+    group: ClassVar = CLASSIFICATION_GROUP.id
+    _metric: ClassificationQualityMetric
+    _by_class_metric: ClassificationQualityByClass
+    _dummy_metric: ClassificationDummyMetric
+    _conf_matrix: ClassificationConfusionMatrix
+    label: Label
+    probas_threshold: Optional[float] = None
+    k: Optional[Union[float, int]] = None
 
     def __init__(
         self,
         label: Label,
         probas_threshold: Optional[float] = None,
         k: Optional[Union[float, int]] = None,
         eq: Optional[Numeric] = None,
@@ -482,35 +496,51 @@
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
     ):
+        if k is not None and probas_threshold is not None:
+            raise ValueError("Only one of 'probas_threshold' or 'k' should be given")
+
+        self.label = label
+        self.probas_threshold = probas_threshold
+        self.k = k
         super().__init__(
             eq=eq,
             gt=gt,
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
 
-        if k is not None and probas_threshold is not None:
-            raise ValueError("Only one of 'probas_threshold' or 'k' should be given")
-
-        self.label = label
-        self.probas_threshold = probas_threshold
-        self.k = k
-        self.metric = ClassificationQualityMetric(probas_threshold=self.probas_threshold, k=self.k)
-        self.dummy_metric = ClassificationDummyMetric(probas_threshold=self.probas_threshold, k=self.k)
-        self.by_class_metric = ClassificationQualityByClass(probas_threshold=self.probas_threshold, k=self.k)
-        self.conf_matrix = ClassificationConfusionMatrix(probas_threshold=self.probas_threshold, k=self.k)
+        self._metric = ClassificationQualityMetric(probas_threshold=self.probas_threshold, k=self.k)
+        self._dummy_metric = ClassificationDummyMetric(probas_threshold=self.probas_threshold, k=self.k)
+        self._by_class_metric = ClassificationQualityByClass(probas_threshold=self.probas_threshold, k=self.k)
+        self._conf_matrix = ClassificationConfusionMatrix(probas_threshold=self.probas_threshold, k=self.k)
+
+    @property
+    def metric(self):
+        return self._metric
+
+    @property
+    def dummy_metric(self):
+        return self._dummy_metric
+
+    @property
+    def by_class_metric(self):
+        return self._by_class_metric
+
+    @property
+    def conf_matrix(self):
+        return self._conf_matrix
 
     def calculate_value_for_test(self) -> Optional[Any]:
         return self.get_value(self.by_class_metric.get_result().current.metrics[self.label])
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
@@ -529,19 +559,19 @@
         return TestValueCondition(gt=self.get_value(dummy_result))
 
     @abc.abstractmethod
     def get_value(self, result: ClassMetric):
         raise NotImplementedError()
 
     def get_parameters(self) -> ByClassParameters:
-        return ByClassParameters(condition=self.get_condition(), value=self.value, label=self.label)
+        return ByClassParameters(condition=self.get_condition(), value=self._value, label=self.label)
 
 
 class TestPrecisionByClass(ByClassClassificationTest):
-    name: str = "Precision Score by Class"
+    name: ClassVar[str] = "Precision Score by Class"
 
     def get_value(self, result: ClassMetric):
         return result.precision
 
     def get_description(self, value: Numeric) -> str:
         return (
             f"The precision score of the label **{self.label}** is {value:.3g}. "
@@ -557,15 +587,15 @@
         ref_matrix = obj.conf_matrix.get_result().reference_matrix
         fig = plot_conf_mtrx(curr_matrix, ref_matrix)
         info.with_details("Precision by Class", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestRecallByClass(ByClassClassificationTest):
-    name: str = "Recall Score by Class"
+    name: ClassVar[str] = "Recall Score by Class"
 
     def get_value(self, result: ClassMetric):
         return result.recall
 
     def get_description(self, value: Numeric) -> str:
         return (
             f"The recall score of the label **{self.label}** is {value:.3g}. "
@@ -581,15 +611,15 @@
         ref_matrix = obj.conf_matrix.get_result().reference_matrix
         fig = plot_conf_mtrx(curr_matrix, ref_matrix)
         info.with_details("Recall by Class", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestF1ByClass(ByClassClassificationTest):
-    name: str = "F1 Score by Class"
+    name: ClassVar[str] = "F1 Score by Class"
 
     def get_value(self, result: ClassMetric):
         return result.f1
 
     def get_description(self, value: Numeric) -> str:
         return (
             f"The F1 score of the label **{self.label}** is {value:.3g}. The test threshold is {self.get_condition()}"
```

### Comparing `evidently-0.3.2.1/src/evidently/tests/data_drift_tests.py` & `evidently-0.3.3/src/evidently/tests/data_drift_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC
 from typing import Callable
+from typing import ClassVar
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
@@ -39,15 +40,15 @@
 from evidently.utils.types import Numeric
 from evidently.utils.visualizations import plot_contour_single
 
 DATA_DRIFT_GROUP = GroupData("data_drift", "Data Drift", "")
 GroupingTypes.TestGroup.add_value(DATA_DRIFT_GROUP)
 
 
-class ColumnDriftParameter(ExcludeNoneMixin, TestParameters):
+class ColumnDriftParameter(ExcludeNoneMixin, TestParameters):  # type: ignore[misc] # pydantic Config
     stattest: str
     score: float
     threshold: float
     detected: bool
     column_name: Optional[str] = None
 
     @classmethod
@@ -86,16 +87,16 @@
                 }
                 for feature, data in self.features.items()
             ],
         )
 
 
 class BaseDataDriftMetricsTest(BaseCheckValueTest, ABC):
-    group = DATA_DRIFT_GROUP.id
-    metric: DataDriftTable
+    group: ClassVar = DATA_DRIFT_GROUP.id
+    _metric: DataDriftTable
 
     def __init__(
         self,
         columns: Optional[List[str]] = None,
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
@@ -121,43 +122,47 @@
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        self.metric = DataDriftTable(
+        self._metric = DataDriftTable(
             columns=columns,
             stattest=stattest,
             cat_stattest=cat_stattest,
             num_stattest=num_stattest,
             text_stattest=text_stattest,
             per_column_stattest=per_column_stattest,
             stattest_threshold=stattest_threshold,
             cat_stattest_threshold=cat_stattest_threshold,
             num_stattest_threshold=num_stattest_threshold,
             text_stattest_threshold=text_stattest_threshold,
             per_column_stattest_threshold=per_column_stattest_threshold,
         )
 
+    @property
+    def metric(self):
+        return self._metric
+
     def check(self):
         result = super().check()
         metrics = self.metric.get_result()
 
         return TestResult(
             name=result.name,
             description=result.description,
             status=TestStatus(result.status),
             group=self.group,
             parameters=ColumnsDriftParameters.from_data_drift_table(metrics, self.get_condition()),
         )
 
 
 class TestNumberOfDriftedColumns(BaseDataDriftMetricsTest):
-    name = "Number of Drifted Features"
+    name: ClassVar = "Number of Drifted Features"
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
         else:
             return TestValueCondition(lt=max(0, self.metric.get_result().number_of_columns // 3))
 
@@ -169,15 +174,15 @@
         return (
             f"The drift is detected for {value} out of {n_features} features. "
             f"The test threshold is {self.get_condition()}."
         )
 
 
 class TestShareOfDriftedColumns(BaseDataDriftMetricsTest):
-    name = "Share of Drifted Columns"
+    name: ClassVar = "Share of Drifted Columns"
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
         else:
             return TestValueCondition(lt=0.3)
 
@@ -190,34 +195,41 @@
         return (
             f"The drift is detected for {value * 100:.3g}% features "
             f"({n_drifted_features} out of {n_features}). The test threshold is {self.get_condition()}"
         )
 
 
 class TestColumnDrift(Test):
-    name = "Drift per Column"
-    group = DATA_DRIFT_GROUP.id
-    metric: ColumnDriftMetric
+    name: ClassVar = "Drift per Column"
+    group: ClassVar = DATA_DRIFT_GROUP.id
+    _metric: ColumnDriftMetric
     column_name: ColumnName
+    stattest: Optional[PossibleStatTestType] = None
+    stattest_threshold: Optional[float] = None
 
     def __init__(
         self,
         column_name: Union[str, ColumnName],
         stattest: Optional[PossibleStatTestType] = None,
         stattest_threshold: Optional[float] = None,
     ):
-        if isinstance(column_name, str):
-            self.column_name = ColumnName.main_dataset(column_name)
-        else:
-            self.column_name = column_name
-        self.metric = ColumnDriftMetric(
+        self.column_name = ColumnName.from_any(column_name)
+        self.stattest = stattest
+        self.stattest_threshold = stattest_threshold
+
+        self._metric = ColumnDriftMetric(
             column_name=column_name,
             stattest=stattest,
             stattest_threshold=stattest_threshold,
         )
+        super().__init__()
+
+    @property
+    def metric(self):
+        return self._metric
 
     def check(self):
         drift_info = self.metric.get_result()
 
         p_value = np.round(drift_info.drift_score, 3)
         stattest_name = drift_info.stattest_name
         threshold = drift_info.stattest_threshold
@@ -510,20 +522,25 @@
                 color_options=self.color_options,
             )
             info.with_details(f"{column_name}", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestEmbeddingsDrift(Test):
-    name = "Drift for embeddings"
-    group = DATA_DRIFT_GROUP.id
-    metric: EmbeddingsDriftMetric
+    name: ClassVar = "Drift for embeddings"
+    group: ClassVar = DATA_DRIFT_GROUP.id
+    _metric: EmbeddingsDriftMetric
 
     def __init__(self, embeddings_name: str, drift_method: Optional[Callable] = None):
-        self.metric = EmbeddingsDriftMetric(embeddings_name=embeddings_name, drift_method=drift_method)
+        super().__init__()
+        self._metric = EmbeddingsDriftMetric(embeddings_name=embeddings_name, drift_method=drift_method)
+
+    @property
+    def metric(self):
+        return self._metric
 
     def check(self):
         drift_info = self.metric.get_result()
         drift_score = drift_info.drift_score
         if drift_info.drift_detected:
             drift = "detected"
```

### Comparing `evidently-0.3.2.1/src/evidently/tests/data_integrity_tests.py` & `evidently-0.3.3/src/evidently/tests/data_integrity_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC
+from typing import ClassVar
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
@@ -42,16 +43,16 @@
 from evidently.utils.types import NumericApprox
 
 DATA_INTEGRITY_GROUP = GroupData("data_integrity", "Data Integrity", "")
 GroupingTypes.TestGroup.add_value(DATA_INTEGRITY_GROUP)
 
 
 class BaseIntegrityValueTest(ConditionFromReferenceMixin[DatasetSummary], ABC):
-    group = DATA_INTEGRITY_GROUP.id
-    metric: DatasetSummaryMetric
+    group: ClassVar = DATA_INTEGRITY_GROUP.id
+    _metric: DatasetSummaryMetric
 
     def __init__(
         self,
         eq: Optional[NumericApprox] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
@@ -66,21 +67,21 @@
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        self.metric = DatasetSummaryMetric()
+        self._metric = DatasetSummaryMetric()
 
 
 class TestNumberOfColumns(BaseIntegrityValueTest):
     """Number of all columns in the data, including utility columns (id/index, datetime, target, predictions)"""
 
-    name = "Number of Columns"
+    name: ClassVar = "Number of Columns"
 
     def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
         if reference is not None:
             return TestValueCondition(eq=reference.number_of_columns, source=ValueSource.REFERENCE)
         return TestValueCondition(gt=0)
 
     def calculate_value_for_test(self) -> Numeric:
@@ -107,15 +108,15 @@
         info.details = additional_plots
         return info
 
 
 class TestNumberOfRows(BaseIntegrityValueTest):
     """Number of rows in the data"""
 
-    name = "Number of Rows"
+    name: ClassVar = "Number of Rows"
 
     def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
         if reference is not None:
             return TestValueCondition(eq=approx(reference.number_of_rows, relative=0.1), source=ValueSource.REFERENCE)
 
         return TestValueCondition(gt=30)
 
@@ -123,16 +124,16 @@
         return self.metric.get_result().current.number_of_rows
 
     def get_description(self, value: Numeric) -> str:
         return f"The number of rows is {value}. The test threshold is {self.get_condition()}."
 
 
 class BaseIntegrityMissingValuesValuesTest(ConditionFromReferenceMixin[DatasetMissingValues], ABC):
-    group = DATA_INTEGRITY_GROUP.id
-    metric: DatasetMissingValuesMetric
+    group: ClassVar = DATA_INTEGRITY_GROUP.id
+    _metric: DatasetMissingValuesMetric
 
     def __init__(
         self,
         missing_values: Optional[list] = None,
         replace: bool = True,
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
@@ -149,15 +150,15 @@
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        self.metric = DatasetMissingValuesMetric(missing_values=missing_values, replace=replace)
+        self._metric = DatasetMissingValuesMetric(missing_values=missing_values, replace=replace)
 
 
 class BaseTestMissingValuesRenderer(TestRenderer):
     """Common class for tests of missing values.
     Some tests have the same details visualizations.
     """
 
@@ -230,15 +231,15 @@
         info.details = additional_plots
         return info
 
 
 class TestNumberOfDifferentMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a number of different encoded missing values."""
 
-    name = "Different Types of Missing Values"
+    name: ClassVar = "Different Types of Missing Values"
 
     def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
             return TestValueCondition(eq=reference.number_of_different_missing_values, source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
@@ -273,15 +274,15 @@
             "number_of_different_missing_values",
         )
 
 
 class TestNumberOfMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a number of missing values."""
 
-    name = "The Number of Missing Values"
+    name: ClassVar = "The Number of Missing Values"
 
     def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
             curr_number_of_rows = self.metric.get_result().current.number_of_rows
             ref_number_of_rows = reference.number_of_rows
             mult = curr_number_of_rows / ref_number_of_rows
             return TestValueCondition(
@@ -310,15 +311,15 @@
             info, metric_result, "number_of_missing_values"
         )
 
 
 class TestShareOfMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a share of missing values."""
 
-    name = "Share of Missing Values"
+    name: ClassVar = "Share of Missing Values"
 
     def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
             return TestValueCondition(
                 lte=approx(reference.share_of_missing_values, relative=0.1), source=ValueSource.REFERENCE
             )
 
@@ -338,15 +339,15 @@
         metric_result = obj.metric.get_result()
         return self.get_table_with_missing_values_and_percents_by_column(info, metric_result, "share_of_missing_values")
 
 
 class TestNumberOfColumnsWithMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a number of columns with a missing value."""
 
-    name = "The Number of Columns With Missing Values"
+    name: ClassVar = "The Number of Columns With Missing Values"
 
     def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
             return TestValueCondition(lte=reference.number_of_columns_with_missing_values, source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
@@ -368,15 +369,15 @@
             info, metric_result, "number_of_columns_with_missing_values"
         )
 
 
 class TestShareOfColumnsWithMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a share of columns with a missing value."""
 
-    name = "The Share of Columns With Missing Values"
+    name: ClassVar = "The Share of Columns With Missing Values"
 
     def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
             return TestValueCondition(lte=reference.share_of_columns_with_missing_values, source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
@@ -399,15 +400,15 @@
             info, metric_result, "share_of_columns_with_missing_values"
         )
 
 
 class TestNumberOfRowsWithMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a number of rows with a missing value."""
 
-    name = "The Number Of Rows With Missing Values"
+    name: ClassVar = "The Number Of Rows With Missing Values"
 
     def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
             curr_number_of_rows = self.metric.get_result().current.number_of_rows
             ref_number_of_rows = reference.number_of_rows
             mult = curr_number_of_rows / ref_number_of_rows
             return TestValueCondition(
@@ -423,15 +424,15 @@
     def get_description(self, value: Numeric) -> str:
         return f"The number of rows with missing values is {value}. " f"The test threshold is {self.get_condition()}."
 
 
 class TestShareOfRowsWithMissingValues(BaseIntegrityMissingValuesValuesTest):
     """Check a share of rows with a missing value."""
 
-    name = "The Share of Rows With Missing Values"
+    name: ClassVar = "The Share of Rows With Missing Values"
 
     def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
             return TestValueCondition(
                 lte=approx(reference.share_of_rows_with_missing_values, relative=0.1), source=ValueSource.REFERENCE
             )
 
@@ -443,16 +444,16 @@
     def get_description(self, value: Numeric) -> str:
         return (
             f"The share of rows with missing values is {value:.3g}. " f"The test threshold is {self.get_condition()}."
         )
 
 
 class BaseIntegrityColumnMissingValuesTest(ConditionFromReferenceMixin[DatasetMissingValues], ABC):
-    group = DATA_INTEGRITY_GROUP.id
-    metric: DatasetMissingValuesMetric
+    group: ClassVar = DATA_INTEGRITY_GROUP.id
+    _metric: DatasetMissingValuesMetric
     column_name: str
 
     def __init__(
         self,
         column_name: str,
         missing_values: Optional[list] = None,
         replace: bool = True,
@@ -461,32 +462,32 @@
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
     ):
+        self.column_name = column_name
         super().__init__(
             eq=eq,
             gt=gt,
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        self.column_name = column_name
-        self.metric = DatasetMissingValuesMetric(missing_values=missing_values, replace=replace)
+        self._metric = DatasetMissingValuesMetric(missing_values=missing_values, replace=replace)
 
 
 class TestColumnNumberOfDifferentMissingValues(BaseIntegrityColumnMissingValuesTest):
     """Check a number of differently encoded missing values in one column."""
 
-    name = "Different Types of Missing Values in a Column"
+    name: ClassVar = "Different Types of Missing Values in a Column"
 
     def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
             if self.column_name not in reference.number_of_different_missing_values_by_column:
                 raise ValueError(
                     f"Cannot define test default conditions: no column '{self.column_name}' in reference dataset."
                 )
@@ -528,15 +529,15 @@
             "number_of_different_missing_values",
         )
 
 
 class TestColumnNumberOfMissingValues(BaseIntegrityColumnMissingValuesTest):
     """Check a number of missing values in one column."""
 
-    name = "The Number of Missing Values in a Column"
+    name: ClassVar = "The Number of Missing Values in a Column"
 
     def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
             curr_number_of_rows = self.metric.get_result().current.number_of_rows
             ref_number_of_rows = reference.number_of_rows
             mult = curr_number_of_rows / ref_number_of_rows
             ref_value = reference.number_of_missing_values_by_column[self.column_name]
@@ -553,15 +554,15 @@
             f"The test threshold is {self.get_condition()}."
         )
 
 
 class TestColumnShareOfMissingValues(BaseIntegrityColumnMissingValuesTest):
     """Check a share of missing values in one column."""
 
-    name = "The Share of Missing Values in a Column"
+    name: ClassVar = "The Share of Missing Values in a Column"
 
     def get_condition_from_reference(self, reference: Optional[DatasetMissingValues]):
         if reference is not None:
             ref_value = reference.share_of_missing_values_by_column[self.column_name]
             return TestValueCondition(lte=approx(ref_value, relative=0.1), source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
@@ -573,15 +574,15 @@
         return (
             f"The share of missing values in the column **{self.column_name}** is {value:.3g}. "
             f"The test threshold is {self.get_condition()}."
         )
 
     def get_parameters(self):
         return ColumnCheckValueParameters(
-            condition=self.get_condition(), value=self.value, column_name=self.column_name
+            condition=self.get_condition(), value=self._value, column_name=self.column_name
         )
 
 
 class TestAllColumnsShareOfMissingValues(BaseGenerator):
     columns: Optional[List[str]]
 
     def __init__(self, columns: Optional[List[str]] = None):
@@ -596,15 +597,15 @@
 
         return [TestColumnShareOfMissingValues(column_name=name) for name in columns]
 
 
 class TestNumberOfConstantColumns(BaseIntegrityValueTest):
     """Number of columns contained only one unique value"""
 
-    name = "Number of Constant Columns"
+    name: ClassVar = "Number of Constant Columns"
 
     def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
         if reference is not None:
             value = reference.number_of_constant_columns
             return TestValueCondition(lte=value, source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
@@ -633,15 +634,15 @@
         info.details = additional_plots
         return info
 
 
 class TestNumberOfEmptyRows(BaseIntegrityValueTest):
     """Number of rows contained all NAN values"""
 
-    name = "Number of Empty Rows"
+    name: ClassVar = "Number of Empty Rows"
 
     def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
         if reference is not None:
             ref_number_of_empty_rows = reference.number_of_empty_rows
             curr_number_of_rows = self.metric.get_result().current.number_of_rows
             ref_number_of_rows = reference.number_of_rows
             mult = curr_number_of_rows / ref_number_of_rows
@@ -655,15 +656,15 @@
     def get_description(self, value: Numeric) -> str:
         return f"Number of Empty Rows is {value}. The test threshold is {self.get_condition()}."
 
 
 class TestNumberOfEmptyColumns(BaseIntegrityValueTest):
     """Number of columns contained all NAN values"""
 
-    name = "Number of Empty Columns"
+    name: ClassVar = "Number of Empty Columns"
 
     def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
         if reference is not None:
             return TestValueCondition(lte=reference.number_of_empty_columns, source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
 
@@ -691,15 +692,15 @@
         info.details = additional_plots
         return info
 
 
 class TestNumberOfDuplicatedRows(BaseIntegrityValueTest):
     """How many rows have duplicates in the dataset"""
 
-    name = "Number of Duplicate Rows"
+    name: ClassVar = "Number of Duplicate Rows"
 
     def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
         if reference is not None:
             ref_num_of_duplicates = reference.number_of_duplicated_rows
             curr_number_of_rows = self.metric.get_result().current.number_of_rows
             ref_number_of_rows = reference.number_of_rows
             mult = curr_number_of_rows / ref_number_of_rows
@@ -713,15 +714,15 @@
     def get_description(self, value: Numeric) -> str:
         return f"The number of duplicate rows is {value}. The test threshold is {self.get_condition()}."
 
 
 class TestNumberOfDuplicatedColumns(BaseIntegrityValueTest):
     """How many columns have duplicates in the dataset"""
 
-    name = "Number of Duplicate Columns"
+    name: ClassVar = "Number of Duplicate Columns"
 
     def get_condition_from_reference(self, reference: Optional[DatasetSummary]):
         if reference is not None:
             value = reference.number_of_duplicated_columns
             return TestValueCondition(lte=value, source=ValueSource.REFERENCE)
 
         return TestValueCondition(eq=0)
@@ -730,16 +731,16 @@
         return self.metric.get_result().current.number_of_duplicated_columns
 
     def get_description(self, value: Numeric) -> str:
         return f"The number of duplicate columns is {value}. The test threshold is {self.get_condition()}."
 
 
 class BaseIntegrityByColumnsConditionTest(BaseCheckValueTest, ABC):
-    group = DATA_INTEGRITY_GROUP.id
-    data_integrity_metric: ColumnSummaryMetric
+    group: ClassVar = DATA_INTEGRITY_GROUP.id
+    _data_integrity_metric: ColumnSummaryMetric
     column_name: ColumnName
 
     def __init__(
         self,
         column_name: Union[str, ColumnName],
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
@@ -756,47 +757,46 @@
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        if isinstance(column_name, str):
-            self.column_name = ColumnName.main_dataset(column_name)
-        else:
-            self.column_name = column_name
-        self.data_integrity_metric = ColumnSummaryMetric(column_name=column_name)
+        self.column_name = ColumnName.from_any(column_name)
+        self._data_integrity_metric = ColumnSummaryMetric(column_name=column_name)
 
     def groups(self) -> Dict[str, str]:
         if self.column_name is not None:
             return {GroupingTypes.ByFeature.id: self.column_name.display_name}
         return {}
 
 
 class BaseIntegrityOneColumnTest(Test, ABC):
-    group = DATA_INTEGRITY_GROUP.id
-    metric: ColumnSummaryMetric
+    group: ClassVar = DATA_INTEGRITY_GROUP.id
+    _metric: ColumnSummaryMetric
     column_name: ColumnName
 
     def __init__(self, column_name: Union[str, ColumnName]):
-        if isinstance(column_name, str):
-            self.column_name = ColumnName.main_dataset(column_name)
-        else:
-            self.column_name = column_name
-        self.metric = ColumnSummaryMetric(self.column_name)
+        self.column_name = ColumnName.from_any(column_name)
+        super().__init__()
+        self._metric = ColumnSummaryMetric(self.column_name)
+
+    @property
+    def metric(self):
+        return self._metric
 
     def groups(self) -> Dict[str, str]:
         return {GroupingTypes.ByFeature.id: self.column_name.display_name}
 
 
 class TestColumnAllConstantValues(BaseIntegrityOneColumnTest):
     """Test that there is only one unique value in a column"""
 
-    name = "All Constant Values in a Column"
-    metric: ColumnSummaryMetric
+    name: ClassVar = "All Constant Values in a Column"
+    _metric: ColumnSummaryMetric
 
     def check(self):
         uniques_in_column = self.metric.get_result().current_characteristics.unique
         number_of_rows = self.metric.get_result().current_characteristics.number_of_rows
         column_name = self.column_name
 
         description = (
@@ -830,15 +830,15 @@
             info.details = additional_plots
         return info
 
 
 class TestColumnAllUniqueValues(BaseIntegrityOneColumnTest):
     """Test that there is only uniques values in a column"""
 
-    name = "All Unique Values in a Column"
+    name: ClassVar = "All Unique Values in a Column"
 
     def check(self):
         uniques_in_column = self.metric.get_result().current_characteristics.unique
         number_of_rows = self.metric.get_result().current_characteristics.number_of_rows
         nans_in_column = self.metric.get_result().current_characteristics.missing
         column_name = self.column_name
 
@@ -883,22 +883,27 @@
 class ColumnTypesParameter(TestParameters):
     columns: List[ColumnTypeParameter]
 
 
 class TestColumnsType(Test):
     """This test compares columns type against the specified ones or a reference dataframe"""
 
-    group = DATA_INTEGRITY_GROUP.id
-    name = "Column Types"
+    group: ClassVar = DATA_INTEGRITY_GROUP.id
+    name: ClassVar = "Column Types"
     columns_type: Optional[dict]
-    metric: DatasetSummaryMetric
+    _metric: DatasetSummaryMetric
 
     def __init__(self, columns_type: Optional[dict] = None):
         self.columns_type = columns_type
-        self.metric = DatasetSummaryMetric()
+        self._metric = DatasetSummaryMetric()
+        super().__init__()
+
+    @property
+    def metric(self):
+        return self._metric
 
     def check(self):
         status = TestStatus.SUCCESS
         data_columns_type = self.metric.get_result().current.columns_type
 
         if self.columns_type is None:
             if self.metric.get_result().reference is None:
@@ -974,44 +979,50 @@
                 ),
             ),
         ]
         return info
 
 
 class TestColumnRegExp(BaseCheckValueTest, ABC):
-    group = DATA_INTEGRITY_GROUP.id
-    name = "RegExp Match"
-    metric: ColumnRegExpMetric
+    group: ClassVar = DATA_INTEGRITY_GROUP.id
+    name: ClassVar = "RegExp Match"
+    _metric: ColumnRegExpMetric
     column_name: str
+    reg_exp: str
 
     def __init__(
         self,
         column_name: str,
         reg_exp: str,
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
     ):
+        self.column_name = column_name
+        self.reg_exp = reg_exp
         super().__init__(
             eq=eq,
             gt=gt,
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        self.column_name = column_name
-        self.metric = ColumnRegExpMetric(column_name=column_name, reg_exp=reg_exp)
+        self._metric = ColumnRegExpMetric(column_name=column_name, reg_exp=reg_exp)
+
+    @property
+    def metric(self):
+        return self._metric
 
     def groups(self) -> Dict[str, str]:
         if self.column_name is not None:
             return {GroupingTypes.ByFeature.id: self.column_name}
         return {}
 
     def get_condition(self) -> TestValueCondition:
```

### Comparing `evidently-0.3.2.1/src/evidently/tests/data_quality_tests.py` & `evidently-0.3.3/src/evidently/tests/data_quality_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,16 +54,17 @@
 
 DATA_QUALITY_GROUP = GroupData("data_quality", "Data Quality", "")
 GroupingTypes.TestGroup.add_value(DATA_QUALITY_GROUP)
 
 
 class BaseDataQualityMetricsValueTest(ConditionFromReferenceMixin[ColumnCharacteristics], ABC):
     reference_field: ClassVar = "reference_characteristics"
-    group = DATA_QUALITY_GROUP.id
-    metric: ColumnSummaryMetric
+    group: ClassVar = DATA_QUALITY_GROUP.id
+    _metric: ColumnSummaryMetric
+    column_name: ColumnName
 
     def __init__(
         self,
         column_name: Union[str, ColumnName],
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
@@ -78,25 +79,31 @@
             gt=gt,
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
+            column_name=ColumnName.from_any(column_name),
         )
-        self.metric = ColumnSummaryMetric(column_name)
+        self._metric = ColumnSummaryMetric(column_name)
 
 
 class TestConflictTarget(Test):
-    group = DATA_QUALITY_GROUP.id
-    name = "Test number of conflicts in target"
-    metric: ConflictTargetMetric
+    group: ClassVar = DATA_QUALITY_GROUP.id
+    name: ClassVar = "Test number of conflicts in target"
+    _metric: ConflictTargetMetric
 
     def __init__(self):
-        self.metric = ConflictTargetMetric()
+        self._metric = ConflictTargetMetric()
+        super().__init__()
+
+    @property
+    def metric(self):
+        return self._metric
 
     def check(self):
         metric_result = self.metric.get_result()
 
         if metric_result.number_not_stable_target is None:
             test_result = TestStatus.ERROR
             description = "No target in the dataset"
@@ -109,20 +116,25 @@
             test_result = TestStatus.SUCCESS
             description = "Target is stable"
 
         return TestResult(name=self.name, description=description, status=test_result, group=self.group)
 
 
 class TestConflictPrediction(Test):
-    group = DATA_QUALITY_GROUP.id
-    name = "Test number of conflicts in prediction"
-    metric: ConflictPredictionMetric
+    group: ClassVar = DATA_QUALITY_GROUP.id
+    name: ClassVar = "Test number of conflicts in prediction"
+    _metric: ConflictPredictionMetric
 
     def __init__(self):
-        self.metric = ConflictPredictionMetric()
+        self._metric = ConflictPredictionMetric()
+        super().__init__()
+
+    @property
+    def metric(self):
+        return self._metric
 
     def check(self):
         metric_result = self.metric.get_result()
 
         if metric_result.current.number_not_stable_prediction is None:
             test_result = TestStatus.ERROR
             description = "No prediction in the dataset"
@@ -135,16 +147,16 @@
             test_result = TestStatus.SUCCESS
             description = "Prediction is stable"
 
         return TestResult(name=self.name, description=description, status=test_result, group=self.group)
 
 
 class BaseDataQualityCorrelationsMetricsValueTest(ConditionFromReferenceMixin[DatasetCorrelation], ABC):
-    group = DATA_QUALITY_GROUP.id
-    metric: DatasetCorrelationsMetric
+    group: ClassVar = DATA_QUALITY_GROUP.id
+    _metric: DatasetCorrelationsMetric
     method: Optional[str]
 
     def __init__(
         self,
         method: Optional[str] = None,
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
@@ -162,19 +174,19 @@
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        self.metric = DatasetCorrelationsMetric()
+        self._metric = DatasetCorrelationsMetric()
 
 
 class TestTargetPredictionCorrelation(BaseDataQualityCorrelationsMetricsValueTest):
-    name = "Correlation between Target and Prediction"
+    name: ClassVar = "Correlation between Target and Prediction"
 
     def get_condition_from_reference(self, reference: Optional[DatasetCorrelation]) -> TestValueCondition:
         if reference is not None:
             method = get_corr_method(self.method, self.metric.get_result().target_correlation, False)
             value = reference.stats[method].target_prediction_correlation
 
             if value is not None:
@@ -192,15 +204,15 @@
         return (
             f"The correlation between the target and prediction is {value:.3}. "
             f"The test threshold is {self.get_condition()}."
         )
 
 
 class TestHighlyCorrelatedColumns(BaseDataQualityCorrelationsMetricsValueTest):
-    name = "Highly Correlated Columns"
+    name: ClassVar = "Highly Correlated Columns"
 
     def get_condition_from_reference(self, reference: Optional[DatasetCorrelation]) -> TestValueCondition:
         if reference is not None:
             value = reference.stats[get_corr_method(self.method)].abs_max_features_correlation
 
             if value is not None:
                 return TestValueCondition(eq=approx(value, relative=0.1), source=ValueSource.REFERENCE)
@@ -230,15 +242,15 @@
 
         fig = plot_correlations(current_correlations, reference_correlations)
         info.with_details("Highly Correlated Features", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestTargetFeaturesCorrelations(BaseDataQualityCorrelationsMetricsValueTest):
-    name = "Correlation between Target and Features"
+    name: ClassVar = "Correlation between Target and Features"
 
     def get_condition_from_reference(self, reference: Optional[DatasetCorrelation]) -> TestValueCondition:
         if reference is not None:
             method = get_corr_method(self.method, self.metric.get_result().target_correlation, False)
             value = reference.stats[method].abs_max_target_features_correlation
 
             if value is not None:
@@ -255,15 +267,15 @@
             return "No target in the current dataset"
 
         else:
             return f"The maximum correlation is {value:.3g}. The test threshold is {self.get_condition()}."
 
 
 class TestPredictionFeaturesCorrelations(BaseDataQualityCorrelationsMetricsValueTest):
-    name = "Correlation between Prediction and Features"
+    name: ClassVar = "Correlation between Prediction and Features"
 
     def get_condition_from_reference(self, reference: Optional[DatasetCorrelation]) -> TestValueCondition:
         if reference is not None:
             method = get_corr_method(self.method, self.metric.get_result().target_correlation, False)
             value = reference.stats[method].abs_max_prediction_features_correlation
 
             if value is not None:
@@ -300,17 +312,17 @@
 
         fig = plot_correlations(current_correlations, reference_correlations)
         info.with_details("Target-Features Correlations", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestCorrelationChanges(BaseDataQualityCorrelationsMetricsValueTest):
-    group = DATA_QUALITY_GROUP.id
-    name = "Change in Correlation"
-    metric: DatasetCorrelationsMetric
+    group: ClassVar = DATA_QUALITY_GROUP.id
+    name: ClassVar = "Change in Correlation"
+    _metric: DatasetCorrelationsMetric
     corr_diff: float
 
     def __init__(
         self,
         corr_diff: float = 0.25,
         method: str = "pearson",
         eq: Optional[Numeric] = None,
@@ -318,26 +330,26 @@
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
     ):
+        self.corr_diff = corr_diff
         super().__init__(
             method=method,
             eq=eq,
             gt=gt,
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        self.corr_diff = corr_diff
 
     def get_condition_from_reference(self, reference: Optional[DatasetCorrelation]) -> TestValueCondition:
         pass
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
@@ -379,32 +391,26 @@
 
         fig = plot_correlations(current_correlations, reference_correlations)
         info.with_details("Target-Features Correlations", plotly_figure(title="", figure=fig))
         return info
 
 
 class BaseFeatureDataQualityMetricsTest(BaseDataQualityMetricsValueTest, ABC):
-    column_name: ColumnName
-
     def __init__(
         self,
         column_name: Union[str, ColumnName],
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
     ):
-        if isinstance(column_name, str):
-            self.column_name = ColumnName.main_dataset(column_name)
-        else:
-            self.column_name = column_name
         super().__init__(
             column_name=column_name,
             eq=eq,
             gt=gt,
             gte=gte,
             is_in=is_in,
             lt=lt,
@@ -417,26 +423,26 @@
         return {
             GroupingTypes.ByFeature.id: self.column_name.display_name,
         }
 
     def check(self):
         result = super().check()
 
-        if self.value is None:
+        if self._value is None:
             result.mark_as_error(f"No value for the feature '{self.column_name}'")
             return result
 
         return result
 
     def get_stat(self, current: NumericCharacteristics):
         raise NotImplementedError
 
 
 class TestColumnValueMin(BaseFeatureDataQualityMetricsTest):
-    name = "Min Value"
+    name: ClassVar = "Min Value"
 
     def get_stat(self, current: NumericCharacteristics):
         return current.min
 
     def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
         if reference is not None:
             if not isinstance(reference, NumericCharacteristics):
@@ -453,15 +459,15 @@
         return min_value
 
     def get_description(self, value: Numeric) -> str:
         return f"The minimum value of the column **{self.column_name}** is {value} The test threshold is {self.get_condition()}."
 
 
 class TestColumnValueMax(BaseFeatureDataQualityMetricsTest):
-    name = "Max Value"
+    name: ClassVar = "Max Value"
 
     def get_stat(self, current: NumericCharacteristics):
         return current.max
 
     def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
         if reference is not None:
             if not isinstance(reference, NumericCharacteristics):
@@ -480,15 +486,15 @@
         return max_value
 
     def get_description(self, value: Numeric) -> str:
         return f"The maximum value of the column **{self.column_name}** is {value}. The test threshold is {self.get_condition()}."
 
 
 class TestColumnValueMean(BaseFeatureDataQualityMetricsTest):
-    name = "Mean Value"
+    name: ClassVar = "Mean Value"
 
     def get_stat(self, current: NumericCharacteristics):
         return current.mean
 
     def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
         if reference is not None:
             if not isinstance(reference, NumericCharacteristics):
@@ -503,15 +509,15 @@
         return features_stats.mean
 
     def get_description(self, value: Numeric) -> str:
         return f"The mean value of the column **{self.column_name}** is {value:.3g}. The test threshold is {self.get_condition()}."
 
 
 class TestColumnValueMedian(BaseFeatureDataQualityMetricsTest):
-    name = "Median Value"
+    name: ClassVar = "Median Value"
 
     def get_stat(self, current: NumericCharacteristics):
         return current.p50
 
     def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
         if reference is not None:
             if not isinstance(reference, NumericCharacteristics):
@@ -557,15 +563,15 @@
         curr_distr = bins_for_hist.current
         ref_distr = bins_for_hist.reference
         fig = plot_distr(hist_curr=curr_distr, hist_ref=ref_distr, color_options=self.color_options)
         return column_name, fig, info, metric_result
 
 
 class TestColumnValueStd(BaseFeatureDataQualityMetricsTest):
-    name = "Standard Deviation (SD)"
+    name: ClassVar = "Standard Deviation (SD)"
 
     def get_stat(self, current: NumericCharacteristics):
         return current.std
 
     def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
         if reference is not None:
             if not isinstance(reference, NumericCharacteristics):
@@ -591,15 +597,15 @@
     def render_html(self, obj: BaseFeatureDataQualityMetricsTest) -> TestHtmlInfo:
         column_name, fig, info, _ = self._feature_render_html(obj)
         info.with_details(f"Std Value {column_name}", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestNumberOfUniqueValues(BaseFeatureDataQualityMetricsTest):
-    name = "Number of Unique Values"
+    name: ClassVar = "Number of Unique Values"
 
     def get_stat(self, current: NumericCharacteristics):
         return current.unique
 
     def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
         if reference is not None:
             if not isinstance(reference, (NumericCharacteristics, CategoricalCharacteristics, DatetimeCharacteristics)):
@@ -635,15 +641,15 @@
                 ref_df = counts_data["reference"]
             info.details = plot_value_counts_tables_ref_curr(column_name, curr_df, ref_df, "num_of_unique_vals")
 
         return info
 
 
 class TestUniqueValuesShare(BaseFeatureDataQualityMetricsTest):
-    name = "Share of Unique Values"
+    name: ClassVar = "Share of Unique Values"
 
     def get_stat(self, current: NumericCharacteristics):
         return current.unique_percentage
 
     def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
         if reference is not None:
             if not isinstance(reference, (NumericCharacteristics, CategoricalCharacteristics, DatetimeCharacteristics)):
@@ -686,15 +692,15 @@
                 ref_df = counts_data["reference"]
             info.details = plot_value_counts_tables_ref_curr(column_name, curr_df, ref_df, "unique_vals_sare")
 
         return info
 
 
 class TestMostCommonValueShare(BaseFeatureDataQualityMetricsTest):
-    name = "Share of the Most Common Value"
+    name: ClassVar = "Share of the Most Common Value"
 
     def get_stat(self, current: NumericCharacteristics):
         return current.most_common_percentage
 
     def get_condition_from_reference(self, reference: Optional[ColumnCharacteristics]) -> TestValueCondition:
         if reference is not None:
             if not isinstance(reference, (NumericCharacteristics, CategoricalCharacteristics, DatetimeCharacteristics)):
@@ -726,15 +732,15 @@
             f"The most common value in the column **{self.column_name}** is {most_common_value}. "
             f"Its share is {value:.3g}. "
             f"The test threshold is {self.get_condition()}."
         )
 
     def get_parameters(self) -> ColumnCheckValueParameters:
         return ColumnCheckValueParameters(
-            column_name=self.column_name.display_name, condition=self.get_condition(), value=self.value
+            column_name=self.column_name.display_name, condition=self.get_condition(), value=self._value
         )
 
 
 @default_renderer(wrap_type=TestMostCommonValueShare)
 class TestMostCommonValueShareRenderer(TestRenderer):
     def render_html(self, obj: TestMostCommonValueShare) -> TestHtmlInfo:
         info = super().render_html(obj)
@@ -778,27 +784,29 @@
     n_sigmas: int  # ? float
     reference_mean: float
     reference_std: float
 
 
 class TestMeanInNSigmas(Test):
 
-    group = DATA_QUALITY_GROUP.id
-    name = "Mean Value Stability"
-    metric: ColumnSummaryMetric
+    group: ClassVar = DATA_QUALITY_GROUP.id
+    name: ClassVar = "Mean Value Stability"
+    _metric: ColumnSummaryMetric
     column_name: ColumnName
     n_sigmas: int
 
     def __init__(self, column_name: Union[str, ColumnName], n_sigmas: int = 2):
-        if isinstance(column_name, str):
-            self.column_name = ColumnName.main_dataset(column_name)
-        else:
-            self.column_name = column_name
+        self.column_name = ColumnName.from_any(column_name)
         self.n_sigmas = n_sigmas
-        self.metric = ColumnSummaryMetric(column_name)
+        self._metric = ColumnSummaryMetric(column_name)
+        super().__init__()
+
+    @property
+    def metric(self):
+        return self._metric
 
     def check(self):
         reference_feature_stats = self.metric.get_result().reference_characteristics
         features_stats = self.metric.get_result().current_characteristics
 
         # todo: this was thrown in a render, do we just cut it?
         # if not isinstance(features_stats, NumericCharacteristics):
@@ -903,34 +911,36 @@
         else:
             columns = [column for column in self.columns if column in columns_info.num_feature_names]
 
         return [TestMeanInNSigmas(column_name=name, n_sigmas=2) for name in columns]
 
 
 class TestValueRange(Test):
-    group = DATA_QUALITY_GROUP.id
-    name = "Value Range"
-    metric: ColumnValueRangeMetric
+    group: ClassVar = DATA_QUALITY_GROUP.id
+    name: ClassVar = "Value Range"
+    _metric: ColumnValueRangeMetric
     column_name: ColumnName
     left: Optional[float]
     right: Optional[float]
 
     def __init__(
         self,
         column_name: Union[str, ColumnName],
         left: Optional[float] = None,
         right: Optional[float] = None,
     ):
-        if isinstance(column_name, str):
-            self.column_name = ColumnName.main_dataset(column_name)
-        else:
-            self.column_name = column_name
+        self.column_name = ColumnName.from_any(column_name)
         self.left = left
         self.right = right
-        self.metric = ColumnValueRangeMetric(column_name=self.column_name, left=left, right=right)
+        super().__init__()
+        self._metric = ColumnValueRangeMetric(column_name=self.column_name, left=left, right=right)
+
+    @property
+    def metric(self):
+        return self._metric
 
     def check(self):
         number_not_in_range = self.metric.get_result().current.number_not_in_range
 
         if number_not_in_range > 0:
             description = f"The column **{self.column_name}** has values out of range."
             test_result = TestStatus.FAIL
@@ -966,16 +976,16 @@
             f"Value Range {column_name.display_name}",
             plotly_figure(title="", figure=fig),
         )
         return info
 
 
 class BaseDataQualityValueRangeMetricsTest(BaseCheckValueTest, ABC):
-    group = DATA_QUALITY_GROUP.id
-    metric: ColumnValueRangeMetric
+    group: ClassVar = DATA_QUALITY_GROUP.id
+    _metric: ColumnValueRangeMetric
     column_name: ColumnName
     left: Optional[float]
     right: Optional[float]
 
     def __init__(
         self,
         column_name: Union[str, ColumnName],
@@ -986,21 +996,18 @@
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
     ):
-        if isinstance(column_name, str):
-            self.column_name = ColumnName.main_dataset(column_name)
-        else:
-            self.column_name = column_name
+        self.column_name = ColumnName.from_any(column_name)
         self.left = left
         self.right = right
-        self.metric = ColumnValueRangeMetric(column_name=column_name, left=left, right=right)
+        self._metric = ColumnValueRangeMetric(column_name=column_name, left=left, right=right)
 
         super().__init__(
             eq=eq,
             gt=gt,
             gte=gte,
             is_in=is_in,
             lt=lt,
@@ -1013,17 +1020,21 @@
         return {GroupingTypes.ByFeature.id: self.column_name.display_name}
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
         return TestValueCondition(eq=approx(0))
 
+    @property
+    def metric(self):
+        return self._metric
+
 
 class TestNumberOfOutRangeValues(BaseDataQualityValueRangeMetricsTest):
-    name = "Number of Out-of-Range Values "
+    name: ClassVar = "Number of Out-of-Range Values "
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_not_in_range
 
     def get_description(self, value: Numeric) -> str:
         return (
             f"The number of values out of range in the column **{self.column_name}** is {value}. "
@@ -1033,30 +1044,30 @@
 
 class ShareOfOutRangeParameters(CheckValueParameters):
     left: Optional[float]
     right: Optional[float]
 
 
 class TestShareOfOutRangeValues(BaseDataQualityValueRangeMetricsTest):
-    name = "Share of Out-of-Range Values"
+    name: ClassVar = "Share of Out-of-Range Values"
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.share_not_in_range
 
     def get_description(self, value: Numeric) -> str:
         current_result = self.metric.get_result().current
         return (
             f"The share of values out of range in the column **{self.column_name.display_name}** is {value:.3g} "
             f"({current_result.number_not_in_range} out of {current_result.number_of_values}). "
             f" The test threshold is {self.get_condition()}."
         )
 
     def get_parameters(self) -> ShareOfOutRangeParameters:
         return ShareOfOutRangeParameters(
-            condition=self.get_condition(), value=self.value, left=self.left, right=self.right
+            condition=self.get_condition(), value=self._value, left=self.left, right=self.right
         )
 
 
 @default_renderer(wrap_type=TestShareOfOutRangeValues)
 @default_renderer(wrap_type=TestNumberOfOutRangeValues)
 class TestRangeValuesRenderer(TestRenderer):
     def render_html(self, obj: BaseDataQualityValueRangeMetricsTest) -> TestHtmlInfo:
@@ -1096,25 +1107,30 @@
 class ColumnValueListParameters(TestParameters):
     value: Numeric
     column_name: str
     values: Optional[List[Any]] = None
 
 
 class TestValueList(Test):
-    group = DATA_QUALITY_GROUP.id
-    name = "Out-of-List Values"
-    alias = "value_list"
-    metric: ColumnValueListMetric
+    group: ClassVar = DATA_QUALITY_GROUP.id
+    name: ClassVar = "Out-of-List Values"
+    alias: ClassVar = "value_list"
+    _metric: ColumnValueListMetric
     column_name: str
     values: Optional[list]
 
     def __init__(self, column_name: str, values: Optional[list] = None):
         self.column_name = column_name
         self.values = values
-        self.metric = ColumnValueListMetric(column_name=column_name, values=values)
+        self._metric = ColumnValueListMetric(column_name=column_name, values=values)
+        super().__init__()
+
+    @property
+    def metric(self):
+        return self._metric
 
     def check(self):
         metric_result = self.metric.get_result()
 
         if metric_result.current.number_not_in_list > 0:
             test_result = TestStatus.FAIL
             description = f"The column **{self.column_name}** has values out of list."
@@ -1133,16 +1149,16 @@
                 value=metric_result.current.number_not_in_list, values=self.values, column_name=self.column_name
             ),
         )
 
 
 class BaseDataQualityValueListMetricsTest(BaseCheckValueTest, ABC):
     alias: ClassVar[str]
-    group = DATA_QUALITY_GROUP.id
-    metric: ColumnValueListMetric
+    group: ClassVar = DATA_QUALITY_GROUP.id
+    _metric: ColumnValueListMetric
     column_name: str
     values: Optional[list]
 
     def __init__(
         self,
         column_name: str,
         values: Optional[list] = None,
@@ -1163,28 +1179,32 @@
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        self.metric = ColumnValueListMetric(column_name=column_name, values=values)
+        self._metric = ColumnValueListMetric(column_name=column_name, values=values)
+
+    @property
+    def metric(self):
+        return self._metric
 
     def groups(self) -> Dict[str, str]:
         return {GroupingTypes.ByFeature.id: self.column_name}
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
         return TestValueCondition(eq=approx(0))
 
 
 class TestNumberOfOutListValues(BaseDataQualityValueListMetricsTest):
-    name = "Number Out-of-List Values"
-    alias = "number_value_list"
+    name: ClassVar = "Number Out-of-List Values"
+    alias: ClassVar = "number_value_list"
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.number_not_in_list
 
     def get_description(self, value: Numeric) -> str:
         return (
             f"The number of values out of list in the column **{self.column_name}** is {value}. "
@@ -1194,16 +1214,16 @@
 
 class ValueListParameters(CheckValueParameters):
     # todo: typing
     values: Optional[List[Any]] = None
 
 
 class TestShareOfOutListValues(BaseDataQualityValueListMetricsTest):
-    name = "Share of Out-of-List Values"
-    alias = "share_value_list"
+    name: ClassVar = "Share of Out-of-List Values"
+    alias: ClassVar = "share_value_list"
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.share_not_in_list
 
     def get_description(self, value: Numeric) -> str:
         metric_result = self.metric.get_result()
         number_not_in_range = metric_result.current.number_not_in_list
@@ -1211,15 +1231,15 @@
         return (
             f"The share of values out of list in the column **{self.column_name}** is {value:.3g} "
             f"({number_not_in_range} out of {rows_count}). "
             f"The test threshold is {self.get_condition()}."
         )
 
     def get_parameters(self) -> CheckValueParameters:
-        return ValueListParameters(condition=self.get_condition(), value=self.value, values=self.values)
+        return ValueListParameters(condition=self.get_condition(), value=self._value, values=self.values)
 
 
 class TestCatColumnsOutOfListValues(BaseGenerator):
     """Create share of out of list values tests for category columns"""
 
     columns: Optional[List[str]]
 
@@ -1233,18 +1253,18 @@
         else:
             columns = [column for column in self.columns if column in columns_info.cat_feature_names]
 
         return [TestShareOfOutListValues(column_name=name) for name in columns]
 
 
 class TestColumnQuantile(BaseCheckValueTest):
-    group = DATA_QUALITY_GROUP.id
-    name = "Quantile Value"
-    metric: ColumnQuantileMetric
-    column: ColumnName
+    group: ClassVar = DATA_QUALITY_GROUP.id
+    name: ClassVar = "Quantile Value"
+    _metric: ColumnQuantileMetric
+    column_name: ColumnName
     quantile: float
 
     def __init__(
         self,
         column_name: Union[str, ColumnName],
         quantile: float,
         eq: Optional[Numeric] = None,
@@ -1252,33 +1272,34 @@
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
     ):
-        if isinstance(column_name, str):
-            self.column = ColumnName.main_dataset(column_name)
-        else:
-            self.column = column_name
+        self.column_name = ColumnName.from_any(column_name)
         self.quantile = quantile
         super().__init__(
             eq=eq,
             gt=gt,
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        self.metric = ColumnQuantileMetric(column_name=column_name, quantile=quantile)
+        self._metric = ColumnQuantileMetric(column_name=column_name, quantile=quantile)
+
+    @property
+    def metric(self):
+        return self._metric
 
     def groups(self) -> Dict[str, str]:
-        return {GroupingTypes.ByFeature.id: self.column.display_name}
+        return {GroupingTypes.ByFeature.id: self.column_name.display_name}
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
 
         reference = self.metric.get_result().reference
 
@@ -1288,15 +1309,15 @@
         raise ValueError("Neither required test parameters nor reference data has been provided.")
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.value
 
     def get_description(self, value: Numeric) -> str:
         return (
-            f"The {self.quantile} quantile value of the column **{self.column}** is {value:.3g}. "
+            f"The {self.quantile} quantile value of the column **{self.column_name}** is {value:.3g}. "
             f"The test threshold is {self.get_condition()}."
         )
 
 
 @default_renderer(wrap_type=TestColumnQuantile)
 class TestColumnQuantileRenderer(TestRenderer):
     def render_html(self, obj: TestColumnQuantile) -> TestHtmlInfo:
```

### Comparing `evidently-0.3.2.1/src/evidently/tests/regression_performance_tests.py` & `evidently-0.3.3/src/evidently/tests/regression_performance_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC
+from typing import ClassVar
 from typing import List
 from typing import Optional
 from typing import Union
 
 from evidently.metrics import RegressionDummyMetric
 from evidently.metrics import RegressionQualityMetric
 from evidently.metrics.regression_performance.visualization import regression_perf_plot
@@ -21,17 +22,17 @@
 from evidently.utils.types import Numeric
 
 REGRESSION_GROUP = GroupData("regression", "Regression", "")
 GroupingTypes.TestGroup.add_value(REGRESSION_GROUP)
 
 
 class BaseRegressionPerformanceMetricsTest(BaseCheckValueTest, ABC):
-    group = REGRESSION_GROUP.id
-    metric: RegressionQualityMetric
-    dummy_metric: RegressionDummyMetric
+    group: ClassVar = REGRESSION_GROUP.id
+    _metric: RegressionQualityMetric
+    _dummy_metric: RegressionDummyMetric
 
     def __init__(
         self,
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
@@ -46,20 +47,28 @@
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        self.metric = RegressionQualityMetric()
-        self.dummy_metric = RegressionDummyMetric()
+        self._metric = RegressionQualityMetric()
+        self._dummy_metric = RegressionDummyMetric()
+
+    @property
+    def metric(self):
+        return self._metric
+
+    @property
+    def dummy_metric(self):
+        return self._dummy_metric
 
 
 class TestValueMAE(BaseRegressionPerformanceMetricsTest):
-    name = "Mean Absolute Error (MAE)"
+    name: ClassVar = "Mean Absolute Error (MAE)"
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
         metric_result = self.metric.get_result()
         ref_mae = metric_result.reference.mean_abs_error if metric_result.reference is not None else None
         if ref_mae is not None:
@@ -87,15 +96,15 @@
             color_options=self.color_options,
         )
         info.with_details("MAE", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestValueMAPE(BaseRegressionPerformanceMetricsTest):
-    name = "Mean Absolute Percentage Error (MAPE)"
+    name: ClassVar = "Mean Absolute Percentage Error (MAPE)"
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
         metric_result = self.metric.get_result()
         ref_mae = metric_result.reference.mean_abs_perc_error if metric_result.reference is not None else None
         if ref_mae is not None:
@@ -125,15 +134,15 @@
             color_options=self.color_options,
         )
         info.with_details("MAPE", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestValueRMSE(BaseRegressionPerformanceMetricsTest):
-    name = "Root Mean Square Error (RMSE)"
+    name: ClassVar = "Root Mean Square Error (RMSE)"
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
         metric_result = self.metric.get_result()
         rmse_ref = metric_result.reference.rmse if metric_result.reference is not None else None
         if rmse_ref is not None:
@@ -161,15 +170,15 @@
             color_options=self.color_options,
         )
         info.with_details("RMSE", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestValueMeanError(BaseRegressionPerformanceMetricsTest):
-    name = "Mean Error (ME)"
+    name: ClassVar = "Mean Error (ME)"
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
         return TestValueCondition(eq=approx(0, absolute=0.1 * self.metric.get_result().me_default_sigma))
 
     def calculate_value_for_test(self) -> Numeric:
@@ -192,15 +201,15 @@
         fig = plot_check(fig, obj.get_condition(), color_options=self.color_options)
         fig = plot_metric_value(fig, metric_result.current.mean_error, "current mean error")
         info.with_details("", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestValueAbsMaxError(BaseRegressionPerformanceMetricsTest):
-    name = "Max Absolute Error"
+    name: ClassVar = "Max Absolute Error"
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
         metric_result = self.metric.get_result()
         abs_error_max_ref = metric_result.reference.abs_error_max if metric_result.reference is not None else None
         if abs_error_max_ref is not None:
@@ -224,15 +233,15 @@
 
         fig = plot_distr(hist_curr=hist_curr, hist_ref=hist_ref, color_options=self.color_options)
         info.with_details("", plotly_figure(title="", figure=fig))
         return info
 
 
 class TestValueR2Score(BaseRegressionPerformanceMetricsTest):
-    name = "R2 Score"
+    name: ClassVar = "R2 Score"
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
         result = self.metric.get_result()
         r2_score_ref = result.reference.r2_score if result.reference is not None else None
         if r2_score_ref is not None:
```

### Comparing `evidently-0.3.2.1/src/evidently/tests/utils.py` & `evidently-0.3.3/src/evidently/tests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import numpy as np
 import pandas as pd
 import plotly.graph_objs as go
@@ -60,28 +59,28 @@
     if left_line and right_line:
         fig.add_vrect(x0=left_line, x1=right_line, fillcolor="green", opacity=0.25, line_width=0)
 
     if condition.eq is not None and isinstance(condition.eq, ApproxValue):
         left_border = 0.0
         right_border = 0.0
 
-        if condition.eq._relative > 1e-6:
-            left_border = condition.eq.value - condition.eq.value * condition.eq._relative
-            right_border = condition.eq.value + condition.eq.value * condition.eq._relative
+        if condition.eq.relative > 1e-6:
+            left_border = condition.eq.value - condition.eq.value * condition.eq.relative
+            right_border = condition.eq.value + condition.eq.value * condition.eq.relative
             fig.add_vrect(
                 x0=left_border,
                 x1=right_border,
                 fillcolor="green",
                 opacity=0.25,
                 line_width=0,
             )
 
-        elif condition.eq._absolute > 1e-12:
-            left_border = condition.eq.value - condition.eq._absolute
-            right_border = condition.eq.value + condition.eq._absolute
+        elif condition.eq.absolute > 1e-12:
+            left_border = condition.eq.value - condition.eq.absolute
+            right_border = condition.eq.value + condition.eq.absolute
             fig.add_vrect(
                 x0=left_border,
                 x1=right_border,
                 fillcolor="green",
                 opacity=0.25,
                 line_width=0,
             )
```

### Comparing `evidently-0.3.2.1/src/evidently/utils/dashboard.py` & `evidently-0.3.3/src/evidently/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/utils/data_drift_utils.py` & `evidently-0.3.3/src/evidently/utils/data_drift_utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/utils/data_operations.py` & `evidently-0.3.3/src/evidently/utils/data_operations.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/utils/data_preprocessing.py` & `evidently-0.3.3/src/evidently/utils/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/utils/generators.py` & `evidently-0.3.3/src/evidently/utils/generators.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2.1/src/evidently/utils/numpy_encoder.py` & `evidently-0.3.3/src/evidently/utils/numpy_encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import datetime
 import json
-from enum import Enum
 
 import numpy as np
 import pandas as pd
 
 from evidently.utils.types import ApproxValue
 
 _TYPES_MAPPING = (
@@ -15,16 +14,18 @@
     ((np.float_, np.float16, np.float32, np.float64), float),
     ((np.ndarray,), lambda obj: obj.tolist()),
     ((np.bool_), bool),
     ((pd.Timedelta,), str),
     ((np.void, type(pd.NaT)), lambda obj: None),  # should be before datetime as NaT is subclass of datetime.
     ((pd.Timestamp, datetime.datetime, datetime.date), lambda obj: obj.isoformat()),
     # map ApproxValue to json value
-    ((ApproxValue,), lambda obj: obj.as_dict()),
+    ((ApproxValue,), lambda obj: obj.dict()),
     ((pd.Series, pd.Index, pd.Categorical), lambda obj: obj.tolist()),
+    ((pd.DataFrame,), lambda obj: obj.to_dict()),
+    ((frozenset,), lambda obj: list(obj)),
 )
 
 
 class NumpyEncoder(json.JSONEncoder):
     """Numpy and Pandas data types to JSON types encoder"""
 
     def default(self, o):
```

### Comparing `evidently-0.3.2.1/src/evidently/utils/visualizations.py` & `evidently-0.3.3/src/evidently/utils/visualizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Dict
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
-from pandas import IntervalIndex
+from pandas.api.types import is_datetime64_any_dtype
 from plotly import graph_objs as go
 from plotly.subplots import make_subplots
 from scipy import stats
 from scipy.linalg.basic import LinAlgError
 
 from evidently.metric_results import ContourData
 from evidently.metric_results import Distribution
@@ -584,24 +584,24 @@
                 showlegend=False,
             )
             fig.add_trace(trace, 1, 2)
 
     # Add zero trace
     trace = go.Scatter(
         x=curr[x_name],
-        y=[0] * curr[x_name].shape[0],
+        y=[0] * len(curr[x_name]),
         mode="lines",
         marker_color=color_options.zero_line_color,
         showlegend=False,
     )
     fig.add_trace(trace, 1, 1)
     if ref is not None:
         trace = go.Scatter(
             x=ref[x_name],
-            y=[0] * ref[x_name].shape[0],
+            y=[0] * len(ref[x_name]),
             mode="lines",
             marker_color=color_options.zero_line_color,
             showlegend=False,
         )
         fig.add_trace(trace, 1, 2)
         fig.update_xaxes(title_text=xaxis_name, row=1, col=2)
 
@@ -638,15 +638,15 @@
         name=y_name,
         legendgroup=y_name,
     )
     fig.add_trace(trace, 1, 1)
     # Add zero trace
     trace = go.Scatter(
         x=curr[x_name],
-        y=[0] * curr[x_name].shape[0],
+        y=[0] * len(curr[x_name]),
         mode="lines",
         marker_color=color_options.zero_line_color,
         showlegend=False,
     )
     fig.add_trace(trace, 1, 1)
 
     if ref is not None:
@@ -659,15 +659,15 @@
             legendgroup=y_name,
             showlegend=False,
         )
         fig.add_trace(trace, 1, 2)
         # Add zero trace
         trace = go.Scatter(
             x=ref[x_name],
-            y=[0] * ref[x_name].shape[0],
+            y=[0] * len(ref[x_name]),
             mode="lines",
             marker_color=color_options.zero_line_color,
             showlegend=False,
         )
         fig.add_trace(trace, 1, 2)
         fig.update_xaxes(title_text=xaxis_name, row=1, col=2)
     fig.update_xaxes(title_text=xaxis_name, row=1, col=1)
@@ -774,15 +774,15 @@
 
 
 def is_possible_contour(m1, m2) -> bool:
     try:
         values = np.vstack([m1, m2])
         stats.gaussian_kde(values)
         return True
-    except LinAlgError:
+    except (LinAlgError, ValueError):
         return False
 
 
 def get_gaussian_kde(m1, m2):
     xmin = m1.min()
     xmax = m1.max()
     ymin = m2.min()
@@ -970,24 +970,30 @@
     df: pd.DataFrame,
     column_name: str,
     datetime_name: Optional[str],
     prefix: Optional[str] = None,
     freq: Optional[str] = None,
     bins: Optional[np.ndarray] = None,
 ) -> Tuple[pd.DataFrame, Optional[str]]:
+    index_name = df.index.name
+    if index_name is None:
+        index_name = "index"
+    if datetime_name is None and is_datetime64_any_dtype(df.index):
+        df = df.copy().reset_index()
+        datetime_name = index_name
     if datetime_name is not None:
         if prefix is None and freq is None:
             prefix, freq = choose_agg_period(df[datetime_name], None)
         plot_df = df.copy()
         plot_df["per"] = plot_df[datetime_name].dt.to_period(freq=freq)
         plot_df = plot_df.groupby("per")[column_name].agg(["mean", "std"]).reset_index()
         plot_df["per"] = plot_df["per"].dt.to_timestamp()
         return plot_df, prefix
     plot_df = df[column_name].reset_index().sort_values("index")
-    plot_df["per"] = pd.cut(plot_df["index"], OPTIMAL_POINTS if bins is None else bins, labels=False)
+    plot_df["per"] = pd.cut(plot_df[index_name], OPTIMAL_POINTS if bins is None else bins, labels=False)
     plot_df = plot_df.groupby("per")[column_name].agg(["mean", "std"]).reset_index()
     return plot_df, None
 
 
 def get_traces(df, color, error_band_opacity, name, showlegend):
     error_band_trace = go.Scatter(
         x=list(df["per"]) + list(df["per"][::-1]),  # x, then x reversed
@@ -1071,17 +1077,17 @@
     curr_data: Dict,
     ref_data: Optional[Dict],
     line: Optional[float],
     std: Optional[float],
     xaxis_name: str,
     xaxis_name_ref: Optional[str],
     yaxis_name: str,
+    color_options: ColorOptions,
     return_json: bool = True,
 ):
-    color_options = ColorOptions()
     cols = 1
     subplot_titles: Union[list, str] = ""
 
     if ref_data is not None:
         cols = 2
         subplot_titles = ["current", "reference"]
```

